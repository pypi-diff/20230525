# Comparing `tmp/cacheyou-23.2.tar.gz` & `tmp/cacheyou-23.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cacheyou-23.2.tar", last modified: Mon May 22 08:29:46 2023, max compression
+gzip compressed data, was "cacheyou-23.3.tar", last modified: Thu May 25 02:54:32 2023, max compression
```

## Comparing `cacheyou-23.2.tar` & `cacheyou-23.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      575 2023-05-22 08:29:27.176707 cacheyou-23.2/LICENSE.txt
--rw-r--r--   0        0        0      830 2023-05-22 08:29:27.176707 cacheyou-23.2/README.md
--rw-r--r--   0        0        0      516 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/_cmd.py
--rw-r--r--   0        0        0     5832 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/adapter.py
--rw-r--r--   0        0        0     1895 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/cache.py
--rw-r--r--   0        0        0      288 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/caches/__init__.py
--rw-r--r--   0        0        0     5347 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/caches/file_cache.py
--rw-r--r--   0        0        0     1709 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/caches/redis_cache.py
--rw-r--r--   0        0        0    17699 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/controller.py
--rw-r--r--   0        0        0     4208 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/filewrapper.py
--rw-r--r--   0        0        0     4808 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/heuristics.py
--rw-r--r--   0        0        0        0 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/py.typed
--rw-r--r--   0        0        0     7612 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/serialize.py
--rw-r--r--   0        0        0     1284 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/wrapper.py
--rw-r--r--   0        0        0     5673 2023-05-22 08:29:27.176707 cacheyou-23.2/docs/Makefile
--rw-r--r--   0        0        0     8119 2023-05-22 08:29:27.176707 cacheyou-23.2/docs/conf.py
--rw-r--r--   0        0        0     5478 2023-05-22 08:29:27.176707 cacheyou-23.2/docs/custom_heuristics.rst
--rw-r--r--   0        0        0     5209 2023-05-22 08:29:27.176707 cacheyou-23.2/docs/etags.rst
--rw-r--r--   0        0        0     2289 2023-05-22 08:29:27.176707 cacheyou-23.2/docs/index.rst
--rw-r--r--   0        0        0     4161 2023-05-22 08:29:27.176707 cacheyou-23.2/docs/release_notes.rst
--rw-r--r--   0        0        0      643 2023-05-22 08:29:27.176707 cacheyou-23.2/docs/requirements.txt
--rw-r--r--   0        0        0     4297 2023-05-22 08:29:27.180707 cacheyou-23.2/docs/storage.rst
--rw-r--r--   0        0        0     2372 2023-05-22 08:29:27.180707 cacheyou-23.2/docs/tips.rst
--rw-r--r--   0        0        0     1792 2023-05-22 08:29:27.180707 cacheyou-23.2/docs/usage.rst
--rw-r--r--   0        0        0     2626 2023-05-22 08:29:46.849022 cacheyou-23.2/pyproject.toml
--rw-r--r--   0        0        0       30 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/__init__.py
--rw-r--r--   0        0        0     4750 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/conftest.py
--rw-r--r--   0        0        0     1114 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/issue_263.py
--rw-r--r--   0        0        0     1682 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_adapter.py
--rw-r--r--   0        0        0    10845 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_cache_control.py
--rw-r--r--   0        0        0     1470 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_chunked_response.py
--rw-r--r--   0        0        0     5110 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_etag.py
--rw-r--r--   0        0        0     6679 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_expires_heuristics.py
--rw-r--r--   0        0        0     1747 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_max_age.py
--rw-r--r--   0        0        0     1597 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_redirects.py
--rw-r--r--   0        0        0      941 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_regressions.py
--rw-r--r--   0        0        0     5484 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_serialization.py
--rw-r--r--   0        0        0      259 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_server_http_version.py
--rw-r--r--   0        0        0     5689 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_storage_filecache.py
--rw-r--r--   0        0        0      789 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_storage_redis.py
--rw-r--r--   0        0        0     2957 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_vary.py
--rw-r--r--   0        0        0      792 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/utils.py
--rw-r--r--   0        0        0      484 2023-05-22 08:29:27.180707 cacheyou-23.2/tox.ini
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 cacheyou-23.2/PKG-INFO
+-rw-r--r--   0        0        0      575 2023-05-25 02:54:18.560089 cacheyou-23.3/LICENSE.txt
+-rw-r--r--   0        0        0      830 2023-05-25 02:54:18.560089 cacheyou-23.3/README.md
+-rw-r--r--   0        0        0      516 2023-05-25 02:54:18.560089 cacheyou-23.3/cacheyou/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-25 02:54:18.564089 cacheyou-23.3/cacheyou/_cmd.py
+-rw-r--r--   0        0        0     5832 2023-05-25 02:54:18.564089 cacheyou-23.3/cacheyou/adapter.py
+-rw-r--r--   0        0        0     1895 2023-05-25 02:54:18.564089 cacheyou-23.3/cacheyou/cache.py
+-rw-r--r--   0        0        0      288 2023-05-25 02:54:18.564089 cacheyou-23.3/cacheyou/caches/__init__.py
+-rw-r--r--   0        0        0     5347 2023-05-25 02:54:18.564089 cacheyou-23.3/cacheyou/caches/file_cache.py
+-rw-r--r--   0        0        0     1709 2023-05-25 02:54:18.564089 cacheyou-23.3/cacheyou/caches/redis_cache.py
+-rw-r--r--   0        0        0    17699 2023-05-25 02:54:18.564089 cacheyou-23.3/cacheyou/controller.py
+-rw-r--r--   0        0        0     4208 2023-05-25 02:54:18.564089 cacheyou-23.3/cacheyou/filewrapper.py
+-rw-r--r--   0        0        0     4808 2023-05-25 02:54:18.564089 cacheyou-23.3/cacheyou/heuristics.py
+-rw-r--r--   0        0        0        0 2023-05-25 02:54:18.564089 cacheyou-23.3/cacheyou/py.typed
+-rw-r--r--   0        0        0     7612 2023-05-25 02:54:18.564089 cacheyou-23.3/cacheyou/serialize.py
+-rw-r--r--   0        0        0     1284 2023-05-25 02:54:18.564089 cacheyou-23.3/cacheyou/wrapper.py
+-rw-r--r--   0        0        0     5673 2023-05-25 02:54:18.564089 cacheyou-23.3/docs/Makefile
+-rw-r--r--   0        0        0     8119 2023-05-25 02:54:18.564089 cacheyou-23.3/docs/conf.py
+-rw-r--r--   0        0        0     5478 2023-05-25 02:54:18.564089 cacheyou-23.3/docs/custom_heuristics.rst
+-rw-r--r--   0        0        0     5209 2023-05-25 02:54:18.564089 cacheyou-23.3/docs/etags.rst
+-rw-r--r--   0        0        0     2289 2023-05-25 02:54:18.564089 cacheyou-23.3/docs/index.rst
+-rw-r--r--   0        0        0     4236 2023-05-25 02:54:18.564089 cacheyou-23.3/docs/release_notes.rst
+-rw-r--r--   0        0        0      643 2023-05-25 02:54:18.564089 cacheyou-23.3/docs/requirements.txt
+-rw-r--r--   0        0        0     4297 2023-05-25 02:54:18.564089 cacheyou-23.3/docs/storage.rst
+-rw-r--r--   0        0        0     2372 2023-05-25 02:54:18.564089 cacheyou-23.3/docs/tips.rst
+-rw-r--r--   0        0        0     1792 2023-05-25 02:54:18.564089 cacheyou-23.3/docs/usage.rst
+-rw-r--r--   0        0        0     2704 2023-05-25 02:54:32.952340 cacheyou-23.3/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-05-25 02:54:18.564089 cacheyou-23.3/tests/__init__.py
+-rw-r--r--   0        0        0     4750 2023-05-25 02:54:18.564089 cacheyou-23.3/tests/conftest.py
+-rw-r--r--   0        0        0     1114 2023-05-25 02:54:18.564089 cacheyou-23.3/tests/issue_263.py
+-rw-r--r--   0        0        0     1682 2023-05-25 02:54:18.564089 cacheyou-23.3/tests/test_adapter.py
+-rw-r--r--   0        0        0    10845 2023-05-25 02:54:18.564089 cacheyou-23.3/tests/test_cache_control.py
+-rw-r--r--   0        0        0     1470 2023-05-25 02:54:18.564089 cacheyou-23.3/tests/test_chunked_response.py
+-rw-r--r--   0        0        0     5110 2023-05-25 02:54:18.564089 cacheyou-23.3/tests/test_etag.py
+-rw-r--r--   0        0        0     6679 2023-05-25 02:54:18.564089 cacheyou-23.3/tests/test_expires_heuristics.py
+-rw-r--r--   0        0        0     1747 2023-05-25 02:54:18.564089 cacheyou-23.3/tests/test_max_age.py
+-rw-r--r--   0        0        0     1597 2023-05-25 02:54:18.564089 cacheyou-23.3/tests/test_redirects.py
+-rw-r--r--   0        0        0      941 2023-05-25 02:54:18.564089 cacheyou-23.3/tests/test_regressions.py
+-rw-r--r--   0        0        0     5484 2023-05-25 02:54:18.564089 cacheyou-23.3/tests/test_serialization.py
+-rw-r--r--   0        0        0      259 2023-05-25 02:54:18.564089 cacheyou-23.3/tests/test_server_http_version.py
+-rw-r--r--   0        0        0     5689 2023-05-25 02:54:18.564089 cacheyou-23.3/tests/test_storage_filecache.py
+-rw-r--r--   0        0        0      789 2023-05-25 02:54:18.564089 cacheyou-23.3/tests/test_storage_redis.py
+-rw-r--r--   0        0        0     2957 2023-05-25 02:54:18.564089 cacheyou-23.3/tests/test_vary.py
+-rw-r--r--   0        0        0      792 2023-05-25 02:54:18.564089 cacheyou-23.3/tests/utils.py
+-rw-r--r--   0        0        0      484 2023-05-25 02:54:18.564089 cacheyou-23.3/tox.ini
+-rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 cacheyou-23.3/PKG-INFO
```

### Comparing `cacheyou-23.2/LICENSE.txt` & `cacheyou-23.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/README.md` & `cacheyou-23.3/README.md`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/cacheyou/__init__.py` & `cacheyou-23.3/cacheyou/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 """
 import logging
 
 from cacheyou.adapter import CacheControlAdapter
 from cacheyou.controller import CacheController
 from cacheyou.wrapper import CacheControl
 
-__version__ = "23.2"
+__version__ = "23.3"
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 __all__ = ("CacheControl", "CacheControlAdapter", "CacheController")
```

