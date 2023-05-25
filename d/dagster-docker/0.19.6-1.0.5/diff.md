# Comparing `tmp/dagster-docker-0.19.6.tar.gz` & `tmp/dagster-docker-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-docker-0.19.6.tar", last modified: Thu May 25 17:26:16 2023, max compression
+gzip compressed data, was "dagster-docker-1.0.5.tar", last modified: Fri Aug 26 13:44:58 2022, max compression
```

## Comparing `dagster-docker-0.19.6.tar` & `dagster-docker-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:26:16.345965 dagster-docker-0.19.6/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-05-25 17:16:50.000000 dagster-docker-0.19.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-25 17:16:50.000000 dagster-docker-0.19.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      656 2023-05-25 17:26:16.345965 dagster-docker-0.19.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2023-05-25 17:16:50.000000 dagster-docker-0.19.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:26:16.345965 dagster-docker-0.19.6/dagster_docker/
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-25 17:16:50.000000 dagster-docker-0.19.6/dagster_docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6470 2023-05-25 17:16:50.000000 dagster-docker-0.19.6/dagster_docker/container_context.py
--rw-r--r--   0 root         (0) root         (0)    11738 2023-05-25 17:16:50.000000 dagster-docker-0.19.6/dagster_docker/docker_executor.py
--rw-r--r--   0 root         (0) root         (0)     7426 2023-05-25 17:16:50.000000 dagster-docker-0.19.6/dagster_docker/docker_run_launcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:26:16.345965 dagster-docker-0.19.6/dagster_docker/ops/
--rw-r--r--   0 root         (0) root         (0)      143 2023-05-25 17:16:50.000000 dagster-docker-0.19.6/dagster_docker/ops/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6365 2023-05-25 17:16:50.000000 dagster-docker-0.19.6/dagster_docker/ops/docker_container_op.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-25 17:16:50.000000 dagster-docker-0.19.6/dagster_docker/py.typed
--rw-r--r--   0 root         (0) root         (0)     1892 2023-05-25 17:16:50.000000 dagster-docker-0.19.6/dagster_docker/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-25 17:16:50.000000 dagster-docker-0.19.6/dagster_docker/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:26:16.345965 dagster-docker-0.19.6/dagster_docker.egg-info/
--rw-r--r--   0 root         (0) root         (0)      656 2023-05-25 17:26:16.000000 dagster-docker-0.19.6/dagster_docker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      556 2023-05-25 17:26:16.000000 dagster-docker-0.19.6/dagster_docker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:26:16.000000 dagster-docker-0.19.6/dagster_docker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:26:16.000000 dagster-docker-0.19.6/dagster_docker.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-25 17:26:16.000000 dagster-docker-0.19.6/dagster_docker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-25 17:26:16.000000 dagster-docker-0.19.6/dagster_docker.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      125 2023-05-25 17:26:16.349965 dagster-docker-0.19.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1391 2023-05-25 17:16:50.000000 dagster-docker-0.19.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:58.028292 dagster-docker-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-docker-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       48 2022-08-26 13:33:01.000000 dagster-docker-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      632 2022-08-26 13:44:58.028292 dagster-docker-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2022-08-26 13:33:01.000000 dagster-docker-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:58.028292 dagster-docker-1.0.5/dagster_docker/
+-rw-r--r--   0 root         (0) root         (0)      254 2022-08-26 13:33:01.000000 dagster-docker-1.0.5/dagster_docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6406 2022-08-26 13:33:01.000000 dagster-docker-1.0.5/dagster_docker/container_context.py
+-rw-r--r--   0 root         (0) root         (0)    10233 2022-08-26 13:33:01.000000 dagster-docker-1.0.5/dagster_docker/docker_executor.py
+-rw-r--r--   0 root         (0) root         (0)     7121 2022-08-26 13:33:01.000000 dagster-docker-1.0.5/dagster_docker/docker_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-docker-1.0.5/dagster_docker/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1818 2022-08-26 13:33:01.000000 dagster-docker-1.0.5/dagster_docker/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-docker-1.0.5/dagster_docker/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:58.028292 dagster-docker-1.0.5/dagster_docker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      632 2022-08-26 13:44:57.000000 dagster-docker-1.0.5/dagster_docker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      483 2022-08-26 13:44:57.000000 dagster-docker-1.0.5/dagster_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:44:57.000000 dagster-docker-1.0.5/dagster_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:44:57.000000 dagster-docker-1.0.5/dagster_docker.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2022-08-26 13:44:57.000000 dagster-docker-1.0.5/dagster_docker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-08-26 13:44:57.000000 dagster-docker-1.0.5/dagster_docker.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      125 2022-08-26 13:44:58.032292 dagster-docker-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1308 2022-08-26 13:33:01.000000 dagster-docker-1.0.5/setup.py
```

### Comparing `dagster-docker-0.19.6/LICENSE` & `dagster-docker-1.0.5/LICENSE`

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

### Comparing `dagster-docker-0.19.6/dagster_docker/container_context.py` & `dagster-docker-1.0.5/dagster_docker/container_context.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-from typing import TYPE_CHECKING, Any, Mapping, NamedTuple, Optional, Sequence, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Mapping, NamedTuple, Optional, cast
 
