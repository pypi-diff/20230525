# Comparing `tmp/dagster-pyspark-0.9.9rc1.tar.gz` & `tmp/dagster-pyspark-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-pyspark-0.9.9rc1.tar", last modified: Thu Sep 17 21:07:36 2020, max compression
+gzip compressed data, was "dagster-pyspark-1.0.5.tar", last modified: Fri Aug 26 13:44:51 2022, max compression
```

## Comparing `dagster-pyspark-0.9.9rc1.tar` & `dagster-pyspark-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,21 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       16 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      542 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      131 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark/
--rw-r--r--   0 bobchen    (501) staff       (20)      283 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1151 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)    50077 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark/types.py
--rw-r--r--   0 bobchen    (501) staff       (20)      692 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark/utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      542 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      562 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)      107 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       38 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      960 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark_tests/test_resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4166 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark_tests/test_types.py
--rw-r--r--   0 bobchen    (501) staff       (20)       85 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1201 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:51.268255 dagster-pyspark-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-pyspark-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2022-08-26 13:33:01.000000 dagster-pyspark-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      651 2022-08-26 13:44:51.268255 dagster-pyspark-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2022-08-26 13:33:01.000000 dagster-pyspark-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:51.264255 dagster-pyspark-1.0.5/dagster_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      284 2022-08-26 13:33:01.000000 dagster-pyspark-1.0.5/dagster_pyspark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-pyspark-1.0.5/dagster_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1571 2022-08-26 13:33:01.000000 dagster-pyspark-1.0.5/dagster_pyspark/resources.py
+-rw-r--r--   0 root         (0) root         (0)    45885 2022-08-26 13:33:01.000000 dagster-pyspark-1.0.5/dagster_pyspark/types.py
+-rw-r--r--   0 root         (0) root         (0)      692 2022-08-26 13:33:01.000000 dagster-pyspark-1.0.5/dagster_pyspark/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-pyspark-1.0.5/dagster_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:51.268255 dagster-pyspark-1.0.5/dagster_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      651 2022-08-26 13:44:51.000000 dagster-pyspark-1.0.5/dagster_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      439 2022-08-26 13:44:51.000000 dagster-pyspark-1.0.5/dagster_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:44:51.000000 dagster-pyspark-1.0.5/dagster_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:44:51.000000 dagster-pyspark-1.0.5/dagster_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      121 2022-08-26 13:44:51.000000 dagster-pyspark-1.0.5/dagster_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2022-08-26 13:44:51.000000 dagster-pyspark-1.0.5/dagster_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2022-08-26 13:44:51.272255 dagster-pyspark-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1527 2022-08-26 13:33:01.000000 dagster-pyspark-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-pyspark-0.9.9rc1/LICENSE` & `dagster-pyspark-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-pyspark-0.9.9rc1/PKG-INFO` & `dagster-pyspark-1.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-pyspark
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: Package for PySpark Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-framework/pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-pyspark-0.9.9rc1/dagster_pyspark/resources.py` & `dagster-pyspark-1.0.5/dagster_pyspark/resources.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,54 @@
 from dagster_spark.configs_spark import spark_config
 from dagster_spark.utils import flatten_dict
 from pyspark.sql import SparkSession
 
-from dagster import check, resource
+import dagster._check as check
+from dagster import resource
 
 
 def spark_session_from_config(spark_conf=None):
     spark_conf = check.opt_dict_param(spark_conf, "spark_conf")
     builder = SparkSession.builder
     flat = flatten_dict(spark_conf)
     for key, value in flat:
         builder = builder.config(key, value)
 
     return builder.getOrCreate()
 
 
-class PySparkResource(object):
+class PySparkResource:
     def __init__(self, spark_conf):
         self._spark_session = spark_session_from_config(spark_conf)
 
     @property
     def spark_session(self):
         return self._spark_session
 
     @property
     def spark_context(self):
         return self.spark_session.sparkContext
 
 
 @resource({"spark_conf": spark_config()})
 def pyspark_resource(init_context):
-    """This resource provides access to a PySpark SparkSession for executing PySpark code within
-    Dagster.
+    """This resource provides access to a PySpark SparkSession for executing PySpark code within Dagster.
 
     Example:
 
