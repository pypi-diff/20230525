# Comparing `tmp/cache_decorator-2.1.8.tar.gz` & `tmp/cache_decorator-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cache_decorator-2.1.8.tar", last modified: Fri Jun 24 20:07:37 2022, max compression
+gzip compressed data, was "cache_decorator-2.1.9.tar", last modified: Fri Aug  5 07:26:09 2022, max compression
```

## Comparing `cache_decorator-2.1.8.tar` & `cache_decorator-2.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 zommiommy  (1000) zommiommy  (1001)        0 2022-06-24 20:07:37.907932 cache_decorator-2.1.8/
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     1072 2021-11-09 13:58:38.000000 cache_decorator-2.1.8/LICENSE
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)        0 2021-11-09 13:58:38.000000 cache_decorator-2.1.8/MANIFEST.in
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)    17908 2022-06-24 20:07:37.907932 cache_decorator-2.1.8/PKG-INFO
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)    17462 2022-05-31 19:20:23.000000 cache_decorator-2.1.8/README.rst
-drwxr-xr-x   0 zommiommy  (1000) zommiommy  (1001)        0 2022-06-24 20:07:37.901265 cache_decorator-2.1.8/cache_decorator/
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)      425 2021-11-09 13:58:38.000000 cache_decorator-2.1.8/cache_decorator/__init__.py
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)       72 2022-06-24 20:06:59.000000 cache_decorator-2.1.8/cache_decorator/__version__.py
-drwxr-xr-x   0 zommiommy  (1000) zommiommy  (1001)        0 2022-06-24 20:07:37.904599 cache_decorator-2.1.8/cache_decorator/backends/
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)      217 2021-11-09 13:58:38.000000 cache_decorator-2.1.8/cache_decorator/backends/__init__.py
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     2913 2022-05-24 14:04:29.000000 cache_decorator-2.1.8/cache_decorator/backends/backend.py
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     2331 2022-05-24 14:04:29.000000 cache_decorator-2.1.8/cache_decorator/backends/backend_template.py
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     1086 2022-05-24 14:04:29.000000 cache_decorator-2.1.8/cache_decorator/backends/compress_json_backend.py
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     1135 2022-05-24 14:04:29.000000 cache_decorator-2.1.8/cache_decorator/backends/compress_pickle_backend.py
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)      524 2021-11-09 13:58:38.000000 cache_decorator-2.1.8/cache_decorator/backends/exceptions.py
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     1584 2022-05-24 14:04:29.000000 cache_decorator-2.1.8/cache_decorator/backends/json_backend.py
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     2346 2022-05-24 14:04:29.000000 cache_decorator-2.1.8/cache_decorator/backends/keras_model_backend.py
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     4092 2022-05-24 14:04:29.000000 cache_decorator-2.1.8/cache_decorator/backends/numpy_backend.py
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     6204 2022-06-24 20:02:08.000000 cache_decorator-2.1.8/cache_decorator/backends/pandas_csv_backend.py
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     3569 2022-05-24 14:04:29.000000 cache_decorator-2.1.8/cache_decorator/backends/pandas_embedding_backend.py
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     1080 2022-05-24 14:04:29.000000 cache_decorator-2.1.8/cache_decorator/backends/pickle_backend.py
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     1573 2022-05-24 14:04:29.000000 cache_decorator-2.1.8/cache_decorator/backends/txt_backend.py
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)    33186 2022-05-31 19:50:12.000000 cache_decorator-2.1.8/cache_decorator/cache.py
-drwxr-xr-x   0 zommiommy  (1000) zommiommy  (1001)        0 2022-06-24 20:07:37.904599 cache_decorator-2.1.8/cache_decorator/utils/
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)      615 2022-05-31 19:49:28.000000 cache_decorator-2.1.8/cache_decorator/utils/__init__.py
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     2399 2022-05-27 10:39:06.000000 cache_decorator-2.1.8/cache_decorator/utils/get_format_groups.py
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)      658 2022-05-31 17:25:41.000000 cache_decorator-2.1.8/cache_decorator/utils/get_params.py
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)      730 2021-11-09 13:58:38.000000 cache_decorator-2.1.8/cache_decorator/utils/parse_time.py
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)       93 2021-11-09 13:58:38.000000 cache_decorator-2.1.8/cache_decorator/utils/random_string.py
-drwxr-xr-x   0 zommiommy  (1000) zommiommy  (1001)        0 2022-06-24 20:07:37.904599 cache_decorator-2.1.8/cache_decorator.egg-info/
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)    17908 2022-06-24 20:07:37.000000 cache_decorator-2.1.8/cache_decorator.egg-info/PKG-INFO
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     1078 2022-06-24 20:07:37.000000 cache_decorator-2.1.8/cache_decorator.egg-info/SOURCES.txt
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)        1 2022-06-24 20:07:37.000000 cache_decorator-2.1.8/cache_decorator.egg-info/dependency_links.txt
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)       91 2022-06-24 20:07:37.000000 cache_decorator-2.1.8/cache_decorator.egg-info/requires.txt
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)       16 2022-06-24 20:07:37.000000 cache_decorator-2.1.8/cache_decorator.egg-info/top_level.txt
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)       38 2022-06-24 20:07:37.907932 cache_decorator-2.1.8/setup.cfg
--rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     2099 2022-06-21 08:16:03.000000 cache_decorator-2.1.8/setup.py
+drwxr-xr-x   0 zommiommy  (1000) zommiommy  (1001)        0 2022-08-05 07:26:09.796667 cache_decorator-2.1.9/
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     1072 2021-11-09 13:58:38.000000 cache_decorator-2.1.9/LICENSE
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)        0 2021-11-09 13:58:38.000000 cache_decorator-2.1.9/MANIFEST.in
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)    17908 2022-08-05 07:26:09.793333 cache_decorator-2.1.9/PKG-INFO
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)    17462 2022-05-31 19:20:23.000000 cache_decorator-2.1.9/README.rst
+drwxr-xr-x   0 zommiommy  (1000) zommiommy  (1001)        0 2022-08-05 07:26:09.793333 cache_decorator-2.1.9/cache_decorator/
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)      425 2021-11-09 13:58:38.000000 cache_decorator-2.1.9/cache_decorator/__init__.py
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)       72 2022-08-05 07:25:58.000000 cache_decorator-2.1.9/cache_decorator/__version__.py
+drwxr-xr-x   0 zommiommy  (1000) zommiommy  (1001)        0 2022-08-05 07:26:09.793333 cache_decorator-2.1.9/cache_decorator/backends/
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)      217 2021-11-09 13:58:38.000000 cache_decorator-2.1.9/cache_decorator/backends/__init__.py
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     2913 2022-05-24 14:04:29.000000 cache_decorator-2.1.9/cache_decorator/backends/backend.py
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     2331 2022-05-24 14:04:29.000000 cache_decorator-2.1.9/cache_decorator/backends/backend_template.py
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     1086 2022-05-24 14:04:29.000000 cache_decorator-2.1.9/cache_decorator/backends/compress_json_backend.py
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     1135 2022-05-24 14:04:29.000000 cache_decorator-2.1.9/cache_decorator/backends/compress_pickle_backend.py
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)      524 2021-11-09 13:58:38.000000 cache_decorator-2.1.9/cache_decorator/backends/exceptions.py
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     1584 2022-05-24 14:04:29.000000 cache_decorator-2.1.9/cache_decorator/backends/json_backend.py
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     2346 2022-05-24 14:04:29.000000 cache_decorator-2.1.9/cache_decorator/backends/keras_model_backend.py
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     4092 2022-05-24 14:04:29.000000 cache_decorator-2.1.9/cache_decorator/backends/numpy_backend.py
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     6076 2022-08-05 07:23:48.000000 cache_decorator-2.1.9/cache_decorator/backends/pandas_csv_backend.py
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     3569 2022-05-24 14:04:29.000000 cache_decorator-2.1.9/cache_decorator/backends/pandas_embedding_backend.py
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     1080 2022-05-24 14:04:29.000000 cache_decorator-2.1.9/cache_decorator/backends/pickle_backend.py
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     1573 2022-05-24 14:04:29.000000 cache_decorator-2.1.9/cache_decorator/backends/txt_backend.py
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)    33186 2022-05-31 19:50:12.000000 cache_decorator-2.1.9/cache_decorator/cache.py
+drwxr-xr-x   0 zommiommy  (1000) zommiommy  (1001)        0 2022-08-05 07:26:09.793333 cache_decorator-2.1.9/cache_decorator/utils/
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)      615 2022-05-31 19:49:28.000000 cache_decorator-2.1.9/cache_decorator/utils/__init__.py
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     2399 2022-05-27 10:39:06.000000 cache_decorator-2.1.9/cache_decorator/utils/get_format_groups.py
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)      658 2022-05-31 17:25:41.000000 cache_decorator-2.1.9/cache_decorator/utils/get_params.py
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)      730 2021-11-09 13:58:38.000000 cache_decorator-2.1.9/cache_decorator/utils/parse_time.py
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)       93 2021-11-09 13:58:38.000000 cache_decorator-2.1.9/cache_decorator/utils/random_string.py
+drwxr-xr-x   0 zommiommy  (1000) zommiommy  (1001)        0 2022-08-05 07:26:09.793333 cache_decorator-2.1.9/cache_decorator.egg-info/
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)    17908 2022-08-05 07:26:09.000000 cache_decorator-2.1.9/cache_decorator.egg-info/PKG-INFO
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     1078 2022-08-05 07:26:09.000000 cache_decorator-2.1.9/cache_decorator.egg-info/SOURCES.txt
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)        1 2022-08-05 07:26:09.000000 cache_decorator-2.1.9/cache_decorator.egg-info/dependency_links.txt
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)       91 2022-08-05 07:26:09.000000 cache_decorator-2.1.9/cache_decorator.egg-info/requires.txt
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)       16 2022-08-05 07:26:09.000000 cache_decorator-2.1.9/cache_decorator.egg-info/top_level.txt
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)       38 2022-08-05 07:26:09.796667 cache_decorator-2.1.9/setup.cfg
+-rw-r--r--   0 zommiommy  (1000) zommiommy  (1001)     2099 2022-06-21 08:16:03.000000 cache_decorator-2.1.9/setup.py
```

### Comparing `cache_decorator-2.1.8/LICENSE` & `cache_decorator-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cache_decorator-2.1.8/PKG-INFO` & `cache_decorator-2.1.9/cache_decorator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cache_decorator
-Version: 2.1.8
+Name: cache-decorator
+Version: 2.1.9
 Summary: a simple decorator to cache the results of computationally heavy functions
 Home-page: https://github.com/zommiommy/cache_decorator
 Author: Tommaso Fontana
 Author-email: tommaso.fontana.96@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cache_decorator-2.1.8/README.rst` & `cache_decorator-2.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `cache_decorator-2.1.8/cache_decorator/backends/backend.py` & `cache_decorator-2.1.9/cache_decorator/backends/backend.py`

 * *Files identical despite different names*