-from dagster import (
-    Array,
-    Field,
-    Permissive,
-    StringSource,
-    _check as check,
-)
+from dagster import Array, Field, Permissive, StringSource
+from dagster import _check as check
 from dagster._config import process_config
 from dagster._core.container_context import process_shared_container_context_config
 from dagster._core.errors import DagsterInvalidConfigError
-from dagster._core.storage.dagster_run import DagsterRun
+from dagster._core.storage.pipeline_run import PipelineRun
+from dagster._utils import merge_dicts
 
 if TYPE_CHECKING:
     from . import DockerRunLauncher
 
 DOCKER_CONTAINER_CONTEXT_SCHEMA = {
     "registry": Field(
         {
@@ -24,105 +20,100 @@
         },
         is_required=False,
         description="Information for using a non local/public docker registry",
     ),
     "env_vars": Field(
         [str],
         is_required=False,
-        description=(
-            "The list of environment variables names to include in the docker container. "
-            "Each can be of the form KEY=VALUE or just KEY (in which case the value will be pulled "
-            "from the local environment)"
-        ),
+        description="The list of environment variables names to include in the docker container. "
+        "Each can be of the form KEY=VALUE or just KEY (in which case the value will be pulled "
+        "from the local environment)",
     ),
     "container_kwargs": Field(
         Permissive(),
         is_required=False,
-        description=(
-            "key-value pairs that can be passed into containers.create. See "
-            "https://docker-py.readthedocs.io/en/stable/containers.html for the full list "
-            "of available options."
-        ),
+        description="key-value pairs that can be passed into containers.create. See "
+        "https://docker-py.readthedocs.io/en/stable/containers.html for the full list "
+        "of available options.",
     ),
     "networks": Field(
         Array(StringSource),
         is_required=False,
-        description=(
-            "Names of the networks to which to connect the launched container at creation time"
-        ),
+        description="Names of the networks to which to connect the launched container at creation time",
     ),
 }
 
 
 class DockerContainerContext(
     NamedTuple(
         "_DockerContainerContext",
         [
-            ("registry", Optional[Mapping[str, str]]),
-            ("env_vars", Sequence[str]),
-            ("networks", Sequence[str]),
-            ("container_kwargs", Mapping[str, Any]),
+            ("registry", Optional[Dict[str, str]]),
+            ("env_vars", List[str]),
+            ("networks", List[str]),
+            ("container_kwargs", Dict[str, Any]),
         ],
     )
 ):
     """Encapsulates the configuration that can be applied to a Docker container running
     Dagster code. Can be set at the instance level (via config in the `DockerRunLauncher`),
     repository location level, and at the individual step level (for runs using the
     `docker_executor` to run each op in its own container). Config at each of these lower levels is
     merged in with any config set at a higher level, following the policy laid out in the
     merge() method below.
     """
 
     def __new__(
         cls,
-        registry: Optional[Mapping[str, str]] = None,
-        env_vars: Optional[Sequence[str]] = None,
-        networks: Optional[Sequence[str]] = None,
-        container_kwargs: Optional[Mapping[str, Any]] = None,
+        registry: Optional[Dict[str, str]] = None,
+        env_vars: Optional[List[str]] = None,
+        networks: Optional[List[str]] = None,
+        container_kwargs: Optional[Dict[str, Any]] = None,
     ):
         return super(DockerContainerContext, cls).__new__(
             cls,
-            registry=check.opt_nullable_mapping_param(registry, "registry"),
-            env_vars=check.opt_sequence_param(env_vars, "env_vars", of_type=str),
-            networks=check.opt_sequence_param(networks, "networks", of_type=str),
-            container_kwargs=check.opt_mapping_param(container_kwargs, "container_kwargs"),
+            registry=check.dict_param(registry, "registry") if registry != None else None,
+            env_vars=check.opt_list_param(env_vars, "env_vars", of_type=str),
+            networks=check.opt_list_param(networks, "networks", of_type=str),
+            container_kwargs=check.opt_dict_param(container_kwargs, "container_kwargs"),
         )
 
     def merge(self, other: "DockerContainerContext"):
         # Combines config set at a higher level with overrides/additions that are set at a lower
         # level. For example, a certain set of config set in the `DockerRunLauncher`` can be
         # combined with config set at the step level in the `docker_executor`.
         # Lists of env vars and secrets are appended, the registry is replaced, and the
         # `container_kwargs` field does a shallow merge so that different kwargs can be combined
         # or replaced without replacing the full set of arguments.
         return DockerContainerContext(
-            registry=other.registry if other.registry is not None else self.registry,
-            env_vars=[*self.env_vars, *other.env_vars],
-            networks=[*self.networks, *other.networks],
-            container_kwargs={**self.container_kwargs, **other.container_kwargs},
+            registry=other.registry if other.registry != None else self.registry,
+            env_vars=self.env_vars + other.env_vars,
+            networks=self.networks + other.networks,
+            container_kwargs=merge_dicts(other.container_kwargs, self.container_kwargs),
         )
 
     @staticmethod
