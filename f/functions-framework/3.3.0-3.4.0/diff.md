# Comparing `tmp/functions-framework-3.3.0.tar.gz` & `tmp/functions-framework-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "functions-framework-3.3.0.tar", last modified: Wed Dec 21 15:37:48 2022, max compression
+gzip compressed data, was "functions-framework-3.4.0.tar", last modified: Thu May 25 21:18:38 2023, max compression
```

## Comparing `functions-framework-3.3.0.tar` & `functions-framework-3.4.0.tar`

### file list

```diff
@@ -1,41 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 15:37:48.543549 functions-framework-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-12-21 15:37:37.000000 functions-framework-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15954 2022-12-21 15:37:48.543549 functions-framework-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14975 2022-12-21 15:37:37.000000 functions-framework-3.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      302 2022-12-21 15:37:48.547549 functions-framework-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2022-12-21 15:37:37.000000 functions-framework-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 15:37:48.539549 functions-framework-3.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 15:37:48.543549 functions-framework-3.3.0/src/functions_framework/
--rw-r--r--   0 runner    (1001) docker     (123)    13364 2022-12-21 15:37:37.000000 functions-framework-3.3.0/src/functions_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2022-12-21 15:37:37.000000 functions-framework-3.3.0/src/functions_framework/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2022-12-21 15:37:37.000000 functions-framework-3.3.0/src/functions_framework/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2022-12-21 15:37:37.000000 functions-framework-3.3.0/src/functions_framework/_function_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 15:37:48.543549 functions-framework-3.3.0/src/functions_framework/_http/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2022-12-21 15:37:37.000000 functions-framework-3.3.0/src/functions_framework/_http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2022-12-21 15:37:37.000000 functions-framework-3.3.0/src/functions_framework/_http/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2022-12-21 15:37:37.000000 functions-framework-3.3.0/src/functions_framework/_http/gunicorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2022-12-21 15:37:37.000000 functions-framework-3.3.0/src/functions_framework/_typed_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2022-12-21 15:37:37.000000 functions-framework-3.3.0/src/functions_framework/background_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    14588 2022-12-21 15:37:37.000000 functions-framework-3.3.0/src/functions_framework/event_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2022-12-21 15:37:37.000000 functions-framework-3.3.0/src/functions_framework/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 15:37:48.543549 functions-framework-3.3.0/src/functions_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15954 2022-12-21 15:37:48.000000 functions-framework-3.3.0/src/functions_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2022-12-21 15:37:48.000000 functions-framework-3.3.0/src/functions_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 15:37:48.000000 functions-framework-3.3.0/src/functions_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      275 2022-12-21 15:37:48.000000 functions-framework-3.3.0/src/functions_framework.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-21 15:37:48.000000 functions-framework-3.3.0/src/functions_framework.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-21 15:37:48.000000 functions-framework-3.3.0/src/functions_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2022-12-21 15:37:48.000000 functions-framework-3.3.0/src/functions_framework.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 15:37:48.543549 functions-framework-3.3.0/src/google/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2022-12-21 15:37:37.000000 functions-framework-3.3.0/src/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 15:37:48.543549 functions-framework-3.3.0/src/google/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2022-12-21 15:37:37.000000 functions-framework-3.3.0/src/google/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 15:37:48.543549 functions-framework-3.3.0/src/google/cloud/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2022-12-21 15:37:37.000000 functions-framework-3.3.0/src/google/cloud/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2022-12-21 15:37:37.000000 functions-framework-3.3.0/src/google/cloud/functions/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 15:37:48.543549 functions-framework-3.3.0/src/google/cloud/functions_v1/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2022-12-21 15:37:37.000000 functions-framework-3.3.0/src/google/cloud/functions_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2022-12-21 15:37:37.000000 functions-framework-3.3.0/src/google/cloud/functions_v1/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 15:37:48.543549 functions-framework-3.3.0/src/google/cloud/functions_v1beta2/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2022-12-21 15:37:37.000000 functions-framework-3.3.0/src/google/cloud/functions_v1beta2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2022-12-21 15:37:37.000000 functions-framework-3.3.0/src/google/cloud/functions_v1beta2/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:18:38.926162 functions-framework-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-25 21:18:27.000000 functions-framework-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-05-25 21:18:38.930162 functions-framework-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-05-25 21:18:27.000000 functions-framework-3.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-25 21:18:38.930162 functions-framework-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-25 21:18:27.000000 functions-framework-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:18:38.918162 functions-framework-3.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:18:38.922162 functions-framework-3.4.0/src/functions_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)    13510 2023-05-25 21:18:27.000000 functions-framework-3.4.0/src/functions_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-25 21:18:27.000000 functions-framework-3.4.0/src/functions_framework/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-25 21:18:27.000000 functions-framework-3.4.0/src/functions_framework/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-25 21:18:27.000000 functions-framework-3.4.0/src/functions_framework/_function_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:18:38.922162 functions-framework-3.4.0/src/functions_framework/_http/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-25 21:18:27.000000 functions-framework-3.4.0/src/functions_framework/_http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-25 21:18:27.000000 functions-framework-3.4.0/src/functions_framework/_http/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-25 21:18:27.000000 functions-framework-3.4.0/src/functions_framework/_http/gunicorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-05-25 21:18:27.000000 functions-framework-3.4.0/src/functions_framework/_typed_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-25 21:18:27.000000 functions-framework-3.4.0/src/functions_framework/background_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14588 2023-05-25 21:18:27.000000 functions-framework-3.4.0/src/functions_framework/event_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 21:18:27.000000 functions-framework-3.4.0/src/functions_framework/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:18:38.922162 functions-framework-3.4.0/src/functions_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-05-25 21:18:38.000000 functions-framework-3.4.0/src/functions_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-25 21:18:38.000000 functions-framework-3.4.0/src/functions_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:18:38.000000 functions-framework-3.4.0/src/functions_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-25 21:18:38.000000 functions-framework-3.4.0/src/functions_framework.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 21:18:38.000000 functions-framework-3.4.0/src/functions_framework.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-25 21:18:38.000000 functions-framework-3.4.0/src/functions_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 21:18:38.000000 functions-framework-3.4.0/src/functions_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:18:38.922162 functions-framework-3.4.0/src/google/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-25 21:18:27.000000 functions-framework-3.4.0/src/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:18:38.922162 functions-framework-3.4.0/src/google/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-25 21:18:27.000000 functions-framework-3.4.0/src/google/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:18:38.922162 functions-framework-3.4.0/src/google/cloud/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 21:18:27.000000 functions-framework-3.4.0/src/google/cloud/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-25 21:18:27.000000 functions-framework-3.4.0/src/google/cloud/functions/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:18:38.926162 functions-framework-3.4.0/src/google/cloud/functions_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 21:18:27.000000 functions-framework-3.4.0/src/google/cloud/functions_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-25 21:18:27.000000 functions-framework-3.4.0/src/google/cloud/functions_v1/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:18:38.926162 functions-framework-3.4.0/src/google/cloud/functions_v1beta2/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 21:18:27.000000 functions-framework-3.4.0/src/google/cloud/functions_v1beta2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-25 21:18:27.000000 functions-framework-3.4.0/src/google/cloud/functions_v1beta2/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:18:38.926162 functions-framework-3.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-25 21:18:27.000000 functions-framework-3.4.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-05-25 21:18:27.000000 functions-framework-3.4.0/tests/test_cloud_event_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22960 2023-05-25 21:18:27.000000 functions-framework-3.4.0/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-25 21:18:27.000000 functions-framework-3.4.0/tests/test_decorator_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-25 21:18:27.000000 functions-framework-3.4.0/tests/test_function_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18868 2023-05-25 21:18:27.000000 functions-framework-3.4.0/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-25 21:18:27.000000 functions-framework-3.4.0/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-25 21:18:27.000000 functions-framework-3.4.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-25 21:18:27.000000 functions-framework-3.4.0/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-25 21:18:27.000000 functions-framework-3.4.0/tests/test_typed_event_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-25 21:18:27.000000 functions-framework-3.4.0/tests/test_view_functions.py
```

### Comparing `functions-framework-3.3.0/LICENSE` & `functions-framework-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `functions-framework-3.3.0/PKG-INFO` & `functions-framework-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functions-framework
-Version: 3.3.0
+Version: 3.4.0
 Summary: An open source FaaS (Function as a service) framework for writing portable Python functions -- brought to you by the Google Cloud Functions team.
 Home-page: https://github.com/googlecloudplatform/functions-framework-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 Keywords: functions-framework
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `functions-framework-3.3.0/README.md` & `functions-framework-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `functions-framework-3.3.0/setup.py` & `functions-framework-3.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="functions-framework",
-    version="3.3.0",
+    version="3.4.0",
     description="An open source FaaS (Function as a service) framework for writing portable Python functions -- brought to you by the Google Cloud Functions team.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/googlecloudplatform/functions-framework-python",
     author="Google LLC",
     author_email="googleapis-packages@google.com",
     classifiers=[
```

