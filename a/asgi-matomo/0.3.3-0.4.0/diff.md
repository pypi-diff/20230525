# Comparing `tmp/asgi_matomo-0.3.3.tar.gz` & `tmp/asgi_matomo-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgi_matomo-0.3.3.tar", max compression
+gzip compressed data, was "asgi_matomo-0.4.0.tar", max compression
```

## Comparing `asgi_matomo-0.3.3.tar` & `asgi_matomo-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-05-24 11:54:16.478030 asgi_matomo-0.3.3/LICENSE
--rw-r--r--   0        0        0     5278 2023-05-24 11:54:16.478030 asgi_matomo-0.3.3/README.md
--rw-r--r--   0        0        0      186 2023-05-24 11:54:16.478030 asgi_matomo-0.3.3/asgi_matomo/__init__.py
--rw-r--r--   0        0        0     9799 2023-05-24 11:54:16.478030 asgi_matomo-0.3.3/asgi_matomo/middleware.py
--rw-r--r--   0        0        0        0 2023-05-24 11:54:16.478030 asgi_matomo-0.3.3/asgi_matomo/py.typed
--rw-r--r--   0        0        0     1024 2023-05-24 11:54:16.478030 asgi_matomo-0.3.3/asgi_matomo/trackers.py
--rw-r--r--   0        0        0      879 2023-05-24 11:54:16.478030 asgi_matomo-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     6163 1970-01-01 00:00:00.000000 asgi_matomo-0.3.3/setup.py
--rw-r--r--   0        0        0     6011 1970-01-01 00:00:00.000000 asgi_matomo-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-25 18:35:48.385600 asgi_matomo-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5574 2023-05-25 18:35:48.385600 asgi_matomo-0.4.0/README.md
+-rw-r--r--   0        0        0      186 2023-05-25 18:35:48.385600 asgi_matomo-0.4.0/asgi_matomo/__init__.py
+-rw-r--r--   0        0        0    13164 2023-05-25 18:35:48.385600 asgi_matomo-0.4.0/asgi_matomo/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-25 18:35:48.385600 asgi_matomo-0.4.0/asgi_matomo/py.typed
+-rw-r--r--   0        0        0     1024 2023-05-25 18:35:48.385600 asgi_matomo-0.4.0/asgi_matomo/trackers.py
+-rw-r--r--   0        0        0     1072 2023-05-25 18:35:48.389600 asgi_matomo-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6463 1970-01-01 00:00:00.000000 asgi_matomo-0.4.0/setup.py
+-rw-r--r--   0        0        0     6307 1970-01-01 00:00:00.000000 asgi_matomo-0.4.0/PKG-INFO
```

### Comparing `asgi_matomo-0.3.3/LICENSE` & `asgi_matomo-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asgi_matomo-0.3.3/README.md` & `asgi_matomo-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 ```python
 from fastapi import FastAPI
 from asgi_matomo import MatomoMiddleware
 
 app = FastAPI()
 app.add_middleware(
-  BrotliMiddleware,
+  MatomoMiddleware,
   matomo_url="YOUR MATOMO TRACKING URL",
   idsite=12345, # your service tracking id
 )
 
 @app.get("/")
 def home() -> dict:
     return {"data": "a" * 4000}
@@ -161,14 +161,18 @@
 
 This project keeps a [changelog](https://github.com/spraakbanken/asgi-matomo/CHANGELOG.md).
 
 # Releas Notes
 
 ## Latest Changes
 
+## [0.4.0] - 2023-05-25
+
+* Handle lifespan correctly. PR [#13](https://github.com/spraakbanken/asgi-matomo/pull/13) by [@kod-kristoff](https://github.com/kod-kristoff).
+* add docs. PR [#11](https://github.com/spraakbanken/asgi-matomo/pull/11) by [@kod-kristoff](https://github.com/kod-kristoff).
 ## [0.3.2] - 2023-05-23
 
 * feat: add PerfMsTracker. PR [#10](https://github.com/spraakbanken/asgi-matomo/pull/10) by [@kod-kristoff](https://github.com/kod-kristoff).
 
 ## [0.3.0] - 2023-05-22
 ### Added
```

### Comparing `asgi_matomo-0.3.3/asgi_matomo/middleware.py` & `asgi_matomo-0.4.0/asgi_matomo/middleware.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 import logging
 import random
 import re
 import time
 import traceback
 import typing
 import urllib.parse
