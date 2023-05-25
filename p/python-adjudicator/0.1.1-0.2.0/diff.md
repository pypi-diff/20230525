# Comparing `tmp/python_adjudicator-0.1.1.tar.gz` & `tmp/python_adjudicator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_adjudicator-0.1.1.tar", max compression
+gzip compressed data, was "python_adjudicator-0.2.0.tar", max compression
```

## Comparing `python_adjudicator-0.1.1.tar` & `python_adjudicator-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      988 2023-05-19 08:45:58.545191 python_adjudicator-0.1.1/LICENSE
--rw-r--r--   0        0        0     2560 2023-05-19 09:34:38.810342 python_adjudicator-0.1.1/README.md
--rw-r--r--   0        0        0     1852 2023-05-19 09:52:38.123361 python_adjudicator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2019 2023-05-19 08:50:35.058438 python_adjudicator-0.1.1/src/adjudicator/Cache.py
--rw-r--r--   0        0        0     3137 2023-05-19 08:50:35.058438 python_adjudicator-0.1.1/src/adjudicator/Executor.py
--rw-r--r--   0        0        0     1530 2023-05-19 09:42:57.372585 python_adjudicator-0.1.1/src/adjudicator/HashSupport.py
--rw-r--r--   0        0        0     5579 2023-05-19 09:50:25.658731 python_adjudicator-0.1.1/src/adjudicator/Params.py
--rw-r--r--   0        0        0      892 2023-05-19 08:51:12.194651 python_adjudicator-0.1.1/src/adjudicator/Params_test.py
--rw-r--r--   0        0        0     3687 2023-05-19 08:50:35.062438 python_adjudicator-0.1.1/src/adjudicator/Rule.py
--rw-r--r--   0        0        0      411 2023-05-19 08:50:35.062438 python_adjudicator-0.1.1/src/adjudicator/Rule_test.py
--rw-r--r--   0        0        0     4385 2023-05-19 09:51:54.739163 python_adjudicator-0.1.1/src/adjudicator/RulesEngine.py
--rw-r--r--   0        0        0     2643 2023-05-19 09:37:37.623158 python_adjudicator-0.1.1/src/adjudicator/RulesEngine_test.py
--rw-r--r--   0        0        0     3036 2023-05-19 08:50:35.090438 python_adjudicator-0.1.1/src/adjudicator/RulesGraph.py
--rw-r--r--   0        0        0     2615 2023-05-19 08:50:35.062438 python_adjudicator-0.1.1/src/adjudicator/RulesGraph_test.py
--rw-r--r--   0        0        0      420 2023-05-16 21:13:35.338396 python_adjudicator-0.1.1/src/adjudicator/Signature.py
--rw-r--r--   0        0        0      682 2023-05-19 09:52:38.123361 python_adjudicator-0.1.1/src/adjudicator/__init__.py
--rw-r--r--   0        0        0     1397 2023-05-19 08:50:35.062438 python_adjudicator-0.1.1/src/adjudicator/errors.py
--rw-r--r--   0        0        0        0 2023-05-19 08:45:58.549191 python_adjudicator-0.1.1/src/adjudicator/py.typed
--rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 python_adjudicator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-05-19 08:45:58.545191 python_adjudicator-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2560 2023-05-19 09:34:38.810342 python_adjudicator-0.2.0/README.md
+-rw-r--r--   0        0        0     1852 2023-05-25 21:39:30.539279 python_adjudicator-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2019 2023-05-19 08:50:35.058438 python_adjudicator-0.2.0/src/adjudicator/Cache.py
+-rw-r--r--   0        0        0     3137 2023-05-19 08:50:35.058438 python_adjudicator-0.2.0/src/adjudicator/Executor.py
+-rw-r--r--   0        0        0     1530 2023-05-19 09:42:57.372585 python_adjudicator-0.2.0/src/adjudicator/HashSupport.py
+-rw-r--r--   0        0        0     5579 2023-05-19 09:50:25.658731 python_adjudicator-0.2.0/src/adjudicator/Params.py
+-rw-r--r--   0        0        0      892 2023-05-19 08:51:12.194651 python_adjudicator-0.2.0/src/adjudicator/Params_test.py
+-rw-r--r--   0        0        0     4652 2023-05-25 21:37:23.072475 python_adjudicator-0.2.0/src/adjudicator/Rule.py
+-rw-r--r--   0        0        0      739 2023-05-25 21:37:23.012476 python_adjudicator-0.2.0/src/adjudicator/Rule_test.py
+-rw-r--r--   0        0        0     4385 2023-05-19 09:51:54.739163 python_adjudicator-0.2.0/src/adjudicator/RulesEngine.py
+-rw-r--r--   0        0        0     2643 2023-05-19 09:37:37.623158 python_adjudicator-0.2.0/src/adjudicator/RulesEngine_test.py
+-rw-r--r--   0        0        0     3036 2023-05-19 08:50:35.090438 python_adjudicator-0.2.0/src/adjudicator/RulesGraph.py
+-rw-r--r--   0        0        0     2615 2023-05-19 08:50:35.062438 python_adjudicator-0.2.0/src/adjudicator/RulesGraph_test.py
+-rw-r--r--   0        0        0      420 2023-05-16 21:13:35.338396 python_adjudicator-0.2.0/src/adjudicator/Signature.py
+-rw-r--r--   0        0        0      682 2023-05-25 21:39:30.539279 python_adjudicator-0.2.0/src/adjudicator/__init__.py
+-rw-r--r--   0        0        0     1397 2023-05-19 08:50:35.062438 python_adjudicator-0.2.0/src/adjudicator/errors.py
+-rw-r--r--   0        0        0        0 2023-05-19 08:45:58.549191 python_adjudicator-0.2.0/src/adjudicator/py.typed
+-rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 python_adjudicator-0.2.0/PKG-INFO
```

### Comparing `python_adjudicator-0.1.1/LICENSE` & `python_adjudicator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.1/README.md` & `python_adjudicator-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.1/pyproject.toml` & `python_adjudicator-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python-adjudicator"
-version = "0.1.1"
+version = "0.2.0"
 description = ""
 authors = ["Unknown <me@unknown.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "adjudicator", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `python_adjudicator-0.1.1/src/adjudicator/Cache.py` & `python_adjudicator-0.2.0/src/adjudicator/Cache.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.1/src/adjudicator/Executor.py` & `python_adjudicator-0.2.0/src/adjudicator/Executor.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.1/src/adjudicator/HashSupport.py` & `python_adjudicator-0.2.0/src/adjudicator/HashSupport.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.1/src/adjudicator/Params.py` & `python_adjudicator-0.2.0/src/adjudicator/Params.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.1/src/adjudicator/Params_test.py` & `python_adjudicator-0.2.0/src/adjudicator/Params_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.1/src/adjudicator/RulesEngine.py` & `python_adjudicator-0.2.0/src/adjudicator/RulesEngine.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.1/src/adjudicator/RulesEngine_test.py` & `python_adjudicator-0.2.0/src/adjudicator/RulesEngine_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.1/src/adjudicator/RulesGraph.py` & `python_adjudicator-0.2.0/src/adjudicator/RulesGraph.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.1/src/adjudicator/RulesGraph_test.py` & `python_adjudicator-0.2.0/src/adjudicator/RulesGraph_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.1/src/adjudicator/__init__.py` & `python_adjudicator-0.2.0/src/adjudicator/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,8 +21,8 @@
     "rule",
     "Rule",
     "RuleResolveError",
     "RulesEngine",
     "RulesGraph",
 ]
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
```

### Comparing `python_adjudicator-0.1.1/src/adjudicator/errors.py` & `python_adjudicator-0.2.0/src/adjudicator/errors.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.1/PKG-INFO` & `python_adjudicator-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-adjudicator
-Version: 0.1.1
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Unknown
 Author-email: me@unknown.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

