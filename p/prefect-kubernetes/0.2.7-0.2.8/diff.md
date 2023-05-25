# Comparing `tmp/prefect-kubernetes-0.2.7.tar.gz` & `tmp/prefect-kubernetes-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-kubernetes/prefect-kubernetes/dist/.tmp-uuh3r2jr/prefect-kubernetes-0.2.7.tar", last modified: Thu May  4 16:17:35 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-kubernetes/prefect-kubernetes/dist/.tmp-siz5suu5/prefect-kubernetes-0.2.8.tar", last modified: Thu May 25 19:29:13 2023, max compression
```

## Comparing `prefect-kubernetes-0.2.7.tar` & `prefect-kubernetes-0.2.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/custom_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/pods.py
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    32770 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/prefect_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/prefect_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/prefect_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/prefect_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/prefect_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/prefect_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/prefect_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_custom_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_events_replicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_pods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    77624 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/custom_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33250 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/prefect_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/prefect_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/prefect_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/prefect_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/prefect_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/prefect_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/prefect_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_custom_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_events_replicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82835 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/versioneer.py
```

### Comparing `prefect-kubernetes-0.2.7/LICENSE` & `prefect-kubernetes-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/PKG-INFO` & `prefect-kubernetes-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-kubernetes
-Version: 0.2.7
+Version: 0.2.8
 Summary: Prefect integrations for interacting with Kubernetes.
 Home-page: https://github.com/PrefectHQ/prefect-kubernetes
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-kubernetes-0.2.7/README.md` & `prefect-kubernetes-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/prefect_kubernetes/credentials.py` & `prefect-kubernetes-0.2.8/prefect_kubernetes/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/prefect_kubernetes/custom_objects.py` & `prefect-kubernetes-0.2.8/prefect_kubernetes/custom_objects.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/prefect_kubernetes/deployments.py` & `prefect-kubernetes-0.2.8/prefect_kubernetes/deployments.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/prefect_kubernetes/events.py` & `prefect-kubernetes-0.2.8/prefect_kubernetes/events.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/prefect_kubernetes/exceptions.py` & `prefect-kubernetes-0.2.8/prefect_kubernetes/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/prefect_kubernetes/flows.py` & `prefect-kubernetes-0.2.8/prefect_kubernetes/flows.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/prefect_kubernetes/jobs.py` & `prefect-kubernetes-0.2.8/prefect_kubernetes/jobs.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/prefect_kubernetes/pods.py` & `prefect-kubernetes-0.2.8/prefect_kubernetes/pods.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/prefect_kubernetes/services.py` & `prefect-kubernetes-0.2.8/prefect_kubernetes/services.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/prefect_kubernetes/utilities.py` & `prefect-kubernetes-0.2.8/prefect_kubernetes/utilities.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/prefect_kubernetes/worker.py` & `prefect-kubernetes-0.2.8/prefect_kubernetes/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,26 +84,29 @@
     allocated to Kubernetes jobs created by workers in this work pool, but the limit
     is hard-coded and cannot be changed by deployments.
 
 For more information about work pools and workers,
 checkout out the [Prefect docs](https://docs.prefect.io/concepts/work-pools/).
 """
 import enum
+import logging
 import math
 import os
 import time
 from contextlib import contextmanager
-from typing import TYPE_CHECKING, Any, Dict, Generator, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Dict, Generator, Optional, Tuple
 
 import anyio.abc
 from prefect.blocks.kubernetes import KubernetesClusterConfig
 from prefect.docker import get_prefect_image_name
-from prefect.events import RelatedResource
-from prefect.events.related import object_as_related_resource, tags_as_related_resources
-from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
+from prefect.exceptions import (
+    InfrastructureError,
+    InfrastructureNotAvailable,
+    InfrastructureNotFound,
+)
 from prefect.server.schemas.core import Flow
 from prefect.server.schemas.responses import DeploymentResponse
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
 from prefect.utilities.importtools import lazy_import
 from prefect.utilities.pydantic import JsonPatch
 from prefect.utilities.templating import find_placeholders
 from prefect.workers.base import (
@@ -391,29 +394,14 @@
             if self.name:
                 generate_name = _slugify_name(self.name)
             # _slugify_name will return None if the slugified name in an exception
             if not generate_name:
                 generate_name = "prefect-job"
             self.job_manifest["metadata"]["generateName"] = f"{generate_name}-"
 
-    def _related_resources(self) -> List[RelatedResource]:
-        tags = set()
-        related = []
-
-        for kind, obj in self._related_objects.items():
-            # TODO: Remove this method once we've updated the Prefect core side
-            # to ignore objects that are None.
-            if not obj:
-                continue
-            if hasattr(obj, "tags"):
-                tags.update(obj.tags)
-            related.append(object_as_related_resource(kind=kind, role=kind, object=obj))
-
-        return related + tags_as_related_resources(tags)
-
 
 class KubernetesWorkerVariables(BaseVariables):
     """
     Default variables for the Kubernetes worker.
 
     The schema for this class is used to populate the `variables` section of the default
     base job template.
@@ -472,14 +460,22 @@
 
 class KubernetesWorker(BaseWorker):
     """Prefect worker that executes flow runs within Kubernetes Jobs."""
 
     type = "kubernetes"
     job_configuration = KubernetesWorkerJobConfiguration
     job_configuration_variables = KubernetesWorkerVariables
+    _description = (
+        "Execute flow runs within jobs scheduled on a Kubernetes cluster. Requires a "
+        "Kubernetes cluster."
+    )
+    _display_name = "Kubernetes"
+    _documentation_url = "https://prefecthq.github.io/prefect-kubernetes/worker/"
+    _is_beta = True
+    _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/1zrSeY8DZ1MJZs2BAyyyGk/20445025358491b8b72600b8f996125b/Kubernetes_logo_without_workmark.svg.png?h=250"  # noqa
 
     async def run(
         self,
         flow_run: "FlowRun",
         configuration: KubernetesWorkerJobConfiguration,
         task_status: Optional[anyio.abc.TaskStatus] = None,
     ) -> KubernetesWorkerResult:
@@ -493,15 +489,18 @@
             task_status: The task status object for the current flow run. If provided,
                 the task will be marked as started.
 
         Returns:
             KubernetesWorkerResult: A result object containing information about the
                 final state of the flow run
         """
+        logger = self.get_flow_run_logger(flow_run)
+
         with self._get_configured_kubernetes_client(configuration) as client:
+            logger.info("Creating Kubernetes job...")
             job = await run_sync_in_worker_thread(
                 self._create_job, configuration, client
             )
             pid = await run_sync_in_worker_thread(
                 self._get_infrastructure_pid, job, client
             )
             # Indicate that the job has started
@@ -519,15 +518,15 @@
                     configuration=configuration
                 ),
                 timeout_seconds=configuration.pod_watch_timeout_seconds,
             )
 
             with events_replicator:
                 status_code = await run_sync_in_worker_thread(
-                    self._watch_job, job.metadata.name, configuration, client
+                    self._watch_job, logger, job.metadata.name, configuration, client
                 )
             return KubernetesWorkerResult(identifier=pid, status_code=status_code)
 
     async def kill_infrastructure(
         self,
         infrastructure_pid: str,
         configuration: KubernetesWorkerJobConfiguration,
@@ -614,18 +613,31 @@
 
     def _create_job(
         self, configuration: KubernetesWorkerJobConfiguration, client: "ApiClient"
     ) -> "V1Job":
         """
         Creates a Kubernetes job from a job manifest.
         """
-        with self._get_batch_client(client) as batch_client:
-            job = batch_client.create_namespaced_job(
-                configuration.namespace, configuration.job_manifest
-            )
+        try:
+            with self._get_batch_client(client) as batch_client:
+                job = batch_client.create_namespaced_job(
+                    configuration.namespace, configuration.job_manifest
+                )
+        except kubernetes.client.exceptions.ApiException as exc:
+            # Parse the reason and message from the response if feasible
+            message = ""
+            if exc.reason:
+                message += ": " + exc.reason
+            if exc.body and "message" in exc.body:
+                message += ": " + exc.body["message"]
+
+            raise InfrastructureError(
+                f"Unable to create Kubernetes job{message}"
+            ) from exc
+
         return job
 
     @contextmanager
     def _get_batch_client(
         self, client: "ApiClient"
     ) -> Generator["BatchV1Api", None, None]:
         """
@@ -693,30 +705,31 @@
             namespace = core_client.read_namespace("kube-system")
         cluster_uid = namespace.metadata.uid
 
         return cluster_uid
 
     def _watch_job(
         self,
+        logger: logging.Logger,
         job_name: str,
         configuration: KubernetesWorkerJobConfiguration,
         client: "ApiClient",
     ) -> int:
         """
         Watch a job.
 
         Return the final status code of the first container.
         """
-        self._logger.debug(f"Job {job_name!r}: Monitoring job...")
+        logger.debug(f"Job {job_name!r}: Monitoring job...")
 
-        job = self._get_job(job_name, configuration, client)
+        job = self._get_job(logger, job_name, configuration, client)
         if not job:
             return -1
 
-        pod = self._get_job_pod(job_name, configuration, client)
+        pod = self._get_job_pod(logger, job_name, configuration, client)
         if not pod:
             return -1
 
         # Calculate the deadline before streaming output
         deadline = (
             (time.monotonic() + configuration.job_watch_timeout_seconds)
             if configuration.job_watch_timeout_seconds is not None
@@ -741,15 +754,15 @@
                         remaining_time = (
                             deadline - time.monotonic() if deadline else None
                         )
                         if deadline and remaining_time <= 0:
                             break
 
                 except Exception:
-                    self._logger.warning(
+                    logger.warning(
                         (
                             "Error occurred while streaming logs - "
                             "Job will continue to run but logs will "
                             "no longer be streamed to stdout."
                         ),
                         exc_info=True,
                     )
@@ -762,15 +775,15 @@
             completed = job.status.completion_time is not None
 
             while not completed:
                 remaining_time = (
                     math.ceil(deadline - time.monotonic()) if deadline else None
                 )
                 if deadline and remaining_time <= 0:
-                    self._logger.error(
+                    logger.error(
                         f"Job {job_name!r}: Job did not complete within "
                         f"timeout of {configuration.job_watch_timeout_seconds}s."
                     )
                     return -1
 
                 watch = kubernetes.watch.Watch()
                 # The kubernetes library will disable retries if the timeout kwarg is
@@ -785,65 +798,67 @@
                     field_selector=f"metadata.name={job_name}",
                     namespace=configuration.namespace,
                     **timeout_seconds,
                 ):
                     if event["object"].status.completion_time:
                         if not event["object"].status.succeeded:
                             # Job failed, exit while loop and return pod exit code
-                            self._logger.error(f"Job {job_name!r}: Job failed.")
+                            logger.error(f"Job {job_name!r}: Job failed.")
                         completed = True
                         watch.stop()
                         break
 
         with self._get_core_client(client) as core_client:
             pod_status = core_client.read_namespaced_pod_status(
                 namespace=configuration.namespace, name=pod.metadata.name
             )
             first_container_status = pod_status.status.container_statuses[0]
 
         return first_container_status.state.terminated.exit_code
 
     def _get_job(
         self,
+        logger: logging.Logger,
         job_id: str,
         configuration: KubernetesWorkerJobConfiguration,
         client: "ApiClient",
     ) -> Optional["V1Job"]:
         """Get a Kubernetes job by id."""
         with self._get_batch_client(client) as batch_client:
             try:
                 job = batch_client.read_namespaced_job(
                     name=job_id, namespace=configuration.namespace
                 )
             except kubernetes.client.exceptions.ApiException:
-                self._logger.error(f"Job {job_id!r} was removed.", exc_info=True)
+                logger.error(f"Job {job_id!r} was removed.", exc_info=True)
                 return None
             return job
 
     def _get_job_pod(
         self,
+        logger: logging.Logger,
         job_name: str,
         configuration: KubernetesWorkerJobConfiguration,
         client: "ApiClient",
     ) -> Optional["V1Pod"]:
         """Get the first running pod for a job."""
         watch = kubernetes.watch.Watch()
-        self._logger.debug(f"Job {job_name!r}: Starting watch for pod start...")
+        logger.debug(f"Job {job_name!r}: Starting watch for pod start...")
         last_phase = None
         with self._get_core_client(client) as core_client:
             for event in watch.stream(
                 func=core_client.list_namespaced_pod,
                 namespace=configuration.namespace,
                 label_selector=f"job-name={job_name}",
                 timeout_seconds=configuration.pod_watch_timeout_seconds,
             ):
                 phase = event["object"].status.phase
                 if phase != last_phase:
-                    self._logger.info(f"Job {job_name!r}: Pod has status {phase!r}.")
+                    logger.info(f"Job {job_name!r}: Pod has status {phase!r}.")
 
                 if phase != "Pending":
                     watch.stop()
                     return event["object"]
 
                 last_phase = phase
 
-        self._logger.error(f"Job {job_name!r}: Pod never started.")
+        logger.error(f"Job {job_name!r}: Pod never started.")
```

### Comparing `prefect-kubernetes-0.2.7/prefect_kubernetes.egg-info/PKG-INFO` & `prefect-kubernetes-0.2.8/prefect_kubernetes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-kubernetes
-Version: 0.2.7
+Version: 0.2.8
 Summary: Prefect integrations for interacting with Kubernetes.
 Home-page: https://github.com/PrefectHQ/prefect-kubernetes
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-kubernetes-0.2.7/prefect_kubernetes.egg-info/SOURCES.txt` & `prefect-kubernetes-0.2.8/prefect_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/setup.cfg` & `prefect-kubernetes-0.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/setup.py` & `prefect-kubernetes-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/tests/test_block_standards.py` & `prefect-kubernetes-0.2.8/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/tests/test_credentials.py` & `prefect-kubernetes-0.2.8/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/tests/test_custom_objects.py` & `prefect-kubernetes-0.2.8/tests/test_custom_objects.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/tests/test_deployments.py` & `prefect-kubernetes-0.2.8/tests/test_deployments.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/tests/test_events_replicator.py` & `prefect-kubernetes-0.2.8/tests/test_events_replicator.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/tests/test_flows.py` & `prefect-kubernetes-0.2.8/tests/test_flows.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/tests/test_jobs.py` & `prefect-kubernetes-0.2.8/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/tests/test_pods.py` & `prefect-kubernetes-0.2.8/tests/test_pods.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/tests/test_services.py` & `prefect-kubernetes-0.2.8/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/tests/test_utilities.py` & `prefect-kubernetes-0.2.8/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.7/tests/test_worker.py` & `prefect-kubernetes-0.2.8/tests/test_worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from contextlib import contextmanager
 from time import monotonic, sleep
 from unittest import mock
 from unittest.mock import MagicMock, Mock
 
 import anyio
 import anyio.abc
@@ -9,15 +10,19 @@
 import pendulum
 import prefect
 import pytest
 from kubernetes.client.exceptions import ApiException
 from kubernetes.config import ConfigException
 from prefect.client.schemas import FlowRun
 from prefect.docker import get_prefect_image_name
-from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
+from prefect.exceptions import (
+    InfrastructureError,
+    InfrastructureNotAvailable,
+    InfrastructureNotFound,
+)
 from prefect.server.schemas.core import Flow
 from prefect.server.schemas.responses import DeploymentResponse
 from prefect.settings import (
     PREFECT_EXPERIMENTAL_ENABLE_WORKERS,
     PREFECT_EXPERIMENTAL_WARN_WORKERS,
     get_current_settings,
     temporary_settings,
@@ -1067,14 +1072,154 @@
             await k8s_worker.run(flow_run, configuration)
             mock_batch_client.create_namespaced_job.assert_called_once()
             image = mock_batch_client.create_namespaced_job.call_args[0][1]["spec"][
                 "template"
             ]["spec"]["containers"][0]["image"]
             assert image == "foo"
 
+    async def test_create_job_failure(
+        self,
+        flow_run,
+        mock_core_client,
+        mock_watch,
+        mock_batch_client,
+    ):
+        response = MagicMock()
+        response.data = {
+            "kind": "Status",
+            "apiVersion": "v1",
+            "metadata": {},
+            "status": "Failure",
+            "message": 'jobs.batch is forbidden: User "system:serviceaccount:helm-test:prefect-worker-dev" cannot create resource "jobs" in API group "batch" in the namespace "prefect"',
+            "reason": "Forbidden",
+            "details": {"group": "batch", "kind": "jobs"},
+            "code": 403,
+        }
+        response.status = 403
+        response.reason = "Forbidden"
+
+        mock_batch_client.create_namespaced_job.side_effect = ApiException(
+            http_resp=response
+        )
+
+        configuration = await KubernetesWorkerJobConfiguration.from_template_and_values(
+            KubernetesWorker.get_default_base_job_template(), {"image": "foo"}
+        )
+        async with KubernetesWorker(work_pool_name="test") as k8s_worker:
+            with pytest.raises(
+                InfrastructureError,
+                match=re.escape(
+                    "Unable to create Kubernetes job: Forbidden: jobs.batch is forbidden: User "
+                    '"system:serviceaccount:helm-test:prefect-worker-dev" cannot '
+                    'create resource "jobs" in API group "batch" in the namespace '
+                    '"prefect"'
+                ),
+            ):
+                await k8s_worker.run(flow_run, configuration)
+
+    async def test_create_job_failure_no_reason(
+        self,
+        flow_run,
+        mock_core_client,
+        mock_watch,
+        mock_batch_client,
+    ):
+        response = MagicMock()
+        response.data = {
+            "kind": "Status",
+            "apiVersion": "v1",
+            "metadata": {},
+            "status": "Failure",
+            "message": 'jobs.batch is forbidden: User "system:serviceaccount:helm-test:prefect-worker-dev" cannot create resource "jobs" in API group "batch" in the namespace "prefect"',
+            "reason": "Forbidden",
+            "details": {"group": "batch", "kind": "jobs"},
+            "code": 403,
+        }
+        response.status = 403
+        response.reason = None
+
+        mock_batch_client.create_namespaced_job.side_effect = ApiException(
+            http_resp=response
+        )
+
+        configuration = await KubernetesWorkerJobConfiguration.from_template_and_values(
+            KubernetesWorker.get_default_base_job_template(), {"image": "foo"}
+        )
+        async with KubernetesWorker(work_pool_name="test") as k8s_worker:
+            with pytest.raises(
+                InfrastructureError,
+                match=re.escape(
+                    "Unable to create Kubernetes job: jobs.batch is forbidden: User "
+                    '"system:serviceaccount:helm-test:prefect-worker-dev" cannot '
+                    'create resource "jobs" in API group "batch" in the namespace '
+                    '"prefect"'
+                ),
+            ):
+                await k8s_worker.run(flow_run, configuration)
+
+    async def test_create_job_failure_no_message(
+        self,
+        flow_run,
+        mock_core_client,
+        mock_watch,
+        mock_batch_client,
+    ):
+        response = MagicMock()
+        response.data = {
+            "kind": "Status",
+            "apiVersion": "v1",
+            "metadata": {},
+            "status": "Failure",
+            "reason": "Forbidden",
+            "details": {"group": "batch", "kind": "jobs"},
+            "code": 403,
+        }
+        response.status = 403
+        response.reason = "Test"
+
+        mock_batch_client.create_namespaced_job.side_effect = ApiException(
+            http_resp=response
+        )
+
+        configuration = await KubernetesWorkerJobConfiguration.from_template_and_values(
+            KubernetesWorker.get_default_base_job_template(), {"image": "foo"}
+        )
+        async with KubernetesWorker(work_pool_name="test") as k8s_worker:
+            with pytest.raises(
+                InfrastructureError,
+                match=re.escape("Unable to create Kubernetes job: Test"),
+            ):
+                await k8s_worker.run(flow_run, configuration)
+
+    async def test_create_job_failure_no_response_body(
+        self,
+        flow_run,
+        mock_core_client,
+        mock_watch,
+        mock_batch_client,
+    ):
+        response = MagicMock()
+        response.data = None
+        response.status = 403
+        response.reason = "Test"
+
+        mock_batch_client.create_namespaced_job.side_effect = ApiException(
+            http_resp=response
+        )
+
+        configuration = await KubernetesWorkerJobConfiguration.from_template_and_values(
+            KubernetesWorker.get_default_base_job_template(), {"image": "foo"}
+        )
+        async with KubernetesWorker(work_pool_name="test") as k8s_worker:
+            with pytest.raises(
+                InfrastructureError,
+                match=re.escape("Unable to create Kubernetes job: Test"),
+            ):
+                await k8s_worker.run(flow_run, configuration)
+
     async def test_allows_image_setting_from_manifest(
         self,
         default_configuration: KubernetesWorkerJobConfiguration,
         flow_run,
         mock_core_client,
         mock_watch,
         mock_batch_client,
```

### Comparing `prefect-kubernetes-0.2.7/versioneer.py` & `prefect-kubernetes-0.2.8/versioneer.py`

 * *Files identical despite different names*

