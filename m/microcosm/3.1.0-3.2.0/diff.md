# Comparing `tmp/microcosm-3.1.0.tar.gz` & `tmp/microcosm-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/microcosm-3.1.0.tar", last modified: Wed Oct  5 12:49:21 2022, max compression
+gzip compressed data, was "dist/microcosm-3.2.0.tar", last modified: Thu May 25 09:17:46 2023, max compression
```

## Comparing `microcosm-3.1.0.tar` & `microcosm-3.2.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-05 12:49:21.000000 microcosm-3.1.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10273 2022-10-05 12:46:28.000000 microcosm-3.1.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-10-05 12:46:28.000000 microcosm-3.1.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5464 2022-10-05 12:49:21.000000 microcosm-3.1.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5046 2022-10-05 12:46:28.000000 microcosm-3.1.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-05 12:49:21.000000 microcosm-3.1.0/microcosm/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      450 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2162 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/caching.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-05 12:49:21.000000 microcosm-3.1.0/microcosm/config/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/config/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      512 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/config/api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6309 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/config/model.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       90 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/config/sentinel.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      704 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/config/types.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1224 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/config/validation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      732 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/decorators.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      595 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/errors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      227 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/example.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2144 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/hooks.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-05 12:49:21.000000 microcosm-3.1.0/microcosm/loaders/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      976 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/loaders/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3776 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/loaders/compose.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1676 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/loaders/environment.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1223 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/loaders/keys.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1130 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/loaders/settings.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1863 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/metadata.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6001 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/object_graph.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2861 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/opaque.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      877 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/profile.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2882 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/registry.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-05 12:49:21.000000 microcosm-3.1.0/microcosm/scoping/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      231 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/scoping/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      351 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/scoping/decorators.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3021 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/scoping/factories.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      312 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/scoping/object_graph.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2071 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/scoping/proxies.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      687 2022-10-05 12:46:28.000000 microcosm-3.1.0/microcosm/typing.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-05 12:49:21.000000 microcosm-3.1.0/microcosm.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5464 2022-10-05 12:49:21.000000 microcosm-3.1.0/microcosm.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1047 2022-10-05 12:49:21.000000 microcosm-3.1.0/microcosm.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-10-05 12:49:21.000000 microcosm-3.1.0/microcosm.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      117 2022-10-05 12:49:21.000000 microcosm-3.1.0/microcosm.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-10-05 12:49:21.000000 microcosm-3.1.0/microcosm.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      158 2022-10-05 12:49:21.000000 microcosm-3.1.0/microcosm.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-10-05 12:49:21.000000 microcosm-3.1.0/microcosm.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      731 2022-10-05 12:49:21.000000 microcosm-3.1.0/setup.cfg
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1397 2022-10-05 12:46:28.000000 microcosm-3.1.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-25 09:17:46.000000 microcosm-3.2.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10273 2023-05-25 09:14:07.000000 microcosm-3.2.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-25 09:14:07.000000 microcosm-3.2.0/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5464 2023-05-25 09:17:46.000000 microcosm-3.2.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5046 2023-05-25 09:14:07.000000 microcosm-3.2.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-25 09:17:46.000000 microcosm-3.2.0/microcosm/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      450 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2162 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/caching.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-25 09:17:46.000000 microcosm-3.2.0/microcosm/config/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/config/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      512 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/config/api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6309 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/config/model.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       90 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/config/sentinel.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      704 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/config/types.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1224 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/config/validation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      732 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/decorators.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      595 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/errors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      227 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/example.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2144 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/hooks.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-25 09:17:46.000000 microcosm-3.2.0/microcosm/loaders/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      976 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/loaders/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3776 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/loaders/compose.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1676 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/loaders/environment.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1223 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/loaders/keys.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1130 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/loaders/settings.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1863 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/metadata.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6001 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/object_graph.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2662 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/opaque.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      877 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/profile.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2882 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/registry.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-25 09:17:46.000000 microcosm-3.2.0/microcosm/scoping/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      231 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/scoping/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      351 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/scoping/decorators.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3021 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/scoping/factories.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      312 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/scoping/object_graph.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2071 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/scoping/proxies.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      687 2023-05-25 09:14:07.000000 microcosm-3.2.0/microcosm/typing.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-25 09:17:46.000000 microcosm-3.2.0/microcosm.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5464 2023-05-25 09:17:46.000000 microcosm-3.2.0/microcosm.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1047 2023-05-25 09:17:46.000000 microcosm-3.2.0/microcosm.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-25 09:17:46.000000 microcosm-3.2.0/microcosm.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      117 2023-05-25 09:17:46.000000 microcosm-3.2.0/microcosm.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-25 09:17:46.000000 microcosm-3.2.0/microcosm.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      158 2023-05-25 09:17:46.000000 microcosm-3.2.0/microcosm.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-05-25 09:17:46.000000 microcosm-3.2.0/microcosm.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      731 2023-05-25 09:17:46.000000 microcosm-3.2.0/setup.cfg
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1397 2023-05-25 09:14:07.000000 microcosm-3.2.0/setup.py
```

### Comparing `microcosm-3.1.0/LICENSE` & `microcosm-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/PKG-INFO` & `microcosm-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcosm
-Version: 3.1.0
+Version: 3.2.0
 Summary: Microcosm - Simple microservice configuration
 Home-page: https://github.com/globality-corp/microcosm
 Author: Globality Engineering
 Author-email: engineering@globality.com
 License: UNKNOWN
 Keywords: microcosm
 Platform: UNKNOWN
