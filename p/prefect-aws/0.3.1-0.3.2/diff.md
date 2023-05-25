# Comparing `tmp/prefect-aws-0.3.1.tar.gz` & `tmp/prefect-aws-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-aws/prefect-aws/dist/.tmp-o3glckyr/prefect-aws-0.3.1.tar", last modified: Fri Apr 21 00:08:40 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-aws/prefect-aws/dist/.tmp-vsru1pap/prefect-aws-0.3.2.tar", last modified: Thu May 25 19:27:14 2023, max compression
```

## Comparing `prefect-aws-0.3.1.tar` & `prefect-aws-0.3.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/client_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/client_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    57767 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/ecs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws/projects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/projects/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    32782 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    17380 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/secrets_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56563 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/workers/ecs_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/tests/test_client_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/tests/test_client_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    67274 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/tests/test_ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23866 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/tests/test_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    80043 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/client_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/client_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57767 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/ecs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/projects/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32900 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17380 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/secrets_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56892 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/workers/ecs_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/tests/test_client_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/tests/test_client_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67274 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/tests/test_ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26625 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/tests/test_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80043 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/versioneer.py
```

### Comparing `prefect-aws-0.3.1/LICENSE` & `prefect-aws-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.1/PKG-INFO` & `prefect-aws-0.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-aws
-Version: 0.3.1
+Version: 0.3.2
 Summary: Prefect collection of tasks and subflows to integrate with AWS
 Home-page: https://github.com/PrefectHQ/prefect-aws
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
@@ -54,8 +54,8 @@
 
 ```bash
 pip install prefect-aws
 ```
 
 ### Contributing
 
