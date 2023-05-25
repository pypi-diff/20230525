# Comparing `tmp/dagster-celery-0.9.9rc1.tar.gz` & `tmp/dagster-celery-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-celery-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:14 2020, max compression
+gzip compressed data, was "dagster-celery-1.0.5.tar", last modified: Fri Aug 26 13:46:51 2022, max compression
```

## Comparing `dagster-celery-0.9.9rc1.tar` & `dagster-celery-1.0.5.tar`

### file list

```diff
@@ -1,42 +1,28 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      668 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      128 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery/
--rw-r--r--   0 bobchen    (501) staff       (20)      226 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      346 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/app.py
--rw-r--r--   0 bobchen    (501) staff       (20)     8673 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/cli.py
--rw-r--r--   0 bobchen    (501) staff       (20)      507 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/config.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7123 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/core_execution_loop.py
--rw-r--r--   0 bobchen    (501) staff       (20)      488 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/defaults.py
--rw-r--r--   0 bobchen    (501) staff       (20)     6300 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/executor.py
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/k8s_job_task.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1122 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/make_app.py
--rw-r--r--   0 bobchen    (501) staff       (20)      453 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/tags.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2680 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/tasks.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      668 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)     1079 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       60 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery.egg-info/entry_points.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)      106 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       36 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1317 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/empty.py
--rw-r--r--   0 bobchen    (501) staff       (20)       57 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/engine_config.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7683 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/repo.py
--rw-r--r--   0 bobchen    (501) staff       (20)     5749 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/test_cli.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1666 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/test_config.py
--rw-r--r--   0 bobchen    (501) staff       (20)    12342 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/test_execute.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3068 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/test_priority.py
--rw-r--r--   0 bobchen    (501) staff       (20)      770 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/test_queues.py
--rw-r--r--   0 bobchen    (501) staff       (20)      289 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/test_utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       95 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2773 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1273 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:51.076913 dagster-celery-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-celery-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2022-08-26 13:33:01.000000 dagster-celery-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      748 2022-08-26 13:46:51.076913 dagster-celery-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2022-08-26 13:33:01.000000 dagster-celery-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:51.076913 dagster-celery-1.0.5/dagster_celery/
+-rw-r--r--   0 root         (0) root         (0)      227 2022-08-26 13:33:01.000000 dagster-celery-1.0.5/dagster_celery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      346 2022-08-26 13:33:01.000000 dagster-celery-1.0.5/dagster_celery/app.py
+-rw-r--r--   0 root         (0) root         (0)     9744 2022-08-26 13:33:01.000000 dagster-celery-1.0.5/dagster_celery/cli.py
+-rw-r--r--   0 root         (0) root         (0)      499 2022-08-26 13:33:01.000000 dagster-celery-1.0.5/dagster_celery/config.py
+-rw-r--r--   0 root         (0) root         (0)     8757 2022-08-26 13:33:01.000000 dagster-celery-1.0.5/dagster_celery/core_execution_loop.py
+-rw-r--r--   0 root         (0) root         (0)      488 2022-08-26 13:33:01.000000 dagster-celery-1.0.5/dagster_celery/defaults.py
+-rw-r--r--   0 root         (0) root         (0)     6410 2022-08-26 13:33:01.000000 dagster-celery-1.0.5/dagster_celery/executor.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2022-08-26 13:33:01.000000 dagster-celery-1.0.5/dagster_celery/make_app.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-celery-1.0.5/dagster_celery/py.typed
+-rw-r--r--   0 root         (0) root         (0)      323 2022-08-26 13:33:01.000000 dagster-celery-1.0.5/dagster_celery/tags.py
+-rw-r--r--   0 root         (0) root         (0)     2829 2022-08-26 13:33:01.000000 dagster-celery-1.0.5/dagster_celery/tasks.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-celery-1.0.5/dagster_celery/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:51.076913 dagster-celery-1.0.5/dagster_celery.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      748 2022-08-26 13:46:51.000000 dagster-celery-1.0.5/dagster_celery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      627 2022-08-26 13:46:51.000000 dagster-celery-1.0.5/dagster_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:51.000000 dagster-celery-1.0.5/dagster_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2022-08-26 13:46:51.000000 dagster-celery-1.0.5/dagster_celery.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:51.000000 dagster-celery-1.0.5/dagster_celery.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      117 2022-08-26 13:46:51.000000 dagster-celery-1.0.5/dagster_celery.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-08-26 13:46:51.000000 dagster-celery-1.0.5/dagster_celery.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      195 2022-08-26 13:46:51.080913 dagster-celery-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1649 2022-08-26 13:33:01.000000 dagster-celery-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-celery-0.9.9rc1/LICENSE` & `dagster-celery-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-celery-0.9.9rc1/PKG-INFO` & `dagster-celery-1.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: dagster-celery
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: Package for using Celery as Dagster's execution engine.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-celery
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
-Provides-Extra: redis
 Provides-Extra: flower
