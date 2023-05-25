# Comparing `tmp/spic-0.0.5.tar.gz` & `tmp/spic-0.0.6.tar.gz`

## Comparing `spic-0.0.5.tar` & `spic-0.0.6.tar`

### file list

```diff
@@ -1,68 +1,67 @@
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 spic-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 spic-0.0.5/COVERAGE.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 spic-0.0.5/Makefile
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 spic-0.0.5/book.toml
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 spic-0.0.5/test.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 spic-0.0.5/.github/workflows/coverage.yaml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 spic-0.0.5/.github/workflows/ruff.yaml
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 spic-0.0.5/docs/SUMMARY.md
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 spic-0.0.5/docs/USERGUIDE.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 spic-0.0.5/docs/installation.md
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 spic-0.0.5/docs/intro.md
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 spic-0.0.5/docs/tldr.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 spic-0.0.5/performance/go.mod
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 spic-0.0.5/performance/perf_test.go
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 spic-0.0.5/performance/results.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 spic-0.0.5/performance/run.sh
--rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 spic-0.0.5/scripts/cov.sh
--rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 spic-0.0.5/scripts/test.sh
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/__about__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/__init__.py
--rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/default.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/defaults.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/emit.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/encoders.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/enums.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/exception_handlers.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/exceptions.py
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/func_handler.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/inspect.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/middleware.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/request.py
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/responses.py
--rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/routing.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/types.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/utils.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/openapi/__init__.py
--rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/openapi/models.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/openapi/utils.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/params/__init__.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 spic-0.0.5/src/spic/params/params.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 spic-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 spic-0.0.5/tests/buf.gen.yaml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 spic-0.0.5/tests/buf.yaml
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 spic-0.0.5/tests/methods.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_call.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_dataclass_headers.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_dataclass_mixed.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_dataclass_query.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_grpc.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_hdr_args.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_openapi.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_param_wrapper.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_query_args.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_responses.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_router.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_schema.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 spic-0.0.5/tests/test_start.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spic-0.0.5/tests/protos/__init.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 spic-0.0.5/tests/protos/hello.proto
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spic-0.0.5/tests/protos/gen/__init__.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 spic-0.0.5/tests/protos/gen/hello_pb2.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 spic-0.0.5/tests/protos/gen/hello_pb2.pyi
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 spic-0.0.5/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 spic-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 spic-0.0.5/README.md
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 spic-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 spic-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 spic-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 spic-0.0.6/COVERAGE.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 spic-0.0.6/Makefile
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 spic-0.0.6/book.toml
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 spic-0.0.6/test.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 spic-0.0.6/.github/workflows/coverage.yaml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 spic-0.0.6/.github/workflows/ruff.yaml
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 spic-0.0.6/docs/SUMMARY.md
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 spic-0.0.6/docs/USERGUIDE.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 spic-0.0.6/docs/installation.md
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 spic-0.0.6/docs/intro.md
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 spic-0.0.6/docs/tldr.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 spic-0.0.6/performance/go.mod
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 spic-0.0.6/performance/perf_test.go
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 spic-0.0.6/performance/results.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 spic-0.0.6/performance/run.sh
+-rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 spic-0.0.6/scripts/cov.sh
+-rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 spic-0.0.6/scripts/test.sh
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/__about__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/__init__.py
+-rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/app.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/defaults.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/emit.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/encoders.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/enums.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/exception_handlers.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/exceptions.py
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/func_handler.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/inspect.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/middleware.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/request.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/responses.py
+-rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/routing.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/types.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/utils.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/openapi/__init__.py
+-rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/openapi/models.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/openapi/utils.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/params/__init__.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 spic-0.0.6/src/spic/params/params.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 spic-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 spic-0.0.6/tests/buf.gen.yaml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 spic-0.0.6/tests/buf.yaml
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 spic-0.0.6/tests/methods.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 spic-0.0.6/tests/test_call.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 spic-0.0.6/tests/test_dataclass_headers.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 spic-0.0.6/tests/test_dataclass_mixed.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 spic-0.0.6/tests/test_dataclass_query.py
+-rw-r--r--   0        0        0     5438 2020-02-02 00:00:00.000000 spic-0.0.6/tests/test_encoders.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 spic-0.0.6/tests/test_grpc.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 spic-0.0.6/tests/test_hdr_args.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 spic-0.0.6/tests/test_openapi.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 spic-0.0.6/tests/test_param_wrapper.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 spic-0.0.6/tests/test_query_args.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 spic-0.0.6/tests/test_router.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 spic-0.0.6/tests/test_schema.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 spic-0.0.6/tests/test_start.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spic-0.0.6/tests/protos/__init.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 spic-0.0.6/tests/protos/hello.proto
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spic-0.0.6/tests/protos/gen/__init__.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 spic-0.0.6/tests/protos/gen/hello_pb2.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 spic-0.0.6/tests/protos/gen/hello_pb2.pyi
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 spic-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 spic-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 spic-0.0.6/README.md
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 spic-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 spic-0.0.6/PKG-INFO
```

