# Comparing `tmp/bovine_herd-0.2.0.tar.gz` & `tmp/bovine_herd-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine_herd-0.2.0.tar", max compression
+gzip compressed data, was "bovine_herd-0.2.2.tar", max compression
```

## Comparing `bovine_herd-0.2.0.tar` & `bovine_herd-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1099 2023-05-22 14:17:04.642842 bovine_herd-0.2.0/README.md
--rw-r--r--   0        0        0     1802 2023-05-22 14:17:04.646842 bovine_herd-0.2.0/bovine_herd/__init__.py
--rw-r--r--   0        0        0      488 2023-05-22 14:17:04.646842 bovine_herd-0.2.0/bovine_herd/config.py
--rw-r--r--   0        0        0      345 2023-05-22 14:17:04.646842 bovine_herd-0.2.0/bovine_herd/server/__init__.py
--rw-r--r--   0        0        0      698 2023-05-22 14:17:04.646842 bovine_herd-0.2.0/bovine_herd/server/activitypub.py
--rw-r--r--   0        0        0     4923 2023-05-22 14:18:01.387066 bovine_herd-0.2.0/bovine_herd/server/endpoints.py
--rw-r--r--   0        0        0      832 2023-05-22 14:17:04.646842 bovine_herd-0.2.0/bovine_herd/server/info.py
--rw-r--r--   0        0        0     2039 2023-05-22 14:17:04.646842 bovine_herd-0.2.0/bovine_herd/server/wellknown.py
--rw-r--r--   0        0        0   154974 2023-05-22 14:17:04.646842 bovine_herd-0.2.0/bovine_herd/static/cow.jpg
--rw-r--r--   0        0        0   285585 2023-05-22 14:17:04.646842 bovine_herd-0.2.0/bovine_herd/static/moocow.png
--rw-r--r--   0        0        0   549258 2023-05-22 14:17:04.650842 bovine_herd-0.2.0/bovine_herd/static/profile.png
--rw-r--r--   0        0        0     1234 2023-05-22 14:17:04.650842 bovine_herd-0.2.0/bovine_herd/static/style.css
--rw-r--r--   0        0        0   362136 2023-05-22 14:17:04.654842 bovine_herd-0.2.0/bovine_herd/static/woodpecker.png
--rw-r--r--   0        0        0      961 2023-05-22 14:17:04.654842 bovine_herd-0.2.0/bovine_herd/templates/index.html
--rw-r--r--   0        0        0     1128 2023-05-22 14:17:04.654842 bovine_herd-0.2.0/bovine_herd/utils/__init__.py
--rw-r--r--   0        0        0     1084 2023-05-22 14:17:04.654842 bovine_herd-0.2.0/bovine_herd/utils/test/__init__.py
--rw-r--r--   0        0        0      274 2023-05-22 14:17:04.654842 bovine_herd-0.2.0/bovine_herd/utils/test_utils.py
--rw-r--r--   0        0        0       23 2023-05-22 14:17:04.654842 bovine_herd-0.2.0/bovine_herd/version.py
--rw-r--r--   0        0        0      924 2023-05-22 14:28:57.451393 bovine_herd-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2235 1970-01-01 00:00:00.000000 bovine_herd-0.2.0/setup.py
--rw-r--r--   0        0        0     1951 1970-01-01 00:00:00.000000 bovine_herd-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1345 2023-05-25 18:44:02.786690 bovine_herd-0.2.2/README.md
+-rw-r--r--   0        0        0     1763 2023-05-25 18:44:02.786690 bovine_herd-0.2.2/bovine_herd/__init__.py
+-rw-r--r--   0        0        0      488 2023-05-22 14:17:04.646842 bovine_herd-0.2.2/bovine_herd/config.py
+-rw-r--r--   0        0        0      345 2023-05-22 14:17:04.646842 bovine_herd-0.2.2/bovine_herd/server/__init__.py
+-rw-r--r--   0        0        0      698 2023-05-22 14:17:04.646842 bovine_herd-0.2.2/bovine_herd/server/activitypub.py
+-rw-r--r--   0        0        0     4986 2023-05-25 18:44:02.786690 bovine_herd-0.2.2/bovine_herd/server/endpoints.py
+-rw-r--r--   0        0        0      832 2023-05-22 14:17:04.646842 bovine_herd-0.2.2/bovine_herd/server/info.py
+-rw-r--r--   0        0        0     1993 2023-05-25 18:44:02.786690 bovine_herd-0.2.2/bovine_herd/server/wellknown.py
+-rw-r--r--   0        0        0   154974 2023-05-22 14:17:04.646842 bovine_herd-0.2.2/bovine_herd/static/cow.jpg
+-rw-r--r--   0        0        0   285585 2023-05-22 14:17:04.646842 bovine_herd-0.2.2/bovine_herd/static/moocow.png
+-rw-r--r--   0        0        0   549258 2023-05-22 14:17:04.650842 bovine_herd-0.2.2/bovine_herd/static/profile.png
+-rw-r--r--   0        0        0     1234 2023-05-22 14:17:04.650842 bovine_herd-0.2.2/bovine_herd/static/style.css
+-rw-r--r--   0        0        0   362136 2023-05-22 14:17:04.654842 bovine_herd-0.2.2/bovine_herd/static/woodpecker.png
+-rw-r--r--   0        0        0      961 2023-05-22 14:17:04.654842 bovine_herd-0.2.2/bovine_herd/templates/index.html
+-rw-r--r--   0        0        0     1128 2023-05-22 14:17:04.654842 bovine_herd-0.2.2/bovine_herd/utils/__init__.py
+-rw-r--r--   0        0        0     1084 2023-05-22 14:17:04.654842 bovine_herd-0.2.2/bovine_herd/utils/test/__init__.py
+-rw-r--r--   0        0        0      274 2023-05-22 14:17:04.654842 bovine_herd-0.2.2/bovine_herd/utils/test_utils.py
+-rw-r--r--   0        0        0       23 2023-05-22 14:17:04.654842 bovine_herd-0.2.2/bovine_herd/version.py
+-rw-r--r--   0        0        0      875 2023-05-25 18:44:02.802690 bovine_herd-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2383 1970-01-01 00:00:00.000000 bovine_herd-0.2.2/setup.py
+-rw-r--r--   0        0        0     2197 1970-01-01 00:00:00.000000 bovine_herd-0.2.2/PKG-INFO
```

### Comparing `bovine_herd-0.2.0/README.md` & `bovine_herd-0.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -21,19 +21,22 @@
 pip install bovine_tool
 python -mbovine_tool.register --domain $DOMAIN moocow
 ```
 
 you create a new account for __moocow__. This command returns its bovine name, which will be of the form `moocow + uuid4()`, e.g. `moocow_09c80006-483c-4826-b48c-cf5134b4e898`. By running:
 
 ```bash
