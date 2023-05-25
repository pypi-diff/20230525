# Comparing `tmp/arcane_datastore-1.1.2.tar.gz` & `tmp/arcane_datastore-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcane_datastore-1.1.2.tar", max compression
+gzip compressed data, was "arcane_datastore-1.1.3.tar", max compression
```

## Comparing `arcane_datastore-1.1.2.tar` & `arcane_datastore-1.1.3.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0      554 2022-12-28 09:20:16.066571 arcane_datastore-1.1.2/README.md
--rw-r--r--   0        0        0       46 2022-12-28 09:20:16.066571 arcane_datastore-1.1.2/arcane/datastore/__init__.py
--rw-r--r--   0        0        0      226 2022-12-28 09:20:16.066571 arcane_datastore-1.1.2/arcane/datastore/const.py
--rw-r--r--   0        0        0     5521 2022-12-28 09:20:16.066571 arcane_datastore-1.1.2/arcane/datastore/datastore.py
--rw-r--r--   0        0        0      440 2022-12-28 09:20:16.066571 arcane_datastore-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 arcane_datastore-1.1.2/setup.py
--rw-r--r--   0        0        0     1208 1970-01-01 00:00:00.000000 arcane_datastore-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      554 2023-05-25 07:43:22.679298 arcane_datastore-1.1.3/README.md
+-rw-r--r--   0        0        0       46 2023-05-25 07:43:22.679298 arcane_datastore-1.1.3/arcane/datastore/__init__.py
+-rw-r--r--   0        0        0      325 2023-05-25 07:43:22.679298 arcane_datastore-1.1.3/arcane/datastore/const.py
+-rw-r--r--   0        0        0     5521 2023-05-25 07:43:22.679298 arcane_datastore-1.1.3/arcane/datastore/datastore.py
+-rw-r--r--   0        0        0      440 2023-05-25 07:43:22.679298 arcane_datastore-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1208 1970-01-01 00:00:00.000000 arcane_datastore-1.1.3/PKG-INFO
```

### Comparing `arcane_datastore-1.1.2/README.md` & `arcane_datastore-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `arcane_datastore-1.1.2/arcane/datastore/datastore.py` & `arcane_datastore-1.1.3/arcane/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `arcane_datastore-1.1.2/PKG-INFO` & `arcane_datastore-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcane-datastore
-Version: 1.1.2
+Version: 1.1.3
 Summary: Override datastore client
 Author: Arcane
 Author-email: product@arcane.run
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