-    .. literalinclude:: ../../../../../examples/basic_pyspark/repo.py
-       :language: python
+    .. code-block:: python
+
+        @op(required_resource_keys={"pyspark"})
+        def my_op(context):
+            spark_session = context.resources.pyspark.spark_session
+            dataframe = spark_session.read.json("examples/src/main/resources/people.json")
+
+        my_pyspark_resource = pyspark_resource.configured(
+            {"spark_conf": {"spark.executor.memory": "2g"}}
+        )
+
+        @job(resource_defs={"pyspark": my_pyspark_resource})
+        def my_spark_job():
+            my_op()
 
     """
     return PySparkResource(init_context.resource_config["spark_conf"])
```

### Comparing `dagster-pyspark-0.9.9rc1/dagster_pyspark/types.py` & `dagster-pyspark-1.0.5/dagster_pyspark/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os
-
 from pyspark.sql import DataFrame as NativeSparkDataFrame
 
 from dagster import (
     Any,
     AssetMaterialization,
     Bool,
     DagsterInvariantViolationError,
@@ -14,29 +12,32 @@
     Int,
     Permissive,
     PythonObjectDagsterType,
     String,
     dagster_type_loader,
     dagster_type_materializer,
 )
-from dagster.config.field_utils import Selector
-from dagster.core.storage.system_storage import fs_intermediate_storage, fs_system_storage
-from dagster.core.storage.type_storage import TypeStoragePlugin
-from dagster.utils import dict_without_keys
+from dagster._config import Selector
+from dagster._utils import dict_without_keys
 
 WriteModeOptions = Enum(
     "WriteMode",
     [
         EnumValue(
-            "append", description="Append contents of this :class:`DataFrame` to existing data."
+            "append",
+            description="Append contents of this :class:`DataFrame` to existing data.",
         ),
         EnumValue("overwrite", description="Overwrite existing data."),
-        EnumValue("ignore", description="Silently ignore this operation if data already exists."),
         EnumValue(
-            "error", description="(default case): Throw an exception if data already exists."
+            "ignore",
+            description="Silently ignore this operation if data already exists.",
+        ),
+        EnumValue(
+            "error",
+            description="(default case): Throw an exception if data already exists.",
         ),
         EnumValue(
             "errorifexists",
             description="(default case): Throw an exception if data already exists.",
         ),
     ],
 )
@@ -53,15 +54,20 @@
         EnumValue("deflate"),
     ],
 )
 
 
 WriteCompressionOrcOptions = Enum(
     "WriteCompressionOrc",
-    [EnumValue("none"), EnumValue("snappy"), EnumValue("zlib"), EnumValue("lzo"),],
+    [
+        EnumValue("none"),
+        EnumValue("snappy"),
+        EnumValue("zlib"),
+        EnumValue("lzo"),
+    ],
 )
 
 
 WriteCompressionParquetOptions = Enum(
     "WriteCompressionParquet",
     [
         EnumValue("none"),
@@ -178,15 +184,17 @@
                     ),
                     "mode": Field(
                         WriteModeOptions,
                         is_required=False,
                         description="specifies the behavior of the save operation when data already exists.",
                     ),
                     "partitionBy": Field(
-                        String, is_required=False, description="names of partitioning columns."
+                        String,
+                        is_required=False,
+                        description="names of partitioning columns.",
                     ),
                     "compression": Field(
                         WriteCompressionParquetOptions,
                         is_required=False,
                         description="compression codec to use when saving to file. This will override ``spark.sql.parquet.compression.codec``. If None is set, it uses the value specified in ``spark.sql.parquet.compression.codec``.",
                     ),
                 }
@@ -263,39 +271,47 @@
                     ),
                     "mode": Field(
                         WriteModeOptions,
                         is_required=False,
                         description="specifies the behavior of the save operation when data already exists.",
                     ),
                     "partitionBy": Field(
-                        String, is_required=False, description="names of partitioning columns."
+                        String,
+                        is_required=False,
+                        description="names of partitioning columns.",
                     ),
                     "compression": Field(
                         WriteCompressionOrcOptions,
                         is_required=False,
                         description="compression codec to use when saving to file. This will override ``orc.compress`` and ``spark.sql.orc.compression.codec``. If None is set, it uses the value specified in ``spark.sql.orc.compression.codec``.",
                     ),
                 }
             ),
             "saveAsTable": Permissive(
                 {
                     "name": Field(String, is_required=True, description="the table name."),
                     "format": Field(
-                        String, is_required=False, description="the format used to save."
+                        String,
+                        is_required=False,
+                        description="the format used to save.",
                     ),
                     "mode": Field(
                         WriteModeOptions,
                         is_required=False,
                         description="specifies the behavior of the save operation when data already exists.",
                     ),
                     "partitionBy": Field(
-                        String, is_required=False, description="names of partitioning columns."
+                        String,
+                        is_required=False,
+                        description="names of partitioning columns.",
                     ),
                     "options": Field(
-                        Permissive(), is_required=False, description="all other string options."
+                        Permissive(),
+                        is_required=False,
+                        description="all other string options.",
                     ),
                 }
             ),
             "text": Permissive(
                 {
                     "path": Field(
                         String,
@@ -819,15 +835,19 @@
             "jdbc": Permissive(
                 {
                     "url": Field(
                         String,
                         is_required=True,
                         description="a JDBC URL of the form ``jdbc:subprotocol:subname``.",
                     ),
-                    "table": Field(String, is_required=True, description="the name of the table.",),
+                    "table": Field(
+                        String,
+                        is_required=True,
+                        description="the name of the table.",
+                    ),
                     "column": Field(
                         String,
                         is_required=False,
                         description="""
                             the name of a column of numeric, date, or timestamp type
                             that will be used for partitioning;
                             if this parameter is specified, then ``numPartitions``, ``lowerBound``
