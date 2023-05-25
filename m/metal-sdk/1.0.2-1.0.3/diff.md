# Comparing `tmp/metal_sdk-1.0.2.tar.gz` & `tmp/metal_sdk-1.0.3.tar.gz`

## Comparing `metal_sdk-1.0.2.tar` & `metal_sdk-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/.github/workflows/lint.yml
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/examples/example.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/examples/example_async.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/src/metal_sdk/__init__.py
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/src/metal_sdk/metal.py
--rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/src/metal_sdk/metal_async.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/src/metal_sdk/typings.py
--rw-r--r--   0        0        0     7183 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/tests/test_metal.py
--rw-r--r--   0        0        0     7180 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/tests/test_metal_async.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/.gitignore
--rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/LICENSE
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/README.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/examples/example.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/examples/example_async.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/src/metal_sdk/__init__.py
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/src/metal_sdk/metal.py
+-rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/src/metal_sdk/metal_async.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/src/metal_sdk/motorhead.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/src/metal_sdk/motorhead_async.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/src/metal_sdk/typings.py
+-rw-r--r--   0        0        0     7183 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/tests/test_metal.py
+-rw-r--r--   0        0        0     7180 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/tests/test_metal_async.py
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/tests/test_motorhead.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/tests/test_motorhead_async.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/.gitignore
+-rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/LICENSE
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/README.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/PKG-INFO
```

### Comparing `metal_sdk-1.0.2/.github/workflows/publish.yml` & `metal_sdk-1.0.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.2/.github/workflows/test.yml` & `metal_sdk-1.0.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.2/examples/example.py` & `metal_sdk-1.0.3/examples/example.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.2/examples/example_async.py` & `metal_sdk-1.0.3/examples/example_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.2/src/metal_sdk/metal.py` & `metal_sdk-1.0.3/src/metal_sdk/metal.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.2/src/metal_sdk/metal_async.py` & `metal_sdk-1.0.3/src/metal_sdk/metal_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.2/src/metal_sdk/typings.py` & `metal_sdk-1.0.3/src/metal_sdk/typings.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.2/tests/test_metal.py` & `metal_sdk-1.0.3/tests/test_metal.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.2/tests/test_metal_async.py` & `metal_sdk-1.0.3/tests/test_metal_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.2/.gitignore` & `metal_sdk-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.2/LICENSE` & `metal_sdk-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.2/README.md` & `metal_sdk-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.2/pyproject.toml` & `metal_sdk-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "metal_sdk"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Metal Technologies Inc", email="james@getmetal.io" },
 ]
 description = "SDK for getmetal.io"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `metal_sdk-1.0.2/PKG-INFO` & `metal_sdk-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metal_sdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: SDK for getmetal.io
 Project-URL: Github, https://github.com/getmetal/metal-python
 Author-email: Metal Technologies Inc <james@getmetal.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

