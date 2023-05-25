# Comparing `tmp/bmsdna_lakeapi-0.4.6.tar.gz` & `tmp/bmsdna_lakeapi-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.4.6.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.4.7.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.4.6.tar` & `bmsdna_lakeapi-0.4.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1081 2023-05-25 12:11:08.143754 bmsdna_lakeapi-0.4.6/LICENSE
--rw-r--r--   0        0        0     8431 2023-05-25 12:11:08.143754 bmsdna_lakeapi-0.4.6/README.md
--rw-r--r--   0        0        0      271 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1074 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      926 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     5989 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0     4072 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/context/df_datafusion.py
--rw-r--r--   0        0        0     8573 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6390 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    11432 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    11558 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    19486 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6836 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     7822 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4450 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3141 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2367 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      326 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1790 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     1842 2023-05-25 12:11:08.155754 bmsdna_lakeapi-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     9725 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-25 15:16:53.787064 bmsdna_lakeapi-0.4.7/LICENSE
+-rw-r--r--   0        0        0     8431 2023-05-25 15:16:53.787064 bmsdna_lakeapi-0.4.7/README.md
+-rw-r--r--   0        0        0      271 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1074 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      926 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     5989 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0     4072 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/context/df_datafusion.py
+-rw-r--r--   0        0        0     8573 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6390 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    11432 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    11558 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    19758 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-05-25 15:16:53.795065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6836 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     7822 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4497 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3151 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2367 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      326 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1790 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     1842 2023-05-25 15:16:53.799065 bmsdna_lakeapi-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     9725 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.4.7/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.4.6/LICENSE` & `bmsdna_lakeapi-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.6/README.md` & `bmsdna_lakeapi-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/context/df_base.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/context/df_datafusion.py` & `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/context/df_datafusion.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/config.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,29 +113,36 @@
         "description": tblmeta.description,
         "partition_columns": tblmeta.partition_columns,
         "configuration": tblmeta.configuration,
     }
 
 
 def create_detailed_meta_endpoint(
-    metamodel: Optional[ResultData], config: Config, router: APIRouter, basic_config: BasicConfig
+    metamodel: Optional[ResultData], config: Config, configs: Configs, router: APIRouter, basic_config: BasicConfig
 ):
     route = config.route + "/metadata_detail"
     has_complex = True
     if metamodel is not None:
         has_complex = any((pa.types.is_nested(t) for t in metamodel.arrow_schema().types))
 
+    async def get_username(req: Request):
+        res = basic_config.username_retriever(req, basic_config, configs.users)
+        if inspect.isawaitable(res):
+            res = await res
+        return res
+
     @router.get(
         route,
         tags=["metadata", "metadata:" + config.tag],
         operation_id=config.tag + "_" + config.name,
         name=config.name + "_metadata",
     )
     def get_detailed_metadata(
         req: Request,
+        username=Depends(get_username),
         jsonify_complex: bool = Query(title="jsonify_complex", include_in_schema=has_complex, default=False),
     ) -> MetadataDetailResult:
         import json
 
         req.state.lake_api_basic_config = basic_config
         from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContext
```

### Comparing `bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/route.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,17 @@
                 )
 
             except Exception as err:
                 logger.warning(f"Could not get response type for f{config.route}. Error:{err}")
                 metamodel = None
 
             response_model = get_response_model(config=config, metamodel=metamodel) if metamodel is not None else None
-            create_detailed_meta_endpoint(metamodel=metamodel, config=config, router=router, basic_config=basic_config)
+            create_detailed_meta_endpoint(
+                metamodel=metamodel, config=config, configs=configs, router=router, basic_config=basic_config
+            )
             for am in methods:
                 create_config_endpoint(
                     apimethod=am,
                     config=config,
                     router=router,
                     response_model=response_model,
                     metamodel=metamodel,
```

### Comparing `bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         self._real_default = ast.literal_eval(self.default) if self.default else None
         return cast(str, self._real_default)
 
 
 class MetadataDetailResult(BaseModel):
     partition_values: Optional[list[dict[str, Any]]]
     partition_columns: List[str]
-    max_string_lengths: dict[str, int]
+    max_string_lengths: dict[str, Optional[int]]
     data_schema: list[MetadataSchemaField]
     delta_meta: Optional[dict]
     delta_schema: Any
     parameters: Optional[List[Any]]
     search: Optional[List[Any]]
```

### Comparing `bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.6/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.4.7/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.6/pyproject.toml` & `bmsdna_lakeapi-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.4.6"
+version = "0.4.7"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.4.6/PKG-INFO` & `bmsdna_lakeapi-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.4.6
+Version: 0.4.7
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

