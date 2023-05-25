# Comparing `tmp/pymodd-1.0.2.tar.gz` & `tmp/pymodd-1.0.3.tar.gz`

## Comparing `pymodd-1.0.2.tar` & `pymodd-1.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      367 1970-01-01 00:00:00.000000 pymodd-1.0.2/Cargo.toml
--rw-r--r--   0     1001      123     2156 2023-05-25 20:48:29.000000 pymodd-1.0.2/.github/workflows/publish.yml
--rw-r--r--   0     1001      123      372 2023-05-25 20:48:29.000000 pymodd-1.0.2/.github/workflows/test.yml
--rw-r--r--   0     1001      123     3103 2023-05-25 20:48:29.000000 pymodd-1.0.2/.gitignore
--rw-r--r--   0     1001      123     1043 2023-05-25 20:48:29.000000 pymodd-1.0.2/LICENSE.txt
--rw-r--r--   0     1001      123     2041 2023-05-25 20:48:29.000000 pymodd-1.0.2/README.rst
--rw-r--r--   0     1001      123     1059 2023-05-25 20:48:29.000000 pymodd-1.0.2/examples/froge/entity_scripts.py
--rw-r--r--   0     1001      123     2823 2023-05-25 20:48:29.000000 pymodd-1.0.2/examples/froge/game_variables.py
--rw-r--r--   0     1001      123      559 2023-05-25 20:48:29.000000 pymodd-1.0.2/examples/froge/mapping.py
--rw-r--r--   0     1001      123     5672 2023-05-25 20:48:29.000000 pymodd-1.0.2/examples/froge/scripts.py
--rw-r--r--   0     1001      123    78239 2023-05-25 20:48:29.000000 pymodd-1.0.2/examples/froge/utils/game.json
--rw-r--r--   0     1001      123        0 2023-05-25 20:48:29.000000 pymodd-1.0.2/pymodd/__init__.py
--rw-r--r--   0     1001      123     1050 2023-05-25 20:48:29.000000 pymodd-1.0.2/pymodd/_pymodd_helper.pyi
--rw-r--r--   0     1001      123    46037 2023-05-25 20:48:29.000000 pymodd-1.0.2/pymodd/actions.py
--rw-r--r--   0     1001      123     3998 2023-05-25 20:48:29.000000 pymodd-1.0.2/pymodd/console_scripts/pymodd_command.py
--rw-r--r--   0     1001      123     2563 2023-05-25 20:48:29.000000 pymodd-1.0.2/pymodd/entity_script.py
--rw-r--r--   0     1001      123    51870 2023-05-25 20:48:29.000000 pymodd-1.0.2/pymodd/functions.py
--rw-r--r--   0     1001      123     6188 2023-05-25 20:48:29.000000 pymodd-1.0.2/pymodd/game.py
--rw-r--r--   0     1001      123       26 2023-05-25 20:48:29.000000 pymodd-1.0.2/pymodd/py.typed
--rw-r--r--   0     1001      123    15438 2023-05-25 20:48:29.000000 pymodd-1.0.2/pymodd/script.py
--rw-r--r--   0     1001      123   122364 2023-05-25 20:48:29.000000 pymodd-1.0.2/pymodd/utils/Default Game.json
--rw-r--r--   0     1001      123    38332 2023-05-25 20:48:29.000000 pymodd-1.0.2/pymodd/variable_types.py
--rw-r--r--   0     1001      123      790 2023-05-25 20:48:29.000000 pymodd-1.0.2/pyproject.toml
--rw-r--r--   0     1001      123       41 2023-05-25 20:48:29.000000 pymodd-1.0.2/requirements.txt
--rw-r--r--   0     1001      123     7772 2023-05-25 20:48:29.000000 pymodd-1.0.2/src/game_data/actions.rs
--rw-r--r--   0     1001      123    20109 2023-05-25 20:48:29.000000 pymodd-1.0.2/src/game_data/argument.rs
--rw-r--r--   0     1001      123     9875 2023-05-25 20:48:29.000000 pymodd-1.0.2/src/game_data/directory.rs
--rw-r--r--   0     1001      123     5295 2023-05-25 20:48:29.000000 pymodd-1.0.2/src/game_data/entity_types.rs
--rw-r--r--   0     1001      123    10379 2023-05-25 20:48:29.000000 pymodd-1.0.2/src/game_data/variable_categories.rs
--rw-r--r--   0     1001      123     1799 2023-05-25 20:48:29.000000 pymodd-1.0.2/src/game_data.rs
--rw-r--r--   0     1001      123     1992 2023-05-25 20:48:29.000000 pymodd-1.0.2/src/lib.rs
--rw-r--r--   0     1001      123    12703 2023-05-25 20:48:29.000000 pymodd-1.0.2/src/project_generator/entity_scripts_file.rs
--rw-r--r--   0     1001      123      183 2023-05-25 20:48:29.000000 pymodd-1.0.2/src/project_generator/game_json_file.rs
--rw-r--r--   0     1001      123    12760 2023-05-25 20:48:29.000000 pymodd-1.0.2/src/project_generator/game_variables_file.rs
--rw-r--r--   0     1001      123     4350 2023-05-25 20:48:29.000000 pymodd-1.0.2/src/project_generator/mapping_file.rs
--rw-r--r--   0     1001      123    44725 2023-05-25 20:48:29.000000 pymodd-1.0.2/src/project_generator/scripts_file.rs
--rw-r--r--   0     1001      123     9842 2023-05-25 20:48:29.000000 pymodd-1.0.2/src/project_generator/utils/iterators/argument_values_iterator.rs
--rw-r--r--   0     1001      123     1820 2023-05-25 20:48:29.000000 pymodd-1.0.2/src/project_generator/utils/iterators/directory_iterator.rs
--rw-r--r--   0     1001      123       62 2023-05-25 20:48:29.000000 pymodd-1.0.2/src/project_generator/utils/iterators.rs
--rw-r--r--   0     1001      123    10154 2023-05-25 20:48:29.000000 pymodd-1.0.2/src/project_generator/utils/to_pymodd_maps.rs
--rw-r--r--   0     1001      123     2518 2023-05-25 20:48:29.000000 pymodd-1.0.2/src/project_generator/utils.rs
--rw-r--r--   0     1001      123     2442 2023-05-25 20:48:29.000000 pymodd-1.0.2/src/project_generator.rs
--rw-r--r--   0     1001      123    12887 2023-05-25 20:48:29.000000 pymodd-1.0.2/Cargo.lock
--rw-r--r--   0        0        0     2616 1970-01-01 00:00:00.000000 pymodd-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      367 1970-01-01 00:00:00.000000 pymodd-1.0.3/Cargo.toml
+-rw-r--r--   0     1001      123     2156 2023-05-25 21:01:48.000000 pymodd-1.0.3/.github/workflows/publish.yml
+-rw-r--r--   0     1001      123      372 2023-05-25 21:01:48.000000 pymodd-1.0.3/.github/workflows/test.yml
+-rw-r--r--   0     1001      123     3103 2023-05-25 21:01:48.000000 pymodd-1.0.3/.gitignore
+-rw-r--r--   0     1001      123     1043 2023-05-25 21:01:48.000000 pymodd-1.0.3/LICENSE.txt
+-rw-r--r--   0     1001      123     2041 2023-05-25 21:01:48.000000 pymodd-1.0.3/README.rst
+-rw-r--r--   0     1001      123     1059 2023-05-25 21:01:48.000000 pymodd-1.0.3/examples/froge/entity_scripts.py
+-rw-r--r--   0     1001      123     2823 2023-05-25 21:01:48.000000 pymodd-1.0.3/examples/froge/game_variables.py
+-rw-r--r--   0     1001      123      559 2023-05-25 21:01:48.000000 pymodd-1.0.3/examples/froge/mapping.py
+-rw-r--r--   0     1001      123     5672 2023-05-25 21:01:48.000000 pymodd-1.0.3/examples/froge/scripts.py
+-rw-r--r--   0     1001      123    78239 2023-05-25 21:01:48.000000 pymodd-1.0.3/examples/froge/utils/game.json
+-rw-r--r--   0     1001      123        0 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/__init__.py
+-rw-r--r--   0     1001      123     1050 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/_pymodd_helper.pyi
+-rw-r--r--   0     1001      123    46037 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/actions.py
+-rw-r--r--   0     1001      123     3998 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/console_scripts/pymodd_command.py
+-rw-r--r--   0     1001      123     2563 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/entity_script.py
+-rw-r--r--   0     1001      123    51870 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/functions.py
+-rw-r--r--   0     1001      123     6188 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/game.py
+-rw-r--r--   0     1001      123       26 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/py.typed
+-rw-r--r--   0     1001      123    15438 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/script.py
+-rw-r--r--   0     1001      123   122364 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/utils/Default Game.json
+-rw-r--r--   0     1001      123    38332 2023-05-25 21:01:48.000000 pymodd-1.0.3/pymodd/variable_types.py
+-rw-r--r--   0     1001      123      790 2023-05-25 21:01:48.000000 pymodd-1.0.3/pyproject.toml
+-rw-r--r--   0     1001      123       41 2023-05-25 21:01:48.000000 pymodd-1.0.3/requirements.txt
+-rw-r--r--   0     1001      123     7772 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/game_data/actions.rs
+-rw-r--r--   0     1001      123    20109 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/game_data/argument.rs
+-rw-r--r--   0     1001      123     9875 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/game_data/directory.rs
+-rw-r--r--   0     1001      123     5295 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/game_data/entity_types.rs
+-rw-r--r--   0     1001      123    10379 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/game_data/variable_categories.rs
+-rw-r--r--   0     1001      123     1799 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/game_data.rs
+-rw-r--r--   0     1001      123     1992 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/lib.rs
+-rw-r--r--   0     1001      123    12703 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/entity_scripts_file.rs
+-rw-r--r--   0     1001      123      183 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/game_json_file.rs
+-rw-r--r--   0     1001      123    12760 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/game_variables_file.rs
+-rw-r--r--   0     1001      123     4350 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/mapping_file.rs
+-rw-r--r--   0     1001      123    44725 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/scripts_file.rs
+-rw-r--r--   0     1001      123     9842 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/utils/iterators/argument_values_iterator.rs
+-rw-r--r--   0     1001      123     1820 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/utils/iterators/directory_iterator.rs
+-rw-r--r--   0     1001      123       62 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/utils/iterators.rs
+-rw-r--r--   0     1001      123    10239 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/utils/to_pymodd_maps.rs
+-rw-r--r--   0     1001      123     2518 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator/utils.rs
+-rw-r--r--   0     1001      123     2442 2023-05-25 21:01:48.000000 pymodd-1.0.3/src/project_generator.rs
+-rw-r--r--   0     1001      123    12887 2023-05-25 21:01:48.000000 pymodd-1.0.3/Cargo.lock
+-rw-r--r--   0        0        0     2616 1970-01-01 00:00:00.000000 pymodd-1.0.3/PKG-INFO
```

### Comparing `pymodd-1.0.2/.github/workflows/publish.yml` & `pymodd-1.0.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/.gitignore` & `pymodd-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/LICENSE.txt` & `pymodd-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/README.rst` & `pymodd-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/examples/froge/entity_scripts.py` & `pymodd-1.0.3/examples/froge/entity_scripts.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/examples/froge/game_variables.py` & `pymodd-1.0.3/examples/froge/game_variables.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/examples/froge/mapping.py` & `pymodd-1.0.3/examples/froge/mapping.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/examples/froge/scripts.py` & `pymodd-1.0.3/examples/froge/scripts.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/examples/froge/utils/game.json` & `pymodd-1.0.3/examples/froge/utils/game.json`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/pymodd/_pymodd_helper.pyi` & `pymodd-1.0.3/pymodd/_pymodd_helper.pyi`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/pymodd/actions.py` & `pymodd-1.0.3/pymodd/actions.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/pymodd/console_scripts/pymodd_command.py` & `pymodd-1.0.3/pymodd/console_scripts/pymodd_command.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/pymodd/entity_script.py` & `pymodd-1.0.3/pymodd/entity_script.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/pymodd/functions.py` & `pymodd-1.0.3/pymodd/functions.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/pymodd/game.py` & `pymodd-1.0.3/pymodd/game.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/pymodd/script.py` & `pymodd-1.0.3/pymodd/script.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/pymodd/utils/Default Game.json` & `pymodd-1.0.3/pymodd/utils/Default Game.json`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/pymodd/variable_types.py` & `pymodd-1.0.3/pymodd/variable_types.py`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/pyproject.toml` & `pymodd-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "pymodd"
-version = "1.0.2"
+version = "1.0.3"
 description = "create and edit modd.io games in python"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
     {name = "Jeff"}
 ]