+Provides-Extra: redis
 Provides-Extra: kubernetes
+Provides-Extra: test
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-celery-0.9.9rc1/dagster_celery/cli.py` & `dagster-celery-1.0.5/dagster_celery/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import os
 import subprocess
 import uuid
 
 import click
 from celery.utils.nodenames import default_nodename, host_format
 
-from dagster import check
-from dagster.config.post_process import post_process_config
-from dagster.config.validate import validate_config
-from dagster.core.errors import DagsterInvalidConfigError
-from dagster.core.instance import DagsterInstance
-from dagster.utils import load_yaml_from_path, mkdir_p
+import dagster._check as check
+from dagster._config import post_process_config, validate_config
+from dagster._core.errors import DagsterInvalidConfigError
+from dagster._core.instance import DagsterInstance
+from dagster._utils import load_yaml_from_path, mkdir_p
 
 from .executor import CeleryExecutor, celery_executor
 from .make_app import make_app
 
 
 def create_worker_cli_group():
     group = click.Group(name="worker")
@@ -44,39 +43,42 @@
     return (
         name + "@%h"
         if name is not None
         else "dagster-{uniq}@%h".format(uniq=str(uuid.uuid4())[-6:])
     )
 
 
-def get_config_dir(config_yaml=None):
-    instance = DagsterInstance.get()
+def get_validated_config(config_yaml=None):
     config_type = celery_executor.config_schema.config_type
     config_value = get_config_value_from_yaml(config_yaml)
+    config = validate_config(config_type, config_value)
+    if not config.success:
+        raise DagsterInvalidConfigError(
+            "Errors while loading Celery executor config at {}.".format(config_yaml),
+            config.errors,
+            config_value,
+        )
+    return post_process_config(config_type, config_value).value
+
+
+def get_config_dir(config_yaml=None):
+    instance = DagsterInstance.get()
 
     config_module_name = "dagster_celery_config"
 
     config_dir = os.path.join(
         instance.root_directory, "dagster_celery", "config", str(uuid.uuid4())
     )
     mkdir_p(config_dir)
     config_path = os.path.join(
         config_dir, "{config_module_name}.py".format(config_module_name=config_module_name)
     )
 