### Comparing `cacheyou-23.2/cacheyou/_cmd.py` & `cacheyou-23.3/cacheyou/_cmd.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/cacheyou/adapter.py` & `cacheyou-23.3/cacheyou/adapter.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/cacheyou/cache.py` & `cacheyou-23.3/cacheyou/cache.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/cacheyou/caches/file_cache.py` & `cacheyou-23.3/cacheyou/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/cacheyou/caches/redis_cache.py` & `cacheyou-23.3/cacheyou/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/cacheyou/controller.py` & `cacheyou-23.3/cacheyou/controller.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/cacheyou/filewrapper.py` & `cacheyou-23.3/cacheyou/filewrapper.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/cacheyou/heuristics.py` & `cacheyou-23.3/cacheyou/heuristics.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/cacheyou/serialize.py` & `cacheyou-23.3/cacheyou/serialize.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/cacheyou/wrapper.py` & `cacheyou-23.3/cacheyou/wrapper.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/docs/Makefile` & `cacheyou-23.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/docs/conf.py` & `cacheyou-23.3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 copyright = "2013, Eric Larson, 2023 Frost Ming"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
-release = "23.2"
+release = "23.3"
 # The short X.Y version.
 version = release
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
```

### Comparing `cacheyou-23.2/docs/custom_heuristics.rst` & `cacheyou-23.3/docs/custom_heuristics.rst`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/docs/etags.rst` & `cacheyou-23.3/docs/etags.rst`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/docs/index.rst` & `cacheyou-23.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/docs/release_notes.rst` & `cacheyou-23.3/docs/release_notes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 
   SPDX-License-Identifier: Apache-2.0
 
 ===============
  Release Notes
 ===============
 
