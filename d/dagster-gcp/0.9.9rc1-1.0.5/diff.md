# Comparing `tmp/dagster-gcp-0.9.9rc1.tar.gz` & `tmp/dagster-gcp-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-gcp-0.9.9rc1.tar", last modified: Thu Sep 17 21:07:28 2020, max compression
+gzip compressed data, was "dagster-gcp-1.0.5.tar", last modified: Fri Aug 26 13:44:40 2022, max compression
```

## Comparing `dagster-gcp-0.9.9rc1.tar` & `dagster-gcp-1.0.5.tar`

### file list

```diff
@@ -1,57 +1,43 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       16 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      632 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      119 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp/
--rw-r--r--   0 bobchen    (501) staff       (20)      877 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp/bigquery/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/bigquery/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    14635 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/bigquery/configs.py
--rw-r--r--   0 bobchen    (501) staff       (20)      304 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/bigquery/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)     6066 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/bigquery/solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4405 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/bigquery/types.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1280 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/configs.py
--rw-r--r--   0 bobchen    (501) staff       (20)    42391 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/configs_dataproc_cluster.py
--rw-r--r--   0 bobchen    (501) staff       (20)    30599 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/configs_dataproc_job.py
--rw-r--r--   0 bobchen    (501) staff       (20)     5167 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1537 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)       41 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/types.py
--rw-r--r--   0 bobchen    (501) staff       (20)      692 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/types_dataproc_cluster.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1735 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/types_dataproc_job.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp/gcs/
--rw-r--r--   0 bobchen    (501) staff       (20)      170 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/gcs/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3367 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/gcs/file_manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1270 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/gcs/intermediate_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4495 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/gcs/object_store.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1244 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/gcs/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2563 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/gcs/system_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      632 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)     1587 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)      165 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       30 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/bigquery_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/bigquery_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    11092 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/bigquery_tests/test_solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1972 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/bigquery_tests/test_types.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/dataproc_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/dataproc_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4826 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/dataproc_tests/test_resources.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/gcs_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/gcs_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      103 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/gcs_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2506 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/gcs_tests/test_gcs_file_manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)    16628 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/gcs_tests/test_intermediate_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)      961 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/gcs_tests/test_object_store.py
--rw-r--r--   0 bobchen    (501) staff       (20)      566 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/gcs_tests/test_resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       89 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1431 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:40.212195 dagster-gcp-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       45 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      688 2022-08-26 13:44:40.212195 dagster-gcp-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      119 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:40.196194 dagster-gcp-1.0.5/dagster_gcp/
+-rw-r--r--   0 root         (0) root         (0)      892 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:40.204194 dagster-gcp-1.0.5/dagster_gcp/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14765 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/bigquery/configs.py
+-rw-r--r--   0 root         (0) root         (0)     5841 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/bigquery/ops.py
+-rw-r--r--   0 root         (0) root         (0)      320 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/bigquery/resources.py
+-rw-r--r--   0 root         (0) root         (0)      123 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/bigquery/solids.py
+-rw-r--r--   0 root         (0) root         (0)     4402 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/bigquery/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:40.208194 dagster-gcp-1.0.5/dagster_gcp/dataproc/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/dataproc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1280 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/dataproc/configs.py
+-rw-r--r--   0 root         (0) root         (0)    42391 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/dataproc/configs_dataproc_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    30599 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/dataproc/configs_dataproc_job.py
+-rw-r--r--   0 root         (0) root         (0)     2286 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/dataproc/ops.py
+-rw-r--r--   0 root         (0) root         (0)     5202 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/dataproc/resources.py
+-rw-r--r--   0 root         (0) root         (0)      101 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/dataproc/solids.py
+-rw-r--r--   0 root         (0) root         (0)       41 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/dataproc/types.py
+-rw-r--r--   0 root         (0) root         (0)      692 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/dataproc/types_dataproc_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/dataproc/types_dataproc_job.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:40.212195 dagster-gcp-1.0.5/dagster_gcp/gcs/
+-rw-r--r--   0 root         (0) root         (0)      294 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/gcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7293 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/gcs/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     3864 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/gcs/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2889 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/gcs/gcs_fake_resource.py
+-rw-r--r--   0 root         (0) root         (0)     4887 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/gcs/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1415 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/gcs/resources.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/dagster_gcp/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:40.196194 dagster-gcp-1.0.5/dagster_gcp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      688 2022-08-26 13:44:40.000000 dagster-gcp-1.0.5/dagster_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1079 2022-08-26 13:44:40.000000 dagster-gcp-1.0.5/dagster_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:44:40.000000 dagster-gcp-1.0.5/dagster_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:44:40.000000 dagster-gcp-1.0.5/dagster_gcp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      154 2022-08-26 13:44:40.000000 dagster-gcp-1.0.5/dagster_gcp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-08-26 13:44:40.000000 dagster-gcp-1.0.5/dagster_gcp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2022-08-26 13:44:40.216194 dagster-gcp-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1744 2022-08-26 13:33:01.000000 dagster-gcp-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-gcp-0.9.9rc1/LICENSE` & `dagster-gcp-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9rc1/PKG-INFO` & `dagster-gcp-1.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: dagster-gcp
-Version: 0.9.9rc1
-Summary: Package for GCP-specific Dagster framework solid and resource components.
+Version: 1.0.5
+Summary: Package for GCP-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp
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
 Provides-Extra: pyarrow
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-gcp-0.9.9rc1/dagster_gcp/__init__.py` & `dagster-gcp-1.0.5/dagster_gcp/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-from dagster.core.utils import check_dagster_package_version
+from dagster._core.utils import check_dagster_package_version
 
