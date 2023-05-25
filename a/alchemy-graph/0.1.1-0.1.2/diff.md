# Comparing `tmp/alchemy_graph-0.1.1.tar.gz` & `tmp/alchemy_graph-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchemy_graph-0.1.1.tar", max compression
+gzip compressed data, was "alchemy_graph-0.1.2.tar", max compression
```

## Comparing `alchemy_graph-0.1.1.tar` & `alchemy_graph-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-05-17 13:31:02.080130 alchemy_graph-0.1.1/LICENSE
--rw-r--r--   0        0        0     2725 2023-05-17 13:31:02.080130 alchemy_graph-0.1.1/README.md
--rw-r--r--   0        0        0      268 2023-05-17 13:31:02.080130 alchemy_graph-0.1.1/alchemy_graph/__init__.py
--rw-r--r--   0        0        0       22 2023-05-17 13:31:02.080130 alchemy_graph-0.1.1/alchemy_graph/__version__.py
--rw-r--r--   0        0        0     6844 2023-05-17 13:31:02.080130 alchemy_graph-0.1.1/alchemy_graph/main.py
--rw-r--r--   0        0        0     3279 2023-05-17 13:31:02.080130 alchemy_graph-0.1.1/alchemy_graph/utils.py
--rw-r--r--   0        0        0     1599 2023-05-17 13:31:02.080130 alchemy_graph-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2651 2023-05-17 13:31:02.080130 alchemy_graph-0.1.1/tests/test_utils.py
--rw-r--r--   0        0        0     3804 1970-01-01 00:00:00.000000 alchemy_graph-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-25 16:53:32.336463 alchemy_graph-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3183 2023-05-25 16:53:32.336463 alchemy_graph-0.1.2/README.md
+-rw-r--r--   0        0        0      268 2023-05-25 16:53:32.336463 alchemy_graph-0.1.2/alchemy_graph/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-25 16:53:32.336463 alchemy_graph-0.1.2/alchemy_graph/__version__.py
+-rw-r--r--   0        0        0     6844 2023-05-25 16:53:32.336463 alchemy_graph-0.1.2/alchemy_graph/main.py
+-rw-r--r--   0        0        0     3279 2023-05-25 16:53:32.336463 alchemy_graph-0.1.2/alchemy_graph/utils.py
+-rw-r--r--   0        0        0     1656 2023-05-25 16:53:32.336463 alchemy_graph-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2651 2023-05-25 16:53:32.336463 alchemy_graph-0.1.2/tests/test_utils.py
+-rw-r--r--   0        0        0     4160 1970-01-01 00:00:00.000000 alchemy_graph-0.1.2/PKG-INFO
```

### Comparing `alchemy_graph-0.1.1/LICENSE` & `alchemy_graph-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alchemy_graph-0.1.1/alchemy_graph/main.py` & `alchemy_graph-0.1.2/alchemy_graph/main.py`

 * *Files identical despite different names*

### Comparing `alchemy_graph-0.1.1/alchemy_graph/utils.py` & `alchemy_graph-0.1.2/alchemy_graph/utils.py`

 * *Files identical despite different names*

### Comparing `alchemy_graph-0.1.1/pyproject.toml` & `alchemy_graph-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alchemy_graph"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Kiel Ed <kieledssh@gmail.com>"]
 readme = "README.md"
 keywords = ["strawberry-graphql", "sqlalchemy-mapper", "sqlalchemy", "strawberry", "mapper", "dict"]
 homepage = "https://github.com/kieled/alchemy_graph"
 repository = "https://github.com/kieled/alchemy_graph"
 packages = [
@@ -19,17 +19,17 @@
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Intended Audience :: Developers",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-sqlalchemy = "^2.0.12"
+sqlalchemy = "^2.0.15"
 fastapi = "^0.95.2"
-strawberry-graphql = { extras = ["fastapi"], version = "^0.177.1" }
+strawberry-graphql = { extras = ["fastapi"], version = "^0.178.0" }
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.264"
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 pre-commit = "^3.3.1"
@@ -69,7 +69,10 @@
     "B",
 ]
 ignore = [
     "E501",
     "B008",
     "C901",
 ]
