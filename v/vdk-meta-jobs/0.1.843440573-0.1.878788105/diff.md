# Comparing `tmp/vdk-meta-jobs-0.1.843440573.tar.gz` & `tmp/vdk-meta-jobs-0.1.878788105.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-meta-jobs-0.1.843440573.tar", last modified: Thu Apr 20 13:17:42 2023, max compression
+gzip compressed data, was "vdk-meta-jobs-0.1.878788105.tar", last modified: Thu May 25 10:48:22 2023, max compression
```

## Comparing `vdk-meta-jobs-0.1.843440573.tar` & `vdk-meta-jobs-0.1.878788105.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:17:42.420170 vdk-meta-jobs-0.1.843440573/
--rw-r--r--   0 root         (0) root         (0)     8509 2023-04-20 13:17:42.420170 vdk-meta-jobs-0.1.843440573/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7936 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 13:17:42.420170 vdk-meta-jobs-0.1.843440573/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1456 2023-04-20 13:17:30.000000 vdk-meta-jobs-0.1.843440573/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:17:42.416170 vdk-meta-jobs-0.1.843440573/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:17:42.416170 vdk-meta-jobs-0.1.843440573/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:17:42.416170 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:17:42.416170 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:17:42.416170 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/api/
--rw-rw-rw-   0 root         (0) root         (0)     1402 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/api/meta_job.py
--rw-rw-rw-   0 root         (0) root         (0)     9347 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/cached_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     7949 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/dag_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/dags_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2269 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     6713 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/meta_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     6438 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/meta_dag.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/meta_job_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     9344 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/remote_data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1743 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/remote_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     2579 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/time_based_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:17:42.420170 vdk-meta-jobs-0.1.843440573/src/vdk_meta_jobs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8509 2023-04-20 13:17:42.000000 vdk-meta-jobs-0.1.843440573/src/vdk_meta_jobs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      858 2023-04-20 13:17:42.000000 vdk-meta-jobs-0.1.843440573/src/vdk_meta_jobs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 13:17:42.000000 vdk-meta-jobs-0.1.843440573/src/vdk_meta_jobs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 13:17:42.000000 vdk-meta-jobs-0.1.843440573/src/vdk_meta_jobs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-20 13:17:42.000000 vdk-meta-jobs-0.1.843440573/src/vdk_meta_jobs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-20 13:17:42.000000 vdk-meta-jobs-0.1.843440573/src/vdk_meta_jobs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:17:42.420170 vdk-meta-jobs-0.1.843440573/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2624 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/tests/test_meta_dag.py
--rw-rw-rw-   0 root         (0) root         (0)    15096 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/tests/test_meta_job.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/tests/test_time_based_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2303 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/tests/test_tracking_job_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:48:22.422975 vdk-meta-jobs-0.1.878788105/
+-rw-r--r--   0 root         (0) root         (0)     8391 2023-05-25 10:48:22.422975 vdk-meta-jobs-0.1.878788105/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7818 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 10:48:22.422975 vdk-meta-jobs-0.1.878788105/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2023-05-25 10:48:12.000000 vdk-meta-jobs-0.1.878788105/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:48:22.418975 vdk-meta-jobs-0.1.878788105/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:48:22.418975 vdk-meta-jobs-0.1.878788105/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:48:22.418975 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:48:22.418975 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:48:22.418975 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1402 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/api/meta_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     9347 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/cached_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7949 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/dag_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/dags_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2269 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     6713 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/meta_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     6148 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/meta_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/meta_job_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     9346 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/remote_data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1743 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/remote_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2579 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/time_based_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:48:22.418975 vdk-meta-jobs-0.1.878788105/src/vdk_meta_jobs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8391 2023-05-25 10:48:22.000000 vdk-meta-jobs-0.1.878788105/src/vdk_meta_jobs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      858 2023-05-25 10:48:22.000000 vdk-meta-jobs-0.1.878788105/src/vdk_meta_jobs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 10:48:22.000000 vdk-meta-jobs-0.1.878788105/src/vdk_meta_jobs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-05-25 10:48:22.000000 vdk-meta-jobs-0.1.878788105/src/vdk_meta_jobs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-25 10:48:22.000000 vdk-meta-jobs-0.1.878788105/src/vdk_meta_jobs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-25 10:48:22.000000 vdk-meta-jobs-0.1.878788105/src/vdk_meta_jobs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:48:22.422975 vdk-meta-jobs-0.1.878788105/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/tests/test_meta_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)    15690 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/tests/test_meta_job.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/tests/test_time_based_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2303 2023-05-25 10:48:08.000000 vdk-meta-jobs-0.1.878788105/tests/test_tracking_job_executor.py
```

### Comparing `vdk-meta-jobs-0.1.843440573/PKG-INFO` & `vdk-meta-jobs-0.1.878788105/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: vdk-meta-jobs
-Version: 0.1.843440573
+Version: 0.1.878788105
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Meta Jobs
 
