# Comparing `tmp/dagster-celery-docker-0.9.9rc1.tar.gz` & `tmp/dagster-celery-docker-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-celery-docker-0.9.9rc1.tar", last modified: Thu Sep 17 21:09:03 2020, max compression
+gzip compressed data, was "dagster-celery-docker-1.0.5.tar", last modified: Fri Aug 26 13:45:53 2022, max compression
```

## Comparing `dagster-celery-docker-0.9.9rc1.tar` & `dagster-celery-docker-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)      583 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      149 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker/
--rw-r--r--   0 bobchen    (501) staff       (20)      209 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      312 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker/app.py
--rw-r--r--   0 bobchen    (501) staff       (20)    13029 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker/executor.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      583 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      597 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       46 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       50 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2702 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker_tests/test_execute_docker.py
--rw-r--r--   0 bobchen    (501) staff       (20)      207 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker_tests/test_inclusion.py
--rw-r--r--   0 bobchen    (501) staff       (20)       99 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       38 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1072 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:53.124595 dagster-celery-docker-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-celery-docker-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       55 2022-08-26 13:33:01.000000 dagster-celery-docker-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      620 2022-08-26 13:45:53.124595 dagster-celery-docker-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      149 2022-08-26 13:33:01.000000 dagster-celery-docker-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:53.120595 dagster-celery-docker-1.0.5/dagster_celery_docker/
+-rw-r--r--   0 root         (0) root         (0)      210 2022-08-26 13:33:01.000000 dagster-celery-docker-1.0.5/dagster_celery_docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      346 2022-08-26 13:33:01.000000 dagster-celery-docker-1.0.5/dagster_celery_docker/app.py
+-rw-r--r--   0 root         (0) root         (0)    13117 2022-08-26 13:33:01.000000 dagster-celery-docker-1.0.5/dagster_celery_docker/executor.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-celery-docker-1.0.5/dagster_celery_docker/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-celery-docker-1.0.5/dagster_celery_docker/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:53.124595 dagster-celery-docker-1.0.5/dagster_celery_docker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      620 2022-08-26 13:45:53.000000 dagster-celery-docker-1.0.5/dagster_celery_docker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      477 2022-08-26 13:45:53.000000 dagster-celery-docker-1.0.5/dagster_celery_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:53.000000 dagster-celery-docker-1.0.5/dagster_celery_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:53.000000 dagster-celery-docker-1.0.5/dagster_celery_docker.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       67 2022-08-26 13:45:53.000000 dagster-celery-docker-1.0.5/dagster_celery_docker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:45:53.000000 dagster-celery-docker-1.0.5/dagster_celery_docker.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2022-08-26 13:45:53.124595 dagster-celery-docker-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1391 2022-08-26 13:33:01.000000 dagster-celery-docker-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-celery-docker-0.9.9rc1/PKG-INFO` & `dagster-celery-docker-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-celery-docker
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: A Dagster integration for celery-docker
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-celery-docker
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

### Comparing `dagster-celery-docker-0.9.9rc1/dagster_celery_docker/executor.py` & `dagster-celery-docker-1.0.5/dagster_celery_docker/executor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,37 @@
+import json
 import os
 
 import docker.client
 from dagster_celery.config import DEFAULT_CONFIG, dict_wrapper
 from dagster_celery.core_execution_loop import DELEGATE_MARKER, core_celery_execution_loop
 from dagster_celery.defaults import broker_url, result_backend
 from dagster_celery.executor import CELERY_CONFIG
-from dagster_graphql.client.mutations import handle_execute_plan_result, handle_execution_errors
 