```

### Comparing `microcosm-3.1.0/README.md` & `microcosm-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/caching.py` & `microcosm-3.2.0/microcosm/caching.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/config/api.py` & `microcosm-3.2.0/microcosm/config/api.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/config/model.py` & `microcosm-3.2.0/microcosm/config/model.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/config/types.py` & `microcosm-3.2.0/microcosm/config/types.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/config/validation.py` & `microcosm-3.2.0/microcosm/config/validation.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/decorators.py` & `microcosm-3.2.0/microcosm/decorators.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/errors.py` & `microcosm-3.2.0/microcosm/errors.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/hooks.py` & `microcosm-3.2.0/microcosm/hooks.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/loaders/__init__.py` & `microcosm-3.2.0/microcosm/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/loaders/compose.py` & `microcosm-3.2.0/microcosm/loaders/compose.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/loaders/environment.py` & `microcosm-3.2.0/microcosm/loaders/environment.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/loaders/keys.py` & `microcosm-3.2.0/microcosm/loaders/keys.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/loaders/settings.py` & `microcosm-3.2.0/microcosm/loaders/settings.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/metadata.py` & `microcosm-3.2.0/microcosm/metadata.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/object_graph.py` & `microcosm-3.2.0/microcosm/object_graph.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/opaque.py` & `microcosm-3.2.0/microcosm/opaque.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,41 +15,31 @@
  -  An outbound web request might insert opaque values as HTTP headers
 
 Combining opaque data across an entire fleet of services allows for consistent tracing and
 easier debugging of distributed operations.
 
 """
 from collections.abc import MutableMapping
-from contextlib import ContextDecorator, ExitStack
+from contextlib import contextmanager
+from contextvars import ContextVar
 from copy import deepcopy
-from types import MethodType
+from typing import Optional
 
 
 def _make_initializer(opaque):
+    @contextmanager
+    def initialiser(func, *args, **kwargs):
+        token = opaque._store.set(deepcopy(opaque._store.get()))
+        opaque.update(func(*args, **kwargs))
+        try:
+            yield
+        finally:
+            opaque._store.reset(token)
 
-    class OpaqueInitializer(ContextDecorator, ExitStack):
-        def __init__(self, func, *args, **kwargs):
-            super().__init__()
-
-            def member_func(self):
-                return func(*args, **kwargs)
-
-            self.func = MethodType(member_func, self)
-            self.saved = None
-
-        def __enter__(self):
-            self.saved = deepcopy(opaque._store)
-            opaque.update(self.func())
-
-        def __exit__(self, *exc):
-            opaque._store = self.saved
-            self.saved = None
-            super().__exit__(*exc)
-
-    return OpaqueInitializer
+    return initialiser
 
 
 class Opaque(MutableMapping):
     """
     Define a dict-like opaque context that can be initialized with application-specific values.
 
     Exposes a context manager/decorator interface that takes a generic function:
@@ -66,33 +56,34 @@
         @opaque.initialize(func, *args, **kwargs)
         def foo():
             pass
 
     See tests for usage examples.
 
     """
-    def __init__(self, *args, **kwargs):
-        self.service_name = kwargs.pop("name", None)
-        self._store = dict(*args, **kwargs)
+
+    def __init__(self, *args, **kwargs) -> None:
+        self.service_name: Optional[str] = kwargs.pop("name", None)
+        self._store = ContextVar("store", default=dict(*args, **kwargs))
         self.initialize = _make_initializer(self)
 
     def __getitem__(self, key):
-        return self._store[key]
+        return self._store.get()[key]
 
     def __setitem__(self, key, value):
-        self._store[key] = value
+        self._store.get()[key] = value
 
     def __delitem__(self, key):
-        del self._store[key]
+        del self._store.get()[key]
 
     def __iter__(self):
-        return iter(self._store)
+        return iter(self._store.get())
 
     def __len__(self):
-        return len(self._store)
+        return len(self._store.get())
 
     def as_dict(self):
-        return self._store
+        return self._store.get()
 
 
 def configure_opaque(graph):
     return Opaque(graph.config.opaque, name=graph.metadata.name)
```

### Comparing `microcosm-3.1.0/microcosm/profile.py` & `microcosm-3.2.0/microcosm/profile.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/registry.py` & `microcosm-3.2.0/microcosm/registry.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/scoping/factories.py` & `microcosm-3.2.0/microcosm/scoping/factories.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/scoping/proxies.py` & `microcosm-3.2.0/microcosm/scoping/proxies.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm/typing.py` & `microcosm-3.2.0/microcosm/typing.py`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/microcosm.egg-info/PKG-INFO` & `microcosm-3.2.0/microcosm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcosm
-Version: 3.1.0
+Version: 3.2.0
 Summary: Microcosm - Simple microservice configuration
 Home-page: https://github.com/globality-corp/microcosm
 Author: Globality Engineering
 Author-email: engineering@globality.com
 License: UNKNOWN
 Keywords: microcosm
 Platform: UNKNOWN
```

### Comparing `microcosm-3.1.0/microcosm.egg-info/SOURCES.txt` & `microcosm-3.2.0/microcosm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/setup.cfg` & `microcosm-3.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `microcosm-3.1.0/setup.py` & `microcosm-3.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import find_packages, setup
 
 
 project = "microcosm"
-version = "3.1.0"
+version = "3.2.0"
 
 setup(
     name=project,
     version=version,
     description="Microcosm - Simple microservice configuration",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

