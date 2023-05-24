# Comparing `tmp/retrack-0.7.0a1.tar.gz` & `tmp/retrack-0.7.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retrack-0.7.0a1.tar", max compression
+gzip compressed data, was "retrack-0.7.0a2.tar", max compression
```

## Comparing `retrack-0.7.0a1.tar` & `retrack-0.7.0a2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1072 2023-05-24 23:26:02.166525 retrack-0.7.0a1/LICENSE
--rw-r--r--   0        0        0     4914 2023-05-24 23:26:02.166525 retrack-0.7.0a1/README.md
--rw-r--r--   0        0        0     2119 2023-05-24 23:26:02.166525 retrack-0.7.0a1/pyproject.toml
--rw-r--r--   0        0        0      366 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/engine/__init__.py
--rw-r--r--   0        0        0     6986 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/engine/parser.py
--rw-r--r--   0        0        0     2907 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/engine/request_manager.py
--rw-r--r--   0        0        0     6463 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/engine/runner.py
--rw-r--r--   0        0        0     1614 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/nodes/__init__.py
--rw-r--r--   0        0        0     1800 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/nodes/base.py
--rw-r--r--   0        0        0     2574 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/nodes/check.py
--rw-r--r--   0        0        0     2234 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/nodes/constants.py
--rw-r--r--   0        0        0      873 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/nodes/contains.py
--rw-r--r--   0        0        0      951 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/nodes/datetime.py
--rw-r--r--   0        0        0      543 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/nodes/dynamic/__init__.py
--rw-r--r--   0        0        0      813 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/nodes/dynamic/base.py
--rw-r--r--   0        0        0     2485 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/nodes/dynamic/csv_table.py
--rw-r--r--   0        0        0      910 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/nodes/endswith.py
--rw-r--r--   0        0        0      941 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/nodes/endswithany.py
--rw-r--r--   0        0        0     1009 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/nodes/inputs.py
--rw-r--r--   0        0        0     1606 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/nodes/logic.py
--rw-r--r--   0        0        0     1056 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/nodes/match.py
--rw-r--r--   0        0        0     2623 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/nodes/math.py
--rw-r--r--   0        0        0     1085 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/nodes/outputs.py
--rw-r--r--   0        0        0      581 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/nodes/start.py
--rw-r--r--   0        0        0      926 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/nodes/startswith.py
--rw-r--r--   0        0        0      957 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/nodes/startswithany.py
--rw-r--r--   0        0        0        0 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/utils/__init__.py
--rw-r--r--   0        0        0      197 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/utils/constants.py
--rw-r--r--   0        0        0     1324 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/utils/registry.py
--rw-r--r--   0        0        0      154 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/utils/transformers.py
--rw-r--r--   0        0        0      594 2023-05-24 23:26:02.166525 retrack-0.7.0a1/retrack/validators/__init__.py
--rw-r--r--   0        0        0      267 2023-05-24 23:26:02.170524 retrack-0.7.0a1/retrack/validators/base.py
--rw-r--r--   0        0        0      407 2023-05-24 23:26:02.170524 retrack-0.7.0a1/retrack/validators/check_is_dag.py
--rw-r--r--   0        0        0     1296 2023-05-24 23:26:02.170524 retrack-0.7.0a1/retrack/validators/node_exists.py
--rw-r--r--   0        0        0     6023 1970-01-01 00:00:00.000000 retrack-0.7.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-24 23:33:59.228805 retrack-0.7.0a2/LICENSE
+-rw-r--r--   0        0        0     4914 2023-05-24 23:33:59.228805 retrack-0.7.0a2/README.md
+-rw-r--r--   0        0        0     2119 2023-05-24 23:33:59.228805 retrack-0.7.0a2/pyproject.toml
+-rw-r--r--   0        0        0      366 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/engine/__init__.py
+-rw-r--r--   0        0        0     6986 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/engine/parser.py
+-rw-r--r--   0        0        0     2907 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/engine/request_manager.py
+-rw-r--r--   0        0        0     6463 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/engine/runner.py
+-rw-r--r--   0        0        0     1614 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/nodes/__init__.py
+-rw-r--r--   0        0        0     1800 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/nodes/base.py
+-rw-r--r--   0        0        0     2574 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/nodes/check.py
+-rw-r--r--   0        0        0     2234 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/nodes/constants.py
+-rw-r--r--   0        0        0      873 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/nodes/contains.py
+-rw-r--r--   0        0        0      951 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/nodes/datetime.py
+-rw-r--r--   0        0        0      543 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/nodes/dynamic/__init__.py
+-rw-r--r--   0        0        0      813 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/nodes/dynamic/base.py
+-rw-r--r--   0        0        0     2485 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/nodes/dynamic/csv_table.py
+-rw-r--r--   0        0        0      910 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/nodes/endswith.py
+-rw-r--r--   0        0        0      941 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/nodes/endswithany.py
+-rw-r--r--   0        0        0     1009 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/nodes/inputs.py
+-rw-r--r--   0        0        0     1606 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/nodes/logic.py
+-rw-r--r--   0        0        0     1056 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/nodes/match.py
+-rw-r--r--   0        0        0     2623 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/nodes/math.py
+-rw-r--r--   0        0        0     1085 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/nodes/outputs.py
+-rw-r--r--   0        0        0      581 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/nodes/start.py
+-rw-r--r--   0        0        0      926 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/nodes/startswith.py
+-rw-r--r--   0        0        0      957 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/nodes/startswithany.py
+-rw-r--r--   0        0        0        0 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/utils/__init__.py
+-rw-r--r--   0        0        0      197 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/utils/constants.py
+-rw-r--r--   0        0        0     1324 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/utils/registry.py
+-rw-r--r--   0        0        0      154 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/utils/transformers.py
+-rw-r--r--   0        0        0      594 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/validators/__init__.py
+-rw-r--r--   0        0        0      267 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/validators/base.py
+-rw-r--r--   0        0        0      407 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/validators/check_is_dag.py
+-rw-r--r--   0        0        0     1296 2023-05-24 23:33:59.228805 retrack-0.7.0a2/retrack/validators/node_exists.py
+-rw-r--r--   0        0        0     6023 1970-01-01 00:00:00.000000 retrack-0.7.0a2/PKG-INFO
```

### Comparing `retrack-0.7.0a1/LICENSE` & `retrack-0.7.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/README.md` & `retrack-0.7.0a2/README.md`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/pyproject.toml` & `retrack-0.7.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "retrack"
-version = "0.7.0a1"
+version = "0.7.0a2"
 description = "A business rules engine"
 authors = ["Gabriel Guarisa <gabrielguarisa@gmail.com>", "Nathalia Trotte <nathaliatrotte@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gabrielguarisa/retrack"
 homepage = "https://github.com/gabrielguarisa/retrack"
 keywords = ["rules", "models", "business", "node", "graph"]
```