+
+[tool.ruff.isort]
+known-third-party = ["alchemy_graph"]
```

### Comparing `alchemy_graph-0.1.1/tests/test_utils.py` & `alchemy_graph-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `alchemy_graph-0.1.1/PKG-INFO` & `alchemy_graph-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 Metadata-Version: 2.1
 Name: alchemy-graph
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Home-page: https://github.com/kieled/alchemy_graph
 Keywords: strawberry-graphql,sqlalchemy-mapper,sqlalchemy,strawberry,mapper,dict
 Author: Kiel Ed
 Author-email: kieledssh@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: fastapi (>=0.95.2,<0.96.0)
-Requires-Dist: sqlalchemy (>=2.0.12,<3.0.0)
-Requires-Dist: strawberry-graphql[fastapi] (>=0.177.1,<0.178.0)
+Requires-Dist: sqlalchemy (>=2.0.15,<3.0.0)
+Requires-Dist: strawberry-graphql[fastapi] (>=0.178.0,<0.179.0)
 Project-URL: Repository, https://github.com/kieled/alchemy_graph
 Description-Content-Type: text/markdown
 
 <h2 align="center">:small_red_triangle: alchemy_graph :small_red_triangle:</h2>
 
 ![New Project](https://user-images.githubusercontent.com/68655454/236483334-a3c86f5c-f732-4465-bf78-692ddd4609b2.png)
 
 <p align="center">
- <a href="https://github.com/kieled/alchemy_graph/actions/workflows/test.yml" alt="GitFlow">
+    <a href="https://pypi.python.org/pypi/alchemy_graph" alt="PyPi Package Version">
+        <img src="https://img.shields.io/pypi/v/alchemy_graph.svg" /></a>
+    <a href="https://pypi.python.org/pypi/alchemy_graph" alt="Supported Python versions">
+        <img src="https://img.shields.io/pypi/pyversions/alchemy_graph.svg" /></a>
+    <a href="https://github.com/kieled/alchemy_graph/actions/workflows/test.yml" alt="GitFlow">
         <img src="https://github.com/kieled/alchemy_graph/actions/workflows/test.yml/badge.svg" /></a>
 </p>
 
-SQLAlchemy mapper to Strawberry types
+<p align="center">SQLAlchemy mapper to Strawberry types</p>
+
+
+## :pencil2: Installation
+You can install mapper using pip:
+
+```bash
+pip install alchemy-graph
+```
 
 ## Functions:
 ### `get_only_selected_fields`
 Given a SQLAlchemy model class and a Strawberry Info object representing a selection set, returns a SQLAlchemy Select object that loads only the fields and relations specified in the selection set.
 
 #### Parameters:
```

#### html2text {}

