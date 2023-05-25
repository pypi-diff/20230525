# Comparing `tmp/camminapy-0.9.8.tar.gz` & `tmp/camminapy-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camminapy-0.9.8.tar", max compression
+gzip compressed data, was "camminapy-0.9.9.tar", max compression
```

## Comparing `camminapy-0.9.8.tar` & `camminapy-0.9.9.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1074 2023-05-25 08:57:11.658456 camminapy-0.9.8/LICENSE
--rw-r--r--   0        0        0      343 2023-05-25 13:19:50.996652 camminapy-0.9.8/README.rst
--rw-r--r--   0        0        0      232 2023-05-25 09:36:38.187302 camminapy-0.9.8/camminapy/__init__.py
--rw-r--r--   0        0        0      343 2023-05-25 09:40:51.581748 camminapy-0.9.8/camminapy/data/__init__.py
--rw-r--r--   0        0        0     6280 2023-05-25 13:30:09.781467 camminapy-0.9.8/camminapy/data/resample.py
--rw-r--r--   0        0        0      163 2023-05-25 11:46:26.866899 camminapy-0.9.8/camminapy/plot/__init__.py
--rw-r--r--   0        0        0     1085 2023-05-25 11:44:40.466282 camminapy-0.9.8/camminapy/plot/altair_config.py
--rw-r--r--   0        0        0     6221 2023-05-25 11:45:21.605193 camminapy-0.9.8/camminapy/plot/altair_theme.py
--rw-r--r--   0        0        0     2633 2023-05-25 12:58:34.534445 camminapy-0.9.8/camminapy/plot/footer.py
--rw-r--r--   0        0        0        0 2023-05-25 08:57:11.673431 camminapy-0.9.8/camminapy/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-05-25 08:57:11.672848 camminapy-0.9.8/camminapy/utils/config.py
--rw-r--r--   0        0        0      721 2023-05-25 08:57:11.674539 camminapy-0.9.8/camminapy/utils/logger.py
--rw-r--r--   0        0        0     1084 2023-05-25 13:30:18.678815 camminapy-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 camminapy-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-25 08:57:11.658456 camminapy-0.9.9/LICENSE
+-rw-r--r--   0        0        0      343 2023-05-25 13:19:50.996652 camminapy-0.9.9/README.rst
+-rw-r--r--   0        0        0      232 2023-05-25 09:36:38.187302 camminapy-0.9.9/camminapy/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-25 09:40:51.581748 camminapy-0.9.9/camminapy/data/__init__.py
+-rw-r--r--   0        0        0     6280 2023-05-25 13:30:09.781467 camminapy-0.9.9/camminapy/data/resample.py
+-rw-r--r--   0        0        0       76 2023-05-25 13:32:39.413943 camminapy-0.9.9/camminapy/documentation.rst
+-rw-r--r--   0        0        0      163 2023-05-25 11:46:26.866899 camminapy-0.9.9/camminapy/plot/__init__.py
+-rw-r--r--   0        0        0     1085 2023-05-25 11:44:40.466282 camminapy-0.9.9/camminapy/plot/altair_config.py
+-rw-r--r--   0        0        0     6221 2023-05-25 11:45:21.605193 camminapy-0.9.9/camminapy/plot/altair_theme.py
+-rw-r--r--   0        0        0     2633 2023-05-25 12:58:34.534445 camminapy-0.9.9/camminapy/plot/footer.py
+-rw-r--r--   0        0        0        0 2023-05-25 08:57:11.673431 camminapy-0.9.9/camminapy/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-25 08:57:11.672848 camminapy-0.9.9/camminapy/utils/config.py
+-rw-r--r--   0        0        0      721 2023-05-25 08:57:11.674539 camminapy-0.9.9/camminapy/utils/logger.py
+-rw-r--r--   0        0        0     1084 2023-05-25 13:32:51.671887 camminapy-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 camminapy-0.9.9/PKG-INFO
```

### Comparing `camminapy-0.9.8/LICENSE` & `camminapy-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `camminapy-0.9.8/camminapy/data/resample.py` & `camminapy-0.9.9/camminapy/data/resample.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.9.8/camminapy/plot/altair_config.py` & `camminapy-0.9.9/camminapy/plot/altair_config.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.9.8/camminapy/plot/altair_theme.py` & `camminapy-0.9.9/camminapy/plot/altair_theme.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.9.8/camminapy/plot/footer.py` & `camminapy-0.9.9/camminapy/plot/footer.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.9.8/camminapy/utils/config.py` & `camminapy-0.9.9/camminapy/utils/config.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.9.8/camminapy/utils/logger.py` & `camminapy-0.9.9/camminapy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.9.8/pyproject.toml` & `camminapy-0.9.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "camminapy"
-version = "0.9.8"
+version = "0.9.9"
 description = "Personal helper functions and code snippets."
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 readme = "README.rst"
 repository = "https://github.com/thomascamminady/camminapy"
 
 
 [tool.poetry.dependencies]
```

### Comparing `camminapy-0.9.8/PKG-INFO` & `camminapy-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camminapy
-Version: 0.9.8
+Version: 0.9.9
 Summary: Personal helper functions and code snippets.
 Home-page: https://github.com/thomascamminady/camminapy
 Author: Thomas Camminady
 Author-email: 0milieux_member@icloud.com
 Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

