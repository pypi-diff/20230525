# Comparing `tmp/dagster-k8s-0.9.9rc1.tar.gz` & `tmp/dagster-k8s-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-k8s-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:18 2020, max compression
+gzip compressed data, was "dagster-k8s-1.0.5.tar", last modified: Fri Aug 26 13:45:28 2022, max compression
```

## Comparing `dagster-k8s-0.9.9rc1.tar` & `dagster-k8s-1.0.5.tar`

### file list

```diff
@@ -1,33 +1,29 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:18.000000 dagster-k8s-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      564 2020-09-17 21:08:18.000000 dagster-k8s-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      119 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:18.000000 dagster-k8s-0.9.9rc1/dagster_k8s/
--rw-r--r--   0 bobchen    (501) staff       (20)      337 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    16154 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s/client.py
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s/config.py
--rw-r--r--   0 bobchen    (501) staff       (20)    22168 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s/job.py
--rw-r--r--   0 bobchen    (501) staff       (20)    14915 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s/launcher.py
--rw-r--r--   0 bobchen    (501) staff       (20)     9341 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s/scheduler.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1558 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s/test.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3253 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s/utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:18.000000 dagster-k8s-0.9.9rc1/dagster_k8s.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      564 2020-09-17 21:08:17.000000 dagster-k8s-0.9.9rc1/dagster_k8s.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      751 2020-09-17 21:08:17.000000 dagster-k8s-0.9.9rc1/dagster_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:17.000000 dagster-k8s-0.9.9rc1/dagster_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:17.000000 dagster-k8s-0.9.9rc1/dagster_k8s.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       69 2020-09-17 21:08:17.000000 dagster-k8s-0.9.9rc1/dagster_k8s.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       30 2020-09-17 21:08:17.000000 dagster-k8s-0.9.9rc1/dagster_k8s.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:18.000000 dagster-k8s-0.9.9rc1/dagster_k8s_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s_tests/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:18.000000 dagster-k8s-0.9.9rc1/dagster_k8s_tests/unit_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s_tests/unit_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    17876 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s_tests/unit_tests/test_client.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1193 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s_tests/unit_tests/test_job.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2780 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s_tests/unit_tests/test_resource_tags.py
--rw-r--r--   0 bobchen    (501) staff       (20)     8042 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s_tests/unit_tests/test_utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       89 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s_tests/unit_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:18.000000 dagster-k8s-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1202 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:28.932462 dagster-k8s-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-k8s-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       63 2022-08-26 13:33:01.000000 dagster-k8s-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      623 2022-08-26 13:45:28.932462 dagster-k8s-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      119 2022-08-26 13:33:01.000000 dagster-k8s-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:28.932462 dagster-k8s-1.0.5/dagster_k8s/
+-rw-r--r--   0 root         (0) root         (0)      364 2022-08-26 13:33:01.000000 dagster-k8s-1.0.5/dagster_k8s/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21182 2022-08-26 13:33:01.000000 dagster-k8s-1.0.5/dagster_k8s/client.py
+-rw-r--r--   0 root         (0) root         (0)     9140 2022-08-26 13:33:01.000000 dagster-k8s-1.0.5/dagster_k8s/container_context.py
+-rw-r--r--   0 root         (0) root         (0)    10690 2022-08-26 13:33:01.000000 dagster-k8s-1.0.5/dagster_k8s/executor.py
+-rw-r--r--   0 root         (0) root         (0)    31855 2022-08-26 13:33:01.000000 dagster-k8s-1.0.5/dagster_k8s/job.py
+-rw-r--r--   0 root         (0) root         (0)    12926 2022-08-26 13:33:01.000000 dagster-k8s-1.0.5/dagster_k8s/launcher.py
+-rw-r--r--   0 root         (0) root         (0)     4853 2022-08-26 13:33:01.000000 dagster-k8s-1.0.5/dagster_k8s/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:28.932462 dagster-k8s-1.0.5/dagster_k8s/ops/
+-rw-r--r--   0 root         (0) root         (0)       35 2022-08-26 13:33:01.000000 dagster-k8s-1.0.5/dagster_k8s/ops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7697 2022-08-26 13:33:01.000000 dagster-k8s-1.0.5/dagster_k8s/ops/k8s_job_op.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-k8s-1.0.5/dagster_k8s/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1004 2022-08-26 13:33:01.000000 dagster-k8s-1.0.5/dagster_k8s/test.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2022-08-26 13:33:01.000000 dagster-k8s-1.0.5/dagster_k8s/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-k8s-1.0.5/dagster_k8s/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:28.932462 dagster-k8s-1.0.5/dagster_k8s.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      623 2022-08-26 13:45:28.000000 dagster-k8s-1.0.5/dagster_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      567 2022-08-26 13:45:28.000000 dagster-k8s-1.0.5/dagster_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:28.000000 dagster-k8s-1.0.5/dagster_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:28.000000 dagster-k8s-1.0.5/dagster_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       26 2022-08-26 13:45:28.000000 dagster-k8s-1.0.5/dagster_k8s.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-08-26 13:45:28.000000 dagster-k8s-1.0.5/dagster_k8s.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2022-08-26 13:45:28.932462 dagster-k8s-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1278 2022-08-26 13:33:01.000000 dagster-k8s-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-k8s-0.9.9rc1/LICENSE` & `dagster-k8s-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-k8s-0.9.9rc1/PKG-INFO` & `dagster-k8s-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-k8s
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: A Dagster integration for k8s
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-k8s
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
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-k8s-0.9.9rc1/dagster_k8s/client.py` & `dagster-k8s-1.0.5/dagster_k8s/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,133 @@
 import logging
+import sys
 import time
 from enum import Enum
 
 import kubernetes
-import six
 
-from dagster import DagsterInstance, check
-from dagster.core.storage.pipeline_run import PipelineRunStatus
+from dagster import DagsterInstance
+from dagster import _check as check
+from dagster._core.storage.pipeline_run import PipelineRunStatus
 
 DEFAULT_WAIT_TIMEOUT = 86400.0  # 1 day
-DEFAULT_WAIT_BETWEEN_ATTEMPTS = 1.0  # 1 second
+DEFAULT_WAIT_BETWEEN_ATTEMPTS = 10.0  # 10 seconds
 DEFAULT_JOB_POD_COUNT = 1  # expect job:pod to be 1:1 by default
 
 
 class WaitForPodState(Enum):
     Ready = "READY"
     Terminated = "TERMINATED"
 
 
 class DagsterK8sError(Exception):
     pass
 
 
+class DagsterK8sTimeoutError(DagsterK8sError):
+    pass
+
+
+class DagsterK8sAPIRetryLimitExceeded(Exception):
+    def __init__(self, *args, **kwargs):
+        k8s_api_exception = check.inst_param(
+            kwargs.pop("k8s_api_exception"), "k8s_api_exception", Exception
+        )
+        original_exc_info = check.tuple_param(kwargs.pop("original_exc_info"), "original_exc_info")
+        max_retries = check.int_param(kwargs.pop("max_retries"), "max_retries")
+
+        check.invariant(original_exc_info[0] is not None)
+        super(DagsterK8sAPIRetryLimitExceeded, self).__init__(
+            f"Retry limit of {max_retries} exceeded: " + args[0],
+            *args[1:],
+            **kwargs,
+        )
+
+        self.k8s_api_exception = check.opt_inst_param(
+            k8s_api_exception, "k8s_api_exception", Exception
+        )
+        self.original_exc_info = original_exc_info
+
+
+class DagsterK8sUnrecoverableAPIError(Exception):
+    def __init__(self, *args, **kwargs):
+        k8s_api_exception = check.inst_param(
+            kwargs.pop("k8s_api_exception"), "k8s_api_exception", Exception
+        )
+        original_exc_info = check.tuple_param(kwargs.pop("original_exc_info"), "original_exc_info")
+
+        check.invariant(original_exc_info[0] is not None)
+        super(DagsterK8sUnrecoverableAPIError, self).__init__(args[0], *args[1:], **kwargs)
+
+        self.k8s_api_exception = check.opt_inst_param(
+            k8s_api_exception, "k8s_api_exception", Exception
+        )
+        self.original_exc_info = original_exc_info
+
+
 class DagsterK8sPipelineStatusException(Exception):
     pass
 
 
+WHITELISTED_TRANSIENT_K8S_STATUS_CODES = [
+    503,  # Service unavailable
+    504,  # Gateway timeout
+    500,  # Internal server error
+]
+
+
+def k8s_api_retry(
+    fn,
+    max_retries,
+    timeout,
+    msg_fn=lambda: "Unexpected error encountered in Kubernetes API Client.",
+):
+    check.callable_param(fn, "fn")
+    check.int_param(max_retries, "max_retries")
+    check.numeric_param(timeout, "timeout")
+
+    remaining_attempts = 1 + max_retries
+    while remaining_attempts > 0:
+        remaining_attempts -= 1
+
+        try:
+            return fn()
+        except kubernetes.client.rest.ApiException as e:
+            # Only catch whitelisted ApiExceptions
+            status = e.status
+
+            # Check if the status code is generally whitelisted
+            whitelisted = status in WHITELISTED_TRANSIENT_K8S_STATUS_CODES
+
+            # If there are remaining attempts, swallow the error
+            if whitelisted and remaining_attempts > 0:
+                time.sleep(timeout)
+            elif whitelisted and remaining_attempts == 0:
+                raise DagsterK8sAPIRetryLimitExceeded(
+                    msg_fn(),
+                    k8s_api_exception=e,
+                    max_retries=max_retries,
+                    original_exc_info=sys.exc_info(),
+                ) from e
+            else:
+                raise DagsterK8sUnrecoverableAPIError(
+                    msg_fn(),
+                    k8s_api_exception=e,
+                    original_exc_info=sys.exc_info(),
+                ) from e
+
+
 class KubernetesWaitingReasons:
     PodInitializing = "PodInitializing"
     ContainerCreating = "ContainerCreating"
     ErrImagePull = "ErrImagePull"
     ImagePullBackOff = "ImagePullBackOff"
     CrashLoopBackOff = "CrashLoopBackOff"
     RunContainerError = "RunContainerError"
+    CreateContainerConfigError = "CreateContainerConfigError"
 
 
 class DagsterKubernetesClient:
     def __init__(self, batch_api, core_api, logger, sleeper, timer):
         self.batch_api = batch_api
         self.core_api = core_api
         self.logger = logger
@@ -49,78 +140,75 @@
             kubernetes.client.BatchV1Api(),
             kubernetes.client.CoreV1Api(),
             logging.info,
             time.sleep,
             time.time,
         )
 
