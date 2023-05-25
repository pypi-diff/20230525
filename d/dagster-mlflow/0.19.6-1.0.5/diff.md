# Comparing `tmp/dagster-mlflow-0.19.6.tar.gz` & `tmp/dagster-mlflow-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-mlflow-0.19.6.tar", last modified: Thu May 25 17:26:39 2023, max compression
+gzip compressed data, was "dagster-mlflow-1.0.5.tar", last modified: Fri Aug 26 13:47:04 2022, max compression
```

## Comparing `dagster-mlflow-0.19.6.tar` & `dagster-mlflow-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:26:39.346076 dagster-mlflow-0.19.6/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-05-25 17:16:50.000000 dagster-mlflow-0.19.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       66 2023-05-25 17:16:50.000000 dagster-mlflow-0.19.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      621 2023-05-25 17:26:39.346076 dagster-mlflow-0.19.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2023-05-25 17:16:50.000000 dagster-mlflow-0.19.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:26:39.346076 dagster-mlflow-0.19.6/dagster_mlflow/
--rw-r--r--   0 root         (0) root         (0)      303 2023-05-25 17:16:50.000000 dagster-mlflow-0.19.6/dagster_mlflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-05-25 17:16:50.000000 dagster-mlflow-0.19.6/dagster_mlflow/hooks.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-25 17:16:50.000000 dagster-mlflow-0.19.6/dagster_mlflow/py.typed
--rw-r--r--   0 root         (0) root         (0)    10800 2023-05-25 17:16:50.000000 dagster-mlflow-0.19.6/dagster_mlflow/resources.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-25 17:16:50.000000 dagster-mlflow-0.19.6/dagster_mlflow/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:26:39.346076 dagster-mlflow-0.19.6/dagster_mlflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      621 2023-05-25 17:26:39.000000 dagster-mlflow-0.19.6/dagster_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      403 2023-05-25 17:26:39.000000 dagster-mlflow-0.19.6/dagster_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:26:39.000000 dagster-mlflow-0.19.6/dagster_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:26:39.000000 dagster-mlflow-0.19.6/dagster_mlflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-25 17:26:39.000000 dagster-mlflow-0.19.6/dagster_mlflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-25 17:26:39.000000 dagster-mlflow-0.19.6/dagster_mlflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      161 2023-05-25 17:26:39.350076 dagster-mlflow-0.19.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1103 2023-05-25 17:16:50.000000 dagster-mlflow-0.19.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:47:04.560989 dagster-mlflow-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-mlflow-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2022-08-26 13:33:01.000000 dagster-mlflow-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      648 2022-08-26 13:47:04.560989 dagster-mlflow-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2022-08-26 13:33:01.000000 dagster-mlflow-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:47:04.556988 dagster-mlflow-1.0.5/dagster_mlflow/
+-rw-r--r--   0 root         (0) root         (0)      304 2022-08-26 13:33:01.000000 dagster-mlflow-1.0.5/dagster_mlflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2022-08-26 13:33:01.000000 dagster-mlflow-1.0.5/dagster_mlflow/hooks.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-mlflow-1.0.5/dagster_mlflow/py.typed
+-rw-r--r--   0 root         (0) root         (0)    10919 2022-08-26 13:33:01.000000 dagster-mlflow-1.0.5/dagster_mlflow/resources.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-mlflow-1.0.5/dagster_mlflow/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:47:04.560989 dagster-mlflow-1.0.5/dagster_mlflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      648 2022-08-26 13:47:04.000000 dagster-mlflow-1.0.5/dagster_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      403 2022-08-26 13:47:04.000000 dagster-mlflow-1.0.5/dagster_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:47:04.000000 dagster-mlflow-1.0.5/dagster_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:47:04.000000 dagster-mlflow-1.0.5/dagster_mlflow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       30 2022-08-26 13:47:04.000000 dagster-mlflow-1.0.5/dagster_mlflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-08-26 13:47:04.000000 dagster-mlflow-1.0.5/dagster_mlflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2022-08-26 13:47:04.560989 dagster-mlflow-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1289 2022-08-26 13:33:01.000000 dagster-mlflow-1.0.5/setup.py
```

### Comparing `dagster-mlflow-0.19.6/LICENSE` & `dagster-mlflow-1.0.5/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2023 Elementl, Inc.
+   Copyright {yyyy} {name of copyright owner}
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `dagster-mlflow-0.19.6/dagster_mlflow/hooks.py` & `dagster-mlflow-1.0.5/dagster_mlflow/hooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from mlflow.entities.run_status import RunStatus
+
 from dagster._core.definitions.decorators.hook_decorator import event_list_hook
 from dagster._core.definitions.events import HookExecutionResult
-from mlflow.entities.run_status import RunStatus
 
 
 def _create_mlflow_run_hook(name):
     @event_list_hook(name=name, required_resource_keys={"mlflow"})
     def _hook(context, event_list):
         for event in event_list:
             if event.is_step_success:
@@ -15,18 +16,19 @@
 
         return HookExecutionResult(hook_name=name, is_skipped=False)
 
     return _hook
 
 
 def _cleanup_on_success(context):
-    """Checks if the current solid in the context is the last solid in the job
+    """
+    Checks if the current solid in the context is the last solid in the pipeline
     and ends the mlflow run with a successful status when this is the case.
     """
-    last_solid_name = context._step_execution_context.job_def.nodes_in_topological_order[  # noqa: SLF001  # fmt: skip
+    last_solid_name = context._step_execution_context.pipeline_def.solids_in_topological_order[  # pylint: disable=protected-access
         -1
     ].name
 
     if context.op.name == last_solid_name:
         context.resources.mlflow.end_run()
```