-    def create_for_run(dagster_run: DagsterRun, run_launcher: Optional["DockerRunLauncher"]):
+    def create_for_run(pipeline_run: PipelineRun, run_launcher: Optional["DockerRunLauncher"]):
+
         context = DockerContainerContext()
 
         # First apply the instance / run_launcher-level context
         if run_launcher:
             context = context.merge(
                 DockerContainerContext(
                     registry=run_launcher.registry,
                     env_vars=run_launcher.env_vars,
                     networks=run_launcher.networks,
                     container_kwargs=run_launcher.container_kwargs,
                 )
             )
 
         run_container_context = (
-            dagster_run.job_code_origin.repository_origin.container_context
-            if dagster_run.job_code_origin
+            pipeline_run.pipeline_code_origin.repository_origin.container_context
+            if pipeline_run.pipeline_code_origin
             else None
         )
 
         if not run_container_context:
             return context
 
         return context.merge(DockerContainerContext.create_from_config(run_container_context))
```

### Comparing `dagster-docker-0.19.6/dagster_docker/docker_executor.py` & `dagster-docker-1.0.5/dagster_docker/docker_executor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,48 @@
 from typing import Iterator, Optional, cast
 
-import dagster._check as check
 import docker
-import docker.errors
-from dagster import Field, IntSource, executor
+from dagster_docker.utils import DOCKER_CONFIG_SCHEMA, validate_docker_config, validate_docker_image
+
+import dagster._check as check
+from dagster import executor
 from dagster._annotations import experimental
 from dagster._core.definitions.executor_definition import multiple_process_executor_requirements
-from dagster._core.events import DagsterEvent, EngineEventData
+from dagster._core.events import DagsterEvent, EngineEventData, MetadataEntry
 from dagster._core.execution.retries import RetryMode, get_retries_config
-from dagster._core.execution.tags import get_tag_concurrency_limits_config
 from dagster._core.executor.base import Executor
 from dagster._core.executor.init import InitExecutorContext
 from dagster._core.executor.step_delegating import StepDelegatingExecutor
 from dagster._core.executor.step_delegating.step_handler.base import (
     CheckStepHealthResult,
     StepHandler,
     StepHandlerContext,
 )
-from dagster._core.origin import JobPythonOrigin
+from dagster._core.origin import PipelinePythonOrigin
 from dagster._core.utils import parse_env_var
