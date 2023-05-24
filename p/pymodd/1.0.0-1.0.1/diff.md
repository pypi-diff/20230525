# Comparing `tmp/pymodd-1.0.0.tar.gz` & `tmp/pymodd-1.0.1.tar.gz`

## Comparing `pymodd-1.0.0.tar` & `pymodd-1.0.1.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0      367 1970-01-01 00:00:00.000000 pymodd-1.0.0/Cargo.toml
--rw-r--r--   0      501       20     1513 2023-04-16 22:43:12.000000 pymodd-1.0.0/.github/workflows/CI.yml
--rw-r--r--   0      501       20     3103 2023-04-16 22:43:12.000000 pymodd-1.0.0/.gitignore
--rw-r--r--   0      501       20     1043 2023-04-16 22:43:12.000000 pymodd-1.0.0/LICENSE.txt
--rw-r--r--   0      501       20     2039 2023-05-21 23:49:14.000000 pymodd-1.0.0/README.rst
--rw-r--r--   0      501       20     1059 2023-05-21 00:56:47.000000 pymodd-1.0.0/examples/froge/entity_scripts.py
--rw-r--r--   0      501       20     2823 2023-05-21 02:01:59.000000 pymodd-1.0.0/examples/froge/game_variables.py
--rw-r--r--   0      501       20      559 2023-05-20 03:48:26.000000 pymodd-1.0.0/examples/froge/mapping.py
--rw-r--r--   0      501       20     5672 2023-05-21 00:56:47.000000 pymodd-1.0.0/examples/froge/scripts.py
--rw-r--r--   0      501       20    78239 2023-05-20 03:48:26.000000 pymodd-1.0.0/examples/froge/utils/game.json
--rw-r--r--   0      501       20        0 2023-04-16 22:43:12.000000 pymodd-1.0.0/pymodd/__init__.py
--rw-r--r--   0      501       20     1050 2023-05-21 00:56:56.000000 pymodd-1.0.0/pymodd/_pymodd_helper.pyi
--rw-r--r--   0      501       20    46037 2023-05-21 20:34:51.000000 pymodd-1.0.0/pymodd/actions.py
--rw-r--r--   0      501       20     3837 2023-05-21 21:43:25.000000 pymodd-1.0.0/pymodd/console_scripts/pymodd_command.py
--rw-r--r--   0      501       20     2563 2023-05-20 02:49:12.000000 pymodd-1.0.0/pymodd/entity_script.py
--rw-r--r--   0      501       20    51870 2023-05-21 00:56:47.000000 pymodd-1.0.0/pymodd/functions.py
--rw-r--r--   0      501       20     6188 2023-05-21 00:56:47.000000 pymodd-1.0.0/pymodd/game.py
--rw-r--r--   0      501       20       26 2023-04-16 22:43:12.000000 pymodd-1.0.0/pymodd/py.typed
--rw-r--r--   0      501       20    15438 2023-05-21 20:34:51.000000 pymodd-1.0.0/pymodd/script.py
--rw-r--r--   0      501       20   122364 2023-05-21 00:56:56.000000 pymodd-1.0.0/pymodd/utils/Default Game.json
--rw-r--r--   0      501       20    38332 2023-05-21 00:56:47.000000 pymodd-1.0.0/pymodd/variable_types.py
--rw-r--r--   0      501       20      801 2023-05-21 23:49:58.000000 pymodd-1.0.0/pyproject.toml
--rw-r--r--   0      501       20       41 2023-04-16 22:43:12.000000 pymodd-1.0.0/requirements.txt
--rw-r--r--   0      501       20     7772 2023-05-09 00:34:09.000000 pymodd-1.0.0/src/game_data/actions.rs
--rw-r--r--   0      501       20    20109 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/game_data/argument.rs
--rw-r--r--   0      501       20     9875 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/game_data/directory.rs
--rw-r--r--   0      501       20     5295 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/game_data/entity_types.rs
--rw-r--r--   0      501       20    10379 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/game_data/variable_categories.rs
--rw-r--r--   0      501       20     1799 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/game_data.rs
--rw-r--r--   0      501       20     1992 2023-05-21 00:56:56.000000 pymodd-1.0.0/src/lib.rs
--rw-r--r--   0      501       20    12703 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/project_generator/entity_scripts_file.rs
--rw-r--r--   0      501       20      183 2023-04-16 22:43:12.000000 pymodd-1.0.0/src/project_generator/game_json_file.rs
--rw-r--r--   0      501       20    12760 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/project_generator/game_variables_file.rs
--rw-r--r--   0      501       20     4350 2023-05-19 00:56:39.000000 pymodd-1.0.0/src/project_generator/mapping_file.rs
--rw-r--r--   0      501       20    44725 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/project_generator/scripts_file.rs
--rw-r--r--   0      501       20     9842 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/project_generator/utils/iterators/argument_values_iterator.rs
--rw-r--r--   0      501       20     1820 2023-04-16 22:43:12.000000 pymodd-1.0.0/src/project_generator/utils/iterators/directory_iterator.rs
--rw-r--r--   0      501       20       62 2023-04-16 22:43:12.000000 pymodd-1.0.0/src/project_generator/utils/iterators.rs
--rw-r--r--   0      501       20    10069 2023-05-15 23:54:58.000000 pymodd-1.0.0/src/project_generator/utils/to_pymodd_maps.rs
--rw-r--r--   0      501       20     2518 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/project_generator/utils.rs
--rw-r--r--   0      501       20     2442 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/project_generator.rs
--rw-r--r--   0      501       20    12887 2023-04-16 22:43:12.000000 pymodd-1.0.0/Cargo.lock
--rw-r--r--   0        0        0     2625 1970-01-01 00:00:00.000000 pymodd-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      367 1970-01-01 00:00:00.000000 pymodd-1.0.1/Cargo.toml
+-rw-r--r--   0     1001      123     2156 2023-05-24 22:13:12.000000 pymodd-1.0.1/.github/workflows/publish.yml
+-rw-r--r--   0     1001      123      372 2023-05-24 22:13:12.000000 pymodd-1.0.1/.github/workflows/test.yml
+-rw-r--r--   0     1001      123     3103 2023-05-24 22:13:12.000000 pymodd-1.0.1/.gitignore
+-rw-r--r--   0     1001      123     1043 2023-05-24 22:13:12.000000 pymodd-1.0.1/LICENSE.txt
+-rw-r--r--   0     1001      123     2041 2023-05-24 22:13:12.000000 pymodd-1.0.1/README.rst
+-rw-r--r--   0     1001      123     1059 2023-05-24 22:13:12.000000 pymodd-1.0.1/examples/froge/entity_scripts.py
+-rw-r--r--   0     1001      123     2823 2023-05-24 22:13:12.000000 pymodd-1.0.1/examples/froge/game_variables.py
+-rw-r--r--   0     1001      123      559 2023-05-24 22:13:12.000000 pymodd-1.0.1/examples/froge/mapping.py
+-rw-r--r--   0     1001      123     5672 2023-05-24 22:13:12.000000 pymodd-1.0.1/examples/froge/scripts.py
+-rw-r--r--   0     1001      123    78239 2023-05-24 22:13:12.000000 pymodd-1.0.1/examples/froge/utils/game.json
+-rw-r--r--   0     1001      123        0 2023-05-24 22:13:12.000000 pymodd-1.0.1/pymodd/__init__.py
+-rw-r--r--   0     1001      123     1050 2023-05-24 22:13:12.000000 pymodd-1.0.1/pymodd/_pymodd_helper.pyi
+-rw-r--r--   0     1001      123    46037 2023-05-24 22:13:12.000000 pymodd-1.0.1/pymodd/actions.py
+-rw-r--r--   0     1001      123     3998 2023-05-24 22:13:12.000000 pymodd-1.0.1/pymodd/console_scripts/pymodd_command.py
+-rw-r--r--   0     1001      123     2563 2023-05-24 22:13:12.000000 pymodd-1.0.1/pymodd/entity_script.py
+-rw-r--r--   0     1001      123    51870 2023-05-24 22:13:12.000000 pymodd-1.0.1/pymodd/functions.py
+-rw-r--r--   0     1001      123     6188 2023-05-24 22:13:12.000000 pymodd-1.0.1/pymodd/game.py
+-rw-r--r--   0     1001      123       26 2023-05-24 22:13:12.000000 pymodd-1.0.1/pymodd/py.typed
+-rw-r--r--   0     1001      123    15438 2023-05-24 22:13:12.000000 pymodd-1.0.1/pymodd/script.py
+-rw-r--r--   0     1001      123   122364 2023-05-24 22:13:12.000000 pymodd-1.0.1/pymodd/utils/Default Game.json
+-rw-r--r--   0     1001      123    38332 2023-05-24 22:13:12.000000 pymodd-1.0.1/pymodd/variable_types.py
+-rw-r--r--   0     1001      123      790 2023-05-24 22:13:12.000000 pymodd-1.0.1/pyproject.toml
+-rw-r--r--   0     1001      123       41 2023-05-24 22:13:12.000000 pymodd-1.0.1/requirements.txt
+-rw-r--r--   0     1001      123     7772 2023-05-24 22:13:12.000000 pymodd-1.0.1/src/game_data/actions.rs
+-rw-r--r--   0     1001      123    20109 2023-05-24 22:13:12.000000 pymodd-1.0.1/src/game_data/argument.rs
+-rw-r--r--   0     1001      123     9875 2023-05-24 22:13:12.000000 pymodd-1.0.1/src/game_data/directory.rs
+-rw-r--r--   0     1001      123     5295 2023-05-24 22:13:12.000000 pymodd-1.0.1/src/game_data/entity_types.rs
+-rw-r--r--   0     1001      123    10379 2023-05-24 22:13:12.000000 pymodd-1.0.1/src/game_data/variable_categories.rs
+-rw-r--r--   0     1001      123     1799 2023-05-24 22:13:12.000000 pymodd-1.0.1/src/game_data.rs
+-rw-r--r--   0     1001      123     1992 2023-05-24 22:13:12.000000 pymodd-1.0.1/src/lib.rs
+-rw-r--r--   0     1001      123    12703 2023-05-24 22:13:12.000000 pymodd-1.0.1/src/project_generator/entity_scripts_file.rs
+-rw-r--r--   0     1001      123      183 2023-05-24 22:13:12.000000 pymodd-1.0.1/src/project_generator/game_json_file.rs
+-rw-r--r--   0     1001      123    12760 2023-05-24 22:13:12.000000 pymodd-1.0.1/src/project_generator/game_variables_file.rs
+-rw-r--r--   0     1001      123     4350 2023-05-24 22:13:12.000000 pymodd-1.0.1/src/project_generator/mapping_file.rs
+-rw-r--r--   0     1001      123    44725 2023-05-24 22:13:12.000000 pymodd-1.0.1/src/project_generator/scripts_file.rs
+-rw-r--r--   0     1001      123     9842 2023-05-24 22:13:12.000000 pymodd-1.0.1/src/project_generator/utils/iterators/argument_values_iterator.rs
+-rw-r--r--   0     1001      123     1820 2023-05-24 22:13:12.000000 pymodd-1.0.1/src/project_generator/utils/iterators/directory_iterator.rs
+-rw-r--r--   0     1001      123       62 2023-05-24 22:13:12.000000 pymodd-1.0.1/src/project_generator/utils/iterators.rs
+-rw-r--r--   0     1001      123    10069 2023-05-24 22:13:12.000000 pymodd-1.0.1/src/project_generator/utils/to_pymodd_maps.rs
+-rw-r--r--   0     1001      123     2518 2023-05-24 22:13:12.000000 pymodd-1.0.1/src/project_generator/utils.rs
+-rw-r--r--   0     1001      123     2442 2023-05-24 22:13:12.000000 pymodd-1.0.1/src/project_generator.rs
+-rw-r--r--   0     1001      123    12887 2023-05-24 22:14:46.000000 pymodd-1.0.1/Cargo.lock
+-rw-r--r--   0        0        0     2616 1970-01-01 00:00:00.000000 pymodd-1.0.1/PKG-INFO
```

### Comparing `pymodd-1.0.0/.gitignore` & `pymodd-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/LICENSE.txt` & `pymodd-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/README.rst` & `pymodd-1.0.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 pymodd
 ======
 
 |Build| |Version| |License|
 
 pymodd is a python package for creating and editing modd.io games in python
 
