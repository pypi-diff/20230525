# Comparing `tmp/camminapy-0.8.2.tar.gz` & `tmp/camminapy-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camminapy-0.8.2.tar", max compression
+gzip compressed data, was "camminapy-0.8.3.tar", max compression
```

## Comparing `camminapy-0.8.2.tar` & `camminapy-0.8.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1074 2023-05-25 08:57:11.658456 camminapy-0.8.2/LICENSE
--rw-r--r--   0        0        0      146 2023-05-25 09:19:32.338910 camminapy-0.8.2/README.rst
--rw-r--r--   0        0        0      254 2023-05-25 08:57:11.671705 camminapy-0.8.2/camminapy/__init__.py
--rw-r--r--   0        0        0       63 2023-05-25 09:24:37.675451 camminapy-0.8.2/camminapy/plot/__init__.py
--rw-r--r--   0        0        0     2583 2023-05-25 09:25:59.612697 camminapy-0.8.2/camminapy/plot/footer.py
--rw-r--r--   0        0        0        0 2023-05-25 08:57:11.673431 camminapy-0.8.2/camminapy/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-05-25 08:57:11.672848 camminapy-0.8.2/camminapy/utils/config.py
--rw-r--r--   0        0        0      721 2023-05-25 08:57:11.674539 camminapy-0.8.2/camminapy/utils/logger.py
--rw-r--r--   0        0        0      991 2023-05-25 09:34:57.702280 camminapy-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 camminapy-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-25 08:57:11.658456 camminapy-0.8.3/LICENSE
+-rw-r--r--   0        0        0      173 2023-05-25 09:36:05.703996 camminapy-0.8.3/README.rst
+-rw-r--r--   0        0        0      254 2023-05-25 08:57:11.671705 camminapy-0.8.3/camminapy/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-25 09:24:37.675451 camminapy-0.8.3/camminapy/plot/__init__.py
+-rw-r--r--   0        0        0     2583 2023-05-25 09:25:59.612697 camminapy-0.8.3/camminapy/plot/footer.py
+-rw-r--r--   0        0        0        0 2023-05-25 08:57:11.673431 camminapy-0.8.3/camminapy/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-25 08:57:11.672848 camminapy-0.8.3/camminapy/utils/config.py
+-rw-r--r--   0        0        0      721 2023-05-25 08:57:11.674539 camminapy-0.8.3/camminapy/utils/logger.py
+-rw-r--r--   0        0        0      991 2023-05-25 09:36:11.404281 camminapy-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 camminapy-0.8.3/PKG-INFO
```

### Comparing `camminapy-0.8.2/LICENSE` & `camminapy-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.2/camminapy/plot/footer.py` & `camminapy-0.8.3/camminapy/plot/footer.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.2/camminapy/utils/config.py` & `camminapy-0.8.3/camminapy/utils/config.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.2/camminapy/utils/logger.py` & `camminapy-0.8.3/camminapy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.2/pyproject.toml` & `camminapy-0.8.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "camminapy"
-version = "0.8.2"
+version = "0.8.3"
 description = "Personal helper functions and code snippets."
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 readme = "README.rst"
 repository = "https://github.com/thomascamminady/camminapy"
 
 
 [tool.poetry.dependencies]
```

### Comparing `camminapy-0.8.2/PKG-INFO` & `camminapy-0.8.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camminapy
-Version: 0.8.2
+Version: 0.8.3
 Summary: Personal helper functions and code snippets.
 Home-page: https://github.com/thomascamminady/camminapy
 Author: Thomas Camminady
 Author-email: 0milieux_member@icloud.com
 Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -18,15 +18,21 @@
 =========
 camminapy
 =========
 
 
 
 
-Install via pip_:
+Install via `pip`:
 
 .. code-block:: bash
 
    pip install camminapy
 
-.. _pip: https://pypi.org/project/camminapy/
+
+
+Install via `poetry`:
+
+.. code-block:: bash
+
+   poetry add camminapy
```

