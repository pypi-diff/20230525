# Comparing `tmp/prefect-gcp-0.4.1.tar.gz` & `tmp/prefect-gcp-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-gcp/prefect-gcp/dist/.tmp-pvh27_8d/prefect-gcp-0.4.1.tar", last modified: Fri Apr 21 00:07:50 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-gcp/prefect-gcp/dist/.tmp-b22u9uqx/prefect-gcp-0.4.2.tar", last modified: Thu May 25 19:23:55 2023, max compression
```

## Comparing `prefect-gcp-0.4.1.tar` & `prefect-gcp-0.4.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15903 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/aiplatform.py
--rw-r--r--   0 runner    (1001) docker     (123)    33862 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    27602 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    45746 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp/projects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/projects/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    30893 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/tests/test_aiplatform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/tests/test_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)    29089 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/tests/test_cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/tests/test_cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/tests/test_secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    24842 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/aiplatform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27540 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45746 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/projects/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31604 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/tests/test_aiplatform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/tests/test_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29089 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/tests/test_cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/tests/test_cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/tests/test_secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24842 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/versioneer.py
```

### Comparing `prefect-gcp-0.4.1/LICENSE` & `prefect-gcp-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.1/PKG-INFO` & `prefect-gcp-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-gcp
-Version: 0.4.1
+Version: 0.4.2
 Summary: Prefect tasks and subflows for interacting with Google Cloud Platform.
 Home-page: https://github.com/PrefectHQ/prefect-gcp
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.1 Summary: Prefect tasks
+Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.2 Summary: Prefect tasks
 and subflows for interacting with Google Cloud Platform. Home-page: https://
 github.com/PrefectHQ/prefect-gcp Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-gcp-0.4.1/README.md` & `prefect-gcp-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.1/prefect_gcp/aiplatform.py` & `prefect-gcp-0.4.2/prefect_gcp/aiplatform.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         CustomJob,
         CustomJobSpec,
         Scheduling,
         WorkerPoolSpec,
     )
     from google.cloud.aiplatform_v1.types.job_service import CancelCustomJobRequest
     from google.cloud.aiplatform_v1.types.job_state import JobState
-    from google.cloud.aiplatform_v1.types.machine_resources import MachineSpec
+    from google.cloud.aiplatform_v1.types.machine_resources import DiskSpec, MachineSpec
     from google.protobuf.duration_pb2 import Duration
 except ModuleNotFoundError:
     pass
 
 from prefect_gcp.credentials import GcpCredentials
 
 
@@ -134,14 +134,27 @@
         default="n1-standard-4",
         description="The machine type to use for the run, which controls the available "
         "CPU and memory.",
     )
     accelerator_type: Optional[str] = Field(
         default=None, description="The type of accelerator to attach to the machine."
     )
+    accelerator_count: Optional[int] = Field(
+        default=None, description="The number of accelerators to attach to the machine."
+    )
+    boot_disk_type: str = Field(
+        default="pd-ssd",
+        title="Boot Disk Type",
+        description="The type of boot disk to attach to the machine.",
+    )
+    boot_disk_size_gb: int = Field(
+        default=100,
+        title="Boot Disk Size",
+        description="The size of the boot disk to attach to the machine, in gigabytes.",
+    )
     maximum_run_time: datetime.timedelta = Field(
         default=datetime.timedelta(days=7), description="The maximum job running time."
     )
     network: Optional[str] = Field(
         default=None,
         description="The full name of the Compute Engine network"
         "to which the Job should be peered. Private services access must "
@@ -211,20 +224,27 @@
                 **self.env,
             }.items()
         ]
         container_spec = ContainerSpec(
             image_uri=self.image, command=self.command, args=[], env=env_list
         )
         machine_spec = MachineSpec(
-            machine_type=self.machine_type, accelerator_type=self.accelerator_type
+            machine_type=self.machine_type,
+            accelerator_type=self.accelerator_type,
+            accelerator_count=self.accelerator_count,
         )
         worker_pool_spec = WorkerPoolSpec(
-            container_spec=container_spec, machine_spec=machine_spec, replica_count=1
+            container_spec=container_spec,
+            machine_spec=machine_spec,
+            replica_count=1,
+            disk_spec=DiskSpec(
+                boot_disk_type=self.boot_disk_type,
+                boot_disk_size_gb=self.boot_disk_size_gb,
+            ),
         )
