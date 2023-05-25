# Comparing `tmp/troncos-4.0.0b2.tar.gz` & `tmp/troncos-4.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troncos-4.0.0b2.tar", max compression
+gzip compressed data, was "troncos-4.0.0b3.tar", max compression
```

## Comparing `troncos-4.0.0b2.tar` & `troncos-4.0.0b3.tar`

### file list

```diff
@@ -1,32 +1,35 @@
--rw-r--r--   0        0        0     1077 2023-05-24 09:45:35.272978 troncos-4.0.0b2/LICENSE
--rw-r--r--   0        0        0     6282 2023-05-24 09:45:35.272978 troncos-4.0.0b2/README.md
--rw-r--r--   0        0        0     2220 2023-05-24 09:45:35.272978 troncos-4.0.0b2/pyproject.toml
--rw-r--r--   0        0        0      291 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/asgi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/asgi/logging/__init__.py
--rw-r--r--   0        0        0     5042 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/asgi/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/asgi/profiling/__init__.py
--rw-r--r--   0        0        0      576 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/asgi/profiling/app.py
--rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/django/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/django/logging/__init__.py
--rw-r--r--   0        0        0     2318 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/django/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/django/profiling/__init__.py
--rw-r--r--   0        0        0      265 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/django/profiling/views.py
--rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/starlette/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/starlette/profiling/__init__.py
--rw-r--r--   0        0        0      291 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/starlette/profiling/views.py
--rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/structlog/__init__.py
--rw-r--r--   0        0        0      705 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/contrib/structlog/processors.py
--rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/profiling/__init__.py
--rw-r--r--   0        0        0      192 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/profiling/auto.py
--rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/profiling/bootstrap/__init__.py
--rw-r--r--   0        0        0      439 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/profiling/bootstrap/profile.py
--rw-r--r--   0        0        0      343 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/profiling/bootstrap/start.py
--rw-r--r--   0        0        0     1814 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/profiling/profiler.py
--rw-r--r--   0        0        0        0 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/py.typed
--rw-r--r--   0        0        0      570 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/tracing/__init__.py
--rw-r--r--   0        0        0     1298 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/tracing/_otel.py
--rw-r--r--   0        0        0     4062 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/tracing/_span.py
--rw-r--r--   0        0        0     1672 2023-05-24 09:45:35.272978 troncos-4.0.0b2/troncos/tracing/_writer.py
--rw-r--r--   0        0        0     7169 1970-01-01 00:00:00.000000 troncos-4.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-24 13:48:05.147781 troncos-4.0.0b3/LICENSE
+-rw-r--r--   0        0        0     6939 2023-05-24 13:48:05.147781 troncos-4.0.0b3/README.md
+-rw-r--r--   0        0        0     2238 2023-05-24 13:48:05.147781 troncos-4.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/contrib/asgi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/contrib/asgi/logging/__init__.py
+-rw-r--r--   0        0        0     5058 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/contrib/asgi/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/contrib/asgi/profiling/__init__.py
+-rw-r--r--   0        0        0      576 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/contrib/asgi/profiling/app.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/contrib/celery/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/contrib/celery/logging/__init__.py
+-rw-r--r--   0        0        0      949 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/contrib/celery/logging/signals.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/contrib/django/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/contrib/django/logging/__init__.py
+-rw-r--r--   0        0        0     2334 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/contrib/django/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/contrib/django/profiling/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/contrib/django/profiling/views.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/contrib/starlette/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/contrib/starlette/profiling/__init__.py
+-rw-r--r--   0        0        0      291 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/contrib/starlette/profiling/views.py
+-rw-r--r--   0        0        0     4053 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/contrib/structlog/__init__.py
+-rw-r--r--   0        0        0      705 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/contrib/structlog/processors.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/profiling/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/profiling/auto.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/profiling/bootstrap/__init__.py
+-rw-r--r--   0        0        0      439 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/profiling/bootstrap/profile.py
+-rw-r--r--   0        0        0      343 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/profiling/bootstrap/start.py
+-rw-r--r--   0        0        0     1814 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/profiling/profiler.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/py.typed
+-rw-r--r--   0        0        0      570 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/tracing/__init__.py
+-rw-r--r--   0        0        0     1298 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/tracing/_otel.py
+-rw-r--r--   0        0        0     4062 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/tracing/_span.py
+-rw-r--r--   0        0        0     1672 2023-05-24 13:48:05.147781 troncos-4.0.0b3/troncos/tracing/_writer.py
+-rw-r--r--   0        0        0     7826 1970-01-01 00:00:00.000000 troncos-4.0.0b3/PKG-INFO
```

### Comparing `troncos-4.0.0b2/LICENSE` & `troncos-4.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b2/README.md` & `troncos-4.0.0b3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -144,14 +144,27 @@
 ```python
 MIDDLEWARE = [
     "troncos.contrib.django.logging.middleware.DjangoLoggingMiddleware",
     ...
 ]
 ```
 
