# Comparing `tmp/camminapy-0.9.4.tar.gz` & `tmp/camminapy-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camminapy-0.9.4.tar", max compression
+gzip compressed data, was "camminapy-0.9.5.tar", max compression
```

## Comparing `camminapy-0.9.4.tar` & `camminapy-0.9.5.tar`

### file list

```diff
@@ -1,17 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-05-25 08:57:11.658456 camminapy-0.9.4/LICENSE
--rw-r--r--   0        0        0      343 2023-05-25 13:19:50.996652 camminapy-0.9.4/README.rst
--rw-r--r--   0        0        0      232 2023-05-25 09:36:38.187302 camminapy-0.9.4/camminapy/__init__.py
--rw-r--r--   0        0        0      343 2023-05-25 09:40:51.581748 camminapy-0.9.4/camminapy/data/__init__.py
--rw-r--r--   0        0        0     6276 2023-05-25 13:16:26.338410 camminapy-0.9.4/camminapy/data/resample.py
--rw-r--r--   0        0        0      163 2023-05-25 11:46:26.866899 camminapy-0.9.4/camminapy/plot/__init__.py
--rw-r--r--   0        0        0     1085 2023-05-25 11:44:40.466282 camminapy-0.9.4/camminapy/plot/altair_config.py
--rw-r--r--   0        0        0     6221 2023-05-25 11:45:21.605193 camminapy-0.9.4/camminapy/plot/altair_theme.py
--rw-r--r--   0        0        0     2633 2023-05-25 12:58:34.534445 camminapy-0.9.4/camminapy/plot/footer.py
--rw-r--r--   0        0        0        0 2023-05-25 08:57:11.673431 camminapy-0.9.4/camminapy/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-25 13:20:44.139887 camminapy-0.9.4/camminapy/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      937 2023-05-25 13:20:44.140280 camminapy-0.9.4/camminapy/utils/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0      759 2023-05-25 13:20:44.141151 camminapy-0.9.4/camminapy/utils/__pycache__/logger.cpython-310.pyc
--rw-r--r--   0        0        0      600 2023-05-25 08:57:11.672848 camminapy-0.9.4/camminapy/utils/config.py
--rw-r--r--   0        0        0      721 2023-05-25 08:57:11.674539 camminapy-0.9.4/camminapy/utils/logger.py
--rw-r--r--   0        0        0     1084 2023-05-25 13:20:43.618811 camminapy-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 camminapy-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-25 08:57:11.658456 camminapy-0.9.5/LICENSE
+-rw-r--r--   0        0        0      343 2023-05-25 13:19:50.996652 camminapy-0.9.5/README.rst
+-rw-r--r--   0        0        0      232 2023-05-25 09:36:38.187302 camminapy-0.9.5/camminapy/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-25 09:40:51.581748 camminapy-0.9.5/camminapy/data/__init__.py
+-rw-r--r--   0        0        0     6276 2023-05-25 13:16:26.338410 camminapy-0.9.5/camminapy/data/resample.py
+-rw-r--r--   0        0        0      163 2023-05-25 11:46:26.866899 camminapy-0.9.5/camminapy/plot/__init__.py
+-rw-r--r--   0        0        0     1085 2023-05-25 11:44:40.466282 camminapy-0.9.5/camminapy/plot/altair_config.py
+-rw-r--r--   0        0        0     6221 2023-05-25 11:45:21.605193 camminapy-0.9.5/camminapy/plot/altair_theme.py
+-rw-r--r--   0        0        0     2633 2023-05-25 12:58:34.534445 camminapy-0.9.5/camminapy/plot/footer.py
+-rw-r--r--   0        0        0        0 2023-05-25 08:57:11.673431 camminapy-0.9.5/camminapy/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-25 08:57:11.672848 camminapy-0.9.5/camminapy/utils/config.py
+-rw-r--r--   0        0        0      721 2023-05-25 08:57:11.674539 camminapy-0.9.5/camminapy/utils/logger.py
+-rw-r--r--   0        0        0     1084 2023-05-25 13:22:51.216946 camminapy-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 camminapy-0.9.5/PKG-INFO
```

### Comparing `camminapy-0.9.4/LICENSE` & `camminapy-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `camminapy-0.9.4/camminapy/data/resample.py` & `camminapy-0.9.5/camminapy/data/resample.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.9.4/camminapy/plot/altair_config.py` & `camminapy-0.9.5/camminapy/plot/altair_config.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.9.4/camminapy/plot/altair_theme.py` & `camminapy-0.9.5/camminapy/plot/altair_theme.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.9.4/camminapy/plot/footer.py` & `camminapy-0.9.5/camminapy/plot/footer.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.9.4/camminapy/utils/config.py` & `camminapy-0.9.5/camminapy/utils/config.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.9.4/camminapy/utils/logger.py` & `camminapy-0.9.5/camminapy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.9.4/pyproject.toml` & `camminapy-0.9.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "camminapy"
-version = "0.9.4"
+version = "0.9.5"
 description = "Personal helper functions and code snippets."
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 readme = "README.rst"
 repository = "https://github.com/thomascamminady/camminapy"
 
 
 [tool.poetry.dependencies]
```

### Comparing `camminapy-0.9.4/PKG-INFO` & `camminapy-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camminapy
-Version: 0.9.4
+Version: 0.9.5
 Summary: Personal helper functions and code snippets.
 Home-page: https://github.com/thomascamminady/camminapy
 Author: Thomas Camminady
 Author-email: 0milieux_member@icloud.com
 Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