-    config = validate_config(config_type, config_value)
-    if not config.success:
-        raise DagsterInvalidConfigError(
-            "Errors while loading Celery executor config at {}.".format(config_yaml),
-            config.errors,
-            config_value,
-        )
-
-    validated_config = post_process_config(config_type, config_value).value
-    with open(config_path, "w") as fd:
+    validated_config = get_validated_config(config_yaml)
+    with open(config_path, "w", encoding="utf8") as fd:
         if "broker" in validated_config and validated_config["broker"]:
             fd.write(
                 "broker_url = '{broker_url}'\n".format(broker_url=str(validated_config["broker"]))
             )
         if "backend" in validated_config and validated_config["backend"]:
             fd.write(
                 "result_backend = '{result_backend}'\n".format(
@@ -113,15 +115,15 @@
     "--config-yaml",
     "-y",
     type=click.Path(exists=True),
     default=None,
     help=(
         "Specify the path to a config YAML file with options for the worker. This is the same "
         "config block that you provide to dagster_celery.celery_executor when configuring a "
-        "pipeline for execution with Celery, with, e.g., the URL of the broker to use."
+        "job for execution with Celery, with, e.g., the URL of the broker to use."
     ),
 )
 @click.option(
     "--queue",
     "-q",
     type=click.STRING,
     multiple=True,
@@ -146,15 +148,22 @@
 )
 @click.option(
     "--loglevel", "-l", type=click.STRING, default="INFO", help="Log level for the worker."
 )
 @click.option("--app", "-A", type=click.STRING)
 @click.argument("additional_args", nargs=-1, type=click.UNPROCESSED)
 def worker_start_command(
-    name, config_yaml, background, queue, includes, loglevel, app, additional_args,
+    name,
+    config_yaml,
+    background,
+    queue,
+    includes,
+    loglevel,
+    app,
+    additional_args,
 ):
     check.invariant(app, "App must be specified. E.g. dagster_celery.app or dagster_celery_k8s.app")
 
     loglevel_args = ["--loglevel", loglevel]
 
     if len(queue) > 4:
         check.failed(
@@ -185,27 +194,56 @@
 
     if background:
         launch_background_worker(subprocess_args, env=env)
     else:
         return subprocess.check_call(subprocess_args, env=env)
 
 
+@click.command(name="status", help="wrapper around `celery status`")
+@click.option(
+    "--config-yaml",
+    "-y",
+    type=click.Path(exists=True),
+    required=True,
+    help=(
+        "Specify the path to a config YAML file with options for the worker. This is the same "
+        "config block that you provide to dagster_celery.celery_executor when configuring a "
+        "job for execution with Celery, with, e.g., the URL of the broker to use."
+    ),
+)
+@click.option("--app", "-A", type=click.STRING)
+@click.argument("additional_args", nargs=-1, type=click.UNPROCESSED)
+def status_command(
+    config_yaml,
+    app,
+    additional_args,
+):
+    check.invariant(app, "App must be specified. E.g. dagster_celery.app or dagster_celery_k8s.app")
+
+    config = get_validated_config(config_yaml)
+    subprocess_args = ["celery", "-A", app, "-b", str(config["broker"]), "status"] + list(
+        additional_args
+    )
+
+    subprocess.check_call(subprocess_args)
+
+
 @click.command(
     name="list",
     help="List running dagster-celery workers. Note that we use the broker to contact the workers.",
 )
 @click.option(
     "--config-yaml",
     "-y",
     type=click.Path(exists=True),
     default=None,
     help=(
         "Specify the path to a config YAML file with options for the workers you are trying to "
         "manage. This is the same config block that you provide to dagster_celery.celery_executor "
-        "when configuring a pipeline for execution with Celery, with, e.g., the URL of the broker "
+        "when configuring a job for execution with Celery, with, e.g., the URL of the broker "
         "to use. Without this config file, you will not be able to find your workers (since the "
         "CLI won't know how to reach the broker)."
     ),
 )
 def worker_list_command(config_yaml=None):
     app = get_app(config_yaml)
 
@@ -228,15 +266,15 @@
     "--config-yaml",
     "-y",
     type=click.Path(exists=True),
     default=None,
     help=(
         "Specify the path to a config YAML file with options for the workers you are trying to "
         "manage. This is the same config block that you provide to dagster_celery.celery_executor "
-        "when configuring a pipeline for execution with Celery, with, e.g., the URL of the broker "
+        "when configuring a job for execution with Celery, with, e.g., the URL of the broker "
         "to use. Without this config file, you will not be able to terminate your workers (since "
         "the CLI won't know how to reach the broker)."
     ),
 )
 def worker_terminate_command(name="dagster", config_yaml=None, all_=False):
     app = get_app(config_yaml)
 
@@ -247,15 +285,15 @@
             "shutdown", destination=[host_format(default_nodename(get_worker_name(name)))]
         )
 
 
 worker_cli = create_worker_cli_group()
 
 
-@click.group(commands={"worker": worker_cli})
+@click.group(commands={"worker": worker_cli, "status": status_command})
 def main():
     """dagster-celery"""
 
 
 if __name__ == "__main__":
     # pylint doesn't understand click
     main()  # pylint:disable=no-value-for-parameter
```

### Comparing `dagster-celery-0.9.9rc1/dagster_celery/core_execution_loop.py` & `dagster-celery-1.0.5/dagster_celery/core_execution_loop.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,149 +1,179 @@
 import sys
 import time
 