-from dagster import (
-    DagsterInstance,
-    EventMetadataEntry,
-    Executor,
-    Field,
-    StringSource,
-    check,
-    executor,
-    seven,
-)
-from dagster.core.definitions.executor import check_cross_process_constraints
-from dagster.core.events import EngineEventData
-from dagster.core.execution.retries import Retries
-from dagster.core.host_representation.handle import IN_PROCESS_NAME
-from dagster.core.instance import InstanceRef
-from dagster.serdes import serialize_dagster_namedtuple
-from dagster.seven import JSONDecodeError
-from dagster.utils import merge_dicts
+from dagster import DagsterInstance, Executor, Field, MetadataEntry, Permissive, StringSource
+from dagster import _check as check
+from dagster import executor, multiple_process_executor_requirements
+from dagster._cli.api import ExecuteStepArgs
+from dagster._core.events import EngineEventData
+from dagster._core.events.utils import filter_dagster_events_from_cli_logs
+from dagster._core.execution.retries import RetryMode
+from dagster._core.storage.pipeline_run import PipelineRun
+from dagster._serdes import pack_value, serialize_dagster_namedtuple, unpack_value
+from dagster._utils import merge_dicts
 
 CELERY_DOCKER_CONFIG_KEY = "celery-docker"
 
 
 def celery_docker_config():
     additional_config = {
         "docker": Field(
             {
                 "image": Field(
                     StringSource,
-                    is_required=True,
+                    is_required=False,
                     description="The docker image to be used for step execution.",
                 ),
                 "registry": Field(
                     {
                         "url": Field(StringSource),
                         "username": Field(StringSource),
                         "password": Field(StringSource),
@@ -48,216 +40,213 @@
                     description="Information for using a non local/public docker registry",
                 ),
                 "env_vars": Field(
                     [str],
                     is_required=False,
                     description="The list of environment variables names to forward from the celery worker in to the docker container",
                 ),
+                "network": Field(
+                    str,
+                    is_required=False,
+                    description="Name of the network this container will be connected to at creation time",
+                ),
+                "container_kwargs": Field(
+                    Permissive(),
+                    is_required=False,
+                    description="Additional keyword args for the docker container",
+                ),
             },
             is_required=True,
             description="The configuration for interacting with docker in the celery worker.",
         ),
-        "repo_location_name": Field(
-            StringSource,
-            is_required=False,
-            default_value=IN_PROCESS_NAME,
-            description="[temporary workaround] The repository location name to use for execution.",
-        ),
     }
 
     cfg = merge_dicts(CELERY_CONFIG, additional_config)
     return cfg
 
 
-@executor(name=CELERY_DOCKER_CONFIG_KEY, config_schema=celery_docker_config())
+@executor(
+    name=CELERY_DOCKER_CONFIG_KEY,
+    config_schema=celery_docker_config(),
+    requirements=multiple_process_executor_requirements(),
+)
 def celery_docker_executor(init_context):
     """Celery-based executor which launches tasks in docker containers.
 
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
+    different requirements around idempotence or retry, it may make sense to execute jobs
     with variations on these settings.
 
-    If you'd like to configure a Celery Docker executor in addition to the
-    :py:class:`~dagster.default_executors`, you should add it to the ``executor_defs`` defined on a
-    :py:class:`~dagster.ModeDefinition` as follows:
+    To use the `celery_docker_executor`, set it as the `executor_def` when defining a job:
 
     .. code-block:: python
 
-        from dagster import ModeDefinition, default_executors, pipeline
+        from dagster import job
         from dagster_celery_docker.executor import celery_docker_executor
 
-        @pipeline(mode_defs=[
-            ModeDefinition(executor_defs=default_executors + [celery_docker_executor])
-        ])
-        def celery_enabled_pipeline():
+        @job(executor_def=celery_docker_executor)
+        def celery_enabled_job():
             pass
 
     Then you can configure the executor as follows:
 
     .. code-block:: YAML
 
         execution:
-          celery-docker:
-            config:
-
-              docker:
-                image: 'my_repo.com/image_name:latest'
-                registry:
-                  url: 'my_repo.com'
-                  username: 'my_user'
-                  password: {env: 'DOCKER_PASSWORD'}
-                env_vars: ["DAGSTER_HOME"] # environment vars to pass from celery worker to docker
-
-              broker: 'pyamqp://guest@localhost//'  # Optional[str]: The URL of the Celery broker
-              backend: 'rpc://' # Optional[str]: The URL of the Celery results backend
-              include: ['my_module'] # Optional[List[str]]: Modules every worker should import
-              config_source: # Dict[str, Any]: Any additional parameters to pass to the
-                  #...       # Celery workers. This dict will be passed as the `config_source`
-                  #...       # argument of celery.Celery().
+          config:
+            docker:
+              image: 'my_repo.com/image_name:latest'
+              registry:
+                url: 'my_repo.com'
+                username: 'my_user'
+                password: {env: 'DOCKER_PASSWORD'}
+              env_vars: ["DAGSTER_HOME"] # environment vars to pass from celery worker to docker
+              container_kwargs: # keyword args to be passed to the container. example:
+                volumes: ['/home/user1/:/mnt/vol2','/var/www:/mnt/vol1']
+
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
 
-    In deployments where the celery_k8s_job_executor is used all appropriate celery and dagster_celery
+    In deployments where the celery_docker_job_executor is used all appropriate celery and dagster_celery
     commands must be invoked with the `-A dagster_celery_docker.app` argument.
     """
-    check_cross_process_constraints(init_context)
 
     exc_cfg = init_context.executor_config
 
     return CeleryDockerExecutor(
         broker=exc_cfg.get("broker"),
         backend=exc_cfg.get("backend"),
         config_source=exc_cfg.get("config_source"),
         include=exc_cfg.get("include"),
-        retries=Retries.from_config(exc_cfg.get("retries")),
+        retries=RetryMode.from_config(exc_cfg.get("retries")),
         docker_config=exc_cfg.get("docker"),
-        repo_location_name=exc_cfg.get("repo_location_name"),
     )
 
 
 class CeleryDockerExecutor(Executor):
     def __init__(
         self,
         retries,
         docker_config,
         broker=None,
         backend=None,
         include=None,
         config_source=None,
-        repo_location_name=None,
     ):
-        self._retries = check.inst_param(retries, "retries", Retries)
+        self._retries = check.inst_param(retries, "retries", RetryMode)
         self.broker = check.opt_str_param(broker, "broker", default=broker_url)
         self.backend = check.opt_str_param(backend, "backend", default=result_backend)
         self.include = check.opt_list_param(include, "include", of_type=str)
         self.config_source = dict_wrapper(
             dict(DEFAULT_CONFIG, **check.opt_dict_param(config_source, "config_source"))
         )
         self.docker_config = check.dict_param(docker_config, "docker_config")
-        self.repo_location_name = check.str_param(repo_location_name, "repo_location_name")
 
     @property
     def retries(self):
         return self._retries
 
-    def execute(self, pipeline_context, execution_plan):
+    def execute(self, plan_context, execution_plan):
 
         return core_celery_execution_loop(
-            pipeline_context, execution_plan, step_execution_fn=_submit_task_docker
+            plan_context, execution_plan, step_execution_fn=_submit_task_docker
         )
 
     def app_args(self):
         return {
             "broker": self.broker,
             "backend": self.backend,
             "include": self.include,
             "config_source": self.config_source,
             "retries": self.retries,
         }
 
 
-def _submit_task_docker(app, pipeline_context, step, queue, priority):
-    task = create_docker_task(app)
-
-    recon_repo = pipeline_context.pipeline.get_reconstructable_repository()
+def _submit_task_docker(app, plan_context, step, queue, priority, known_state):
+    execute_step_args = ExecuteStepArgs(
+        pipeline_origin=plan_context.reconstructable_pipeline.get_python_origin(),
+        pipeline_run_id=plan_context.pipeline_run.run_id,
+        step_keys_to_execute=[step.key],
+        instance_ref=plan_context.instance.get_ref(),
+        retry_mode=plan_context.executor.retries.for_inner_plan(),
+        known_state=known_state,
+    )
 
+    task = create_docker_task(app)
     task_signature = task.si(
-        instance_ref_dict=pipeline_context.instance.get_ref().to_dict(),
-        step_keys=[step.key],
-        run_config=pipeline_context.pipeline_run.run_config,
-        mode=pipeline_context.pipeline_run.mode,
-        repo_name=recon_repo.get_definition().name,
-        repo_location_name=pipeline_context.executor.repo_location_name,
-        run_id=pipeline_context.pipeline_run.run_id,
-        docker_config=pipeline_context.executor.docker_config,
+        execute_step_args_packed=pack_value(execute_step_args),
+        docker_config=plan_context.executor.docker_config,
     )
     return task_signature.apply_async(
         priority=priority,
         queue=queue,
         routing_key="{queue}.execute_step_docker".format(queue=queue),
     )
 
 
 def create_docker_task(celery_app, **task_kwargs):
     @celery_app.task(bind=True, name="execute_step_docker", **task_kwargs)
     def _execute_step_docker(
         self,
-        instance_ref_dict,
-        step_keys,
-        run_config,
-        mode,
-        repo_name,
-        repo_location_name,
-        run_id,
+        execute_step_args_packed,
         docker_config,
     ):
-        """Run step execution in a Docker container.
-        """
-        instance_ref = InstanceRef.from_dict(instance_ref_dict)
-        instance = DagsterInstance.from_ref(instance_ref)
-        pipeline_run = instance.get_run_by_id(run_id)
-        check.invariant(pipeline_run, "Could not load run {}".format(run_id))
-
-        step_keys_str = ", ".join(step_keys)
-
-        variables = {
-            "executionParams": {
-                "runConfigData": run_config,
-                "mode": mode,
-                "selector": {
-                    "repositoryLocationName": repo_location_name,
-                    "repositoryName": repo_name,
-                    "pipelineName": pipeline_run.pipeline_name,
-                    "solidSelection": list(pipeline_run.solids_to_execute)
-                    if pipeline_run.solids_to_execute
-                    else None,
-                },
-                "executionMetadata": {"runId": run_id},
-                "stepKeys": step_keys,
-            }
-        }
+        """Run step execution in a Docker container."""
+        execute_step_args = unpack_value(
+            check.dict_param(
+                execute_step_args_packed,
+                "execute_step_args_packed",
+            )
+        )
+        check.inst_param(execute_step_args, "execute_step_args", ExecuteStepArgs)
+
+        check.dict_param(docker_config, "docker_config")
+
+        instance = DagsterInstance.from_ref(execute_step_args.instance_ref)
+        pipeline_run = instance.get_run_by_id(execute_step_args.pipeline_run_id)
+        check.inst(
+            pipeline_run,
+            PipelineRun,
+            "Could not load run {}".format(execute_step_args.pipeline_run_id),
+        )
+        step_keys_str = ", ".join(execute_step_args.step_keys_to_execute)
+
+        input_json = serialize_dagster_namedtuple(execute_step_args)
+
+        command = "dagster api execute_step {}".format(json.dumps(input_json))
 
-        command = "dagster-graphql -v '{variables}' -p executePlan".format(
-            variables=seven.json.dumps(variables)
+        docker_image = (
+            docker_config["image"]
+            if docker_config.get("image")
+            else pipeline_run.pipeline_code_origin.repository_origin.container_image
         )
-        docker_image = docker_config["image"]
+
+        if not docker_image:
+            raise Exception("No docker image specified by either the job or the repository")
+
         client = docker.client.from_env()
 
         if docker_config.get("registry"):
             client.login(
                 registry=docker_config["registry"]["url"],
                 username=docker_config["registry"]["username"],
                 password=docker_config["registry"]["password"],
@@ -265,76 +254,76 @@
 
         # Post event for starting execution
         engine_event = instance.report_engine_event(
             "Executing steps {} in Docker container {}".format(step_keys_str, docker_image),
             pipeline_run,
             EngineEventData(
                 [
-                    EventMetadataEntry.text(step_keys_str, "Step keys"),
-                    EventMetadataEntry.text(docker_image, "Image"),
-                    EventMetadataEntry.text(self.request.hostname, "Celery worker"),
+                    MetadataEntry("Step keys", value=step_keys_str),
+                    MetadataEntry("Image", value=docker_image),
+                    MetadataEntry("Celery worker", value=self.request.hostname),
                 ],
                 marker_end=DELEGATE_MARKER,
             ),
             CeleryDockerExecutor,
-            step_key=step_keys[0],
+            step_key=execute_step_args.step_keys_to_execute[0],
         )
 
-        events = [engine_event]
+        serialized_events = [serialize_dagster_namedtuple(engine_event)]
 
         docker_env = {}
         if docker_config.get("env_vars"):
             docker_env = {env_name: os.getenv(env_name) for env_name in docker_config["env_vars"]}
 
+        container_kwargs = check.opt_dict_param(
+            docker_config.get("container_kwargs"), "container_kwargs", key_type=str
+        )
+
+        # set defaults for detach and auto_remove
+        container_kwargs["detach"] = container_kwargs.get("detach", False)
+        container_kwargs["auto_remove"] = container_kwargs.get("auto_remove", True)
+
+        # if environment variables are provided via container_kwargs, merge with env_vars
+        if container_kwargs.get("environment") is not None:
+            e_vars = container_kwargs.get("environment")
+            if isinstance(e_vars, dict):
+                docker_env.update(e_vars)
+            else:
+                for v in e_vars:
+                    key, val = v.split("=")
+                    docker_env[key] = val
+            del container_kwargs["environment"]
+
         try:
             docker_response = client.containers.run(
                 docker_image,
                 command=command,
-                detach=False,
-                auto_remove=True,
                 # pass through this worker's environment for things like AWS creds etc.
                 environment=docker_env,
+                network=docker_config.get("network", None),
+                **container_kwargs,
             )
-            res = seven.json.loads(docker_response)
 
+            res = docker_response.decode("utf-8")
         except docker.errors.ContainerError as err:
-            instance.report_engine_event(
-                "Failed to run steps {} in Docker container {}".format(step_keys_str, docker_image),
-                pipeline_run,
-                EngineEventData(
-                    [
-                        EventMetadataEntry.text(docker_image, "Job image"),
-                        EventMetadataEntry.text(err.stderr, "Docker stderr"),
-                    ],
-                ),
-                CeleryDockerExecutor,
-                step_key=step_keys[0],
-            )
-            raise
+            entries = [MetadataEntry("Job image", value=docker_image)]
+            if err.stderr is not None:
+                entries.append(MetadataEntry("Docker stderr", value=err.stderr))
 
-        except JSONDecodeError:
             instance.report_engine_event(
-                "Failed to parse response for steps {} from Docker container {}".format(
-                    step_keys_str, docker_image
-                ),
+                "Failed to run steps {} in Docker container {}".format(step_keys_str, docker_image),
                 pipeline_run,
-                EngineEventData(
-                    [
-                        EventMetadataEntry.text(docker_image, "Job image"),
-                        EventMetadataEntry.text(docker_response, "Docker Response"),
-                    ],
-                ),
+                EngineEventData(entries),
                 CeleryDockerExecutor,
-                step_key=step_keys[0],
+                step_key=execute_step_args.step_keys_to_execute[0],
             )
             raise
-
         else:
-            handle_execution_errors(res, "executePlan")
-            step_events = handle_execute_plan_result(res)
+            if res is None:
+                raise Exception("No response from execute_step in CeleryDockerExecutor")
 
-        events += step_events
+            events = filter_dagster_events_from_cli_logs(res.split("\n"))
+            serialized_events += [serialize_dagster_namedtuple(event) for event in events]
 
-        serialized_events = [serialize_dagster_namedtuple(event) for event in events]
         return serialized_events
 
     return _execute_step_docker
```

### Comparing `dagster-celery-docker-0.9.9rc1/dagster_celery_docker.egg-info/PKG-INFO` & `dagster-celery-docker-1.0.5/dagster_celery_docker.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-celery-docker
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: A Dagster integration for celery-docker
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-celery-docker
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

### Comparing `dagster-celery-docker-0.9.9rc1/setup.py` & `dagster-celery-docker-1.0.5/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,41 @@
+from typing import Dict
+
 from setuptools import find_packages, setup
 
 
-def get_version():
-    version = {}
-    with open("dagster_celery_docker/version.py") as fp:
+def get_version() -> str:
+    version: Dict[str, str] = {}
+    with open("dagster_celery_docker/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
 if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
     setup(
         name="dagster-celery-docker",
-        version=get_version(),
+        version=ver,
         author="Elementl",
         license="Apache-2.0",
         description="A Dagster integration for celery-docker",
         url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-celery-docker",
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
-        install_requires=["dagster", "dagster-celery", "dagster-graphql", "docker"],
-        tests_require=[],
+        packages=find_packages(exclude=["dagster_celery_docker_tests*"]),
+        install_requires=[
+            "dagster==1.0.5",
+            "dagster-celery==1.0.5",
+            "dagster-graphql==1.0.5",
+            "docker",
+        ],
         zip_safe=False,
     )
```

