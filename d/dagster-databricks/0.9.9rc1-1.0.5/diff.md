# Comparing `tmp/dagster-databricks-0.9.9rc1.tar.gz` & `tmp/dagster-databricks-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-databricks-0.9.9rc1.tar", last modified: Thu Sep 17 21:07:32 2020, max compression
+gzip compressed data, was "dagster-databricks-1.0.5.tar", last modified: Fri Aug 26 13:45:37 2022, max compression
```

## Comparing `dagster-databricks-0.9.9rc1.tar` & `dagster-databricks-1.0.5.tar`

### file list

```diff
@@ -1,30 +1,25 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)      193 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      629 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      140 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/dagster_databricks/
--rw-r--r--   0 bobchen    (501) staff       (20)     1264 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    24423 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks/configs.py
--rw-r--r--   0 bobchen    (501) staff       (20)    11098 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks/databricks.py
--rw-r--r--   0 bobchen    (501) staff       (20)    14184 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks/databricks_pyspark_step_launcher.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2241 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks/databricks_step_main.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1012 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3238 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks/solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1332 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks/types.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/dagster_databricks.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      629 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/dagster_databricks.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      808 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/dagster_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/dagster_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/dagster_databricks.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       39 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/dagster_databricks.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       44 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/dagster_databricks.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/dagster_databricks_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      293 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4200 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks_tests/test_databricks.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7543 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks_tests/test_pyspark.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3171 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks_tests/test_solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1146 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:37.764510 dagster-databricks-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-databricks-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      229 2022-08-26 13:33:01.000000 dagster-databricks-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      688 2022-08-26 13:45:37.764510 dagster-databricks-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      140 2022-08-26 13:33:01.000000 dagster-databricks-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:37.760510 dagster-databricks-1.0.5/dagster_databricks/
+-rw-r--r--   0 root         (0) root         (0)     1257 2022-08-26 13:33:01.000000 dagster-databricks-1.0.5/dagster_databricks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29827 2022-08-26 13:33:01.000000 dagster-databricks-1.0.5/dagster_databricks/configs.py
+-rw-r--r--   0 root         (0) root         (0)    11339 2022-08-26 13:33:01.000000 dagster-databricks-1.0.5/dagster_databricks/databricks.py
+-rw-r--r--   0 root         (0) root         (0)    25286 2022-08-26 13:33:01.000000 dagster-databricks-1.0.5/dagster_databricks/databricks_pyspark_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     5633 2022-08-26 13:33:01.000000 dagster-databricks-1.0.5/dagster_databricks/databricks_step_main.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-databricks-1.0.5/dagster_databricks/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1058 2022-08-26 13:33:01.000000 dagster-databricks-1.0.5/dagster_databricks/resources.py
+-rw-r--r--   0 root         (0) root         (0)     4399 2022-08-26 13:33:01.000000 dagster-databricks-1.0.5/dagster_databricks/solids.py
+-rw-r--r--   0 root         (0) root         (0)     1332 2022-08-26 13:33:01.000000 dagster-databricks-1.0.5/dagster_databricks/types.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-databricks-1.0.5/dagster_databricks/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:37.764510 dagster-databricks-1.0.5/dagster_databricks.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      688 2022-08-26 13:45:37.000000 dagster-databricks-1.0.5/dagster_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      637 2022-08-26 13:45:37.000000 dagster-databricks-1.0.5/dagster_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:37.000000 dagster-databricks-1.0.5/dagster_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:37.000000 dagster-databricks-1.0.5/dagster_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       53 2022-08-26 13:45:37.000000 dagster-databricks-1.0.5/dagster_databricks.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2022-08-26 13:45:37.000000 dagster-databricks-1.0.5/dagster_databricks.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      165 2022-08-26 13:45:37.764510 dagster-databricks-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1469 2022-08-26 13:33:01.000000 dagster-databricks-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-databricks-0.9.9rc1/LICENSE` & `dagster-databricks-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-databricks-0.9.9rc1/dagster_databricks/__init__.py` & `dagster-databricks-1.0.5/dagster_databricks/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """Databricks integration for Dagster.
 
 This package provides:
 
 - the :py:class:`~dagster_databricks.databricks_pyspark_step_launcher` resource, which
-    launches a Databricks job in which a solid can be run
+    launches a Databricks job in which an op can be run
 - the :py:class:`~dagster_databricks.DatabricksRunJobSolidDefinition`, which can be used
     to execute an arbitrary task in Databricks.
 """
 