```

### Comparing `pymodd-1.0.2/src/game_data/actions.rs` & `pymodd-1.0.3/src/game_data/actions.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/src/game_data/argument.rs` & `pymodd-1.0.3/src/game_data/argument.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/src/game_data/directory.rs` & `pymodd-1.0.3/src/game_data/directory.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/src/game_data/entity_types.rs` & `pymodd-1.0.3/src/game_data/entity_types.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/src/game_data/variable_categories.rs` & `pymodd-1.0.3/src/game_data/variable_categories.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/src/game_data.rs` & `pymodd-1.0.3/src/game_data.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/src/lib.rs` & `pymodd-1.0.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/src/project_generator/entity_scripts_file.rs` & `pymodd-1.0.3/src/project_generator/entity_scripts_file.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/src/project_generator/game_variables_file.rs` & `pymodd-1.0.3/src/project_generator/game_variables_file.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/src/project_generator/mapping_file.rs` & `pymodd-1.0.3/src/project_generator/mapping_file.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/src/project_generator/scripts_file.rs` & `pymodd-1.0.3/src/project_generator/scripts_file.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/src/project_generator/utils/iterators/argument_values_iterator.rs` & `pymodd-1.0.3/src/project_generator/utils/iterators/argument_values_iterator.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/src/project_generator/utils/iterators/directory_iterator.rs` & `pymodd-1.0.3/src/project_generator/utils/iterators/directory_iterator.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/src/project_generator/utils/to_pymodd_maps.rs` & `pymodd-1.0.3/src/project_generator/utils/to_pymodd_maps.rs`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,19 @@
     // Condition class is formatted differently from the other classes
     functions_to_structure.insert(
         String::from("condition"),
         PymoddStructure::new("Condition", vec!["item_a", "operator", "item_b"]),
     );
 
     let function_classes: Vec<&str> = PYMODD_FUNCTIONS_FILE_CONTENT
-        .split("\n\n\n")
+        .split(if cfg!(windows) {
+            "\r\n\r\n\r\n"
+        } else {
+            "\n\n\n"
+        })
         .skip(5)
         .collect();
     function_classes.into_iter().for_each(|class_content| {
         // skip over invalid classes
         if class_content.contains("self.options = ") {
             functions_to_structure.insert(
                 parse_function_type_of_pymodd_function_class(&class_content),
```

### Comparing `pymodd-1.0.2/src/project_generator/utils.rs` & `pymodd-1.0.3/src/project_generator/utils.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/src/project_generator.rs` & `pymodd-1.0.3/src/project_generator.rs`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/Cargo.lock` & `pymodd-1.0.3/Cargo.lock`

 * *Files identical despite different names*

### Comparing `pymodd-1.0.2/PKG-INFO` & `pymodd-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pymodd
-Version: 1.0.2
+Version: 1.0.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: case-converter==1.1.0
 License-File: LICENSE.txt
 Summary: create and edit modd.io games in python
 Author: Jeff
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
-Project-URL: changelog, https://github.com/jeff5343/pymodd/releases
 Project-URL: repository, https://github.com/jeff5343/pymodd
+Project-URL: changelog, https://github.com/jeff5343/pymodd/releases
 
 ======
 pymodd
 ======
 
 |Build| |Version| |License|
```