+#### Celery signals
+
+`
+Log Celery tasks. Run the code bellow when you configure Celery.
+
+```python
+from troncos.contrib.celery.logging.signals import (
+    connect_troncos_logging_celery_signals,
+)
+
+connect_troncos_logging_celery_signals()
+```
+
 ## Profiling
 
 ### Enabling the profiler
 
 Start the profiler by importing the profiler module early in your application. This is
 typically done in `settings.py` of you want to profile a Django application, or in `__init__.py`
 in the root project package.
@@ -227,18 +240,33 @@
 ```
 
 ## Logging
 
 Troncos is not designed to take control over your logger. But, we do include logging
 related tools to make instrumenting your code easer.
 
+### Configure Structlog
+
+Troncos contains a helper method that lets you configure Structlog.
+
+First, run `poetry add structlog` to install structlog in your project.
+
+You can now replace your existing logger config with
+
+```python
+from troncos.contrib.structlog import configure_structlog
+
+configure_structlog(format="json", level="INFO")
+```
+
 ### Adding tracing context to your log
 
 Troncos has a Structlog processor that can be used to add the `span_id` and `trace_id`
 properties to your log. More infomation can be found in the [Tracing](#tracing)
-section in this document.
+section in this document. This is used by the `configure_structlog` helper method
+by default.
 
 ### Request logging middleware
 
 Finding the relevant traces in Tempo and Grafana can be difficult. The request logging
 middleware exist to make it easier to connect HTTP requests to traces. More infomation
 can be found in the [Tracing](#tracing) section in this document.
```

#### html2text {}

```diff
@@ -44,37 +44,46 @@
 above needs to be enabled before logging your major actions is relevant. ####
 ASGI middleware Log ASGI requests. ```python from starlette.applications import
 Starlette from troncos.contrib.asgi.logging.middleware import
 AsgiLoggingMiddleware application = AsgiLoggingMiddleware(Starlette()) ``` ####
 Django middleware Log Django requests. This is not needed if you run Django
 with ASGI and use the ASGI middleware. ```python MIDDLEWARE =
 [ "troncos.contrib.django.logging.middleware.DjangoLoggingMiddleware", ... ]
-``` ## Profiling ### Enabling the profiler Start the profiler by importing the
-profiler module early in your application. This is typically done in
-`settings.py` of you want to profile a Django application, or in `__init__.py`
-in the root project package. ```python import troncos.profiling.auto ``` ###
-Setup profile endpoint Use one of the methods bellow based on your selected
-framework. #### Django Add the profile view to the url config. ```python from
-django.urls import path from troncos.contrib.django.profiling.views import
-profiling_view urlpatterns = [ path("/debug/pprof", profiling_view,
-name="profiling"), ] ``` #### Starlette Add the profile view to your router.
-```python from starlette.routing import Route from
-troncos.contrib.starlette.profiling.views import profiling_view routes =
-[ Route("/debug/pprof", profiling_view), ] ``` #### ASGI Mount the generic ASGI
-profiling application. There is no generic way to do this, please check the
-relevant ASGI framework documentation. ```python from
+``` #### Celery signals ` Log Celery tasks. Run the code bellow when you
+configure Celery. ```python from troncos.contrib.celery.logging.signals import
+( connect_troncos_logging_celery_signals, )
+connect_troncos_logging_celery_signals() ``` ## Profiling ### Enabling the
+profiler Start the profiler by importing the profiler module early in your
+application. This is typically done in `settings.py` of you want to profile a
+Django application, or in `__init__.py` in the root project package. ```python
+import troncos.profiling.auto ``` ### Setup profile endpoint Use one of the
+methods bellow based on your selected framework. #### Django Add the profile
+view to the url config. ```python from django.urls import path from
+troncos.contrib.django.profiling.views import profiling_view urlpatterns =
+[ path("/debug/pprof", profiling_view, name="profiling"), ] ``` #### Starlette
+Add the profile view to your router. ```python from starlette.routing import
+Route from troncos.contrib.starlette.profiling.views import profiling_view
+routes = [ Route("/debug/pprof", profiling_view), ] ``` #### ASGI Mount the
+generic ASGI profiling application. There is no generic way to do this, please
+check the relevant ASGI framework documentation. ```python from
 troncos.contrib.asgi.profiling.app import profiling_asgi_app # FastAPI example
 from fastapi import FastAPI app = FastAPI() app.mount("/debug/pprof",
 profiling_asgi_app) ``` ### Verify setup You can verify that your setup works
 with the [pprof](https://github.com/google/pprof) cli: ```console $ pprof -http
 :6060 "http://localhost:8080/debug/pprof" ``` ### Enable scraping When you
 deploy your application, be sure to use the custom oda annotation for scraping:
 ```yaml annotations: phlare.oda.com/port: "8080" phlare.oda.com/scrape: "true"
 ``` ## Logging Troncos is not designed to take control over your logger. But,
 we do include logging related tools to make instrumenting your code easer. ###
-Adding tracing context to your log Troncos has a Structlog processor that can
-be used to add the `span_id` and `trace_id` properties to your log. More
-infomation can be found in the [Tracing](#tracing) section in this document.
-### Request logging middleware Finding the relevant traces in Tempo and Grafana
-can be difficult. The request logging middleware exist to make it easier to
-connect HTTP requests to traces. More infomation can be found in the [Tracing]
-(#tracing) section in this document.
+Configure Structlog Troncos contains a helper method that lets you configure
+Structlog. First, run `poetry add structlog` to install structlog in your
+project. You can now replace your existing logger config with ```python from
+troncos.contrib.structlog import configure_structlog configure_structlog
+(format="json", level="INFO") ``` ### Adding tracing context to your log
+Troncos has a Structlog processor that can be used to add the `span_id` and
+`trace_id` properties to your log. More infomation can be found in the
+[Tracing](#tracing) section in this document. This is used by the
+`configure_structlog` helper method by default. ### Request logging middleware
+Finding the relevant traces in Tempo and Grafana can be difficult. The request
+logging middleware exist to make it easier to connect HTTP requests to traces.
+More infomation can be found in the [Tracing](#tracing) section in this
+document.
```

### Comparing `troncos-4.0.0b2/pyproject.toml` & `troncos-4.0.0b3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troncos"
-version = "4.0.0b2"
+version = "4.0.0b3"
 description = "Collection of Python logging, tracing and profiling tools"
 authors = [
     "Guðmundur Björn Birkisson <gudmundur.birkisson@oda.com>",
     "Karl Fredrik Haugland <karlfredrik.haugland@oda.com>",
     "Eirik Martiniussen Sylliaas <eirik.sylliaas@oda.com>",
 ]
 license = "MIT"
@@ -35,14 +35,15 @@
 pytest-asyncio = ">=0.20.3,<0.22.0"
 django-environ = "^0.9.0"
 pytest-benchmark = "^4.0.0"
 snakeviz = "^2.2.0"
 django = "^4.2.1"
 starlette = "^0.27.0"
 structlog = "^23.1.0"
+celery = "^5.2.7"
 
 
 [tool.black]
 target-version = ['py311']
 line-length = 88
 include = '\.pyi?$'
 safe = true
```

### Comparing `troncos-4.0.0b2/troncos/contrib/asgi/logging/middleware.py` & `troncos-4.0.0b3/troncos/contrib/asgi/logging/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,16 @@
     def __init__(
         self,
         app: Any,
         logger_name: str | None = None,
     ) -> None:
         self._app = app
         ln = logger_name or "asgi"
-        self._access = get_logger(f"{ln}.access")
-        self._error = get_logger(f"{ln}.error")
+        self._access = get_logger(f"troncos.{ln}.access")
+        self._error = get_logger(f"troncos.{ln}.error")
 
     async def __call__(
         self,
         scope: dict[str, Any],
         receive: Callable[[Any], Any],
         send: Callable[[dict[str, Any]], Awaitable[Any]],
     ) -> Any:
```

### Comparing `troncos-4.0.0b2/troncos/contrib/asgi/profiling/app.py` & `troncos-4.0.0b3/troncos/contrib/asgi/profiling/app.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b2/troncos/contrib/django/logging/middleware.py` & `troncos-4.0.0b3/troncos/contrib/django/logging/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 @sync_and_async_middleware
 def DjangoLoggingMiddleware(get_response):  # type: ignore
     """
     Django middleware that logs requests.
     """
 
-    access = get_logger("django.access")
-    error = get_logger("django.error")
+    access = get_logger("troncos.django.access")
+    error = get_logger("troncos.django.error")
 
     ipware = IpWare()
 
     def extract_request_data(request: HttpRequest) -> tuple[dict[str, Any], float]:
         start_time = time.perf_counter()
 
         client_ip, _ = ipware.get_client_ip(request.META)
```

### Comparing `troncos-4.0.0b2/troncos/contrib/structlog/processors.py` & `troncos-4.0.0b3/troncos/contrib/structlog/processors.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b2/troncos/profiling/profiler.py` & `troncos-4.0.0b3/troncos/profiling/profiler.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b2/troncos/tracing/__init__.py` & `troncos-4.0.0b3/troncos/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b2/troncos/tracing/_otel.py` & `troncos-4.0.0b3/troncos/tracing/_otel.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b2/troncos/tracing/_span.py` & `troncos-4.0.0b3/troncos/tracing/_span.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b2/troncos/tracing/_writer.py` & `troncos-4.0.0b3/troncos/tracing/_writer.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b2/PKG-INFO` & `troncos-4.0.0b3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troncos
-Version: 4.0.0b2
+Version: 4.0.0b3
 Summary: Collection of Python logging, tracing and profiling tools
 Home-page: https://github.com/kolonialno/troncos
 License: MIT
 Keywords: logs,traces,opentelemetry
 Author: Guðmundur Björn Birkisson
 Author-email: gudmundur.birkisson@oda.com
 Requires-Python: >=3.10,<4.0
@@ -166,14 +166,27 @@
 ```python
 MIDDLEWARE = [
     "troncos.contrib.django.logging.middleware.DjangoLoggingMiddleware",
     ...
 ]
 ```
 
+#### Celery signals
+
+`
+Log Celery tasks. Run the code bellow when you configure Celery.
+
+```python
+from troncos.contrib.celery.logging.signals import (
+    connect_troncos_logging_celery_signals,
+)
+
+connect_troncos_logging_celery_signals()
+```
+
 ## Profiling
 
 ### Enabling the profiler
 
 Start the profiler by importing the profiler module early in your application. This is
 typically done in `settings.py` of you want to profile a Django application, or in `__init__.py`
 in the root project package.
@@ -249,19 +262,34 @@
 ```
 
 ## Logging
 
 Troncos is not designed to take control over your logger. But, we do include logging
 related tools to make instrumenting your code easer.
 
+### Configure Structlog
+
+Troncos contains a helper method that lets you configure Structlog.
+
+First, run `poetry add structlog` to install structlog in your project.
+
+You can now replace your existing logger config with
+
+```python
+from troncos.contrib.structlog import configure_structlog
+
+configure_structlog(format="json", level="INFO")
+```
+
 ### Adding tracing context to your log
 
 Troncos has a Structlog processor that can be used to add the `span_id` and `trace_id`
 properties to your log. More infomation can be found in the [Tracing](#tracing)
-section in this document.
+section in this document. This is used by the `configure_structlog` helper method
+by default.
 
 ### Request logging middleware
 
 Finding the relevant traces in Tempo and Grafana can be difficult. The request logging
 middleware exist to make it easier to connect HTTP requests to traces. More infomation
 can be found in the [Tracing](#tracing) section in this document.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: troncos Version: 4.0.0b2 Summary: Collection of
+Metadata-Version: 2.1 Name: troncos Version: 4.0.0b3 Summary: Collection of
 Python logging, tracing and profiling tools Home-page: https://github.com/
 kolonialno/troncos License: MIT Keywords: logs,traces,opentelemetry Author:
 GuÃ°mundur BjÃ¶rn Birkisson Author-email: gudmundur.birkisson@oda.com Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ddtrace (==1.13.3) Requires-Dist: opentelemetry-exporter-otlp-
@@ -56,37 +56,46 @@
 above needs to be enabled before logging your major actions is relevant. ####
 ASGI middleware Log ASGI requests. ```python from starlette.applications import
 Starlette from troncos.contrib.asgi.logging.middleware import
 AsgiLoggingMiddleware application = AsgiLoggingMiddleware(Starlette()) ``` ####
 Django middleware Log Django requests. This is not needed if you run Django
 with ASGI and use the ASGI middleware. ```python MIDDLEWARE =
 [ "troncos.contrib.django.logging.middleware.DjangoLoggingMiddleware", ... ]
-``` ## Profiling ### Enabling the profiler Start the profiler by importing the
-profiler module early in your application. This is typically done in
-`settings.py` of you want to profile a Django application, or in `__init__.py`
-in the root project package. ```python import troncos.profiling.auto ``` ###
-Setup profile endpoint Use one of the methods bellow based on your selected
-framework. #### Django Add the profile view to the url config. ```python from
-django.urls import path from troncos.contrib.django.profiling.views import
-profiling_view urlpatterns = [ path("/debug/pprof", profiling_view,
-name="profiling"), ] ``` #### Starlette Add the profile view to your router.
-```python from starlette.routing import Route from
-troncos.contrib.starlette.profiling.views import profiling_view routes =
-[ Route("/debug/pprof", profiling_view), ] ``` #### ASGI Mount the generic ASGI
-profiling application. There is no generic way to do this, please check the
-relevant ASGI framework documentation. ```python from
+``` #### Celery signals ` Log Celery tasks. Run the code bellow when you
+configure Celery. ```python from troncos.contrib.celery.logging.signals import
+( connect_troncos_logging_celery_signals, )
+connect_troncos_logging_celery_signals() ``` ## Profiling ### Enabling the
+profiler Start the profiler by importing the profiler module early in your
+application. This is typically done in `settings.py` of you want to profile a
+Django application, or in `__init__.py` in the root project package. ```python
+import troncos.profiling.auto ``` ### Setup profile endpoint Use one of the
+methods bellow based on your selected framework. #### Django Add the profile
+view to the url config. ```python from django.urls import path from
+troncos.contrib.django.profiling.views import profiling_view urlpatterns =
+[ path("/debug/pprof", profiling_view, name="profiling"), ] ``` #### Starlette
+Add the profile view to your router. ```python from starlette.routing import
+Route from troncos.contrib.starlette.profiling.views import profiling_view
+routes = [ Route("/debug/pprof", profiling_view), ] ``` #### ASGI Mount the
+generic ASGI profiling application. There is no generic way to do this, please
+check the relevant ASGI framework documentation. ```python from
 troncos.contrib.asgi.profiling.app import profiling_asgi_app # FastAPI example
 from fastapi import FastAPI app = FastAPI() app.mount("/debug/pprof",
 profiling_asgi_app) ``` ### Verify setup You can verify that your setup works
 with the [pprof](https://github.com/google/pprof) cli: ```console $ pprof -http
 :6060 "http://localhost:8080/debug/pprof" ``` ### Enable scraping When you
 deploy your application, be sure to use the custom oda annotation for scraping:
 ```yaml annotations: phlare.oda.com/port: "8080" phlare.oda.com/scrape: "true"
 ``` ## Logging Troncos is not designed to take control over your logger. But,
 we do include logging related tools to make instrumenting your code easer. ###
-Adding tracing context to your log Troncos has a Structlog processor that can
-be used to add the `span_id` and `trace_id` properties to your log. More
-infomation can be found in the [Tracing](#tracing) section in this document.
-### Request logging middleware Finding the relevant traces in Tempo and Grafana
-can be difficult. The request logging middleware exist to make it easier to
-connect HTTP requests to traces. More infomation can be found in the [Tracing]
-(#tracing) section in this document.
+Configure Structlog Troncos contains a helper method that lets you configure
+Structlog. First, run `poetry add structlog` to install structlog in your
+project. You can now replace your existing logger config with ```python from
+troncos.contrib.structlog import configure_structlog configure_structlog
+(format="json", level="INFO") ``` ### Adding tracing context to your log
+Troncos has a Structlog processor that can be used to add the `span_id` and
+`trace_id` properties to your log. More infomation can be found in the
+[Tracing](#tracing) section in this document. This is used by the
+`configure_structlog` helper method by default. ### Request logging middleware
+Finding the relevant traces in Tempo and Grafana can be difficult. The request
+logging middleware exist to make it easier to connect HTTP requests to traces.
+More infomation can be found in the [Tracing](#tracing) section in this
+document.
```