-from dagster.core.utils import check_dagster_package_version
+from dagster._core.utils import check_dagster_package_version
 
 from .databricks import DatabricksError, DatabricksJobRunner
 from .databricks_pyspark_step_launcher import (
     DatabricksConfig,
     DatabricksPySparkStepLauncher,
     databricks_pyspark_step_launcher,
 )
 from .resources import databricks_client
-from .solids import create_databricks_job_solid
+from .solids import create_databricks_job_op
 from .types import (
     DATABRICKS_RUN_TERMINATED_STATES,
     DatabricksRunLifeCycleState,
     DatabricksRunResultState,
 )
 from .version import __version__
 
 check_dagster_package_version("dagster-databricks", __version__)
 
 __all__ = [
-    "create_databricks_job_solid",
+    "create_databricks_job_op",
     "databricks_client",
     "DatabricksConfig",
     "DatabricksError",
     "DatabricksJobRunner",
     "DatabricksPySparkStepLauncher",
     "databricks_pyspark_step_launcher",
     "DATABRICKS_RUN_TERMINATED_STATES",
```

### Comparing `dagster-databricks-0.9.9rc1/dagster_databricks/configs.py` & `dagster-databricks-1.0.5/dagster_databricks/configs.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 the requirements.
 
 See:
 - https://docs.databricks.com/dev-tools/api/latest/jobs.html
 - https://docs.databricks.com/dev-tools/api/latest/clusters.html
 - https://docs.databricks.com/dev-tools/api/latest/libraries.html
 """
-from dagster import Bool, Field, Int, Permissive, Selector, Shape, String
+from dagster import Array, Bool, Enum, EnumValue, Field, Int, Permissive, Selector, Shape, String
 
 
 def _define_autoscale():
     return Field(
         Shape(
             fields={
                 "min_workers": Field(
@@ -134,14 +134,91 @@
                 "canned_acl": canned_acl,
             }
         ),
         description="S3 storage information",
     )
 
 
+def _define_aws_attributes_conf():
+    return Field(
+        Permissive(
+            fields={
+                "first_on_demand": Field(
+                    Int,
+                    description="The first first_on_demand nodes of the cluster will be placed on on-demand instances. "
+                    "If this value is greater than 0, the cluster driver node will be placed on an on-demand instance. "
+                    "If this value is greater than or equal to the current cluster size, all nodes will be placed on on-demand instances. "
+                    "If this value is less than the current cluster size, first_on_demand nodes will be placed on on-demand instances and "
+                    "the remainder will be placed on availability instances. This value does not affect cluster size and cannot be mutated "
+                    "over the lifetime of a cluster.",
+                    is_required=False,
+                ),
+                "availability": Field(
+                    Enum(
+                        "AWSAvailability",
+                        [
+                            EnumValue("SPOT"),
+                            EnumValue("ON_DEMAND"),
+                            EnumValue("SPOT_WITH_FALLBACK"),
+                        ],
+                    ),
+                    description="Availability type used for all subsequent nodes past the first_on_demand ones. "
+                    "Note: If first_on_demand is zero, this availability type will be used for the entire cluster.",
+                    is_required=False,
+                ),
+                "zone_id": Field(
+                    String,
+                    description="Identifier for the availability zone/datacenter in which the cluster resides.",
+                    is_required=False,
+                ),
+                "instance_profile_arn": Field(
+                    String,
+                    description="Nodes for this cluster will only be placed on AWS instances with this instance profile.",
+                    is_required=False,
+                ),
+                "spot_bid_price_percent": Field(
+                    Int,
+                    description="The max price for AWS spot instances, as a percentage of the corresponding instance type's on-demand price.",
+                    is_required=False,
+                ),
+                "ebs_volume_type": Field(
+                    Enum(
+                        "EBSVolumeType",
+                        [EnumValue("GENERAL_PURPOSE_SSD"), EnumValue("THROUGHPUT_OPTIMIZED_HDD")],
+                    ),
+                    description="The type of EBS volumes that will be launched with this cluster.",
+                    is_required=False,
+                ),
+                "ebs_volume_count": Field(
+                    Int,
+                    description="The number of volumes launched for each instance. You can choose up to 10 volumes.",
+                    is_required=False,
+                ),
+                "ebs_volume_size": Field(
+                    Int,
+                    description="The size of each EBS volume (in GiB) launched for each instance.",
+                    is_required=False,
+                ),
+                "ebs_volume_iops": Field(
+                    Int, description="The number of IOPS per EBS gp3 volume.", is_required=False
+                ),
+                "ebs_volume_throughput": Field(
+                    Int,
+                    description="The throughput per EBS gp3 volume, in MiB per second.",
+                    is_required=False,
+                ),
+            }
+        ),
+        description="Attributes related to clusters running on Amazon Web Services. "
+        "If not specified at cluster creation, a set of default values is used. "
+        "See aws_attributes at https://docs.databricks.com/dev-tools/api/latest/clusters.html.",
+        is_required=False,
+    )
+
+
 def _define_cluster_log_conf():
     return Field(
         Selector({"dbfs": _define_dbfs_storage_info(), "s3": _define_s3_storage_info()}),
         description="Recommended! The configuration for delivering Spark logs to a long-term "
         "storage destination. Only one destination can be specified for one cluster. If the conf "
         "is given, the logs will be delivered to the destination every 5 mins. "
         "The destination of driver logs is <destination>/<cluster-id>/driver, while the "
@@ -260,14 +337,15 @@
     return Field(
         Shape(
             fields={
                 "size": _define_size(),
                 "spark_version": spark_version,
                 "spark_conf": spark_conf,
                 "nodes": _define_nodes(),
+                "aws_attributes": _define_aws_attributes_conf(),
                 "ssh_public_keys": ssh_public_keys,
                 "custom_tags": _define_custom_tags(),
                 "cluster_log_conf": _define_cluster_log_conf(),
                 "init_scripts": init_scripts,
                 "spark_env_vars": spark_env_vars,
                 "enable_elastic_disk": enable_elastic_disk,
             }
@@ -483,15 +561,17 @@
         default_value=[],
     )
     return Field(Shape(fields={"python_file": python_file, "parameters": parameters}))
 
 
 def _define_spark_submit_task():
     parameters = Field(
-        [String], description="Command-line parameters passed to spark submit.", is_required=True,
+        [String],
+        description="Command-line parameters passed to spark submit.",
+        is_required=True,
     )
     return Field(
         Shape(fields={"parameters": parameters}),
         description="Important!"
         "You can Spark submit tasks only on new clusters. "
         "In the new_cluster specification, libraries and spark_conf are not supported. Instead, "
         "use --jars and --py-files to add Java and Python libraries and use --conf to set the "
@@ -524,15 +604,16 @@
     fields = _define_submit_run_fields()
     fields["task"] = _define_task()
     return Field(Shape(fields=fields), description="Databricks job run configuration")
 
 
 def define_databricks_submit_run_config():
     return Field(
-        Shape(fields=_define_submit_run_fields()), description="Databricks job run configuration",
+        Shape(fields=_define_submit_run_fields()),
+        description="Databricks job run configuration",
     )
 
 
 def _define_secret_scope():
     return Field(
         String,
         description="The Databricks secret scope containing the storage secrets.",
@@ -582,31 +663,34 @@
                 "storage_account_key_key": storage_account_key_key,
             }
         ),
         description="ADLS2 storage secret configuration",
     )
 
 
-def _define_storage_credentials():
-    return Selector(
-        {"s3": _define_s3_storage_credentials(), "adls2": _define_adls2_storage_credentials()},
-    )
-
-
 def define_databricks_storage_config():
     return Field(
         Selector(
-            {"s3": _define_s3_storage_credentials(), "adls2": _define_adls2_storage_credentials()}
+            {
+                "s3": _define_s3_storage_credentials(),
+                "adls2": _define_adls2_storage_credentials(),
+            }
         ),
-        description="Databricks storage configuration. Solids using the "
-        "DatabricksPySparkStepLauncher to execute pipeline steps in Databricks MUST configure "
-        "storage using this config (either S3 or ADLS2 can be used). Access credentials for the "
-        "storage must be stored in Databricks secrets; this config indicates the secret scope "
-        "and the secret keys used to access either S3 or ADLS2.",
-        is_required=True,
+        description="Databricks storage configuration for either S3 or ADLS2. If access credentials "
+        "for your Databricks storage are stored in Databricks secrets, this config indicates the "
+        "secret scope and the secret keys used to access either S3 or ADLS2.",
+        is_required=False,
+    )
+
+
+def define_databricks_env_variables():
+    return Field(
+        Permissive(),
+        description="Dictionary of arbitrary environment variables to be set on the databricks cluster.",
+        is_required=False,
     )
 
 
 def define_databricks_secrets_config():
     name = Field(
         String,
         description="The environment variable name, e.g. `DATABRICKS_TOKEN`.",
@@ -619,7 +703,53 @@
         description="Databricks secrets to be exported as environment variables. Since runs "
         "will execute in the Databricks runtime environment, environment variables (such as those "
         "required for a `StringSource` config variable) will not be accessible to Dagster. These "
         "variables must be stored as Databricks secrets and specified here, which will ensure "
         "they are re-exported as environment variables accessible to Dagster upon execution.",
         is_required=False,
     )
+
+
+def _define_accessor():
+    return Selector(
+        {"group_name": str, "user_name": str},
+        description="Group or User that shall access the target.",
+    )
+
+
+def _define_databricks_job_permission():
+    job_permission_levels = [
+        "NO_PERMISSIONS",
+        "CAN_VIEW",
+        "CAN_MANAGE_RUN",
+        "IS_OWNER",
+        "CAN_MANAGE",
+    ]
+    return Field(
+        {
+            permission_level: Field(Array(_define_accessor()), is_required=False)
+            for permission_level in job_permission_levels
+        },
+        description="job permission spec; ref: https://docs.databricks.com/security/access-control/jobs-acl.html#job-permissions",
+        is_required=False,
+    )
+
+
+def _define_databricks_cluster_permission():
+    cluster_permission_levels = ["NO_PERMISSIONS", "CAN_ATTACH_TO", "CAN_RESTART", "CAN_MANAGE"]
+    return Field(
+        {
+            permission_level: Field(Array(_define_accessor()), is_required=False)
+            for permission_level in cluster_permission_levels
+        },
+        description="cluster permission spec; ref: https://docs.databricks.com/security/access-control/cluster-acl.html#cluster-level-permissions",
+        is_required=False,
+    )
+
+
+def define_databricks_permissions():
+    return Field(
+        {
+            "job_permissions": _define_databricks_job_permission(),
+            "cluster_permissions": _define_databricks_cluster_permission(),
+        }
+    )
```

### Comparing `dagster-databricks-0.9.9rc1/dagster_databricks/databricks.py` & `dagster-databricks-1.0.5/dagster_databricks/databricks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import base64
 import time
 
 import requests.exceptions
 from databricks_api import DatabricksAPI
 
 import dagster
-from dagster import check
+import dagster._check as check
 
 from .types import (
     DATABRICKS_RUN_TERMINATED_STATES,
     DatabricksRunLifeCycleState,
     DatabricksRunResultState,
 )
 
 # wait at most 24 hours by default for run execution
-_DEFAULT_RUN_MAX_WAIT_TIME_SEC = 24 * 60 * 60
+DEFAULT_RUN_MAX_WAIT_TIME_SEC = 24 * 60 * 60
 
 
 class DatabricksError(Exception):
     pass
 
 
 class DatabricksClient:
@@ -29,32 +29,32 @@
         self.workspace_id = workspace_id
         self.client = DatabricksAPI(host=host, token=token)
 
     def submit_run(self, *args, **kwargs):
         """Submit a run directly to the 'Runs Submit' API."""
         return self.client.jobs.submit_run(*args, **kwargs)["run_id"]  # pylint: disable=no-member
 
-    def read_file(self, dbfs_path, block_size=1024 ** 2):
+    def read_file(self, dbfs_path, block_size=1024**2):
         """Read a file from DBFS to a **byte string**."""
-
         if dbfs_path.startswith("dbfs://"):
             dbfs_path = dbfs_path[7:]
         data = b""
         bytes_read = 0
         jdoc = self.client.dbfs.read(path=dbfs_path, length=block_size)  # pylint: disable=no-member
         data += base64.b64decode(jdoc["data"])
         while jdoc["bytes_read"] == block_size:
             bytes_read += jdoc["bytes_read"]
             jdoc = self.client.dbfs.read(  # pylint: disable=no-member
                 path=dbfs_path, offset=bytes_read, length=block_size
             )
             data += base64.b64decode(jdoc["data"])
+
         return data
 
-    def put_file(self, file_obj, dbfs_path, overwrite=False, block_size=1024 ** 2):
+    def put_file(self, file_obj, dbfs_path, overwrite=False, block_size=1024**2):
         """Upload an arbitrary large file to DBFS.
 
         This doesn't use the DBFS `Put` API because that endpoint is limited to 1MB.
         """
         if dbfs_path.startswith("dbfs://"):
             dbfs_path = dbfs_path[7:]
         create_response = self.client.dbfs.create(  # pylint: disable=no-member
@@ -66,21 +66,24 @@
         while block:
             data = base64.b64encode(block).decode("utf-8")
             self.client.dbfs.add_block(data=data, handle=handle)  # pylint: disable=no-member
             block = file_obj.read(block_size)
 
         self.client.dbfs.close(handle=handle)  # pylint: disable=no-member
 
+    def get_run(self, databricks_run_id):
+        return self.client.jobs.get_run(databricks_run_id)  # pylint: disable=no-member
+
     def get_run_state(self, databricks_run_id):
         """Get the state of a run by Databricks run ID (_not_ dagster run ID).
 
         Return a `DatabricksRunState` object. Note that the `result_state`
         attribute may be `None` if the run hasn't yet terminated.
         """
-        run = self.client.jobs.get_run(databricks_run_id)  # pylint: disable=no-member
+        run = self.get_run(databricks_run_id)
         state = run["state"]
         result_state = state.get("result_state")
         if result_state:
             result_state = DatabricksRunResultState(result_state)
         return DatabricksRunState(
             life_cycle_state=DatabricksRunLifeCycleState(state["life_cycle_state"]),
             result_state=result_state,
@@ -108,19 +111,19 @@
         return str(self.__dict__)
 
 
 class DatabricksJobRunner:
     """Submits jobs created using Dagster config to Databricks, and monitors their progress."""
 
     def __init__(
-        self, host, token, poll_interval_sec=10, max_wait_time_sec=_DEFAULT_RUN_MAX_WAIT_TIME_SEC
+        self, host, token, poll_interval_sec=5, max_wait_time_sec=DEFAULT_RUN_MAX_WAIT_TIME_SEC
     ):
         """Args:
-            host (str): Databricks host, e.g. https://uksouth.azuredatabricks.net
-            token (str): Databricks token
+        host (str): Databricks host, e.g. https://uksouth.azuredatabricks.net
+        token (str): Databricks token
         """
         self.host = check.str_param(host, "host")
         self.token = check.str_param(token, "token")
         self.poll_interval_sec = check.numeric_param(poll_interval_sec, "poll_interval_sec")
         self.max_wait_time_sec = check.int_param(max_wait_time_sec, "max_wait_time_sec")
 
         self._client = DatabricksClient(host=self.host, token=self.token)
@@ -166,16 +169,18 @@
             "Invalid value for run_config.cluster",
         )
 
         # We'll always need some libraries, namely dagster/dagster_databricks/dagster_pyspark,
         # since they're imported by our scripts.
         # Add them if they're not already added by users in config.
         libraries = list(run_config.get("libraries", []))
-        python_libraries = {x["pypi"]["package"].split("==")[0] for x in libraries if "pypi" in x}
-        for library in ["dagster", "dagster_databricks", "dagster_pyspark"]:
+        python_libraries = {
+            x["pypi"]["package"].split("==")[0].replace("_", "-") for x in libraries if "pypi" in x
+        }
+        for library in ["dagster", "dagster-databricks", "dagster-pyspark"]:
             if library not in python_libraries:
                 libraries.append(
                     {"pypi": {"package": "{}=={}".format(library, dagster.__version__)}}
                 )
 
         # Only one task should be able to be chosen really; make sure of that here.
         check.invariant(
@@ -193,15 +198,15 @@
         )
 
         config = dict(
             run_name=run_config.get("run_name"),
             new_cluster=new_cluster,
             existing_cluster_id=existing_cluster_id,
             libraries=libraries,
-            **task
+            **task,
         )
         return self.client.submit_run(**config)
 
     def retrieve_logs_for_run_id(self, log, databricks_run_id):
         """Retrieve the stdout and stderr logs for a run."""
         api_client = self.client.client
         run = api_client.jobs.get_run(databricks_run_id)  # pylint: disable=no-member
@@ -244,36 +249,47 @@
 
     def wait_for_run_to_complete(self, log, databricks_run_id):
         return wait_for_run_to_complete(
             self.client, log, databricks_run_id, self.poll_interval_sec, self.max_wait_time_sec
         )
 
 
+def poll_run_state(
+    client,
+    log,
+    start_poll_time: float,
+    databricks_run_id: int,
+    max_wait_time_sec: float,
+):
+    run_state = client.get_run_state(databricks_run_id)
+    if run_state.has_terminated():
+        if run_state.is_successful():
+            log.info("Run %s completed successfully" % databricks_run_id)
+            return True
+        else:
+            error_message = "Run %s failed with result state: %s. Message: %s" % (
+                databricks_run_id,
+                run_state.result_state,
+                run_state.state_message,
+            )
+            log.error(error_message)
+            raise DatabricksError(error_message)
+    else:
+        log.debug("Run %s in state %s" % (databricks_run_id, run_state))
+    if time.time() - start_poll_time > max_wait_time_sec:
+        raise DatabricksError(
+            "Job run {} took more than {}s to complete; failing".format(
+                databricks_run_id, max_wait_time_sec
+            )
+        )
+    return False
+
+
 def wait_for_run_to_complete(client, log, databricks_run_id, poll_interval_sec, max_wait_time_sec):
     """Wait for a Databricks run to complete."""
     check.int_param(databricks_run_id, "databricks_run_id")
     log.info("Waiting for Databricks run %s to complete..." % databricks_run_id)
     start = time.time()
     while True:
-        log.debug("Waiting %.1f seconds..." % poll_interval_sec)
+        if poll_run_state(client, log, start, databricks_run_id, max_wait_time_sec):
+            return
         time.sleep(poll_interval_sec)
-        run_state = client.get_run_state(databricks_run_id)
-        if run_state.has_terminated():
-            if run_state.is_successful():
-                log.info("Run %s completed successfully" % databricks_run_id)
-                return
-            else:
-                error_message = "Run %s failed with result state: %s. Message: %s" % (
-                    databricks_run_id,
-                    run_state.result_state,
-                    run_state.state_message,
-                )
-                log.error(error_message)
-                raise DatabricksError(error_message)
-        else:
-            log.info("Run %s in state %s" % (databricks_run_id, run_state))
-        if time.time() - start > max_wait_time_sec:
-            raise DatabricksError(
-                "Job run {} took more than {}s to complete; failing".format(
-                    databricks_run_id, max_wait_time_sec
-                )
-            )
```

### Comparing `dagster-databricks-0.9.9rc1/dagster_databricks/resources.py` & `dagster-databricks-1.0.5/dagster_databricks/resources.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 @resource(
     config_schema={
         "host": Field(
             StringSource,
             is_required=True,
             description="Databricks host, e.g. uksouth.azuredatabricks.com",
         ),
-        "token": Field(StringSource, is_required=True, description="Databricks access token",),
+        "token": Field(
+            StringSource,
+            is_required=True,
+            description="Databricks access token",
+        ),
         "workspace_id": Field(
             StringSource,
             description="The Databricks workspace ID, as described in"
             "https://docs.databricks.com/workspace/workspace-details.html#workspace-instance-names-urls-and-ids."
             "This is used to log a URL for accessing the job in the Databricks UI.",
             is_required=False,
         ),
```

### Comparing `dagster-databricks-0.9.9rc1/dagster_databricks/solids.py` & `dagster-databricks-1.0.5/dagster_databricks/solids.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,89 +1,128 @@
-from dagster import Field, InputDefinition, Nothing, OutputDefinition, Permissive, check, solid
+from dagster import Field, In, Nothing, Out, Permissive
+from dagster import _check as check
+from dagster import op
 
 from .databricks import wait_for_run_to_complete
 
 _START = "start"
 
 _DEFAULT_POLL_INTERVAL = 10
 # wait at most 24 hours by default for run execution
 _DEFAULT_RUN_MAX_WAIT_TIME_SEC = 24 * 60 * 60
 
 
-def create_databricks_job_solid(
+def create_databricks_job_op(
     name="databricks_job",
     num_inputs=1,
     description=None,
     required_resource_keys=frozenset(["databricks_client"]),
 ):
     """
-    Creates a solid that launches a databricks job.
+    Creates an op that launches a databricks job (not to be confused with Dagster's job API).
 
-    As config, the solid accepts a blob of the form described in Databricks' job API:
+    As config, the op accepts a blob of the form described in Databricks' job API:
     https://docs.databricks.com/dev-tools/api/latest/jobs.html.
+
+    Returns:
+        OpDefinition: An op definition.
+
+    Example:
+
+        .. code-block:: python
+
+            from dagster import graph
+            from dagster_databricks import create_databricks_job_op, databricks_client
+
+            sparkpi = create_databricks_job_op().configured(
+                {
+                    "job": {
+                        "name": "SparkPi Python job",
+                        "new_cluster": {
+                            "spark_version": "7.3.x-scala2.12",
+                            "node_type_id": "i3.xlarge",
+                            "num_workers": 2,
+                        },
+                        "spark_python_task": {"python_file": "dbfs:/docs/pi.py", "parameters": ["10"]},
+                    }
+                },
+                name="sparkpi",
+            )
+
+            @graph
+            def my_spark():
+                sparkpi()
+
+            my_spark.to_job(
+                resource_defs={
+                    "databricks_client": databricks_client.configured(
+                        {"host": "my.workspace.url", "token": "my.access.token"}
+                    )
+                }
+            )
     """
     check.str_param(name, "name")
     check.opt_str_param(description, "description")
     check.int_param(num_inputs, "num_inputs")
     check.set_param(required_resource_keys, "required_resource_keys", of_type=str)
 
-    input_defs = [InputDefinition("input_" + str(i), Nothing) for i in range(num_inputs)]
+    ins = {"input_" + str(i): In(Nothing) for i in range(num_inputs)}
 
-    @solid(
+    @op(
         name=name,
         description=description,
         config_schema={
             "job": Field(
                 Permissive(),
                 description="Databricks job run configuration, in the form described in "
                 "Databricks' job API: https://docs.databricks.com/dev-tools/api/latest/jobs.html",
             ),
             "poll_interval_sec": Field(
                 float,
                 description="Check whether the job is done at this interval.",
-                default_value=10,
+                default_value=_DEFAULT_POLL_INTERVAL,
             ),
             "max_wait_time_sec": Field(
                 float,
                 description="If the job is not complete after this length of time, raise an error.",
-                default_value=(24 * 60 * 60),
+                default_value=_DEFAULT_RUN_MAX_WAIT_TIME_SEC,
             ),
         },
-        input_defs=input_defs,
-        output_defs=[OutputDefinition(Nothing)],
+        ins=ins,
+        out=Out(Nothing),
         required_resource_keys=required_resource_keys,
         tags={"kind": "databricks"},
     )
-    def databricks_solid(context):
-        job_config = context.solid_config["job"]
+    def databricks_fn(context):
+        job_config = context.op_config["job"]
         databricks_client = context.resources.databricks_client
         run_id = databricks_client.submit_run(**job_config)
 
         context.log.info(
             "Launched databricks job with run id {run_id}. UI: {url}. Waiting to run to completion...".format(
-                run_id=run_id, url=create_ui_url(databricks_client, context.solid_config)
+                run_id=run_id, url=create_ui_url(databricks_client, context.op_config)
             )
         )
         wait_for_run_to_complete(
             databricks_client,
             context.log,
             run_id,
-            context.solid_config["poll_interval_sec"],
-            context.solid_config["max_wait_time_sec"],
+            context.op_config["poll_interval_sec"],
+            context.op_config["max_wait_time_sec"],
         )
 
-    return databricks_solid
+    return databricks_fn
 
 
-def create_ui_url(databricks_client, solid_config):
+def create_ui_url(databricks_client, op_config):
     host = databricks_client.host
     workspace_id = databricks_client.workspace_id or "<workspace_id>"
-    if "existing_cluster_id" in solid_config["job"]:
+    if "existing_cluster_id" in op_config["job"]:
         return "https://{host}/?o={workspace_id}#/setting/clusters/{cluster_id}/sparkUi".format(
             host=host,
             workspace_id=workspace_id,
-            cluster_id=solid_config["job"]["existing_cluster_id"],
+            cluster_id=op_config["job"]["existing_cluster_id"],
         )
     else:
         return "https://{host}/?o={workspace_id}#joblist".format(
             host=host, workspace_id=workspace_id
         )
```

### Comparing `dagster-databricks-0.9.9rc1/dagster_databricks/types.py` & `dagster-databricks-1.0.5/dagster_databricks/types.py`

 * *Files identical despite different names*

### Comparing `dagster-databricks-0.9.9rc1/dagster_databricks.egg-info/SOURCES.txt` & `dagster-databricks-1.0.5/dagster_databricks.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,22 +4,18 @@
 setup.cfg
 setup.py
 dagster_databricks/__init__.py
 dagster_databricks/configs.py
 dagster_databricks/databricks.py
 dagster_databricks/databricks_pyspark_step_launcher.py
 dagster_databricks/databricks_step_main.py
+dagster_databricks/py.typed
 dagster_databricks/resources.py
 dagster_databricks/solids.py
 dagster_databricks/types.py
 dagster_databricks/version.py
 dagster_databricks.egg-info/PKG-INFO
 dagster_databricks.egg-info/SOURCES.txt
 dagster_databricks.egg-info/dependency_links.txt
 dagster_databricks.egg-info/not-zip-safe
 dagster_databricks.egg-info/requires.txt
-dagster_databricks.egg-info/top_level.txt
-dagster_databricks_tests/__init__.py
-dagster_databricks_tests/conftest.py
-dagster_databricks_tests/test_databricks.py
-dagster_databricks_tests/test_pyspark.py
-dagster_databricks_tests/test_solids.py
+dagster_databricks.egg-info/top_level.txt
```

### Comparing `dagster-databricks-0.9.9rc1/setup.py` & `dagster-databricks-1.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,42 @@
+from typing import Dict
+
 from setuptools import find_packages, setup
 
 
-def get_version():
-    version = {}
-    with open("dagster_databricks/version.py") as fp:
+def get_version() -> str:
+    version: Dict[str, str] = {}
+    with open("dagster_databricks/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
 if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
     setup(
         name="dagster-databricks",
-        version=get_version(),
+        version=ver,
         author="Elementl",
         author_email="hello@elementl.com",
         license="Apache-2.0",
         description="Package for Databricks-specific Dagster framework solid and resource components.",
         url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-databricks",
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
+        packages=find_packages(exclude=["dagster_databricks_tests*"]),
         include_package_data=True,
-        install_requires=["dagster", "dagster-pyspark", "databricks_api"],
+        install_requires=[
+            "dagster==1.0.5",
+            "dagster-pyspark==1.0.5",
+            "databricks_api",
+        ],
         zip_safe=False,
     )
```