-from dagster._grpc.types import ExecuteStepArgs
 from dagster._serdes.utils import hash_str
-from dagster._utils.merger import merge_dicts
-
-from dagster_docker.utils import DOCKER_CONFIG_SCHEMA, validate_docker_config, validate_docker_image
+from dagster._utils import merge_dicts
 
 from .container_context import DockerContainerContext
 
 
 @executor(
     name="docker",
     config_schema=merge_dicts(
         DOCKER_CONFIG_SCHEMA,
         {
             "retries": get_retries_config(),
-            "max_concurrent": Field(
-                IntSource,
-                is_required=False,
-                description=(
-                    "Limit on the number of containers that will run concurrently within the scope "
-                    "of a Dagster run. Note that this limit is per run, not global."
-                ),
-            ),
-            "tag_concurrency_limits": get_tag_concurrency_limits_config(),
         },
     ),
     requirements=multiple_process_executor_requirements(),
 )
 @experimental
 def docker_executor(init_context: InitExecutorContext) -> Executor:
-    """Executor which launches steps as Docker containers.
+    """
+    Executor which launches steps as Docker containers.
 
     To use the `docker_executor`, set it as the `executor_def` when defining a job:
 
     .. literalinclude:: ../../../../../../python_modules/libraries/dagster-docker/dagster_docker_tests/test_example_executor.py
        :start-after: start_marker
        :end-before: end_marker
        :language: python
