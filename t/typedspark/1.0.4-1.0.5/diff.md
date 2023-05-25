# Comparing `tmp/typedspark-1.0.4.tar.gz` & `tmp/typedspark-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedspark-1.0.4.tar", last modified: Wed May 24 19:58:59 2023, max compression
+gzip compressed data, was "typedspark-1.0.5.tar", last modified: Thu May 25 19:04:38 2023, max compression
```

## Comparing `typedspark-1.0.4.tar` & `typedspark-1.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:59.619227 typedspark-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 19:58:48.000000 typedspark-1.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-24 19:58:59.619227 typedspark-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-24 19:58:48.000000 typedspark-1.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-24 19:58:48.000000 typedspark-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 19:58:59.619227 typedspark-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-24 19:58:48.000000 typedspark-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:59.615227 typedspark-1.0.4/typedspark/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:59.615227 typedspark-1.0.4/typedspark/_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_core/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_core/column_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_core/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_core/validate_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:59.619227 typedspark-1.0.4/typedspark/_schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_schema/dlt_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_schema/get_schema_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_schema/get_schema_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_schema/structfield.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:59.619227 typedspark-1.0.4/typedspark/_transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_transforms/structtype_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_transforms/transform_to_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_transforms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:59.619227 typedspark-1.0.4/typedspark/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_utils/create_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_utils/load_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/_utils/register_schema_to_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:48.000000 typedspark-1.0.4/typedspark/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:58:59.615227 typedspark-1.0.4/typedspark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-24 19:58:59.000000 typedspark-1.0.4/typedspark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-24 19:58:59.000000 typedspark-1.0.4/typedspark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 19:58:59.000000 typedspark-1.0.4/typedspark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-24 19:58:59.000000 typedspark-1.0.4/typedspark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 19:58:59.000000 typedspark-1.0.4/typedspark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:04:38.484933 typedspark-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 19:04:26.000000 typedspark-1.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-25 19:04:38.484933 typedspark-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-25 19:04:26.000000 typedspark-1.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-25 19:04:26.000000 typedspark-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 19:04:38.484933 typedspark-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-25 19:04:26.000000 typedspark-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:04:38.480932 typedspark-1.0.5/typedspark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:04:38.480932 typedspark-1.0.5/typedspark/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_core/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_core/column_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_core/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_core/validate_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:04:38.484933 typedspark-1.0.5/typedspark/_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_schema/dlt_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_schema/get_schema_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_schema/get_schema_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_schema/structfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:04:38.484933 typedspark-1.0.5/typedspark/_transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_transforms/structtype_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_transforms/transform_to_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_transforms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:04:38.484933 typedspark-1.0.5/typedspark/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_utils/create_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_utils/load_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/_utils/register_schema_to_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:04:26.000000 typedspark-1.0.5/typedspark/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:04:38.480932 typedspark-1.0.5/typedspark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-25 19:04:38.000000 typedspark-1.0.5/typedspark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-25 19:04:38.000000 typedspark-1.0.5/typedspark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:04:38.000000 typedspark-1.0.5/typedspark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 19:04:38.000000 typedspark-1.0.5/typedspark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 19:04:38.000000 typedspark-1.0.5/typedspark.egg-info/top_level.txt
```

### Comparing `typedspark-1.0.4/LICENSE.txt` & `typedspark-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/PKG-INFO` & `typedspark-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedspark
-Version: 1.0.4
+Version: 1.0.5
 Summary: Column-wise type annotations for pyspark DataFrames
 Home-page: https://github.com/kaiko-ai/typedspark
 Author: Nanne Aben
 Author-email: nanne@kaiko.ai
 License: Apache-2.0
 Keywords: pyspark spark typing type checking annotations
 Classifier: Programming Language :: Python
```

### Comparing `typedspark-1.0.4/README.rst` & `typedspark-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/pyproject.toml` & `typedspark-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/setup.py` & `typedspark-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/typedspark/__init__.py` & `typedspark-1.0.5/typedspark/__init__.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/typedspark/_core/column.py` & `typedspark-1.0.5/typedspark/_core/column.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/typedspark/_core/column_meta.py` & `typedspark-1.0.5/typedspark/_core/column_meta.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/typedspark/_core/dataset.py` & `typedspark-1.0.5/typedspark/_core/dataset.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/typedspark/_core/datatypes.py` & `typedspark-1.0.5/typedspark/_core/datatypes.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/typedspark/_core/validate_schema.py` & `typedspark-1.0.5/typedspark/_core/validate_schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/typedspark/_schema/get_schema_definition.py` & `typedspark-1.0.5/typedspark/_schema/get_schema_definition.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/typedspark/_schema/get_schema_imports.py` & `typedspark-1.0.5/typedspark/_schema/get_schema_imports.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/typedspark/_schema/schema.py` & `typedspark-1.0.5/typedspark/_schema/schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/typedspark/_schema/structfield.py` & `typedspark-1.0.5/typedspark/_schema/structfield.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/typedspark/_transforms/structtype_column.py` & `typedspark-1.0.5/typedspark/_transforms/structtype_column.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/typedspark/_transforms/transform_to_schema.py` & `typedspark-1.0.5/typedspark/_transforms/transform_to_schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/typedspark/_transforms/utils.py` & `typedspark-1.0.5/typedspark/_transforms/utils.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/typedspark/_utils/create_dataset.py` & `typedspark-1.0.5/typedspark/_utils/create_dataset.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/typedspark/_utils/load_table.py` & `typedspark-1.0.5/typedspark/_utils/load_table.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/typedspark/_utils/register_schema_to_dataset.py` & `typedspark-1.0.5/typedspark/_utils/register_schema_to_dataset.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.4/typedspark.egg-info/PKG-INFO` & `typedspark-1.0.5/typedspark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedspark
-Version: 1.0.4
+Version: 1.0.5
 Summary: Column-wise type annotations for pyspark DataFrames
 Home-page: https://github.com/kaiko-ai/typedspark
 Author: Nanne Aben
 Author-email: nanne@kaiko.ai
 License: Apache-2.0
 Keywords: pyspark spark typing type checking annotations
 Classifier: Programming Language :: Python
```

### Comparing `typedspark-1.0.4/typedspark.egg-info/SOURCES.txt` & `typedspark-1.0.5/typedspark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