### Comparing `spic-0.0.5/.pre-commit-config.yaml` & `spic-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/test.py` & `spic-0.0.6/test.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/.github/workflows/coverage.yaml` & `spic-0.0.6/.github/workflows/coverage.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -7,12 +7,12 @@
       - name: Checkout
         uses: actions/checkout@v3
       - name: Set up Python 3.10
         uses: actions/setup-python@v4
         with:
           python-version: '3.10'
       - name: Install dependencies
-        run: pip install '.[dev,msgpack,core,experimental]'
+        run: pip install '.[dev,msgpack,grpc-compat,experimental]'
       - name: Run tests and collect coverage
         run: pytest --cov app
       - name: Upload coverage to Codecov
         uses: codecov/codecov-action@v3
```

### Comparing `spic-0.0.5/docs/intro.md` & `spic-0.0.6/docs/intro.md`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/docs/tldr.md` & `spic-0.0.6/docs/tldr.md`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/performance/perf_test.go` & `spic-0.0.6/performance/perf_test.go`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/src/spic/app.py` & `spic-0.0.6/src/spic/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 from typing import cast
 
 from beartype.roar import BeartypeCallException, BeartypeCallHintParamViolation, BeartypeCallHintReturnViolation
 from hypercorn.typing import HTTPScope, Scope
 from rich.console import Console
 
 from .__about__ import __version__
-from .defaults import DefaultConsole
+from .defaults import DEFAULT_LOG_LEVEL, DefaultConsole
 from .emit import _emit
 from .enums import LogLevel
 from .exceptions import HTTPError, JSONError, SerializableValidationErrors, send_error
 from .func_handler import ManyValidationErrors
 from .middleware import Middleware
 from .openapi import OAPI_VERSION, OpenAPISchema, get_schema_from_route
+from .openapi.models import ExternalDocumentation, Info, Server
 from .request import Request
 from .routing import Router
 from .types import P
 from .utils import log_level, safe_path, when_none
 
 
 class Spic:
@@ -25,73 +26,76 @@
     routes = []
     router: Router
     console: Console
     schema: OpenAPISchema
     middlewares: list[Middleware] = []
     log_level: LogLevel
     type_validation: bool
+    servers: list[Server]
+    tags: list[dict]
+    external_docs: ExternalDocumentation
 
     def __init__(
         self,
         title: str = None,
         console: Console = None,
         prefix: str = None,
         version: str = None,
-        log_level: LogLevel = LogLevel.follow,
+        log_level: LogLevel = None,
         type_validation: bool = None,
+        servers: list[Server] = None,
+        tags: list[dict] = None,
+        external_docs: ExternalDocumentation = None,
     ):
-        self.log_level = log_level
+        self.log_level = when_none(log_level, DEFAULT_LOG_LEVEL)
         if console is None:
             console = DefaultConsole
         self.console = console
         self.root_path = prefix
         self.title = when_none(title, "SPIC app")
         self.version = when_none(version, f"spic-{__version__}")
         self.router = Router(
             prefix=prefix,
             console=self.console,
             log_level=self.log_level,
         )
         self.type_validation = when_none(type_validation, True)
+        self.servers = when_none(servers, [])
+        self.tags = when_none(tags, [])
+        self.external_docs = external_docs
 
     async def __call__(self, scope: Scope, receive, send):
         if scope["type"] != "http":
             msg = "Only the HTTP protocol is supported"
             raise Exception(msg)
         scope = cast(HTTPScope, scope)
         path = safe_path(scope.get("path", "/"))[1:]
         mtd = scope.get("method")
         route = self.router.hashed.get(path)
         if route is None:
             __err__ = f"no path matching {path} with the attempted method ({mtd})"
-            await send_error(
+            await self.send_error(
                 send,
                 HTTPError(status_code=HTTPStatus.NOT_FOUND, message=__err__),
-                l_level=self.log_level,
-                trace=self.console,
             )
             return
 
         elif mtd not in route.methods:
             __err__ = f"invalid method ({mtd}) for path: {path}"
-            await send_error(
+            await self.send_error(
                 send,
                 HTTPError(status_code=HTTPStatus.METHOD_NOT_ALLOWED, message=__err__),
-                l_level=self.log_level,
-                trace=self.console,
             )
             return
         handler = route.func.get(mtd)
         if handler is None or not callable(handler):
             __err__ = "internal server error"
-            await send_error(
+            await self.send_error(
                 send,
                 HTTPError(status_code=HTTPStatus.INTERNAL_SERVER_ERROR, message=__err__),
-                l_level=self.log_level,
-                trace=self.console,
             )
             return
         _ = await receive()
         request = Request(**scope)
         try:
             response = await handler(request)
             await _emit(send, response, trace=self.console, l_level=self.log_level)
@@ -135,20 +139,24 @@
         await send_error(
             send,
             exception,
             trace=self.console,
             l_level=self.log_level,
         )
 
-    async def match_paths(self, path):
-        pass
-
     @property
     def base_schema(self):
-        return {"openapi": OAPI_VERSION, "info": {"title": self.title, "version": self.version}, "paths": {}}
+        return {
+            "openapi": OAPI_VERSION,
+            "info": Info(title=self.title, version=self.version),
+            "paths": {},
+            "tags": self.tags,
+            "servers": self.servers,
+            "external_docs": self.external_docs,
+        }
 
     def finalize_schema(self):
         schema = self.schema
 
         for route in self.routes:
             if route.include_in_schema:
                 schema.paths[route.path] = get_schema_from_route(route)
```

