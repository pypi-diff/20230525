# Comparing `tmp/rfrx-1.0.0.tar.gz` & `tmp/rfrx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfrx-1.0.0.tar", max compression
+gzip compressed data, was "rfrx-1.0.1.tar", max compression
```

## Comparing `rfrx-1.0.0.tar` & `rfrx-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1303 2023-05-25 18:21:42.108442 rfrx-1.0.0/LICENSE
--rw-r--r--   0        0        0      873 2023-05-25 18:21:42.108442 rfrx-1.0.0/README.md
--rw-r--r--   0        0        0      853 2023-05-25 18:21:42.108442 rfrx-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      139 2023-05-25 18:21:42.108442 rfrx-1.0.0/rfrx/__init__.py
--rw-r--r--   0        0        0     2410 2023-05-25 18:21:42.108442 rfrx-1.0.0/rfrx/protronik.py
--rw-r--r--   0        0        0     3901 2023-05-25 18:21:42.108442 rfrx-1.0.0/rfrx/sbus.py
--rw-r--r--   0        0        0     1523 1970-01-01 00:00:00.000000 rfrx-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1303 2023-05-25 18:33:35.437019 rfrx-1.0.1/LICENSE
+-rw-r--r--   0        0        0      873 2023-05-25 18:33:35.437019 rfrx-1.0.1/README.md
+-rw-r--r--   0        0        0      853 2023-05-25 18:33:35.437019 rfrx-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-05-25 18:33:35.437019 rfrx-1.0.1/rfrx/__init__.py
+-rw-r--r--   0        0        0     2410 2023-05-25 18:33:35.437019 rfrx-1.0.1/rfrx/protronik.py
+-rw-r--r--   0        0        0     3901 2023-05-25 18:33:35.437019 rfrx-1.0.1/rfrx/sbus.py
+-rw-r--r--   0        0        0     1523 1970-01-01 00:00:00.000000 rfrx-1.0.1/PKG-INFO
```

### Comparing `rfrx-1.0.0/LICENSE` & `rfrx-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rfrx-1.0.0/README.md` & `rfrx-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `rfrx-1.0.0/pyproject.toml` & `rfrx-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.poetry]
 authors = ["Guilhem Saurel <guilhem.saurel@laas.fr>"]
 description = "Receive SBUS frames from pro-tronik remote controller"
 license = "BSD-2-Clauses"
 name = "rfrx"
 readme = "README.md"
-version = "1.0.0"
+version = "1.0.1"
 
 [tool.poetry.dependencies]
 pyserial = "^3.5"
 python = "^3.7"
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `rfrx-1.0.0/rfrx/protronik.py` & `rfrx-1.0.1/rfrx/protronik.py`

 * *Files identical despite different names*

### Comparing `rfrx-1.0.0/rfrx/sbus.py` & `rfrx-1.0.1/rfrx/sbus.py`

 * *Files identical despite different names*

### Comparing `rfrx-1.0.0/PKG-INFO` & `rfrx-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfrx
-Version: 1.0.0
+Version: 1.0.1
 Summary: Receive SBUS frames from pro-tronik remote controller
 License: BSD-2-Clauses
 Author: Guilhem Saurel
 Author-email: guilhem.saurel@laas.fr
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