@@ -68,24 +57,23 @@
             network: ...
             networks: ...
             container_kwargs: ...
 
     If you're using the DockerRunLauncher, configuration set on the containers created by the run
     launcher will also be set on the containers that are created for each step.
     """
+
     config = init_context.executor_config
     image = check.opt_str_elem(config, "image")
     registry = check.opt_dict_elem(config, "registry", key_type=str)
     env_vars = check.opt_list_elem(config, "env_vars", of_type=str)
     network = check.opt_str_elem(config, "network")
     networks = check.opt_list_elem(config, "networks", of_type=str)
     container_kwargs = check.opt_dict_elem(config, "container_kwargs", key_type=str)
     retries = check.dict_elem(config, "retries", key_type=str)
-    max_concurrent = check.opt_int_elem(config, "max_concurrent")
-    tag_concurrency_limits = check.opt_list_elem(config, "tag_concurrency_limits")
 
     validate_docker_config(network, networks, container_kwargs)
 
     if network and not networks:
         networks = [network]
 
     container_context = DockerContainerContext(
@@ -94,16 +82,14 @@
         networks=networks or [],
         container_kwargs=container_kwargs,
     )
 
     return StepDelegatingExecutor(
         DockerStepHandler(image, container_context),
         retries=check.not_none(RetryMode.from_config(retries)),
-        max_concurrent=max_concurrent,
-        tag_concurrency_limits=tag_concurrency_limits,
     )
 
 
 class DockerStepHandler(StepHandler):
     def __init__(
         self,
         image: Optional[str],
@@ -116,15 +102,15 @@
             container_context, "container_context", DockerContainerContext
         )
 
     def _get_image(self, step_handler_context: StepHandlerContext):
         from . import DockerRunLauncher
 
         image = cast(
-            JobPythonOrigin, step_handler_context.dagster_run.job_code_origin
+            PipelinePythonOrigin, step_handler_context.pipeline_run.pipeline_code_origin
         ).repository_origin.container_image
         if not image:
             image = self._image
 
         run_launcher = step_handler_context.instance.run_launcher
 
         if not image and isinstance(run_launcher, DockerRunLauncher):
@@ -133,21 +119,21 @@
         if not image:
             raise Exception("No docker image specified by the executor config or repository")
 
         return image
 
     def _get_docker_container_context(self, step_handler_context: StepHandlerContext):
         # This doesn't vary per step: would be good to have a hook where it can be set once
-        # for the whole StepHandler but we need access to the DagsterRun for that
+        # for the whole StepHandler but we need access to the PipelineRun for that
 
         from .docker_run_launcher import DockerRunLauncher
 
         run_launcher = step_handler_context.instance.run_launcher
         run_target = DockerContainerContext.create_for_run(
-            step_handler_context.dagster_run,
+            step_handler_context.pipeline_run,
             run_launcher if isinstance(run_launcher, DockerRunLauncher) else None,
         )
 
         merged_container_context = run_target.merge(self._container_context)
 
         validate_docker_config(
             network=None,
@@ -167,71 +153,46 @@
             client.login(
                 registry=docker_container_context.registry["url"],
                 username=docker_container_context.registry["username"],
                 password=docker_container_context.registry["password"],
             )
         return client
 
-    def _get_container_name(self, execute_step_args: ExecuteStepArgs):
-        run_id = execute_step_args.run_id
-        step_keys_to_execute = check.not_none(execute_step_args.step_keys_to_execute)
-        assert len(step_keys_to_execute) == 1, "Launching multiple steps is not currently supported"
-        step_key = step_keys_to_execute[0]
-
-        step_name = f"dagster-step-{hash_str(run_id + step_key)}"
-
-        if execute_step_args.known_state:
-            retry_state = execute_step_args.known_state.get_retry_state()
-            retry_number = retry_state.get_attempt_count(step_key)
-            if retry_number:
-                step_name = f"{step_name}-{retry_number}"
+    def _get_container_name(self, run_id, step_key):
+        return f"dagster-step-{hash_str(run_id + step_key)}"
 
-        return step_name
-
-    def _create_step_container(
-        self,
-        client,
-        container_context,
-        step_image,
-        step_handler_context: StepHandlerContext,
-    ):
-        execute_step_args = step_handler_context.execute_step_args
-        step_keys_to_execute = check.not_none(execute_step_args.step_keys_to_execute)
-        assert len(step_keys_to_execute) == 1, "Launching multiple steps is not currently supported"
-        step_key = step_keys_to_execute[0]
-
-        env_vars = dict([parse_env_var(env_var) for env_var in container_context.env_vars])
-        env_vars["DAGSTER_RUN_JOB_NAME"] = step_handler_context.dagster_run.job_name
-        env_vars["DAGSTER_RUN_STEP_KEY"] = step_key
+    def _create_step_container(self, client, container_context, step_image, execute_step_args):
         return client.containers.create(
             step_image,
-            name=self._get_container_name(execute_step_args),
+            name=self._get_container_name(
+                execute_step_args.pipeline_run_id, execute_step_args.step_keys_to_execute[0]
+            ),
             detach=True,
             network=container_context.networks[0] if len(container_context.networks) else None,
             command=execute_step_args.get_command_args(),
-            environment=env_vars,
+            environment=(dict([parse_env_var(env_var) for env_var in container_context.env_vars])),
             **container_context.container_kwargs,
         )
 
     def launch_step(self, step_handler_context: StepHandlerContext) -> Iterator[DagsterEvent]:
         container_context = self._get_docker_container_context(step_handler_context)
 
         client = self._get_client(container_context)
 
         step_image = self._get_image(step_handler_context)
         validate_docker_image(step_image)
 
         try:
             step_container = self._create_step_container(
-                client, container_context, step_image, step_handler_context
+                client, container_context, step_image, step_handler_context.execute_step_args
             )
         except docker.errors.ImageNotFound:
             client.images.pull(step_image)
             step_container = self._create_step_container(
-                client, container_context, step_image, step_handler_context
+                client, container_context, step_image, step_handler_context.execute_step_args
             )
 
         if len(container_context.networks) > 1:
             for network_name in container_context.networks[1:]:
                 network = client.networks.get(network_name)
                 network.connect(step_container)
 
@@ -240,38 +201,44 @@
         )
         assert len(step_keys_to_execute) == 1, "Launching multiple steps is not currently supported"
         step_key = step_keys_to_execute[0]
 
         yield DagsterEvent.step_worker_starting(
             step_handler_context.get_step_context(step_key),
             message="Launching step in Docker container.",
-            metadata={
-                "Docker container id": step_container.id,
-            },
+            metadata_entries=[
+                MetadataEntry("Docker container id", value=step_container.id),
+            ],
         )
         step_container.start()
 
     def check_step_health(self, step_handler_context: StepHandlerContext) -> CheckStepHealthResult:
+        step_keys_to_execute = check.not_none(
+            step_handler_context.execute_step_args.step_keys_to_execute
+        )
+        step_key = step_keys_to_execute[0]
         container_context = self._get_docker_container_context(step_handler_context)
 
         client = self._get_client(container_context)
 
-        container_name = self._get_container_name(step_handler_context.execute_step_args)
+        container_name = self._get_container_name(
+            step_handler_context.execute_step_args.pipeline_run_id,
+            step_key,
+        )
 
         container = client.containers.get(container_name)
 
         if container.status == "running":
             return CheckStepHealthResult.healthy()
 
         try:
             container_info = container.wait(timeout=0.1)
         except Exception as e:
             raise Exception(
-                f"Container status is {container.status}. Raised exception attempting to get its"
-                " return code."
+                f"Container status is {container.status}. Raised exception attempting to get its return code."
             ) from e
 
         ret_code = container_info.get("StatusCode")
         if ret_code == 0:
             return CheckStepHealthResult.healthy()
 
         return CheckStepHealthResult.unhealthy(
@@ -285,15 +252,17 @@
             step_handler_context.execute_step_args.step_keys_to_execute
         )
         assert (
             len(step_keys_to_execute) == 1
         ), "Terminating multiple steps is not currently supported"
         step_key = step_keys_to_execute[0]
 
-        container_name = self._get_container_name(step_handler_context.execute_step_args)
+        container_name = self._get_container_name(
+            step_handler_context.execute_step_args.pipeline_run_id, step_key
+        )
 
         yield DagsterEvent.engine_event(
             step_handler_context.get_step_context(step_key),
             message=f"Stopping Docker container {container_name} for step.",
             event_specific_data=EngineEventData(),
         )
```

### Comparing `dagster-docker-0.19.6/dagster_docker/docker_run_launcher.py` & `dagster-docker-1.0.5/dagster_docker/docker_run_launcher.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-from typing import Any, Mapping, Optional
+import docker
+from dagster_docker.utils import DOCKER_CONFIG_SCHEMA, validate_docker_config, validate_docker_image
 
 import dagster._check as check
-import docker
 from dagster._core.launcher.base import (
     CheckRunHealthResult,
     LaunchRunContext,
     ResumeRunContext,
     RunLauncher,
     WorkerStatus,
 )
-from dagster._core.storage.dagster_run import DagsterRun
+from dagster._core.storage.pipeline_run import PipelineRun
 from dagster._core.storage.tags import DOCKER_IMAGE_TAG
 from dagster._core.utils import parse_env_var
 from dagster._grpc.types import ExecuteRunArgs, ResumeRunArgs
 from dagster._serdes import ConfigurableClass
-from dagster._serdes.config_class import ConfigurableClassData
-from typing_extensions import Self
-
-from dagster_docker.utils import DOCKER_CONFIG_SCHEMA, validate_docker_config, validate_docker_image
 
 from .container_context import DockerContainerContext
 
 DOCKER_CONTAINER_ID_TAG = "docker/container_id"
 
 
 class DockerRunLauncher(RunLauncher, ConfigurableClass):
     """Launches runs in a Docker container."""
 
     def __init__(
         self,
-        inst_data: Optional[ConfigurableClassData] = None,
+        inst_data=None,
         image=None,
         registry=None,
         env_vars=None,
         network=None,
         networks=None,
         container_kwargs=None,
     ):
@@ -61,49 +57,46 @@
     def inst_data(self):
         return self._inst_data
 
     @classmethod
     def config_type(cls):
         return DOCKER_CONFIG_SCHEMA
 
-    @classmethod
-    def from_config_value(
-        cls, inst_data: ConfigurableClassData, config_value: Mapping[str, Any]
-    ) -> Self:
+    @staticmethod
+    def from_config_value(inst_data, config_value):
         return DockerRunLauncher(inst_data=inst_data, **config_value)
 
-    def get_container_context(self, dagster_run: DagsterRun) -> DockerContainerContext:
-        return DockerContainerContext.create_for_run(dagster_run, self)
+    def get_container_context(self, pipeline_run: PipelineRun) -> DockerContainerContext:
+        return DockerContainerContext.create_for_run(pipeline_run, self)
 
     def _get_client(self, container_context: DockerContainerContext):
         client = docker.client.from_env()
         if container_context.registry:
             client.login(
                 registry=container_context.registry["url"],
                 username=container_context.registry["username"],
                 password=container_context.registry["password"],
             )
         return client
 
-    def _get_docker_image(self, job_code_origin):
-        docker_image = job_code_origin.repository_origin.container_image
+    def _get_docker_image(self, pipeline_code_origin):
+        docker_image = pipeline_code_origin.repository_origin.container_image
 
         if not docker_image:
             docker_image = self.image
 
         if not docker_image:
             raise Exception("No docker image specified by the instance config or repository")
 
         validate_docker_image(docker_image)
         return docker_image
 
     def _launch_container_with_command(self, run, docker_image, command):
         container_context = self.get_container_context(run)
         docker_env = dict([parse_env_var(env_var) for env_var in container_context.env_vars])
-        docker_env["DAGSTER_RUN_JOB_NAME"] = run.job_name
 
         client = self._get_client(container_context)
 
         try:
             container = client.containers.create(
                 image=docker_image,
                 command=command,
@@ -126,56 +119,54 @@
 
         if len(container_context.networks) > 1:
             for network_name in container_context.networks[1:]:
                 network = client.networks.get(network_name)
                 network.connect(container)
 
         self._instance.report_engine_event(
-            message=(
-                "Launching run in a new container {container_id} with image {docker_image}".format(
-                    container_id=container.id,
-                    docker_image=docker_image,
-                )
+            message="Launching run in a new container {container_id} with image {docker_image}".format(
+                container_id=container.id,
+                docker_image=docker_image,
             ),
-            dagster_run=run,
+            pipeline_run=run,
             cls=self.__class__,
         )
 
         self._instance.add_run_tags(
             run.run_id,
             {DOCKER_CONTAINER_ID_TAG: container.id, DOCKER_IMAGE_TAG: docker_image},
         )
 
         container.start()
 
     def launch_run(self, context: LaunchRunContext) -> None:
-        run = context.dagster_run
-        job_code_origin = check.not_none(context.job_code_origin)
-        docker_image = self._get_docker_image(job_code_origin)
+        run = context.pipeline_run
+        pipeline_code_origin = check.not_none(context.pipeline_code_origin)
+        docker_image = self._get_docker_image(pipeline_code_origin)
 
         command = ExecuteRunArgs(
-            job_origin=job_code_origin,
-            run_id=run.run_id,
+            pipeline_origin=pipeline_code_origin,
+            pipeline_run_id=run.run_id,
             instance_ref=self._instance.get_ref(),
         ).get_command_args()
 
         self._launch_container_with_command(run, docker_image, command)
 
     @property
     def supports_resume_run(self):
         return True
 
     def resume_run(self, context: ResumeRunContext) -> None:
-        run = context.dagster_run
-        job_code_origin = check.not_none(context.job_code_origin)
-        docker_image = self._get_docker_image(job_code_origin)
+        run = context.pipeline_run
+        pipeline_code_origin = check.not_none(context.pipeline_code_origin)
+        docker_image = self._get_docker_image(pipeline_code_origin)
 
         command = ResumeRunArgs(
-            job_origin=job_code_origin,
-            run_id=run.run_id,
+            pipeline_origin=pipeline_code_origin,
+            pipeline_run_id=run.run_id,
             instance_ref=self._instance.get_ref(),
         ).get_command_args()
 
         self._launch_container_with_command(run, docker_image, command)
 
     def _get_container(self, run):
         if not run or run.is_finished:
@@ -191,40 +182,36 @@
         try:
             return self._get_client(container_context).containers.get(container_id)
         except Exception:
             return None
 
     def terminate(self, run_id):
         run = self._instance.get_run_by_id(run_id)
-
-        if not run:
-            return False
-
-        self._instance.report_run_canceling(run)
-
         container = self._get_container(run)
 
         if not container:
             self._instance.report_engine_event(
                 message="Unable to get docker container to send termination request to.",
-                dagster_run=run,
+                pipeline_run=run,
                 cls=self.__class__,
             )
             return False
 
+        self._instance.report_run_canceling(run)
+
         container.stop()
 
         return True
 
     @property
     def supports_check_run_worker_health(self):
         return True
 
-    def check_run_worker_health(self, run: DagsterRun):
+    def check_run_worker_health(self, run: PipelineRun):
         container = self._get_container(run)
-        if container is None:
+        if container == None:
             return CheckRunHealthResult(WorkerStatus.NOT_FOUND)
         if container.status == "running":
             return CheckRunHealthResult(WorkerStatus.RUNNING)
         return CheckRunHealthResult(
             WorkerStatus.FAILED, msg=f"Container status is {container.status}"
         )
```

### Comparing `dagster-docker-0.19.6/dagster_docker/utils.py` & `dagster-docker-1.0.5/dagster_docker/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,26 @@
-from dagster import (
-    Field,
-    StringSource,
-    _check as check,
-)
-from dagster._utils.merger import merge_dicts
 from docker_image import reference
 
+from dagster import Field, StringSource
+from dagster import _check as check
+from dagster._utils import merge_dicts
+
 from .container_context import DOCKER_CONTAINER_CONTEXT_SCHEMA
 
 DOCKER_CONFIG_SCHEMA = merge_dicts(
     {
         "image": Field(
             StringSource,
             is_required=False,
             description="The docker image to be used if the repository does not specify one.",
         ),
         "network": Field(
             StringSource,
             is_required=False,
-            description=(
-                "Name of the network to which to connect the launched container at creation time"
-            ),
+            description="Name of the network to which to connect the launched container at creation time",
         ),
     },
     DOCKER_CONTAINER_CONTEXT_SCHEMA,
 )
 
 
 def validate_docker_config(network, networks, container_kwargs):
@@ -35,22 +31,20 @@
         if "image" in container_kwargs:
             raise Exception(
                 "'image' cannot be used in 'container_kwargs'. Use the 'image' config key instead."
             )
 
         if "environment" in container_kwargs:
             raise Exception(
-                "'environment' cannot be used in 'container_kwargs'. Use the 'env_vars' config key"
-                " instead."
+                "'environment' cannot be used in 'container_kwargs'. Use the 'env_vars' config key instead."
             )
 
         if "network" in container_kwargs:
             raise Exception(
-                "'network' cannot be used in 'container_kwargs'. Use the 'networks' config key"
-                " instead."
+                "'network' cannot be used in 'container_kwargs'. Use the 'networks' config key instead."
             )
 
 
 def validate_docker_image(docker_image):
     try:
         # validate that the docker image name is valid
         reference.Reference.parse(docker_image)
```

### Comparing `dagster-docker-0.19.6/setup.py` & `dagster-docker-1.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,37 @@
-from pathlib import Path
 from typing import Dict
 
 from setuptools import find_packages, setup
 
 
 def get_version() -> str:
     version: Dict[str, str] = {}
-    with open(Path(__file__).parent / "dagster_docker/version.py", encoding="utf8") as fp:
-        exec(fp.read(), version)
+    with open("dagster_docker/version.py", encoding="utf8") as fp:
+        exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
-ver = get_version()
-# dont pin dev installs to avoid pip dep resolver issues
-pin = "" if ver == "1!0+dev" else f"=={ver}"
-setup(
-    name="dagster-docker",
-    version=ver,
-    author="Elementl",
-    author_email="hello@elementl.com",
-    license="Apache-2.0",
-    description="A Dagster integration for docker",
-    url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-docker",
-    classifiers=[
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: OS Independent",
-    ],
-    packages=find_packages(exclude=["dagster_docker_tests*"]),
-    # urllib3<2 pin needed until docker-py is updated
-    # see: https://github.com/docker/docker-py/issues/3113
-    install_requires=["dagster==1.3.6", "docker", "docker-image-py", "urllib3<2"],
-    zip_safe=False,
-)
+if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
+    setup(
+        name="dagster-docker",
+        version=ver,
+        author="Elementl",
+        author_email="hello@elementl.com",
+        license="Apache-2.0",
+        description="A Dagster integration for docker",
+        url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-docker",
+        classifiers=[
+            "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "License :: OSI Approved :: Apache Software License",
+            "Operating System :: OS Independent",
+        ],
+        packages=find_packages(exclude=["dagster_docker_tests*"]),
+        install_requires=["dagster==1.0.5", "docker", "docker-image-py"],
+        zip_safe=False,
+    )
```