### Comparing `spic-0.0.5/src/spic/emit.py` & `spic-0.0.6/src/spic/emit.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/src/spic/encoders.py` & `spic-0.0.6/src/spic/encoders.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,122 +1,143 @@
-from collections.abc import Iterable, Mapping
+from collections.abc import Generator, Mapping
 from dataclasses import is_dataclass
-from typing import Any, Callable
+from typing import Callable
 from typing import Mapping as TMapping
 
 from serde import is_serializable
 from serde.json import to_json as dc_to_json
 
 from .enums import FormatMessageOps, RegisteredContent
 from .exception_handlers import NoImplmt
 from .responses import Response
 from .types import P, T, create_raises_dep_error
-from .utils import merged_mapping
 
+try:  # no cov
+    from serde.msgpack import to_msgpack as dc_to_msg  # no cov
+except ImportError:  # no cov
+    dc_to_msg = create_raises_dep_error("pyserde[msgpack]")  # no cov
 try:
-    from serde.msgpack import to_msgpack as dc_to_msg
-except ImportError:
-    dc_to_msg = create_raises_dep_error("pyserde[msgpack]")
-try:
-    from srsly import json_dumps as mapping_to_json
-except ImportError:
-    mapping_to_json = create_raises_dep_error("srsly")
-try:
-    from google.protobuf.json_format import MessageToDict, MessageToJson
-    from google.protobuf.message import Message
-except ImportError:
-    MessageToDict = create_raises_dep_error("protobuf")
-    MessageToJson = create_raises_dep_error("protobuf")
+    from msgpack import packb  # no cov
+except ImportError:  # no cov
+    packb = create_raises_dep_error("msgpack")  # no cov
+try:  # no cov
+    from srsly import json_dumps as mapping_to_json  # no cov
+except ImportError:  # no cov
+    mapping_to_json = create_raises_dep_error("srsly")  # no cov
+try:  # no cov
+    from google.protobuf.json_format import MessageToDict, MessageToJson  # no cov
+    from google.protobuf.message import Message  # no cov
+except ImportError:  # no cov
+    MessageToDict = create_raises_dep_error("protobuf")  # no cov
+    MessageToJson = create_raises_dep_error("protobuf")  # no cov
 
     class Message:
         __call__ = create_raises_dep_error("protobuf")
 
 