### Comparing `retrack-0.7.0a1/retrack/engine/parser.py` & `retrack-0.7.0a2/retrack/engine/parser.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/engine/request_manager.py` & `retrack-0.7.0a2/retrack/engine/request_manager.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/engine/runner.py` & `retrack-0.7.0a2/retrack/engine/runner.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/nodes/__init__.py` & `retrack-0.7.0a2/retrack/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/nodes/base.py` & `retrack-0.7.0a2/retrack/nodes/base.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/nodes/check.py` & `retrack-0.7.0a2/retrack/nodes/check.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/nodes/constants.py` & `retrack-0.7.0a2/retrack/nodes/constants.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/nodes/contains.py` & `retrack-0.7.0a2/retrack/nodes/contains.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/nodes/datetime.py` & `retrack-0.7.0a2/retrack/nodes/datetime.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/nodes/dynamic/__init__.py` & `retrack-0.7.0a2/retrack/nodes/dynamic/__init__.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/nodes/dynamic/base.py` & `retrack-0.7.0a2/retrack/nodes/dynamic/base.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/nodes/dynamic/csv_table.py` & `retrack-0.7.0a2/retrack/nodes/dynamic/csv_table.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/nodes/endswith.py` & `retrack-0.7.0a2/retrack/nodes/endswith.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/nodes/endswithany.py` & `retrack-0.7.0a2/retrack/nodes/endswithany.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/nodes/inputs.py` & `retrack-0.7.0a2/retrack/nodes/inputs.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/nodes/logic.py` & `retrack-0.7.0a2/retrack/nodes/logic.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/nodes/match.py` & `retrack-0.7.0a2/retrack/nodes/match.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/nodes/math.py` & `retrack-0.7.0a2/retrack/nodes/math.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/nodes/outputs.py` & `retrack-0.7.0a2/retrack/nodes/outputs.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/nodes/start.py` & `retrack-0.7.0a2/retrack/nodes/start.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/nodes/startswith.py` & `retrack-0.7.0a2/retrack/nodes/startswith.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/nodes/startswithany.py` & `retrack-0.7.0a2/retrack/nodes/startswithany.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/utils/registry.py` & `retrack-0.7.0a2/retrack/utils/registry.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/validators/__init__.py` & `retrack-0.7.0a2/retrack/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/retrack/validators/node_exists.py` & `retrack-0.7.0a2/retrack/validators/node_exists.py`

 * *Files identical despite different names*

### Comparing `retrack-0.7.0a1/PKG-INFO` & `retrack-0.7.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retrack
-Version: 0.7.0a1
+Version: 0.7.0a2
 Summary: A business rules engine
 Home-page: https://github.com/gabrielguarisa/retrack
 License: MIT
 Keywords: rules,models,business,node,graph
 Author: Gabriel Guarisa
 Author-email: gabrielguarisa@gmail.com
 Requires-Python: >=3.7.16,<4.0.0
```