+23.3
+====
+
+* Exclude the ``tests`` directory from the wheel distribution.
+
 23.2
 ====
 
 * Handle ``strict`` parameter for both ``urllib3`` 1.x and 2.x.
 
 23.1
 ====
```

### Comparing `cacheyou-23.2/docs/requirements.txt` & `cacheyou-23.3/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/docs/storage.rst` & `cacheyou-23.3/docs/storage.rst`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/docs/tips.rst` & `cacheyou-23.3/docs/tips.rst`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/docs/usage.rst` & `cacheyou-23.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/pyproject.toml` & `cacheyou-23.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "CacheYou"
-version = "23.2"
+version = "23.3"
 description = "httplib2 caching for requests"
 keywords = [
     "requests",
     "http",
     "caching",
     "web",
 ]
@@ -52,17 +52,20 @@
     "pdm-autoexport",
 ]
 
 [tool.pdm.build]
 source-includes = [
     "docs/",
     "tox.ini",
+    "tests/",
 ]
 
 [tool.pdm.scripts]
+test = "pytest"
+release = "bumpver update"
 docs = [
     "sphinx-autobuild",
     "docs/",
     "build/docs",
     "-a",
     "--watch",
     "cacheyou",
@@ -70,14 +73,15 @@
     "8765",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "tox",
     "bumpver>=2023.1124",
+    "pytest>=7.3.1",
 ]
 docs = [
     "sphinx",
     "sphinx-autobuild",
     "sphinx-rtd-theme>=1.2.0",
 ]
 