-def content_media_handler(content_type: RegisteredContent, *resp_args: P.args, **resp_kwargs: P.kwargs):
-    defaults = {}
-
+def content_encoding(content_type: RegisteredContent, *resp_args: P.args, **resp_kwargs: P.kwargs):
     def call(encode: Callable[[T], bytes]):
         def inner(obj: T):
+            if isinstance(obj, Generator):
+                obj = list(obj)
             content = encode(obj)
-            return Response(
-                *resp_args, content=content, content_type=content_type, **merged_mapping(defaults, resp_kwargs)
-            )
+            return Response(*resp_args, content=content, content_type=content_type, **resp_kwargs)
 
         return inner
 
     return call
 
 
-@content_media_handler(RegisteredContent.TEXT)
+@content_encoding(RegisteredContent.TEXT)
 def text(obj):
-    return str(obj)
+    if isinstance(obj, (bool, int, float, str, bytes)):
+        return obj
+    elif obj is None:
+        return ""
+    raise NoImplmt() from None
+
+
+def _msgpack_obj(obj):
+    if is_dataclass(obj) and is_serializable(obj):
+        return dc_to_msg(obj)
+    try:
+        return packb(obj)
+    except:  # noqa: E722
+        raise NoImplmt() from None
 
 
-@content_media_handler(RegisteredContent.MSGPACK)
+@content_encoding(RegisteredContent.MSGPACK)
 def msgpack(obj):
-    if is_dataclass(obj):
-        msg = dc_to_msg(obj)
-    else:
-        raise NoImplmt() from obj
-    return msg
+    if not isinstance(obj, list):
+        return _msgpack_obj(obj)
+    elif len(obj) == 0:
+        return packb(obj)
+    elif is_dataclass(obj[0]) and is_serializable(obj[0]):
+        return dc_to_msg(obj)
+    return _msgpack_obj(obj)
 
 
-def message_to(obj: Message, op: FormatMessageOps, *args: P.args, **kwargs: P.kwargs):
+def message_to(obj: Message, op: FormatMessageOps, *args: P.args, **kwargs: P.kwargs) -> dict | str:
     func = MessageToJson if op is FormatMessageOps.to_json else MessageToDict
-    try:
-        return func(obj, *args, **kwargs)
-    except:  # noqa: E722
-        raise NoImplmt() from None
+    return func(obj, *args, **kwargs)
 
 
 def _grpc_conversion(obj: Message | list[Message], *args: P.args, **kwargs: P.kwargs):
-    if isinstance(obj, list):
-        json = mapping_to_json([message_to(o, FormatMessageOps.to_dict) for o in obj])
+    isli = isinstance(obj, list)
+    if isli and len(obj) != 0 and isinstance(obj[0], Message):
+        json: str = mapping_to_json([message_to(o, FormatMessageOps.to_dict) for o in obj])
+    elif isli and len(obj) == 0:
+        json: str = "[]"
+    elif isinstance(obj, Message):
+        json: str = message_to(obj, FormatMessageOps.to_json, *args, **kwargs)
     else:
-        json = message_to(obj, FormatMessageOps.to_json, *args, **kwargs)
+        raise NoImplmt() from None
     return json
 
 