-
         # look for service account
         service_account = (
             self.service_account or self.gcp_credentials._service_account_email
         )
         if service_account is None:
             raise ValueError(
                 "A service account is required for the Vertex job. "
```

### Comparing `prefect-gcp-0.4.1/prefect_gcp/bigquery.py` & `prefect-gcp-0.4.2/prefect_gcp/bigquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Tasks for interacting with GCP BigQuery"""
 
 import os
 from functools import partial
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from anyio import to_thread
 from prefect import get_run_logger, task
 from prefect.blocks.abstract import DatabaseBlock
 from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
 from prefect.utilities.hashing import hash_objects
 from pydantic import Field
@@ -48,16 +48,17 @@
     query_params: Optional[List[tuple]] = None,  # 3-tuples
     dry_run_max_bytes: Optional[int] = None,
     dataset: Optional[str] = None,
     table: Optional[str] = None,
     to_dataframe: bool = False,
     job_config: Optional[dict] = None,
     project: Optional[str] = None,
+    result_transformer: Optional[Callable[[List["Row"]], Any]] = None,
     location: str = "US",
-) -> List["Row"]:
+) -> Any:
     """
     Runs a BigQuery query.
 
     Args:
         query: String of the query to execute.
         gcp_credentials: Credentials to use for authentication with GCP.
         query_params: List of 3-tuples specifying BigQuery query parameters; currently
@@ -74,14 +75,15 @@
         to_dataframe: If provided, returns the results of the query as a pandas
             dataframe instead of a list of `bigquery.table.Row` objects.
         job_config: Dictionary of job configuration parameters;
             note that the parameters provided here must be pickleable
             (e.g., dataset references will be rejected).
         project: The project to initialize the BigQuery Client with; if not
             provided, will default to the one inferred from your credentials.
+        result_transformer: Function that can be passed to transform the result of a query before returning. The function will be passed the list of rows returned by BigQuery for the given query.
         location: Location of the dataset that will be queried.
 
     Returns:
         A list of rows, or pandas DataFrame if to_dataframe,
         matching the query criteria.
 
     Example:
@@ -152,18 +154,22 @@
     partial_query = partial(
         _result_sync,
         client.query,
         query,
         job_config=job_config,
     )
     result = await to_thread.run_sync(partial_query)
+
     if to_dataframe:
         return result.to_dataframe()
     else:
-        return list(result)
+        if result_transformer:
+            return result_transformer(result)
+        else:
+            return list(result)
 
 
 @task
 async def bigquery_create_table(
     dataset: str,
     table: str,
     gcp_credentials: GcpCredentials,
```

### Comparing `prefect-gcp-0.4.1/prefect_gcp/cloud_run.py` & `prefect-gcp-0.4.2/prefect_gcp/cloud_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,32 +28,27 @@
 
 """
 from __future__ import annotations
 
 import json
 import re
 import time
-
-try:
-    from typing import Literal
-except ImportError:
-    from typing_extensions import Literal
-
 from typing import Any, Dict, List, Optional
 from uuid import uuid4
 
 import googleapiclient
 from anyio.abc import TaskStatus
 from google.api_core.client_options import ClientOptions
 from googleapiclient import discovery
 from googleapiclient.discovery import Resource
 from prefect.exceptions import InfrastructureNotFound
 from prefect.infrastructure.base import Infrastructure, InfrastructureResult
 from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
 from pydantic import BaseModel, Field, root_validator, validator
+from typing_extensions import Literal
 
 from prefect_gcp.credentials import GcpCredentials
 
 
 class Job(BaseModel):
     """
     Utility class to call GCP `jobs` API and
```

### Comparing `prefect-gcp-0.4.1/prefect_gcp/cloud_storage.py` & `prefect-gcp-0.4.2/prefect_gcp/cloud_storage.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.1/prefect_gcp/credentials.py` & `prefect-gcp-0.4.2/prefect_gcp/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.1/prefect_gcp/projects/steps.py` & `prefect-gcp-0.4.2/prefect_gcp/projects/steps.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,25 +29,27 @@
     folder: str
     directory: str
 
 
 def push_project_to_gcs(
     bucket: str,
     folder: str,
+    project: Optional[str] = None,
     credentials: Optional[Dict] = None,
     ignore_file=".prefectignore",
 ) -> PushProjectToGcsOutput:
     """
-    Pushes the contents of the current working directory to an S3 bucket,
+    Pushes the contents of the current working directory to a GCS bucket,
     excluding files and folders specified in the ignore_file.
 
     Args:
-        bucket: The name of the S3 bucket where the project files will be uploaded.
-        folder: The folder in the S3 bucket where the project files will be uploaded.
-        project: The project the bucket belongs to.
+        bucket: The name of the GCS bucket where the project files will be uploaded.
+        folder: The folder in the GCS bucket where the project files will be uploaded.
+        project: The GCP project the bucket belongs to. If not provided, the project
+            will be inferred from the credentials or the local environment.
         credentials: A dictionary containing the service account information and project
             used for authentication. If not provided, the application default
             credentials will be used.
         ignore_file: The name of the file containing ignore patterns.
 
     Returns:
         A dictionary containing the bucket and folder where the project was uploaded.
@@ -132,23 +134,25 @@
         "folder": folder,
     }
 
 
 def pull_project_from_gcs(
     bucket: str,
     folder: str,
+    project: Optional[str] = None,
     credentials: Optional[Dict] = None,
 ) -> PullProjectFromGcsOutput:
     """
     Pulls the contents of a project from an GCS bucket to the current working directory.
 
     Args:
         bucket: The name of the GCS bucket where the project files are stored.
         folder: The folder in the GCS bucket where the project files are stored.
-        project: The project the bucket belongs to.
+        project: The GCP project the bucket belongs to. If not provided, the project will be
+            inferred from the credentials or the local environment.
         credentials: A dictionary containing the service account information and project
             used for authentication. If not provided, the application default
             credentials will be used.
 
     Returns:
         A dictionary containing the bucket, folder, and local directory where the
             project files were downloaded.
```

### Comparing `prefect-gcp-0.4.1/prefect_gcp/secret_manager.py` & `prefect-gcp-0.4.2/prefect_gcp/secret_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.1/prefect_gcp/worker.py` & `prefect-gcp-0.4.2/prefect_gcp/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,15 @@
 import googleapiclient
 from anyio.abc import TaskStatus  # noqa
 from google.api_core.client_options import ClientOptions
 from googleapiclient import discovery
 from googleapiclient.discovery import Resource
 from prefect.docker import get_prefect_image_name
 from prefect.exceptions import InfrastructureNotFound
+from prefect.logging.loggers import PrefectLogAdapter
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
 from prefect.utilities.pydantic import JsonPatch
 from prefect.workers.base import (
     BaseJobConfiguration,
     BaseVariables,
     BaseWorker,
     BaseWorkerResult,
@@ -512,14 +513,22 @@
 
 class CloudRunWorker(BaseWorker):
     """Prefect worker that executes flow runs within Cloud Run Jobs."""
 
     type = "cloud-run"
     job_configuration = CloudRunWorkerJobConfiguration
     job_configuration_variables = CloudRunWorkerVariables
+    _description = (
+        "Execute flow runs within containers on Google Cloud Run. Requires "
+        "a Google Cloud Platform account."
+    )
+    _display_name = "Google Cloud Run"
+    _documentation_url = "https://prefecthq.github.io/prefect-gcp/worker/"
+    _is_beta = True
+    _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/4SpnOBvMYkHp6z939MDKP6/549a91bc1ce9afd4fb12c68db7b68106/social-icon-google-cloud-1200-630.png?h=250"  # noqa
 
     def _create_job_error(self, exc, configuration):
         """Provides a nicer error for 404s when trying to create a Cloud Run Job."""
         # TODO consider lookup table instead of the if/else,
         # also check for documented errors
         if exc.status_code == 404:
             raise RuntimeError(
@@ -570,30 +579,37 @@
             task_status: The task status object for the current flow run. If provided,
                 the task will be marked as started.
 
         Returns:
             CloudRunWorkerResult: A result object containing information about the
                 final state of the flow run
         """
+
+        logger = self.get_flow_run_logger(flow_run)
+
         with self._get_client(configuration) as client:
             await run_sync_in_worker_thread(
-                self._create_job_and_wait_for_registration, configuration, client
+                self._create_job_and_wait_for_registration,
+                configuration,
+                client,
+                logger,
             )
             job_execution = await run_sync_in_worker_thread(
-                self._begin_job_execution, configuration, client
+                self._begin_job_execution, configuration, client, logger
             )
 
             if task_status:
                 task_status.started(configuration.job_name)
 
             result = await run_sync_in_worker_thread(
                 self._watch_job_execution_and_get_result,
                 configuration,
                 client,
                 job_execution,
+                logger,
             )
             return result
 
     def _get_client(self, configuration: CloudRunWorkerJobConfiguration) -> Resource:
         """Get the base client needed for interacting with GCP APIs."""
         # region needed for 'v1' API
         api_endpoint = f"https://{configuration.region}-run.googleapis.com"
@@ -601,58 +617,66 @@
         options = ClientOptions(api_endpoint=api_endpoint)
 
         return discovery.build(
             "run", "v1", client_options=options, credentials=gcp_creds
         ).namespaces()
 
     def _create_job_and_wait_for_registration(
-        self, configuration: CloudRunWorkerJobConfiguration, client: Resource
+        self,
+        configuration: CloudRunWorkerJobConfiguration,
+        client: Resource,
+        logger: PrefectLogAdapter,
     ) -> None:
         """Create a new job wait for it to finish registering."""
         try:
-            self._logger.info(f"Creating Cloud Run Job {configuration.job_name}")
+            logger.info(f"Creating Cloud Run Job {configuration.job_name}")
 
             Job.create(
                 client=client,
                 namespace=configuration.credentials.project,
                 body=configuration.job_body,
             )
         except googleapiclient.errors.HttpError as exc:
             self._create_job_error(exc, configuration)
 
         try:
-            self._wait_for_job_creation(client=client, configuration=configuration)
+            self._wait_for_job_creation(
+                client=client, configuration=configuration, logger=logger
+            )
         except Exception:
-            self._logger.exception(
+            logger.exception(
                 "Encountered an exception while waiting for job run creation"
             )
             if not configuration.keep_job:
-                self._logger.info(
+                logger.info(
                     f"Deleting Cloud Run Job {configuration.job_name} from "
                     "Google Cloud Run."
                 )
                 try:
                     Job.delete(
                         client=client,
                         namespace=configuration.credentials.project,
                         job_name=configuration.job_name,
                     )
                 except Exception:
-                    self._logger.exception(
+                    logger.exception(
                         "Received an unexpected exception while attempting to delete"
                         f" Cloud Run Job {configuration.job_name!r}"
                     )
             raise
 
     def _begin_job_execution(
-        self, configuration: CloudRunWorkerJobConfiguration, client: Resource
+        self,
+        configuration: CloudRunWorkerJobConfiguration,
+        client: Resource,
+        logger: PrefectLogAdapter,
     ) -> Execution:
         """Submit a job run for execution and return the execution object."""
         try:
-            self._logger.info(
+            logger.info(
                 f"Submitting Cloud Run Job {configuration.job_name!r} for execution."
             )
             submission = Job.run(
                 client=client,
                 namespace=configuration.project,
                 job_name=configuration.job_name,
             )
@@ -668,61 +692,58 @@
         return job_execution
 
     def _watch_job_execution_and_get_result(
         self,
         configuration: CloudRunWorkerJobConfiguration,
         client: Resource,
         execution: Execution,
+        logger: PrefectLogAdapter,
         poll_interval: int = 5,
     ) -> CloudRunWorkerResult:
         """Wait for execution to complete and then return result."""
         try:
             job_execution = self._watch_job_execution(
                 client=client,
                 job_execution=execution,
                 timeout=configuration.timeout,
                 poll_interval=poll_interval,
             )
         except Exception:
-            self._logger.exception(
+            logger.exception(
                 "Received an unexpected exception while monitoring Cloud Run Job "
                 f"{configuration.job_name!r}"
             )
             raise
 
         if job_execution.succeeded():
             status_code = 0
-            self._logger.info(
-                f"Job Run {configuration.job_name} completed successfully"
-            )
+            logger.info(f"Job Run {configuration.job_name} completed successfully")
         else:
             status_code = 1
             error_msg = job_execution.condition_after_completion()["message"]
-            self._logger.error(
+            logger.error(
                 "Job Run {configuration.job_name} did not complete successfully. "
                 f"{error_msg}"
             )
 
-        self._logger.info(
-            f"Job Run logs can be found on GCP at: {job_execution.log_uri}"
-        )
+        logger.info(f"Job Run logs can be found on GCP at: {job_execution.log_uri}")
 
         if not configuration.keep_job:
-            self._logger.info(
+            logger.info(
                 f"Deleting completed Cloud Run Job {configuration.job_name!r} "
                 "from Google Cloud Run..."
             )
             try:
                 Job.delete(
                     client=client,
                     namespace=configuration.project,
                     job_name=configuration.job_name,
                 )
             except Exception:
-                self._logger.exception(
+                logger.exception(
                     "Received an unexpected exception while attempting to delete Cloud"
                     f" Run Job {configuration.job_name}"
                 )
 
         return CloudRunWorkerResult(
             identifier=configuration.job_name, status_code=status_code
         )
@@ -752,14 +773,15 @@
 
         return job_execution
 
     def _wait_for_job_creation(
         self,
         client: Resource,
         configuration: CloudRunWorkerJobConfiguration,
+        logger: PrefectLogAdapter,
         poll_interval: int = 5,
     ):
         """Give created job time to register."""
         job = Job.get(
             client=client,
             namespace=configuration.project,
             job_name=configuration.job_name,
@@ -768,17 +790,15 @@
         t0 = time.time()
         while not job.is_ready():
             ready_condition = (
                 job.ready_condition
                 if job.ready_condition
                 else "waiting for condition update"
             )
-            self._logger.info(
-                f"Job is not yet ready... Current condition: {ready_condition}"
-            )
+            logger.info(f"Job is not yet ready... Current condition: {ready_condition}")
             job = Job.get(
                 client=client,
                 namespace=configuration.project,
                 job_name=configuration.job_name,
             )
 
             elapsed_time = time.time() - t0
```

### Comparing `prefect-gcp-0.4.1/prefect_gcp.egg-info/PKG-INFO` & `prefect-gcp-0.4.2/prefect_gcp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-gcp
-Version: 0.4.1
+Version: 0.4.2
 Summary: Prefect tasks and subflows for interacting with Google Cloud Platform.
 Home-page: https://github.com/PrefectHQ/prefect-gcp
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.1 Summary: Prefect tasks
+Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.2 Summary: Prefect tasks
 and subflows for interacting with Google Cloud Platform. Home-page: https://
 github.com/PrefectHQ/prefect-gcp Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-gcp-0.4.1/prefect_gcp.egg-info/SOURCES.txt` & `prefect-gcp-0.4.2/prefect_gcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.1/prefect_gcp.egg-info/requires.txt` & `prefect-gcp-0.4.2/prefect_gcp.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-prefect>=2.10.5
+prefect>=2.10.9
 google-api-python-client>=2.20.0
 google-cloud-storage>=2.0.0
 
 [aiplatform]
 google-cloud-aiplatform
 
 [all_extras]
```

### Comparing `prefect-gcp-0.4.1/setup.cfg` & `prefect-gcp-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.1/setup.py` & `prefect-gcp-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.1/tests/test_aiplatform.py` & `prefect-gcp-0.4.2/tests/test_aiplatform.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from unittest.mock import MagicMock, patch
 
 import pytest
+from google.cloud.aiplatform_v1.types.accelerator_type import AcceleratorType
 from google.cloud.aiplatform_v1.types.job_state import JobState
 from prefect.exceptions import InfrastructureNotFound
 
 from prefect_gcp.aiplatform import (
     VertexAICustomTrainingJob,
     VertexAICustomTrainingJobResult,
 )
@@ -41,14 +42,18 @@
                           value: "secret"
                       }
                     }
                     machine_spec {
                         machine_type: "n1-standard-4"
                     }
                     replica_count: 1
+                    disk_spec {
+                        boot_disk_type: "pd-ssd"
+                        boot_disk_size_gb: 100
+                    }
                 }
                 scheduling {
                 }
                 service_account: "my_service_account_email"
             }
         """.strip().splitlines()
 
@@ -136,7 +141,21 @@
         )
         gcp_credentials = vertex_ai_custom_training_job.gcp_credentials
         gcp_credentials.job_service_client.get_custom_job.return_value = (
             failed_run_final
         )
         with pytest.raises(RuntimeError, match="my error msg"):
             vertex_ai_custom_training_job.run()
+
+    def test_machine_spec(
+        self, vertex_ai_custom_training_job: VertexAICustomTrainingJob
+    ):
+        vertex_ai_custom_training_job.accelerator_count = 1
+        vertex_ai_custom_training_job.accelerator_type = "NVIDIA_TESLA_T4"
+
+        job_spec = vertex_ai_custom_training_job._build_job_spec()
+
+        assert job_spec.worker_pool_specs[0].machine_spec.accelerator_count == 1
+        assert (
+            job_spec.worker_pool_specs[0].machine_spec.accelerator_type
+            == AcceleratorType.NVIDIA_TESLA_T4
+        )
```

### Comparing `prefect-gcp-0.4.1/tests/test_bigquery.py` & `prefect-gcp-0.4.2/tests/test_bigquery.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,40 +13,47 @@
     bigquery_load_cloud_storage,
     bigquery_load_file,
     bigquery_query,
 )
 
 
 @pytest.mark.parametrize("to_dataframe", [False, True])
+@pytest.mark.parametrize("result_transformer", [None, lambda _: ("test_transformer",)])
 @pytest.mark.parametrize("dry_run_max_bytes", [None, 5, 15])
-def test_bigquery_query(to_dataframe, dry_run_max_bytes, gcp_credentials):
+def test_bigquery_query(
+    to_dataframe, result_transformer, dry_run_max_bytes, gcp_credentials
+):
     @flow
     def test_flow():
         return bigquery_query(
             "query",
             gcp_credentials,
             to_dataframe=to_dataframe,
             query_params=[("param", str, "parameter")],
             dry_run_max_bytes=dry_run_max_bytes,
             dataset="dataset",
             table="test_table",
             job_config={},
             project="project",
             location="US",
+            result_transformer=result_transformer,
         )
 
     if dry_run_max_bytes is not None and dry_run_max_bytes < 10:
         with pytest.raises(RuntimeError):
             test_flow()
     else:
         result = test_flow()
         if to_dataframe:
             assert result == "dataframe_query"
         else:
-            assert result == ["query"]
+            if result_transformer:
+                assert result == ("test_transformer",)
+            else:
+                assert result == ["query"]
 
 
 def test_bigquery_create_table(gcp_credentials):
     @flow
     def test_flow():
         schema = [
             SchemaField("number", field_type="INTEGER", mode="REQUIRED"),
```

### Comparing `prefect-gcp-0.4.1/tests/test_block_standards.py` & `prefect-gcp-0.4.2/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.1/tests/test_cloud_run.py` & `prefect-gcp-0.4.2/tests/test_cloud_run.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.1/tests/test_cloud_storage.py` & `prefect-gcp-0.4.2/tests/test_cloud_storage.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.1/tests/test_credentials.py` & `prefect-gcp-0.4.2/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.1/tests/test_secret_manager.py` & `prefect-gcp-0.4.2/tests/test_secret_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.1/tests/test_worker.py` & `prefect-gcp-0.4.2/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.1/versioneer.py` & `prefect-gcp-0.4.2/versioneer.py`

 * *Files identical despite different names*