-python -mbovine_tool.manage --new-did-key $BOVINE_NAME
+python -mbovine_tool.manage --new_did_key $BOVINE_NAME
 ```
 
 you will be given a secret (an Ed25519 private key, i.e. starts with `z3u2`). Once you have this secret, you can send a message via
 
 ```bash
 python -mbovine.msg --secret $SECRET --host $DOMAIN moooo
 ```
 
 ## Configuration
 
 The default database connection is "sqlite://bovine.sqlite3". This can be overwridden with the environment variable "BOVINE_DB_URL".
+
+- `BOVINE_REDIS` represents how to reach redis, e.g. `redis://localhost`. If not set, redis is not used. Redis is necessary when using more than one worker.
+- `BOVINE_LOGFILE` gives the path of the log file. When not present bovine.log is used.
```

### Comparing `bovine_herd-0.2.0/bovine_herd/__init__.py` & `bovine_herd-0.2.2/bovine_herd/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,36 +8,33 @@
 from quart_redis import RedisHandler
 from tortoise.contrib.quart import register_tortoise
 
 from .config import TORTOISE_ORM, configure_bovine_herd
 from .server import default_configuration
 from .server.endpoints import endpoints
 
-# from .version import __version__
-
 logfile = os.environ.get("BOVINE_LOGFILE", "bovine.log")
