# Comparing `tmp/honeycomb_beeline-3.5.1.tar.gz` & `tmp/honeycomb_beeline-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honeycomb_beeline-3.5.1.tar", max compression
+gzip compressed data, was "honeycomb_beeline-3.5.2.tar", max compression
```

## Comparing `honeycomb_beeline-3.5.1.tar` & `honeycomb_beeline-3.5.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11357 2023-01-19 13:22:06.524243 honeycomb_beeline-3.5.1/LICENSE
--rw-r--r--   0        0        0     1493 2023-01-19 13:22:06.524243 honeycomb_beeline-3.5.1/README.md
--rw-r--r--   0        0        0    28706 2023-01-19 13:22:06.524243 honeycomb_beeline-3.5.1/beeline/__init__.py
--rw-r--r--   0        0        0     4396 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/aiotrace.py
--rw-r--r--   0        0        0      557 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/internal.py
--rw-r--r--   0        0        0        0 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/middleware/__init__.py
--rw-r--r--   0        0        0     5977 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/middleware/awslambda/__init__.py
--rw-r--r--   0        0        0    10594 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/middleware/awslambda/test_awslambda.py
--rw-r--r--   0        0        0      646 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/middleware/bottle/__init__.py
--rw-r--r--   0        0        0     1110 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/middleware/bottle/test_bottle.py
--rw-r--r--   0        0        0     8190 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/middleware/django/__init__.py
--rw-r--r--   0        0        0     3534 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/middleware/django/test_django.py
--rw-r--r--   0        0        0     4611 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/middleware/flask/__init__.py
--rw-r--r--   0        0        0     2210 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/middleware/flask/test_flask.py
--rw-r--r--   0        0        0      648 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/middleware/werkzeug/__init__.py
--rw-r--r--   0        0        0     1114 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/middleware/werkzeug/test_werkzeug.py
--rw-r--r--   0        0        0     1678 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/patch/__init__.py
--rw-r--r--   0        0        0      413 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/patch/jinja2.py
--rw-r--r--   0        0        0     1971 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/patch/requests.py
--rw-r--r--   0        0        0     1160 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/patch/test_jinja2.py
--rw-r--r--   0        0        0     4507 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/patch/test_requests.py
--rw-r--r--   0        0        0     2207 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/patch/test_urllib.py
--rw-r--r--   0        0        0     1857 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/patch/tornado.py
--rw-r--r--   0        0        0     2311 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/patch/urllib.py
--rw-r--r--   0        0        0     3483 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/propagation/__init__.py
--rw-r--r--   0        0        0      769 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/propagation/default.py
--rw-r--r--   0        0        0     3682 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/propagation/honeycomb.py
--rw-r--r--   0        0        0     4349 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/propagation/test_honeycomb.py
--rw-r--r--   0        0        0     1365 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/propagation/test_propagation.py
--rw-r--r--   0        0        0     3392 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/propagation/test_w3c.py
--rw-r--r--   0        0        0     3299 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/propagation/w3c.py
--rw-r--r--   0        0        0    14634 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/test_async.py
--rw-r--r--   0        0        0    10573 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/test_beeline.py
--rw-r--r--   0        0        0      398 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/test_internal.py
--rw-r--r--   0        0        0     1129 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/test_suite.py
--rw-r--r--   0        0        0    29567 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/test_trace.py
--rw-r--r--   0        0        0    15263 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/trace.py
--rw-r--r--   0        0        0       47 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/beeline/version.py
--rw-r--r--   0        0        0      805 2023-01-19 13:22:06.528243 honeycomb_beeline-3.5.1/pyproject.toml
--rw-r--r--   0        0        0     2561 1970-01-01 00:00:00.000000 honeycomb_beeline-3.5.1/setup.py
--rw-r--r--   0        0        0     2322 1970-01-01 00:00:00.000000 honeycomb_beeline-3.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-25 19:42:35.481932 honeycomb_beeline-3.5.2/LICENSE
+-rw-r--r--   0        0        0     1742 2023-05-25 19:42:35.481932 honeycomb_beeline-3.5.2/README.md
+-rw-r--r--   0        0        0    28706 2023-05-25 19:42:35.481932 honeycomb_beeline-3.5.2/beeline/__init__.py
+-rw-r--r--   0        0        0     4396 2023-05-25 19:42:35.481932 honeycomb_beeline-3.5.2/beeline/aiotrace.py
+-rw-r--r--   0        0        0      557 2023-05-25 19:42:35.481932 honeycomb_beeline-3.5.2/beeline/internal.py
+-rw-r--r--   0        0        0        0 2023-05-25 19:42:35.481932 honeycomb_beeline-3.5.2/beeline/middleware/__init__.py
+-rw-r--r--   0        0        0     5977 2023-05-25 19:42:35.481932 honeycomb_beeline-3.5.2/beeline/middleware/awslambda/__init__.py
+-rw-r--r--   0        0        0    10594 2023-05-25 19:42:35.481932 honeycomb_beeline-3.5.2/beeline/middleware/awslambda/test_awslambda.py
+-rw-r--r--   0        0        0      646 2023-05-25 19:42:35.481932 honeycomb_beeline-3.5.2/beeline/middleware/bottle/__init__.py
+-rw-r--r--   0        0        0     1110 2023-05-25 19:42:35.481932 honeycomb_beeline-3.5.2/beeline/middleware/bottle/test_bottle.py
+-rw-r--r--   0        0        0     8208 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/middleware/django/__init__.py
+-rw-r--r--   0        0        0     3534 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/middleware/django/test_django.py
+-rw-r--r--   0        0        0     4611 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/middleware/flask/__init__.py
+-rw-r--r--   0        0        0     2210 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/middleware/flask/test_flask.py
+-rw-r--r--   0        0        0      648 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/middleware/werkzeug/__init__.py
+-rw-r--r--   0        0        0     1114 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/middleware/werkzeug/test_werkzeug.py
+-rw-r--r--   0        0        0     1678 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/patch/__init__.py
+-rw-r--r--   0        0        0      413 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/patch/jinja2.py
+-rw-r--r--   0        0        0     1971 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/patch/requests.py
+-rw-r--r--   0        0        0     1160 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/patch/test_jinja2.py
+-rw-r--r--   0        0        0     4507 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/patch/test_requests.py
+-rw-r--r--   0        0        0     2207 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/patch/test_urllib.py
+-rw-r--r--   0        0        0     1857 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/patch/tornado.py
+-rw-r--r--   0        0        0     2311 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/patch/urllib.py
+-rw-r--r--   0        0        0     3483 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/propagation/__init__.py
+-rw-r--r--   0        0        0      769 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/propagation/default.py
+-rw-r--r--   0        0        0     3682 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/propagation/honeycomb.py
+-rw-r--r--   0        0        0     4349 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/propagation/test_honeycomb.py
+-rw-r--r--   0        0        0     1365 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/propagation/test_propagation.py
+-rw-r--r--   0        0        0     3392 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/propagation/test_w3c.py
+-rw-r--r--   0        0        0     3299 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/propagation/w3c.py
+-rw-r--r--   0        0        0    14634 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/test_async.py
+-rw-r--r--   0        0        0    10573 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/test_beeline.py
+-rw-r--r--   0        0        0      398 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/test_internal.py
+-rw-r--r--   0        0        0     1129 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/test_suite.py
+-rw-r--r--   0        0        0    29567 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/test_trace.py
+-rw-r--r--   0        0        0    15263 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/trace.py
+-rw-r--r--   0        0        0       47 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/beeline/version.py
+-rw-r--r--   0        0        0      805 2023-05-25 19:42:35.485932 honeycomb_beeline-3.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2812 1970-01-01 00:00:00.000000 honeycomb_beeline-3.5.2/setup.py
+-rw-r--r--   0        0        0     2571 1970-01-01 00:00:00.000000 honeycomb_beeline-3.5.2/PKG-INFO
```

### Comparing `honeycomb_beeline-3.5.1/LICENSE` & `honeycomb_beeline-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/README.md` & `honeycomb_beeline-3.5.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Honeycomb Beeline for Python
 
 [![OSS Lifecycle](https://img.shields.io/osslifecycle/honeycombio/beeline-python?color=success)](https://github.com/honeycombio/home/blob/main/honeycomb-oss-lifecycle-and-practices.md)
 [![Build Status](https://circleci.com/gh/honeycombio/beeline-python.svg?style=svg)](https://app.circleci.com/pipelines/github/honeycombio/beeline-python)
 
+**Note**: Honeycomb embraces OpenTelemetry as the effective way to instrument applications. For any new observability efforts, we recommend [instrumenting with OpenTelemetry](https://docs.honeycomb.io/getting-data-in/opentelemetry/python-distro/).
+
 This package makes it easy to instrument your Python web application to send useful events to [Honeycomb](https://honeycomb.io), a service for debugging your software in production.
 
 - [Usage and Examples](https://docs.honeycomb.io/getting-data-in/beelines/beeline-python/)
 - [API Reference](https://honeycombio.github.io/beeline-python/)
 
 ## Compatible with
```

### Comparing `honeycomb_beeline-3.5.1/beeline/__init__.py` & `honeycomb_beeline-3.5.2/beeline/__init__.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/aiotrace.py` & `honeycomb_beeline-3.5.2/beeline/aiotrace.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/internal.py` & `honeycomb_beeline-3.5.2/beeline/internal.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/middleware/awslambda/__init__.py` & `honeycomb_beeline-3.5.2/beeline/middleware/awslambda/__init__.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/middleware/awslambda/test_awslambda.py` & `honeycomb_beeline-3.5.2/beeline/middleware/awslambda/test_awslambda.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/middleware/bottle/__init__.py` & `honeycomb_beeline-3.5.2/beeline/middleware/bottle/__init__.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/middleware/bottle/test_bottle.py` & `honeycomb_beeline-3.5.2/beeline/middleware/bottle/test_bottle.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/middleware/django/__init__.py` & `honeycomb_beeline-3.5.2/beeline/middleware/django/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                     "db.error_detail", beeline.internal.stringify_exception(e))
                 raise
             else:
                 return result
             finally:
                 if vendor in ('postgresql', 'mysql'):
                     beeline.add_context({
-                        "db.last_insert_id": context['cursor'].cursor.lastrowid,
+                        "db.last_insert_id": getattr(context['cursor'].cursor, 'lastrowid', None),
                         "db.rows_affected": context['cursor'].cursor.rowcount,
                     })
 
 
 class HoneyMiddlewareBase(object):
     def __init__(self, get_response):
         self.get_response = get_response
```

### Comparing `honeycomb_beeline-3.5.1/beeline/middleware/django/test_django.py` & `honeycomb_beeline-3.5.2/beeline/middleware/django/test_django.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/middleware/flask/__init__.py` & `honeycomb_beeline-3.5.2/beeline/middleware/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/middleware/flask/test_flask.py` & `honeycomb_beeline-3.5.2/beeline/middleware/flask/test_flask.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/middleware/werkzeug/__init__.py` & `honeycomb_beeline-3.5.2/beeline/middleware/werkzeug/__init__.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/middleware/werkzeug/test_werkzeug.py` & `honeycomb_beeline-3.5.2/beeline/middleware/werkzeug/test_werkzeug.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/middleware/wsgi.py` & `honeycomb_beeline-3.5.2/beeline/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/patch/requests.py` & `honeycomb_beeline-3.5.2/beeline/patch/requests.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/patch/test_jinja2.py` & `honeycomb_beeline-3.5.2/beeline/patch/test_jinja2.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/patch/test_requests.py` & `honeycomb_beeline-3.5.2/beeline/patch/test_requests.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/patch/test_urllib.py` & `honeycomb_beeline-3.5.2/beeline/patch/test_urllib.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/patch/tornado.py` & `honeycomb_beeline-3.5.2/beeline/patch/tornado.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/patch/urllib.py` & `honeycomb_beeline-3.5.2/beeline/patch/urllib.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/propagation/__init__.py` & `honeycomb_beeline-3.5.2/beeline/propagation/__init__.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/propagation/default.py` & `honeycomb_beeline-3.5.2/beeline/propagation/default.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/propagation/honeycomb.py` & `honeycomb_beeline-3.5.2/beeline/propagation/honeycomb.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/propagation/test_honeycomb.py` & `honeycomb_beeline-3.5.2/beeline/propagation/test_honeycomb.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/propagation/test_propagation.py` & `honeycomb_beeline-3.5.2/beeline/propagation/test_propagation.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/propagation/test_w3c.py` & `honeycomb_beeline-3.5.2/beeline/propagation/test_w3c.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/propagation/w3c.py` & `honeycomb_beeline-3.5.2/beeline/propagation/w3c.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/test_async.py` & `honeycomb_beeline-3.5.2/beeline/test_async.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/test_beeline.py` & `honeycomb_beeline-3.5.2/beeline/test_beeline.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/test_suite.py` & `honeycomb_beeline-3.5.2/beeline/test_suite.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/test_trace.py` & `honeycomb_beeline-3.5.2/beeline/test_trace.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/beeline/trace.py` & `honeycomb_beeline-3.5.2/beeline/trace.py`

 * *Files identical despite different names*

### Comparing `honeycomb_beeline-3.5.1/pyproject.toml` & `honeycomb_beeline-3.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "honeycomb-beeline"
-version = "3.5.1" # Update using bump2version
+version = "3.5.2" # Update using bump2version
 description = "Honeycomb library for easy instrumentation"
 authors = ["Honeycomb.io <feedback@honeycomb.io>"]
 license = "Apache-2.0"
 packages = [
     { include = "beeline" }
 ]
 readme = "README.md"
@@ -12,18 +12,18 @@
 repository = "https://github.com/honeycombio/beeline-python"
 
 [tool.poetry.dependencies]
 python = ">=3.7, <4"
 libhoney = "^2.3.0"
 wrapt = "^1.12.1"
 [tool.poetry.dev-dependencies]
-mock = "^5.0.0"
-coverage = "^7.0.5"
+mock = "^5.0.2"
+coverage = "^7.2.5"
 pylint = [{version = "^2.13", python = ">=3.7,<4"}]
 django = [{version = "^3.2", python = ">= 3.7,<4"}]
 tornado = "^6.2"
 pycodestyle = "^2.10.0"
 bump2version = "^1.0.1"
-Flask = "2.2.2"
+Flask = "2.2.5"
 
 [tool.poetry.scripts]
 tests = "beeline.test_suite:run_tests"
```

### Comparing `honeycomb_beeline-3.5.1/setup.py` & `honeycomb_beeline-3.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 ['libhoney>=2.3.0,<3.0.0', 'wrapt>=1.12.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['tests = beeline.test_suite:run_tests']}
 
 setup_kwargs = {
     'name': 'honeycomb-beeline',
-    'version': '3.5.1',
+    'version': '3.5.2',
     'description': 'Honeycomb library for easy instrumentation',
-    'long_description': '# Honeycomb Beeline for Python\n\n[![OSS Lifecycle](https://img.shields.io/osslifecycle/honeycombio/beeline-python?color=success)](https://github.com/honeycombio/home/blob/main/honeycomb-oss-lifecycle-and-practices.md)\n[![Build Status](https://circleci.com/gh/honeycombio/beeline-python.svg?style=svg)](https://app.circleci.com/pipelines/github/honeycombio/beeline-python)\n\nThis package makes it easy to instrument your Python web application to send useful events to [Honeycomb](https://honeycomb.io), a service for debugging your software in production.\n\n- [Usage and Examples](https://docs.honeycomb.io/getting-data-in/beelines/beeline-python/)\n- [API Reference](https://honeycombio.github.io/beeline-python/)\n\n## Compatible with\n\nCurrently, supports Django (>3.2), Flask, Bottle, and Tornado.\n\nCompatible with Python >3.7.\n\n## Updating to 3.3.0\n\nVersion 3.3.0 added support for Environment & Services, which changes sending behavior based on API Key.\n\nIf you are using the [FileTransmission](https://github.com/honeycombio/libhoney-py/blob/main/libhoney/transmission.py#L448) method and setting a false API key - and still working in Classic mode - you must update the key to be 32 characters in length to keep the same behavior.\n\n## Contributions\n\nFeatures, bug fixes and other changes to `beeline-python` are gladly accepted.\n\nIf you add a new test module, be sure and update `beeline.test_suite` to pick up the new tests.\n\nAll contributions will be released under the Apache License 2.0.\n',
+    'long_description': '# Honeycomb Beeline for Python\n\n[![OSS Lifecycle](https://img.shields.io/osslifecycle/honeycombio/beeline-python?color=success)](https://github.com/honeycombio/home/blob/main/honeycomb-oss-lifecycle-and-practices.md)\n[![Build Status](https://circleci.com/gh/honeycombio/beeline-python.svg?style=svg)](https://app.circleci.com/pipelines/github/honeycombio/beeline-python)\n\n**Note**: Honeycomb embraces OpenTelemetry as the effective way to instrument applications. For any new observability efforts, we recommend [instrumenting with OpenTelemetry](https://docs.honeycomb.io/getting-data-in/opentelemetry/python-distro/).\n\nThis package makes it easy to instrument your Python web application to send useful events to [Honeycomb](https://honeycomb.io), a service for debugging your software in production.\n\n- [Usage and Examples](https://docs.honeycomb.io/getting-data-in/beelines/beeline-python/)\n- [API Reference](https://honeycombio.github.io/beeline-python/)\n\n## Compatible with\n\nCurrently, supports Django (>3.2), Flask, Bottle, and Tornado.\n\nCompatible with Python >3.7.\n\n## Updating to 3.3.0\n\nVersion 3.3.0 added support for Environment & Services, which changes sending behavior based on API Key.\n\nIf you are using the [FileTransmission](https://github.com/honeycombio/libhoney-py/blob/main/libhoney/transmission.py#L448) method and setting a false API key - and still working in Classic mode - you must update the key to be 32 characters in length to keep the same behavior.\n\n## Contributions\n\nFeatures, bug fixes and other changes to `beeline-python` are gladly accepted.\n\nIf you add a new test module, be sure and update `beeline.test_suite` to pick up the new tests.\n\nAll contributions will be released under the Apache License 2.0.\n',
     'author': 'Honeycomb.io',
     'author_email': 'feedback@honeycomb.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/honeycombio/beeline-python',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `honeycomb_beeline-3.5.1/PKG-INFO` & `honeycomb_beeline-3.5.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeycomb-beeline
-Version: 3.5.1
+Version: 3.5.2
 Summary: Honeycomb library for easy instrumentation
 Home-page: https://github.com/honeycombio/beeline-python
 License: Apache-2.0
 Author: Honeycomb.io
 Author-email: feedback@honeycomb.io
 Requires-Python: >=3.7,<4
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,14 +20,16 @@
 Description-Content-Type: text/markdown
 
 # Honeycomb Beeline for Python
 
 [![OSS Lifecycle](https://img.shields.io/osslifecycle/honeycombio/beeline-python?color=success)](https://github.com/honeycombio/home/blob/main/honeycomb-oss-lifecycle-and-practices.md)
 [![Build Status](https://circleci.com/gh/honeycombio/beeline-python.svg?style=svg)](https://app.circleci.com/pipelines/github/honeycombio/beeline-python)
 
+**Note**: Honeycomb embraces OpenTelemetry as the effective way to instrument applications. For any new observability efforts, we recommend [instrumenting with OpenTelemetry](https://docs.honeycomb.io/getting-data-in/opentelemetry/python-distro/).
+
 This package makes it easy to instrument your Python web application to send useful events to [Honeycomb](https://honeycomb.io), a service for debugging your software in production.
 
 - [Usage and Examples](https://docs.honeycomb.io/getting-data-in/beelines/beeline-python/)
 - [API Reference](https://honeycombio.github.io/beeline-python/)
 
 ## Compatible with
```

