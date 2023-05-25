# Comparing `tmp/ols_py-0.2.6.tar.gz` & `tmp/ols_py-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ols_py-0.2.6.tar", max compression
+gzip compressed data, was "ols_py-0.2.7.tar", max compression
```

## Comparing `ols_py-0.2.6.tar` & `ols_py-0.2.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3406 2023-05-17 03:38:57.503710 ols_py-0.2.6/README.md
--rw-r--r--   0        0        0     2167 2023-05-17 03:38:57.503710 ols_py-0.2.6/pyproject.toml
--rw-r--r--   0        0        0       55 2023-05-17 03:38:57.503710 ols_py-0.2.6/src/ols_py/__init__.py
--rw-r--r--   0        0        0    10705 2023-05-17 03:38:57.503710 ols_py-0.2.6/src/ols_py/client.py
--rw-r--r--   0        0        0     1596 2023-05-17 03:38:57.503710 ols_py-0.2.6/src/ols_py/instances.py
--rw-r--r--   0        0        0        0 2023-05-17 03:38:57.503710 ols_py-0.2.6/src/ols_py/py.typed
--rw-r--r--   0        0        0       89 2023-05-17 03:38:57.503710 ols_py-0.2.6/src/ols_py/schemas/__init__.py
--rw-r--r--   0        0        0      408 2023-05-17 03:38:57.503710 ols_py-0.2.6/src/ols_py/schemas/common.py
--rw-r--r--   0        0        0     4197 2023-05-17 03:38:57.503710 ols_py-0.2.6/src/ols_py/schemas/requests.py
--rw-r--r--   0        0        0     3752 2023-05-17 03:38:57.503710 ols_py-0.2.6/src/ols_py/schemas/responses.py
--rw-r--r--   0        0        0     4461 1970-01-01 00:00:00.000000 ols_py-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     3406 2023-05-25 01:48:00.900427 ols_py-0.2.7/README.md
+-rw-r--r--   0        0        0     2167 2023-05-25 01:48:00.900427 ols_py-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0       55 2023-05-25 01:48:00.900427 ols_py-0.2.7/src/ols_py/__init__.py
+-rw-r--r--   0        0        0    10705 2023-05-25 01:48:00.900427 ols_py-0.2.7/src/ols_py/client.py
+-rw-r--r--   0        0        0     1596 2023-05-25 01:48:00.900427 ols_py-0.2.7/src/ols_py/instances.py
+-rw-r--r--   0        0        0        0 2023-05-25 01:48:00.900427 ols_py-0.2.7/src/ols_py/py.typed
+-rw-r--r--   0        0        0       89 2023-05-25 01:48:00.900427 ols_py-0.2.7/src/ols_py/schemas/__init__.py
+-rw-r--r--   0        0        0      408 2023-05-25 01:48:00.900427 ols_py-0.2.7/src/ols_py/schemas/common.py
+-rw-r--r--   0        0        0     4219 2023-05-25 01:48:00.900427 ols_py-0.2.7/src/ols_py/schemas/requests.py
+-rw-r--r--   0        0        0     3752 2023-05-25 01:48:00.900427 ols_py-0.2.7/src/ols_py/schemas/responses.py
+-rw-r--r--   0        0        0     4413 1970-01-01 00:00:00.000000 ols_py-0.2.7/PKG-INFO
```

### Comparing `ols_py-0.2.6/README.md` & `ols_py-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ols_py-0.2.6/pyproject.toml` & `ols_py-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ols-py"
-version = "0.2.6"
+version = "0.2.7"
 description = "Python client for the Ontology Lookup Service"
 authors = [
     "Marius Mather <marius.mather@sydney.edu.au>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `ols_py-0.2.6/src/ols_py/client.py` & `ols_py-0.2.7/src/ols_py/client.py`

 * *Files identical despite different names*

### Comparing `ols_py-0.2.6/src/ols_py/instances.py` & `ols_py-0.2.7/src/ols_py/instances.py`

 * *Files identical despite different names*

### Comparing `ols_py-0.2.6/src/ols_py/schemas/requests.py` & `ols_py-0.2.7/src/ols_py/schemas/requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     ontology: Optional[list[str]]
     """Ontologies to search, e.g. `["mondo", "upheno"]`"""
     type: Optional[EntityType]
     """Type of term to search for, e.g. "class", "property" """
     slim: Optional[list[str]]
     fieldList: Optional[list[SearchReturnFields | AnnotationFieldName]]
     """Which fields to return in the results"""
-    queryFields: Optional[list[SearchQueryFields]]
+    queryFields: Optional[list[SearchQueryFields | AnnotationFieldName]]
     """Which fields to search over"""
     exact: Optional[bool]
     groupField: Optional[bool]
     """Group results by unique ID"""
     obsoletes: Optional[bool]
     """Include obsoleted terms in the results"""
     local: Optional[bool]
```

### Comparing `ols_py-0.2.6/src/ols_py/schemas/responses.py` & `ols_py-0.2.7/src/ols_py/schemas/responses.py`

 * *Files identical despite different names*

### Comparing `ols_py-0.2.6/PKG-INFO` & `ols_py-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: ols-py
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python client for the Ontology Lookup Service
 Home-page: https://ahida-development.github.io/ols-py
 License: MIT
 Author: Marius Mather
 Author-email: marius.mather@sydney.edu.au
 Requires-Python: >=3.10.1,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: requests (>=2.0,<3.0)
 Project-URL: Documentation, https://ahida-development.github.io/ols-py
 Project-URL: Repository, https://github.com/ahida-development/ols-py
```