-## This plugin has been deprecated. Please use vdk-dag instead. You may install it by running `pip install vdk-dag`.
-
 Express dependencies between data jobs.
 
 A plugin for Versatile Data Kit extends its Job API with an additional feature that allows users to trigger so-called Meta Jobs.
 
 A meta job is a regular Data Job that invokes other Data Jobs using Control Service Execution API.
 In this way, there's nothing different from other data jobs except for its purpose. See [Data Job types](https://github.com/vmware/versatile-data-kit/wiki/User-Guide#data-job-types) for more info.
```

### Comparing `vdk-meta-jobs-0.1.843440573/README.md` & `vdk-meta-jobs-0.1.878788105/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # Meta Jobs
 
-## This plugin has been deprecated. Please use vdk-dag instead. You may install it by running `pip install vdk-dag`.
-
 Express dependencies between data jobs.
 
 A plugin for Versatile Data Kit extends its Job API with an additional feature that allows users to trigger so-called Meta Jobs.
 
 A meta job is a regular Data Job that invokes other Data Jobs using Control Service Execution API.
 In this way, there's nothing different from other data jobs except for its purpose. See [Data Job types](https://github.com/vmware/versatile-data-kit/wiki/User-Guide#data-job-types) for more info.
```

### Comparing `vdk-meta-jobs-0.1.843440573/setup.py` & `vdk-meta-jobs-0.1.878788105/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.843440573"
+__version__ = "0.1.878788105"
 
 setuptools.setup(
     name="vdk-meta-jobs",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Express dependecies between data jobs.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/api/meta_job.py` & `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/api/meta_job.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/cached_data_job_executor.py` & `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/cached_data_job_executor.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/dag_validator.py` & `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/dag_validator.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/dags_plugin.py` & `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/dags_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/meta.py` & `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/meta.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/meta_configuration.py` & `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/meta_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/meta_dag.py` & `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/meta_dag.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,20 +25,14 @@
     def __init__(self, team_name: str, meta_config: MetaPluginConfiguration):
         """
         This module deals with all the DAG-related operations such as build and execute.
 
         :param team_name: the name of the owning team
         :param meta_config: the DAG job configuration
         """
-        log.warning(
-            "-------------------------------------------"
-            "This plugin has been deprecated. Please use vdk-dag instead. "
-            "You may install it by running `pip install vdk-dag`."
-            "-------------------------------------------"
-        )
         self._team_name = team_name
         self._topological_sorter = TopologicalSorter()
         self._delayed_starting_jobs = TimeBasedQueue(
             min_ready_time_seconds=meta_config.meta_jobs_delayed_jobs_min_delay_seconds(),
             randomize_delay_seconds=meta_config.meta_jobs_delayed_jobs_randomized_added_delay_seconds(),
         )
         self._max_concurrent_running_jobs = (
```

### Comparing `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/meta_job_runner.py` & `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/meta_job_runner.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/remote_data_job.py` & `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/remote_data_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,21 +96,21 @@
 
         :param: request_kwargs: Request arguments to be included with the HTTP request
         """
         execution_request = DataJobExecutionRequest(
             started_by="meta-job",  # TODO: specify name of meta job
             args=self.__arguments,
         )
-        _, _, headers = self.__execution_api.data_job_execution_start_with_http_info(
+        headers = self.__execution_api.data_job_execution_start_with_http_info(
             team_name=self.__team_name,
             job_name=self.__job_name,
             deployment_id=self.deployment_id,
             data_job_execution_request=execution_request,
             _request_timeout=self.timeout,
-        )
+        ).headers
         log.debug(f"Received headers: {headers}")
 
         job_execution_id = os.path.basename(headers["Location"])
         return job_execution_id
 
     def cancel_job_execution(self, execution_id: str) -> None:
         """
```

### Comparing `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/remote_data_job_executor.py` & `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/remote_data_job_executor.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/time_based_queue.py` & `vdk-meta-jobs-0.1.878788105/src/vdk/plugin/meta_jobs/time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.843440573/src/vdk_meta_jobs.egg-info/PKG-INFO` & `vdk-meta-jobs-0.1.878788105/src/vdk_meta_jobs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: vdk-meta-jobs
-Version: 0.1.843440573
+Version: 0.1.878788105
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Meta Jobs
 
-## This plugin has been deprecated. Please use vdk-dag instead. You may install it by running `pip install vdk-dag`.
-
 Express dependencies between data jobs.
 
 A plugin for Versatile Data Kit extends its Job API with an additional feature that allows users to trigger so-called Meta Jobs.
 
 A meta job is a regular Data Job that invokes other Data Jobs using Control Service Execution API.
 In this way, there's nothing different from other data jobs except for its purpose. See [Data Job types](https://github.com/vmware/versatile-data-kit/wiki/User-Guide#data-job-types) for more info.
```

### Comparing `vdk-meta-jobs-0.1.843440573/src/vdk_meta_jobs.egg-info/SOURCES.txt` & `vdk-meta-jobs-0.1.878788105/src/vdk_meta_jobs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.843440573/tests/test_meta_dag.py` & `vdk-meta-jobs-0.1.878788105/tests/test_meta_dag.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.843440573/tests/test_meta_job.py` & `vdk-meta-jobs-0.1.878788105/tests/test_meta_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import json
 import os
 import time
+from datetime import date
+from datetime import datetime
 from unittest import mock
 
 from click.testing import Result
 from pytest_httpserver.pytest_plugin import PluginHTTPServer
 from taurus_datajob_api import DataJobDeployment
 from taurus_datajob_api import DataJobExecution
 from vdk.internal.core.errors import UserCodeError
@@ -14,14 +16,22 @@
 from vdk.plugin.test_utils.util_funcs import cli_assert_equal
 from vdk.plugin.test_utils.util_funcs import CliEntryBasedTestRunner
 from vdk.plugin.test_utils.util_funcs import jobs_path_from_caller_directory
 from werkzeug import Request
 from werkzeug import Response
 
 
+def json_serial(obj):
+    """JSON serializer for objects not serializable by default json code"""
+
+    if isinstance(obj, (datetime, date)):
+        return obj.isoformat()
+    raise TypeError("Type %s not serializable" % type(obj))
+
+
 class TestMetaJob:
     def _prepare(self):
         rest_api_url = self.httpserver.url_for("")
         team_name = "team-awesome"
         if self.jobs is None:
             self.jobs = [("job" + str(i), [200], "succeeded", 0) for i in range(1, 5)]
 
@@ -58,18 +68,21 @@
                         actual_job_status = "running"
                     execution: DataJobExecution = DataJobExecution(
                         id=job_name,
                         job_name=job_name,
                         logs_url="http://url",
                         deployment=DataJobDeployment(),
                         start_time="2021-09-24T14:14:03.922Z",
+                        end_time="2021-09-24T14:14:03.922Z",
                         status=actual_job_status,
                         message="foo",
                     )
-                    response_data = json.dumps(execution.to_dict(), indent=4)
+                    response_data = json.dumps(
+                        execution.to_dict(), indent=4, default=json_serial
+                    )
                     return Response(
                         response_data,
                         status=200,
                         headers=None,
                         content_type="application/json",
                     )
 
@@ -89,17 +102,19 @@
                         job_name=job_name,
                         logs_url="http://url",
                         deployment=DataJobDeployment(),
                         start_time="2021-09-24T14:14:03.922Z",
                         status="succeeded",
                         message="foo",
                     )
-                    response_data = json.dumps(execution.to_dict(), indent=4)
+                    response_data = json.dumps(
+                        [execution.to_dict()], indent=4, default=json_serial
+                    )
                     return Response(
-                        [response_data],
+                        response_data,
                         status=200,
                         headers=None,
                         content_type="application/json",
                     )
 
                 return _handler_fn
 
@@ -295,14 +310,16 @@
                         job_name = request.path.split("/jobs/")[1].split("/")[0]
                         running_jobs.add(job_name)
                         assert (
                             len(running_jobs) <= expected_max_running_jobs
                         )  # assert that max concurrent running jobs is not exceeded
                     if request.method == "GET":
                         execution = json.loads(response.response[0])
+                        if isinstance(execution, list):
+                            execution = execution[0]
                         if execution["status"] == "succeeded":
                             running_jobs.discard(execution["job_name"])
             cli_assert_equal(0, result)
             # assert that all the jobs finished successfully
             assert len(running_jobs) == 0
             self.httpserver.stop()
```

### Comparing `vdk-meta-jobs-0.1.843440573/tests/test_time_based_queue.py` & `vdk-meta-jobs-0.1.878788105/tests/test_time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.843440573/tests/test_tracking_job_executor.py` & `vdk-meta-jobs-0.1.878788105/tests/test_tracking_job_executor.py`

 * *Files identical despite different names*