-from typing import Any
+from contextlib import AsyncExitStack, asynccontextmanager
+from typing import Any, AsyncIterator
 
 import httpx
 from asgiref.typing import (
     ASGI3Application,
     ASGIReceiveCallable,
+    ASGIReceiveEvent,
     ASGISendCallable,
+    ASGISendEvent,
     HTTPScope,
 )
 
 logger = logging.getLogger(__name__)
 
 
 _T = typing.TypeVar("_T")
@@ -62,49 +65,113 @@
             re.compile(pattern) for pattern in (exclude_patterns or [])
         ]
         self.route_details = route_details or {}
 
     async def startup(self) -> None:
         if self.client is None:
             self.client = httpx.AsyncClient()
+        print("middleware startup: done")
 
     async def shutdown(self) -> None:
         if self.client is not None:
             await self.client.aclose()
+        print("middleware shutdown: done")
 
     async def lifespan(
         self, scope: HTTPScope, receive: ASGIReceiveCallable, send: ASGISendCallable
     ) -> None:
         """
         Handle ASGI lifespan messages, which allows us to manage application
         startup and shutdown events.
+
+        Code borrowed from: https://github.com/adriangb/asgi-lifespan
         """
-        started = False
-        app: typing.Any = scope.get("app")
-        await receive()
-        try:
-            async with self.lifespan_context(app) as maybe_state:
-                if maybe_state is not None:
-                    if "state" not in scope:
-                        raise RuntimeError(
-                            'The server does not support "state" in the lifespan scope.'
-                        )
-                    scope["state"].update(maybe_state)  # type: ignore
+        rcv_events: dict[str, bool] = {}
+        send_events: dict[str, bool] = {}
+
+        async def wrapped_rcv() -> ASGIReceiveEvent:
+            message = await receive()
+            rcv_events[message["type"]] = True
+            return message
+
+        async def wrapped_send(message: ASGISendEvent) -> None:
+            send_events[message["type"]] = True
+            if message["type"] == "lifespan.shutdown.complete":
+                # we want to send this one ourselves
+                # once we are done
+                return
+            await send(message)
+
+        @asynccontextmanager
+        async def cleanup() -> "AsyncIterator[None]":
+            try:
+                yield
+            except BaseException:
+                exc_text = traceback.format_exc()
+                if "lifespan.startup.complete" in send_events:
+                    await send(
+                        {"type": "lifespan.shutdown.failed", "message": exc_text}
+                    )
+                else:
+                    await send({"type": "lifespan.startup.failed", "message": exc_text})
+                raise
+            else:
+                await send({"type": "lifespan.shutdown.complete"})
+
+        lifespan_cm = self.lifespan_context(self.app)
+
+        async with AsyncExitStack() as stack:
+            await stack.enter_async_context(cleanup())
+            await stack.enter_async_context(lifespan_cm)
+            try:
+                # one of 4 things will happen when we call the app:
+                # 1. it supports lifespans. it will block until the server
+                #    sends the shutdown signal, at which point we get control
+                #    back and can run our own teardown
+                # 2. it does nothing and returns. in this case we do the
+                #    back and forth with the ASGI server ourselves
+                # 3. it raises an exception.
+                #    a. before raising the exception it sent a
+                #       "lifespan.startup.failed" message
+                #       this means it supports lifespans, but it's lifespan
+                #       errored out. we'll re-raise to trigger our teardown
+                #    b. it did not send a "lifespan.startup.failed" message
+                #       this app doesn't support lifespans, the spec says
+                #       to just swallow the exception and proceed
+                # 4. it supports lifespan events and it's lifespan fails
+                #    (it sends a "lifespan.startup.failed" message)
+                #    in this case we'll run our teardown and then return
+                await self.app(scope, wrapped_rcv, wrapped_send)
+            except BaseException:  # noqa: BLE001
+                if (
+                    "lifespan.startup.failed" in send_events
+                    or "lifespan.shutdown.failed" in send_events
+                ):
+                    # the app tried to start and failed
+                    # this app re-raises the exceptions (Starlette does this)
+                    # re-raise so that our teardown is triggered
+                    raise
+                # the app doesn't support lifespans
+                # the spec says to ignore these errors and just don't send
+                # more lifespan events
+            if "lifespan.startup.failed" in send_events:
+                # the app supports lifespan events
+                # but it failed to start
+                # this app does not re-raise exceptions
+                # so all we can do is run our teardown and exit
+                return
+            if "lifespan.startup.complete" not in send_events:
+                # the app doesn't support lifespans at all
+                # so we'll have to talk to the ASGI server ourselves
+                await receive()
                 await send({"type": "lifespan.startup.complete"})