@@ -843,15 +863,17 @@
                     ),
                     "upperBound": Field(
                         Int,
                         is_required=False,
                         description="the maximum value of ``column`` used to decide partition stride.",
                     ),
                     "numPartitions": Field(
-                        Int, is_required=False, description="the number of partitions",
+                        Int,
+                        is_required=False,
+                        description="the number of partitions",
                     ),
                     "predicates": Field(
                         list,
                         is_required=False,
                         description="""
                             a list of expressions suitable for inclusion in WHERE clauses;
                             each one defines one partition of the :class:`DataFrame`
@@ -876,15 +898,17 @@
                         description="string, or list of strings, for input path(s).",
                     ),
                 }
             ),
             "table": Permissive(
                 {
                     "tableName": Field(
-                        String, is_required=True, description="string, name of the table.",
+                        String,
+                        is_required=True,
+                        description="string, name of the table.",
                     ),
                 }
             ),
             "text": Permissive(
                 {
                     "path": Field(
                         Any,
@@ -951,133 +975,14 @@
         return spark_read.load(**file_options)
     else:
         raise DagsterInvariantViolationError(
             "Unsupported file_type {file_type}".format(file_type=file_type)
         )
 
 
-class SparkDataFrameS3StoragePlugin(TypeStoragePlugin):  # pylint: disable=no-init
-    @classmethod
-    def compatible_with_storage_def(cls, system_storage_def):
-        return system_storage_def.required_resource_keys == {"s3"}
-
-    @classmethod
-    def set_intermediate_object(
-        cls, intermediate_storage, context, _dagster_type, step_output_handle, value
-    ):
-        paths = ["intermediates", step_output_handle.step_key, step_output_handle.output_name]
-        target_path = intermediate_storage.object_store.key_for_paths(paths)
-        value.write.parquet(
-            intermediate_storage.uri_for_paths(paths, protocol=cls.protocol(context))
-        )
-        return target_path
-
-    @classmethod
-    def get_intermediate_object(
-        cls, intermediate_storage, context, _dagster_type, step_output_handle
-    ):
-        paths = ["intermediates", step_output_handle.step_key, step_output_handle.output_name]
-        return context.resources.pyspark.spark_session.read.parquet(
-            intermediate_storage.uri_for_paths(paths, protocol=cls.protocol(context))
-        )
-
-    @classmethod
-    def required_resource_keys(cls):
-        return frozenset({"pyspark"})
-
-    @staticmethod
-    def protocol(context):
-        # pylint: disable=protected-access
-        hadoopConf = context.resources.pyspark.spark_session.sparkContext._jsc.hadoopConfiguration()
-        # If we're on EMR, s3 is preferred:
-        # https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-plan-file-systems.html
-        # Otherwise, s3a is preferred
-        if hadoopConf.get("fs.s3.impl") == "com.amazon.ws.emr.hadoop.fs.EmrFileSystem":
-            return "s3://"
-        else:
-            return "s3a://"
-
-
-class SparkDataFrameADLS2StoragePlugin(TypeStoragePlugin):  # pylint: disable=no-init
-    @classmethod
-    def compatible_with_storage_def(cls, system_storage_def):
-        try:
-            from dagster_azure.adls2 import adls2_system_storage, adls2_intermediate_storage
-
-            return (
-                system_storage_def is adls2_system_storage
-                or system_storage_def is adls2_intermediate_storage
-            )
-        except ImportError:
-            return False
-
-    @classmethod
-    def set_intermediate_object(
-        cls, intermediate_storage, context, _dagster_type, step_output_handle, value
-    ):
-        paths = ["intermediates", step_output_handle.step_key, step_output_handle.output_name]
-        target_path = intermediate_storage.object_store.key_for_paths(paths)
-        value.write.parquet(
-            intermediate_storage.uri_for_paths(paths, protocol=cls.protocol(context))
-        )
-        return target_path
-
-    @classmethod
-    def get_intermediate_object(
-        cls, intermediate_storage, context, _dagster_type, step_output_handle
-    ):
-        paths = ["intermediates", step_output_handle.step_key, step_output_handle.output_name]
-        return context.resources.pyspark.spark_session.read.parquet(
-            intermediate_storage.uri_for_paths(paths, protocol=cls.protocol(context))
-        )
-
-    @classmethod
-    def required_resource_keys(cls):
-        return frozenset({"pyspark"})
-
-    @staticmethod
-    def protocol(_context):
-        return "abfss://"
-
-
-class SparkDataFrameFilesystemStoragePlugin(TypeStoragePlugin):  # pylint: disable=no-init
-    @classmethod
-    def compatible_with_storage_def(cls, system_storage_def):
-        return (
-            system_storage_def is fs_system_storage or system_storage_def is fs_intermediate_storage
-        )
-
-    @classmethod
-    def set_intermediate_object(
-        cls, intermediate_storage, _context, _dagster_type, step_output_handle, value
-    ):
-        paths = ["intermediates", step_output_handle.step_key, step_output_handle.output_name]
-        target_path = os.path.join(intermediate_storage.root, *paths)
-        value.write.parquet(intermediate_storage.uri_for_paths(paths))
-        return target_path
-
-    @classmethod
-    def get_intermediate_object(
-        cls, intermediate_storage, context, _dagster_type, step_output_handle
-    ):
-        paths = ["intermediates", step_output_handle.step_key, step_output_handle.output_name]
-        return context.resources.pyspark.spark_session.read.parquet(
-            os.path.join(intermediate_storage.root, *paths)
-        )
-
-    @classmethod
-    def required_resource_keys(cls):
-        return frozenset({"pyspark"})
-
-
 DataFrame = PythonObjectDagsterType(
     python_type=NativeSparkDataFrame,
     name="PySparkDataFrame",
     description="A PySpark data frame.",
-    auto_plugins=[
-        SparkDataFrameS3StoragePlugin,
-        SparkDataFrameADLS2StoragePlugin,
-        SparkDataFrameFilesystemStoragePlugin,
-    ],
     loader=dataframe_loader,
     materializer=dataframe_materializer,
 )
```

### Comparing `dagster-pyspark-0.9.9rc1/dagster_pyspark/utils.py` & `dagster-pyspark-1.0.5/dagster_pyspark/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import zipfile
 
-from dagster import check
+import dagster._check as check
 
 
 def build_pyspark_zip(zip_file, path):
-    """Archives the current path into a file named `zip_file`
-    """
+    """Archives the current path into a file named `zip_file`"""
     check.str_param(zip_file, "zip_file")
     check.str_param(path, "path")
 
     with zipfile.ZipFile(zip_file, "w", zipfile.ZIP_DEFLATED) as zf:
         for root, _, files in os.walk(path):
             for fname in files:
                 abs_fname = os.path.join(root, fname)
```

### Comparing `dagster-pyspark-0.9.9rc1/dagster_pyspark.egg-info/PKG-INFO` & `dagster-pyspark-1.0.5/dagster_pyspark.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-pyspark
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: Package for PySpark Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-framework/pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-pyspark-0.9.9rc1/setup.py` & `dagster-pyspark-1.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,43 @@
+from typing import Dict
+
 from setuptools import find_packages, setup
 
 
-def get_version():
-    version = {}
-    with open("dagster_pyspark/version.py") as fp:
+def get_version() -> str:
+    version: Dict[str, str] = {}
+    with open("dagster_pyspark/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
 if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
     setup(
         name="dagster-pyspark",
-        version=get_version(),
+        version=ver,
         author="Elementl",
         author_email="hello@elementl.com",
         license="Apache-2.0",
         description="Package for PySpark Dagster framework components.",
         url="https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-framework/pyspark",
         classifiers=[
-            "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: OS Independent",
         ],
-        packages=find_packages(exclude=["test"]),
+        packages=find_packages(exclude=["dagster_pyspark_tests*"]),
         install_requires=[
-            "dagster",
-            "dagster_spark",
+            "dagster==1.0.5",
+            "dagster_spark==1.0.5",
             # Pyspark 2.x is incompatible with Python 3.8+
             'pyspark>=3.0.0; python_version >= "3.8"',
             'pyspark>=2.0.2; python_version < "3.8"',
         ],
         zip_safe=False,
     )
```