```diff
@@ -1,50 +1,52 @@
-Metadata-Version: 2.1 Name: alchemy-graph Version: 0.1.1 Summary: Home-page:
+Metadata-Version: 2.1 Name: alchemy-graph Version: 0.1.2 Summary: Home-page:
 https://github.com/kieled/alchemy_graph Keywords: strawberry-
 graphql,sqlalchemy-mapper,sqlalchemy,strawberry,mapper,dict Author: Kiel Ed
 Author-email: kieledssh@gmail.com Requires-Python: >=3.10,<4.0 Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
-PyPy Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: fastapi (>=0.95.2,<0.96.0) Requires-Dist: sqlalchemy
-(>=2.0.12,<3.0.0) Requires-Dist: strawberry-graphql[fastapi]
-(>=0.177.1,<0.178.0) Project-URL: Repository, https://github.com/kieled/
-alchemy_graph Description-Content-Type: text/markdown
+Programming Language :: Python :: Implementation :: PyPy Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Requires-Dist: fastapi
+(>=0.95.2,<0.96.0) Requires-Dist: sqlalchemy (>=2.0.15,<3.0.0) Requires-Dist:
+strawberry-graphql[fastapi] (>=0.178.0,<0.179.0) Project-URL: Repository,
+https://github.com/kieled/alchemy_graph Description-Content-Type: text/markdown
       ***** :small_red_triangle: alchemy_graph :small_red_triangle: *****
 ![New Project](https://user-images.githubusercontent.com/68655454/236483334-
 a3c86f5c-f732-4465-bf78-692ddd4609b2.png)
-[https://github.com/kieled/alchemy_graph/actions/workflows/test.yml/badge.svg]
-SQLAlchemy mapper to Strawberry types ## Functions: ###
-`get_only_selected_fields` Given a SQLAlchemy model class and a Strawberry Info
-object representing a selection set, returns a SQLAlchemy Select object that
-loads only the fields and relations specified in the selection set. ####
-Parameters: - sqlalchemy_class: The SQLAlchemy model class to select fields
-from. - info: The Strawberry Info object representing the selection set. -
-inner_selection_name: The name of an inner selection set to consider. If
-specified, only fields and relations under this selection set will be included
-in the Select object. #### Returns: A SQLAlchemy Select object that loads only
-the specified fields and relations. ### `orm_to_strawberry` Function maps
-sqlalchemy model to strawberry class. #### Parameters: - input_data: SqlAlchemy
-Base Model or list of base models. - strawberry_type: Strawberry class wrapped
-in strawberry.input or strawberry.type. #### Returns: Strawberry objects or
-list of them. ### `strawberry_to_dict` Given a Strawberry object and an
-optional list of allowed keys, returns a dictionary representation of the
-object. #### Parameters: - `obj`: A Strawberry object to convert to a
-dictionary. - `allowed_keys`: An optional list of keys to include in the output
-dictionary. If not specified, all keys are included. #### Returns: A dictionary
-representation of the input object. ### `orm_mapper` Function returns decorator
-for your Query strawberry.field(). #### Parameters: - `strawberry_type`:
-Strawberry type that should be return. Required if result_to_strawberry=True. -
-`inject_query`: Inject into current function SqlAlchemy Query. Default value:
-False. - `sqlalchemy_class`: SqlAlchemy model class. - `inner_selection_name`:
-The name of an inner selection set to consider. If specified, only fields and
-relations under this selection set will be included in the Select object. -
+[https://img.shields.io/pypi/v/alchemy_graph.svg] [https://img.shields.io/pypi/
+pyversions/alchemy_graph.svg] [https://github.com/kieled/alchemy_graph/actions/
+                         workflows/test.yml/badge.svg]
+                     SQLAlchemy mapper to Strawberry types
+## :pencil2: Installation You can install mapper using pip: ```bash pip install
+alchemy-graph ``` ## Functions: ### `get_only_selected_fields` Given a
+SQLAlchemy model class and a Strawberry Info object representing a selection
+set, returns a SQLAlchemy Select object that loads only the fields and
+relations specified in the selection set. #### Parameters: - sqlalchemy_class:
+The SQLAlchemy model class to select fields from. - info: The Strawberry Info
+object representing the selection set. - inner_selection_name: The name of an
+inner selection set to consider. If specified, only fields and relations under
+this selection set will be included in the Select object. #### Returns: A
+SQLAlchemy Select object that loads only the specified fields and relations.
+### `orm_to_strawberry` Function maps sqlalchemy model to strawberry class.
+#### Parameters: - input_data: SqlAlchemy Base Model or list of base models. -
+strawberry_type: Strawberry class wrapped in strawberry.input or
+strawberry.type. #### Returns: Strawberry objects or list of them. ###
+`strawberry_to_dict` Given a Strawberry object and an optional list of allowed
+keys, returns a dictionary representation of the object. #### Parameters: -
+`obj`: A Strawberry object to convert to a dictionary. - `allowed_keys`: An
+optional list of keys to include in the output dictionary. If not specified,
+all keys are included. #### Returns: A dictionary representation of the input
+object. ### `orm_mapper` Function returns decorator for your Query
+strawberry.field(). #### Parameters: - `strawberry_type`: Strawberry type that
+should be return. Required if result_to_strawberry=True. - `inject_query`:
+Inject into current function SqlAlchemy Query. Default value: False. -
+`sqlalchemy_class`: SqlAlchemy model class. - `inner_selection_name`: The name
+of an inner selection set to consider. If specified, only fields and relations
+under this selection set will be included in the Select object. -
 `result_to_strawberry`: If True, it returns Strawberry object(s). Default
 value: True. ### `get_dict_object` Given an SQLAlchemy object, returns a
 dictionary representation of the object. #### Parameters: - `obj`: An
 SQLAlchemy object to convert to a dictionary. #### Returns: A dictionary
 representation of the input object. ## LICENSE This project is licensed under
 the terms of the MIT license.
```