### Comparing `dagster-mlflow-0.19.6/dagster_mlflow/resources.py` & `dagster-mlflow-1.0.5/dagster_mlflow/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-"""This module contains the mlflow resource provided by the MlFlow
+"""
+This module contains the mlflow resource provided by the MlFlow
 class. This resource provides an easy way to configure mlflow for logging various
 things from dagster runs.
 """
 import atexit
 import sys
 from itertools import islice
 from os import environ
 from typing import Any, Optional
 
 import mlflow
-from dagster import Field, Noneable, Permissive, StringSource, resource
 from mlflow.entities.run_status import RunStatus
 
+from dagster import Field, Noneable, Permissive, StringSource, resource
+
 CONFIG_SCHEMA = {
     "experiment_name": Field(StringSource, is_required=True, description="MlFlow experiment name."),
     "mlflow_tracking_uri": Field(
         Noneable(StringSource),
         default_value=None,
         is_required=False,
         description="MlFlow tracking server uri.",
@@ -57,17 +59,18 @@
 class MlFlow(metaclass=MlflowMeta):
     """Class for setting up an mlflow resource for dagster runs.
     This takes care of all the configuration required to use mlflow tracking and the complexities of
     mlflow tracking dagster parallel runs.
     """
 
     def __init__(self, context):
+
         # Context associated attributes
         self.log = context.log
-        self.run_name = context.dagster_run.job_name
+        self.run_name = context.dagster_run.pipeline_name
         self.dagster_run_id = context.run_id
 
         # resource config attributes
         resource_config = context.resource_config
         self.tracking_uri = resource_config.get("mlflow_tracking_uri")
         if self.tracking_uri:
             mlflow.set_tracking_uri(self.tracking_uri)
@@ -88,20 +91,21 @@
         # Get the client object
         self.tracking_client = mlflow.tracking.MlflowClient()
 
         # Set up the active run and tags
         self._setup()
 
     def _setup(self):
-        """Sets the active run and tags. If an Mlflow run_id exists then the
+        """
+        Sets the active run and tags. If an Mlflow run_id exists then the
         active run is set to it. This way a single Dagster run outputs data
         to the same Mlflow run, even when multiprocess executors are used.
         """
         # Get the run id
-        run_id = self._get_current_run_id()
+        run_id = self._get_current_run_id()  # pylint: disable=no-member
         self._set_active_run(run_id=run_id)
         self._set_all_tags()
 
         # hack needed to stop mlflow from marking run as finished when
         # a process exits in parallel runs
         atexit.unregister(mlflow.end_run)
 
@@ -114,46 +118,49 @@
         Args:
             experiment (optional): Mlflow experiment.
             When none is passed it fetches the experiment object set in
             the constructor.  Defaults to None.
             dagster_run_id (optional): The Dagster run id.
             When none is passed it fetches the dagster_run_id object set in
             the constructor.  Defaults to None.
-
         Returns:
             run_id (str or None): run_id if it is found else None
         """
         experiment = experiment or self.experiment
         dagster_run_id = dagster_run_id or self.dagster_run_id
         if experiment:
             # Check if a run with this dagster run id has already been started
             # in mlflow, will get an empty dataframe if not
             current_run_df = mlflow.search_runs(
                 experiment_ids=[experiment.experiment_id],
                 filter_string=f"tags.dagster_run_id='{dagster_run_id}'",
             )
             if not current_run_df.empty:
-                return current_run_df.run_id.values[0]
+                return current_run_df.run_id.values[0]  # pylint: disable=no-member
 
     def _set_active_run(self, run_id=None):
-        """This method sets the active run to be that of the specified
+        """
+        This method sets the active run to be that of the specified
         run_id. If None is passed then a new run is started. The new run also
         takes care of nested runs.
 
         Args:
             run_id (str, optional): Mlflow run_id. Defaults to None.
         """
         nested_run = False
         if self.parent_run_id is not None:
             self._start_run(run_id=self.parent_run_id, run_name=self.run_name)
             nested_run = True
         self._start_run(run_id=run_id, run_name=self.run_name, nested=nested_run)
 
     def _start_run(self, **kwargs):
-        """Catches the Mlflow exception if a run is already active."""
+        """
+        Catches the Mlflow exception if a run is already active.
+        """
+
         try:
             run = mlflow.start_run(**kwargs)
             self.log.info(
                 f"Starting a new mlflow run with id {run.info.run_id} "
                 f"in experiment {self.experiment_name}"
             )
         except Exception as ex:
@@ -216,32 +223,34 @@
         it = iter(params)
         for _ in range(0, len(params), size):
             yield {k: params[k] for k in islice(it, size)}
 
 
 @resource(config_schema=CONFIG_SCHEMA)
 def mlflow_tracking(context):
-    """This resource initializes an MLflow run that's used for all steps within a Dagster run.
+    """
+    This resource initializes an MLflow run that's used for all steps within a Dagster run.
 
     This resource provides access to all of mlflow's methods as well as the mlflow tracking client's
     methods.
 
     Usage:
 
-    1. Add the mlflow resource to any ops in which you want to invoke mlflow tracking APIs.
-    2. Add the `end_mlflow_on_run_finished` hook to your job to end the MLflow run
+    1. Add the mlflow resource to any solids in which you want to invoke mlflow tracking APIs.
+    2. Add the `end_mlflow_on_run_finished` hook to your pipeline to end the MLflow run
        when the Dagster run is finished.
 
     Examples:
+
         .. code-block:: python
 
             from dagster_mlflow import end_mlflow_on_run_finished, mlflow_tracking
 
             @op(required_resource_keys={"mlflow"})
-            def mlflow_op(context):
+            def mlflow_solid(context):
                 mlflow.log_params(some_params)
                 mlflow.tracking.MlflowClient().create_registered_model(some_model_name)
 
             @end_mlflow_on_run_finished
             @job(resource_defs={"mlflow": mlflow_tracking})
             def mlf_example():
                 mlflow_op()
```

### Comparing `dagster-mlflow-0.19.6/setup.py` & `dagster-mlflow-1.0.5/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-from pathlib import Path
 from typing import Dict
 
 from setuptools import find_packages, setup
 
 
 def get_version() -> str:
     version: Dict[str, str] = {}
-    with open(Path(__file__).parent / "dagster_mlflow/version.py", encoding="utf8") as fp:
-        exec(fp.read(), version)
+    with open("dagster_mlflow/version.py", encoding="utf8") as fp:
+        exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
-setup(
-    name="dagster-mlflow",
-    version=get_version(),
-    author="Elementl",
-    author_email="hello@elementl.com",
-    license="Apache-2.0",
-    description="Package for mlflow Dagster framework components.",
-    url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mlflow",
-    classifiers=[
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: OS Independent",
-    ],
-    packages=find_packages(exclude=["dagster_mlflow_tests*"]),
-    install_requires=["dagster", "mlflow", "pandas"],
-    zip_safe=False,
-)
+if __name__ == "__main__":
+    setup(
+        name="dagster-mlflow",
+        version=get_version(),
+        author="Elementl",
+        author_email="hello@elementl.com",
+        license="Apache-2.0",
+        description="Package for mlflow Dagster framework components.",
+        url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mlflow",
+        classifiers=[
+            "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "License :: OSI Approved :: Apache Software License",
+            "Operating System :: OS Independent",
+        ],
+        packages=find_packages(exclude=["dagster_mlflow_tests*"]),
+        install_requires=[
+            "dagster",
+            "mlflow<=1.26.0",  # https://github.com/mlflow/mlflow/issues/5968
+            "pandas",
+        ],
+        zip_safe=False,
+    )
```

