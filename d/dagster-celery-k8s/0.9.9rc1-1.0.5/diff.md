# Comparing `tmp/dagster-celery-k8s-0.9.9rc1.tar.gz` & `tmp/dagster-celery-k8s-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-celery-k8s-0.9.9rc1.tar", last modified: Thu Sep 17 21:07:50 2020, max compression
+gzip compressed data, was "dagster-celery-k8s-1.0.5.tar", last modified: Fri Aug 26 13:46:22 2022, max compression
```

## Comparing `dagster-celery-k8s-0.9.9rc1.tar` & `dagster-celery-k8s-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)      583 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      140 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/
--rw-r--r--   0 bobchen    (501) staff       (20)      250 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      351 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/app.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3003 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/config.py
--rw-r--r--   0 bobchen    (501) staff       (20)    21066 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/executor.py
--rw-r--r--   0 bobchen    (501) staff       (20)    13303 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/launcher.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      583 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      671 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       35 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       44 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      270 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s_tests/example_celery_mode_def.py
--rw-r--r--   0 bobchen    (501) staff       (20)      448 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s_tests/test_inclusion.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4906 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s_tests/test_launcher.py
--rw-r--r--   0 bobchen    (501) staff       (20)       96 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1055 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:22.380756 dagster-celery-k8s-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-celery-k8s-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       52 2022-08-26 13:33:01.000000 dagster-celery-k8s-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      620 2022-08-26 13:46:22.380756 dagster-celery-k8s-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      140 2022-08-26 13:33:01.000000 dagster-celery-k8s-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:22.380756 dagster-celery-k8s-1.0.5/dagster_celery_k8s/
+-rw-r--r--   0 root         (0) root         (0)      251 2022-08-26 13:33:01.000000 dagster-celery-k8s-1.0.5/dagster_celery_k8s/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      351 2022-08-26 13:33:01.000000 dagster-celery-k8s-1.0.5/dagster_celery_k8s/app.py
+-rw-r--r--   0 root         (0) root         (0)     3456 2022-08-26 13:33:01.000000 dagster-celery-k8s-1.0.5/dagster_celery_k8s/config.py
+-rw-r--r--   0 root         (0) root         (0)    22439 2022-08-26 13:33:01.000000 dagster-celery-k8s-1.0.5/dagster_celery_k8s/executor.py
+-rw-r--r--   0 root         (0) root         (0)    15283 2022-08-26 13:33:01.000000 dagster-celery-k8s-1.0.5/dagster_celery_k8s/launcher.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-celery-k8s-1.0.5/dagster_celery_k8s/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-celery-k8s-1.0.5/dagster_celery_k8s/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:22.380756 dagster-celery-k8s-1.0.5/dagster_celery_k8s.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      620 2022-08-26 13:46:22.000000 dagster-celery-k8s-1.0.5/dagster_celery_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      504 2022-08-26 13:46:22.000000 dagster-celery-k8s-1.0.5/dagster_celery_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:22.000000 dagster-celery-k8s-1.0.5/dagster_celery_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:22.000000 dagster-celery-k8s-1.0.5/dagster_celery_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       56 2022-08-26 13:46:22.000000 dagster-celery-k8s-1.0.5/dagster_celery_k8s.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2022-08-26 13:46:22.000000 dagster-celery-k8s-1.0.5/dagster_celery_k8s.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      165 2022-08-26 13:46:22.384757 dagster-celery-k8s-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1359 2022-08-26 13:33:01.000000 dagster-celery-k8s-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-celery-k8s-0.9.9rc1/PKG-INFO` & `dagster-celery-k8s-1.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-celery-k8s
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: A Dagster integration for celery-k8s-executor
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-celery-k8s
 Author: Elementl
-Author-email: UNKNOWN
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
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/config.py` & `dagster-celery-k8s-1.0.5/dagster_celery_k8s/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from dagster_celery.executor import CELERY_CONFIG
 from dagster_k8s import DagsterK8sJobConfig
+from dagster_k8s.client import DEFAULT_WAIT_TIMEOUT
 
-from dagster import Field, Noneable, StringSource
-from dagster.core.host_representation.handle import IN_PROCESS_NAME
-from dagster.utils import merge_dicts
+from dagster import Field, Float, Noneable, StringSource
+from dagster._core.host_representation import IN_PROCESS_NAME
+from dagster._utils import merge_dicts
 
 CELERY_K8S_CONFIG_KEY = "celery-k8s"
 
 
-def celery_k8s_config():
+def celery_k8s_executor_config():
 
     # DagsterK8sJobConfig provides config schema for specifying Dagster K8s Jobs