### Comparing `functions-framework-3.3.0/src/functions_framework/__init__.py` & `functions-framework-3.4.0/src/functions_framework/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,18 +290,21 @@
             )
         )
 
 
 def read_request(response):
     """
     Force the framework to read the entire request before responding, to avoid
-    connection errors when returning prematurely.
+    connection errors when returning prematurely. Skipped on streaming responses
+    as these may continue to operate on the request after they are returned.
     """
 
-    flask.request.get_data()
+    if not response.is_streamed:
+        flask.request.get_data()
+
     return response
 
 
 def crash_handler(e):
     """
     Return crash header to allow logging 'crash' message in logs.
     """
```

### Comparing `functions-framework-3.3.0/src/functions_framework/__main__.py` & `functions-framework-3.4.0/src/functions_framework/__main__.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.3.0/src/functions_framework/_cli.py` & `functions-framework-3.4.0/src/functions_framework/_cli.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.3.0/src/functions_framework/_function_registry.py` & `functions-framework-3.4.0/src/functions_framework/_function_registry.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.3.0/src/functions_framework/_http/__init__.py` & `functions-framework-3.4.0/src/functions_framework/_http/__init__.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.3.0/src/functions_framework/_http/flask.py` & `functions-framework-3.4.0/src/functions_framework/_http/flask.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.3.0/src/functions_framework/_http/gunicorn.py` & `functions-framework-3.4.0/src/functions_framework/_http/gunicorn.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.3.0/src/functions_framework/_typed_event.py` & `functions-framework-3.4.0/src/functions_framework/_typed_event.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.3.0/src/functions_framework/background_event.py` & `functions-framework-3.4.0/src/functions_framework/background_event.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.3.0/src/functions_framework/event_conversion.py` & `functions-framework-3.4.0/src/functions_framework/event_conversion.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.3.0/src/functions_framework/exceptions.py` & `functions-framework-3.4.0/src/functions_framework/exceptions.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.3.0/src/functions_framework.egg-info/PKG-INFO` & `functions-framework-3.4.0/src/functions_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functions-framework
-Version: 3.3.0
+Version: 3.4.0
 Summary: An open source FaaS (Function as a service) framework for writing portable Python functions -- brought to you by the Google Cloud Functions team.
 Home-page: https://github.com/googlecloudplatform/functions-framework-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 Keywords: functions-framework
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `functions-framework-3.3.0/src/functions_framework.egg-info/SOURCES.txt` & `functions-framework-3.4.0/src/functions_framework.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -23,8 +23,19 @@
 src/google/__init__.py
 src/google/cloud/__init__.py
 src/google/cloud/functions/__init__.py
 src/google/cloud/functions/context.py
 src/google/cloud/functions_v1/__init__.py
 src/google/cloud/functions_v1/context.py
 src/google/cloud/functions_v1beta2/__init__.py
-src/google/cloud/functions_v1beta2/context.py
+src/google/cloud/functions_v1beta2/context.py
+tests/test_cli.py
+tests/test_cloud_event_functions.py
+tests/test_convert.py
+tests/test_decorator_functions.py
+tests/test_function_registry.py
+tests/test_functions.py
+tests/test_http.py
+tests/test_main.py
+tests/test_samples.py
+tests/test_typed_event_functions.py
+tests/test_view_functions.py
```

### Comparing `functions-framework-3.3.0/src/google/__init__.py` & `functions-framework-3.4.0/src/google/__init__.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.3.0/src/google/cloud/__init__.py` & `functions-framework-3.4.0/src/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.3.0/src/google/cloud/functions/__init__.py` & `functions-framework-3.4.0/src/google/cloud/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.3.0/src/google/cloud/functions/context.py` & `functions-framework-3.4.0/src/google/cloud/functions/context.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.3.0/src/google/cloud/functions_v1/__init__.py` & `functions-framework-3.4.0/src/google/cloud/functions_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.3.0/src/google/cloud/functions_v1/context.py` & `functions-framework-3.4.0/src/google/cloud/functions_v1/context.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.3.0/src/google/cloud/functions_v1beta2/__init__.py` & `functions-framework-3.4.0/src/google/cloud/functions_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `functions-framework-3.3.0/src/google/cloud/functions_v1beta2/context.py` & `functions-framework-3.4.0/src/google/cloud/functions_v1beta2/context.py`

 * *Files identical despite different names*

