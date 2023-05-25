# Comparing `tmp/marshmallow_peewee-4.2.2.tar.gz` & `tmp/marshmallow_peewee-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marshmallow_peewee-4.2.2.tar", max compression
+gzip compressed data, was "marshmallow_peewee-4.3.0.tar", max compression
```

## Comparing `marshmallow_peewee-4.2.2.tar` & `marshmallow_peewee-4.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4452 2023-05-02 08:53:16.212144 marshmallow_peewee-4.2.2/README.md
--rw-r--r--   0        0        0      302 2023-05-02 08:53:16.212144 marshmallow_peewee-4.2.2/marshmallow_peewee/__init__.py
--rw-r--r--   0        0        0      255 2023-05-02 08:53:16.212144 marshmallow_peewee-4.2.2/marshmallow_peewee/config.py
--rw-r--r--   0        0        0     5708 2023-05-02 08:53:16.212144 marshmallow_peewee-4.2.2/marshmallow_peewee/convert.py
--rw-r--r--   0        0        0     2786 2023-05-02 08:53:16.212144 marshmallow_peewee-4.2.2/marshmallow_peewee/fields.py
--rw-r--r--   0        0        0        0 2023-05-02 08:53:16.212144 marshmallow_peewee-4.2.2/marshmallow_peewee/py.typed
--rw-r--r--   0        0        0     4499 2023-05-02 08:53:16.212144 marshmallow_peewee-4.2.2/marshmallow_peewee/schema.py
--rw-r--r--   0        0        0      264 2023-05-02 08:53:16.212144 marshmallow_peewee-4.2.2/marshmallow_peewee/types.py
--rw-r--r--   0        0        0     1355 2023-05-02 08:53:16.212144 marshmallow_peewee-4.2.2/pyproject.toml
--rw-r--r--   0        0        0     5693 1970-01-01 00:00:00.000000 marshmallow_peewee-4.2.2/PKG-INFO
+-rw-r--r--   0        0        0     4452 2023-05-25 06:54:47.569647 marshmallow_peewee-4.3.0/README.md
+-rw-r--r--   0        0        0      302 2023-05-25 06:54:47.569647 marshmallow_peewee-4.3.0/marshmallow_peewee/__init__.py
+-rw-r--r--   0        0        0      255 2023-05-25 06:54:47.569647 marshmallow_peewee-4.3.0/marshmallow_peewee/config.py
+-rw-r--r--   0        0        0     5727 2023-05-25 06:54:47.569647 marshmallow_peewee-4.3.0/marshmallow_peewee/convert.py
+-rw-r--r--   0        0        0     2786 2023-05-25 06:54:47.569647 marshmallow_peewee-4.3.0/marshmallow_peewee/fields.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:54:47.569647 marshmallow_peewee-4.3.0/marshmallow_peewee/py.typed
+-rw-r--r--   0        0        0     4514 2023-05-25 06:54:47.569647 marshmallow_peewee-4.3.0/marshmallow_peewee/schema.py
+-rw-r--r--   0        0        0      264 2023-05-25 06:54:47.569647 marshmallow_peewee-4.3.0/marshmallow_peewee/types.py
+-rw-r--r--   0        0        0     1355 2023-05-25 06:54:47.569647 marshmallow_peewee-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 marshmallow_peewee-4.3.0/PKG-INFO
```

### Comparing `marshmallow_peewee-4.2.2/README.md` & `marshmallow_peewee-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `marshmallow_peewee-4.2.2/marshmallow_peewee/convert.py` & `marshmallow_peewee-4.3.0/marshmallow_peewee/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     """Convert Peewee model to Marshmallow schema."""
 
     TYPE_MAPPING: TFieldMappingList = []
 
     def __init__(self, opts: SchemaOpts):
         self.opts = opts
 
-    def get_fields(self, model: pw.Model) -> OrderedDict:
+    def get_fields(self, model: pw.Model) -> OrderedDict[str, fields.Field]:
         result = OrderedDict()
         meta = cast(pw.Metadata, model._meta)  # type: ignore[]
         for field in meta.sorted_fields:
             name = field.name
             if self.opts.id_keys and isinstance(field, pw.ForeignKeyField):
                 name = field.column_name
```

### Comparing `marshmallow_peewee-4.2.2/marshmallow_peewee/fields.py` & `marshmallow_peewee-4.3.0/marshmallow_peewee/fields.py`

 * *Files identical despite different names*

### Comparing `marshmallow_peewee-4.2.2/marshmallow_peewee/schema.py` & `marshmallow_peewee-4.3.0/marshmallow_peewee/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
 
 INHERITANCE_OPTIONS = (
     "model",
     "model_converter",
     "dump_only_pk",
     "string_keys",
+    "id_keys",
     # Basic options
     "datetimeformat",
     "dateformat",
     "timeformat",
     "unknown",
 )
```

### Comparing `marshmallow_peewee-4.2.2/pyproject.toml` & `marshmallow_peewee-4.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "marshmallow-peewee"
-version = "4.2.2"
+version = "4.3.0"
 description = "Peewee ORM integration with the Marshmallow (de)serialization library"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/klen/marshmallow-peewee"
 repository = "https://github.com/klen/marshmallow-peewee"
 keywords = ["marshmallow", "peewee", "orm", "serialization", "deserialization"]
@@ -21,16 +21,16 @@
 ]
 packages = [
     { include = "marshmallow_peewee" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-marshmallow = "^3.0.0"
 peewee = "^3.14.0"
+marshmallow = "^3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "*"
 
 [tool.poetry.group.tests.dependencies]
 pytest = "*"
 pytest-mypy = "*"
```

### Comparing `marshmallow_peewee-4.2.2/PKG-INFO` & `marshmallow_peewee-4.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marshmallow-peewee
-Version: 4.2.2
+Version: 4.3.0
 Summary: Peewee ORM integration with the Marshmallow (de)serialization library
 Home-page: https://github.com/klen/marshmallow-peewee
 License: MIT
 Keywords: marshmallow,peewee,orm,serialization,deserialization
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -13,19 +13,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: marshmallow (>=3.0.0,<4.0.0)
 Requires-Dist: peewee (>=3.14.0,<4.0.0)
 Project-URL: Repository, https://github.com/klen/marshmallow-peewee
 Description-Content-Type: text/markdown
 
 # Marshmallow-Peewee
```