-    def delete_job(
-        self, job_name, namespace,
+    ### Job operations ###
+
+    def wait_for_job(
+        self,
+        job_name,
+        namespace,
+        wait_timeout=DEFAULT_WAIT_TIMEOUT,
+        wait_time_between_attempts=DEFAULT_WAIT_BETWEEN_ATTEMPTS,
+        start_time=None,
     ):
-        """Delete Kubernetes Job. We also need to delete corresponding pods due to:
-        https://github.com/kubernetes-client/python/issues/234
+        """Wait for a job to launch and be running.
 
         Args:
             job_name (str): Name of the job to wait for.
             namespace (str): Namespace in which the job is located.
+            wait_timeout (numeric, optional): Timeout after which to give up and raise exception.
+                Defaults to DEFAULT_WAIT_TIMEOUT. Set to 0 to disable.
+            wait_time_between_attempts (numeric, optional): Wait time between polling attempts. Defaults
+                to DEFAULT_WAIT_BETWEEN_ATTEMPTS.
+
+        Raises:
+            DagsterK8sError: Raised when wait_timeout is exceeded or an error is encountered.
         """
         check.str_param(job_name, "job_name")
         check.str_param(namespace, "namespace")
+        check.numeric_param(wait_timeout, "wait_timeout")
+        check.numeric_param(wait_time_between_attempts, "wait_time_between_attempts")
 
-        pod_names = self.get_pod_names_for_job(job_name, namespace)
-
-        try:
-            # Collect all the errors so that we can post-process before raising
-            errors = []
-            try:
-                self.batch_api.delete_namespaced_job(name=job_name, namespace=namespace)
-            except Exception as e:  # pylint: disable=broad-except
-                errors.append(e)
-
-            for pod_name in pod_names:
-                try:
-                    self.core_api.delete_namespaced_pod(name=pod_name, namespace=namespace)
-                except Exception as e:  # pylint: disable=broad-except
-                    errors.append(e)
-
-            if len(errors) > 0:
-                # Raise first non-expected error. Else, raise first error.
-                for error in errors:
-                    if not (
-                        isinstance(error, kubernetes.client.rest.ApiException)
-                        and error.reason == "Not Found"
-                    ):
-                        raise error
-                raise errors[0]
-
-            return True
-        except kubernetes.client.rest.ApiException as e:
-            if e.reason == "Not Found":
-                return False
-            raise e
-
-    def get_pod_names_for_job(self, job_name, namespace):
-        """Get pod names that corresponds to job name
+        job = None
+        start = start_time or self.timer()
 
-        Args:
-            job_name (str): Name of the job to wait for.
-            namespace (str): Namespace in which the job is located.
-        """
-        check.str_param(job_name, "job_name")
-        check.str_param(namespace, "namespace")
+        while not job:
+            if wait_timeout and (self.timer() - start > wait_timeout):
+                raise DagsterK8sTimeoutError(
+                    "Timed out while waiting for job {job_name}"
+                    " to launch".format(job_name=job_name)
+                )
 
-        pods = self.core_api.list_namespaced_pod(
-            label_selector="job-name=={}".format(job_name), namespace=namespace
-        )
+            # Get all jobs in the namespace and find the matching job
+            def _get_jobs_for_namespace():
+                jobs = self.batch_api.list_namespaced_job(
+                    namespace=namespace, field_selector="metadata.name={}".format(job_name)
+                )
+                if jobs.items:
+                    check.invariant(
+                        len(jobs.items) == 1,
+                        'There should only be one k8s job with name "{}", but got multiple jobs:" {}'.format(
+                            job_name, jobs.items
+                        ),
+                    )
+                    return jobs.items[0]
+                else:
+                    return None
 
-        pod_names = []
-        for item in pods.items:
-            pod_names.append(item.metadata.name)
+            job = k8s_api_retry(
+                _get_jobs_for_namespace, max_retries=3, timeout=wait_time_between_attempts
+            )
 
-        return pod_names
+            if not job:
+                self.logger('Job "{job_name}" not yet launched, waiting'.format(job_name=job_name))
+                self.sleeper(wait_time_between_attempts)
 
     def wait_for_job_success(
         self,
         job_name,
         namespace,
         instance=None,
         run_id=None,
@@ -130,145 +218,190 @@
     ):
         """Poll a job for successful completion.
 
         Args:
             job_name (str): Name of the job to wait for.
             namespace (str): Namespace in which the job is located.
             wait_timeout (numeric, optional): Timeout after which to give up and raise exception.
-                Defaults to DEFAULT_WAIT_TIMEOUT.
+                Defaults to DEFAULT_WAIT_TIMEOUT. Set to 0 to disable.
             wait_time_between_attempts (numeric, optional): Wait time between polling attempts. Defaults
                 to DEFAULT_WAIT_BETWEEN_ATTEMPTS.
 
         Raises:
             DagsterK8sError: Raised when wait_timeout is exceeded or an error is encountered.
         """
         check.str_param(job_name, "job_name")
         check.str_param(namespace, "namespace")
         check.opt_inst_param(instance, "instance", DagsterInstance)
         check.opt_str_param(run_id, "run_id")
         check.numeric_param(wait_timeout, "wait_timeout")
         check.numeric_param(wait_time_between_attempts, "wait_time_between_attempts")
         check.int_param(num_pods_to_wait_for, "num_pods_to_wait_for")
 
-        job = None
         start = self.timer()
 
-        # Ensure we found the job that we launched
-        while not job:
-            if self.timer() - start > wait_timeout:
-
-                raise DagsterK8sError("Timed out while waiting for job to launch")
-
-            jobs = self.batch_api.list_namespaced_job(namespace=namespace)
-            job = next((j for j in jobs.items if j.metadata.name == job_name), None)
+        # Wait for job to be running
+        self.wait_for_job(
+            job_name,
+            namespace,
+            wait_timeout=wait_timeout,
+            wait_time_between_attempts=wait_time_between_attempts,
+            start_time=start,
+        )
 
-            if not job:
-                self.logger('Job "{job_name}" not yet launched, waiting'.format(job_name=job_name))
-                self.sleeper(wait_time_between_attempts)
+        self.wait_for_running_job_to_succeed(
+            job_name,
+            namespace,
+            instance,
+            run_id,
+            wait_timeout,
+            wait_time_between_attempts,
+            num_pods_to_wait_for,
+            start=start,
+        )
 
-        # Wait for job completed status
+    def wait_for_running_job_to_succeed(
+        self,
+        job_name,
+        namespace,
+        instance=None,
+        run_id=None,
+        wait_timeout=DEFAULT_WAIT_TIMEOUT,
+        wait_time_between_attempts=DEFAULT_WAIT_BETWEEN_ATTEMPTS,
+        num_pods_to_wait_for=DEFAULT_JOB_POD_COUNT,
+        start=None,
+    ):
+        # Wait for the job status to be completed. We check the status every
+        # wait_time_between_attempts seconds
         while True:
-            if self.timer() - start > wait_timeout:
-                raise DagsterK8sError("Timed out while waiting for job to complete")
-
-            # See: https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.11/#jobstatus-v1-batch
-            status = self.batch_api.read_namespaced_job_status(job_name, namespace=namespace).status
-
-            if status.failed and status.failed > 0:
-                pods = self.core_api.list_namespaced_pod(
-                    label_selector="job-name=={}".format(job_name), namespace=namespace
+            if wait_timeout and (self.timer() - start > wait_timeout):
+                raise DagsterK8sTimeoutError(
+                    "Timed out while waiting for job {job_name}"
+                    " to complete".format(job_name=job_name)
                 )
-                logs = {}
-                for pod in pods.items:
-                    pod_name = pod.metadata.name
-                    try:
-                        logs[pod_name] = self.core_api.read_namespaced_pod_log(
-                            name=pod_name, namespace=namespace
-                        )
-                    except kubernetes.client.rest.ApiException as e:
-                        logs[pod_name] = e
 
-                raise DagsterK8sError(
-                    "Encountered failed job pods with status: {}, and logs: {}".format(status, logs)
-                )
+            # Reads the status of the specified job. Returns a V1Job object that
+            # we need to read the status off of.
+            status = None
+
+            def _get_job_status():
+                job = self.batch_api.read_namespaced_job_status(job_name, namespace=namespace)
+                return job.status
+
+            status = k8s_api_retry(
+                _get_job_status, max_retries=3, timeout=wait_time_between_attempts
+            )
 
-            # done waiting for pod completion
+            # status.succeeded represents the number of pods which reached phase Succeeded.
             if status.succeeded == num_pods_to_wait_for:
                 break
 
+            # status.failed represents the number of pods which reached phase Failed.
+            if status.failed and status.failed > 0:
+                raise DagsterK8sError(
+                    "Encountered failed job pods for job {job_name} with status: {status}, "
+                    "in namespace {namespace}".format(
+                        job_name=job_name, status=status, namespace=namespace
+                    )
+                )
+
             if instance and run_id:
-                pipeline_run_status = instance.get_run_by_id(run_id).status
+                pipeline_run = instance.get_run_by_id(run_id)
+                if not pipeline_run:
+                    raise DagsterK8sPipelineStatusException()
+
+                pipeline_run_status = pipeline_run.status
                 if pipeline_run_status != PipelineRunStatus.STARTED:
                     raise DagsterK8sPipelineStatusException()
 
             self.sleeper(wait_time_between_attempts)
 
-    def retrieve_pod_logs(self, pod_name, namespace):
-        """Retrieves the raw pod logs for the pod named `pod_name` from Kubernetes.
+    def delete_job(
+        self,
+        job_name,
+        namespace,
+    ):
+        """Delete Kubernetes Job. We also need to delete corresponding pods due to:
+        https://github.com/kubernetes-client/python/issues/234
 
         Args:
-            pod_name (str): The name of the pod from which to retrieve logs.
-            namespace (str): The namespace of the pod.
-
-        Returns:
-            str: The raw logs retrieved from the pod.
+            job_name (str): Name of the job to wait for.
+            namespace (str): Namespace in which the job is located.
         """
-        check.str_param(pod_name, "pod_name")
+        check.str_param(job_name, "job_name")
         check.str_param(namespace, "namespace")
 
-        # We set _preload_content to False here to prevent the k8 python api from processing the response.
-        # If the logs happen to be JSON - it will parse in to a dict and then coerce back to a str leaving
-        # us with invalid JSON as the quotes have been switched to '
-        #
-        # https://github.com/kubernetes-client/python/issues/811
-        return six.ensure_str(
-            self.core_api.read_namespaced_pod_log(
-                name=pod_name, namespace=namespace, _preload_content=False
-            ).data
-        )
+        try:
+            pod_names = self.get_pod_names_in_job(job_name, namespace)
 
-    def wait_for_job(
-        self,
-        job_name,
-        namespace,
-        wait_timeout=DEFAULT_WAIT_TIMEOUT,
-        wait_time_between_attempts=DEFAULT_WAIT_BETWEEN_ATTEMPTS,
-    ):
-        """ Wait for a job to launch and be running.
+            # Collect all the errors so that we can post-process before raising
+            pod_names = self.get_pod_names_in_job(job_name, namespace)
+
+            errors = []
+            try:
+                self.batch_api.delete_namespaced_job(name=job_name, namespace=namespace)
+            except Exception as e:
+                errors.append(e)
+
+            for pod_name in pod_names:
+                try:
+                    self.core_api.delete_namespaced_pod(name=pod_name, namespace=namespace)
+                except Exception as e:
+                    errors.append(e)
+
+            if len(errors) > 0:
+                # Raise first non-expected error. Else, raise first error.
+                for error in errors:
+                    if not (
+                        isinstance(error, kubernetes.client.rest.ApiException)
+                        and error.reason == "Not Found"
+                    ):
+                        raise error
+                raise errors[0]
+
+            return True
+        except kubernetes.client.rest.ApiException as e:
+            if e.reason == "Not Found":
+                return False
+            raise e
+
+    ### Pod operations ###
+
+    def get_pods_in_job(self, job_name, namespace):
+        """Get the pods launched by the job ``job_name``.
 
         Args:
-            job_name (str): Name of the job to wait for.
+            job_name (str): Name of the job to inspect.
             namespace (str): Namespace in which the job is located.
-            wait_timeout (numeric, optional): Timeout after which to give up and raise exception.
-                Defaults to DEFAULT_WAIT_TIMEOUT.
-            wait_time_between_attempts (numeric, optional): Wait time between polling attempts. Defaults
-                to DEFAULT_WAIT_BETWEEN_ATTEMPTS.
 
-        Raises:
-            DagsterK8sError: Raised when wait_timeout is exceeded or an error is encountered.
+        Returns:
+            List[V1Pod]: List of all pod objects that have been launched by the job ``job_name``.
         """
         check.str_param(job_name, "job_name")
         check.str_param(namespace, "namespace")
-        check.numeric_param(wait_timeout, "wait_timeout")
-        check.numeric_param(wait_time_between_attempts, "wait_time_between_attempts")
 
-        job = None
+        return self.core_api.list_namespaced_pod(
+            namespace=namespace, label_selector="job-name={}".format(job_name)
+        ).items
 
-        start = self.timer()
-        # Ensure we found the job that we launched
-        while not job:
-            if self.timer() - start > wait_timeout:
-                raise DagsterK8sError("Timed out while waiting for job to launch")
+    def get_pod_names_in_job(self, job_name, namespace):
+        """Get the names of pods launched by the job ``job_name``.
 
-            jobs = self.batch_api.list_namespaced_job(namespace=namespace)
-            job = next((j for j in jobs.items if j.metadata.name == job_name), None)
+        Args:
+            job_name (str): Name of the job to inspect.
+            namespace (str): Namespace in which the job is located.
 
-            if not job:
-                self.logger('Job "{job_name}" not yet launched, waiting'.format(job_name=job_name))
-                self.sleeper(wait_time_between_attempts)
+        Returns:
+            List[str]: List of all pod names that have been launched by the job ``job_name``.
+        """
+        check.str_param(job_name, "job_name")
+        check.str_param(namespace, "namespace")
+
+        pods = self.get_pods_in_job(job_name, namespace)
+        return [p.metadata.name for p in pods]
 
     def wait_for_pod(
         self,
         pod_name,
         namespace,
         wait_for_state=WaitForPodState.Ready,
         wait_timeout=DEFAULT_WAIT_TIMEOUT,
@@ -278,15 +411,15 @@
 
         Args:
             pod_name (str): Name of the pod to wait for.
             namespace (str): Namespace in which the pod is located.
             wait_for_state (WaitForPodState, optional): Whether to wait for pod readiness or
                 termination. Defaults to waiting for readiness.
             wait_timeout (numeric, optional): Timeout after which to give up and raise exception.
-                Defaults to DEFAULT_WAIT_TIMEOUT.
+                Defaults to DEFAULT_WAIT_TIMEOUT. Set to 0 to disable.
             wait_time_between_attempts (numeric, optional): Wait time between polling attempts. Defaults
                 to DEFAULT_WAIT_BETWEEN_ATTEMPTS.
 
         Raises:
             DagsterK8sError: Raised when wait_timeout is exceeded or an error is encountered
         """
         check.str_param(pod_name, "pod_name")
@@ -302,15 +435,15 @@
         while True:
 
             pods = self.core_api.list_namespaced_pod(
                 namespace=namespace, field_selector="metadata.name=%s" % pod_name
             ).items
             pod = pods[0] if pods else None
 
-            if self.timer() - start > wait_timeout:
+            if wait_timeout and self.timer() - start > wait_timeout:
                 raise DagsterK8sError(
                     "Timed out while waiting for pod to become ready with pod info: %s" % str(pod)
                 )
 
             if pod is None:
                 self.logger('Waiting for pod "%s" to launch...' % pod_name)
                 self.sleeper(wait_time_between_attempts)
@@ -348,14 +481,21 @@
 
             elif state.waiting is not None:
                 # https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#containerstatewaiting-v1-core
                 if state.waiting.reason == KubernetesWaitingReasons.PodInitializing:
                     self.logger('Waiting for pod "%s" to initialize...' % pod_name)
                     self.sleeper(wait_time_between_attempts)
                     continue
+                if state.waiting.reason == KubernetesWaitingReasons.CreateContainerConfigError:
+                    self.logger(
+                        'Pod "%s" is waiting due to a CreateContainerConfigError with message "%s" - trying again to see if it recovers'
+                        % (pod_name, state.waiting.message)
+                    )
+                    self.sleeper(wait_time_between_attempts)
+                    continue
                 elif state.waiting.reason == KubernetesWaitingReasons.ContainerCreating:
                     self.logger("Waiting for container creation...")
                     self.sleeper(wait_time_between_attempts)
                     continue
                 elif state.waiting.reason in [
                     KubernetesWaitingReasons.ErrImagePull,
                     KubernetesWaitingReasons.ImagePullBackOff,
@@ -370,35 +510,40 @@
                 else:
                     raise DagsterK8sError("Unknown issue: %s" % state.waiting)
 
             # https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#containerstateterminated-v1-core
             elif state.terminated is not None:
                 if not state.terminated.exit_code == 0:
                     raw_logs = self.retrieve_pod_logs(pod_name, namespace)
+                    message = state.terminated.message
                     raise DagsterK8sError(
-                        'Pod did not exit successfully. Failed with message: "%s" and pod logs: "%s"'
-                        % (state.terminated.message, str(raw_logs))
+                        f'Pod did not exit successfully. Failed with message: "{message}" '
+                        f'and pod logs: "{raw_logs}"'
                     )
                 else:
                     self.logger("Pod {pod_name} exitted successfully".format(pod_name=pod_name))
                 break
 
             else:
                 raise DagsterK8sError("Should not get here, unknown pod state")
 
-    def get_pod_names_in_job(self, job_name, namespace):
-        """Get the names of pods launched by the job ``job_name``.
+    def retrieve_pod_logs(self, pod_name: str, namespace: str) -> str:
+        """Retrieves the raw pod logs for the pod named `pod_name` from Kubernetes.
 
         Args:
-            job_name (str): Name of the job to inspect.
-            namespace (str): Namespace in which the job is located.
+            pod_name (str): The name of the pod from which to retrieve logs.
+            namespace (str): The namespace of the pod.
 
         Returns:
-            List[str]: List of all pod names that have been launched by the job ``job_name``.
+            str: The raw logs retrieved from the pod.
         """
-        check.str_param(job_name, "job_name")
+        check.str_param(pod_name, "pod_name")
         check.str_param(namespace, "namespace")
 
-        pods = self.core_api.list_namespaced_pod(
-            namespace=namespace, label_selector="job-name={}".format(job_name)
-        ).items
-        return [p.metadata.name for p in pods]
+        # We set _preload_content to False here to prevent the k8 python api from processing the response.
+        # If the logs happen to be JSON - it will parse in to a dict and then coerce back to a str leaving
+        # us with invalid JSON as the quotes have been switched to '
+        #
+        # https://github.com/kubernetes-client/python/issues/811
+        return self.core_api.read_namespaced_pod_log(
+            name=pod_name, namespace=namespace, _preload_content=False
+        ).data.decode("utf-8")
```

### Comparing `dagster-k8s-0.9.9rc1/dagster_k8s/job.py` & `dagster-k8s-1.0.5/dagster_k8s/job.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,46 @@
+import copy
 import hashlib
 import json
 import random
 import string
 from collections import namedtuple
+from typing import Any, Dict, List, Optional
 
 import kubernetes
-import six
 
-from dagster import Array, Field, Noneable, StringSource
+import dagster._check as check
+from dagster import Array, BoolSource, Field, Noneable, StringSource
 from dagster import __version__ as dagster_version
-from dagster import check
-from dagster.config.field_utils import Permissive, Shape
-from dagster.config.validate import validate_config
-from dagster.core.errors import DagsterInvalidConfigError
-from dagster.serdes import whitelist_for_serdes
-from dagster.utils import frozentags, merge_dicts
+from dagster._config import Permissive, Shape, validate_config
+from dagster._core.errors import DagsterInvalidConfigError
+from dagster._core.utils import parse_env_var
+from dagster._serdes import whitelist_for_serdes
+from dagster._utils import frozentags, merge_dicts
 
-# To retry step job, users should raise RetryRequested() so that the dagster system is aware of the
+from .models import k8s_model_from_dict, k8s_snake_case_dict
+from .utils import sanitize_k8s_label
+
+# To retry step worker, users should raise RetryRequested() so that the dagster system is aware of the
 # retry. As an example, see retry_pipeline in dagster_test.test_project.test_pipelines.repo
 # To override this config, user can specify UserDefinedDagsterK8sConfig.
-K8S_JOB_BACKOFF_LIMIT = 0
+DEFAULT_K8S_JOB_BACKOFF_LIMIT = 0
 
-K8S_JOB_TTL_SECONDS_AFTER_FINISHED = 24 * 60 * 60  # 1 day
+DEFAULT_K8S_JOB_TTL_SECONDS_AFTER_FINISHED = 24 * 60 * 60  # 1 day
 
 DAGSTER_HOME_DEFAULT = "/opt/dagster/dagster_home"
 
 # The Kubernetes Secret containing the PG password will be exposed as this env var in the job
 # container.
 DAGSTER_PG_PASSWORD_ENV_VAR = "DAGSTER_PG_PASSWORD"
 
 # We expect the PG secret to have this key.
 #
 # For an example, see:
-# python_modules/libraries/dagster-k8s/helm/dagster/templates/secret-postgres.yaml
+# helm/dagster/templates/secret-postgres.yaml
 DAGSTER_PG_PASSWORD_SECRET_KEY = "postgresql-password"
 
 # Kubernetes Job object names cannot be longer than 63 characters
 MAX_K8S_NAME_LEN = 63
 
 # TODO: Deprecate this tag
 K8S_RESOURCE_REQUIREMENTS_KEY = "dagster-k8s/resource_requirements"
@@ -50,14 +54,19 @@
         "pod_spec_config": Permissive(),
         "job_config": Permissive(),
         "job_metadata": Permissive(),
         "job_spec_config": Permissive(),
     }
 )
 
+DEFAULT_JOB_SPEC_CONFIG = {
+    "ttl_seconds_after_finished": DEFAULT_K8S_JOB_TTL_SECONDS_AFTER_FINISHED,
+    "backoff_limit": DEFAULT_K8S_JOB_BACKOFF_LIMIT,
+}
+
 
 class UserDefinedDagsterK8sConfig(
     namedtuple(
         "_UserDefinedDagsterK8sConfig",
         "container_config pod_template_spec_metadata pod_spec_config job_config job_metadata job_spec_config",
     )
 ):
@@ -76,14 +85,34 @@
             pod_template_spec_metadata, "pod_template_spec_metadata", key_type=str
         )
         pod_spec_config = check.opt_dict_param(pod_spec_config, "pod_spec_config", key_type=str)
         job_config = check.opt_dict_param(job_config, "job_config", key_type=str)
         job_metadata = check.opt_dict_param(job_metadata, "job_metadata", key_type=str)
         job_spec_config = check.opt_dict_param(job_spec_config, "job_spec_config", key_type=str)
 
+        if container_config:
+            container_config = k8s_snake_case_dict(kubernetes.client.V1Container, container_config)
+
+        if pod_template_spec_metadata:
+            pod_template_spec_metadata = k8s_snake_case_dict(
+                kubernetes.client.V1ObjectMeta, pod_template_spec_metadata
+            )
+
+        if pod_spec_config:
+            pod_spec_config = k8s_snake_case_dict(kubernetes.client.V1PodSpec, pod_spec_config)
+
+        if job_config:
+            job_config = k8s_snake_case_dict(kubernetes.client.V1Job, job_config)
+
+        if job_metadata:
+            job_metadata = k8s_snake_case_dict(kubernetes.client.V1ObjectMeta, job_metadata)
+
+        if job_spec_config:
+            job_spec_config = k8s_snake_case_dict(kubernetes.client.V1JobSpec, job_spec_config)
+
         return super(UserDefinedDagsterK8sConfig, cls).__new__(
             cls,
             container_config=container_config,
             pod_template_spec_metadata=pod_template_spec_metadata,
             pod_spec_config=pod_spec_config,
             job_config=job_config,
             job_metadata=job_metadata,
@@ -117,15 +146,17 @@
     check.invariant(K8S_RESOURCE_REQUIREMENTS_KEY in tags)
 
     resource_requirements = json.loads(tags[K8S_RESOURCE_REQUIREMENTS_KEY])
     result = validate_config(K8S_RESOURCE_REQUIREMENTS_SCHEMA, resource_requirements)
 
     if not result.success:
         raise DagsterInvalidConfigError(
-            "Error in tags for {}".format(K8S_RESOURCE_REQUIREMENTS_KEY), result.errors, result,
+            "Error in tags for {}".format(K8S_RESOURCE_REQUIREMENTS_KEY),
+            result.errors,
+            result,
         )
 
     return result.value
 
 
 def get_user_defined_k8s_config(tags):
     check.inst_param(tags, "tags", frozentags)
@@ -137,15 +168,17 @@
 
     if USER_DEFINED_K8S_CONFIG_KEY in tags:
         user_defined_k8s_config_value = json.loads(tags[USER_DEFINED_K8S_CONFIG_KEY])
         result = validate_config(USER_DEFINED_K8S_CONFIG_SCHEMA, user_defined_k8s_config_value)
 
         if not result.success:
             raise DagsterInvalidConfigError(
-                "Error in tags for {}".format(USER_DEFINED_K8S_CONFIG_KEY), result.errors, result,
+                "Error in tags for {}".format(USER_DEFINED_K8S_CONFIG_KEY),
+                result.errors,
+                result,
             )
 
         user_defined_k8s_config = result.value
 
     container_config = user_defined_k8s_config.get("container_config", {})
 
     # Backcompat for resource requirements key
@@ -156,35 +189,37 @@
         )
 
     return UserDefinedDagsterK8sConfig(
         container_config=container_config,
         pod_template_spec_metadata=user_defined_k8s_config.get("pod_template_spec_metadata"),
         pod_spec_config=user_defined_k8s_config.get("pod_spec_config"),
         job_config=user_defined_k8s_config.get("job_config"),
+        job_metadata=user_defined_k8s_config.get("job_metadata"),
         job_spec_config=user_defined_k8s_config.get("job_spec_config"),
     )
 
 
-def get_job_name_from_run_id(run_id):
-    return "dagster-run-{}".format(run_id)
+def get_job_name_from_run_id(run_id, resume_attempt_number=None):
+    return "dagster-run-{}".format(run_id) + (
+        "" if not resume_attempt_number else "-{}".format(resume_attempt_number)
+    )
 
 
 @whitelist_for_serdes
 class DagsterK8sJobConfig(
     namedtuple(
         "_K8sJobTaskConfig",
         "job_image dagster_home image_pull_policy image_pull_secrets service_account_name "
-        "instance_config_map postgres_password_secret env_config_maps env_secrets",
+        "instance_config_map postgres_password_secret env_config_maps env_secrets env_vars "
+        "volume_mounts volumes labels resources",
     )
 ):
     """Configuration parameters for launching Dagster Jobs on Kubernetes.
 
     Params:
-        job_image (str): The docker image to use. The Job container will be launched with this
-            image.
         dagster_home (str): The location of DAGSTER_HOME in the Job container; this is where the
             ``dagster.yaml`` file will be mounted from the instance ConfigMap specified here.
         image_pull_policy (Optional[str]): Allows the image pull policy to be overridden, e.g. to
             facilitate local testing with `kind <https://kind.sigs.k8s.io/>`_. Default:
             ``"Always"``. See:
             https://kubernetes.io/docs/concepts/containers/images/#updating-images.
         image_pull_secrets (Optional[List[Dict[str, str]]]): Optionally, a list of dicts, each of
@@ -195,126 +230,175 @@
             https://kubernetes.io/docs/concepts/containers/images/#specifying-imagepullsecrets-on-a-pod
             and https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.17/#podspec-v1-core
         service_account_name (Optional[str]): The name of the Kubernetes service account under which
             to run the Job. Defaults to "default"
         instance_config_map (str): The ``name`` of an existing Volume to mount into the pod in
             order to provide a ConfigMap for the Dagster instance. This Volume should contain a
             ``dagster.yaml`` with appropriate values for run storage, event log storage, etc.
-        postgres_password_secret (str): The name of the Kubernetes Secret where the postgres
+        postgres_password_secret (Optional[str]): The name of the Kubernetes Secret where the postgres
             password can be retrieved. Will be mounted and supplied as an environment variable to
             the Job Pod.
         env_config_maps (Optional[List[str]]): A list of custom ConfigMapEnvSource names from which to
             draw environment variables (using ``envFrom``) for the Job. Default: ``[]``. See:
-        https://kubernetes.io/docs/tasks/inject-data-application/define-environment-variable-container/#define-an-environment-variable-for-a-container
+            https://kubernetes.io/docs/tasks/inject-data-application/define-environment-variable-container/#define-an-environment-variable-for-a-container
         env_secrets (Optional[List[str]]): A list of custom Secret names from which to
             draw environment variables (using ``envFrom``) for the Job. Default: ``[]``. See:
-        https://kubernetes.io/docs/tasks/inject-data-application/distribute-credentials-secure/#configure-all-key-value-pairs-in-a-secret-as-container-environment-variables
-
+            https://kubernetes.io/docs/tasks/inject-data-application/distribute-credentials-secure/#configure-all-key-value-pairs-in-a-secret-as-container-environment-variables
+        env_vars (Optional[List[str]]): A list of environment variables to inject into the Job.
+            Default: ``[]``. See: https://kubernetes.io/docs/tasks/inject-data-application/distribute-credentials-secure/#configure-all-key-value-pairs-in-a-secret-as-container-environment-variables
+        job_image (Optional[str]): The docker image to use. The Job container will be launched with this
+            image. Should not be specified if using userDeployments.
+        volume_mounts (Optional[List[Permissive]]): A list of volume mounts to include in the job's
+            container. Default: ``[]``. See:
+            https://v1-18.docs.kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#volumemount-v1-core
+        volumes (Optional[List[Permissive]]): A list of volumes to include in the Job's Pod. Default: ``[]``. See:
+            https://v1-18.docs.kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#volume-v1-core
+        labels (Optional[Dict[str, str]]): Additional labels that should be included in the Job's Pod. See:
+            https://kubernetes.io/docs/concepts/overview/working-with-objects/labels
+        resources (Optional[Dict[str, Any]]) Compute resource requirements for the container. See:
+            https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/
     """
 
     def __new__(
         cls,
         job_image=None,
         dagster_home=None,
         image_pull_policy=None,
         image_pull_secrets=None,
         service_account_name=None,
         instance_config_map=None,
         postgres_password_secret=None,
         env_config_maps=None,
         env_secrets=None,
+        env_vars=None,
+        volume_mounts=None,
+        volumes=None,
+        labels=None,
+        resources=None,
     ):
         return super(DagsterK8sJobConfig, cls).__new__(
             cls,
             job_image=check.opt_str_param(job_image, "job_image"),
-            dagster_home=check.opt_str_param(
-                dagster_home, "dagster_home", default=DAGSTER_HOME_DEFAULT
-            ),
-            image_pull_policy=check.opt_str_param(image_pull_policy, "image_pull_policy"),
+            dagster_home=check.opt_str_param(dagster_home, "dagster_home"),
+            image_pull_policy=check.opt_str_param(image_pull_policy, "image_pull_policy", "Always"),
             image_pull_secrets=check.opt_list_param(
                 image_pull_secrets, "image_pull_secrets", of_type=dict
             ),
             service_account_name=check.opt_str_param(service_account_name, "service_account_name"),
-            instance_config_map=check.str_param(instance_config_map, "instance_config_map"),
-            postgres_password_secret=check.str_param(
+            instance_config_map=check.opt_str_param(instance_config_map, "instance_config_map"),
+            postgres_password_secret=check.opt_str_param(
                 postgres_password_secret, "postgres_password_secret"
             ),
             env_config_maps=check.opt_list_param(env_config_maps, "env_config_maps", of_type=str),
             env_secrets=check.opt_list_param(env_secrets, "env_secrets", of_type=str),
+            env_vars=check.opt_list_param(env_vars, "env_vars", of_type=str),
+            volume_mounts=[
+                k8s_snake_case_dict(kubernetes.client.V1VolumeMount, mount)
+                for mount in check.opt_list_param(volume_mounts, "volume_mounts")
+            ],
+            volumes=[
+                k8s_snake_case_dict(kubernetes.client.V1Volume, volume)
+                for volume in check.opt_list_param(volumes, "volumes")
+            ],
+            labels=check.opt_dict_param(labels, "labels", key_type=str, value_type=str),
+            resources=check.opt_dict_param(resources, "resources", key_type=str),
         )
 
     @classmethod
-    def config_type(cls):
-        """Combined config type which includes both run launcher and pipeline run config.
-        """
-        cfg_run_launcher = DagsterK8sJobConfig.config_type_run_launcher()
-        cfg_pipeline_run = DagsterK8sJobConfig.config_type_pipeline_run()
-        return merge_dicts(cfg_run_launcher, cfg_pipeline_run)
+    def config_type_run_launcher(cls):
+        """Configuration intended to be set on the Dagster instance for the run launcher."""
+
+        return merge_dicts(
+            DagsterK8sJobConfig.config_type_job(),
+            {
+                "instance_config_map": Field(
+                    StringSource,
+                    is_required=True,
+                    description="The ``name`` of an existing Volume to mount into the pod in order to "
+                    "provide a ConfigMap for the Dagster instance. This Volume should contain a "
+                    "``dagster.yaml`` with appropriate values for run storage, event log storage, etc.",
+                ),
+                "postgres_password_secret": Field(
+                    StringSource,
+                    is_required=False,
+                    description="The name of the Kubernetes Secret where the postgres password can be "
+                    "retrieved. Will be mounted and supplied as an environment variable to the Job Pod."
+                    'Secret must contain the key ``"postgresql-password"`` which will be exposed in '
+                    "the Job environment as the environment variable ``DAGSTER_PG_PASSWORD``.",
+                ),
+                "dagster_home": Field(
+                    StringSource,
+                    is_required=False,
+                    default_value=DAGSTER_HOME_DEFAULT,
+                    description="The location of DAGSTER_HOME in the Job container; this is where the "
+                    "``dagster.yaml`` file will be mounted from the instance ConfigMap specified here. "
+                    "Defaults to /opt/dagster/dagster_home.",
+                ),
+                "load_incluster_config": Field(
+                    bool,
+                    is_required=False,
+                    default_value=True,
+                    description="""Set this value if you are running the launcher
+            within a k8s cluster. If ``True``, we assume the launcher is running within the target
+            cluster and load config using ``kubernetes.config.load_incluster_config``. Otherwise,
+            we will use the k8s config specified in ``kubeconfig_file`` (using
+            ``kubernetes.config.load_kube_config``) or fall back to the default kubeconfig.""",
+                ),
+                "kubeconfig_file": Field(
+                    Noneable(str),
+                    is_required=False,
+                    default_value=None,
+                    description="The kubeconfig file from which to load config. Defaults to using the default kubeconfig.",
+                ),
+                "fail_pod_on_run_failure": Field(
+                    bool,
+                    is_required=False,
+                    description="Whether the launched Kubernetes Jobs and Pods should fail if the Dagster run fails",
+                ),
+            },
+        )
 
     @classmethod
-    def config_type_run_launcher(cls):
-        """Configuration intended to be set on the Dagster instance.
-        """
-        return {
-            "instance_config_map": Field(
-                StringSource,
-                is_required=True,
-                description="The ``name`` of an existing Volume to mount into the pod in order to "
-                "provide a ConfigMap for the Dagster instance. This Volume should contain a "
-                "``dagster.yaml`` with appropriate values for run storage, event log storage, etc.",
-            ),
-            "postgres_password_secret": Field(
-                StringSource,
-                is_required=True,
-                description="The name of the Kubernetes Secret where the postgres password can be "
-                "retrieved. Will be mounted and supplied as an environment variable to the Job Pod."
-                'Secret must contain the key ``"postgresql-password"`` which will be exposed in '
-                "the Job environment as the environment variable ``DAGSTER_PG_PASSWORD``.",
-            ),
-            "dagster_home": Field(
-                StringSource,
-                is_required=False,
-                default_value=DAGSTER_HOME_DEFAULT,
-                description="The location of DAGSTER_HOME in the Job container; this is where the "
-                "``dagster.yaml`` file will be mounted from the instance ConfigMap specified here. "
-                "Defaults to /opt/dagster/dagster_home.",
-            ),
-        }
+    def config_type_job(cls):
+        """Configuration intended to be set when creating a k8s job (e.g. in an executor that runs
+        each op in its own k8s job, or a run launcher that create a k8s job for the run worker).
+        Shares most of the schema with the container_context, but for back-compat reasons,
+        'namespace' is called 'job_namespace'."""
+
+        return merge_dicts(
+            {
+                "job_image": Field(
+                    Noneable(StringSource),
+                    is_required=False,
+                    description="Docker image to use for launched Jobs. If this field is empty, "
+                    "the image that was used to originally load the Dagster repository will be used. "
+                    '(Ex: "mycompany.com/dagster-k8s-image:latest").',
+                ),
+            },
+            DagsterK8sJobConfig.config_type_container(),
+        )
 
     @classmethod
-    def config_type_pipeline_run(cls):
-        """Configuration intended to be set at pipeline execution time.
-        """
+    def config_type_container(cls):
         return {
-            "job_image": Field(
-                Noneable(StringSource),
-                is_required=False,
-                description="Docker image to use for launched task Jobs. If the repository is not "
-                "loaded from a GRPC server, then this field is required. If the repository is "
-                "loaded from a GRPC server, then leave this field empty."
-                '(Ex: "mycompany.com/dagster-k8s-image:latest").',
-            ),
             "image_pull_policy": Field(
-                StringSource,
+                Noneable(StringSource),
                 is_required=False,
-                default_value="IfNotPresent",
-                description="Image pull policy to set on the launched task Job Pods. Defaults to "
-                '"IfNotPresent".',
+                description="Image pull policy to set on launched Pods.",
             ),
             "image_pull_secrets": Field(
                 Noneable(Array(Shape({"name": StringSource}))),
                 is_required=False,
-                description="(Advanced) Specifies that Kubernetes should get the credentials from "
+                description="Specifies that Kubernetes should get the credentials from "
                 "the Secrets named in this list.",
             ),
             "service_account_name": Field(
                 Noneable(StringSource),
                 is_required=False,
-                description="(Advanced) Override the name of the Kubernetes service account under "
-                "which to run the Job.",
+                description="The name of the Kubernetes service account under which to run.",
             ),
             "env_config_maps": Field(
                 Noneable(Array(StringSource)),
                 is_required=False,
                 description="A list of custom ConfigMapEnvSource names from which to draw "
                 "environment variables (using ``envFrom``) for the Job. Default: ``[]``. See:"
                 "https://kubernetes.io/docs/tasks/inject-data-application/define-environment-variable-container/#define-an-environment-variable-for-a-container",
@@ -322,187 +406,309 @@
             "env_secrets": Field(
                 Noneable(Array(StringSource)),
                 is_required=False,
                 description="A list of custom Secret names from which to draw environment "
                 "variables (using ``envFrom``) for the Job. Default: ``[]``. See:"
                 "https://kubernetes.io/docs/tasks/inject-data-application/distribute-credentials-secure/#configure-all-key-value-pairs-in-a-secret-as-container-environment-variables",
             ),
+            "env_vars": Field(
+                Noneable(Array(str)),
+                is_required=False,
+                description="A list of environment variables to inject into the Job. Each can be "
+                "of the form KEY=VALUE or just KEY (in which case the value will be pulled from "
+                "the current process). Default: ``[]``. See: "
+                "https://kubernetes.io/docs/tasks/inject-data-application/distribute-credentials-secure/#configure-all-key-value-pairs-in-a-secret-as-container-environment-variables",
+            ),
+            "volume_mounts": Field(
+                Array(
+                    # Can supply either snake_case or camelCase, but in typeaheads based on the
+                    # schema we assume snake_case
+                    Permissive(
+                        {
+                            "name": StringSource,
+                            "mount_path": Field(StringSource, is_required=False),
+                            "mount_propagation": Field(StringSource, is_required=False),
+                            "read_only": Field(BoolSource, is_required=False),
+                            "sub_path": Field(StringSource, is_required=False),
+                            "sub_path_expr": Field(StringSource, is_required=False),
+                        }
+                    )
+                ),
+                is_required=False,
+                default_value=[],
+                description="A list of volume mounts to include in the job's container. Default: ``[]``. See: "
+                "https://v1-18.docs.kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#volumemount-v1-core",
+            ),
+            "volumes": Field(
+                Array(
+                    Permissive(
+                        {
+                            "name": str,
+                        }
+                    )
+                ),
+                is_required=False,
+                default_value=[],
+                description="A list of volumes to include in the Job's Pod. Default: ``[]``. For the many "
+                "possible volume source types that can be included, see: "
+                "https://v1-18.docs.kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#volume-v1-core",
+            ),
+            "labels": Field(
+                dict,
+                is_required=False,
+                description="Labels to apply to all created pods. See: "
+                "https://kubernetes.io/docs/concepts/overview/working-with-objects/labels",
+            ),
+            "resources": Field(
+                Noneable(
+                    {
+                        "limits": Field(dict, is_required=False),
+                        "requests": Field(dict, is_required=False),
+                    }
+                ),
+                is_required=False,
+                description="Compute resource requirements for the container. See: "
+                "https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/",
+            ),
         }
 
+    @classmethod
+    def config_type_container_context(cls):
+        return merge_dicts(
+            DagsterK8sJobConfig.config_type_container(),
+            {
+                "namespace": Field(
+                    Noneable(StringSource),
+                    is_required=False,
+                    description="The namespace into which to launch Kubernetes resources. Note that any "
+                    "other required resources (such as the service account) must be "
+                    "present in this namespace.",
+                ),
+            },
+        )
+
+    @property
+    def env(self) -> List[Dict[str, Optional[str]]]:
+        parsed_env_vars = [parse_env_var(key) for key in (self.env_vars or [])]
+        return [
+            {"name": parsed_env_var[0], "value": parsed_env_var[1]}
+            for parsed_env_var in parsed_env_vars
+        ]
+
     @property
-    def env_from_sources(self):
+    def env_from_sources(self) -> List[Dict[str, Any]]:
         """This constructs a list of env_from sources. Along with a default base environment
         config map which we always load, the ConfigMaps and Secrets specified via
         env_config_maps and env_secrets will be pulled into the job construction here.
         """
         config_maps = [
-            kubernetes.client.V1EnvFromSource(
-                config_map_ref=kubernetes.client.V1ConfigMapEnvSource(name=config_map)
-            )
-            for config_map in self.env_config_maps
+            {"config_map_ref": {"name": config_map}} for config_map in self.env_config_maps
         ]
 
-        secrets = [
-            kubernetes.client.V1EnvFromSource(
-                secret_ref=kubernetes.client.V1SecretEnvSource(name=secret)
-            )
-            for secret in self.env_secrets
-        ]
+        secrets = [{"secret_ref": {"name": secret}} for secret in self.env_secrets]
 
         return config_maps + secrets
 
     def to_dict(self):
         return self._asdict()
 
+    def with_image(self, image):
+        return self._replace(job_image=image)
+
     @staticmethod
     def from_dict(config=None):
         check.opt_dict_param(config, "config")
         return DagsterK8sJobConfig(**config)
 
 
 def construct_dagster_k8s_job(
     job_config,
-    command,
     args,
     job_name,
     user_defined_k8s_config=None,
     pod_name=None,
     component=None,
-    env_vars=None,
+    labels=None,
 ):
     """Constructs a Kubernetes Job object for a dagster-graphql invocation.
 
     Args:
         job_config (DagsterK8sJobConfig): Job configuration to use for constructing the Kubernetes
             Job object.
-        command (List[str]): Command to run.
         args (List[str]): CLI arguments to use with dagster-graphql in this Job.
         job_name (str): The name of the Job. Note that this name must be <= 63 characters in length.
-        resources (Dict[str, Dict[str, str]]): The resource requirements for the container
+        user_defined_k8s_config(Optional[UserDefinedDagsterK8sConfig]): Additional k8s config in tags or Dagster config
+            to apply to the job.
         pod_name (str, optional): The name of the Pod. Note that this name must be <= 63 characters
             in length. Defaults to "<job_name>-pod".
         component (str, optional): The name of the component, used to provide the Job label
             app.kubernetes.io/component. Defaults to None.
-        env_vars(Dict[str, str]): Additional environment variables to add to the K8s Container.
+        labels(Dict[str, str]): Additional labels to be attached to k8s jobs and pod templates.
+            Long label values are may be truncated.
 
     Returns:
         kubernetes.client.V1Job: A Kubernetes Job object.
     """
     check.inst_param(job_config, "job_config", DagsterK8sJobConfig)
-    command = check.list_param(command, "command", of_type=str)
     check.list_param(args, "args", of_type=str)
     check.str_param(job_name, "job_name")
     user_defined_k8s_config = check.opt_inst_param(
         user_defined_k8s_config,
         "user_defined_k8s_config",
         UserDefinedDagsterK8sConfig,
-        UserDefinedDagsterK8sConfig(),
+        default=UserDefinedDagsterK8sConfig(),
     )
 
     pod_name = check.opt_str_param(pod_name, "pod_name", default=job_name + "-pod")
     check.opt_str_param(component, "component")
-    check.opt_dict_param(env_vars, "env_vars", key_type=str, value_type=str)
+    check.opt_dict_param(labels, "labels", key_type=str, value_type=str)
 
     check.invariant(
         len(job_name) <= MAX_K8S_NAME_LEN,
         "job_name is %d in length; Kubernetes Jobs cannot be longer than %d characters."
         % (len(job_name), MAX_K8S_NAME_LEN),
     )
 
     check.invariant(
         len(pod_name) <= MAX_K8S_NAME_LEN,
         "job_name is %d in length; Kubernetes Pods cannot be longer than %d characters."
         % (len(pod_name), MAX_K8S_NAME_LEN),
     )
 
     # See: https://kubernetes.io/docs/concepts/overview/working-with-objects/common-labels/
-    dagster_labels = {
+    k8s_common_labels = {
         "app.kubernetes.io/name": "dagster",
         "app.kubernetes.io/instance": "dagster",
-        "app.kubernetes.io/version": dagster_version,
+        "app.kubernetes.io/version": sanitize_k8s_label(dagster_version),
         "app.kubernetes.io/part-of": "dagster",
     }
 
     if component:
-        dagster_labels["app.kubernetes.io/component"] = component
+        k8s_common_labels["app.kubernetes.io/component"] = component
 
-    additional_k8s_env_vars = []
-    if env_vars:
-        for key, value in env_vars.items():
-            additional_k8s_env_vars.append(kubernetes.client.V1EnvVar(name=key, value=value))
-
-    job_container = kubernetes.client.V1Container(
-        name=job_name,
-        image=job_config.job_image,
-        command=command,
-        args=args,
-        image_pull_policy=job_config.image_pull_policy,
-        env=[
-            kubernetes.client.V1EnvVar(name="DAGSTER_HOME", value=job_config.dagster_home),
-            kubernetes.client.V1EnvVar(
-                name=DAGSTER_PG_PASSWORD_ENV_VAR,
-                value_from=kubernetes.client.V1EnvVarSource(
-                    secret_key_ref=kubernetes.client.V1SecretKeySelector(
-                        name=job_config.postgres_password_secret, key=DAGSTER_PG_PASSWORD_SECRET_KEY
-                    )
-                ),
-            ),
-        ]
-        + additional_k8s_env_vars,
-        env_from=job_config.env_from_sources,
-        volume_mounts=[
-            kubernetes.client.V1VolumeMount(
-                name="dagster-instance",
-                mount_path="{dagster_home}/dagster.yaml".format(
-                    dagster_home=job_config.dagster_home
-                ),
-                sub_path="dagster.yaml",
-            )
-        ],
-        **user_defined_k8s_config.container_config
+    additional_labels = {k: sanitize_k8s_label(v) for k, v in (labels or {}).items()}
+    dagster_labels = merge_dicts(k8s_common_labels, additional_labels)
+
+    env = (
+        [{"name": "DAGSTER_HOME", "value": job_config.dagster_home}]
+        if job_config.dagster_home
+        else []
     )
+    if job_config.postgres_password_secret:
+        env.append(
+            {
+                "name": DAGSTER_PG_PASSWORD_ENV_VAR,
+                "value_from": {
+                    "secret_key_ref": {
+                        "name": job_config.postgres_password_secret,
+                        "key": DAGSTER_PG_PASSWORD_SECRET_KEY,
+                    }
+                },
+            }
+        )
 
-    config_map_volume = kubernetes.client.V1Volume(
-        name="dagster-instance",
-        config_map=kubernetes.client.V1ConfigMapVolumeSource(name=job_config.instance_config_map),
+    container_config = copy.deepcopy(user_defined_k8s_config.container_config)
+
+    user_defined_env_vars = container_config.pop("env", [])
+
+    user_defined_env_from = container_config.pop("env_from", [])
+
+    job_image = container_config.pop("image", job_config.job_image)
+
+    user_defined_k8s_volume_mounts = container_config.pop("volume_mounts", [])
+
+    user_defined_resources = container_config.pop("resources", {})
+
+    volume_mounts = job_config.volume_mounts + user_defined_k8s_volume_mounts
+
+    resources = user_defined_resources if user_defined_resources else job_config.resources
+
+    container_config = merge_dicts(
+        container_config,
+        {
+            "name": "dagster",
+            "image": job_image,
+            "args": args,
+            "image_pull_policy": job_config.image_pull_policy,
+            "env": env + job_config.env + user_defined_env_vars,
+            "env_from": job_config.env_from_sources + user_defined_env_from,
+            "volume_mounts": volume_mounts,
+            "resources": resources,
+        },
     )
 
-    template = kubernetes.client.V1PodTemplateSpec(
-        metadata=kubernetes.client.V1ObjectMeta(
-            name=pod_name,
-            labels=dagster_labels,
-            **user_defined_k8s_config.pod_template_spec_metadata
+    pod_spec_config = copy.deepcopy(user_defined_k8s_config.pod_spec_config)
+
+    user_defined_volumes = pod_spec_config.pop("volumes", [])
+
+    volumes = job_config.volumes + user_defined_volumes
+
+    # If the user has defined custom labels, remove them from the pod_template_spec_metadata
+    # key and merge them with the dagster labels
+    pod_template_spec_metadata = copy.deepcopy(user_defined_k8s_config.pod_template_spec_metadata)
+    user_defined_pod_template_labels = pod_template_spec_metadata.pop("labels", {})
+
+    service_account_name = pod_spec_config.pop(
+        "service_account_name", job_config.service_account_name
+    )
+
+    user_defined_containers = pod_spec_config.pop("containers", [])
+
+    template = {
+        "metadata": merge_dicts(
+            pod_template_spec_metadata,
+            {
+                "name": pod_name,
+                "labels": merge_dicts(
+                    dagster_labels, user_defined_pod_template_labels, job_config.labels
+                ),
+            },
         ),
-        spec=kubernetes.client.V1PodSpec(
-            image_pull_secrets=[
-                kubernetes.client.V1LocalObjectReference(name=x["name"])
-                for x in job_config.image_pull_secrets
-            ],
-            service_account_name=job_config.service_account_name,
-            restart_policy="Never",
-            containers=[job_container],
-            volumes=[config_map_volume],
-            **user_defined_k8s_config.pod_spec_config
+        "spec": merge_dicts(
+            pod_spec_config,
+            {
+                "image_pull_secrets": job_config.image_pull_secrets,
+                "service_account_name": service_account_name,
+                "restart_policy": "Never",
+                "containers": [container_config] + user_defined_containers,
+                "volumes": volumes,
+            },
         ),
+    }
+
+    job_spec_config = merge_dicts(
+        DEFAULT_JOB_SPEC_CONFIG,
+        user_defined_k8s_config.job_spec_config,
+        {"template": template},
     )
 
-    job = kubernetes.client.V1Job(
-        api_version="batch/v1",
-        kind="Job",
-        metadata=kubernetes.client.V1ObjectMeta(
-            name=job_name, labels=dagster_labels, **user_defined_k8s_config.job_metadata
-        ),
-        spec=kubernetes.client.V1JobSpec(
-            template=template,
-            backoff_limit=K8S_JOB_BACKOFF_LIMIT,
-            ttl_seconds_after_finished=K8S_JOB_TTL_SECONDS_AFTER_FINISHED,
-            **user_defined_k8s_config.job_spec_config
+    user_defined_job_metadata = copy.deepcopy(user_defined_k8s_config.job_metadata)
+    user_defined_job_labels = user_defined_job_metadata.pop("labels", {})
+
+    job = k8s_model_from_dict(
+        kubernetes.client.V1Job,
+        merge_dicts(
+            user_defined_k8s_config.job_config,
+            {
+                "api_version": "batch/v1",
+                "kind": "Job",
+                "metadata": merge_dicts(
+                    user_defined_job_metadata,
+                    {
+                        "name": job_name,
+                        "labels": merge_dicts(
+                            dagster_labels, user_defined_job_labels, job_config.labels
+                        ),
+                    },
+                ),
+                "spec": job_spec_config,
+            },
         ),
-        **user_defined_k8s_config.job_config
     )
+
     return job
 
 
 def get_k8s_job_name(input_1, input_2=None):
     """Creates a unique (short!) identifier to name k8s objects based on run ID and step key(s).
 
     K8s Job names are limited to 63 characters, because they are used as labels. For more info, see:
@@ -512,10 +718,10 @@
     check.str_param(input_1, "input_1")
     check.opt_str_param(input_2, "input_2")
     if not input_2:
         letters = string.ascii_lowercase
         input_2 = "".join(random.choice(letters) for i in range(20))
 
     # Creates 32-bit signed int, so could be negative
-    name_hash = hashlib.md5(six.ensure_binary(input_1 + input_2))
+    name_hash = hashlib.md5((input_1 + input_2).encode("utf-8"))
 
     return name_hash.hexdigest()
```

### Comparing `dagster-k8s-0.9.9rc1/dagster_k8s/launcher.py` & `dagster-k8s-1.0.5/dagster_k8s/launcher.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,325 +1,365 @@
-import weakref
+import sys
+from typing import Dict, List, Optional
 
 import kubernetes
 
-from dagster import (
-    DagsterInvariantViolationError,
-    EventMetadataEntry,
-    Field,
-    Noneable,
-    StringSource,
-    check,
-)
-from dagster.cli.api import ExecuteRunArgs
-from dagster.core.events import EngineEventData
-from dagster.core.host_representation import ExternalPipeline
-from dagster.core.host_representation.handle import GrpcServerRepositoryLocationHandle
-from dagster.core.instance import DagsterInstance
-from dagster.core.launcher import RunLauncher
-from dagster.core.origin import PipelineGrpcServerOrigin, PipelinePythonOrigin
-from dagster.core.storage.pipeline_run import PipelineRun, PipelineRunStatus
-from dagster.serdes import ConfigurableClass, ConfigurableClassData, serialize_dagster_namedtuple
-from dagster.utils import frozentags, merge_dicts
+from dagster import Field, MetadataEntry, StringSource
+from dagster import _check as check
+from dagster._cli.api import ExecuteRunArgs
+from dagster._core.events import EngineEventData
+from dagster._core.launcher import LaunchRunContext, ResumeRunContext, RunLauncher
+from dagster._core.launcher.base import CheckRunHealthResult, WorkerStatus
+from dagster._core.storage.pipeline_run import PipelineRun, PipelineRunStatus
+from dagster._core.storage.tags import DOCKER_IMAGE_TAG
+from dagster._grpc.types import ResumeRunArgs
+from dagster._serdes import ConfigurableClass, ConfigurableClassData
+from dagster._utils import frozentags, merge_dicts
+from dagster._utils.error import serializable_error_info_from_exc_info
 
+from .container_context import K8sContainerContext
 from .job import (
     DagsterK8sJobConfig,
     construct_dagster_k8s_job,
     get_job_name_from_run_id,
     get_user_defined_k8s_config,
 )
 from .utils import delete_job
 
 
 class K8sRunLauncher(RunLauncher, ConfigurableClass):
-    """RunLauncher that starts a Kubernetes Job for each pipeline run.
+    """RunLauncher that starts a Kubernetes Job for each Dagster job run.
 
-    Encapsulates each pipeline run in a separate, isolated invocation of ``dagster-graphql``.
+    Encapsulates each run in a separate, isolated invocation of ``dagster-graphql``.
 
-    You may configure a Dagster instance to use this RunLauncher by adding a section to your
+    You can configure a Dagster instance to use this RunLauncher by adding a section to your
     ``dagster.yaml`` like the following:
 
     .. code-block:: yaml
 
         run_launcher:
-            module: dagster_k8s.launcher
-            class: K8sRunLauncher
-            config:
-                service_account_name: pipeline_run_service_account
-                job_image: my_project/dagster_image:latest
-                instance_config_map: dagster-instance
-                postgres_password_secret: dagster-postgresql-secret
-
-    As always when using a :py:class:`~dagster.serdes.ConfigurableClass`, the values
-    under the ``config`` key of this YAML block will be passed to the constructor. The full list
-    of acceptable values is given below by the constructor args.
-
-    Args:
-        service_account_name (str): The name of the Kubernetes service account under which to run
-            the Job.
-        job_image (str): The ``name`` of the image to use for the Job's Dagster container. This
-            image will be run with the command
-            ``dagster-graphql -p startPipelineExecution -v {executionParams}``.
-        instance_config_map (str): The ``name`` of an existing Volume to mount into the pod in
-            order to provide a ConfigMap for the Dagster instance. This Volume should contain a
-            ``dagster.yaml`` with appropriate values for run storage, event log storage, etc.
-        postgres_password_secret (str): The name of the Kubernetes Secret where the postgres
-            password can be retrieved. Will be mounted and supplied as an environment variable to
-            the Job Pod.
-        dagster_home (str): The location of DAGSTER_HOME in the Job container; this is where the
-            ``dagster.yaml`` file will be mounted from the instance ConfigMap specified above.
-        load_incluster_config (Optional[bool]):  Set this value if you are running the launcher
-            within a k8s cluster. If ``True``, we assume the launcher is running within the target
-            cluster and load config using ``kubernetes.config.load_incluster_config``. Otherwise,
-            we will use the k8s config specified in ``kubeconfig_file`` (using
-            ``kubernetes.config.load_kube_config``) or fall back to the default kubeconfig. Default:
-            ``True``.
-        kubeconfig_file (Optional[str]): The kubeconfig file from which to load config. Defaults to
-            None (using the default kubeconfig).
-        image_pull_secrets (Optional[List[Dict[str, str]]]): Optionally, a list of dicts, each of
-            which corresponds to a Kubernetes ``LocalObjectReference`` (e.g.,
-            ``{'name': 'myRegistryName'}``). This allows you to specify the ```imagePullSecrets`` on
-            a pod basis. Typically, these will be provided through the service account, when needed,
-            and you will not need to pass this argument.
-            See:
-            https://kubernetes.io/docs/concepts/containers/images/#specifying-imagepullsecrets-on-a-pod
-            and https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.17/#podspec-v1-core.
-        image_pull_policy (Optional[str]): Allows the image pull policy to be overridden, e.g. to
-            facilitate local testing with `kind <https://kind.sigs.k8s.io/>`_. Default:
-            ``"Always"``. See: https://kubernetes.io/docs/concepts/containers/images/#updating-images.
-        job_namespace (Optional[str]): The namespace into which to launch new jobs. Note that any
-            other Kubernetes resources the Job requires (such as the service account) must be
-            present in this namespace. Default: ``"default"``
-        env_config_maps (Optional[List[str]]): A list of custom ConfigMapEnvSource names from which to
-            draw environment variables (using ``envFrom``) for the Job. Default: ``[]``. See:
-        https://kubernetes.io/docs/tasks/inject-data-application/define-environment-variable-container/#define-an-environment-variable-for-a-container
-        env_secrets (Optional[List[str]]): A list of custom Secret names from which to
-            draw environment variables (using ``envFrom``) for the Job. Default: ``[]``. See:
-        https://kubernetes.io/docs/tasks/inject-data-application/distribute-credentials-secure/#configure-all-key-value-pairs-in-a-secret-as-container-environment-variables
+          module: dagster_k8s.launcher
+          class: K8sRunLauncher
+          config:
+            service_account_name: your_service_account
+            job_image: my_project/dagster_image:latest
+            instance_config_map: dagster-instance
+            postgres_password_secret: dagster-postgresql-secret
+
     """
 
     def __init__(
         self,
         service_account_name,
         instance_config_map,
-        postgres_password_secret,
-        dagster_home,
+        postgres_password_secret=None,
+        dagster_home=None,
         job_image=None,
-        image_pull_policy="Always",
+        image_pull_policy=None,
         image_pull_secrets=None,
         load_incluster_config=True,
         kubeconfig_file=None,
         inst_data=None,
         job_namespace="default",
         env_config_maps=None,
         env_secrets=None,
+        env_vars=None,
+        k8s_client_batch_api=None,
+        volume_mounts=None,
+        volumes=None,
+        labels=None,
+        fail_pod_on_run_failure=None,
+        resources=None,
     ):
         self._inst_data = check.opt_inst_param(inst_data, "inst_data", ConfigurableClassData)
         self.job_namespace = check.str_param(job_namespace, "job_namespace")
 
+        self.load_incluster_config = load_incluster_config
+        self.kubeconfig_file = kubeconfig_file
         if load_incluster_config:
             check.invariant(
                 kubeconfig_file is None,
                 "`kubeconfig_file` is set but `load_incluster_config` is True.",
             )
             kubernetes.config.load_incluster_config()
         else:
             check.opt_str_param(kubeconfig_file, "kubeconfig_file")
             kubernetes.config.load_kube_config(kubeconfig_file)
 
-        self._batch_api = kubernetes.client.BatchV1Api()
-        self._core_api = kubernetes.client.CoreV1Api()
+        self._fixed_batch_api = k8s_client_batch_api
 
-        self.job_config = None
+        self._job_config = None
         self._job_image = check.opt_str_param(job_image, "job_image")
-        self._dagster_home = check.str_param(dagster_home, "dagster_home")
-        self._image_pull_policy = check.str_param(image_pull_policy, "image_pull_policy")
+        self.dagster_home = check.str_param(dagster_home, "dagster_home")
+        self._image_pull_policy = check.opt_str_param(
+            image_pull_policy, "image_pull_policy", "IfNotPresent"
+        )
         self._image_pull_secrets = check.opt_list_param(
             image_pull_secrets, "image_pull_secrets", of_type=dict
         )
         self._service_account_name = check.str_param(service_account_name, "service_account_name")
-        self._instance_config_map = check.str_param(instance_config_map, "instance_config_map")
-        self._postgres_password_secret = check.str_param(
+        self.instance_config_map = check.str_param(instance_config_map, "instance_config_map")
+        self.postgres_password_secret = check.opt_str_param(
             postgres_password_secret, "postgres_password_secret"
         )
         self._env_config_maps = check.opt_list_param(
             env_config_maps, "env_config_maps", of_type=str
         )
         self._env_secrets = check.opt_list_param(env_secrets, "env_secrets", of_type=str)
-        self._instance_ref = None
+        self._env_vars = check.opt_list_param(env_vars, "env_vars", of_type=str)
+        self._volume_mounts = check.opt_list_param(volume_mounts, "volume_mounts")
+        self._volumes = check.opt_list_param(volumes, "volumes")
+        self._labels = check.opt_dict_param(labels, "labels", key_type=str, value_type=str)
+        self._fail_pod_on_run_failure = check.opt_bool_param(
+            fail_pod_on_run_failure, "fail_pod_on_run_failure"
+        )
+        self._resources = check.opt_dict_param(resources, "resources")
+
+        super().__init__()
+
+    @property
+    def job_image(self):
+        return self._job_image
+
+    @property
+    def image_pull_policy(self) -> str:
+        return self._image_pull_policy
+
+    @property
+    def image_pull_secrets(self) -> List[Dict]:
+        return self._image_pull_secrets
+
+    @property
+    def service_account_name(self) -> str:
+        return self._service_account_name
+
+    @property
+    def env_config_maps(self) -> List[str]:
+        return self._env_config_maps
+
+    @property
+    def env_secrets(self) -> List[str]:
+        return self._env_secrets
+
+    @property
+    def volume_mounts(self) -> List:
+        return self._volume_mounts
+
+    @property
+    def volumes(self) -> List:
+        return self._volumes
+
+    @property
+    def resources(self) -> Dict:
+        return self._resources
+
+    @property
+    def env_vars(self) -> List[str]:
+        return self._env_vars
+
+    @property
+    def labels(self) -> Dict[str, str]:
+        return self._labels
+
+    @property
+    def fail_pod_on_run_failure(self) -> Optional[bool]:
+        return self._fail_pod_on_run_failure
+
+    @property
+    def _batch_api(self):
+        return self._fixed_batch_api if self._fixed_batch_api else kubernetes.client.BatchV1Api()
 
     @classmethod
     def config_type(cls):
         """Include all arguments required for DagsterK8sJobConfig along with additional arguments
         needed for the RunLauncher itself.
         """
-        job_cfg = DagsterK8sJobConfig.config_type()
+        job_cfg = DagsterK8sJobConfig.config_type_run_launcher()
 
         run_launcher_extra_cfg = {
-            "job_namespace": StringSource,
-            "load_incluster_config": Field(bool, is_required=False, default_value=True),
-            "kubeconfig_file": Field(Noneable(str), is_required=False, default_value=None),
+            "job_namespace": Field(StringSource, is_required=False, default_value="default"),
         }
         return merge_dicts(job_cfg, run_launcher_extra_cfg)
 
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
-    def _get_static_job_config(self):
-        if self.job_config:
-            return self.job_config
-        else:
-            self.job_config = DagsterK8sJobConfig(
-                job_image=check.str_param(self._job_image, "job_image"),
-                dagster_home=check.str_param(self._dagster_home, "dagster_home"),
-                image_pull_policy=check.str_param(self._image_pull_policy, "image_pull_policy"),
-                image_pull_secrets=check.opt_list_param(
-                    self._image_pull_secrets, "image_pull_secrets", of_type=dict
-                ),
-                service_account_name=check.str_param(
-                    self._service_account_name, "service_account_name"
-                ),
-                instance_config_map=check.str_param(
-                    self._instance_config_map, "instance_config_map"
-                ),
-                postgres_password_secret=check.str_param(
-                    self._postgres_password_secret, "postgres_password_secret"
-                ),
-                env_config_maps=check.opt_list_param(
-                    self._env_config_maps, "env_config_maps", of_type=str
-                ),
-                env_secrets=check.opt_list_param(self._env_secrets, "env_secrets", of_type=str),
-            )
-            return self.job_config
-
-    def _get_grpc_job_config(self, job_image):
-        return DagsterK8sJobConfig(
-            job_image=check.str_param(job_image, "job_image"),
-            dagster_home=check.str_param(self._dagster_home, "dagster_home"),
-            image_pull_policy=check.str_param(self._image_pull_policy, "image_pull_policy"),
-            image_pull_secrets=check.opt_list_param(
-                self._image_pull_secrets, "image_pull_secrets", of_type=dict
-            ),
-            service_account_name=check.str_param(
-                self._service_account_name, "service_account_name"
-            ),
-            instance_config_map=check.str_param(self._instance_config_map, "instance_config_map"),
-            postgres_password_secret=check.str_param(
-                self._postgres_password_secret, "postgres_password_secret"
-            ),
-            env_config_maps=check.opt_list_param(
-                self._env_config_maps, "env_config_maps", of_type=str
-            ),
-            env_secrets=check.opt_list_param(self._env_secrets, "env_secrets", of_type=str),
-        )
-
-    def initialize(self, instance):
-        check.inst_param(instance, "instance", DagsterInstance)
-        # Store a weakref to avoid a circular reference / enable GC
-        self._instance_ref = weakref.ref(instance)
+    def get_container_context_for_run(self, pipeline_run: PipelineRun) -> K8sContainerContext:
+        return K8sContainerContext.create_for_run(pipeline_run, self)
 
-    def launch_run(self, instance, run, external_pipeline):
-        check.inst_param(run, "run", PipelineRun)
-        check.inst_param(external_pipeline, "external_pipeline", ExternalPipeline)
+    def _launch_k8s_job_with_args(self, job_name, args, run):
+        container_context = self.get_container_context_for_run(run)
 
-        job_name = "dagster-run-{}".format(run.run_id)
         pod_name = job_name
 
-        user_defined_k8s_config = get_user_defined_k8s_config(frozentags(external_pipeline.tags))
-
-        pipeline_origin = None
-        job_config = None
-        if isinstance(external_pipeline.get_origin(), PipelineGrpcServerOrigin):
-            if self._job_image:
-                raise DagsterInvariantViolationError(
-                    "Cannot specify job_image in run launcher config when loading pipeline "
-                    "from GRPC server."
-                )
-
-            repository_location_handle = (
-                external_pipeline.repository_handle.repository_location_handle
-            )
-
-            if not isinstance(repository_location_handle, GrpcServerRepositoryLocationHandle):
-                raise DagsterInvariantViolationError(
-                    "Expected RepositoryLocationHandle to be of type "
-                    "GrpcServerRepositoryLocationHandle but found type {}".format(
-                        type(repository_location_handle)
-                    )
-                )
-
-            job_image = repository_location_handle.get_current_image()
-
-            job_config = self._get_grpc_job_config(job_image)
+        pipeline_origin = run.pipeline_code_origin
+        user_defined_k8s_config = get_user_defined_k8s_config(frozentags(run.tags))
+        repository_origin = pipeline_origin.repository_origin
 
-            repository_name = external_pipeline.repository_handle.repository_name
-            pipeline_origin = PipelinePythonOrigin(
-                pipeline_name=external_pipeline.name,
-                repository_origin=repository_location_handle.get_repository_python_origin(
-                    repository_name
-                ),
-            )
-        else:
-            pipeline_origin = external_pipeline.get_origin()
-            job_config = self._get_static_job_config()
+        job_config = container_context.get_k8s_job_config(
+            job_image=repository_origin.container_image, run_launcher=self
+        )
 
-        input_json = serialize_dagster_namedtuple(
-            ExecuteRunArgs(
-                pipeline_origin=pipeline_origin, pipeline_run_id=run.run_id, instance_ref=None,
-            )
+        self._instance.add_run_tags(
+            run.run_id,
+            {DOCKER_IMAGE_TAG: job_config.job_image},
         )
 
         job = construct_dagster_k8s_job(
             job_config=job_config,
-            command=["dagster"],
-            args=["api", "execute_run_with_structured_logs", input_json],
+            args=args,
             job_name=job_name,
             pod_name=pod_name,
-            component="run_coordinator",
+            component="run_worker",
             user_defined_k8s_config=user_defined_k8s_config,
+            labels={
+                "dagster/job": pipeline_origin.pipeline_name,
+                "dagster/run-id": run.run_id,
+            },
         )
 
-        self._batch_api.create_namespaced_job(body=job, namespace=self.job_namespace)
         self._instance.report_engine_event(
-            "Kubernetes run_coordinator job launched",
+            "Creating Kubernetes run worker job",
             run,
             EngineEventData(
                 [
-                    EventMetadataEntry.text(job_name, "Kubernetes Job name"),
-                    EventMetadataEntry.text(pod_name, "Kubernetes Pod name"),
-                    EventMetadataEntry.text(self.job_namespace, "Kubernetes Namespace"),
-                    EventMetadataEntry.text(run.run_id, "Run ID"),
+                    MetadataEntry("Kubernetes Job name", value=job_name),
+                    MetadataEntry("Kubernetes Namespace", value=container_context.namespace),
+                    MetadataEntry("Run ID", value=run.run_id),
                 ]
             ),
-            cls=K8sRunLauncher,
+            cls=self.__class__,
+        )
+
+        self._batch_api.create_namespaced_job(body=job, namespace=container_context.namespace)
+        self._instance.report_engine_event(
+            "Kubernetes run worker job created",
+            run,
+            cls=self.__class__,
+        )
+
+    def launch_run(self, context: LaunchRunContext) -> None:
+        run = context.pipeline_run
+        job_name = get_job_name_from_run_id(run.run_id)
+        pipeline_origin = check.not_none(run.pipeline_code_origin)
+
+        args = ExecuteRunArgs(
+            pipeline_origin=pipeline_origin,
+            pipeline_run_id=run.run_id,
+            instance_ref=self._instance.get_ref(),
+            set_exit_code_on_failure=self._fail_pod_on_run_failure,
+        ).get_command_args()
+
+        self._launch_k8s_job_with_args(job_name, args, run)
+
+    @property
+    def supports_resume_run(self):
+        return True
+
+    def resume_run(self, context: ResumeRunContext) -> None:
+        run = context.pipeline_run
+        job_name = get_job_name_from_run_id(
+            run.run_id, resume_attempt_number=context.resume_attempt_number
         )
-        return run
+        pipeline_origin = check.not_none(run.pipeline_code_origin)
+
+        args = ResumeRunArgs(
+            pipeline_origin=pipeline_origin,
+            pipeline_run_id=run.run_id,
+            instance_ref=self._instance.get_ref(),
+            set_exit_code_on_failure=self._fail_pod_on_run_failure,
+        ).get_command_args()
+
+        self._launch_k8s_job_with_args(job_name, args, run)
 
     # https://github.com/dagster-io/dagster/issues/2741
     def can_terminate(self, run_id):
         check.str_param(run_id, "run_id")
 
         pipeline_run = self._instance.get_run_by_id(run_id)
         if not pipeline_run:
             return False
         if pipeline_run.status != PipelineRunStatus.STARTED:
             return False
         return True
 
     def terminate(self, run_id):
         check.str_param(run_id, "run_id")
+        run = self._instance.get_run_by_id(run_id)
+
+        if not run:
+            return False
 
-        if not self.can_terminate(run_id):
+        container_context = self.get_container_context_for_run(run)
+
+        can_terminate = self.can_terminate(run_id)
+        if not can_terminate:
+            self._instance.report_engine_event(
+                message="Unable to terminate run; can_terminate returned {}".format(can_terminate),
+                pipeline_run=run,
+                cls=self.__class__,
+            )
             return False
 
-        job_name = get_job_name_from_run_id(run_id)
+        self._instance.report_run_canceling(run)
+
+        job_name = get_job_name_from_run_id(
+            run_id, resume_attempt_number=self._instance.count_resume_run_attempts(run.run_id)
+        )
 
-        return delete_job(job_name=job_name, namespace=self.job_namespace)
+        try:
+            termination_result = delete_job(
+                job_name=job_name, namespace=container_context.namespace
+            )
+            if termination_result:
+                self._instance.report_engine_event(
+                    message="Run was terminated successfully.",
+                    pipeline_run=run,
+                    cls=self.__class__,
+                )
+            else:
+                self._instance.report_engine_event(
+                    message="Run was not terminated successfully; delete_job returned {}".format(
+                        termination_result
+                    ),
+                    pipeline_run=run,
+                    cls=self.__class__,
+                )
+            return termination_result
+        except Exception:
+            self._instance.report_engine_event(
+                message="Run was not terminated successfully; encountered error in delete_job",
+                pipeline_run=run,
+                engine_event_data=EngineEventData.engine_error(
+                    serializable_error_info_from_exc_info(sys.exc_info())
+                ),
+                cls=self.__class__,
+            )
+
+    @property
+    def supports_check_run_worker_health(self):
+        return True
+
+    def check_run_worker_health(self, run: PipelineRun):
+        container_context = self.get_container_context_for_run(run)
+
+        job_name = get_job_name_from_run_id(
+            run.run_id, resume_attempt_number=self._instance.count_resume_run_attempts(run.run_id)
+        )
+        try:
+            job = self._batch_api.read_namespaced_job(
+                namespace=container_context.namespace, name=job_name
+            )
+        except Exception:
+            return CheckRunHealthResult(
+                WorkerStatus.UNKNOWN, str(serializable_error_info_from_exc_info(sys.exc_info()))
+            )
+        if job.status.failed:
+            return CheckRunHealthResult(WorkerStatus.FAILED, "K8s job failed")
+        if job.status.succeeded:
+            return CheckRunHealthResult(WorkerStatus.SUCCESS)
+        return CheckRunHealthResult(WorkerStatus.RUNNING)
```

### Comparing `dagster-k8s-0.9.9rc1/dagster_k8s/test.py` & `dagster-k8s-1.0.5/dagster_k8s/test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,35 @@
-from dagster_graphql.client.util import parse_raw_log_lines
 from dagster_k8s.utils import (
     get_pod_names_in_job,
     retrieve_pod_logs,
     wait_for_job,
     wait_for_job_success,
 )
 
-from dagster import check
+import dagster._check as check
 
 
 def wait_for_job_ready(job_name, namespace):
-    """Wait for a dagster-k8s job to be ready
-    """
+    """Wait for a dagster-k8s job to be ready"""
     check.str_param(job_name, "job_name")
     check.str_param(namespace, "namespace")
 
     wait_for_job(job_name=job_name, namespace=namespace)
 
 
-def wait_for_job_and_get_logs(job_name, namespace):
+def wait_for_job_and_get_raw_logs(job_name, namespace, wait_timeout=300):
     """Wait for a dagster-k8s job to complete, ensure it launched only one pod,
     and then grab the logs from the pod it launched.
-    """
-    check.str_param(job_name, "job_name")
-    check.str_param(namespace, "namespace")
 
-    wait_for_job_success(job_name, namespace=namespace)
-
-    pod_names = get_pod_names_in_job(job_name, namespace)
-
-    assert len(pod_names) == 1
-
-    pod_name = pod_names[0]
-
-    raw_logs = retrieve_pod_logs(pod_name, namespace=namespace)
-    return parse_raw_log_lines(raw_logs.split("\n"))
-
-
-def wait_for_job_and_get_raw_logs(job_name, namespace):
-    """Wait for a dagster-k8s job to complete, ensure it launched only one pod,
-    and then grab the logs from the pod it launched.
+    wait_timeout: default 5 minutes
     """
     check.str_param(job_name, "job_name")
     check.str_param(namespace, "namespace")
 
-    wait_for_job_success(job_name, namespace=namespace)
+    wait_for_job_success(job_name, namespace=namespace, wait_timeout=wait_timeout)
 
     pod_names = get_pod_names_in_job(job_name, namespace)
 
     assert len(pod_names) == 1
 
     pod_name = pod_names[0]
```

### Comparing `dagster-k8s-0.9.9rc1/dagster_k8s.egg-info/PKG-INFO` & `dagster-k8s-1.0.5/dagster_k8s.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-k8s
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: A Dagster integration for k8s
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-k8s
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
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-k8s-0.9.9rc1/dagster_k8s.egg-info/SOURCES.txt` & `dagster-k8s-1.0.5/dagster_k8s.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 dagster_k8s/__init__.py
 dagster_k8s/client.py
-dagster_k8s/config.py
+dagster_k8s/container_context.py
+dagster_k8s/executor.py
 dagster_k8s/job.py
 dagster_k8s/launcher.py
-dagster_k8s/scheduler.py
+dagster_k8s/models.py
+dagster_k8s/py.typed
 dagster_k8s/test.py
 dagster_k8s/utils.py
 dagster_k8s/version.py
 dagster_k8s.egg-info/PKG-INFO
 dagster_k8s.egg-info/SOURCES.txt
 dagster_k8s.egg-info/dependency_links.txt
 dagster_k8s.egg-info/not-zip-safe
 dagster_k8s.egg-info/requires.txt
 dagster_k8s.egg-info/top_level.txt
-dagster_k8s_tests/__init__.py
-dagster_k8s_tests/unit_tests/__init__.py
-dagster_k8s_tests/unit_tests/test_client.py
-dagster_k8s_tests/unit_tests/test_job.py
-dagster_k8s_tests/unit_tests/test_resource_tags.py
-dagster_k8s_tests/unit_tests/test_utils.py
-dagster_k8s_tests/unit_tests/test_version.py
+dagster_k8s/ops/__init__.py
+dagster_k8s/ops/k8s_job_op.py
```

### Comparing `dagster-k8s-0.9.9rc1/setup.py` & `dagster-k8s-1.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,37 @@
+from typing import Dict
+
 from setuptools import find_packages, setup
 
 
-def get_version():
-    version = {}
-    with open("dagster_k8s/version.py") as fp:
+def get_version() -> str:
+    version: Dict[str, str] = {}
+    with open("dagster_k8s/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
 if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
     setup(
         name="dagster-k8s",
-        version=get_version(),
+        version=ver,
         author="Elementl",
         author_email="hello@elementl.com",
         license="Apache-2.0",
         description="A Dagster integration for k8s",
         url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-k8s",
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
-        install_requires=[
-            "dagster",
-            "dagster_graphql",
-            "kubernetes",
-            # RSA 4.1+ is incompatible with py2.7
-            'rsa<=4.0; python_version<"3"',
-        ],
-        tests_require=[],
+        packages=find_packages(exclude=["dagster_k8s_tests*"]),
+        install_requires=["dagster==1.0.5", "kubernetes"],
         zip_safe=False,
     )
```