-.. |Build| image:: https://img.shields.io/github/actions/workflow/status/jeff5343/pymodd/CI.yml?label=CI&logo=github&style=plastic
+.. |Build| image:: https://img.shields.io/github/actions/workflow/status/jeff5343/pymodd/test.yml?label=CI&logo=github&style=plastic
    :alt: GitHub Workflow Status
 .. |Version| image:: https://img.shields.io/pypi/v/pymodd?style=plastic
    :alt: PyPI
 .. |License| image:: https://img.shields.io/pypi/l/pymodd?style=plastic
    :alt: PyPI - License
 
 Features
```

### Comparing `pymodd-1.0.0/examples/froge/entity_scripts.py` & `pymodd-1.0.1/examples/froge/entity_scripts.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/examples/froge/game_variables.py` & `pymodd-1.0.1/examples/froge/game_variables.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/examples/froge/mapping.py` & `pymodd-1.0.1/examples/froge/mapping.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/examples/froge/scripts.py` & `pymodd-1.0.1/examples/froge/scripts.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/examples/froge/utils/game.json` & `pymodd-1.0.1/examples/froge/utils/game.json`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/pymodd/_pymodd_helper.pyi` & `pymodd-1.0.1/pymodd/_pymodd_helper.pyi`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/pymodd/actions.py` & `pymodd-1.0.1/pymodd/actions.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/pymodd/console_scripts/pymodd_command.py` & `pymodd-1.0.1/pymodd/console_scripts/pymodd_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import sys
 import json
 import runpy
 from pathlib import Path
 from argparse import ArgumentParser
 
 from pymodd import _pymodd_helper
