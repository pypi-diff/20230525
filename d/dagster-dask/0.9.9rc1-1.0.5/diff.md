# Comparing `tmp/dagster-dask-0.9.9rc1.tar.gz` & `tmp/dagster-dask-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-dask-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:46 2020, max compression
+gzip compressed data, was "dagster-dask-1.0.5.tar", last modified: Fri Aug 26 13:44:45 2022, max compression
```

## Comparing `dagster-dask-0.9.9rc1.tar` & `dagster-dask-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,22 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      652 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      122 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/dagster_dask/
--rw-r--r--   0 bobchen    (501) staff       (20)      278 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    18787 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask/data_frame.py
--rw-r--r--   0 bobchen    (501) staff       (20)    12368 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask/executor.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/dagster_dask.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      652 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/dagster_dask.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      578 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/dagster_dask.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/dagster_dask.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/dagster_dask.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)      136 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/dagster_dask.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       32 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/dagster_dask.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/dagster_dask_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2962 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask_tests/test_data_frame.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3429 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask_tests/test_execute.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2373 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask_tests/test_graphql.py
--rw-r--r--   0 bobchen    (501) staff       (20)      350 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask_tests/test_resource_tags.py
--rw-r--r--   0 bobchen    (501) staff       (20)       90 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1327 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:45.252222 dagster-dask-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-dask-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       64 2022-08-26 13:33:01.000000 dagster-dask-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      732 2022-08-26 13:44:45.252222 dagster-dask-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      122 2022-08-26 13:33:01.000000 dagster-dask-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:45.252222 dagster-dask-1.0.5/dagster_dask/
+-rw-r--r--   0 root         (0) root         (0)      316 2022-08-26 13:33:01.000000 dagster-dask-1.0.5/dagster_dask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19393 2022-08-26 13:33:01.000000 dagster-dask-1.0.5/dagster_dask/data_frame.py
+-rw-r--r--   0 root         (0) root         (0)    12332 2022-08-26 13:33:01.000000 dagster-dask-1.0.5/dagster_dask/executor.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-dask-1.0.5/dagster_dask/py.typed
+-rw-r--r--   0 root         (0) root         (0)     5870 2022-08-26 13:33:01.000000 dagster-dask-1.0.5/dagster_dask/resources.py
+-rw-r--r--   0 root         (0) root         (0)     6454 2022-08-26 13:33:01.000000 dagster-dask-1.0.5/dagster_dask/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-dask-1.0.5/dagster_dask/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:45.252222 dagster-dask-1.0.5/dagster_dask.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      732 2022-08-26 13:44:45.000000 dagster-dask-1.0.5/dagster_dask.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2022-08-26 13:44:45.000000 dagster-dask-1.0.5/dagster_dask.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:44:45.000000 dagster-dask-1.0.5/dagster_dask.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:44:45.000000 dagster-dask-1.0.5/dagster_dask.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      143 2022-08-26 13:44:45.000000 dagster-dask-1.0.5/dagster_dask.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-08-26 13:44:45.000000 dagster-dask-1.0.5/dagster_dask.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      159 2022-08-26 13:44:45.256222 dagster-dask-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1662 2022-08-26 13:33:01.000000 dagster-dask-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-dask-0.9.9rc1/LICENSE` & `dagster-dask-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-dask-0.9.9rc1/PKG-INFO` & `dagster-dask-1.0.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: dagster-dask
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: Package for using Dask as Dagster's execution engine.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-dask
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Provides-Extra: kube
 Provides-Extra: yarn
 Provides-Extra: pbs
+Provides-Extra: kube
+Provides-Extra: test
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-dask-0.9.9rc1/dagster_dask/data_frame.py` & `dagster-dask-1.0.5/dagster_dask/data_frame.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,63 @@
-import warnings
+import contextlib
 
 import dask.dataframe as dd
 
 from dagster import (
     Any,
     AssetMaterialization,
     Bool,
     DagsterInvariantViolationError,
     DagsterType,
     Enum,
     EnumValue,
-    EventMetadataEntry,
     Field,
     Int,
+    MetadataEntry,
     Permissive,
     Selector,
+    Shape,
     String,
     TypeCheck,
-    check,
-    dagster_type_loader,
-    dagster_type_materializer,
 )
