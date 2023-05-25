# Comparing `tmp/pylity-0.0.8.tar.gz` & `tmp/pylity-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylity-0.0.8.tar", max compression
+gzip compressed data, was "pylity-0.0.9.tar", max compression
```

## Comparing `pylity-0.0.8.tar` & `pylity-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-04-18 17:04:39.770426 pylity-0.0.8/LICENSE
--rw-r--r--   0        0        0     5109 2023-04-18 17:04:39.770426 pylity-0.0.8/README.md
--rw-r--r--   0        0        0      882 2023-04-18 17:04:39.770426 pylity-0.0.8/pylity/Async.py
--rw-r--r--   0        0        0     1035 2023-04-18 17:04:39.770426 pylity-0.0.8/pylity/Collection.py
--rw-r--r--   0        0        0     4509 2023-04-18 17:04:39.770426 pylity-0.0.8/pylity/Function.py
--rw-r--r--   0        0        0     4819 2023-04-18 17:04:39.770426 pylity-0.0.8/pylity/Path.py
--rw-r--r--   0        0        0      473 2023-04-18 17:04:39.770426 pylity-0.0.8/pylity/String.py
--rw-r--r--   0        0        0      116 2023-04-18 17:04:39.770426 pylity-0.0.8/pylity/__init__.py
--rw-r--r--   0        0        0     2733 2023-04-18 17:04:39.770426 pylity-0.0.8/pylity/decorators/validate_func_params.py
--rw-r--r--   0        0        0      731 2023-04-18 17:04:39.770426 pylity-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5875 1970-01-01 00:00:00.000000 pylity-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-18 22:22:57.487148 pylity-0.0.9/LICENSE
+-rw-r--r--   0        0        0     5109 2023-04-18 22:22:57.487148 pylity-0.0.9/README.md
+-rw-r--r--   0        0        0      882 2023-04-18 22:22:57.487148 pylity-0.0.9/pylity/Async.py
+-rw-r--r--   0        0        0     1035 2023-04-18 22:22:57.487148 pylity-0.0.9/pylity/Collection.py
+-rw-r--r--   0        0        0     4509 2023-04-18 22:22:57.487148 pylity-0.0.9/pylity/Function.py
+-rw-r--r--   0        0        0     4819 2023-04-18 22:22:57.487148 pylity-0.0.9/pylity/Path.py
+-rw-r--r--   0        0        0      473 2023-04-18 22:22:57.487148 pylity-0.0.9/pylity/String.py
+-rw-r--r--   0        0        0      116 2023-04-18 22:22:57.487148 pylity-0.0.9/pylity/__init__.py
+-rw-r--r--   0        0        0     4929 2023-04-18 22:22:57.487148 pylity-0.0.9/pylity/decorators/validate_func_params.py
+-rw-r--r--   0        0        0      731 2023-04-18 22:22:57.487148 pylity-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5875 1970-01-01 00:00:00.000000 pylity-0.0.9/PKG-INFO
```

### Comparing `pylity-0.0.8/LICENSE` & `pylity-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pylity-0.0.8/README.md` & `pylity-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pylity-0.0.8/pylity/Async.py` & `pylity-0.0.9/pylity/Async.py`

 * *Files identical despite different names*

### Comparing `pylity-0.0.8/pylity/Collection.py` & `pylity-0.0.9/pylity/Collection.py`

 * *Files identical despite different names*

### Comparing `pylity-0.0.8/pylity/Function.py` & `pylity-0.0.9/pylity/Function.py`

 * *Files identical despite different names*

### Comparing `pylity-0.0.8/pylity/Path.py` & `pylity-0.0.9/pylity/Path.py`

 * *Files identical despite different names*

### Comparing `pylity-0.0.8/pyproject.toml` & `pylity-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # https://python-poetry.org/docs/pyproject/
 [tool.poetry]
 name = "pylity"
-version = "0.0.8"
+version = "0.0.9"
 description = "A collection of utility functions for Python. pylity means Python Utility "
 authors = ["Payadel <payadelteam@gmail.com>"]
 license = "GPLV3"
 readme = "README.md"
 repository = "https://github.com/Payadel/pylity"
 keywords = ['utility', 'helpers']
 packages = [{ include = "pylity" }]
```

### Comparing `pylity-0.0.8/PKG-INFO` & `pylity-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylity
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of utility functions for Python. pylity means Python Utility 
 Home-page: https://github.com/Payadel/pylity
 License: GPLV3
 Keywords: utility,helpers
 Author: Payadel
 Author-email: payadelteam@gmail.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylity Version: 0.0.8 Summary: A collection of
+Metadata-Version: 2.1 Name: pylity Version: 0.0.9 Summary: A collection of
 utility functions for Python. pylity means Python Utility Home-page: https://
 github.com/Payadel/pylity License: GPLV3 Keywords: utility,helpers Author:
 Payadel Author-email: payadelteam@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

