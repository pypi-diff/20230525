# Comparing `tmp/retrack-0.5.0.tar.gz` & `tmp/retrack-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retrack-0.5.0.tar", max compression
+gzip compressed data, was "retrack-0.6.0.tar", max compression
```

## Comparing `retrack-0.5.0.tar` & `retrack-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,36 @@
--rw-r--r--   0        0        0     1072 2023-05-18 17:13:18.083398 retrack-0.5.0/LICENSE
--rw-r--r--   0        0        0     4914 2023-05-18 17:13:18.083398 retrack-0.5.0/README.md
--rw-r--r--   0        0        0     1580 2023-05-18 17:13:18.083398 retrack-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      366 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/engine/__init__.py
--rw-r--r--   0        0        0     6675 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/engine/parser.py
--rw-r--r--   0        0        0     2907 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/engine/request_manager.py
--rw-r--r--   0        0        0     6463 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/engine/runner.py
--rw-r--r--   0        0        0     1462 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/__init__.py
--rw-r--r--   0        0        0     1800 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/base.py
--rw-r--r--   0        0        0     2574 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/check.py
--rw-r--r--   0        0        0     2234 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/constants.py
--rw-r--r--   0        0        0      873 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/contains.py
--rw-r--r--   0        0        0      951 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/datetime.py
--rw-r--r--   0        0        0      910 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/endswith.py
--rw-r--r--   0        0        0      941 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/endswithany.py
--rw-r--r--   0        0        0     1009 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/inputs.py
--rw-r--r--   0        0        0     1606 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/logic.py
--rw-r--r--   0        0        0     1056 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/match.py
--rw-r--r--   0        0        0     2623 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/math.py
--rw-r--r--   0        0        0     1085 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/outputs.py
--rw-r--r--   0        0        0      581 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/start.py
--rw-r--r--   0        0        0      926 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/startswith.py
--rw-r--r--   0        0        0      957 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/startswithany.py
--rw-r--r--   0        0        0        0 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/utils/__init__.py
--rw-r--r--   0        0        0      197 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/utils/constants.py
--rw-r--r--   0        0        0     1324 2023-05-18 17:13:18.087399 retrack-0.5.0/retrack/utils/registry.py
--rw-r--r--   0        0        0      154 2023-05-18 17:13:18.087399 retrack-0.5.0/retrack/utils/transformers.py
--rw-r--r--   0        0        0      594 2023-05-18 17:13:18.087399 retrack-0.5.0/retrack/validators/__init__.py
--rw-r--r--   0        0        0      267 2023-05-18 17:13:18.087399 retrack-0.5.0/retrack/validators/base.py
--rw-r--r--   0        0        0      407 2023-05-18 17:13:18.087399 retrack-0.5.0/retrack/validators/check_is_dag.py
--rw-r--r--   0        0        0     1296 2023-05-18 17:13:18.087399 retrack-0.5.0/retrack/validators/node_exists.py
--rw-r--r--   0        0        0     5681 1970-01-01 00:00:00.000000 retrack-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-24 21:06:45.372337 retrack-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4914 2023-05-24 21:06:45.372337 retrack-0.6.0/README.md
+-rw-r--r--   0        0        0     1580 2023-05-24 21:06:45.372337 retrack-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      366 2023-05-24 21:06:45.372337 retrack-0.6.0/retrack/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 21:06:45.372337 retrack-0.6.0/retrack/engine/__init__.py
+-rw-r--r--   0        0        0     6986 2023-05-24 21:06:45.372337 retrack-0.6.0/retrack/engine/parser.py
+-rw-r--r--   0        0        0     2907 2023-05-24 21:06:45.372337 retrack-0.6.0/retrack/engine/request_manager.py
+-rw-r--r--   0        0        0     6463 2023-05-24 21:06:45.372337 retrack-0.6.0/retrack/engine/runner.py
+-rw-r--r--   0        0        0     1614 2023-05-24 21:06:45.372337 retrack-0.6.0/retrack/nodes/__init__.py
+-rw-r--r--   0        0        0     1800 2023-05-24 21:06:45.372337 retrack-0.6.0/retrack/nodes/base.py
+-rw-r--r--   0        0        0     2574 2023-05-24 21:06:45.372337 retrack-0.6.0/retrack/nodes/check.py
+-rw-r--r--   0        0        0     2234 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/nodes/constants.py
+-rw-r--r--   0        0        0      873 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/nodes/contains.py
+-rw-r--r--   0        0        0      951 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/nodes/datetime.py
+-rw-r--r--   0        0        0      543 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/nodes/dynamic/__init__.py
+-rw-r--r--   0        0        0      813 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/nodes/dynamic/base.py
+-rw-r--r--   0        0        0     2485 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/nodes/dynamic/csv_table.py
+-rw-r--r--   0        0        0      910 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/nodes/endswith.py
+-rw-r--r--   0        0        0      941 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/nodes/endswithany.py
+-rw-r--r--   0        0        0     1009 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/nodes/inputs.py
+-rw-r--r--   0        0        0     1606 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/nodes/logic.py
+-rw-r--r--   0        0        0     1056 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/nodes/match.py
+-rw-r--r--   0        0        0     2623 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/nodes/math.py
+-rw-r--r--   0        0        0     1085 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/nodes/outputs.py
+-rw-r--r--   0        0        0      581 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/nodes/start.py
+-rw-r--r--   0        0        0      926 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/nodes/startswith.py
+-rw-r--r--   0        0        0      957 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/nodes/startswithany.py
+-rw-r--r--   0        0        0        0 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/utils/__init__.py
+-rw-r--r--   0        0        0      197 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/utils/constants.py
+-rw-r--r--   0        0        0     1324 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/utils/registry.py
+-rw-r--r--   0        0        0      154 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/utils/transformers.py
+-rw-r--r--   0        0        0      594 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/validators/__init__.py
+-rw-r--r--   0        0        0      267 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/validators/base.py
+-rw-r--r--   0        0        0      407 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/validators/check_is_dag.py
+-rw-r--r--   0        0        0     1296 2023-05-24 21:06:45.376337 retrack-0.6.0/retrack/validators/node_exists.py
+-rw-r--r--   0        0        0     5681 1970-01-01 00:00:00.000000 retrack-0.6.0/PKG-INFO
```

### Comparing `retrack-0.5.0/LICENSE` & `retrack-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/README.md` & `retrack-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/pyproject.toml` & `retrack-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "retrack"
-version = "0.5.0"
+version = "0.6.0"
 description = "A business rules engine"
 authors = ["Gabriel Guarisa <gabrielguarisa@gmail.com>", "Nathalia Trotte <nathaliatrotte@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gabrielguarisa/retrack"
 homepage = "https://github.com/gabrielguarisa/retrack"
 keywords = ["rules", "models", "business", "node", "graph"]
```

### Comparing `retrack-0.5.0/retrack/engine/parser.py` & `retrack-0.6.0/retrack/engine/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 
 
 class Parser:
     def __init__(
         self,
         graph_data: dict,
         component_registry: Registry = nodes.registry(),
+        dynamic_registry: Registry = nodes.dynamic_registry(),
         validator_registry: Registry = validators.registry(),
     ):
         self._execution_order = None
         self.__components = {}
         self.__edges = None
 
         self._check_input_data(graph_data)
 
-        self._set_components(graph_data, component_registry)
+        self._set_components(graph_data, component_registry, dynamic_registry)
         self._set_edges()
 
         self._validate_graph(graph_data, validator_registry)
 
         self._set_indexes_by_name_map()
         self._set_indexes_by_kind_map()
         self._set_execution_order()
@@ -48,25 +49,32 @@
         if not isinstance(node_name, str):
             raise TypeError(f"BaseNode {node_id} name must be a string")
 
     @property
     def components(self) -> typing.Dict[str, nodes.BaseNode]:
         return self.__components
 
-    def _set_components(self, graph_data: dict, component_registry: Registry):
+    def _set_components(
+        self, graph_data: dict, component_registry: Registry, dynamic_registry: Registry
+    ):
         for node_id, node_metadata in graph_data["nodes"].items():
             if node_id in self.__components:
                 raise ValueError(f"Duplicate node id: {node_id}")
 
             node_name = node_metadata.get("name", None)
             self._check_node_name(node_name, node_id)
 
             node_name = node_name.lower()
 
-            validation_model = component_registry.get(node_name)
+            node_factory = dynamic_registry.get(node_name)
+
+            if node_factory is not None:
+                validation_model = node_factory(**node_metadata)
+            else:
+                validation_model = component_registry.get(node_name)
 
             if validation_model is None:
                 raise ValueError(f"Unknown node name: {node_name}")
 
             self.__components[node_id] = validation_model(**node_metadata)
 
     @property
```

### Comparing `retrack-0.5.0/retrack/engine/request_manager.py` & `retrack-0.6.0/retrack/engine/request_manager.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/retrack/engine/runner.py` & `retrack-0.6.0/retrack/engine/runner.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/retrack/nodes/base.py` & `retrack-0.6.0/retrack/nodes/base.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/retrack/nodes/check.py` & `retrack-0.6.0/retrack/nodes/check.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/retrack/nodes/constants.py` & `retrack-0.6.0/retrack/nodes/constants.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/retrack/nodes/contains.py` & `retrack-0.6.0/retrack/nodes/contains.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/retrack/nodes/datetime.py` & `retrack-0.6.0/retrack/nodes/datetime.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/retrack/nodes/endswith.py` & `retrack-0.6.0/retrack/nodes/endswith.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/retrack/nodes/endswithany.py` & `retrack-0.6.0/retrack/nodes/endswithany.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/retrack/nodes/inputs.py` & `retrack-0.6.0/retrack/nodes/inputs.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/retrack/nodes/logic.py` & `retrack-0.6.0/retrack/nodes/logic.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/retrack/nodes/match.py` & `retrack-0.6.0/retrack/nodes/match.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/retrack/nodes/math.py` & `retrack-0.6.0/retrack/nodes/math.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/retrack/nodes/outputs.py` & `retrack-0.6.0/retrack/nodes/outputs.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/retrack/nodes/start.py` & `retrack-0.6.0/retrack/nodes/start.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/retrack/nodes/startswith.py` & `retrack-0.6.0/retrack/nodes/startswith.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/retrack/nodes/startswithany.py` & `retrack-0.6.0/retrack/nodes/startswithany.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/retrack/utils/registry.py` & `retrack-0.6.0/retrack/utils/registry.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/retrack/validators/__init__.py` & `retrack-0.6.0/retrack/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/retrack/validators/node_exists.py` & `retrack-0.6.0/retrack/validators/node_exists.py`

 * *Files identical despite different names*

### Comparing `retrack-0.5.0/PKG-INFO` & `retrack-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retrack
-Version: 0.5.0
+Version: 0.6.0
 Summary: A business rules engine
 Home-page: https://github.com/gabrielguarisa/retrack
 License: MIT
 Keywords: rules,models,business,node,graph
 Author: Gabriel Guarisa
 Author-email: gabrielguarisa@gmail.com
 Requires-Python: >=3.8.16,<4.0.0
```