-from dagster import check
-from dagster.core.errors import DagsterSubprocessError
-from dagster.core.events import DagsterEvent, EngineEventData
-from dagster.core.execution.context.system import SystemPipelineExecutionContext
-from dagster.core.execution.plan.plan import ExecutionPlan
-from dagster.serdes import deserialize_json_to_dagster_namedtuple
-from dagster.utils.error import serializable_error_info_from_exc_info
+from celery.exceptions import TaskRevokedError
+
+import dagster._check as check
+from dagster._core.errors import DagsterSubprocessError
+from dagster._core.events import DagsterEvent, EngineEventData
+from dagster._core.execution.context.system import PlanOrchestrationContext
+from dagster._core.execution.plan.plan import ExecutionPlan
+from dagster._core.storage.tags import PRIORITY_TAG
+from dagster._serdes import deserialize_json_to_dagster_namedtuple
+from dagster._utils.error import serializable_error_info_from_exc_info
 
 from .defaults import task_default_priority, task_default_queue
 from .make_app import make_app
 from .tags import (
     DAGSTER_CELERY_QUEUE_TAG,
     DAGSTER_CELERY_RUN_PRIORITY_TAG,
     DAGSTER_CELERY_STEP_PRIORITY_TAG,
-    DAGSTER_STEP_PRIORITY_TAG,
 )
 
 TICK_SECONDS = 1
 DELEGATE_MARKER = "celery_queue_wait"
 
 
 def core_celery_execution_loop(pipeline_context, execution_plan, step_execution_fn):
 
-    check.inst_param(pipeline_context, "pipeline_context", SystemPipelineExecutionContext)
+    check.inst_param(pipeline_context, "pipeline_context", PlanOrchestrationContext)
     check.inst_param(execution_plan, "execution_plan", ExecutionPlan)
     check.callable_param(step_execution_fn, "step_execution_fn")
 
     executor = pipeline_context.executor
 
-    # https://github.com/dagster-io/dagster/issues/2440
-    check.invariant(
-        execution_plan.artifacts_persisted,
-        "Cannot use in-memory storage with Celery, use filesystem (on top of NFS or "
-        "similar system that allows files to be available to all nodes), S3, or GCS",
-    )
+    # If there are no step keys to execute, then any io managers will not be used.
+    if len(execution_plan.step_keys_to_execute) > 0:
+        # https://github.com/dagster-io/dagster/issues/2440
+        check.invariant(
+            execution_plan.artifacts_persisted,
+            "Cannot use in-memory storage with Celery, use filesystem (on top of NFS or "
+            "similar system that allows files to be available to all nodes), S3, or GCS",
+        )
 
     app = make_app(executor.app_args())
 
     priority_for_step = lambda step: (
         -1 * int(step.tags.get(DAGSTER_CELERY_STEP_PRIORITY_TAG, task_default_priority))
         + -1 * _get_run_priority(pipeline_context)
     )
     priority_for_key = lambda step_key: (
         priority_for_step(execution_plan.get_step_by_key(step_key))
     )
     _warn_on_priority_misuse(pipeline_context, execution_plan)
 
     step_results = {}  # Dict[ExecutionStep, celery.AsyncResult]
     step_errors = {}
-    completed_steps = set({})  # Set[step_key]
 
-    active_execution = execution_plan.start(
-        retries=pipeline_context.executor.retries, sort_key_fn=priority_for_step,
-    )
-    stopping = False
+    with execution_plan.start(
+        retry_mode=pipeline_context.executor.retries,
+        sort_key_fn=priority_for_step,
+    ) as active_execution:
 
-    while (not active_execution.is_complete and not stopping) or step_results:
+        stopping = False
 