+redis_url = os.environ.get("BOVINE_REDIS")
 
 log_format = "[%(asctime)s] %(levelname)-8s %(name)-12s %(message)s"
 logging.basicConfig(
     level=logging.INFO,
     format=log_format,
     filename=(logfile),
 )
-domain = os.environ.get("DOMAIN", "my_domain")
-
 app = Quart(__name__, template_folder="templates", static_folder="static")
-app.config.update(
-    {
-        "REDIS_URI": "redis://localhost",
-        "DOMAIN": domain,
-    }
-)
 
 
-RedisHandler(app)
+if redis_url:
+    app.config.update(
+        {
+            "REDIS_URI": redis_url,
+        }
+    )
+    RedisHandler(app)
 
 
 @app.before_serving
 async def startup():
     await configure_bovine_herd(app)
     await configure_bovine_store(app)
     await configure_bovine_pub_sub(app)
```

### Comparing `bovine_herd-0.2.0/bovine_herd/server/activitypub.py` & `bovine_herd-0.2.2/bovine_herd/server/activitypub.py`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.0/bovine_herd/server/endpoints.py` & `bovine_herd-0.2.2/bovine_herd/server/endpoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 from quart import Blueprint, current_app, g, make_response, request
 
 logger = logging.getLogger(__name__)
 
 endpoints = Blueprint("endpoint", __name__)
 endpoints.before_request(add_authorization)
 
-actor_cache = {}
-
 
 @endpoints.get("/<identifier>")
 async def endpoints_get(identifier):
     endpoint_path = path_from_request(request)
     object_store = current_app.config["bovine_store"]
 
     endpoint_type, actor = await object_store.resolve_endpoint(endpoint_path)
@@ -46,19 +44,16 @@
                 200,
                 {"content-type": "application/activity+json"},
             )
 
         if g.retriever is None or g.retriever == "NONE":
             return {"status": "unauthorized"}, 401
 
-        to_cache = actor.actor_object.build(visibility=Visibility.PUBLIC)
-        actor_cache[endpoint_path] = to_cache
-
         return (
-            to_cache,
+            actor.actor_object.build(visibility=Visibility.PUBLIC),
             200,
             {"content-type": "application/activity+json"},
         )
 
     if endpoint_type == EndpointType.EVENT_SOURCE:
         actor = actor.actor_object.build(visibility=Visibility.OWNER)
         if g.retriever != actor["id"]:
@@ -103,24 +98,28 @@
         return {"status": "created"}, 201, {"location": item.meta["object_location"]}
 
     if endpoint_type == EndpointType.PROXY_URL:
         return await proxy_url_response(actor)
 
 
 async def proxy_url_response(actor):
-    await request.get_data(parse_form_data=True)
     url = (await request.form)["id"]
 
-    if not url.startswith("http") and "@" in url:
-        url = await bovine.clients.lookup_account_with_webfinger(actor.session, url)
-
-    result = await actor.retrieve(url, include=["object", "actor", "attributedTo"])
-    if result:
-        return with_bovine_context(result), 200
-    return {"status": "not found"}, 404
+    try:
+        if not url.startswith("http") and "@" in url:
+            url = await bovine.clients.lookup_account_with_webfinger(actor.session, url)
+
+        result = await actor.retrieve(url, include=["object", "actor", "attributedTo"])
+        if result:
+            return with_bovine_context(result), 200
+        return {"status": "not found"}, 404
+    except Exception as e:
+        logger.error("Something went wrong during proxy url")
+        logger.exception(e)
+        return {"status": "something went wrong"}, 400
 
 
 async def handle_event_source(endpoint_path, actor):
     if endpoint_path != actor["endpoints"]["eventSource"]:
         return {"status": "unauthorized"}, 401
 
     logger.info("Opening event source for %s", actor["name"])
```

### Comparing `bovine_herd-0.2.0/bovine_herd/server/info.py` & `bovine_herd-0.2.2/bovine_herd/server/info.py`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.0/bovine_herd/server/wellknown.py` & `bovine_herd-0.2.2/bovine_herd/server/wellknown.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 from urllib.parse import urljoin
 