-Thanks for thinking about chipping in! Check out this [step-by-step guide](https://prefecthq.github.io/prefect-gcp/#installation) on how to get started.
+Thanks for thinking about chipping in! Check out this [step-by-step guide](https://prefecthq.github.io/prefect-aws/#installation) on how to get started.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.1 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.2 Summary: Prefect
 collection of tasks and subflows to integrate with AWS Home-page: https://
 github.com/PrefectHQ/prefect-aws Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
@@ -23,8 +23,8 @@
             red.svg?color=0052FF&labelColor=090422&logo=discourse]
 ## Welcome! The `prefect-aws` collection makes it easy to leverage the
 capabilities of AWS in your flows, featuring support for ECS, S3, Secrets
 Manager, Batch Job, and Client Waiter. Visit the full docs [here](https://
 PrefectHQ.github.io/prefect-aws). ### Installation To start using `prefect-
 aws`: ```bash pip install prefect-aws ``` ### Contributing Thanks for thinking
 about chipping in! Check out this [step-by-step guide](https://
-prefecthq.github.io/prefect-gcp/#installation) on how to get started.
+prefecthq.github.io/prefect-aws/#installation) on how to get started.
```

### Comparing `prefect-aws-0.3.1/README.md` & `prefect-aws-0.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 
 ```bash
 pip install prefect-aws
 ```
 
 ### Contributing
 
-Thanks for thinking about chipping in! Check out this [step-by-step guide](https://prefecthq.github.io/prefect-gcp/#installation) on how to get started.
+Thanks for thinking about chipping in! Check out this [step-by-step guide](https://prefecthq.github.io/prefect-aws/#installation) on how to get started.
```

#### html2text {}

```diff
@@ -11,8 +11,8 @@
             red.svg?color=0052FF&labelColor=090422&logo=discourse]
 ## Welcome! The `prefect-aws` collection makes it easy to leverage the
 capabilities of AWS in your flows, featuring support for ECS, S3, Secrets
 Manager, Batch Job, and Client Waiter. Visit the full docs [here](https://
 PrefectHQ.github.io/prefect-aws). ### Installation To start using `prefect-
 aws`: ```bash pip install prefect-aws ``` ### Contributing Thanks for thinking
 about chipping in! Check out this [step-by-step guide](https://
-prefecthq.github.io/prefect-gcp/#installation) on how to get started.
+prefecthq.github.io/prefect-aws/#installation) on how to get started.
```

### Comparing `prefect-aws-0.3.1/prefect_aws/batch.py` & `prefect-aws-0.3.2/prefect_aws/batch.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.1/prefect_aws/client_parameters.py` & `prefect-aws-0.3.2/prefect_aws/client_parameters.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.1/prefect_aws/client_waiter.py` & `prefect-aws-0.3.2/prefect_aws/client_waiter.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.1/prefect_aws/credentials.py` & `prefect-aws-0.3.2/prefect_aws/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.1/prefect_aws/ecs.py` & `prefect-aws-0.3.2/prefect_aws/ecs.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.1/prefect_aws/projects/steps.py` & `prefect-aws-0.3.2/prefect_aws/projects/steps.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.1/prefect_aws/s3.py` & `prefect-aws-0.3.2/prefect_aws/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,14 +261,17 @@
         default="",
         description=(
             "A default path to a folder within the S3 bucket to use "
             "for reading and writing objects."
         ),
     )
 
+    class Config:
+        smart_union = True
+
     # Property to maintain compatibility with storage block based deployments
     @property
     def basepath(self) -> str:
         """
         The base path of the S3 bucket.
 
         Returns:
@@ -538,15 +541,18 @@
 
         bucket_path = str(bucket_path)
         if self.bucket_folder != "" and bucket_path.startswith(self.bucket_folder):
             self.logger.info(
                 f"Bucket path {bucket_path!r} is already prefixed with "
                 f"bucket folder {self.bucket_folder!r}; is this intentional?"
             )
-        return (Path(self.bucket_folder) / bucket_path).as_posix()
+
+        return (Path(self.bucket_folder) / bucket_path).as_posix() + (
+            "" if not bucket_path.endswith("/") else "/"
+        )
 
     @sync_compatible
     async def list_objects(
         self,
         folder: str = "",
         delimiter: str = "",
         page_size: Optional[int] = None,
```

### Comparing `prefect-aws-0.3.1/prefect_aws/secrets_manager.py` & `prefect-aws-0.3.2/prefect_aws/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.1/prefect_aws/workers/ecs_worker.py` & `prefect-aws-0.3.2/prefect_aws/workers/ecs_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 
 import anyio
 import anyio.abc
 import boto3
 import yaml
 from prefect.docker import get_prefect_image_name
 from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
-from prefect.logging.loggers import get_logger
 from prefect.server.schemas.core import FlowRun
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
 from prefect.workers.base import (
     BaseJobConfiguration,
     BaseVariables,
     BaseWorker,
     BaseWorkerResult,
@@ -314,14 +313,18 @@
                 "`configure_cloudwatch_log` must be enabled to use "
                 "`cloudwatch_logs_options`."
             )
         return values
 
 
 class ECSVariables(BaseVariables):
+    """
+    Variables for templating an ECS job.
+    """
+
     task_definition_arn: Optional[str] = Field(
         default=None,
         description=(
             "An identifier for an existing task definition to use. If set, options that"
             " require changes to the task definition will be ignored. All contents of "
             "the task definition in the job configuration will be ignored."
         ),
@@ -486,44 +489,50 @@
             "deregistered. Deregistering a task definition does not remove it from "
             "your AWS account, instead it will be marked as INACTIVE."
         ),
     )
 
 
 class ECSWorkerResult(BaseWorkerResult):
-    pass
+    """
+    The result of an ECS job.
+    """
 
 
 class ECSWorker(BaseWorker):
+    """
+    A Prefect worker to run flow runs as ECS tasks.
+    """
+
     type = "ecs"
     job_configuration = ECSJobConfiguration
     job_configuration_variables = ECSVariables
-
-    def get_logger(self, flow_run: FlowRun):
-        """
-        Get a logger for the given flow run.
-        """
-        # This could stream to the API in the future; should be implemented on the base
-        # worker class
-        return get_logger("prefect.workers.ecs").getChild(slugify(flow_run.name))
+    _description = (
+        "Execute flow runs within containers on AWS ECS. Works with existing ECS "
+        "clusters and serverless execution via AWS Fargate. Requires an AWS account."
+    )
+    _display_name = "AWS Elastic Container Service"
+    _documentation_url = "https://prefecthq.github.io/prefect-aws/ecs_worker/"
+    _is_beta = True
+    _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/1jbV4lceHOjGgunX15lUwT/db88e184d727f721575aeb054a37e277/aws.png?h=250"  # noqa
 
     async def run(
         self,
         flow_run: "FlowRun",
         configuration: ECSJobConfiguration,
         task_status: Optional[anyio.abc.TaskStatus] = None,
     ) -> BaseWorkerResult:
         """
         Runs a given flow run on the current worker.
         """
         boto_session, ecs_client = await run_sync_in_worker_thread(
             self._get_session_and_client, configuration
         )
 
-        logger = self.get_logger(flow_run)
+        logger = self.get_flow_run_logger(flow_run)
 
         (
             task_arn,
             cluster_arn,
             task_definition,
             is_new_task_definition,
         ) = await run_sync_in_worker_thread(
@@ -1450,31 +1459,31 @@
             taskdef_2.pop(field, None)
 
         return taskdef_1 == taskdef_2
 
     async def kill_infrastructure(
         self,
         configuration: ECSJobConfiguration,
-        identifier: str,
+        infrastructure_pid: str,
         grace_seconds: int = 30,
     ) -> None:
         """
         Kill a task running on ECS.
 
         Args:
-            identifier: A cluster and task arn combination. This should match a value
-                yielded by `ECSTask.run`.
+            infrastructure_pid: A cluster and task arn combination. This should match a
+                value yielded by `ECSWorker.run`.
         """
         if grace_seconds != 30:
             self._logger.warning(
                 f"Kill grace period of {grace_seconds}s requested, but AWS does not "
                 "support dynamic grace period configuration so 30s will be used. "
                 "See https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-agent-config.html for configuration of grace periods."  # noqa
             )
-        cluster, task = parse_identifier(identifier)
+        cluster, task = parse_identifier(infrastructure_pid)
         await run_sync_in_worker_thread(self._stop_task, configuration, cluster, task)
 
     def _stop_task(
         self, configuration: ECSJobConfiguration, cluster: str, task: str
     ) -> None:
         """
         Stop a running ECS task.
```

### Comparing `prefect-aws-0.3.1/prefect_aws.egg-info/PKG-INFO` & `prefect-aws-0.3.2/prefect_aws.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-aws
-Version: 0.3.1
+Version: 0.3.2
 Summary: Prefect collection of tasks and subflows to integrate with AWS
 Home-page: https://github.com/PrefectHQ/prefect-aws
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
@@ -54,8 +54,8 @@
 
 ```bash
 pip install prefect-aws
 ```
 
 ### Contributing
 
-Thanks for thinking about chipping in! Check out this [step-by-step guide](https://prefecthq.github.io/prefect-gcp/#installation) on how to get started.
+Thanks for thinking about chipping in! Check out this [step-by-step guide](https://prefecthq.github.io/prefect-aws/#installation) on how to get started.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.1 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.2 Summary: Prefect
 collection of tasks and subflows to integrate with AWS Home-page: https://
 github.com/PrefectHQ/prefect-aws Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
@@ -23,8 +23,8 @@
             red.svg?color=0052FF&labelColor=090422&logo=discourse]
 ## Welcome! The `prefect-aws` collection makes it easy to leverage the
 capabilities of AWS in your flows, featuring support for ECS, S3, Secrets
 Manager, Batch Job, and Client Waiter. Visit the full docs [here](https://
 PrefectHQ.github.io/prefect-aws). ### Installation To start using `prefect-
 aws`: ```bash pip install prefect-aws ``` ### Contributing Thanks for thinking
 about chipping in! Check out this [step-by-step guide](https://
-prefecthq.github.io/prefect-gcp/#installation) on how to get started.
+prefecthq.github.io/prefect-aws/#installation) on how to get started.
```

### Comparing `prefect-aws-0.3.1/prefect_aws.egg-info/SOURCES.txt` & `prefect-aws-0.3.2/prefect_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.1/setup.cfg` & `prefect-aws-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.1/setup.py` & `prefect-aws-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.1/tests/test_batch.py` & `prefect-aws-0.3.2/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.1/tests/test_block_standards.py` & `prefect-aws-0.3.2/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.1/tests/test_client_parameters.py` & `prefect-aws-0.3.2/tests/test_client_parameters.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.1/tests/test_client_waiter.py` & `prefect-aws-0.3.2/tests/test_client_waiter.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.1/tests/test_credentials.py` & `prefect-aws-0.3.2/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.1/tests/test_ecs.py` & `prefect-aws-0.3.2/tests/test_ecs.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.1/tests/test_s3.py` & `prefect-aws-0.3.2/tests/test_s3.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,33 @@
     file = tmp_path / "object_in_folder.txt"
     file.write_text("TEST OBJECT IN FOLDER")
     with open(file, "rb") as f:
         return bucket.upload_fileobj(f, "folder/object")
 
 
 @pytest.fixture
+def objects_in_folder(bucket, tmp_path):
+    objects = []
+    for filename in [
+        "folderobject/foo.txt",
+        "folderobject/bar.txt",
+        "folder/object/foo.txt",
+        "folder/object/bar.txt",
+    ]:
+        file = tmp_path / filename
+        file.parent.mkdir(parents=True, exist_ok=True)
+        file.write_text("TEST OBJECTS IN FOLDER")
+        with open(file, "rb") as f:
+            filename = Path(filename)
+            obj = bucket.upload_fileobj(f, (filename.parent / filename.stem).as_posix())
+            objects.append(obj)
+    return objects
+
+
+@pytest.fixture
 def a_lot_of_objects(bucket, tmp_path):
     objects = []
     for i in range(0, 20):
         file = tmp_path / f"object{i}.txt"
         file.write_text("TEST")
         with open(file, "rb") as f:
             objects.append(bucket.upload_fileobj(f, f"object{i}"))
@@ -238,14 +257,44 @@
 
     objects = await test_flow()
     assert len(objects) == 1
     assert [object["Key"] for object in objects] == ["folder/object"]
 
 
 @pytest.mark.parametrize("client_parameters", aws_clients, indirect=True)
+async def test_s3_list_objects_prefix_slashes(
+    object, client_parameters, objects_in_folder, aws_credentials
+):
+    @flow
+    async def test_flow(slash=False):
+        return await s3_list_objects(
+            bucket="bucket",
+            prefix="folder" + ("/" if slash else ""),
+            aws_credentials=aws_credentials,
+            aws_client_parameters=client_parameters,
+        )
+
+    objects = await test_flow(slash=True)
+    assert len(objects) == 2
+    assert [object["Key"] for object in objects] == [
+        "folder/object/bar",
+        "folder/object/foo",
+    ]
+
+    objects = await test_flow(slash=False)
+    assert len(objects) == 4
+    assert [object["Key"] for object in objects] == [
+        "folder/object/bar",
+        "folder/object/foo",
+        "folderobject/bar",
+        "folderobject/foo",
+    ]
+
+
+@pytest.mark.parametrize("client_parameters", aws_clients, indirect=True)
 async def test_s3_list_objects_filter(
     object, client_parameters, object_in_folder, aws_credentials
 ):
     @flow
     async def test_flow():
         return await s3_list_objects(
             bucket="bucket",
@@ -581,14 +630,25 @@
     @pytest.fixture
     def s3_bucket_with_objects(self, s3_bucket_with_object, object_in_folder):
         _s3_bucket_with_objects = (
             s3_bucket_with_object  # object in folder will be added
         )
         return _s3_bucket_with_objects
 
+    @pytest.fixture
+    def s3_bucket_with_similar_objects(self, s3_bucket_with_objects, objects_in_folder):
+        _s3_bucket_with_multiple_objects = (
+            s3_bucket_with_objects  # objects in folder will be added
+        )
+        return _s3_bucket_with_multiple_objects
+
+    def test_credentials_are_correct_type(self, credentials):
+        s3_bucket = S3Bucket(bucket_name="bucket", credentials=credentials)
+        assert isinstance(s3_bucket.credentials, type(credentials))
+
     @pytest.mark.parametrize("client_parameters", aws_clients[-1:], indirect=True)
     def test_list_objects_empty(self, s3_bucket_empty, client_parameters):
         assert s3_bucket_empty.list_objects() == []
 
     @pytest.mark.parametrize("client_parameters", aws_clients[-1:], indirect=True)
     def test_list_objects_one(self, s3_bucket_with_object, client_parameters):
         objects = s3_bucket_with_object.list_objects()
@@ -597,14 +657,35 @@
 
     @pytest.mark.parametrize("client_parameters", aws_clients[-1:], indirect=True)
     def test_list_objects(self, s3_bucket_with_objects, client_parameters):
         objects = s3_bucket_with_objects.list_objects()
         assert len(objects) == 2
         assert [object["Key"] for object in objects] == ["folder/object", "object"]
 
+    @pytest.mark.parametrize("client_parameters", aws_clients[-1:], indirect=True)
+    def test_list_objects_with_params(
+        self, s3_bucket_with_similar_objects, client_parameters
+    ):
+        objects = s3_bucket_with_similar_objects.list_objects("folder/object/")
+        assert len(objects) == 2
+        assert [object["Key"] for object in objects] == [
+            "folder/object/bar",
+            "folder/object/foo",
+        ]
+
+        objects = s3_bucket_with_similar_objects.list_objects("folder")
+        assert len(objects) == 5
+        assert [object["Key"] for object in objects] == [
+            "folder/object",
+            "folder/object/bar",
+            "folder/object/foo",
+            "folderobject/bar",
+            "folderobject/foo",
+        ]
+
     @pytest.mark.parametrize("to_path", [Path("to_path"), "to_path", None])
     @pytest.mark.parametrize("client_parameters", aws_clients[-1:], indirect=True)
     def test_download_object_to_path(
         self, s3_bucket_with_object: S3Bucket, to_path, client_parameters, tmp_path
     ):
         os.chdir(tmp_path)
         s3_bucket_with_object.download_object_to_path("object", to_path)
```

### Comparing `prefect-aws-0.3.1/tests/test_secrets_manager.py` & `prefect-aws-0.3.2/tests/test_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.1/versioneer.py` & `prefect-aws-0.3.2/versioneer.py`

 * *Files identical despite different names*