@@ -87,21 +86,25 @@
     return list(dict(filter(
         is_class_data_of_variable_type,
         project_data.items())).values())
 
 
 def main_cli():
     parser = ArgumentParser(prog='pymodd')
+    parser.set_defaults(func=lambda _: parser.print_help())
     subparsers = parser.add_subparsers(
-        title='subcommands', description='valid subcommands')
+        title='subcommands', description='generate-project, compile', metavar='')
 
     parser_generate_project = subparsers.add_parser(
-        'generate-project', description='Parse a modd.io json file into a pymodd project')
+        'generate-project', description='Generate a pymodd project from a modd.io json file')
     parser_generate_project.add_argument(
-        'json_file_path', type=str, help='the path of the modd.io json file')
+        'json_file_path',
+        type=str,
+        help='the path of the modd.io json file. to generate a default project, fill in `default-template` instead'
+    )
     parser_generate_project.set_defaults(func=generate_project)
 
     parser_build = subparsers.add_parser(
         'compile', description='Compile a pymodd project into a modd.io json file')
     parser_build.set_defaults(func=compile_project)
 
     args = parser.parse_args()
```

### Comparing `pymodd-1.0.0/pymodd/entity_script.py` & `pymodd-1.0.1/pymodd/entity_script.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/pymodd/functions.py` & `pymodd-1.0.1/pymodd/functions.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/pymodd/game.py` & `pymodd-1.0.1/pymodd/game.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/pymodd/script.py` & `pymodd-1.0.1/pymodd/script.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/pymodd/utils/Default Game.json` & `pymodd-1.0.1/pymodd/utils/Default Game.json`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/pymodd/variable_types.py` & `pymodd-1.0.1/pymodd/variable_types.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/pyproject.toml` & `pymodd-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "pymodd"
-version = "1.0.0"
-description = "A package for creating modd.io games using python!"
+version = "1.0.1"
+description = "create and edit modd.io games in python"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
     {name = "Jeff"}
 ]
 classifiers = [
```