-        results_to_pop = []
-        for step_key, result in sorted(step_results.items(), key=lambda x: priority_for_key(x[0])):
-            if result.ready():
-                try:
-                    step_events = result.get()
-                except Exception:  # pylint: disable=broad-except
-                    # We will want to do more to handle the exception here.. maybe subclass Task
-                    # Certainly yield an engine or pipeline event
-                    step_events = []
-                    step_errors[step_key] = serializable_error_info_from_exc_info(sys.exc_info())
-                    stopping = True
-                for step_event in step_events:
-                    event = deserialize_json_to_dagster_namedtuple(step_event)
-                    yield event
-                    active_execution.handle_event(event)
-
-                results_to_pop.append(step_key)
-                completed_steps.add(step_key)
-
-        for step_key in results_to_pop:
-            if step_key in step_results:
-                del step_results[step_key]
-                active_execution.verify_complete(pipeline_context, step_key)
-
-        # process skips from failures or uncovered inputs
-        for event in active_execution.skipped_step_events_iterator(pipeline_context):
-            yield event
-
-        # don't add any new steps if we are stopping
-        if stopping:
-            continue
-
-        # This is a slight refinement. If we have n workers idle and schedule m > n steps for
-        # execution, the first n steps will be picked up by the idle workers in the order in
-        # which they are scheduled (and the following m-n steps will be executed in priority
-        # order, provided that it takes longer to execute a step than to schedule it). The test
-        # case has m >> n to exhibit this behavior in the absence of this sort step.
-        for step in active_execution.get_steps_to_execute():
-            try:
-                queue = step.tags.get(DAGSTER_CELERY_QUEUE_TAG, task_default_queue)
+        while (not active_execution.is_complete and not stopping) or step_results:
+            if active_execution.check_for_interrupts():
                 yield DagsterEvent.engine_event(
                     pipeline_context,
-                    'Submitting celery task for step "{step_key}" to queue "{queue}".'.format(
-                        step_key=step.key, queue=queue
-                    ),
-                    EngineEventData(marker_start=DELEGATE_MARKER),
-                    step_key=step.key,
+                    "Celery executor: received termination signal - revoking active tasks from workers",
+                    EngineEventData.interrupted(list(step_results.keys())),
                 )
-
-                # Get the Celery priority for this step
-                priority = _get_step_priority(pipeline_context, step)
-
-                # Submit the Celery tasks
-                step_results[step.key] = step_execution_fn(
-                    app, pipeline_context, step, queue, priority
-                )
-
-            except Exception:
-                yield DagsterEvent.engine_event(
-                    pipeline_context,
-                    "Encountered error during celery task submission.".format(),
-                    event_specific_data=EngineEventData.engine_error(
-                        serializable_error_info_from_exc_info(sys.exc_info()),
-                    ),
-                )
-                raise
-
-        time.sleep(TICK_SECONDS)
-
-    if step_errors:
-        raise DagsterSubprocessError(
-            "During celery execution errors occurred in workers:\n{error_list}".format(
-                error_list="\n".join(
-                    [
-                        "[{step}]: {err}".format(step=key, err=err.to_string())
-                        for key, err in step_errors.items()
-                    ]
-                )
-            ),
-            subprocess_error_infos=list(step_errors.values()),
-        )
+                stopping = True
+                active_execution.mark_interrupted()
+                for result in step_results.values():
+                    result.revoke()
+            results_to_pop = []
+            for step_key, result in sorted(
+                step_results.items(), key=lambda x: priority_for_key(x[0])
+            ):
+                if result.ready():
+                    try:
+                        step_events = result.get()
+                    except TaskRevokedError:
+                        step_events = []
+                        step = active_execution.get_step_by_key(step_key)
+                        yield DagsterEvent.engine_event(
+                            pipeline_context.for_step(step),
+                            'celery task for running step "{step_key}" was revoked.'.format(
+                                step_key=step_key,
+                            ),
+                            EngineEventData(marker_end=DELEGATE_MARKER),
+                        )
+                    except Exception:
+                        # We will want to do more to handle the exception here.. maybe subclass Task
+                        # Certainly yield an engine or pipeline event
+                        step_events = []
+                        step_errors[step_key] = serializable_error_info_from_exc_info(
+                            sys.exc_info()
+                        )
+                    for step_event in step_events:
+                        event = deserialize_json_to_dagster_namedtuple(step_event)
+                        yield event
+                        active_execution.handle_event(event)
+
+                    results_to_pop.append(step_key)
+
+            for step_key in results_to_pop:
+                if step_key in step_results:
+                    del step_results[step_key]
+                    active_execution.verify_complete(pipeline_context, step_key)
+
+            # process skips from failures or uncovered inputs
+            for event in active_execution.plan_events_iterator(pipeline_context):
+                yield event
+
+            # don't add any new steps if we are stopping
+            if stopping or step_errors:
+                continue
+
+            # This is a slight refinement. If we have n workers idle and schedule m > n steps for
+            # execution, the first n steps will be picked up by the idle workers in the order in
+            # which they are scheduled (and the following m-n steps will be executed in priority
+            # order, provided that it takes longer to execute a step than to schedule it). The test
+            # case has m >> n to exhibit this behavior in the absence of this sort step.
+            for step in active_execution.get_steps_to_execute():
+                try:
+                    queue = step.tags.get(DAGSTER_CELERY_QUEUE_TAG, task_default_queue)
+                    yield DagsterEvent.engine_event(
+                        pipeline_context.for_step(step),
+                        'Submitting celery task for step "{step_key}" to queue "{queue}".'.format(
+                            step_key=step.key, queue=queue
+                        ),
+                        EngineEventData(marker_start=DELEGATE_MARKER),
+                    )
+
+                    # Get the Celery priority for this step
+                    priority = _get_step_priority(pipeline_context, step)
+
+                    # Submit the Celery tasks
+                    step_results[step.key] = step_execution_fn(
+                        app,
+                        pipeline_context,
+                        step,
+                        queue,
+                        priority,
+                        active_execution.get_known_state(),
+                    )
+
+                except Exception:
+                    yield DagsterEvent.engine_event(
+                        pipeline_context,
+                        "Encountered error during celery task submission.",
+                        event_specific_data=EngineEventData.engine_error(
+                            serializable_error_info_from_exc_info(sys.exc_info()),
+                        ),
+                    )
+                    raise
+
+            time.sleep(TICK_SECONDS)
+
+        if step_errors:
+            raise DagsterSubprocessError(
+                "During celery execution errors occurred in workers:\n{error_list}".format(
+                    error_list="\n".join(
+                        [
+                            "[{step}]: {err}".format(step=key, err=err.to_string())
+                            for key, err in step_errors.items()
+                        ]
+                    )
+                ),
+                subprocess_error_infos=list(step_errors.values()),
+            )
 
 
 def _get_step_priority(context, step):
     """Step priority is (currently) set as the overall pipeline run priority plus the individual
     step priority.
     """
     run_priority = _get_run_priority(context)