### Comparing `cache_decorator-2.1.8/cache_decorator/backends/backend_template.py` & `cache_decorator-2.1.9/cache_decorator/backends/backend_template.py`

 * *Files identical despite different names*

### Comparing `cache_decorator-2.1.8/cache_decorator/backends/compress_json_backend.py` & `cache_decorator-2.1.9/cache_decorator/backends/compress_json_backend.py`

 * *Files identical despite different names*

### Comparing `cache_decorator-2.1.8/cache_decorator/backends/compress_pickle_backend.py` & `cache_decorator-2.1.9/cache_decorator/backends/compress_pickle_backend.py`

 * *Files identical despite different names*

### Comparing `cache_decorator-2.1.8/cache_decorator/backends/exceptions.py` & `cache_decorator-2.1.9/cache_decorator/backends/exceptions.py`

 * *Files identical despite different names*

### Comparing `cache_decorator-2.1.8/cache_decorator/backends/json_backend.py` & `cache_decorator-2.1.9/cache_decorator/backends/json_backend.py`

 * *Files identical despite different names*

### Comparing `cache_decorator-2.1.8/cache_decorator/backends/keras_model_backend.py` & `cache_decorator-2.1.9/cache_decorator/backends/keras_model_backend.py`

 * *Files identical despite different names*