-                started = True
+                # we'll block here until the ASGI server shuts us down
                 await receive()
-        except BaseException:
-            exc_text = traceback.format_exc()
-            if started:
-                await send({"type": "lifespan.shutdown.failed", "message": exc_text})
-            else:
-                await send({"type": "lifespan.startup.failed", "message": exc_text})
-            raise
-        else:
-            await send({"type": "lifespan.shutdown.complete"})
+        # even if the app sent this, we intercepted it and discarded it until we were done
+        # await send({"type": "lifespan.shutdown.complete"})
 
     async def __call__(
         self, scope: HTTPScope, receive: ASGIReceiveCallable, send: ASGISendCallable
     ) -> Any:
         # locals inside the app function (send_wrapper) can't be assigned to,
         # as the interpreter detects the assignment and thus creates a new
         # local variable within that function, with that name.
```

### Comparing `asgi_matomo-0.3.3/asgi_matomo/trackers.py` & `asgi_matomo-0.4.0/asgi_matomo/trackers.py`

 * *Files identical despite different names*

### Comparing `asgi_matomo-0.3.3/pyproject.toml` & `asgi_matomo-0.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asgi-matomo"
-version = "0.3.3"
+version = "0.4.0"
 description = "Middleware for tracking ASGI reqeusts with Matomo"
 authors = ["Kristoffer Andersson <kristoffer.andersson@gu.se>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://spraakbanken.gu.se"
 repository = "https://github.com/spraakbanken/asgi-matomo"
 packages = [{include = "asgi_matomo"}]
@@ -27,10 +27,19 @@
 pytest-cov = "^4.0.0"
 bump2version = "^1.0.1"
 
 [tool.poetry.group.ci.dependencies]
 ruff = "0.0.263"
 
 
+
+[tool.poetry.group.docs.dependencies]
+mike = "^1.1.2"
+mkdocs = "^1.4.3"
+mkdocs-material = "<9.0.0"
+mdx-include = "<2.0.0"
+markdown = "<3.4"
+mkdocs-markdownextradata-plugin = ">=0.1.7,<0.3.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `asgi_matomo-0.3.3/setup.py` & `asgi_matomo-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['asgiref>=3.6.0,<4.0.0', 'httpx>=0.24.0,<0.25.0']
 
 setup_kwargs = {
     'name': 'asgi-matomo',
-    'version': '0.3.3',
+    'version': '0.4.0',
     'description': 'Middleware for tracking ASGI reqeusts with Matomo',
-    'long_description': '# asgi-matomo\n[![Packaging status](https://img.shields.io/pypi/v/asgi-matomo?color=%2334D058&label=pypi%20package)](https://pypi.org/project/asgi-matomo)\n[![CI](https://github.com/spraakbanken/asgi-matomo/workflows/CI/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACI)\n[![codecov](https://codecov.io/gh/spraakbanken/asgi-matomo/branch/main/graph/badge.svg?token=MRJZVCJQF5)](https://codecov.io/gh/spraakbanken/asgi-matomo)\n\nTracking requests with Matomo from ASGI apps.\n\n`MatomoMiddleware` adds tracking of all requests to Matomo to ASGI applications (Starlette, FastAPI, Quart, etc.). The intended usage is for api tracking (backends).\n\n**Note** If you serve HTML (directly or by templates), it is suggested to track those parts through Matomo\'s javascript tracking.\n\n**Installation**\n\n```bash\npip install asgi-matomo\n```\n\n## What is tracked\n\nCurrently this middleware tracks:\n- `url`\n- `ua`: user_agent\n- `gt_ms`: mesaured as the time before and after this middleware call next in the asgi stack.\n- `send_image=0` for performance issues\n- `cvar` with at least `http_status_code` and `http_method` set.\n- `lang` if `accept-lang` is set\n- `cip` client ip, **requires** `access_token` to be given.\n- `action_name` that defaults to path, but can be specified.\n\nYou can also pass variable to track by adding an `asgi_matomo`  dict in the `state` dict of the ASGI `scope`:\n```python\nscope = {\n  "state": {\n    "asgi_matomo": {\n      "e_a": "Playing",\n      "cvar": {\n        "your": "custom",\n        "data": "here",\n      }\n    }\n  }\n}\n```\n\nThe keys of the `asgi_matomo` dict is expected to be valid parameter for the [Matomo HTTP Tracking API](https://developer.matomo.org/api-reference/tracking-api). `cvar` is serialized with the standard `json` lib.\n\nYou can also track time spent on different tasks with `trackers.PerfMsTracker`.\n```python\nimport asyncio\nfrom starlette.applications import Starlette\nfrom starlette.responses import JSONResponse\nfrom starlette.routing import Route\nfrom starlette.middleware import Middleware\n\nfrom asgi_matomo import MatomoMiddleware\nfrom asgi_matomo.trackers import PerfMsTracker\n\nasync def homepage(request):\n    async with PerfMsTracker(scope=request.scope, key="pf_srv"):\n        # fetch/compute data\n        await asyncio.sleep(1)\n        data = {"data": "a"*4000}\n    return JSONResponse(data)\n\napp = Starlette(\n  routes=[Route("/", homepage)],\n  middleware=[\n    Middleware(\n      MatomoMiddleware,\n      matomo_url="YOUR MATOMO TRACKING URL",\n      idsite=12345, # your service tracking id\n  )],\n)\n```\n\n## Examples\n\n### Starlette\n\n```python\nfrom starlette.applications import Starlette\nfrom starlette.responses import JSONResponse\nfrom starlette.routing import Route\nfrom starlette.middleware import Middleware\n\nfrom asgi_matomo import MatomoMiddleware\n\nasync def homepage(request):\n    return JSONResponse({"data": "a" * 4000})\n\napp = Starlette(\n  routes=[Route("/", homepage)],\n  middleware=[\n    Middleware(\n      MatomoMiddleware,\n      matomo_url="YOUR MATOMO TRACKING URL",\n      idsite=12345, # your service tracking id\n  )],\n)\n```\n\n### FastAPI\n\n```python\nfrom fastapi import FastAPI\nfrom asgi_matomo import MatomoMiddleware\n\napp = FastAPI()\napp.add_middleware(\n  BrotliMiddleware,\n  matomo_url="YOUR MATOMO TRACKING URL",\n  idsite=12345, # your service tracking id\n)\n\n@app.get("/")\ndef home() -> dict:\n    return {"data": "a" * 4000}\n```\n\n## API Reference\n\n**Overview**\n\n```python\napp.add_middleware(\n  MatomoMiddleware,\n  matomo_url="YOUR MATOMO TRACKING URL",\n  idsite=12345, # your service tracking id\n  access_token="SECRETTOKEN",\n  assume_https=True,\n  exclude_paths=["/health"],\n  exclude_patterns=[".*/old.*"],\n  route_details={\n    "route": {\n      "action_name": "Name",\n    }\n  }\n)\n```\n\n**Parameters**:\n\n- **(Required)** `matomo_url`: The URL to make your tracking calls to.\n- **(Required)** `idsite`: The tracking id for your service.\n- _(Optional)_ `access_token`: Access token for Matomo. If this is set `cip` is also tracked. Required for tracking some data.\n- _(Optional)_ `assume_https`: If `True`, set tracked url scheme to `https`, useful when running behind a proxy. Defaults to `True`.\n- _(Optional)_ `exclude_paths`: A list of paths to exclude, only excludes path that is equal to a path in this list. These are tried before `exclude_patterns`. Defaults to `None`.\n- _(Optional)_ `exclude_patterns`: A list of regex patterns that are compiled, and then exclude a path from tracking if any pattern match. Defaults to `None`.\nThese are tried after `exclude_paths`.\n- _(Optional)_ `route_details`: A dict with custom route-specific tracking data. Defaults to `None`.\n\n\n**Notes**:\n\n- Currently only some parts [Matomo Tracking HTTP API](https://developer.matomo.org/api-reference/tracking-api) is supported.\n\n## Ideas for further work:\n- [x] _filtering tracked of urls_\n- [x] _custom extraction of tracked data_\n\n\nThis project keeps a [changelog](https://github.com/spraakbanken/asgi-matomo/CHANGELOG.md).\n\n# Releas Notes\n\n## Latest Changes\n\n## [0.3.2] - 2023-05-23\n\n* feat: add PerfMsTracker. PR [#10](https://github.com/spraakbanken/asgi-matomo/pull/10) by [@kod-kristoff](https://github.com/kod-kristoff).\n\n## [0.3.0] - 2023-05-22\n### Added\n\n- Allow setting route-details\n\n',
+    'long_description': '# asgi-matomo\n[![Packaging status](https://img.shields.io/pypi/v/asgi-matomo?color=%2334D058&label=pypi%20package)](https://pypi.org/project/asgi-matomo)\n[![CI](https://github.com/spraakbanken/asgi-matomo/workflows/CI/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACI)\n[![codecov](https://codecov.io/gh/spraakbanken/asgi-matomo/branch/main/graph/badge.svg?token=MRJZVCJQF5)](https://codecov.io/gh/spraakbanken/asgi-matomo)\n\nTracking requests with Matomo from ASGI apps.\n\n`MatomoMiddleware` adds tracking of all requests to Matomo to ASGI applications (Starlette, FastAPI, Quart, etc.). The intended usage is for api tracking (backends).\n\n**Note** If you serve HTML (directly or by templates), it is suggested to track those parts through Matomo\'s javascript tracking.\n\n**Installation**\n\n```bash\npip install asgi-matomo\n```\n\n## What is tracked\n\nCurrently this middleware tracks:\n- `url`\n- `ua`: user_agent\n- `gt_ms`: mesaured as the time before and after this middleware call next in the asgi stack.\n- `send_image=0` for performance issues\n- `cvar` with at least `http_status_code` and `http_method` set.\n- `lang` if `accept-lang` is set\n- `cip` client ip, **requires** `access_token` to be given.\n- `action_name` that defaults to path, but can be specified.\n\nYou can also pass variable to track by adding an `asgi_matomo`  dict in the `state` dict of the ASGI `scope`:\n```python\nscope = {\n  "state": {\n    "asgi_matomo": {\n      "e_a": "Playing",\n      "cvar": {\n        "your": "custom",\n        "data": "here",\n      }\n    }\n  }\n}\n```\n\nThe keys of the `asgi_matomo` dict is expected to be valid parameter for the [Matomo HTTP Tracking API](https://developer.matomo.org/api-reference/tracking-api). `cvar` is serialized with the standard `json` lib.\n\nYou can also track time spent on different tasks with `trackers.PerfMsTracker`.\n```python\nimport asyncio\nfrom starlette.applications import Starlette\nfrom starlette.responses import JSONResponse\nfrom starlette.routing import Route\nfrom starlette.middleware import Middleware\n\nfrom asgi_matomo import MatomoMiddleware\nfrom asgi_matomo.trackers import PerfMsTracker\n\nasync def homepage(request):\n    async with PerfMsTracker(scope=request.scope, key="pf_srv"):\n        # fetch/compute data\n        await asyncio.sleep(1)\n        data = {"data": "a"*4000}\n    return JSONResponse(data)\n\napp = Starlette(\n  routes=[Route("/", homepage)],\n  middleware=[\n    Middleware(\n      MatomoMiddleware,\n      matomo_url="YOUR MATOMO TRACKING URL",\n      idsite=12345, # your service tracking id\n  )],\n)\n```\n\n## Examples\n\n### Starlette\n\n```python\nfrom starlette.applications import Starlette\nfrom starlette.responses import JSONResponse\nfrom starlette.routing import Route\nfrom starlette.middleware import Middleware\n\nfrom asgi_matomo import MatomoMiddleware\n\nasync def homepage(request):\n    return JSONResponse({"data": "a" * 4000})\n\napp = Starlette(\n  routes=[Route("/", homepage)],\n  middleware=[\n    Middleware(\n      MatomoMiddleware,\n      matomo_url="YOUR MATOMO TRACKING URL",\n      idsite=12345, # your service tracking id\n  )],\n)\n```\n\n### FastAPI\n\n```python\nfrom fastapi import FastAPI\nfrom asgi_matomo import MatomoMiddleware\n\napp = FastAPI()\napp.add_middleware(\n  MatomoMiddleware,\n  matomo_url="YOUR MATOMO TRACKING URL",\n  idsite=12345, # your service tracking id\n)\n\n@app.get("/")\ndef home() -> dict:\n    return {"data": "a" * 4000}\n```\n\n## API Reference\n\n**Overview**\n\n```python\napp.add_middleware(\n  MatomoMiddleware,\n  matomo_url="YOUR MATOMO TRACKING URL",\n  idsite=12345, # your service tracking id\n  access_token="SECRETTOKEN",\n  assume_https=True,\n  exclude_paths=["/health"],\n  exclude_patterns=[".*/old.*"],\n  route_details={\n    "route": {\n      "action_name": "Name",\n    }\n  }\n)\n```\n\n**Parameters**:\n\n- **(Required)** `matomo_url`: The URL to make your tracking calls to.\n- **(Required)** `idsite`: The tracking id for your service.\n- _(Optional)_ `access_token`: Access token for Matomo. If this is set `cip` is also tracked. Required for tracking some data.\n- _(Optional)_ `assume_https`: If `True`, set tracked url scheme to `https`, useful when running behind a proxy. Defaults to `True`.\n- _(Optional)_ `exclude_paths`: A list of paths to exclude, only excludes path that is equal to a path in this list. These are tried before `exclude_patterns`. Defaults to `None`.\n- _(Optional)_ `exclude_patterns`: A list of regex patterns that are compiled, and then exclude a path from tracking if any pattern match. Defaults to `None`.\nThese are tried after `exclude_paths`.\n- _(Optional)_ `route_details`: A dict with custom route-specific tracking data. Defaults to `None`.\n\n\n**Notes**:\n\n- Currently only some parts [Matomo Tracking HTTP API](https://developer.matomo.org/api-reference/tracking-api) is supported.\n\n## Ideas for further work:\n- [x] _filtering tracked of urls_\n- [x] _custom extraction of tracked data_\n\n\nThis project keeps a [changelog](https://github.com/spraakbanken/asgi-matomo/CHANGELOG.md).\n\n# Releas Notes\n\n## Latest Changes\n\n## [0.4.0] - 2023-05-25\n\n* Handle lifespan correctly. PR [#13](https://github.com/spraakbanken/asgi-matomo/pull/13) by [@kod-kristoff](https://github.com/kod-kristoff).\n* add docs. PR [#11](https://github.com/spraakbanken/asgi-matomo/pull/11) by [@kod-kristoff](https://github.com/kod-kristoff).\n## [0.3.2] - 2023-05-23\n\n* feat: add PerfMsTracker. PR [#10](https://github.com/spraakbanken/asgi-matomo/pull/10) by [@kod-kristoff](https://github.com/kod-kristoff).\n\n## [0.3.0] - 2023-05-22\n### Added\n\n- Allow setting route-details\n\n',
     'author': 'Kristoffer Andersson',
     'author_email': 'kristoffer.andersson@gu.se',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://spraakbanken.gu.se',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `asgi_matomo-0.3.3/PKG-INFO` & `asgi_matomo-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgi-matomo
-Version: 0.3.3
+Version: 0.4.0
 Summary: Middleware for tracking ASGI reqeusts with Matomo
 Home-page: https://spraakbanken.gu.se
 License: MIT
 Author: Kristoffer Andersson
 Author-email: kristoffer.andersson@gu.se
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -122,15 +122,15 @@
 
 ```python
 from fastapi import FastAPI
 from asgi_matomo import MatomoMiddleware
 
 app = FastAPI()
 app.add_middleware(
-  BrotliMiddleware,
+  MatomoMiddleware,
   matomo_url="YOUR MATOMO TRACKING URL",
   idsite=12345, # your service tracking id
 )
 
 @app.get("/")
 def home() -> dict:
     return {"data": "a" * 4000}
@@ -180,14 +180,18 @@
 
 This project keeps a [changelog](https://github.com/spraakbanken/asgi-matomo/CHANGELOG.md).
 
 # Releas Notes
 
 ## Latest Changes
 
+## [0.4.0] - 2023-05-25
+
+* Handle lifespan correctly. PR [#13](https://github.com/spraakbanken/asgi-matomo/pull/13) by [@kod-kristoff](https://github.com/kod-kristoff).
+* add docs. PR [#11](https://github.com/spraakbanken/asgi-matomo/pull/11) by [@kod-kristoff](https://github.com/kod-kristoff).
 ## [0.3.2] - 2023-05-23
 
 * feat: add PerfMsTracker. PR [#10](https://github.com/spraakbanken/asgi-matomo/pull/10) by [@kod-kristoff](https://github.com/kod-kristoff).
 
 ## [0.3.0] - 2023-05-22
 ### Added
```