-@content_media_handler(RegisteredContent.JSON)
+@content_encoding(RegisteredContent.JSON)
 def grpc(obj: Message | list[Message], *args: P.args, **kwargs: P.kwargs):
     return _grpc_conversion(obj, *args, **kwargs)
 
 
-@content_media_handler(RegisteredContent.JSON)
+@content_encoding(RegisteredContent.JSON)
 def json(obj):
     if isinstance(obj, str):
-        json = obj.encode()
+        json = obj
     elif isinstance(obj, (bytes)):
         json = obj
-    elif is_dataclass(obj) and is_serializable(obj):
+    elif isinstance(obj, list) and len(obj) == 0:
+        json = "[]"
+    elif (is_dataclass(obj) and is_serializable(obj)) or (
+        isinstance(obj, list) and is_dataclass(obj[0]) and is_serializable(obj[0])
+    ):
         json = dc_to_json(obj)
     elif hasattr(obj, "json"):
         if callable(obj.json):
             json = obj.json()
         else:
             json = obj.json
     elif hasattr(obj, "dict"):
         if callable(obj.dict):
             json = mapping_to_json(obj.dict())
         else:
             json = mapping_to_json(obj.dict)
+    elif isinstance(obj, (Message)) or (isinstance(obj, list) and isinstance(obj[0], Message)):
+        json = _grpc_conversion(obj)
     elif isinstance(
         obj,
         (
             Mapping,
             TMapping,
-            Iterable,
             dict,
             bool,
             int,
             float,
         ),
     ):
         json = mapping_to_json(obj)
-    elif isinstance(obj, Message):
-        json = _grpc_conversion(obj)
     else:
         try:
             json = mapping_to_json(obj)
         except:  # noqa: E722
-            raise NoImplmt() from obj
+            raise NoImplmt() from None
     return json