-    job_config = DagsterK8sJobConfig.config_type_pipeline_run()
+    job_config = DagsterK8sJobConfig.config_type_job()
 
     additional_config = {
         "load_incluster_config": Field(
             bool,
             is_required=False,
             default_value=True,
             description="""Set this value if you are running the launcher within a k8s cluster. If
@@ -39,42 +40,48 @@
         ),
         "repo_location_name": Field(
             StringSource,
             is_required=False,
             default_value=IN_PROCESS_NAME,
             description="The repository location name to use for execution.",
         ),
+        "job_wait_timeout": Field(
+            Float,
+            is_required=False,
+            default_value=DEFAULT_WAIT_TIMEOUT,
+            description=f"Wait this many seconds for a job to complete before marking the run as failed. Defaults to {DEFAULT_WAIT_TIMEOUT} seconds.",
+        ),
     }
 
     cfg = merge_dicts(CELERY_CONFIG, job_config)
     cfg = merge_dicts(cfg, additional_config)
     return cfg
 
 
-def get_celery_engine_config():
-
-    return {
-        "execution": {
-            CELERY_K8S_CONFIG_KEY: {
-                "config": {
-                    "job_image": {"env": "DAGSTER_K8S_PIPELINE_RUN_IMAGE"},
-                    "job_namespace": {"env": "DAGSTER_K8S_PIPELINE_RUN_NAMESPACE"},
-                    "image_pull_policy": {"env": "DAGSTER_K8S_PIPELINE_RUN_IMAGE_PULL_POLICY"},
-                    "env_config_maps": [{"env": "DAGSTER_K8S_PIPELINE_RUN_ENV_CONFIGMAP"}],
-                }
-            }
-        }
-    }
+def get_celery_engine_config(image_pull_policy=None, additional_env_config_maps=None):
+    job_config = get_celery_engine_job_config(image_pull_policy, additional_env_config_maps)
+    return {"execution": {CELERY_K8S_CONFIG_KEY: {"config": job_config["execution"]["config"]}}}
 
 
-def get_celery_engine_grpc_config():
+def get_celery_engine_job_config(image_pull_policy=None, additional_env_config_maps=None):
     return {
         "execution": {
-            CELERY_K8S_CONFIG_KEY: {
-                "config": {
+            "config": merge_dicts(
+                {
                     "job_namespace": {"env": "DAGSTER_K8S_PIPELINE_RUN_NAMESPACE"},
-                    "image_pull_policy": {"env": "DAGSTER_K8S_PIPELINE_RUN_IMAGE_PULL_POLICY"},
-                    "env_config_maps": [{"env": "DAGSTER_K8S_PIPELINE_RUN_ENV_CONFIGMAP"}],
-                }
-            }
+                    "env_config_maps": (
+                        [
+                            {"env": "DAGSTER_K8S_PIPELINE_RUN_ENV_CONFIGMAP"},
+                        ]
+                        + (additional_env_config_maps if additional_env_config_maps else [])
+                    ),
+                },
+                (
+                    {
+                        "image_pull_policy": image_pull_policy,
+                    }
+                    if image_pull_policy
+                    else {}
+                ),
+            )
         }
     }
```

### Comparing `dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/executor.py` & `dagster-celery-k8s-1.0.5/dagster_celery_k8s/executor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,135 +1,138 @@
+import logging
 import os
+import sys
+import time
 
 import kubernetes
 from dagster_celery.config import DEFAULT_CONFIG, dict_wrapper
 from dagster_celery.core_execution_loop import DELEGATE_MARKER
 from dagster_celery.defaults import broker_url, result_backend
 from dagster_k8s import DagsterK8sJobConfig, construct_dagster_k8s_job
-from dagster_k8s.client import DagsterK8sPipelineStatusException
+from dagster_k8s.client import (
+    DagsterK8sAPIRetryLimitExceeded,
+    DagsterK8sError,
+    DagsterK8sPipelineStatusException,
+    DagsterK8sTimeoutError,
+    DagsterK8sUnrecoverableAPIError,
+)
 from dagster_k8s.job import (
     UserDefinedDagsterK8sConfig,
     get_k8s_job_name,
     get_user_defined_k8s_config,
 )
 from dagster_k8s.utils import (
     delete_job,
-    filter_dagster_events_from_pod_logs,
     get_pod_names_in_job,
     retrieve_pod_logs,
     wait_for_job_success,
 )
 
-from dagster import DagsterInstance, EventMetadataEntry, Executor, check, executor
-from dagster.cli.api import ExecuteStepArgs
-from dagster.core.definitions.executor import check_cross_process_constraints
-from dagster.core.events import EngineEventData
-from dagster.core.execution.retries import Retries
-from dagster.core.instance import InstanceRef
-from dagster.core.origin import PipelineOrigin
-from dagster.core.storage.pipeline_run import PipelineRunStatus
-from dagster.serdes import pack_value, serialize_dagster_namedtuple, unpack_value
+from dagster import DagsterEvent, DagsterEventType, DagsterInstance, Executor, MetadataEntry
+from dagster import _check as check
+from dagster import executor, multiple_process_executor_requirements
+from dagster._cli.api import ExecuteStepArgs
+from dagster._core.errors import DagsterUnmetExecutorRequirementsError
+from dagster._core.events import EngineEventData
+from dagster._core.events.log import EventLogEntry
+from dagster._core.events.utils import filter_dagster_events_from_cli_logs
+from dagster._core.execution.plan.objects import StepFailureData, UserFailureData
+from dagster._core.execution.retries import RetryMode
+from dagster._core.storage.pipeline_run import PipelineRun, PipelineRunStatus
+from dagster._serdes import pack_value, serialize_dagster_namedtuple, unpack_value
+from dagster._utils.error import serializable_error_info_from_exc_info
 
-from .config import CELERY_K8S_CONFIG_KEY, celery_k8s_config
+from .config import CELERY_K8S_CONFIG_KEY, celery_k8s_executor_config
 from .launcher import CeleryK8sRunLauncher
 
 
-@executor(name=CELERY_K8S_CONFIG_KEY, config_schema=celery_k8s_config())
+@executor(
+    name=CELERY_K8S_CONFIG_KEY,
+    config_schema=celery_k8s_executor_config(),
+    requirements=multiple_process_executor_requirements(),
+)
 def celery_k8s_job_executor(init_context):
     """Celery-based executor which launches tasks as Kubernetes Jobs.
 
     The Celery executor exposes config settings for the underlying Celery app under
     the ``config_source`` key. This config corresponds to the "new lowercase settings" introduced
     in Celery version 4.0 and the object constructed from config will be passed to the
     :py:class:`celery.Celery` constructor as its ``config_source`` argument.
-    (See https://docs.celeryproject.org/en/latest/userguide/configuration.html for details.)
+    (See https://docs.celeryq.dev/en/stable/userguide/configuration.html for details.)
 
     The executor also exposes the ``broker``, `backend`, and ``include`` arguments to the
     :py:class:`celery.Celery` constructor.
 
     In the most common case, you may want to modify the ``broker`` and ``backend`` (e.g., to use
     Redis instead of RabbitMQ). We expect that ``config_source`` will be less frequently
-    modified, but that when solid executions are especially fast or slow, or when there are
-    different requirements around idempotence or retry, it may make sense to execute pipelines
+    modified, but that when op executions are especially fast or slow, or when there are
+    different requirements around idempotence or retry, it may make sense to execute dagster jobs
     with variations on these settings.
 
-    If you'd like to configure a Celery Kubernetes Job executor in addition to the
-    :py:class:`~dagster.default_executors`, you should add it to the ``executor_defs`` defined on a
-    :py:class:`~dagster.ModeDefinition` as follows:
+    To use the `celery_k8s_job_executor`, set it as the `executor_def` when defining a job:
 
-    .. literalinclude:: ../dagster_celery_k8s_tests/example_celery_mode_def.py
+    .. literalinclude:: ../../../../../../python_modules/libraries/dagster-celery-k8s/dagster_celery_k8s_tests/example_celery_mode_def.py
        :language: python
 
     Then you can configure the executor as follows:
 
     .. code-block:: YAML
 
         execution:
-          celery-k8s:
-            config:
-              job_image: 'my_repo.com/image_name:latest'
-              job_namespace: 'some-namespace'
-              broker: 'pyamqp://guest@localhost//'  # Optional[str]: The URL of the Celery broker
-              backend: 'rpc://' # Optional[str]: The URL of the Celery results backend
-              include: ['my_module'] # Optional[List[str]]: Modules every worker should import
-              config_source: # Dict[str, Any]: Any additional parameters to pass to the
-                  #...       # Celery workers. This dict will be passed as the `config_source`
-                  #...       # argument of celery.Celery().
+          config:
+            job_image: 'my_repo.com/image_name:latest'
+            job_namespace: 'some-namespace'
+            broker: 'pyamqp://guest@localhost//'  # Optional[str]: The URL of the Celery broker
+            backend: 'rpc://' # Optional[str]: The URL of the Celery results backend
+            include: ['my_module'] # Optional[List[str]]: Modules every worker should import
+            config_source: # Dict[str, Any]: Any additional parameters to pass to the
+                #...       # Celery workers. This dict will be passed as the `config_source`
+                #...       # argument of celery.Celery().
 
     Note that the YAML you provide here must align with the configuration with which the Celery
     workers on which you hope to run were started. If, for example, you point the executor at a
     different broker than the one your workers are listening to, the workers will never be able to
     pick up tasks for execution.
 
     In deployments where the celery_k8s_job_executor is used all appropriate celery and dagster_celery
     commands must be invoked with the `-A dagster_celery_k8s.app` argument.
     """
 
-    check_cross_process_constraints(init_context)
-
     run_launcher = init_context.instance.run_launcher
     exc_cfg = init_context.executor_config
 
-    check.inst(
-        run_launcher,
-        CeleryK8sRunLauncher,
-        "This engine is only compatible with a CeleryK8sRunLauncher; configure the "
-        "CeleryK8sRunLauncher on your instance to use it.",
-    )
+    if not isinstance(run_launcher, CeleryK8sRunLauncher):
+        raise DagsterUnmetExecutorRequirementsError(
+            "This engine is only compatible with a CeleryK8sRunLauncher; configure the "
+            "CeleryK8sRunLauncher on your instance to use it.",
+        )
 
-    job_config = DagsterK8sJobConfig(
-        dagster_home=run_launcher.dagster_home,
-        instance_config_map=run_launcher.instance_config_map,
-        postgres_password_secret=run_launcher.postgres_password_secret,
-        job_image=exc_cfg.get("job_image") or os.getenv("DAGSTER_CURRENT_IMAGE"),
-        image_pull_policy=exc_cfg.get("image_pull_policy"),
-        image_pull_secrets=exc_cfg.get("image_pull_secrets"),
-        service_account_name=exc_cfg.get("service_account_name"),
-        env_config_maps=exc_cfg.get("env_config_maps"),
-        env_secrets=exc_cfg.get("env_secrets"),
+    job_config = run_launcher.get_k8s_job_config(
+        job_image=exc_cfg.get("job_image") or os.getenv("DAGSTER_CURRENT_IMAGE"), exc_config=exc_cfg
     )
 
     # Set on the instance but overrideable here
     broker = run_launcher.broker or exc_cfg.get("broker")
     backend = run_launcher.backend or exc_cfg.get("backend")
     config_source = run_launcher.config_source or exc_cfg.get("config_source")
     include = run_launcher.include or exc_cfg.get("include")
-    retries = run_launcher.retries or Retries.from_config(exc_cfg.get("retries"))
+    retries = run_launcher.retries or RetryMode.from_config(exc_cfg.get("retries"))
 
     return CeleryK8sJobExecutor(
         broker=broker,
         backend=backend,
         config_source=config_source,
         include=include,
         retries=retries,
         job_config=job_config,
         job_namespace=exc_cfg.get("job_namespace"),
         load_incluster_config=exc_cfg.get("load_incluster_config"),
         kubeconfig_file=exc_cfg.get("kubeconfig_file"),
         repo_location_name=exc_cfg.get("repo_location_name"),
+        job_wait_timeout=exc_cfg.get("job_wait_timeout"),
     )
 
 
 class CeleryK8sJobExecutor(Executor):
     def __init__(
         self,
         retries,
@@ -138,369 +141,406 @@
         include=None,
         config_source=None,
         job_config=None,
         job_namespace=None,
         load_incluster_config=False,
         kubeconfig_file=None,
         repo_location_name=None,
+        job_wait_timeout=None,
     ):
 
         if load_incluster_config:
             check.invariant(
                 kubeconfig_file is None,
                 "`kubeconfig_file` is set but `load_incluster_config` is True.",
             )
         else:
             check.opt_str_param(kubeconfig_file, "kubeconfig_file")
 
-        self._retries = check.inst_param(retries, "retries", Retries)
+        self._retries = check.inst_param(retries, "retries", RetryMode)
         self.broker = check.opt_str_param(broker, "broker", default=broker_url)
         self.backend = check.opt_str_param(backend, "backend", default=result_backend)
         self.include = check.opt_list_param(include, "include", of_type=str)
         self.config_source = dict_wrapper(
             dict(DEFAULT_CONFIG, **check.opt_dict_param(config_source, "config_source"))
         )
         self.job_config = check.inst_param(job_config, "job_config", DagsterK8sJobConfig)
         self.job_namespace = check.opt_str_param(job_namespace, "job_namespace", default="default")
 
         self.load_incluster_config = check.bool_param(
             load_incluster_config, "load_incluster_config"
         )
 
         self.kubeconfig_file = check.opt_str_param(kubeconfig_file, "kubeconfig_file")
-        self.repo_location_name = check.str_param(repo_location_name, "repo_location_name")
+        self.repo_location_name = check.opt_str_param(repo_location_name, "repo_location_name")
+        self.job_wait_timeout = check.float_param(job_wait_timeout, "job_wait_timeout")
 
     @property
     def retries(self):
         return self._retries
 
-    def execute(self, pipeline_context, execution_plan):
+    def execute(self, plan_context, execution_plan):
         from dagster_celery.core_execution_loop import core_celery_execution_loop
 
         return core_celery_execution_loop(
-            pipeline_context, execution_plan, step_execution_fn=_submit_task_k8s_job
+            plan_context, execution_plan, step_execution_fn=_submit_task_k8s_job
         )
 
     def app_args(self):
         return {
             "broker": self.broker,
             "backend": self.backend,
             "include": self.include,
             "config_source": self.config_source,
             "retries": self.retries,
         }
 
 
-def _submit_task_k8s_job(app, pipeline_context, step, queue, priority):
+def _submit_task_k8s_job(app, plan_context, step, queue, priority, known_state):
     user_defined_k8s_config = get_user_defined_k8s_config(step.tags)
 
-    task = create_k8s_job_task(app)
+    pipeline_origin = plan_context.reconstructable_pipeline.get_python_origin()
+
+    execute_step_args = ExecuteStepArgs(
+        pipeline_origin=pipeline_origin,
+        pipeline_run_id=plan_context.pipeline_run.run_id,
+        step_keys_to_execute=[step.key],
+        instance_ref=plan_context.instance.get_ref(),
+        retry_mode=plan_context.executor.retries.for_inner_plan(),
+        known_state=known_state,
+        should_verify_step=True,
+    )
 
-    recon_repo = pipeline_context.pipeline.get_reconstructable_repository()
+    job_config = plan_context.executor.job_config
+    if not job_config.job_image:
+        job_config = job_config.with_image(pipeline_origin.repository_origin.container_image)
 
+    if not job_config.job_image:
+        raise Exception("No image included in either executor config or the dagster job")
+
+    task = create_k8s_job_task(app)
     task_signature = task.si(
-        instance_ref_dict=pipeline_context.instance.get_ref().to_dict(),
-        step_keys=[step.key],
-        run_config=pipeline_context.pipeline_run.run_config,
-        mode=pipeline_context.pipeline_run.mode,
-        repo_name=recon_repo.get_definition().name,
-        repo_location_name=pipeline_context.executor.repo_location_name,
-        run_id=pipeline_context.pipeline_run.run_id,
-        job_config_dict=pipeline_context.executor.job_config.to_dict(),
-        job_namespace=pipeline_context.executor.job_namespace,
+        execute_step_args_packed=pack_value(execute_step_args),
+        job_config_dict=job_config.to_dict(),
+        job_namespace=plan_context.executor.job_namespace,
         user_defined_k8s_config_dict=user_defined_k8s_config.to_dict(),
-        retries_dict=pipeline_context.executor.retries.for_inner_plan().to_config(),
-        pipeline_origin_packed=pack_value(pipeline_context.pipeline.get_origin()),
-        load_incluster_config=pipeline_context.executor.load_incluster_config,
-        kubeconfig_file=pipeline_context.executor.kubeconfig_file,
+        load_incluster_config=plan_context.executor.load_incluster_config,
+        job_wait_timeout=plan_context.executor.job_wait_timeout,
+        kubeconfig_file=plan_context.executor.kubeconfig_file,
     )
 
     return task_signature.apply_async(
         priority=priority,
         queue=queue,
         routing_key="{queue}.execute_step_k8s_job".format(queue=queue),
     )
 
 
+def construct_step_failure_event_and_handle(pipeline_run, step_key, err, instance):
+    step_failure_event = DagsterEvent(
+        event_type_value=DagsterEventType.STEP_FAILURE.value,
+        pipeline_name=pipeline_run.pipeline_name,
+        step_key=step_key,
+        event_specific_data=StepFailureData(
+            error=serializable_error_info_from_exc_info(sys.exc_info()),
+            user_failure_data=UserFailureData(label="K8sError"),
+        ),
+    )
+    event_record = EventLogEntry(
+        user_message=str(err),
+        level=logging.ERROR,
+        pipeline_name=pipeline_run.pipeline_name,
+        run_id=pipeline_run.run_id,
+        error_info=None,
+        step_key=step_key,
+        timestamp=time.time(),
+        dagster_event=step_failure_event,
+    )
+    instance.handle_new_event(event_record)
+    return step_failure_event
+
+
 def create_k8s_job_task(celery_app, **task_kwargs):
     @celery_app.task(bind=True, name="execute_step_k8s_job", **task_kwargs)
     def _execute_step_k8s_job(
         self,
-        instance_ref_dict,
-        step_keys,
-        run_config,
-        mode,
-        repo_name,
-        repo_location_name,
-        run_id,
+        execute_step_args_packed,
         job_config_dict,
         job_namespace,
         load_incluster_config,
-        retries_dict,
-        pipeline_origin_packed,
+        job_wait_timeout,
         user_defined_k8s_config_dict=None,
         kubeconfig_file=None,
     ):
-        """Run step execution in a K8s job pod.
-        """
-
-        check.dict_param(instance_ref_dict, "instance_ref_dict")
-        check.list_param(step_keys, "step_keys", of_type=str)
+        """Run step execution in a K8s job pod."""
+        execute_step_args = unpack_value(
+            check.dict_param(
+                execute_step_args_packed,
+                "execute_step_args_packed",
+            )
+        )
+        check.inst_param(execute_step_args, "execute_step_args", ExecuteStepArgs)
         check.invariant(
-            len(step_keys) == 1, "Celery K8s task executor can only execute 1 step at a time"
+            len(execute_step_args.step_keys_to_execute) == 1,
+            "Celery K8s task executor can only execute 1 step at a time",
         )
-        check.dict_param(run_config, "run_config")
-        check.str_param(mode, "mode")
-        check.str_param(repo_name, "repo_name")
-        check.str_param(repo_location_name, "repo_location_name")
-        check.str_param(run_id, "run_id")
 
         # Celery will serialize this as a list
         job_config = DagsterK8sJobConfig.from_dict(job_config_dict)
         check.inst_param(job_config, "job_config", DagsterK8sJobConfig)
         check.str_param(job_namespace, "job_namespace")
 
         check.bool_param(load_incluster_config, "load_incluster_config")
-        check.dict_param(retries_dict, "retries_dict")
-
-        pipeline_origin = unpack_value(
-            check.dict_param(
-                pipeline_origin_packed, "pipeline_origin_packed"
-            )  # TODO: make part of args
-        )
-        check.inst(pipeline_origin, PipelineOrigin)
 
         user_defined_k8s_config = UserDefinedDagsterK8sConfig.from_dict(
             user_defined_k8s_config_dict
         )
         check.opt_inst_param(
-            user_defined_k8s_config, "user_defined_k8s_config", UserDefinedDagsterK8sConfig,
+            user_defined_k8s_config,
+            "user_defined_k8s_config",
+            UserDefinedDagsterK8sConfig,
         )
         check.opt_str_param(kubeconfig_file, "kubeconfig_file")
 
         # For when launched via DinD or running the cluster
         if load_incluster_config:
             kubernetes.config.load_incluster_config()
         else:
             kubernetes.config.load_kube_config(kubeconfig_file)
 
-        instance_ref = InstanceRef.from_dict(instance_ref_dict)
-        instance = DagsterInstance.from_ref(instance_ref)
-        pipeline_run = instance.get_run_by_id(run_id)
+        instance = DagsterInstance.from_ref(execute_step_args.instance_ref)
+        pipeline_run = instance.get_run_by_id(execute_step_args.pipeline_run_id)
 
-        check.invariant(pipeline_run, "Could not load run {}".format(run_id))
-        step_key = step_keys[0]
+        check.inst(
+            pipeline_run,
+            PipelineRun,
+            "Could not load run {}".format(execute_step_args.pipeline_run_id),
+        )
+        step_key = execute_step_args.step_keys_to_execute[0]
 
         celery_worker_name = self.request.hostname
         celery_pod_name = os.environ.get("HOSTNAME")
         instance.report_engine_event(
             "Task for step {step_key} picked up by Celery".format(step_key=step_key),
             pipeline_run,
             EngineEventData(
                 [
-                    EventMetadataEntry.text(celery_worker_name, "Celery worker name"),
-                    EventMetadataEntry.text(celery_pod_name, "Celery worker Kubernetes Pod name"),
+                    MetadataEntry("Celery worker name", value=celery_worker_name),
+                    MetadataEntry("Celery worker Kubernetes Pod name", value=celery_pod_name),
                 ]
             ),
             CeleryK8sJobExecutor,
             step_key=step_key,
         )
 
         if pipeline_run.status != PipelineRunStatus.STARTED:
             instance.report_engine_event(
-                "Not scheduling step because pipeline run status is not STARTED",
+                "Not scheduling step because dagster run status is not STARTED",
                 pipeline_run,
-                EngineEventData([EventMetadataEntry.text(step_key, "Step key"),]),
+                EngineEventData(
+                    [
+                        MetadataEntry("Step key", value=step_key),
+                    ]
+                ),
                 CeleryK8sJobExecutor,
                 step_key=step_key,
             )
-            return
+            return []
 
         # Ensure we stay below k8s name length limits
-        k8s_name_key = get_k8s_job_name(run_id, step_key)
+        k8s_name_key = get_k8s_job_name(execute_step_args.pipeline_run_id, step_key)
 
-        retries = Retries.from_config(retries_dict)
+        retry_state = execute_step_args.known_state.get_retry_state()
 
-        if retries.get_attempt_count(step_key):
-            attempt_number = retries.get_attempt_count(step_key)
-            job_name = "dagster-job-%s-%d" % (k8s_name_key, attempt_number)
-            pod_name = "dagster-job-%s-%d" % (k8s_name_key, attempt_number)
+        if retry_state.get_attempt_count(step_key):
+            attempt_number = retry_state.get_attempt_count(step_key)
+            job_name = "dagster-step-%s-%d" % (k8s_name_key, attempt_number)
+            pod_name = "dagster-step-%s-%d" % (k8s_name_key, attempt_number)
         else:
-            job_name = "dagster-job-%s" % (k8s_name_key)
-            pod_name = "dagster-job-%s" % (k8s_name_key)
+            job_name = "dagster-step-%s" % (k8s_name_key)
+            pod_name = "dagster-step-%s" % (k8s_name_key)
 
-        input_json = serialize_dagster_namedtuple(
-            ExecuteStepArgs(
-                pipeline_origin=pipeline_origin,
-                pipeline_run_id=run_id,
-                instance_ref=None,
-                mode=mode,
-                step_keys_to_execute=step_keys,
-                run_config=run_config,
-                retries_dict=retries_dict,
-            )
-        )
-        command = ["dagster"]
-        args = ["api", "execute_step_with_structured_logs", input_json]
+        args = execute_step_args.get_command_args()
 
         job = construct_dagster_k8s_job(
-            job_config, command, args, job_name, user_defined_k8s_config, pod_name
+            job_config,
+            args,
+            job_name,
+            user_defined_k8s_config,
+            pod_name,
+            component="step_worker",
+            labels={
+                "dagster/job": pipeline_run.pipeline_name,
+                "dagster/op": step_key,
+                "dagster/run-id": execute_step_args.pipeline_run_id,
+            },
         )
 
         # Running list of events generated from this task execution
         events = []
 
         # Post event for starting execution
         job_name = job.metadata.name
         engine_event = instance.report_engine_event(
-            "Executing step {} in Kubernetes job {}".format(step_key, job_name),
+            'Executing step "{}" in Kubernetes job {}.'.format(step_key, job_name),
             pipeline_run,
             EngineEventData(
                 [
-                    EventMetadataEntry.text(step_key, "Step key"),
-                    EventMetadataEntry.text(job_name, "Kubernetes Job name"),
-                    EventMetadataEntry.text(pod_name, "Kubernetes Pod name"),
-                    EventMetadataEntry.text(job_config.job_image, "Job image"),
-                    EventMetadataEntry.text(job_config.image_pull_policy, "Image pull policy"),
-                    EventMetadataEntry.text(
-                        str(job_config.image_pull_secrets), "Image pull secrets"
-                    ),
-                    EventMetadataEntry.text(
-                        str(job_config.service_account_name), "Service account name"
+                    MetadataEntry("Step key", value=step_key),
+                    MetadataEntry("Kubernetes Job name", value=job_name),
+                    MetadataEntry("Job image", value=job_config.job_image),
+                    MetadataEntry("Image pull policy", value=job_config.image_pull_policy),
+                    MetadataEntry("Image pull secrets", value=str(job_config.image_pull_secrets)),
+                    MetadataEntry(
+                        "Service account name", value=str(job_config.service_account_name)
                     ),
                 ],
                 marker_end=DELEGATE_MARKER,
             ),
             CeleryK8sJobExecutor,
             # validated above that step_keys is length 1, and it is not possible to use ETH or
             # execution plan in this function (Celery K8s workers should not access to user code)
             step_key=step_key,
         )
         events.append(engine_event)
-
         try:
             kubernetes.client.BatchV1Api().create_namespaced_job(body=job, namespace=job_namespace)
         except kubernetes.client.rest.ApiException as e:
             if e.reason == "Conflict":
-                # There is an existing job with the same name so do not procede.
+                # There is an existing job with the same name so proceed and see if the existing job succeeded
                 instance.report_engine_event(
                     "Did not create Kubernetes job {} for step {} since job name already "
-                    "exists, exiting.".format(job_name, step_key),
+                    "exists, proceeding with existing job.".format(job_name, step_key),
                     pipeline_run,
                     EngineEventData(
                         [
-                            EventMetadataEntry.text(step_key, "Step key"),
-                            EventMetadataEntry.text(job_name, "Kubernetes Job name"),
-                            EventMetadataEntry.text(pod_name, "Kubernetes Pod name"),
+                            MetadataEntry("Step key", value=step_key),
+                            MetadataEntry("Kubernetes Job name", value=job_name),
                         ],
                         marker_end=DELEGATE_MARKER,
                     ),
                     CeleryK8sJobExecutor,
                     step_key=step_key,
                 )
             else:
                 instance.report_engine_event(
                     "Encountered unexpected error while creating Kubernetes job {} for step {}, "
                     "exiting.".format(job_name, step_key),
                     pipeline_run,
                     EngineEventData(
                         [
-                            EventMetadataEntry.text(step_key, "Step key"),
-                            EventMetadataEntry.text(str(e), "Error"),
-                        ]
+                            MetadataEntry("Step key", value=step_key),
+                        ],
+                        error=serializable_error_info_from_exc_info(sys.exc_info()),
                     ),
                     CeleryK8sJobExecutor,
                     step_key=step_key,
                 )
-            return
+                return []
 
         try:
             wait_for_job_success(
-                job_name=job_name, namespace=job_namespace, instance=instance, run_id=run_id,
+                job_name=job_name,
+                namespace=job_namespace,
+                instance=instance,
+                run_id=execute_step_args.pipeline_run_id,
+                wait_timeout=job_wait_timeout,
             )
+        except (DagsterK8sError, DagsterK8sTimeoutError) as err:
+            step_failure_event = construct_step_failure_event_and_handle(
+                pipeline_run, step_key, err, instance=instance
+            )
+            events.append(step_failure_event)
         except DagsterK8sPipelineStatusException:
             instance.report_engine_event(
-                "Terminating Kubernetes Job because pipeline run status is not STARTED",
+                "Terminating Kubernetes Job because dagster run status is not STARTED",
                 pipeline_run,
                 EngineEventData(
                     [
-                        EventMetadataEntry.text(step_key, "Step key"),
-                        EventMetadataEntry.text(job_name, "Kubernetes Job name"),
-                        EventMetadataEntry.text(job_namespace, "Kubernetes Job namespace"),
+                        MetadataEntry("Step key", value=step_key),
+                        MetadataEntry("Kubernetes Job name", value=job_name),
+                        MetadataEntry("Kubernetes Job namespace", value=job_namespace),
                     ]
                 ),
                 CeleryK8sJobExecutor,
                 step_key=step_key,
             )
             delete_job(job_name=job_name, namespace=job_namespace)
-            return
-        except kubernetes.client.rest.ApiException as e:
+            return []
+        except (
+            DagsterK8sUnrecoverableAPIError,
+            DagsterK8sAPIRetryLimitExceeded,
+            # We shouldn't see unwrapped APIExceptions anymore, as they should all be wrapped in
+            # a retry boundary. We still catch it here just in case we missed one so that we can
+            # report it to the event log
+            kubernetes.client.rest.ApiException,
+        ):
             instance.report_engine_event(
                 "Encountered unexpected error while waiting on Kubernetes job {} for step {}, "
                 "exiting.".format(job_name, step_key),
                 pipeline_run,
                 EngineEventData(
                     [
-                        EventMetadataEntry.text(step_key, "Step key"),
-                        EventMetadataEntry.text(str(e), "Error"),
-                    ]
+                        MetadataEntry("Step key", value=step_key),
+                    ],
+                    error=serializable_error_info_from_exc_info(sys.exc_info()),
                 ),
                 CeleryK8sJobExecutor,
                 step_key=step_key,
             )
-            return
+            return []
 
         try:
             pod_names = get_pod_names_in_job(job_name, namespace=job_namespace)
-        except kubernetes.client.rest.ApiException as e:
+        except kubernetes.client.rest.ApiException:
             instance.report_engine_event(
                 "Encountered unexpected error retreiving Pods for Kubernetes job {} for step {}, "
                 "exiting.".format(job_name, step_key),
                 pipeline_run,
                 EngineEventData(
                     [
-                        EventMetadataEntry.text(step_key, "Step key"),
-                        EventMetadataEntry.text(str(e), "Error"),
-                    ]
+                        MetadataEntry("Step key", value=step_key),
+                    ],
+                    error=serializable_error_info_from_exc_info(sys.exc_info()),
                 ),
                 CeleryK8sJobExecutor,
                 step_key=step_key,
             )
-            return
+            return []
 
         # Post engine event for log retrieval
         engine_event = instance.report_engine_event(
             "Retrieving logs from Kubernetes Job pods",
             pipeline_run,
-            EngineEventData([EventMetadataEntry.text("\n".join(pod_names), "Pod names")]),
+            EngineEventData([MetadataEntry("Pod names", value="\n".join(pod_names))]),
             CeleryK8sJobExecutor,
             step_key=step_key,
         )
         events.append(engine_event)
 
         logs = []
         for pod_name in pod_names:
             try:
                 raw_logs = retrieve_pod_logs(pod_name, namespace=job_namespace)
                 logs += raw_logs.split("\n")
-            except kubernetes.client.rest.ApiException as e:
+            except kubernetes.client.rest.ApiException:
                 instance.report_engine_event(
                     "Encountered unexpected error while fetching pod logs for Kubernetes job {}, "
                     "Pod name {} for step {}. Will attempt to continue with other pods.".format(
                         job_name, pod_name, step_key
                     ),
                     pipeline_run,
                     EngineEventData(
                         [
-                            EventMetadataEntry.text(step_key, "Step key"),
-                            EventMetadataEntry.text(str(e), "Error"),
-                        ]
+                            MetadataEntry("Step key", value=step_key),
+                        ],
+                        error=serializable_error_info_from_exc_info(sys.exc_info()),
                     ),
                     CeleryK8sJobExecutor,
                     step_key=step_key,
                 )
 
-        events += filter_dagster_events_from_pod_logs(logs)
+        events += filter_dagster_events_from_cli_logs(logs)
         serialized_events = [serialize_dagster_namedtuple(event) for event in events]
         return serialized_events
 
     return _execute_step_k8s_job
```

### Comparing `dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/launcher.py` & `dagster-celery-k8s-1.0.5/dagster_celery_k8s/launcher.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,64 @@
-import weakref
+import sys
+from typing import cast
 
 import kubernetes
 from dagster_k8s.job import (
     DagsterK8sJobConfig,
     construct_dagster_k8s_job,
     get_job_name_from_run_id,
     get_user_defined_k8s_config,
 )
 from dagster_k8s.utils import delete_job
 
-from dagster import DagsterInvariantViolationError, EventMetadataEntry, Field, Noneable, check
-from dagster.config.field import resolve_to_config_type
-from dagster.config.validate import process_config
-from dagster.core.events import EngineEventData
-from dagster.core.execution.retries import Retries
-from dagster.core.host_representation import ExternalPipeline
-from dagster.core.host_representation.handle import GrpcServerRepositoryLocationHandle
-from dagster.core.instance import DagsterInstance
-from dagster.core.launcher import RunLauncher
-from dagster.core.origin import PipelineGrpcServerOrigin, PipelinePythonOrigin
-from dagster.core.storage.pipeline_run import PipelineRun, PipelineRunStatus
-from dagster.serdes import ConfigurableClass, ConfigurableClassData, serialize_dagster_namedtuple
-from dagster.utils import frozentags, merge_dicts
+from dagster import DagsterInvariantViolationError, MetadataEntry
+from dagster import _check as check
+from dagster._config import process_config, resolve_to_config_type
+from dagster._core.events import EngineEventData
+from dagster._core.execution.retries import RetryMode
+from dagster._core.launcher import LaunchRunContext, RunLauncher
+from dagster._core.launcher.base import CheckRunHealthResult, WorkerStatus
+from dagster._core.origin import PipelinePythonOrigin
+from dagster._core.storage.pipeline_run import PipelineRun, PipelineRunStatus
+from dagster._core.storage.tags import DOCKER_IMAGE_TAG
+from dagster._serdes import ConfigurableClass, ConfigurableClassData
+from dagster._utils import frozentags, merge_dicts
+from dagster._utils.error import serializable_error_info_from_exc_info
 
-from .config import CELERY_K8S_CONFIG_KEY, celery_k8s_config
+from .config import CELERY_K8S_CONFIG_KEY, celery_k8s_executor_config
 
 
 class CeleryK8sRunLauncher(RunLauncher, ConfigurableClass):
-    """In contrast to the :py:class:`K8sRunLauncher`, which launches pipeline runs as single K8s
+    """In contrast to the :py:class:`K8sRunLauncher`, which launches dagster runs as single K8s
     Jobs, this run launcher is intended for use in concert with
     :py:func:`dagster_celery_k8s.celery_k8s_job_executor`.
 
     With this run launcher, execution is delegated to:
 
-        1. A run coordinator Kubernetes Job, which traverses the pipeline run execution plan and
+        1. A run worker Kubernetes Job, which traverses the dagster run execution plan and
            submits steps to Celery queues for execution;
         2. The step executions which are submitted to Celery queues are picked up by Celery workers,
            and each step execution spawns a step execution Kubernetes Job. See the implementation
            defined in :py:func:`dagster_celery_k8.executor.create_k8s_job_task`.
 
-    You may configure a Dagster instance to use this RunLauncher by adding a section to your
+    You can configure a Dagster instance to use this RunLauncher by adding a section to your
     ``dagster.yaml`` like the following:
 
     .. code-block:: yaml
 
         run_launcher:
           module: dagster_k8s.launcher
           class: CeleryK8sRunLauncher
           config:
             instance_config_map: "dagster-k8s-instance-config-map"
             dagster_home: "/some/path"
             postgres_password_secret: "dagster-k8s-pg-password"
             broker: "some_celery_broker_url"
             backend: "some_celery_backend_url"
 
-    As always when using a :py:class:`~dagster.serdes.ConfigurableClass`, the values
-    under the ``config`` key of this YAML block will be passed to the constructor. The full list
-    of acceptable values is given below by the constructor args.
-
-    Args:
-        instance_config_map (str): The ``name`` of an existing Volume to mount into the pod in
-            order to provide a ConfigMap for the Dagster instance. This Volume should contain a
-            ``dagster.yaml`` with appropriate values for run storage, event log storage, etc.
-        dagster_home (str): The location of DAGSTER_HOME in the Job container; this is where the
-            ``dagster.yaml`` file will be mounted from the instance ConfigMap specified above.
-        postgres_password_secret (str): The name of the Kubernetes Secret where the postgres
-            password can be retrieved. Will be mounted and supplied as an environment variable to
-            the Job Pod.
-        load_incluster_config (Optional[bool]):  Set this value if you are running the launcher
-            within a k8s cluster. If ``True``, we assume the launcher is running within the target
-            cluster and load config using ``kubernetes.config.load_incluster_config``. Otherwise,
-            we will use the k8s config specified in ``kubeconfig_file`` (using
-            ``kubernetes.config.load_kube_config``) or fall back to the default kubeconfig. Default:
-            ``True``.
-        kubeconfig_file (Optional[str]): The kubeconfig file from which to load config. Defaults to
-            None (using the default kubeconfig).
-        broker (Optional[str]): The URL of the Celery broker.
-        backend (Optional[str]): The URL of the Celery backend.
-        include (List[str]): List of includes for the Celery workers
-        config_source: (Optional[dict]): Additional settings for the Celery app.
-        retries: (Optional[dict]): Default retry configuration for Celery tasks.
     """
 
     def __init__(
         self,
         instance_config_map,
         dagster_home,
         postgres_password_secret,
@@ -91,179 +66,207 @@
         kubeconfig_file=None,
         broker=None,
         backend=None,
         include=None,
         config_source=None,
         retries=None,
         inst_data=None,
+        k8s_client_batch_api=None,
+        env_config_maps=None,
+        env_secrets=None,
+        volume_mounts=None,
+        volumes=None,
+        service_account_name=None,
+        image_pull_policy=None,
+        image_pull_secrets=None,
+        labels=None,
+        fail_pod_on_run_failure=None,
     ):
         self._inst_data = check.opt_inst_param(inst_data, "inst_data", ConfigurableClassData)
 
         if load_incluster_config:
             check.invariant(
                 kubeconfig_file is None,
                 "`kubeconfig_file` is set but `load_incluster_config` is True.",
             )
             kubernetes.config.load_incluster_config()
         else:
             check.opt_str_param(kubeconfig_file, "kubeconfig_file")
             kubernetes.config.load_kube_config(kubeconfig_file)
 
+        self._fixed_batch_api = k8s_client_batch_api
+
         self.instance_config_map = check.str_param(instance_config_map, "instance_config_map")
         self.dagster_home = check.str_param(dagster_home, "dagster_home")
         self.postgres_password_secret = check.str_param(
             postgres_password_secret, "postgres_password_secret"
         )
         self.broker = check.opt_str_param(broker, "broker")
         self.backend = check.opt_str_param(backend, "backend")
         self.include = check.opt_list_param(include, "include")
         self.config_source = check.opt_dict_param(config_source, "config_source")
 
         retries = check.opt_dict_param(retries, "retries") or {"enabled": {}}
-        self.retries = Retries.from_config(retries)
-        self._instance_ref = None
+        self.retries = RetryMode.from_config(retries)
+
+        self._env_config_maps = check.opt_list_param(
+            env_config_maps, "env_config_maps", of_type=str
+        )
+        self._env_secrets = check.opt_list_param(env_secrets, "env_secrets", of_type=str)
+
+        self._volume_mounts = check.opt_list_param(volume_mounts, "volume_mounts")
+        self._volumes = check.opt_list_param(volumes, "volumes")
+
+        self._service_account_name = check.opt_str_param(
+            service_account_name, "service_account_name"
+        )
+        self._image_pull_policy = check.opt_str_param(
+            image_pull_policy, "image_pull_policy", "IfNotPresent"
+        )
+        self._image_pull_secrets = check.opt_list_param(
+            image_pull_secrets, "image_pull_secrets", of_type=dict
+        )
+        self._labels = check.opt_dict_param(labels, "labels", key_type=str, value_type=str)
+        self._fail_pod_on_run_failure = check.opt_bool_param(
+            fail_pod_on_run_failure, "fail_pod_on_run_failure"
+        )
+
+        super().__init__()
+
+    @property
+    def _batch_api(self):
+        return self._fixed_batch_api if self._fixed_batch_api else kubernetes.client.BatchV1Api()
 
     @classmethod
     def config_type(cls):
-        """Include all arguments required for DagsterK8sJobConfig along with additional arguments
-        needed for the RunLauncher itself.
-        """
         from dagster_celery.executor import CELERY_CONFIG
 
-        job_cfg = DagsterK8sJobConfig.config_type_run_launcher()
-
-        run_launcher_extra_cfg = {
-            "load_incluster_config": Field(bool, is_required=False, default_value=True),
-            "kubeconfig_file": Field(Noneable(str), is_required=False, default_value=None),
-        }
-
-        res = merge_dicts(job_cfg, run_launcher_extra_cfg)
-        return merge_dicts(res, CELERY_CONFIG)
+        return merge_dicts(DagsterK8sJobConfig.config_type_run_launcher(), CELERY_CONFIG)
 
     @classmethod
     def from_config_value(cls, inst_data, config_value):
         return cls(inst_data=inst_data, **config_value)
 
     @property
     def inst_data(self):
         return self._inst_data
 
-    @property
-    def _instance(self):
-        return self._instance_ref() if self._instance_ref else None
-
-    def initialize(self, instance):
-        check.inst_param(instance, "instance", DagsterInstance)
-        # Store a weakref to avoid a circular reference / enable GC
-        self._instance_ref = weakref.ref(instance)
-
-    def launch_run(self, instance, run, external_pipeline):
-        check.inst_param(instance, "instance", DagsterInstance)
-        check.inst_param(run, "run", PipelineRun)
-        check.inst_param(external_pipeline, "external_pipeline", ExternalPipeline)
+    def launch_run(self, context: LaunchRunContext) -> None:
+        run = context.pipeline_run
 
         job_name = get_job_name_from_run_id(run.run_id)
         pod_name = job_name
         exc_config = _get_validated_celery_k8s_executor_config(run.run_config)
 
-        job_image = None
-        pipeline_origin = None
-        env_vars = None
-        if isinstance(external_pipeline.get_origin(), PipelineGrpcServerOrigin):
-            if exc_config.get("job_image"):
-                raise DagsterInvariantViolationError(
-                    "Cannot specify job_image in executor config when loading pipeline "
-                    "from GRPC server."
-                )
-
-            repository_location_handle = (
-                external_pipeline.repository_handle.repository_location_handle
-            )
+        job_image_from_executor_config = exc_config.get("job_image")
 
-            if not isinstance(repository_location_handle, GrpcServerRepositoryLocationHandle):
-                raise DagsterInvariantViolationError(
-                    "Expected RepositoryLocationHandle to be of type "
-                    "GrpcServerRepositoryLocationHandle but found type {}".format(
-                        type(repository_location_handle)
-                    )
-                )
+        pipeline_origin = cast(PipelinePythonOrigin, context.pipeline_code_origin)
+        repository_origin = pipeline_origin.repository_origin
 
-            job_image = repository_location_handle.get_current_image()
-            env_vars = {"DAGSTER_CURRENT_IMAGE": job_image}
-
-            repository_name = external_pipeline.repository_handle.repository_name
-            pipeline_origin = PipelinePythonOrigin(
-                pipeline_name=external_pipeline.name,
-                repository_origin=repository_location_handle.get_repository_python_origin(
-                    repository_name
-                ),
-            )
+        job_image = repository_origin.container_image
 
+        if job_image:
+            if job_image_from_executor_config:
+                job_image = job_image_from_executor_config
+                self._instance.report_engine_event(
+                    f"You have specified a job_image {job_image_from_executor_config} in your executor configuration, "
+                    f"but also {job_image} in your user-code deployment. Using the job image {job_image_from_executor_config} "
+                    f"from executor configuration as it takes precedence.",
+                    run,
+                    cls=self.__class__,
+                )
         else:
-            job_image = exc_config.get("job_image")
-            if not job_image:
+            if not job_image_from_executor_config:
                 raise DagsterInvariantViolationError(
-                    "Cannot find job_image in celery-k8s executor config."
+                    "You have not specified a job_image in your executor configuration. "
+                    "To resolve this error, specify the job_image configuration in the executor "
+                    "config section in your run config. \n"
+                    "Note: You may also be seeing this error because you are using the configured API. "
+                    "Using configured with the celery-k8s executor is not supported at this time, "
+                    "and the job_image must be configured at the top-level executor config without "
+                    "using configured."
                 )
-            pipeline_origin = external_pipeline.get_origin()
 
-        job_config = DagsterK8sJobConfig(
-            dagster_home=self.dagster_home,
-            instance_config_map=self.instance_config_map,
-            postgres_password_secret=self.postgres_password_secret,
-            job_image=check.str_param(job_image, "job_image"),
-            image_pull_policy=exc_config.get("image_pull_policy"),
-            image_pull_secrets=exc_config.get("image_pull_secrets"),
-            service_account_name=exc_config.get("service_account_name"),
-            env_config_maps=exc_config.get("env_config_maps"),
-            env_secrets=exc_config.get("env_secrets"),
-        )
-
-        user_defined_k8s_config = get_user_defined_k8s_config(frozentags(external_pipeline.tags))
-
-        from dagster.cli.api import ExecuteRunArgs
-
-        input_json = serialize_dagster_namedtuple(
-            # depends on DagsterInstance.get() returning the same instance
-            # https://github.com/dagster-io/dagster/issues/2757
-            ExecuteRunArgs(
-                pipeline_origin=pipeline_origin, pipeline_run_id=run.run_id, instance_ref=None,
-            )
+            job_image = job_image_from_executor_config
+
+        job_config = self.get_k8s_job_config(job_image, exc_config)
+
+        self._instance.add_run_tags(
+            run.run_id,
+            {DOCKER_IMAGE_TAG: job_config.job_image},
         )
 
+        user_defined_k8s_config = get_user_defined_k8s_config(frozentags(run.tags))
+
+        from dagster._cli.api import ExecuteRunArgs
+
+        run_args = ExecuteRunArgs(
+            pipeline_origin=pipeline_origin,
+            pipeline_run_id=run.run_id,
+            instance_ref=self._instance.get_ref(),
+            set_exit_code_on_failure=self._fail_pod_on_run_failure,
+        ).get_command_args()
+
         job = construct_dagster_k8s_job(
             job_config,
-            command=["dagster"],
-            args=["api", "execute_run_with_structured_logs", input_json],
+            args=run_args,
             job_name=job_name,
             pod_name=pod_name,
-            component="run_coordinator",
+            component="run_worker",
             user_defined_k8s_config=user_defined_k8s_config,
-            env_vars=env_vars,
+            labels={
+                "dagster/job": pipeline_origin.pipeline_name,
+                "dagster/run-id": run.run_id,
+            },
         )
 
         job_namespace = exc_config.get("job_namespace")
 
-        api = kubernetes.client.BatchV1Api()
-        api.create_namespaced_job(body=job, namespace=job_namespace)
+        self._instance.report_engine_event(
+            "Creating Kubernetes run worker job",
+            run,
+            EngineEventData(
+                [
+                    MetadataEntry("Kubernetes Job name", value=job_name),
+                    MetadataEntry("Kubernetes Namespace", value=job_namespace),
+                    MetadataEntry("Run ID", value=run.run_id),
+                ]
+            ),
+            cls=self.__class__,
+        )
 
+        self._batch_api.create_namespaced_job(body=job, namespace=job_namespace)
         self._instance.report_engine_event(
-            "Kubernetes run_coordinator job launched",
+            "Kubernetes run worker job created",
             run,
             EngineEventData(
                 [
-                    EventMetadataEntry.text(job_name, "Kubernetes Job name"),
-                    EventMetadataEntry.text(pod_name, "Kubernetes Pod name"),
-                    EventMetadataEntry.text(job_namespace, "Kubernetes Namespace"),
-                    EventMetadataEntry.text(run.run_id, "Run ID"),
+                    MetadataEntry("Kubernetes Job name", value=job_name),
+                    MetadataEntry("Kubernetes Namespace", value=job_namespace),
+                    MetadataEntry("Run ID", value=run.run_id),
                 ]
             ),
-            cls=CeleryK8sRunLauncher,
+            cls=self.__class__,
+        )
+
+    def get_k8s_job_config(self, job_image, exc_config):
+        return DagsterK8sJobConfig(
+            dagster_home=self.dagster_home,
+            instance_config_map=self.instance_config_map,
+            postgres_password_secret=self.postgres_password_secret,
+            job_image=check.opt_str_param(job_image, "job_image"),
+            image_pull_policy=exc_config.get("image_pull_policy", self._image_pull_policy),
+            image_pull_secrets=exc_config.get("image_pull_secrets", []) + self._image_pull_secrets,
+            service_account_name=exc_config.get("service_account_name", self._service_account_name),
+            env_config_maps=exc_config.get("env_config_maps", []) + self._env_config_maps,
+            env_secrets=exc_config.get("env_secrets", []) + self._env_secrets,
+            volume_mounts=exc_config.get("volume_mounts", []) + self._volume_mounts,
+            volumes=exc_config.get("volumes", []) + self._volumes,
+            labels=merge_dicts(self._labels, exc_config.get("labels", {})),
         )
-        return run
 
     # https://github.com/dagster-io/dagster/issues/2741
     def can_terminate(self, run_id):
         check.str_param(run_id, "run_id")
 
         pipeline_run = self._instance.get_run_by_id(run_id)
         if not pipeline_run:
@@ -273,43 +276,111 @@
             return False
 
         return True
 
     def terminate(self, run_id):
         check.str_param(run_id, "run_id")
 
-        if not self.can_terminate(run_id):
+        run = self._instance.get_run_by_id(run_id)
+        if not run:
+            return False
+
+        can_terminate = self.can_terminate(run_id)
+        if not can_terminate:
+            self._instance.report_engine_event(
+                message="Unable to terminate dagster job: can_terminate returned {}.".format(
+                    can_terminate
+                ),
+                pipeline_run=run,
+                cls=self.__class__,
+            )
             return False
 
         job_name = get_job_name_from_run_id(run_id)
 
         job_namespace = self.get_namespace_from_run_config(run_id)
 
-        return delete_job(job_name=job_name, namespace=job_namespace)
+        self._instance.report_run_canceling(run)
+
+        try:
+            termination_result = delete_job(job_name=job_name, namespace=job_namespace)
+            if termination_result:
+                self._instance.report_engine_event(
+                    message="Dagster Job was terminated successfully.",
+                    pipeline_run=run,
+                    cls=self.__class__,
+                )
+            else:
+                self._instance.report_engine_event(
+                    message="Dagster Job was not terminated successfully; delete_job returned {}".format(
+                        termination_result
+                    ),
+                    pipeline_run=run,
+                    cls=self.__class__,
+                )
+            return termination_result
+        except Exception:
+            self._instance.report_engine_event(
+                message="Dagster Job was not terminated successfully; encountered error in delete_job",
+                pipeline_run=run,
+                engine_event_data=EngineEventData.engine_error(
+                    serializable_error_info_from_exc_info(sys.exc_info())
+                ),
+                cls=self.__class__,
+            )
 
     def get_namespace_from_run_config(self, run_id):
         check.str_param(run_id, "run_id")
 
         pipeline_run = self._instance.get_run_by_id(run_id)
         run_config = pipeline_run.run_config
         executor_config = _get_validated_celery_k8s_executor_config(run_config)
         return executor_config.get("job_namespace")
 
+    @property
+    def supports_check_run_worker_health(self):
+        return True
+
+    def check_run_worker_health(self, run: PipelineRun):
+        job_namespace = _get_validated_celery_k8s_executor_config(run.run_config).get(
+            "job_namespace"
+        )
+        job_name = get_job_name_from_run_id(run.run_id)
+        try:
+            job = self._batch_api.read_namespaced_job(namespace=job_namespace, name=job_name)
+        except Exception:
+            return CheckRunHealthResult(
+                WorkerStatus.UNKNOWN, str(serializable_error_info_from_exc_info(sys.exc_info()))
+            )
+        if job.status.failed:
+            return CheckRunHealthResult(WorkerStatus.FAILED, "K8s job failed")
+        return CheckRunHealthResult(WorkerStatus.RUNNING)
+
 
 def _get_validated_celery_k8s_executor_config(run_config):
     check.dict_param(run_config, "run_config")
 
-    check.invariant(
-        CELERY_K8S_CONFIG_KEY in run_config.get("execution", {}),
-        "{} execution must be configured in pipeline execution config to launch runs with "
-        "CeleryK8sRunLauncher".format(CELERY_K8S_CONFIG_KEY),
-    )
+    executor_config = run_config.get("execution", {})
+    execution_config_schema = resolve_to_config_type(celery_k8s_executor_config())
+
+    # In run config on jobs, we don't have an executor key
+    if not CELERY_K8S_CONFIG_KEY in executor_config:
+
+        execution_run_config = executor_config.get("config", {})
+    else:
+        execution_run_config = (run_config["execution"][CELERY_K8S_CONFIG_KEY] or {}).get(
+            "config", {}
+        )
 
-    execution_config_schema = resolve_to_config_type(celery_k8s_config())
-    execution_run_config = run_config["execution"][CELERY_K8S_CONFIG_KEY].get("config", {})
     res = process_config(execution_config_schema, execution_run_config)
 
     check.invariant(
-        res.success, "Incorrect {} execution schema provided".format(CELERY_K8S_CONFIG_KEY)
+        res.success,
+        "Incorrect execution schema provided. Note: You may also be seeing this error "
+        "because you are using the configured API. "
+        "Using configured with the {config_key} executor is not supported at this time, "
+        "and all executor config must be directly in the run config without using configured.".format(
+            config_key=CELERY_K8S_CONFIG_KEY,
+        ),
     )
 
     return res.value
```

### Comparing `dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s.egg-info/PKG-INFO` & `dagster-celery-k8s-1.0.5/dagster_celery_k8s.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-celery-k8s
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: A Dagster integration for celery-k8s-executor
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-celery-k8s
 Author: Elementl
-Author-email: UNKNOWN
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
+License-File: LICENSE
+
+UNKNOWN
+
```