-from .bigquery.resources import bigquery_resource
-from .bigquery.solids import (
+from .bigquery.ops import (
     bq_create_dataset,
     bq_delete_dataset,
-    bq_solid_for_queries,
+    bq_op_for_queries,
     import_df_to_bq,
     import_file_to_bq,
     import_gcs_paths_to_bq,
 )
+from .bigquery.resources import bigquery_resource
 from .bigquery.types import BigQueryError
+from .dataproc.ops import dataproc_op
 from .dataproc.resources import dataproc_resource
-from .dataproc.solids import dataproc_solid
-from .gcs import gcs_resource, gcs_system_storage
+from .gcs import GCSFileHandle, gcs_file_manager, gcs_resource
 from .version import __version__
 
 check_dagster_package_version("dagster-gcp", __version__)
 
 __all__ = [
     "BigQueryError",
+    "GCSFileHandle",
     "bigquery_resource",
     "bq_create_dataset",
     "bq_delete_dataset",
-    "bq_solid_for_queries",
+    "bq_op_for_queries",
     "dataproc_resource",
-    "dataproc_solid",
+    "dataproc_op",
     "gcs_resource",
-    "gcs_system_storage",
+    "gcs_file_manager",
     "import_df_to_bq",
     "import_file_to_bq",
     "import_gcs_paths_to_bq",
 ]
```

### Comparing `dagster-gcp-0.9.9rc1/dagster_gcp/bigquery/configs.py` & `dagster-gcp-1.0.5/dagster_gcp/bigquery/configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """BigQuery configuration.
 
 See the BigQuery Python API documentation for reference:
     https://googleapis.github.io/google-cloud-python/latest/bigquery/reference.html
 """
 
-from dagster import Bool, Field, IntSource, String, StringSource
+from dagster import Array, Bool, Field, IntSource, String, StringSource
 
 from .types import (
     BQCreateDisposition,
     BQEncoding,
     BQPriority,
     BQSchemaUpdateOption,
     BQSourceFormat,
@@ -34,16 +34,15 @@
         is_required=False,
     )
 
     return {"project": project, "location": location}
 
 
 def _define_shared_fields():
-    """The following fields are shared between both QueryJobConfig and LoadJobConfig.
-    """
+    """The following fields are shared between both QueryJobConfig and LoadJobConfig."""
 
     clustering_fields = Field(
         [String],
         description="""Fields defining clustering for the table
 
         (Defaults to None).
 
@@ -330,14 +329,18 @@
 
     quote_character = Field(
         StringSource,
         description="Character used to quote data sections (CSV only).",
         is_required=False,
     )
 
+    schema = Field(
+        Array(inner_type=dict), description="Schema of the destination table.", is_required=False
+    )
+
     skip_leading_rows = Field(
         IntSource,
         description="Number of rows to skip when reading data (CSV only).",
         is_required=False,
     )
 
     source_format = Field(BQSourceFormat, description="File format of the data.", is_required=False)
@@ -362,15 +365,15 @@
             "destination_table_friendly_name": destination_table_friendly_name,
             "encoding": encoding,
             "field_delimiter": field_delimiter,
             "ignore_unknown_values": ignore_unknown_values,
             "max_bad_records": max_bad_records,
             "null_marker": null_marker,
             "quote_character": quote_character,
-            # TODO: schema
+            "schema": schema,
             "schema_update_options": sf["schema_update_options"],
             "skip_leading_rows": skip_leading_rows,
             "source_format": source_format,
             "time_partitioning": sf["time_partitioning"],
             "use_avro_logical_types": use_avro_logical_types,
             "write_disposition": sf["write_disposition"],
         },
```

### Comparing `dagster-gcp-0.9.9rc1/dagster_gcp/bigquery/solids.py` & `dagster-gcp-1.0.5/dagster_gcp/bigquery/ops.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import hashlib
 
 from dagster_pandas import DataFrame
 from google.cloud.bigquery.job import LoadJobConfig, QueryJobConfig
 from google.cloud.bigquery.table import EncryptionConfiguration, TimePartitioning
 
-from dagster import InputDefinition, List, Nothing, OutputDefinition, check, solid
+from dagster import In, List, Nothing, Out
+from dagster import _check as check
+from dagster import op
 
 from .configs import (
     define_bigquery_create_dataset_config,
     define_bigquery_delete_dataset_config,
     define_bigquery_load_config,
     define_bigquery_query_config,
 )
@@ -28,38 +30,38 @@
 
     if time_partitioning is not None:
         cfg["time_partitioning"] = TimePartitioning(**time_partitioning)
 
     return cfg
 
 
-def bq_solid_for_queries(sql_queries):
+def bq_op_for_queries(sql_queries):
     """
     Executes BigQuery SQL queries.
 
     Expects a BQ client to be provisioned in resources as context.resources.bigquery.
     """
 
     sql_queries = check.list_param(sql_queries, "sql queries", of_type=str)
-
     m = hashlib.sha1()
     for query in sql_queries:
-        m.update(query.encode())
-    name = "bq_solid_{hash}".format(hash=m.hexdigest()[:10])
+        m.update(query.encode("utf-8"))
+    hash_str = m.hexdigest()[:10]
+    name = f"bq_op_{hash_str}"
 
-    @solid(
+    @op(
         name=name,
-        input_defs=[InputDefinition(_START, Nothing)],
-        output_defs=[OutputDefinition(List[DataFrame])],
+        ins={_START: In(Nothing)},
+        out=Out(List[DataFrame]),
         config_schema=define_bigquery_query_config(),
         required_resource_keys={"bigquery"},
         tags={"kind": "sql", "sql": "\n".join(sql_queries)},
     )
-    def _solid(context):  # pylint: disable=unused-argument
-        query_job_config = _preprocess_config(context.solid_config.get("query_job_config", {}))
+    def _bq_fn(context):  # pylint: disable=unused-argument
+        query_job_config = _preprocess_config(context.op_config.get("query_job_config", {}))
 
         # Retrieve results as pandas DataFrames
         results = []
         for sql_query in sql_queries:
             # We need to construct a new QueryJobConfig for each query.
             # See: https://bit.ly/2VjD6sl
             cfg = QueryJobConfig(**query_job_config) if query_job_config else None
@@ -69,53 +71,53 @@
             )
             results.append(
                 context.resources.bigquery.query(sql_query, job_config=cfg).to_dataframe()
             )
 
         return results
 
-    return _solid
+    return _bq_fn
 
 
 BIGQUERY_LOAD_CONFIG = define_bigquery_load_config()
 
 
-@solid(
-    input_defs=[InputDefinition("paths", List[str])],
-    output_defs=[OutputDefinition(Nothing)],
+@op(
+    ins={"paths": In(List[str])},
+    out=Out(Nothing),
     config_schema=BIGQUERY_LOAD_CONFIG,
     required_resource_keys={"bigquery"},
 )
 def import_gcs_paths_to_bq(context, paths):
     return _execute_load_in_source(context, paths, BigQueryLoadSource.GCS)
 
 
-@solid(
-    input_defs=[InputDefinition("df", DataFrame)],
-    output_defs=[OutputDefinition(Nothing)],
+@op(
+    ins={"df": In(DataFrame)},
+    out=Out(Nothing),
     config_schema=BIGQUERY_LOAD_CONFIG,
     required_resource_keys={"bigquery"},
 )
 def import_df_to_bq(context, df):
     return _execute_load_in_source(context, df, BigQueryLoadSource.DataFrame)
 
 
-@solid(
-    input_defs=[InputDefinition("path", str)],
-    output_defs=[OutputDefinition(Nothing)],
+@op(
+    ins={"path": In(str)},
+    out=Out(Nothing),
     config_schema=BIGQUERY_LOAD_CONFIG,
     required_resource_keys={"bigquery"},
 )
 def import_file_to_bq(context, path):
     return _execute_load_in_source(context, path, BigQueryLoadSource.File)
 
 
 def _execute_load_in_source(context, source, source_name):
-    destination = context.solid_config.get("destination")
-    load_job_config = _preprocess_config(context.solid_config.get("load_job_config", {}))
+    destination = context.op_config.get("destination")
+    load_job_config = _preprocess_config(context.op_config.get("load_job_config", {}))
     cfg = LoadJobConfig(**load_job_config) if load_job_config else None
 
     context.log.info(
         "executing BQ load with config: %s for source %s"
         % (cfg.to_api_repr() if cfg else "(no config provided)", source)
     )
 
@@ -132,46 +134,46 @@
             ).result()
 
     # Load from GCS. See: https://cloud.google.com/bigquery/docs/loading-data-cloud-storage
     elif source_name == BigQueryLoadSource.GCS:
         context.resources.bigquery.load_table_from_uri(source, destination, job_config=cfg).result()
 
 
-@solid(
-    input_defs=[InputDefinition(_START, Nothing)],
+@op(
+    ins={_START: In(Nothing)},
     config_schema=define_bigquery_create_dataset_config(),
     required_resource_keys={"bigquery"},
 )
 def bq_create_dataset(context):
     """BigQuery Create Dataset.
 
-    This solid encapsulates creating a BigQuery dataset.
+    This op encapsulates creating a BigQuery dataset.
 
     Expects a BQ client to be provisioned in resources as context.resources.bigquery.
     """
-    (dataset, exists_ok) = [context.solid_config.get(k) for k in ("dataset", "exists_ok")]
+    (dataset, exists_ok) = [context.op_config.get(k) for k in ("dataset", "exists_ok")]
     context.log.info("executing BQ create_dataset for dataset %s" % (dataset))
     context.resources.bigquery.create_dataset(dataset, exists_ok)
 
 
-@solid(
-    input_defs=[InputDefinition(_START, Nothing)],
+@op(
+    ins={_START: In(Nothing)},
     config_schema=define_bigquery_delete_dataset_config(),
     required_resource_keys={"bigquery"},
 )
 def bq_delete_dataset(context):
     """BigQuery Delete Dataset.
 
-    This solid encapsulates deleting a BigQuery dataset.
+    This op encapsulates deleting a BigQuery dataset.
 
     Expects a BQ client to be provisioned in resources as context.resources.bigquery.
     """
 
     (dataset, delete_contents, not_found_ok) = [
-        context.solid_config.get(k) for k in ("dataset", "delete_contents", "not_found_ok")
+        context.op_config.get(k) for k in ("dataset", "delete_contents", "not_found_ok")
     ]
 
     context.log.info("executing BQ delete_dataset for dataset %s" % dataset)
 
     context.resources.bigquery.delete_dataset(
         dataset, delete_contents=delete_contents, not_found_ok=not_found_ok
     )
```

### Comparing `dagster-gcp-0.9.9rc1/dagster_gcp/bigquery/types.py` & `dagster-gcp-1.0.5/dagster_gcp/bigquery/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     QueryPriority,
     SchemaUpdateOption,
     SourceFormat,
     WriteDisposition,
 )
 
 from dagster import Enum, EnumValue
-from dagster.config import ConfigScalar, ConfigScalarKind, PostProcessingError
+from dagster._config import ConfigScalar, ConfigScalarKind, PostProcessingError
 
 
 class BigQueryLoadSource(PyEnum):
     DataFrame = "DATA_FRAME"
     GCS = "GCS"
     File = "FILE"
 
@@ -81,16 +81,15 @@
 RE_DS_TABLE = r"[\w\d\_]{1,1024}"
 
 # BigQuery supports writes directly to date partitions with the syntax foo.bar$20190101
 RE_PARTITION_SUFFIX = r"(\$\d{8})?"
 
 
 def _is_valid_dataset(config_value):
-    """Datasets must be of form "project.dataset" or "dataset"
-    """
+    """Datasets must be of form "project.dataset" or "dataset" """
     return re.match(
         # regex matches: project.dataset -- OR -- dataset
         r"^" + RE_PROJECT + r"\." + RE_DS_TABLE + r"$|^" + RE_DS_TABLE + r"$",
         config_value,
     )
```

### Comparing `dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/configs.py` & `dagster-gcp-1.0.5/dagster_gcp/dataproc/configs.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/configs_dataproc_cluster.py` & `dagster-gcp-1.0.5/dagster_gcp/dataproc/configs_dataproc_cluster.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/configs_dataproc_job.py` & `dagster-gcp-1.0.5/dagster_gcp/dataproc/configs_dataproc_job.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/resources.py` & `dagster-gcp-1.0.5/dagster_gcp/dataproc/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .configs import define_dataproc_create_cluster_config
 from .types import DataprocError
 
 TWENTY_MINUTES = 20 * 60
 DEFAULT_ITER_TIME_SEC = 5
 
 
-class DataprocResource(object):
+class DataprocResource:
     """Builds a client to the dataproc API."""
 
     def __init__(self, config):
         # Use Application Default Credentials to check the
         # GOOGLE_APPLICATION_CREDENTIALS environment variable
         # for the location of the service account key file.
         credentials = GoogleCredentials.get_application_default()
@@ -94,42 +94,40 @@
         ).execute()
 
     def get_job(self, job_id):
         return self.dataproc_jobs.get(
             projectId=self.project_id, region=self.region, jobId=job_id
         ).execute()
 
-    def wait_for_job(self, job_id):
-        """This method polls job status every 5 seconds
-        """
+    def wait_for_job(self, job_id, wait_timeout=TWENTY_MINUTES):
+        """This method polls job status every 5 seconds"""
         # TODO: Add logging here print('Waiting for job ID {} to finish...'.format(job_id))
         def iter_fn():
             # See: https://bit.ly/2Lg2tHr
             result = self.get_job(job_id)
 
             # Handle exceptions
             if result["status"]["state"] in {"CANCELLED", "ERROR"}:
                 raise DataprocError("Job error: %s" % str(result["status"]))
 
             if result["status"]["state"] == "DONE":
                 return True
 
             return False
 
-        done = DataprocResource._iter_and_sleep_until_ready(iter_fn)
+        done = DataprocResource._iter_and_sleep_until_ready(iter_fn, max_wait_time_sec=wait_timeout)
         if not done:
             job = self.get_job(job_id)
             raise DataprocError("Job run timed out: %s" % str(job["status"]))
 
     @staticmethod
     def _iter_and_sleep_until_ready(
         callable_fn, max_wait_time_sec=TWENTY_MINUTES, iter_time=DEFAULT_ITER_TIME_SEC
     ):
-        """Iterates and sleeps until callable_fn returns true
-        """
+        """Iterates and sleeps until callable_fn returns true"""
         # Wait for cluster ready state
         ready, curr_iter = False, 0
         max_iter = max_wait_time_sec / iter_time
         while not ready and curr_iter < max_iter:
             ready = callable_fn()
             time.sleep(iter_time)
             curr_iter += 1
```

### Comparing `dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/solids.py` & `dagster-gcp-1.0.5/dagster_gcp/dataproc/ops.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,62 @@
-from dagster import Bool, Field, solid
-from dagster.seven import json
+from dagster import Bool, Field, Int, op
+from dagster._seven import json
 
 from .configs import define_dataproc_submit_job_config
+from .resources import TWENTY_MINUTES
 
+DATAPROC_CONFIG_SCHEMA = {
+    "job_timeout_in_seconds": Field(
+        Int,
+        description="""Optional. Maximum time in seconds to wait for the job being
+                    completed. Default is set to 1200 seconds (20 minutes).
+                    """,
+        is_required=False,
+        default_value=TWENTY_MINUTES,
+    ),
+    "job_config": define_dataproc_submit_job_config(),
+    "job_scoped_cluster": Field(
+        Bool,
+        description="whether to create a cluster or use an existing cluster",
+        is_required=False,
+        default_value=True,
+    ),
+}
 
-@solid(
-    required_resource_keys={"dataproc"},
-    config_schema={
-        "job_config": define_dataproc_submit_job_config(),
-        "job_scoped_cluster": Field(
-            Bool,
-            description="whether to create a cluster or use an existing cluster",
-            is_required=False,
-            default_value=True,
-        ),
-    },
-)
-def dataproc_solid(context):
+
+def _dataproc_compute(context):
     job_config = context.solid_config["job_config"]
+    job_timeout = context.solid_config["job_timeout_in_seconds"]
 
-    context.log.info("submitting job with config: %s" % str(json.dumps(job_config)))
+    context.log.info(
+        "submitting job with config: %s and timeout of: %d seconds"
+        % (str(json.dumps(job_config)), job_timeout)
+    )
 
     if context.solid_config["job_scoped_cluster"]:
         # Cluster context manager, creates and then deletes cluster
         with context.resources.dataproc.cluster_context_manager() as cluster:
             # Submit the job specified by this solid to the cluster defined by the associated resource
             result = cluster.submit_job(job_config)
 
             job_id = result["reference"]["jobId"]
             context.log.info("Submitted job ID {}".format(job_id))
-            cluster.wait_for_job(job_id)
+            cluster.wait_for_job(job_id, wait_timeout=job_timeout)
+
     else:
         # Submit to an existing cluster
         # Submit the job specified by this solid to the cluster defined by the associated resource
         result = context.resources.dataproc.submit_job(job_config)
 
         job_id = result["reference"]["jobId"]
         context.log.info("Submitted job ID {}".format(job_id))
-        context.resources.dataproc.wait_for_job(job_id)
+        context.resources.dataproc.wait_for_job(job_id, wait_timeout=job_timeout)
+
+
+@op(required_resource_keys={"dataproc"}, config_schema=DATAPROC_CONFIG_SCHEMA)
+def dataproc_solid(context):
+    return _dataproc_compute(context)
+
+
+@op(required_resource_keys={"dataproc"}, config_schema=DATAPROC_CONFIG_SCHEMA)
+def dataproc_op(context):
+    return _dataproc_compute(context)
```

### Comparing `dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/types_dataproc_cluster.py` & `dagster-gcp-1.0.5/dagster_gcp/dataproc/types_dataproc_cluster.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/types_dataproc_job.py` & `dagster-gcp-1.0.5/dagster_gcp/dataproc/types_dataproc_job.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9rc1/dagster_gcp/gcs/resources.py` & `dagster-gcp-1.0.5/dagster_gcp/gcs/resources.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from google.cloud import storage
+from google.cloud import storage  # type: ignore
 
 from dagster import Field, Noneable, StringSource, resource
-from dagster.utils.merger import merge_dicts
+from dagster._utils.merger import merge_dicts
 
 from .file_manager import GCSFileManager
 
 GCS_CLIENT_CONFIG = {
     "project": Field(Noneable(StringSource), is_required=False, description="Project name")
 }
 
 
 @resource(
-    GCS_CLIENT_CONFIG, description="This resource provides a GCS client",
+    GCS_CLIENT_CONFIG,
+    description="This resource provides a GCS client",
 )
 def gcs_resource(init_context):
     return _gcs_client_from_config(init_context.resource_config)
 
 
 @resource(
     merge_dicts(
@@ -23,14 +24,18 @@
         {
             "gcs_bucket": Field(StringSource),
             "gcs_prefix": Field(StringSource, is_required=False, default_value="dagster"),
         },
     )
 )
 def gcs_file_manager(context):
+    """FileManager that provides abstract access to GCS.
+
+    Implements the :py:class:`~dagster._core.storage.file_manager.FileManager` API.
+    """
     gcs_client = _gcs_client_from_config(context.resource_config)
     return GCSFileManager(
         client=gcs_client,
         gcs_bucket=context.resource_config["gcs_bucket"],
         gcs_base_key=context.resource_config["gcs_prefix"],
     )
```

### Comparing `dagster-gcp-0.9.9rc1/dagster_gcp.egg-info/PKG-INFO` & `dagster-gcp-1.0.5/dagster_gcp.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: dagster-gcp
-Version: 0.9.9rc1
-Summary: Package for GCP-specific Dagster framework solid and resource components.
+Version: 1.0.5
+Summary: Package for GCP-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp
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
 Provides-Extra: pyarrow
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-gcp-0.9.9rc1/setup.py` & `dagster-gcp-1.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,47 @@
+from typing import Dict
+
 from setuptools import find_packages, setup
 
 
-def get_version():
-    version = {}
-    with open("dagster_gcp/version.py") as fp:
+def get_version() -> str:
+    version: Dict[str, str] = {}
+    with open("dagster_gcp/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
 if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
     setup(
         name="dagster-gcp",
-        version=get_version(),
+        version=ver,
         author="Elementl",
         author_email="hello@elementl.com",
         license="Apache-2.0",
-        description="Package for GCP-specific Dagster framework solid and resource components.",
+        description="Package for GCP-specific Dagster framework op and resource components.",
         # pylint: disable=line-too-long
         url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp",
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
+        packages=find_packages(exclude=["dagster_gcp_tests*"]),
         install_requires=[
-            "dagster",
-            "dagster_pandas",
-            "google-api-python-client",
-            "google-cloud-bigquery>=1.19.*",
+            "dagster==1.0.5",
+            "dagster_pandas==1.0.5",
+            "google-api-python-client<2.0.0",
+            "google-cloud-bigquery>=1.19.*,<3",  # 3.0.0b1 gives ModuleNotFoundError: No module named 'db_dtypes'
             "google-cloud-storage",
             "oauth2client",
-            # RSA 4.1+ is incompatible with py2.7
-            'rsa<=4.0; python_version<"3"',
         ],
+        # we need `pyarrow` for testing read/write parquet files.
         extras_require={"pyarrow": ["pyarrow"]},
         zip_safe=False,
     )
```