@@ -162,15 +192,15 @@
 
 
 def _warn_on_priority_misuse(context, execution_plan):
     bad_keys = []
     for key in execution_plan.step_keys_to_execute:
         step = execution_plan.get_step_by_key(key)
         if (
-            step.tags.get(DAGSTER_STEP_PRIORITY_TAG) is not None
+            step.tags.get(PRIORITY_TAG) is not None
             and step.tags.get(DAGSTER_CELERY_STEP_PRIORITY_TAG) is None
         ):
             bad_keys.append(key)
 
     if bad_keys:
         context.log.warn(
             'The following steps do not have "dagster-celery/priority" set but do '
```

### Comparing `dagster-celery-0.9.9rc1/dagster_celery/executor.py` & `dagster-celery-1.0.5/dagster_celery/executor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from dagster import Executor, Field, Noneable, Permissive, StringSource, check, executor
-from dagster.core.definitions.executor import check_cross_process_constraints
-from dagster.core.execution.retries import Retries, RetryMode, get_retries_config
+from dagster import Executor, Field, Noneable, Permissive, StringSource
+from dagster import _check as check
+from dagster import executor, multiple_process_executor_requirements
+from dagster._core.execution.retries import RetryMode, get_retries_config
+from dagster._grpc.types import ExecuteStepArgs
+from dagster._serdes import pack_value
 
 from .config import DEFAULT_CONFIG, dict_wrapper
 from .defaults import broker_url, result_backend
 
 CELERY_CONFIG = {
     "broker": Field(
         Noneable(StringSource),
@@ -29,120 +32,132 @@
         is_required=False,
         description="Additional settings for the Celery app.",
     ),
     "retries": get_retries_config(),
 }
 
 
-@executor(name="celery", config_schema=CELERY_CONFIG)
+@executor(
+    name="celery",
+    config_schema=CELERY_CONFIG,
+    requirements=multiple_process_executor_requirements(),
+)
 def celery_executor(init_context):
     """Celery-based executor.
 
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
     modified, but that when solid executions are especially fast or slow, or when there are
-    different requirements around idempotence or retry, it may make sense to execute pipelines
+    different requirements around idempotence or retry, it may make sense to execute jobs
     with variations on these settings.
 
-    If you'd like to configure a celery executor in addition to the
-    :py:class:`~dagster.default_executors`, you should add it to the ``executor_defs`` defined on a
-    :py:class:`~dagster.ModeDefinition` as follows:
+    To use the `celery_executor`, set it as the `executor_def` when defining a job:
 
     .. code-block:: python
 
-        from dagster import ModeDefinition, default_executors, pipeline
+        from dagster import job
         from dagster_celery import celery_executor
 
-        @pipeline(mode_defs=[ModeDefinition(executor_defs=default_executors + [celery_executor])])
-        def celery_enabled_pipeline():
+        @job(executor_def=celery_executor)
+        def celery_enabled_job():
             pass
 
     Then you can configure the executor as follows:
 
     .. code-block:: YAML
 
         execution:
-          celery:
-            config:
-              broker: 'pyamqp://guest@localhost//'  # Optional[str]: The URL of the Celery broker
-              backend: 'rpc://' # Optional[str]: The URL of the Celery results backend
-              include: ['my_module'] # Optional[List[str]]: Modules every worker should import
-              config_source: # Dict[str, Any]: Any additional parameters to pass to the
-                  #...       # Celery workers. This dict will be passed as the `config_source`
-                  #...       # argument of celery.Celery().
+          config:
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
     """
-    check_cross_process_constraints(init_context)
 
     return CeleryExecutor(
         broker=init_context.executor_config.get("broker"),
         backend=init_context.executor_config.get("backend"),
         config_source=init_context.executor_config.get("config_source"),
         include=init_context.executor_config.get("include"),
-        retries=Retries.from_config(init_context.executor_config["retries"]),
+        retries=RetryMode.from_config(init_context.executor_config["retries"]),
     )
 
 
-def _submit_task(app, pipeline_context, step, queue, priority):
+def _submit_task(app, plan_context, step, queue, priority, known_state):
     from .tasks import create_task
 
-    task = create_task(app)
+    execute_step_args = ExecuteStepArgs(
+        pipeline_origin=plan_context.reconstructable_pipeline.get_python_origin(),
+        pipeline_run_id=plan_context.pipeline_run.run_id,
+        step_keys_to_execute=[step.key],
+        instance_ref=plan_context.instance.get_ref(),
+        retry_mode=plan_context.executor.retries.for_inner_plan(),
+        known_state=known_state,
+    )
 
+    task = create_task(app)
     task_signature = task.si(
-        instance_ref_dict=pipeline_context.instance.get_ref().to_dict(),
-        executable_dict=pipeline_context.pipeline.to_dict(),
-        run_id=pipeline_context.pipeline_run.run_id,
-        step_keys=[step.key],
-        retries_dict=pipeline_context.executor.retries.for_inner_plan().to_config(),
+        execute_step_args_packed=pack_value(execute_step_args),
+        executable_dict=plan_context.reconstructable_pipeline.to_dict(),
     )
     return task_signature.apply_async(
-        priority=priority, queue=queue, routing_key="{queue}.execute_plan".format(queue=queue),
+        priority=priority,
+        queue=queue,
+        routing_key="{queue}.execute_plan".format(queue=queue),
     )
 
 
 class CeleryExecutor(Executor):
     def __init__(
-        self, retries, broker=None, backend=None, include=None, config_source=None,
+        self,
+        retries,
+        broker=None,
+        backend=None,
+        include=None,
+        config_source=None,
     ):
         self.broker = check.opt_str_param(broker, "broker", default=broker_url)
         self.backend = check.opt_str_param(backend, "backend", default=result_backend)
         self.include = check.opt_list_param(include, "include", of_type=str)
         self.config_source = dict_wrapper(
             dict(DEFAULT_CONFIG, **check.opt_dict_param(config_source, "config_source"))
         )
-        self._retries = check.inst_param(retries, "retries", Retries)
+        self._retries = check.inst_param(retries, "retries", RetryMode)
 
     @property
     def retries(self):
         return self._retries
 
-    def execute(self, pipeline_context, execution_plan):
+    def execute(self, plan_context, execution_plan):
         from .core_execution_loop import core_celery_execution_loop
 
         return core_celery_execution_loop(
-            pipeline_context, execution_plan, step_execution_fn=_submit_task
+            plan_context, execution_plan, step_execution_fn=_submit_task
         )
 
     @staticmethod
     def for_cli(broker=None, backend=None, include=None, config_source=None):
         return CeleryExecutor(
-            retries=Retries(RetryMode.DISABLED),
+            retries=RetryMode(RetryMode.DISABLED),
             broker=broker,
             backend=backend,
             include=include,
             config_source=config_source,
         )
 
     def app_args(self):
```

### Comparing `dagster-celery-0.9.9rc1/dagster_celery/make_app.py` & `dagster-celery-1.0.5/dagster_celery/make_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from celery import Celery
 from celery.utils.collections import force_mapping
 from kombu import Queue
 
-from dagster.seven import is_module_available
+from dagster._seven import is_module_available
 
 
 def make_app(app_args=None):
     return make_app_with_task_routes(
         app_args=app_args,
         task_routes={"execute_plan": {"queue": "dagster", "routing_key": "dagster.execute_plan"}},
     )
```

### Comparing `dagster-celery-0.9.9rc1/dagster_celery.egg-info/PKG-INFO` & `dagster-celery-1.0.5/dagster_celery.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: dagster-celery
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: Package for using Celery as Dagster's execution engine.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-celery
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
-Provides-Extra: redis
 Provides-Extra: flower
+Provides-Extra: redis
 Provides-Extra: kubernetes
+Provides-Extra: test
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-celery-0.9.9rc1/dagster_celery.egg-info/SOURCES.txt` & `dagster-celery-1.0.5/dagster_celery.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -6,32 +6,19 @@
 dagster_celery/__init__.py
 dagster_celery/app.py
 dagster_celery/cli.py
 dagster_celery/config.py
 dagster_celery/core_execution_loop.py
 dagster_celery/defaults.py
 dagster_celery/executor.py
-dagster_celery/k8s_job_task.py
 dagster_celery/make_app.py
+dagster_celery/py.typed
 dagster_celery/tags.py
 dagster_celery/tasks.py
 dagster_celery/version.py
 dagster_celery.egg-info/PKG-INFO
 dagster_celery.egg-info/SOURCES.txt
 dagster_celery.egg-info/dependency_links.txt
 dagster_celery.egg-info/entry_points.txt
 dagster_celery.egg-info/not-zip-safe
 dagster_celery.egg-info/requires.txt
-dagster_celery.egg-info/top_level.txt
-dagster_celery_tests/__init__.py
-dagster_celery_tests/conftest.py
-dagster_celery_tests/empty.py
-dagster_celery_tests/engine_config.py
-dagster_celery_tests/repo.py
-dagster_celery_tests/test_cli.py
-dagster_celery_tests/test_config.py
-dagster_celery_tests/test_execute.py
-dagster_celery_tests/test_priority.py
-dagster_celery_tests/test_queues.py
-dagster_celery_tests/test_utils.py
-dagster_celery_tests/test_version.py
-dagster_celery_tests/utils.py
+dagster_celery.egg-info/top_level.txt
```

### Comparing `dagster-celery-0.9.9rc1/setup.py` & `dagster-celery-1.0.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,48 @@
+from typing import Dict
+
 from setuptools import find_packages, setup
 
 
-def get_version():
-    version = {}
-    with open("dagster_celery/version.py") as fp:
+def get_version() -> str:
+    version: Dict[str, str] = {}
+    with open("dagster_celery/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
 if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
     setup(
         name="dagster-celery",
-        version=get_version(),
+        version=ver,
         author="Elementl",
         author_email="hello@elementl.com",
         license="Apache-2.0",
         description="Package for using Celery as Dagster's execution engine.",
         url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-celery",
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
+        packages=find_packages(exclude=["dagster_celery_tests*"]),
         entry_points={"console_scripts": ["dagster-celery = dagster_celery.cli:main"]},
-        install_requires=["dagster", "dagster_graphql", "celery>=4.3.0", "click>=5.0",],
-        extras_require={"flower": ["flower"], "redis": ["redis"], "kubernetes": ["kubernetes"]},
+        install_requires=[
+            "dagster==1.0.5",
+            "celery>=4.3.0",
+            "click>=5.0,<9.0",
+        ],
+        extras_require={
+            "flower": ["flower"],
+            "redis": ["redis"],
+            "kubernetes": ["kubernetes"],
+            "test": ["docker"],
+        },
         zip_safe=False,
     )
```

