# Comparing `tmp/bmsdna_lakeapi-0.4.4.tar.gz` & `tmp/bmsdna_lakeapi-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.4.4.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.4.5.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.4.4.tar` & `bmsdna_lakeapi-0.4.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1081 2023-05-24 15:07:14.236469 bmsdna_lakeapi-0.4.4/LICENSE
--rw-r--r--   0        0        0     6939 2023-05-24 15:07:14.236469 bmsdna_lakeapi-0.4.4/README.md
--rw-r--r--   0        0        0      271 2023-05-24 15:07:14.236469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 15:07:14.236469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1074 2023-05-24 15:07:14.236469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      926 2023-05-24 15:07:14.236469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     5989 2023-05-24 15:07:14.236469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0     4072 2023-05-24 15:07:14.236469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/context/df_datafusion.py
--rw-r--r--   0        0        0     8573 2023-05-24 15:07:14.236469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6390 2023-05-24 15:07:14.236469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-05-24 15:07:14.236469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    11432 2023-05-24 15:07:14.236469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    11623 2023-05-24 15:07:14.236469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    19268 2023-05-24 15:07:14.236469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-05-24 15:07:14.236469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-05-24 15:07:14.236469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6836 2023-05-24 15:07:14.236469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     7822 2023-05-24 15:07:14.240469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4450 2023-05-24 15:07:14.240469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3141 2023-05-24 15:07:14.240469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2367 2023-05-24 15:07:14.240469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-05-24 15:07:14.240469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-05-24 15:07:14.240469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-05-24 15:07:14.240469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      326 2023-05-24 15:07:14.240469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1790 2023-05-24 15:07:14.240469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-05-24 15:07:14.240469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-05-24 15:07:14.240469 bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     1842 2023-05-24 15:07:14.240469 bmsdna_lakeapi-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     8233 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-24 15:39:29.639444 bmsdna_lakeapi-0.4.5/LICENSE
+-rw-r--r--   0        0        0     7758 2023-05-24 15:39:29.639444 bmsdna_lakeapi-0.4.5/README.md
+-rw-r--r--   0        0        0      271 2023-05-24 15:39:29.639444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 15:39:29.639444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1074 2023-05-24 15:39:29.639444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      926 2023-05-24 15:39:29.639444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     5989 2023-05-24 15:39:29.639444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0     4072 2023-05-24 15:39:29.639444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/context/df_datafusion.py
+-rw-r--r--   0        0        0     8573 2023-05-24 15:39:29.639444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6390 2023-05-24 15:39:29.639444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-05-24 15:39:29.639444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    11432 2023-05-24 15:39:29.639444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    11623 2023-05-24 15:39:29.639444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    19376 2023-05-24 15:39:29.643444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-05-24 15:39:29.643444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-05-24 15:39:29.643444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6836 2023-05-24 15:39:29.643444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     7822 2023-05-24 15:39:29.643444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4450 2023-05-24 15:39:29.643444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3141 2023-05-24 15:39:29.643444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2367 2023-05-24 15:39:29.643444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-05-24 15:39:29.643444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-05-24 15:39:29.643444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-05-24 15:39:29.643444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      326 2023-05-24 15:39:29.643444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1790 2023-05-24 15:39:29.643444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-05-24 15:39:29.643444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-05-24 15:39:29.643444 bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     1842 2023-05-24 15:39:29.643444 bmsdna_lakeapi-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     9052 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.4.5/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.4.4/LICENSE` & `bmsdna_lakeapi-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.4/README.md` & `bmsdna_lakeapi-0.4.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 <h1 align="center">
   <img src="assets\LakeAPI.drawio.png">
   <br>
 </h1>
 
 [![tests](https://github.com/bmsuisse/lakeapi/actions/workflows/python-test.yml/badge.svg?branch=main)](https://github.com/bmsuisse/lakeapi/actions/workflows/python-test.yml)
 
-A FastAPI Plugin that allows you to expose your Data Lake as an API, allowing multiple output formats, such as Parquet, Csv, Json, Excel, ...
+A FastAPI plugin that allows you to expose your data lake as an API, allowing several output formats such as Parquet, Csv, Json, Excel, ...
 
-The lake API also contains a minimal security layer for convenience (Basic Auth), but you can also bring your own.
+The Lake API also includes a minimal security layer for convenience (Basic Auth), but you can also bring your own.
 
-It contrast to [roapi](https://github.com/roapi/roapi), we intentionally do not want to expose most SQL by default, but we limit possible queries using a config. This makes it easy for you to control what happens on your data. If you want the sql endpoint, you can enable this.
+Unlike [roapi](https://github.com/roapi/roapi), we intentionally do not expose most SQL by default, but limit the possible queries with a config. This makes it easy for you to control what happens to your data. If you want the SQL endpoint, you can enable it.
 
-To run the app with default config, just do:
+To run the application with the default config, just do it:
 
 ```python
 app = FastAPI()
 bmsdna.lakeapi.init_lakeapi(app)
 ```
 
 To adjust the config, you can do like this:
@@ -39,18 +39,17 @@
 
 ## OpenApi
 
 Of course, everything works with Open API and FastAPI. Meaning you can add other FastAPI routes, you can use the /docs and /redoc endpoint.
 
 ## Engine
 
-By default, DuckDB is the query engine. Polars and Datafusion are also supported, but lack some features.
-The query engine can be defined on a route level and on a query level with the hidden parameter $engine="duckdb|datafusion|polars". If you want polars or datafusion, also add the extra required
+`DuckDB` is the default query engine. `Polars` and `Datafusion` are also supported, but lack some features. The query engine can be specified at the route level and at the query level with the hidden parameter $engine="duckdb|datafusion|polars". If you want polars or datafusion, add the required extra.
 
-At the moment DuckDB seems to have an edge and performances the best. Also features like full text search are only available with DuckDB.
+At the moment, DuckDB seems to have an advantage and performs the best. Also features like full text search are only available with `DuckDB`.
 
 ## Default Security
 
 By Default, Basic Authentication is enabled. To add a user, simply run `add_lakeapi_user YOURUSERNAME --yaml-file config.yml`. This will add the user to your config yaml (argon2 encrypted).
 The generated Password is printed. If you do not want this logic, you can overwrite the username_retriver of the Default Config
 
 ## Standalone Mode
@@ -181,27 +180,41 @@
     api_method:
       - get
     datasource:
       uri: startest/fruits
       file_type: delta
 ```
 
-## Partioning for awesome performance
+## Partitioning for awesome performance
 
-In order to use partitions, you can either:
+To use partitions, you can either
 
-- partition by a column you filter on. Obviously
-- partition on a special column called `columnname_md5_prefix_2` which means that you're partitioning by the first two chars of
-  your hex-encoded md5 hash. If you now filter by `columnname` this will greatly reduce files searched for. The number of chars used is up to you, we found two to be meaningful
-- partition on a special column called `columnname_md5_mod_NRPARTIIONS` where your partition value is `str(int(hashlib.md5(COLUMNNAME).hexdigest(), 16) % NRPARTITIONS)`. That might look a bit complicated, but it's not that hard :) your just doing a modulo on your md5 hash which
-  allows you to set the exact number of partitions. Filtering is still happening on `columname` correctly
+- Partition by a column that you filter on. Obviously
+- partition on a special column called `columnname_md5_prefix_2`, which means that you're partitioning on the first two characters of your hex-coded md5 hash.
+  of the hexadecimal md5 hash. If you now filter by `columnname`, this will greatly reduce the number of files you search for. The number of characters used is up to you, we found two to be useful
+- partition on a special column called `columnname_md5_mod_NRPARTITIONS`, where your partition value is `str(int(hashlib.md5(COLUMNNAME).hexdigest(), 16) % NRPARTITIONS)`. This might look a bit complicated, but it's not that hard :) You're just doing a modulo on your md5 hash, which allows you to
+  which allows you to set the exact number of partitions. Filtering is still done correctly on `columnname`.
 
-You must use deltalake to use parttions and you must only have str partition columns for now.
+Why partition by MD5 hash? Imagine you have a product id where most id's start with a 1 and some newer ones start with a 2. Most of the data will be in the first partition. If you use an MD5 hash, the data will be spread evenly across the partitions.
+
+With this hack you can get sub-second results on very large data. 🚀🚀🚀
+
+You need to use `deltalake` to use partitions, and you only need str partition columns for now.
+
+[Z-ordering](https://docs.delta.io/latest/optimizations-oss.html#z-ordering-multi-dimensional-clustering) can also help a lot :). This approach should only be used for very large datasets.
 
 ## Even more features
 
-- Paging built-in, you can use limit/offset to control what you receive
-- Full-text Search using DuckDB's Full Text Search Feature
-- jsonify_complex Parameter to turn structs/lists into Json the client cannot deal with structs/lists
+- Built-in paging, you can use limit/offset to control what you get
+- Full-text search using DuckDB's full-text search feature
+- jsonify_complex parameter to convert structs/lists to json, the client cannot handle structs/lists
 - Metadata endpoints to retrieve data types, string lengths and more
-- Expose whole folders easily by using a "\*" wildcard in both the name and the datasource.uri config, see sample in above config
+- Easily expose entire folders by using a "\*" wildcard in both the name and the datasource.uri config, see example in the config above
 - Good test coverage
+
+## Work in progress
+
+Please note that this is a work in progress, changes may be made and things may break. Especially at this early stage.
+
+## Contribution
+
+Feel free to contribute, report bugs or request enhancements.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/context/df_base.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/context/df_datafusion.py` & `bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/context/df_datafusion.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/config.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
 def create_detailed_meta_endpoint(
     metamodel: Optional[ResultData], config: Config, router: APIRouter, basic_config: BasicConfig
 ):
     route = config.route + "/metadata_detail"
     has_complex = True
     if metamodel is not None:
-        has_complex = any((pa.types.is_struct(t) or pa.types.is_list(t) for t in metamodel.arrow_schema().types))
+        has_complex = any((pa.types.is_nested(t) for t in metamodel.arrow_schema().types))
 
     @router.get(
         route,
         tags=["metadata", "metadata:" + config.tag],
         operation_id=config.tag + "_" + config.name,
         name=config.name + "_metadata",
     )
@@ -157,15 +157,19 @@
                 ]  # also hide those from metadata detail
                 if len(partition_columns) > 0:
                     qb: QueryBuilder = (
                         df.query_builder().select(*[pypika.Field(c) for c in partition_columns]).distinct()
                     )
                     partition_values = context.execute_sql(qb).to_arrow_table().to_pylist()
             schema = df.arrow_schema()
-            str_cols = [name for name in schema.names if pa.types.is_string(schema.field(name).type)]
+            str_cols = [
+                name
+                for name in schema.names
+                if pa.types.is_string(schema.field(name).type) or pa.types.is_large_string(schema.field(name).type)
+            ]
             complex_str_cols = (
                 [
                     name
                     for name in schema.names
                     if pa.types.is_struct(schema.field(name).type) or pa.types.is_list(schema.field(name).type)
                 ]
                 if jsonify_complex
@@ -192,27 +196,27 @@
                 )
                 if len(str_cols) > 0 or len(complex_str_cols) > 0
                 else [{}]
             )
             str_lengths = str_lengths_df[0]
 
             def _recursive_get_type(t: pa.DataType) -> MetadataSchemaFieldType:
-                is_complex = pa.types.is_struct(t) or pa.types.is_list(t)
+                is_complex = pa.types.is_nested(t)
 
                 return MetadataSchemaFieldType(
                     type_str=str(pa.string()) if is_complex and jsonify_complex else str(t),
                     orig_type_str=str(t),
                     fields=[
                         MetadataSchemaField(name=f.name, type=_recursive_get_type(f.type))
                         for f in [t.field(find) for find in range(0, cast(pa.StructType, t).num_fields)]
                     ]
                     if pa.types.is_struct(t) and not jsonify_complex
                     else None,
                     inner=_recursive_get_type(t.value_type)
-                    if pa.types.is_list(t) and t.value_type is not None and not jsonify_complex
+                    if pa.types.is_list(t) or pa.types.is_large_list(t) or pa.types.is_fixed_size_list(t) and t.value_type is not None and not jsonify_complex
                     else None,
                 )
 
             schema = df.arrow_schema()
             return MetadataDetailResult(
                 partition_values=partition_values,
                 partition_columns=partition_columns,
@@ -230,15 +234,15 @@
 def exclude_cols(columns: List[str]) -> List[str]:
     columns = [c for c in columns if not should_hide_colname(c)]
     return columns
 
 
 def is_complex_type(schema: pa.Schema, col_name: str):
     f = schema.field(col_name)
-    return pa.types.is_struct(f.type) or pa.types.is_list(f.type)
+    return pa.types.is_nested(f.type)
 
 
 def create_config_endpoint(
     metamodel: Optional[ResultData],
     apimethod: Literal["get", "post"],
     config: Config,
     router: APIRouter,
```

### Comparing `bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/route.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.4/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.4.5/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.4.4/pyproject.toml` & `bmsdna_lakeapi-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.4.4"
+version = "0.4.5"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.4.4/PKG-INFO` & `bmsdna_lakeapi-0.4.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.4.4
+Version: 0.4.5
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -37,21 +37,21 @@
 <h1 align="center">
   <img src="assets\LakeAPI.drawio.png">
   <br>
 </h1>
 
 [![tests](https://github.com/bmsuisse/lakeapi/actions/workflows/python-test.yml/badge.svg?branch=main)](https://github.com/bmsuisse/lakeapi/actions/workflows/python-test.yml)
 
-A FastAPI Plugin that allows you to expose your Data Lake as an API, allowing multiple output formats, such as Parquet, Csv, Json, Excel, ...
+A FastAPI plugin that allows you to expose your data lake as an API, allowing several output formats such as Parquet, Csv, Json, Excel, ...
 
-The lake API also contains a minimal security layer for convenience (Basic Auth), but you can also bring your own.
+The Lake API also includes a minimal security layer for convenience (Basic Auth), but you can also bring your own.
 
-It contrast to [roapi](https://github.com/roapi/roapi), we intentionally do not want to expose most SQL by default, but we limit possible queries using a config. This makes it easy for you to control what happens on your data. If you want the sql endpoint, you can enable this.
+Unlike [roapi](https://github.com/roapi/roapi), we intentionally do not expose most SQL by default, but limit the possible queries with a config. This makes it easy for you to control what happens to your data. If you want the SQL endpoint, you can enable it.
 
-To run the app with default config, just do:
+To run the application with the default config, just do it:
 
 ```python
 app = FastAPI()
 bmsdna.lakeapi.init_lakeapi(app)
 ```
 
 To adjust the config, you can do like this:
@@ -73,18 +73,17 @@
 
 ## OpenApi
 
 Of course, everything works with Open API and FastAPI. Meaning you can add other FastAPI routes, you can use the /docs and /redoc endpoint.
 
 ## Engine
 
-By default, DuckDB is the query engine. Polars and Datafusion are also supported, but lack some features.
-The query engine can be defined on a route level and on a query level with the hidden parameter $engine="duckdb|datafusion|polars". If you want polars or datafusion, also add the extra required
+`DuckDB` is the default query engine. `Polars` and `Datafusion` are also supported, but lack some features. The query engine can be specified at the route level and at the query level with the hidden parameter $engine="duckdb|datafusion|polars". If you want polars or datafusion, add the required extra.
 
-At the moment DuckDB seems to have an edge and performances the best. Also features like full text search are only available with DuckDB.
+At the moment, DuckDB seems to have an advantage and performs the best. Also features like full text search are only available with `DuckDB`.
 
 ## Default Security
 
 By Default, Basic Authentication is enabled. To add a user, simply run `add_lakeapi_user YOURUSERNAME --yaml-file config.yml`. This will add the user to your config yaml (argon2 encrypted).
 The generated Password is printed. If you do not want this logic, you can overwrite the username_retriver of the Default Config
 
 ## Standalone Mode
@@ -215,28 +214,42 @@
     api_method:
       - get
     datasource:
       uri: startest/fruits
       file_type: delta
 ```
 
-## Partioning for awesome performance
+## Partitioning for awesome performance
 
-In order to use partitions, you can either:
+To use partitions, you can either
 
-- partition by a column you filter on. Obviously
-- partition on a special column called `columnname_md5_prefix_2` which means that you're partitioning by the first two chars of
-  your hex-encoded md5 hash. If you now filter by `columnname` this will greatly reduce files searched for. The number of chars used is up to you, we found two to be meaningful
-- partition on a special column called `columnname_md5_mod_NRPARTIIONS` where your partition value is `str(int(hashlib.md5(COLUMNNAME).hexdigest(), 16) % NRPARTITIONS)`. That might look a bit complicated, but it's not that hard :) your just doing a modulo on your md5 hash which
-  allows you to set the exact number of partitions. Filtering is still happening on `columname` correctly
+- Partition by a column that you filter on. Obviously
+- partition on a special column called `columnname_md5_prefix_2`, which means that you're partitioning on the first two characters of your hex-coded md5 hash.
+  of the hexadecimal md5 hash. If you now filter by `columnname`, this will greatly reduce the number of files you search for. The number of characters used is up to you, we found two to be useful
+- partition on a special column called `columnname_md5_mod_NRPARTITIONS`, where your partition value is `str(int(hashlib.md5(COLUMNNAME).hexdigest(), 16) % NRPARTITIONS)`. This might look a bit complicated, but it's not that hard :) You're just doing a modulo on your md5 hash, which allows you to
+  which allows you to set the exact number of partitions. Filtering is still done correctly on `columnname`.
 
-You must use deltalake to use parttions and you must only have str partition columns for now.
+Why partition by MD5 hash? Imagine you have a product id where most id's start with a 1 and some newer ones start with a 2. Most of the data will be in the first partition. If you use an MD5 hash, the data will be spread evenly across the partitions.
+
+With this hack you can get sub-second results on very large data. 🚀🚀🚀
+
+You need to use `deltalake` to use partitions, and you only need str partition columns for now.
+
+[Z-ordering](https://docs.delta.io/latest/optimizations-oss.html#z-ordering-multi-dimensional-clustering) can also help a lot :). This approach should only be used for very large datasets.
 
 ## Even more features
 
-- Paging built-in, you can use limit/offset to control what you receive
-- Full-text Search using DuckDB's Full Text Search Feature
-- jsonify_complex Parameter to turn structs/lists into Json the client cannot deal with structs/lists
+- Built-in paging, you can use limit/offset to control what you get
+- Full-text search using DuckDB's full-text search feature
+- jsonify_complex parameter to convert structs/lists to json, the client cannot handle structs/lists
 - Metadata endpoints to retrieve data types, string lengths and more
-- Expose whole folders easily by using a "\*" wildcard in both the name and the datasource.uri config, see sample in above config
+- Easily expose entire folders by using a "\*" wildcard in both the name and the datasource.uri config, see example in the config above
 - Good test coverage
 
+## Work in progress
+
+Please note that this is a work in progress, changes may be made and things may break. Especially at this early stage.
+
+## Contribution
+
+Feel free to contribute, report bugs or request enhancements.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