### Comparing `cache_decorator-2.1.8/cache_decorator/backends/numpy_backend.py` & `cache_decorator-2.1.9/cache_decorator/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `cache_decorator-2.1.8/cache_decorator/backends/pandas_csv_backend.py` & `cache_decorator-2.1.9/cache_decorator/backends/pandas_csv_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,17 +92,14 @@
                 if not is_consistent(obj_to_serialize[column]):
                     warnings.warn("The column '{}'".format(
                         column) + common_message)
 
             if not is_consistent(obj_to_serialize.index):
                 warnings.warn("The index" + common_message)
 
-            if not is_consistent(obj_to_serialize.columns):
-                warnings.warn("The column names" + common_message)
-
             obj_to_serialize.to_csv(
                 path,
                 sep=self.SUPPORTED_EXTENSIONS[
                     next(
                         x
                         for x in self.SUPPORTED_EXTENSIONS
                         if path.endswith(x)
```

### Comparing `cache_decorator-2.1.8/cache_decorator/backends/pandas_embedding_backend.py` & `cache_decorator-2.1.9/cache_decorator/backends/pandas_embedding_backend.py`

 * *Files identical despite different names*

### Comparing `cache_decorator-2.1.8/cache_decorator/backends/pickle_backend.py` & `cache_decorator-2.1.9/cache_decorator/backends/pickle_backend.py`

 * *Files identical despite different names*

### Comparing `cache_decorator-2.1.8/cache_decorator/backends/txt_backend.py` & `cache_decorator-2.1.9/cache_decorator/backends/txt_backend.py`

 * *Files identical despite different names*

### Comparing `cache_decorator-2.1.8/cache_decorator/cache.py` & `cache_decorator-2.1.9/cache_decorator/cache.py`

 * *Files identical despite different names*

### Comparing `cache_decorator-2.1.8/cache_decorator/utils/__init__.py` & `cache_decorator-2.1.9/cache_decorator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cache_decorator-2.1.8/cache_decorator/utils/get_format_groups.py` & `cache_decorator-2.1.9/cache_decorator/utils/get_format_groups.py`

 * *Files identical despite different names*

### Comparing `cache_decorator-2.1.8/cache_decorator/utils/get_params.py` & `cache_decorator-2.1.9/cache_decorator/utils/get_params.py`

 * *Files identical despite different names*

### Comparing `cache_decorator-2.1.8/cache_decorator/utils/parse_time.py` & `cache_decorator-2.1.9/cache_decorator/utils/parse_time.py`

 * *Files identical despite different names*

### Comparing `cache_decorator-2.1.8/cache_decorator.egg-info/PKG-INFO` & `cache_decorator-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cache-decorator
-Version: 2.1.8
+Name: cache_decorator
+Version: 2.1.9
 Summary: a simple decorator to cache the results of computationally heavy functions
 Home-page: https://github.com/zommiommy/cache_decorator
 Author: Tommaso Fontana
 Author-email: tommaso.fontana.96@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cache_decorator-2.1.8/cache_decorator.egg-info/SOURCES.txt` & `cache_decorator-2.1.9/cache_decorator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cache_decorator-2.1.8/setup.py` & `cache_decorator-2.1.9/setup.py`

 * *Files identical despite different names*