### Comparing `pymodd-1.0.0/src/game_data/actions.rs` & `pymodd-1.0.1/src/game_data/actions.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/src/game_data/argument.rs` & `pymodd-1.0.1/src/game_data/argument.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/src/game_data/directory.rs` & `pymodd-1.0.1/src/game_data/directory.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/src/game_data/entity_types.rs` & `pymodd-1.0.1/src/game_data/entity_types.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/src/game_data/variable_categories.rs` & `pymodd-1.0.1/src/game_data/variable_categories.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/src/game_data.rs` & `pymodd-1.0.1/src/game_data.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/src/lib.rs` & `pymodd-1.0.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/src/project_generator/entity_scripts_file.rs` & `pymodd-1.0.1/src/project_generator/entity_scripts_file.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/src/project_generator/game_variables_file.rs` & `pymodd-1.0.1/src/project_generator/game_variables_file.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/src/project_generator/mapping_file.rs` & `pymodd-1.0.1/src/project_generator/mapping_file.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/src/project_generator/scripts_file.rs` & `pymodd-1.0.1/src/project_generator/scripts_file.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/src/project_generator/utils/iterators/argument_values_iterator.rs` & `pymodd-1.0.1/src/project_generator/utils/iterators/argument_values_iterator.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/src/project_generator/utils/iterators/directory_iterator.rs` & `pymodd-1.0.1/src/project_generator/utils/iterators/directory_iterator.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/src/project_generator/utils/to_pymodd_maps.rs` & `pymodd-1.0.1/src/project_generator/utils/to_pymodd_maps.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/src/project_generator/utils.rs` & `pymodd-1.0.1/src/project_generator/utils.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/src/project_generator.rs` & `pymodd-1.0.1/src/project_generator.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/Cargo.lock` & `pymodd-1.0.1/Cargo.lock`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.0/PKG-INFO` & `pymodd-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pymodd
-Version: 1.0.0
+Version: 1.0.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: case-converter==1.1.0
 License-File: LICENSE.txt
-Summary: A package for creating modd.io games using python!
+Summary: create and edit modd.io games in python
 Author: Jeff
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 Project-URL: changelog, https://github.com/jeff5343/pymodd/releases
 Project-URL: repository, https://github.com/jeff5343/pymodd
 
@@ -18,15 +18,15 @@
 pymodd
 ======
 
 |Build| |Version| |License|
 
 pymodd is a python package for creating and editing modd.io games in python
 
-.. |Build| image:: https://img.shields.io/github/actions/workflow/status/jeff5343/pymodd/CI.yml?label=CI&logo=github&style=plastic
+.. |Build| image:: https://img.shields.io/github/actions/workflow/status/jeff5343/pymodd/test.yml?label=CI&logo=github&style=plastic
    :alt: GitHub Workflow Status
 .. |Version| image:: https://img.shields.io/pypi/v/pymodd?style=plastic
    :alt: PyPI
 .. |License| image:: https://img.shields.io/pypi/l/pymodd?style=plastic
    :alt: PyPI - License
 
 Features
```