@@ -123,15 +127,15 @@
 
 [tool.ruff.isort]
 known-first-party = [
     "cacheyou",
 ]
 
 [tool.bumpver]
-current_version = "23.2"
+current_version = "23.3"
 version_pattern = "YY.INC0[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `cacheyou-23.2/tests/conftest.py` & `cacheyou-23.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/tests/issue_263.py` & `cacheyou-23.3/tests/issue_263.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/tests/test_adapter.py` & `cacheyou-23.3/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/tests/test_cache_control.py` & `cacheyou-23.3/tests/test_cache_control.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/tests/test_chunked_response.py` & `cacheyou-23.3/tests/test_chunked_response.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/tests/test_etag.py` & `cacheyou-23.3/tests/test_etag.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/tests/test_expires_heuristics.py` & `cacheyou-23.3/tests/test_expires_heuristics.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/tests/test_max_age.py` & `cacheyou-23.3/tests/test_max_age.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/tests/test_redirects.py` & `cacheyou-23.3/tests/test_redirects.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/tests/test_regressions.py` & `cacheyou-23.3/tests/test_regressions.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/tests/test_serialization.py` & `cacheyou-23.3/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/tests/test_storage_filecache.py` & `cacheyou-23.3/tests/test_storage_filecache.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/tests/test_storage_redis.py` & `cacheyou-23.3/tests/test_storage_redis.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/tests/test_vary.py` & `cacheyou-23.3/tests/test_vary.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/tests/utils.py` & `cacheyou-23.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.2/PKG-INFO` & `cacheyou-23.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacheyou
-Version: 23.2
+Version: 23.3
 Summary: httplib2 caching for requests
 Keywords: requests http caching web
 Author-Email: Frost Ming <me@frostming.com>, Eric Larson <eric@ionrock.org>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