```

### Comparing `spic-0.0.5/src/spic/exceptions.py` & `spic-0.0.6/src/spic/exceptions.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/src/spic/func_handler.py` & `spic-0.0.6/src/spic/func_handler.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/src/spic/inspect.py` & `spic-0.0.6/src/spic/inspect.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/src/spic/middleware.py` & `spic-0.0.6/src/spic/middleware.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/src/spic/request.py` & `spic-0.0.6/src/spic/request.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/src/spic/responses.py` & `spic-0.0.6/src/spic/responses.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,18 @@
         Returns:
             ResponseBody: TypedDict representing the object returned by the raw response body
         """
         if not isinstance(self.content, bytes):
             if isinstance(self.content, str):
                 self.content = cast(str, self.content).encode()
             elif isinstance(self.content, (int, float)):
-                self.content = f"{self.content:.0f}"
+                fmt = "{:}"
+                if isinstance(self.content, int):
+                    fmt = "{:.0f}"
+                self.content = fmt.format(self.content).encode()
 
         return {
             "type": "http.response.body",
             "body": self.content,
             "headers": [
                 (
                     b"content-length",
```

### Comparing `spic-0.0.5/src/spic/routing.py` & `spic-0.0.6/src/spic/routing.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/src/spic/types.py` & `spic-0.0.6/src/spic/types.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/src/spic/utils.py` & `spic-0.0.6/src/spic/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 from dataclasses import dataclass
 from typing import Optional, TypeVar
 
 from rich.console import Console
 from serde import serde
 
 from .enums import LogLevel
-from .types import LA, Hdr, Lazy, P
-
-# from logging import getLogger, INFO, ERROR, CRITICAL, DEBUG
-
-# logger = getLogger(__name__)
+from .types import LA, Lazy, P
 
 T = TypeVar("T")
 
 
 def safe_path(st: str):
     return st.split("?")[0]
 
@@ -36,18 +32,14 @@
         if iscoro:
             return await func(*args, **kwargs)
         return func(*args, **kwargs)
 
     return inner
 
 
-def merged_mapping(hdr1: Hdr, hdr2: Hdr):
-    return {**when_none(hdr2, {}), **when_none(hdr1, {})}
-
-
 def schema(cls=None, *args: P.args, **kwargs: P.kwargs):
     def inner(adaptor):
         return serde(*args, **kwargs)(dataclass(adaptor))
 
     if cls is None:
         return inner
     return inner(cls)
@@ -59,10 +51,7 @@
 #     LogLevel.headless: None
 # }
 
 
 def log_level(console: Console, l_level: LogLevel, gt: LogLevel, *args: P.args, **kwargs: P.kwargs):
     if l_level.value >= gt.value and console is not None:
         console.log(*args, **kwargs)
-    # level = LEVEL_TO[l_level]
-    # if level:
-    #     logger.log(level, *args, **kwargs)
```

### Comparing `spic-0.0.5/src/spic/openapi/models.py` & `spic-0.0.6/src/spic/openapi/models.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/src/spic/params/__init__.py` & `spic-0.0.6/src/spic/params/__init__.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/src/spic/params/params.py` & `spic-0.0.6/src/spic/params/params.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/tests/test_call.py` & `spic-0.0.6/tests/test_call.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/tests/test_dataclass_headers.py` & `spic-0.0.6/tests/test_dataclass_headers.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/tests/test_dataclass_mixed.py` & `spic-0.0.6/tests/test_dataclass_mixed.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/tests/test_dataclass_query.py` & `spic-0.0.6/tests/test_dataclass_query.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/tests/test_hdr_args.py` & `spic-0.0.6/tests/test_hdr_args.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/tests/test_openapi.py` & `spic-0.0.6/tests/test_openapi.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/tests/test_param_wrapper.py` & `spic-0.0.6/tests/test_param_wrapper.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/tests/test_query_args.py` & `spic-0.0.6/tests/test_query_args.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/tests/test_router.py` & `spic-0.0.6/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/tests/protos/gen/hello_pb2.py` & `spic-0.0.6/tests/protos/gen/hello_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: hello.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
+
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0bhello.proto\x12\x04test\"\x15\n\x03Hey\x12\x0e\n\x02hi\x18\x01 \x01(\tR\x02hiBF\n\x08\x63om.testB\nHelloProtoP\x01\xa2\x02\x03TXX\xaa\x02\x04Test\xca\x02\x04Test\xe2\x02\x10Test\\GPBMetadata\xea\x02\x04Testb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
+    b'\n\x0bhello.proto\x12\x04test\"\x15\n\x03Hey\x12\x0e\n\x02hi\x18\x01 \x01(\tR\x02hiBF\n\x08\x63om.testB\nHelloProtoP\x01\xa2\x02\x03TXX\xaa\x02\x04Test\xca\x02\x04Test\xe2\x02\x10Test\\GPBMetadata\xea\x02\x04Testb\x06proto3'
+)
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'hello_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\010com.testB\nHelloProtoP\001\242\002\003TXX\252\002\004Test\312\002\004Test\342\002\020Test\\GPBMetadata\352\002\004Test'
-  _globals['_HEY']._serialized_start=21
-  _globals['_HEY']._serialized_end=42
+    DESCRIPTOR._options = None
+    DESCRIPTOR._serialized_options = b'\n\010com.testB\nHelloProtoP\001\242\002\003TXX\252\002\004Test\312\002\004Test\342\002\020Test\\GPBMetadata\352\002\004Test'
+    _globals['_HEY']._serialized_start = 21
+    _globals['_HEY']._serialized_end = 42
 # @@protoc_insertion_point(module_scope)
```

### Comparing `spic-0.0.5/LICENSE.txt` & `spic-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/README.md` & `spic-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/pyproject.toml` & `spic-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spic-0.0.5/PKG-INFO` & `spic-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spic
-Version: 0.0.5
+Version: 0.0.6
 Summary: a little opinionated framework for creating spic & span apis
 Project-URL: Documentation, https://github.com/joshua-auchincloss/spic#readme
 Project-URL: Issues, https://github.com/joshua-auchincloss/spic/issues
 Project-URL: Source, https://github.com/joshua-auchincloss/spic
 Author-email: joshua-auchincloss <joshua.auchincloss@proton.me>
 License-Expression: MIT
 License-File: LICENSE.txt
```

