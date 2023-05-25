# Comparing `tmp/poolcontrolpy-0.2.6.tar.gz` & `tmp/poolcontrolpy-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poolcontrolpy-0.2.6.tar", max compression
+gzip compressed data, was "poolcontrolpy-0.2.7.tar", max compression
```

## Comparing `poolcontrolpy-0.2.6.tar` & `poolcontrolpy-0.2.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1073 2023-05-25 19:06:23.514410 poolcontrolpy-0.2.6/LICENSE
--rwxr-xr-x   0        0        0     1237 2023-05-25 19:06:23.514410 poolcontrolpy-0.2.6/README.md
--rwxr-xr-x   0        0        0     1265 2023-05-25 19:06:57.730640 poolcontrolpy-0.2.6/pyproject.toml
--rwxr-xr-x   0        0        0      115 2023-05-25 19:06:23.518410 poolcontrolpy-0.2.6/src/poolcontrolpy/__init__.py
--rw-r--r--   0        0        0      770 2023-05-25 19:06:23.518410 poolcontrolpy-0.2.6/src/poolcontrolpy/exceptions.py
--rwxr-xr-x   0        0        0     4466 2023-05-25 19:06:23.518410 poolcontrolpy-0.2.6/src/poolcontrolpy/poolcontrolpy.py
--rw-r--r--   0        0        0     1784 1970-01-01 00:00:00.000000 poolcontrolpy-0.2.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2023-05-25 19:11:10.574629 poolcontrolpy-0.2.7/LICENSE
+-rwxr-xr-x   0        0        0     1237 2023-05-25 19:11:10.574629 poolcontrolpy-0.2.7/README.md
+-rwxr-xr-x   0        0        0     1265 2023-05-25 19:11:50.415485 poolcontrolpy-0.2.7/pyproject.toml
+-rwxr-xr-x   0        0        0      115 2023-05-25 19:11:10.574629 poolcontrolpy-0.2.7/src/poolcontrolpy/__init__.py
+-rw-r--r--   0        0        0      770 2023-05-25 19:11:10.574629 poolcontrolpy-0.2.7/src/poolcontrolpy/exceptions.py
+-rwxr-xr-x   0        0        0     4466 2023-05-25 19:11:10.578629 poolcontrolpy-0.2.7/src/poolcontrolpy/poolcontrolpy.py
+-rw-r--r--   0        0        0     1784 1970-01-01 00:00:00.000000 poolcontrolpy-0.2.7/PKG-INFO
```

### Comparing `poolcontrolpy-0.2.6/LICENSE` & `poolcontrolpy-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `poolcontrolpy-0.2.6/README.md` & `poolcontrolpy-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `poolcontrolpy-0.2.6/pyproject.toml` & `poolcontrolpy-0.2.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poolcontrolpy"
-version = "0.2.6"
+version = "0.2.7"
 description = "Package for accessing nodejs-poolController"
 authors = ["Kevin Robinson"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `poolcontrolpy-0.2.6/src/poolcontrolpy/exceptions.py` & `poolcontrolpy-0.2.7/src/poolcontrolpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `poolcontrolpy-0.2.6/src/poolcontrolpy/poolcontrolpy.py` & `poolcontrolpy-0.2.7/src/poolcontrolpy/poolcontrolpy.py`

 * *Files identical despite different names*

### Comparing `poolcontrolpy-0.2.6/PKG-INFO` & `poolcontrolpy-0.2.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poolcontrolpy
-Version: 0.2.6
+Version: 0.2.7
 Summary: Package for accessing nodejs-poolController
 License: MIT
 Author: Kevin Robinson
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