+from dagster import _check as check
+from dagster import dagster_type_loader, dagster_type_materializer
+
+from .utils import DataFrameUtilities, apply_utilities_to_df
 
 WriteCompressionTextOptions = Enum(
-    "WriteCompressionText", [EnumValue("gzip"), EnumValue("bz2"), EnumValue("xz"),],
+    "WriteCompressionText",
+    [
+        EnumValue("gzip"),
+        EnumValue("bz2"),
+        EnumValue("xz"),
+    ],
 )
 
 EngineParquetOptions = Enum(
-    "EngineParquet", [EnumValue("auto"), EnumValue("fastparquet"), EnumValue("pyarrow"),],
+    "EngineParquet",
+    [
+        EnumValue("auto"),
+        EnumValue("fastparquet"),
+        EnumValue("pyarrow"),
+    ],
 )
 
 
 DataFrameReadTypes = {
     "csv": {
         "function": dd.read_csv,
         "is_path_based": True,
         "options": {
             "path": (Any, True, "Absolute or relative filepath(s)."),
-            "blocksize": (Any, False, "Number of bytes by which to cut up larger files."),
+            "blocksize": (
+                Any,
+                False,
+                "Number of bytes by which to cut up larger files.",
+            ),
             "sample": (Int, False, "Number of bytes to use when determining dtypes."),
             "assume_missing": (
                 Bool,
                 False,
                 "If True, all integer columns that aren’t specified in `dtype` are assumed to contain missing values, and are converted to floats.",
             ),
             "storage_options": (
@@ -57,29 +73,37 @@
         },
     },
     "parquet": {
         "function": dd.read_parquet,
         "is_path_based": True,
         "options": {
             "path": (Any, True, "Absolute or relative filepath(s)."),
-            "columns": (Any, False, "Field name(s) to read in as columns in the output."),
+            "columns": (
+                Any,
+                False,
+                "Field name(s) to read in as columns in the output.",
+            ),
             "filters": (Any, False, "List of filters to apply."),
             "index": (Any, False, "Field name(s) to use as the output frame index."),
             "categories": (
                 Any,
                 False,
                 "For any fields listed here, if the parquet encoding is Dictionary, the column will be created with dtype category.",
             ),
             "storage_options": (
                 Permissive(),
                 False,
                 "Key/value pairs to be passed on to the file-system backend, if any.",
             ),
             "engine": (EngineParquetOptions, False, "Parquet reader library to use."),
-            "gather_statistics": (Bool, False, "Gather the statistics for each dataset partition."),
+            "gather_statistics": (
+                Bool,
+                False,
+                "Gather the statistics for each dataset partition.",
+            ),
             "split_row_groups": (
                 Bool,
                 False,
                 "If True (default) then output dataframe partitions will correspond to parquet-file row-groups.",
             ),
             "chunksize": (Any, False, "The target task partition size."),
         },
@@ -95,15 +119,19 @@
             "columns": (list, False, "A list of columns names to return."),
             "chunksize": (Any, False, "Maximal number of rows per partition."),
             "sorted_index": (
                 Bool,
                 False,
                 "Option to specify whether or not the input hdf files have a sorted index.",
             ),
-            "lock": (Bool, False, "Option to use a lock to prevent concurrency issues."),
+            "lock": (
+                Bool,
+                False,
+                "Option to use a lock to prevent concurrency issues.",
+            ),
             "mode": (String, False, "Mode to use when opening file(s)."),
         },
     },
     "json": {
         "function": dd.read_json,
         "is_path_based": True,
         "options": {
@@ -111,15 +139,19 @@
             "encoding": (String, False, "The text encoding to implement."),
             "errors": (String, False, "How to respond to errors in the conversion."),
             "storage_options": (
                 Permissive(),
                 False,
                 "Passed to backend file-system implementation.",
             ),
-            "blocksize": (Int, False, "Each partition will be approximately this size in bytes."),
+            "blocksize": (
+                Int,
+                False,
+                "Each partition will be approximately this size in bytes.",
+            ),
             "sample": (
                 Int,
                 False,
                 "Number of bytes to pre-load, to provide an empty dataframe structure to any blocks without data.",
             ),
             "compression": (String, False, "String like ‘gzip’ or ‘xz’."),
         },
@@ -131,18 +163,30 @@
             "table": (Any, True, "Select columns from here."),
             "uri": (String, True, "Full sqlalchemy URI for the database connection."),
             "index_col": (
                 String,
                 True,
                 "Column which becomes the index, and defines the partitioning.",
             ),
-            "divisions": (Any, False, "Values of the index column to split the table by."),
-            "npartitions": (Int, False, "Number of partitions, if divisions is not given."),
+            "divisions": (
+                Any,
+                False,
+                "Values of the index column to split the table by.",
+            ),
+            "npartitions": (
+                Int,
+                False,
+                "Number of partitions, if divisions is not given.",
+            ),
             "columns": (Any, False, "Which columns to select."),
-            "bytes_per_chunk": (Any, False, "The target size of each partition, in bytes."),
+            "bytes_per_chunk": (
+                Any,
+                False,
+                "The target size of each partition, in bytes.",
+            ),
             "head_rows": (
                 Int,
                 False,
                 "How many rows to load for inferring the data-types, unless passing meta.",
             ),
             "schema": (
                 String,
@@ -152,15 +196,19 @@
         },
     },
     "table": {
         "function": dd.read_table,
         "is_path_based": True,
         "options": {
             "path": (Any, True, "Absolute or relative filepath(s)."),
-            "blocksize": (Any, False, "Number of bytes by which to cut up larger files."),
+            "blocksize": (
+                Any,
+                False,
+                "Number of bytes by which to cut up larger files.",
+            ),
             "sample": (Int, False, "Number of bytes to use when determining dtypes."),
             "assume_missing": (
                 Bool,
                 False,
                 "If True, all integer columns that aren’t specified in dtype are assumed to contain missing values, and are converted to floats.",
             ),
             "storage_options": (
@@ -176,15 +224,19 @@
         },
     },
     "fwf": {
         "function": dd.read_fwf,
         "is_path_based": True,
         "options": {
             "path": (Any, True, "Absolute or relative filepath(s)."),
-            "blocksize": (Any, False, "Number of bytes by which to cut up larger files."),
+            "blocksize": (
+                Any,
+                False,
+                "Number of bytes by which to cut up larger files.",
+            ),
             "sample": (Int, False, "Number of bytes to use when determining dtypes."),
             "assume_missing": (
                 Bool,
                 False,
                 "If True, all integer columns that aren’t specified in dtype are assumed to contain missing values, and are converted to floats.",
             ),
             "storage_options": (
@@ -216,28 +268,35 @@
 
 
 DataFrameToTypes = {
     "csv": {
         "function": dd.DataFrame.to_csv,
         "is_path_based": True,
         "options": {
-            "path": (Any, True, "Path glob indicating the naming scheme for the output files"),
-            "single_file": (Bool, False, "Whether to save everything into a single CSV file."),
+            "path": (
+                Any,
+                True,
+                "Path glob indicating the naming scheme for the output files",
+            ),
+            "single_file": (
+                Bool,
+                False,
+                "Whether to save everything into a single CSV file.",
+            ),
             "encoding": (
                 String,
                 False,
                 "A string representing the encoding to use in the output file.",
             ),
             "mode": (String, False, "Python write mode."),
             "compression": (
                 WriteCompressionTextOptions,
                 False,
                 "A string representing the compression to use in the output file.",
             ),
-            "compute": (Bool, False, "If true, immediate executes."),
             "compute_kwargs": (
                 Permissive(),
                 False,
                 "Options to be passed in to the compute method.",
             ),
         },
     },
@@ -249,15 +308,19 @@
             "engine": (EngineParquetOptions, False, "Parquet library to use."),
             "compression": (
                 Any,
                 False,
                 'Either a string like ``"snappy"`` or a dictionary mapping column names to compressors like ``{"name": "gzip", "values": "snappy"}``.',
             ),
             "write_index": (Bool, False, "Whether or not to write the index."),
-            "append": (Bool, False, "Whether to add new row-group(s) to an existing data-set."),
+            "append": (
+                Bool,
+                False,
+                "Whether to add new row-group(s) to an existing data-set.",
+            ),
             "ignore_divisions": (
                 Bool,
                 False,
                 "If False (default) raises error when previous divisions overlap with the new appended divisions.",
             ),
             "partition_on": (
                 list,
@@ -270,71 +333,80 @@
                 "Key/value pairs to be passed on to the file-system backend, if any.",
             ),
             "write_metadata_file": (
                 Bool,
                 False,
                 "Whether to write the special ``_metadata`` file.",
             ),
-            "compute": (Bool, False, "If true, immediate executes."),
             "compute_kwargs": (
                 Permissive(),
                 False,
                 "Options to be passed in to the compute method.",
             ),
+            "schema": (
+                Any,
+                False,
+                "Global schema to use for the output dataset.",
+            ),
         },
     },
     "hdf": {
         "function": dd.DataFrame.to_hdf,
         "is_path_based": True,
         "options": {
             "path": (Any, True, "Path to a target filename."),
             "key": (String, True, "Datapath within the files."),
-            "compute": (Bool, False, "Whether or not to execute immediately."),
-            "scheduler": (String, False, 'The scheduler to use, like "threads" or "processes".'),
+            "scheduler": (
+                String,
+                False,
+                'The scheduler to use, like "threads" or "processes".',
+            ),
         },
     },
     "json": {
         "function": dd.DataFrame.to_json,
         "is_path_based": True,
         "options": {
             "path": (Any, True, "Location to write to."),
             "encoding": (String, False, "The text encoding to implement."),
             "errors": (String, False, "How to respond to errors in the conversion."),
             "storage_options": (
                 Permissive(),
                 False,
                 "Passed to backend file-system implementation.",
             ),
-            "compute": (Bool, False, "If true, immediate executes."),
             "compute_kwargs": (
                 Permissive(),
                 False,
                 "Options to be passed in to the compute method.",
             ),
             "compression": (String, False, 'String like "gzip" or "xz".'),
         },
     },
     "sql": {
         "function": dd.DataFrame.to_sql,
         "is_path_based": False,
         "options": {
             "name": (String, True, "Name of SQL table."),
             "uri": (String, True, "Full sqlalchemy URI for the database connection."),
-            "schema": (String, False, "Specify the schema (if database flavor supports this)."),
+            "schema": (
+                String,
+                False,
+                "Specify the schema (if database flavor supports this).",
+            ),
             "if_exists": (String, False, "How to behave if the table already exists."),
             "index": (Bool, False, "Write DataFrame index as a column."),
             "index_label": (Any, False, "Column label for index column(s)."),
             "chunksize": (
                 Int,
                 False,
                 "Specify the number of rows in each batch to be written at a time.",
             ),
             "dtype": (Any, False, "Specifying the datatype for columns."),
             "method": (String, False, "Controls the SQL insertion clause used."),
-            "compute": (Bool, False, "When true, call dask.compute and perform the load into SQL."),
             "parallel": (
                 Bool,
                 False,
                 "When true, have each block append itself to the DB table concurrently.",
             ),
         },
     },
@@ -342,48 +414,40 @@
 
 
 def _dataframe_loader_config():
     read_fields = {
         read_from: Permissive(
             {
                 option_name: Field(
-                    option_args[0], is_required=option_args[1], description=option_args[2]
+                    option_args[0],
+                    is_required=option_args[1],
+                    description=option_args[2],
                 )
                 for option_name, option_args in read_opts["options"].items()
             }
         )
         for read_from, read_opts in DataFrameReadTypes.items()
     }
 
-    return Selector(
+    return Shape(
         {
-            "read": Field(Selector(read_fields), is_required=False,),
-            # https://github.com/dagster-io/dagster/issues/2872
+            "read": Field(
+                Selector(read_fields),
+            ),
             **{
-                field_name: Field(field_config, is_required=False,)
-                for field_name, field_config in read_fields.items()
+                util_name: util_spec["options"]
+                for util_name, util_spec in DataFrameUtilities.items()
             },
         }
     )
 
 
 @dagster_type_loader(_dataframe_loader_config())
 def dataframe_loader(_context, config):
-    read_type, read_options = None, None
-    if "read" in config:
-        read_type, read_options = next(iter(config["read"].items()))
-
-    # https://github.com/dagster-io/dagster/issues/2872
-    else:
-        for key in DataFrameReadTypes:
-            if key in config:
-                read_type, read_options = key, config[key]
-                warnings.warn(
-                    "Specifying {key}: is deprecated. Use read:{key}: instead.".format(key=key)
-                )
+    read_type, read_options = next(iter(config["read"].items()))
 
     if not read_type:
         raise DagsterInvariantViolationError("No read_type found. Expected read key in config.")
     if not read_type in DataFrameReadTypes:
         raise DagsterInvariantViolationError(
             "Unsupported read_type {read_type}.".format(read_type=read_type)
         )
@@ -395,61 +459,61 @@
     read_options = dict(read_options)
 
     # Get the read function and prepare its arguments.
     read_function = read_meta["function"]
     read_args = [read_options.pop("path")] if read_meta.get("is_path_based", False) else []
     read_kwargs = read_options
 
+    # Read the dataframe and apply any utility functions
     df = read_function(*read_args, **read_kwargs)
+    df = apply_utilities_to_df(df, config)
+    df = df.persist()
 
     return df
 
 
 def _dataframe_materializer_config():
     to_fields = {
         write_to: Permissive(
             {
                 option_name: Field(
-                    option_args[0], is_required=option_args[1], description=option_args[2]
+                    option_args[0],
+                    is_required=option_args[1],
+                    description=option_args[2],
                 )
                 for option_name, option_args in to_opts["options"].items()
             }
         )
         for write_to, to_opts in DataFrameToTypes.items()
     }
 
-    return Selector(
+    return Shape(
         {
-            "to": Field(Selector(to_fields), is_required=False,),
-            # https://github.com/dagster-io/dagster/issues/2872
+            "to": Field(
+                Selector(to_fields),
+            ),
             **{
-                field_name: Field(field_config, is_required=False,)
-                for field_name, field_config in to_fields.items()
+                util_name: util_spec["options"]
+                for util_name, util_spec in DataFrameUtilities.items()
             },
         }
     )
 
 
 @dagster_type_materializer(_dataframe_materializer_config())
 def dataframe_materializer(_context, config, dask_df):
     check.inst_param(dask_df, "dask_df", dd.DataFrame)
 
-    if "to" in config:
-        to_specs = config["to"]
+    to_specs = config["to"]
 
-    # https://github.com/dagster-io/dagster/issues/2872
-    else:
-        to_specs = {
-            to_type: to_options
-            for to_type, to_options in config.items()
-            if to_type in DataFrameToTypes
-        }
-        for key in to_specs.keys():
-            warnings.warn("Specifying {key}: is deprecated. Use to:{key}: instead.".format(key=key))
+    # Apply any utility functions in preparation for materialization
+    dask_df = apply_utilities_to_df(dask_df, config)
+    dask_df = dask_df.persist()
 
+    # Materialize to specified types
     for to_type, to_options in to_specs.items():
         if not to_type in DataFrameToTypes:
             check.failed("Unsupported to_type {to_type}".format(to_type=to_type))
 
         # Get the metadata entry for the read_type in order to know which method
         # to call and whether it uses path as the first argument. And, make
         # to_options mutable if we need to pop off a path argument.
@@ -458,28 +522,35 @@
 
         # Get the to function and prepare its arguments.
         to_function = to_meta["function"]
         to_path = to_options.pop("path") if to_meta.get("is_path_based", False) else None
         to_args = [to_path] if to_path else []
         to_kwargs = to_options
 
-        to_function(dask_df, *to_args, **to_kwargs)
+        # Get the Dask client from the dask resource, if available.
+        client_context = (
+            _context.resources.dask.client.as_current()
+            if hasattr(_context.resources, "dask")
+            else contextlib.suppress()
+        )
+        with client_context:
+            to_function(dask_df, *to_args, **to_kwargs)
 
         if to_path:
             yield AssetMaterialization.file(to_path)
 
 
 def df_type_check(_, value):
     if not isinstance(value, dd.DataFrame):
         return TypeCheck(success=False)
     return TypeCheck(
         success=True,
         metadata_entries=[
             # string cast columns since they may be things like datetime
-            EventMetadataEntry.json({"columns": list(map(str, value.columns))}, "metadata"),
+            MetadataEntry("metadata", value={"columns": list(map(str, value.columns))}),
         ],
     )
 
 
 DataFrame = DagsterType(
     name="DaskDataFrame",
     description="""A Dask DataFrame is a large parallel DataFrame composed of many smaller Pandas DataFrames, split along the index.
```

### Comparing `dagster-dask-0.9.9rc1/dagster_dask/executor.py` & `dagster-dask-1.0.5/dagster_dask/executor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 import dask
 import dask.distributed
-from dagster_graphql.client.mutations import execute_execute_plan_mutation
 
-# Dask resource requirements are specified under this key
-from dagster import Executor, Field, Permissive, Selector, check, seven
-from dagster.core.definitions.executor import check_cross_process_constraints, executor
-from dagster.core.events import DagsterEvent
-from dagster.core.execution.context.system import SystemPipelineExecutionContext
-from dagster.core.execution.plan.plan import ExecutionPlan
-from dagster.core.execution.retries import Retries
-from dagster.utils import frozentags
-from dagster.utils.hosted_user_process import create_in_process_ephemeral_workspace
+from dagster import Executor, Field, Permissive, Selector, StringSource
+from dagster import _check as check
+from dagster import _seven, multiple_process_executor_requirements
+from dagster._core.definitions.executor_definition import executor
+from dagster._core.errors import raise_execution_interrupts
+from dagster._core.events import DagsterEvent
+from dagster._core.execution.api import create_execution_plan, execute_plan
+from dagster._core.execution.context.system import PlanOrchestrationContext
+from dagster._core.execution.plan.plan import ExecutionPlan
+from dagster._core.execution.retries import RetryMode
+from dagster._core.instance import DagsterInstance
+from dagster._utils import frozentags, iterate_with_context
 
+# Dask resource requirements are specified under this key
 DASK_RESOURCE_REQUIREMENTS_KEY = "dagster-dask/resource_requirements"
 
 
 @executor(
     name="dask",
+    requirements=multiple_process_executor_requirements(),
     config_schema={
         "cluster": Field(
             Selector(
                 {
+                    "existing": Field(
+                        {"address": StringSource},
+                        description="Connect to an existing scheduler.",
+                    ),
                     "local": Field(
                         Permissive(), is_required=False, description="Local cluster configuration."
                     ),
                     "yarn": Field(
                         Permissive(), is_required=False, description="YARN cluster configuration."
                     ),
                     "ssh": Field(
@@ -58,15 +66,15 @@
         )
     },
 )
 def dask_executor(init_context):
     """Dask-based executor.
 
     The 'cluster' can be one of the following:
-    ('local', 'yarn', 'ssh', 'pbs', 'moab', 'sge', 'lsf', 'slurm', 'oar', 'kube').
+    ('existing', 'local', 'yarn', 'ssh', 'pbs', 'moab', 'sge', 'lsf', 'slurm', 'oar', 'kube').
 
     If the Dask executor is used without providing executor-specific config, a local Dask cluster
     will be created (as when calling :py:class:`dask.distributed.Client() <dask:distributed.Client>`
     with :py:class:`dask.distributed.LocalCluster() <dask:distributed.LocalCluster>`).
 
     The Dask executor optionally takes the following config:
 
@@ -78,94 +86,107 @@
                     {
                         timeout?: 5,  # Timeout duration for initial connection to the scheduler
                         n_workers?: 4  # Number of workers to start
                         threads_per_worker?: 1 # Number of threads per each worker
                     }
             }
 
-    If you'd like to configure a dask executor in addition to the
-    :py:class:`~dagster.default_executors`, you should add it to the ``executor_defs`` defined on a
-    :py:class:`~dagster.ModeDefinition` as follows:
+    To use the `dask_executor`, set it as the `executor_def` when defining a job:
 
     .. code-block:: python
 
-        from dagster import ModeDefinition, default_executors, pipeline
+        from dagster import job
         from dagster_dask import dask_executor
 
-        @pipeline(mode_defs=[ModeDefinition(executor_defs=default_executors + [dask_executor])])
-        def dask_enabled_pipeline():
+        @job(executor_def=dask_executor)
+        def dask_enabled_job():
             pass
 
     """
-    check_cross_process_constraints(init_context)
     ((cluster_type, cluster_configuration),) = init_context.executor_config["cluster"].items()
     return DaskExecutor(cluster_type, cluster_configuration)
 
 
 def query_on_dask_worker(
-    workspace, variables, dependencies, instance_ref=None
+    dependencies,
+    recon_pipeline,
+    pipeline_run,
+    run_config,
+    step_keys,
+    mode,
+    instance_ref,
+    known_state,
 ):  # pylint: disable=unused-argument
     """Note that we need to pass "dependencies" to ensure Dask sequences futures during task
     scheduling, even though we do not use this argument within the function.
     """
-    return execute_execute_plan_mutation(workspace, variables, instance_ref=instance_ref)
+
+    with DagsterInstance.from_ref(instance_ref) as instance:
+        subset_pipeline = recon_pipeline.subset_for_execution_from_existing_pipeline(
+            pipeline_run.solids_to_execute
+        )
+
+        execution_plan = create_execution_plan(
+            subset_pipeline,
+            run_config=run_config,
+            step_keys_to_execute=step_keys,
+            mode=mode,
+            known_state=known_state,
+        )
+
+        return execute_plan(
+            execution_plan, subset_pipeline, instance, pipeline_run, run_config=run_config
+        )
 
 
 def get_dask_resource_requirements(tags):
     check.inst_param(tags, "tags", frozentags)
     req_str = tags.get(DASK_RESOURCE_REQUIREMENTS_KEY)
     if req_str is not None:
-        return seven.json.loads(req_str)
+        return _seven.json.loads(req_str)
 
     return {}
 
 
 class DaskExecutor(Executor):
     def __init__(self, cluster_type, cluster_configuration):
         self.cluster_type = check.opt_str_param(cluster_type, "cluster_type", default="local")
         self.cluster_configuration = check.opt_dict_param(
             cluster_configuration, "cluster_configuration"
         )
 
     @property
     def retries(self):
-        return Retries.disabled_mode()
+        return RetryMode.DISABLED
 
-    def execute(self, pipeline_context, execution_plan):
-        check.inst_param(pipeline_context, "pipeline_context", SystemPipelineExecutionContext)
+    def execute(self, plan_context, execution_plan):
+        check.inst_param(plan_context, "plan_context", PlanOrchestrationContext)
         check.inst_param(execution_plan, "execution_plan", ExecutionPlan)
         check.param_invariant(
-            isinstance(pipeline_context.executor, DaskExecutor),
-            "pipeline_context",
-            "Expected executor to be DaskExecutor got {}".format(pipeline_context.executor),
+            isinstance(plan_context.executor, DaskExecutor),
+            "plan_context",
+            "Expected executor to be DaskExecutor got {}".format(plan_context.executor),
         )
 
-        # Checks to ensure storage is compatible with Dask configuration
-        storage = pipeline_context.run_config.get("storage")
-        check.invariant(storage.keys(), "Must specify storage to use Dask execution")
-
         check.invariant(
-            pipeline_context.instance.is_persistent,
+            plan_context.instance.is_persistent,
             "Dask execution requires a persistent DagsterInstance",
         )
 
-        # https://github.com/dagster-io/dagster/issues/2440
-        check.invariant(
-            pipeline_context.system_storage_def.is_persistent,
-            "Cannot use in-memory storage with Dask, use filesystem, S3, or GCS",
-        )
-
-        step_levels = execution_plan.execution_step_levels()
+        step_levels = execution_plan.get_steps_to_execute_by_level()
 
-        pipeline_name = pipeline_context.pipeline_def.name
+        pipeline_name = plan_context.pipeline_name
 
-        instance = pipeline_context.instance
+        instance = plan_context.instance
 
         cluster_type = self.cluster_type
-        if cluster_type == "local":
+        if cluster_type == "existing":
+            # address passed directly to Client() below to connect to existing Scheduler
+            cluster = self.cluster_configuration["address"]
+        elif cluster_type == "local":
             from dask.distributed import LocalCluster
 
             cluster = LocalCluster(**self.build_dict(pipeline_name))
         elif cluster_type == "yarn":
             from dask_yarn import YarnCluster
 
             cluster = YarnCluster(**self.build_dict(pipeline_name))
@@ -199,15 +220,15 @@
             cluster = OARCluster(**self.build_dict(pipeline_name))
         elif cluster_type == "kube":
             from dask_kubernetes import KubeCluster
 
             cluster = KubeCluster(**self.build_dict(pipeline_name))
         else:
             raise ValueError(
-                f"Must be providing one of the following ('local', 'yarn', 'ssh', 'pbs', 'moab', 'sge', 'lsf', 'slurm', 'oar', 'kube') not {cluster_type}"
+                f"Must be providing one of the following ('existing', 'local', 'yarn', 'ssh', 'pbs', 'moab', 'sge', 'lsf', 'slurm', 'oar', 'kube') not {cluster_type}"
             )
 
         with dask.distributed.Client(cluster) as client:
             execution_futures = []
             execution_futures_dict = {}
 
             for step_level in step_levels:
@@ -215,55 +236,48 @@
                     # We ensure correctness in sequencing by letting Dask schedule futures and
                     # awaiting dependencies within each step.
                     dependencies = []
                     for step_input in step.step_inputs:
                         for key in step_input.dependency_keys:
                             dependencies.append(execution_futures_dict[key])
 
-                    run_config = dict(pipeline_context.run_config, execution={"in_process": {}})
-                    recon_repo = pipeline_context.pipeline.get_reconstructable_repository()
-                    variables = {
-                        "executionParams": {
-                            "selector": {
-                                "pipelineName": pipeline_name,
-                                "repositoryName": recon_repo.get_definition().name,
-                                "repositoryLocationName": "<<in_process>>",
-                            },
-                            "runConfigData": run_config,
-                            "mode": pipeline_context.mode_def.name,
-                            "executionMetadata": {"runId": pipeline_context.pipeline_run.run_id},
-                            "stepKeys": [step.key],
-                        }
-                    }
+                    if plan_context.pipeline.get_definition().is_job:
+                        run_config = plan_context.run_config
+                    else:
+                        run_config = dict(plan_context.run_config, execution={"in_process": {}})
 
                     dask_task_name = "%s.%s" % (pipeline_name, step.key)
 
-                    workspace = create_in_process_ephemeral_workspace(
-                        pointer=pipeline_context.pipeline.get_reconstructable_repository().pointer
-                    )
+                    recon_pipeline = plan_context.reconstructable_pipeline
 
                     future = client.submit(
                         query_on_dask_worker,
-                        workspace,
-                        variables,
                         dependencies,
+                        recon_pipeline,
+                        plan_context.pipeline_run,
+                        run_config,
+                        [step.key],
+                        plan_context.pipeline_run.mode,
                         instance.get_ref(),
+                        execution_plan.known_state,
                         key=dask_task_name,
                         resources=get_dask_resource_requirements(step.tags),
                     )
 
                     execution_futures.append(future)
                     execution_futures_dict[step.key] = future
 
             # This tells Dask to awaits the step executions and retrieve their results to the
             # master
-            for future in dask.distributed.as_completed(execution_futures):
-                for step_event in future.result():
-                    check.inst(step_event, DagsterEvent)
+            futures = dask.distributed.as_completed(execution_futures, with_results=True)
 
+            # Allow interrupts while waiting for the results from Dask
+            for future, result in iterate_with_context(raise_execution_interrupts, futures):
+                for step_event in result:
+                    check.inst(step_event, DagsterEvent)
                     yield step_event
 
     def build_dict(self, pipeline_name):
         """Returns a dict we can use for kwargs passed to dask client instantiation.
 
         Intended to be used like:
```

### Comparing `dagster-dask-0.9.9rc1/dagster_dask.egg-info/PKG-INFO` & `dagster-dask-1.0.5/dagster_dask.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: dagster-dask
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: Package for using Dask as Dagster's execution engine.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-dask
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Provides-Extra: kube
 Provides-Extra: yarn
 Provides-Extra: pbs
+Provides-Extra: kube
+Provides-Extra: test
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-dask-0.9.9rc1/setup.py` & `dagster-dask-1.0.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,49 @@
+from typing import Dict
+
 from setuptools import find_packages, setup
 
 
-def get_version():
-    version = {}
-    with open("dagster_dask/version.py") as fp:
+def get_version() -> str:
+    version: Dict[str, str] = {}
+    with open("dagster_dask/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
 if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
     setup(
         name="dagster-dask",
-        version=get_version(),
+        version=ver,
         author="Elementl",
         author_email="hello@elementl.com",
         license="Apache-2.0",
         description="Package for using Dask as Dagster's execution engine.",
         url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-dask",
         classifiers=[
-            "Programming Language :: Python :: 2.7",
-            "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: OS Independent",
         ],
-        packages=find_packages(exclude=["test"]),
+        packages=find_packages(exclude=["dagster_dask_tests*"]),
         install_requires=[
             "bokeh",
-            "dagster",
-            "dagster_graphql",
+            "dagster==1.0.5",
             "dask[dataframe]>=1.2.2",
             "distributed>=1.28.1",
         ],
         extras_require={
             "yarn": ["dask-yarn"],
             "pbs": ["dask-jobqueue"],
             "kube": ["dask-kubernetes"],
+            # we need `pyarrow` for testing read/write parquet files.
+            "test": ["pyarrow"],
         },
         zip_safe=False,
     )
```

