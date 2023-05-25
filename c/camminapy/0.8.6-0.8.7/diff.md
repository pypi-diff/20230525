# Comparing `tmp/camminapy-0.8.6.tar.gz` & `tmp/camminapy-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camminapy-0.8.6.tar", max compression
+gzip compressed data, was "camminapy-0.8.7.tar", max compression
```

## Comparing `camminapy-0.8.6.tar` & `camminapy-0.8.7.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1074 2023-05-25 08:57:11.658456 camminapy-0.8.6/LICENSE
--rw-r--r--   0        0        0      177 2023-05-25 09:38:05.904312 camminapy-0.8.6/README.rst
--rw-r--r--   0        0        0      232 2023-05-25 09:36:38.187302 camminapy-0.8.6/camminapy/__init__.py
--rw-r--r--   0        0        0       63 2023-05-25 09:24:37.675451 camminapy-0.8.6/camminapy/plot/__init__.py
--rw-r--r--   0        0        0     2583 2023-05-25 09:25:59.612697 camminapy-0.8.6/camminapy/plot/footer.py
--rw-r--r--   0        0        0        0 2023-05-25 08:57:11.673431 camminapy-0.8.6/camminapy/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-05-25 08:57:11.672848 camminapy-0.8.6/camminapy/utils/config.py
--rw-r--r--   0        0        0      721 2023-05-25 08:57:11.674539 camminapy-0.8.6/camminapy/utils/logger.py
--rw-r--r--   0        0        0      991 2023-05-25 09:38:09.262891 camminapy-0.8.6/pyproject.toml
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 camminapy-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-25 08:57:11.658456 camminapy-0.8.7/LICENSE
+-rw-r--r--   0        0        0      177 2023-05-25 09:38:05.904312 camminapy-0.8.7/README.rst
+-rw-r--r--   0        0        0      232 2023-05-25 09:36:38.187302 camminapy-0.8.7/camminapy/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-25 09:40:51.581748 camminapy-0.8.7/camminapy/data/__init__.py
+-rw-r--r--   0        0        0     3331 2023-05-25 09:40:19.166193 camminapy-0.8.7/camminapy/data/resample.py
+-rw-r--r--   0        0        0       63 2023-05-25 09:24:37.675451 camminapy-0.8.7/camminapy/plot/__init__.py
+-rw-r--r--   0        0        0     2583 2023-05-25 09:25:59.612697 camminapy-0.8.7/camminapy/plot/footer.py
+-rw-r--r--   0        0        0        0 2023-05-25 08:57:11.673431 camminapy-0.8.7/camminapy/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-25 08:57:11.672848 camminapy-0.8.7/camminapy/utils/config.py
+-rw-r--r--   0        0        0      721 2023-05-25 08:57:11.674539 camminapy-0.8.7/camminapy/utils/logger.py
+-rw-r--r--   0        0        0     1011 2023-05-25 09:41:27.897268 camminapy-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 camminapy-0.8.7/PKG-INFO
```

### Comparing `camminapy-0.8.6/LICENSE` & `camminapy-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.6/camminapy/plot/footer.py` & `camminapy-0.8.7/camminapy/plot/footer.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.6/camminapy/utils/config.py` & `camminapy-0.8.7/camminapy/utils/config.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.6/camminapy/utils/logger.py` & `camminapy-0.8.7/camminapy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.6/pyproject.toml` & `camminapy-0.8.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "camminapy"
-version = "0.8.6"
+version = "0.8.7"
 description = "Personal helper functions and code snippets."
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 readme = "README.rst"
 repository = "https://github.com/thomascamminady/camminapy"
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 altair = "^5.0.0"
 gitpython = "^3.1.31"
+polars = "^0.17.15"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.0.1"
 ruff = "^0.0.253"
 black = "^23.1.0"
 pyclean = "^2.2.0"
 pre-commit = "^3.1.1"
```

### Comparing `camminapy-0.8.6/PKG-INFO` & `camminapy-0.8.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: camminapy
-Version: 0.8.6
+Version: 0.8.7
 Summary: Personal helper functions and code snippets.
 Home-page: https://github.com/thomascamminady/camminapy
 Author: Thomas Camminady
 Author-email: 0milieux_member@icloud.com
 Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: altair (>=5.0.0,<6.0.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
+Requires-Dist: polars (>=0.17.15,<0.18.0)
 Project-URL: Repository, https://github.com/thomascamminady/camminapy
 Description-Content-Type: text/x-rst
 
 =========
 camminapy
 =========
```

