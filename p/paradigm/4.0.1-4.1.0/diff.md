# Comparing `tmp/paradigm-4.0.1.tar.gz` & `tmp/paradigm-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradigm-4.0.1.tar", last modified: Thu May 25 06:23:56 2023, max compression
+gzip compressed data, was "paradigm-4.1.0.tar", last modified: Thu May 25 07:09:54 2023, max compression
```

## Comparing `paradigm-4.0.1.tar` & `paradigm-4.1.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:23:56.882045 paradigm-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-25 06:23:47.000000 paradigm-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 06:23:47.000000 paradigm-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-25 06:23:56.882045 paradigm-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-25 06:23:47.000000 paradigm-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:23:56.882045 paradigm-4.0.1/paradigm/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:23:56.882045 paradigm-4.0.1/paradigm/_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/annotated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:23:56.882045 paradigm-4.0.1/paradigm/_core/arboreal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/arboreal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/arboreal/construction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/arboreal/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/arboreal/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/arboreal/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/arboreal/kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/arboreal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    24186 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/namespacing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/pretty.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/scoping.py
--rw-r--r--   0 runner    (1001) docker     (123)    26241 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)    47999 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/stubs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/base.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:23:56.882045 paradigm-4.0.1/paradigm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-25 06:23:56.000000 paradigm-4.0.1/paradigm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-25 06:23:56.000000 paradigm-4.0.1/paradigm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 06:23:56.000000 paradigm-4.0.1/paradigm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 06:23:56.000000 paradigm-4.0.1/paradigm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 06:23:56.000000 paradigm-4.0.1/paradigm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 06:23:47.000000 paradigm-4.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-25 06:23:56.882045 paradigm-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-25 06:23:47.000000 paradigm-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:54.596300 paradigm-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-25 07:09:41.000000 paradigm-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-25 07:09:41.000000 paradigm-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-05-25 07:09:54.596300 paradigm-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-25 07:09:41.000000 paradigm-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:54.592300 paradigm-4.1.0/paradigm/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:54.596300 paradigm-4.1.0/paradigm/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/annotated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:54.596300 paradigm-4.1.0/paradigm/_core/arboreal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/arboreal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/arboreal/construction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/arboreal/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/arboreal/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/arboreal/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/arboreal/kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/arboreal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24186 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/namespacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/scoping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26241 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47999 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/_core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:41.000000 paradigm-4.1.0/paradigm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:54.592300 paradigm-4.1.0/paradigm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-05-25 07:09:54.000000 paradigm-4.1.0/paradigm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-25 07:09:54.000000 paradigm-4.1.0/paradigm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:09:54.000000 paradigm-4.1.0/paradigm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-25 07:09:54.000000 paradigm-4.1.0/paradigm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 07:09:54.000000 paradigm-4.1.0/paradigm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-25 07:09:41.000000 paradigm-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-25 07:09:54.596300 paradigm-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-25 07:09:41.000000 paradigm-4.1.0/setup.py
```

### Comparing `paradigm-4.0.1/LICENSE` & `paradigm-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/PKG-INFO` & `paradigm-4.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,49 @@
 Metadata-Version: 2.1
 Name: paradigm
-Version: 4.0.1
+Version: 4.1.0
 Summary: Python objects metadata parser.
 Home-page: https://github.com/lycantropos/paradigm/
 Download-URL: https://github.com/lycantropos/paradigm/archive/master.zip
-Author: Azat Ibrakov
-Author-email: azatibrakov@gmail.com
+Author-email: Azat Ibrakov <azatibrakov@gmail.com>
 License: MIT License
+        
+        Copyright (c) 2018 Azat Ibrakov
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 License-File: LICENSE
 
 paradigm
 ========
 
 [![](https://github.com/lycantropos/paradigm/workflows/CI/badge.svg)](https://github.com/lycantropos/paradigm/actions/workflows/ci.yml "Github Actions")
 [![](https://codecov.io/gh/lycantropos/paradigm/branch/master/graph/badge.svg)](https://codecov.io/gh/lycantropos/paradigm "Codecov")
```

### Comparing `paradigm-4.0.1/README.md` & `paradigm-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/annotated.py` & `paradigm-4.1.0/paradigm/_core/annotated.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/arboreal/construction.py` & `paradigm-4.1.0/paradigm/_core/arboreal/construction.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/arboreal/conversion.py` & `paradigm-4.1.0/paradigm/_core/arboreal/conversion.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/arboreal/evaluation.py` & `paradigm-4.1.0/paradigm/_core/arboreal/evaluation.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/arboreal/execution.py` & `paradigm-4.1.0/paradigm/_core/arboreal/execution.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/arboreal/utils.py` & `paradigm-4.1.0/paradigm/_core/arboreal/utils.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/caching.py` & `paradigm-4.1.0/paradigm/_core/caching.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/catalog.py` & `paradigm-4.1.0/paradigm/_core/catalog.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/discovery.py` & `paradigm-4.1.0/paradigm/_core/discovery.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/execution.py` & `paradigm-4.1.0/paradigm/_core/execution.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/file_system.py` & `paradigm-4.1.0/paradigm/_core/file_system.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/index.py` & `paradigm-4.1.0/paradigm/_core/index.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/models.py` & `paradigm-4.1.0/paradigm/_core/models.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/modules.py` & `paradigm-4.1.0/paradigm/_core/modules.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/pretty.py` & `paradigm-4.1.0/paradigm/_core/pretty.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/scoping.py` & `paradigm-4.1.0/paradigm/_core/scoping.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/signatures.py` & `paradigm-4.1.0/paradigm/_core/signatures.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/sources.py` & `paradigm-4.1.0/paradigm/_core/sources.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/stubs.py` & `paradigm-4.1.0/paradigm/_core/stubs.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm/_core/utils.py` & `paradigm-4.1.0/paradigm/_core/utils.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.1/paradigm.egg-info/PKG-INFO` & `paradigm-4.1.0/paradigm.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,49 @@
 Metadata-Version: 2.1
 Name: paradigm
-Version: 4.0.1
+Version: 4.1.0
 Summary: Python objects metadata parser.
 Home-page: https://github.com/lycantropos/paradigm/
 Download-URL: https://github.com/lycantropos/paradigm/archive/master.zip
-Author: Azat Ibrakov
-Author-email: azatibrakov@gmail.com
+Author-email: Azat Ibrakov <azatibrakov@gmail.com>
 License: MIT License
+        
+        Copyright (c) 2018 Azat Ibrakov
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 License-File: LICENSE
 
 paradigm
 ========
 
 [![](https://github.com/lycantropos/paradigm/workflows/CI/badge.svg)](https://github.com/lycantropos/paradigm/actions/workflows/ci.yml "Github Actions")
 [![](https://codecov.io/gh/lycantropos/paradigm/branch/master/graph/badge.svg)](https://codecov.io/gh/lycantropos/paradigm "Codecov")
```

### Comparing `paradigm-4.0.1/paradigm.egg-info/SOURCES.txt` & `paradigm-4.1.0/paradigm.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
-requirements.txt
+pyproject.toml
 setup.cfg
 setup.py
 paradigm/__init__.py
 paradigm/base.py
 paradigm/py.typed
 paradigm.egg-info/PKG-INFO
 paradigm.egg-info/SOURCES.txt
```