-import asyncstdlib
 from bovine.utils import webfinger_response_json
 from bovine_store.utils import path_from_request
 from quart import Blueprint, current_app, request
 
 wellknown = Blueprint("wellknown", __name__, url_prefix="/.well-known")
 
 logger = logging.getLogger(__name__)
@@ -34,15 +33,14 @@
 
     if not resource.startswith("did:") and not resource.startswith("acct:"):
         return {"error": "invalid request"}, 400
 
     return await webfinger_response(resource)
 
 
-@asyncstdlib.lru_cache(32)
 async def webfinger_response(resource):
     domain = request.host
     name = None
 
     if resource == f"acct:bovine@{domain}":
         name = "bovine"
         url = f"https://{domain}/activitypub/bovine"
```

### Comparing `bovine_herd-0.2.0/bovine_herd/static/cow.jpg` & `bovine_herd-0.2.2/bovine_herd/static/cow.jpg`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.0/bovine_herd/static/moocow.png` & `bovine_herd-0.2.2/bovine_herd/static/moocow.png`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.0/bovine_herd/static/profile.png` & `bovine_herd-0.2.2/bovine_herd/static/profile.png`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.0/bovine_herd/static/style.css` & `bovine_herd-0.2.2/bovine_herd/static/style.css`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.0/bovine_herd/static/woodpecker.png` & `bovine_herd-0.2.2/bovine_herd/static/woodpecker.png`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.0/bovine_herd/templates/index.html` & `bovine_herd-0.2.2/bovine_herd/templates/index.html`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.0/bovine_herd/utils/__init__.py` & `bovine_herd-0.2.2/bovine_herd/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.0/bovine_herd/utils/test/__init__.py` & `bovine_herd-0.2.2/bovine_herd/utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.0/pyproject.toml` & `bovine_herd-0.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bovine-herd"
-version = "0.2.0"
+version = "0.2.2"
 description = ""
 authors = ["Helge <helge.krueger@gmail.com>"]
 readme = "README.md"
 packages = [{include = "bovine_herd"}]
 repository = "https://codeberg.org/bovine/bovine"
 
 [tool.poetry.dependencies]
@@ -15,17 +15,14 @@
 bovine-store = "^0.2.1"
 bovine-process = "^0.2.0"
 asyncstdlib = "^3.10.5"
 bovine-pubsub = "^0.2.0"
 tortoise-orm = {extras = ["asyncpg"], version = "^0.19.3"}
 aiodns = "^3.0.0"
 
-[tool.poetry.scripts]
-serve = "bovine_herd:run"
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.3"
```

### Comparing `bovine_herd-0.2.0/PKG-INFO` & `bovine_herd-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bovine-herd
-Version: 0.2.0
+Version: 0.2.2
 Summary: 
 Home-page: https://codeberg.org/bovine/bovine
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -44,20 +44,23 @@
 pip install bovine_tool
 python -mbovine_tool.register --domain $DOMAIN moocow
 ```
 
 you create a new account for __moocow__. This command returns its bovine name, which will be of the form `moocow + uuid4()`, e.g. `moocow_09c80006-483c-4826-b48c-cf5134b4e898`. By running:
 
 ```bash
-python -mbovine_tool.manage --new-did-key $BOVINE_NAME
+python -mbovine_tool.manage --new_did_key $BOVINE_NAME
 ```
 
 you will be given a secret (an Ed25519 private key, i.e. starts with `z3u2`). Once you have this secret, you can send a message via
 
 ```bash
 python -mbovine.msg --secret $SECRET --host $DOMAIN moooo
 ```
 
 ## Configuration
 
 The default database connection is "sqlite://bovine.sqlite3". This can be overwridden with the environment variable "BOVINE_DB_URL".
 
+- `BOVINE_REDIS` represents how to reach redis, e.g. `redis://localhost`. If not set, redis is not used. Redis is necessary when using more than one worker.
+- `BOVINE_LOGFILE` gives the path of the log file. When not present bovine.log is used.
+
```

