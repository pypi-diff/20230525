# Comparing `tmp/dagster-census-0.19.6.tar.gz` & `tmp/dagster-census-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-census-0.19.6.tar", last modified: Thu May 25 17:25:00 2023, max compression
+gzip compressed data, was "dagster-census-1.0.5.tar", last modified: Fri Aug 26 13:45:33 2022, max compression
```

## Comparing `dagster-census-0.19.6.tar` & `dagster-census-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:25:00.937594 dagster-census-0.19.6/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-05-25 17:16:50.000000 dagster-census-0.19.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-25 17:16:50.000000 dagster-census-0.19.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      668 2023-05-25 17:25:00.937594 dagster-census-0.19.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:25:00.933594 dagster-census-0.19.6/dagster_census/
--rw-r--r--   0 root         (0) root         (0)      394 2023-05-25 17:16:50.000000 dagster-census-0.19.6/dagster_census/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3551 2023-05-25 17:16:50.000000 dagster-census-0.19.6/dagster_census/ops.py
--rw-r--r--   0 root         (0) root         (0)    10154 2023-05-25 17:16:50.000000 dagster-census-0.19.6/dagster_census/resources.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-05-25 17:16:50.000000 dagster-census-0.19.6/dagster_census/types.py
--rw-r--r--   0 root         (0) root         (0)     1325 2023-05-25 17:16:50.000000 dagster-census-0.19.6/dagster_census/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-25 17:16:50.000000 dagster-census-0.19.6/dagster_census/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:25:00.933594 dagster-census-0.19.6/dagster_census.egg-info/
--rw-r--r--   0 root         (0) root         (0)      668 2023-05-25 17:25:00.000000 dagster-census-0.19.6/dagster_census.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-25 17:25:00.000000 dagster-census-0.19.6/dagster_census.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:25:00.000000 dagster-census-0.19.6/dagster_census.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:25:00.000000 dagster-census-0.19.6/dagster_census.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-25 17:25:00.000000 dagster-census-0.19.6/dagster_census.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-25 17:25:00.000000 dagster-census-0.19.6/dagster_census.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      161 2023-05-25 17:25:00.937594 dagster-census-0.19.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1248 2023-05-25 17:16:50.000000 dagster-census-0.19.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:33.328486 dagster-census-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)       34 2022-08-26 13:33:01.000000 dagster-census-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      622 2022-08-26 13:45:33.328486 dagster-census-1.0.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:33.328486 dagster-census-1.0.5/dagster_census/
+-rw-r--r--   0 root         (0) root         (0)      395 2022-08-26 13:33:01.000000 dagster-census-1.0.5/dagster_census/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3507 2022-08-26 13:33:01.000000 dagster-census-1.0.5/dagster_census/ops.py
+-rw-r--r--   0 root         (0) root         (0)    10046 2022-08-26 13:33:01.000000 dagster-census-1.0.5/dagster_census/resources.py
+-rw-r--r--   0 root         (0) root         (0)      667 2022-08-26 13:33:01.000000 dagster-census-1.0.5/dagster_census/types.py
+-rw-r--r--   0 root         (0) root         (0)     1294 2022-08-26 13:33:01.000000 dagster-census-1.0.5/dagster_census/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-census-1.0.5/dagster_census/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:33.328486 dagster-census-1.0.5/dagster_census.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      622 2022-08-26 13:45:33.000000 dagster-census-1.0.5/dagster_census.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      407 2022-08-26 13:45:33.000000 dagster-census-1.0.5/dagster_census.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:33.000000 dagster-census-1.0.5/dagster_census.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:33.000000 dagster-census-1.0.5/dagster_census.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       15 2022-08-26 13:45:33.000000 dagster-census-1.0.5/dagster_census.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-08-26 13:45:33.000000 dagster-census-1.0.5/dagster_census.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2022-08-26 13:45:33.328486 dagster-census-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1291 2022-08-26 13:33:01.000000 dagster-census-1.0.5/setup.py
```

### Comparing `dagster-census-0.19.6/PKG-INFO` & `dagster-census-1.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: dagster-census
-Version: 0.19.6
+Version: 1.0.5
 Summary: Package for integrating Census with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-census
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-census-0.19.6/dagster_census/ops.py` & `dagster-census-1.0.5/dagster_census/ops.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,45 +6,39 @@
 
 
 @op(
     required_resource_keys={"census"},
     ins={"start_after": In(Nothing)},
     out=Out(
         CensusOutput,
-        description=(
-            "Parsed json dictionary representing the details of the Census sync after "
-            "the sync successfully completes."
-        ),
+        description="Parsed json dictionary representing the details of the Census sync after "
+        "the sync successfully completes.",
     ),
     config_schema={
         "sync_id": Field(
             int,
             is_required=True,
-            description="Id of the parent sync.",
+            description="id of the parent sync.",
         ),
         "force_full_sync": Field(
             config=Bool,
             default_value=False,
-            description=(
-                "If this trigger request should be a Full Sync. "
-                "Note that some sync configurations such as Append do not support full syncs."
-            ),
+            description="If this trigger request should be a Full Sync. "
+            "Note that some sync configurations such as Append do not support full syncs.",
         ),
         "poll_interval": Field(
             float,
             default_value=DEFAULT_POLL_INTERVAL,
-            description="The time (in seconds) to wait between successive polls.",
+            description="The time (in seconds) that will be waited between successive polls.",
         ),
         "poll_timeout": Field(
             Noneable(float),
             default_value=None,
-            description=(
-                "The maximum time to wait before this operation is timed out. By "
-                "default, this will never time out."
-            ),
+            description="The maximum time that will waited before this operation is timed out. By "
+            "default, this will never time out.",
         ),
         "yield_materializations": Field(
             config=Bool,
             default_value=True,
             description=(
                 "If True, materializations corresponding to the results of the Census sync will "
                 "be yielded when the op executes."
@@ -58,24 +52,24 @@
                 "prefix the generated asset keys."
             ),
         ),
     },
     tags={"kind": "census"},
 )
 def census_trigger_sync_op(context):
-    """Executes a Census sync for a given ``sync_id`` and polls until that sync completes, raising
-    an error if it is unsuccessful.
-
-    It outputs a :py:class:`~dagster_census.CensusOutput` which contains the details of the Census
-    sync after it successfully completes.
+    """
+    Executes a Census sync for a given ``sync_id``, and polls until that sync
+    completes, raising an error if it is unsuccessful. It outputs a CensusOutput which contains
+    the details of the Census sync after the sync successfully completes, as well as details
+    about which tables the sync updates.
 
     It requires the use of the :py:class:`~dagster_census.census_resource`, which allows it to
-    communicate with the Census API.
+    communicate with the census API.
 
-    **Examples:**
+    Examples:
 
     .. code-block:: python
 
         from dagster import job
         from dagster_census import census_resource, census_sync_op
 
         my_census_resource = census_resource.configured(
```

### Comparing `dagster-census-0.19.6/dagster_census/resources.py` & `dagster-census-1.0.5/dagster_census/resources.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import datetime
 import json
 import logging
 import time
-from typing import Any, Mapping, Optional
+from typing import Any, Dict, Optional
 
 import requests
-from dagster import Failure, Field, StringSource, __version__, get_dagster_logger, resource
 from requests.auth import HTTPBasicAuth
 from requests.exceptions import RequestException
 
+from dagster import Failure, Field, StringSource, __version__, get_dagster_logger, resource
+
 from .types import CensusOutput
 
 CENSUS_API_BASE = "app.getcensus.com/api"
 CENSUS_VERSION = "v1"
 
 DEFAULT_POLL_INTERVAL = 10
 
 
 class CensusResource:
-    """This class exposes methods on top of the Census REST API."""
+    """
+    This class exposes methods on top of the Census REST API.
+    """
 
     def __init__(
         self,
         api_key: str,
         request_max_retries: int = 3,
         request_retry_delay: float = 0.25,
         log: logging.Logger = get_dagster_logger(),
@@ -40,105 +43,108 @@
             return self.api_key
         return "secret-token:" + self.api_key
 
     @property
     def api_base_url(self) -> str:
         return f"https://{CENSUS_API_BASE}/{CENSUS_VERSION}"
 
-    def make_request(
-        self, method: str, endpoint: str, data: Optional[str] = None
-    ) -> Mapping[str, Any]:
-        """Creates and sends a request to the desired Census API endpoint.
+    def make_request(self, method: str, endpoint: str, data: str = None) -> Dict[str, Any]:
+        """
+        Creates and sends a request to the desired Census API endpoint.
 
         Args:
             method (str): The http method to use for this request (e.g. "POST", "GET", "PATCH").
             endpoint (str): The Census API endpoint to send this request to.
             data (Optional[str]): JSON-formatted data string to be included in the request.
 
         Returns:
             Dict[str, Any]: JSON data from the response to this request
         """
-        url = f"{self.api_base_url}/{endpoint}"
         headers = {
             "User-Agent": f"dagster-census/{__version__}",
             "Content-Type": "application/json;version=2",
         }
 
         num_retries = 0
         while True:
             try:
                 response = requests.request(
                     method=method,
-                    url=url,
+                    url=f"{self.api_base_url}/{endpoint}",
                     headers=headers,
                     auth=HTTPBasicAuth("bearer", self._api_key),
                     data=data,
                 )
                 response.raise_for_status()
                 return response.json()
             except RequestException as e:
                 self._log.error("Request to Census API failed: %s", e)
                 if num_retries == self._request_max_retries:
                     break
                 num_retries += 1
                 time.sleep(self._request_retry_delay)
 
-        raise Failure(f"Max retries ({self._request_max_retries}) exceeded with url: {url}.")
+        raise Failure("Exceeded max number of retries.")
 
-    def get_sync(self, sync_id: int) -> Mapping[str, Any]:
-        """Gets details about a given sync from the Census API.
+    def get_sync(self, sync_id: int) -> Dict[str, Any]:
+        """
+        Gets details about a given sync from the Census API.
 
         Args:
             sync_id (int): The Census Sync ID.
 
         Returns:
             Dict[str, Any]: JSON data from the response to this request
         """
         return self.make_request(method="GET", endpoint=f"syncs/{sync_id}")
 
-    def get_source(self, source_id: int) -> Mapping[str, Any]:
-        """Gets details about a given source from the Census API.
+    def get_source(self, source_id: int) -> Dict[str, Any]:
+        """
+        Gets details about a given source from the Census API.
 
         Args:
             source_id (int): The Census Source ID.
 
         Returns:
             Dict[str, Any]: JSON data from the response to this request
         """
         return self.make_request(method="GET", endpoint=f"sources/{source_id}")
 
-    def get_destination(self, destination_id: int) -> Mapping[str, Any]:
-        """Gets details about a given destination from the Census API.
+    def get_destination(self, destination_id: int) -> Dict[str, Any]:
+        """
+        Gets details about a given destination from the Census API.
 
         Args:
             destination_id (int): The Census Destination ID.
 
         Returns:
             Dict[str, Any]: JSON data from the response to this request
         """
         return self.make_request(method="GET", endpoint=f"destinations/{destination_id}")
 
-    def get_sync_run(self, sync_run_id: int) -> Mapping[str, Any]:
-        """Gets details about a specific sync run from the Census API.
+    def get_sync_run(self, sync_run_id: int) -> Dict[str, Any]:
+        """
+        Gets details about a specific sync run from the Census API.
 
         Args:
             sync_run_id (int): The Census Sync Run ID.
 
         Returns:
             Dict[str, Any]: JSON data from the response to this request
         """
         return self.make_request(method="GET", endpoint=f"sync_runs/{sync_run_id}")
 
     def poll_sync_run(
         self,
         sync_run_id: int,
         poll_interval: float = DEFAULT_POLL_INTERVAL,
         poll_timeout: Optional[float] = None,
-    ) -> Mapping[str, Any]:
-        """Given a Census sync run, poll until the run is complete.
+    ) -> Dict[str, Any]:
+        """
+        Given a Census sync run, poll until the run is complete
 
         Args:
             sync_id (int): The Census Sync Run ID.
             poll_interval (float): The time (in seconds) that will be waited between successive polls.
             poll_timeout (float): The maximum time that will waited before this operation is timed
                 out. By default, this will never time out.
 
@@ -149,45 +155,44 @@
         poll_start = datetime.datetime.now()
 
         while True:
             time.sleep(poll_interval)
             response_dict = self.get_sync_run(sync_run_id)
             if "data" not in response_dict.keys():
                 raise ValueError(
-                    f"Getting status of sync failed, please visit Census Logs at {log_url} to see"
-                    " more."
+                    f"Getting status of sync failed, please visit Census Logs at {log_url} to see more."
                 )
 
             sync_id = response_dict["data"]["sync_id"]
 
-            if response_dict["data"]["status"] == "working":
+            if response_dict["status"] == "working":
                 self._log.debug(
                     f"Sync {sync_id} still running after {datetime.datetime.now() - poll_start}."
                 )
                 continue
 
             if poll_timeout and datetime.datetime.now() > poll_start + datetime.timedelta(
                 seconds=poll_timeout
             ):
                 raise Failure(
-                    f"Sync for sync '{sync_id}' timed out after"
-                    f" {datetime.datetime.now() - poll_start}."
+                    f"Sync for sync '{sync_id}' timed out after {datetime.datetime.now() - poll_start}."
                 )
 
             break
 
         self._log.debug(
             f"Sync {sync_id} has finished running after {datetime.datetime.now() - poll_start}."
         )
         self._log.info(f"View sync details here: {log_url}.")
 
         return response_dict
 
-    def trigger_sync(self, sync_id: int, force_full_sync: bool = False) -> Mapping[str, Any]:
-        """Trigger an asynchronous run for a specific sync.
+    def trigger_sync(self, sync_id: int, force_full_sync: bool = False) -> Dict[str, Any]:
+        """
+        Trigger an asynchronous run for a specific sync.
 
         Args:
             sync_id (int): The Census Sync Run ID.
             force_full_sync (bool): If the Sync should perform a full sync
 
         Returns:
             Dict[str, Any]: JSON data from the response to this request
@@ -200,15 +205,16 @@
     def trigger_sync_and_poll(
         self,
         sync_id: int,
         force_full_sync: bool = False,
         poll_interval: float = DEFAULT_POLL_INTERVAL,
         poll_timeout: Optional[float] = None,
     ) -> CensusOutput:
-        """Trigger a run for a specific sync and poll until it has completed.
+        """
+        Trigger a run for a specific sync and poll until it has completed
 
         Args:
             sync_id (int): The Census Sync Run ID.
             force_full_sync (bool): If the Sync should perform a full sync
             poll_interval (float): The time (in seconds) that will be waited between successive polls.
             poll_timeout (float): The maximum time that will waited before this operation is timed
                 out. By default, this will never time out.
@@ -244,29 +250,28 @@
             StringSource,
             is_required=True,
             description="Census API Key.",
         ),
         "request_max_retries": Field(
             int,
             default_value=3,
-            description=(
-                "The maximum number of times requests to the Census API should be retried "
-                "before failing."
-            ),
+            description="The maximum number of times requests to the Census API should be retried "
+            "before failing.",
         ),
         "request_retry_delay": Field(
             float,
             default_value=0.25,
             description="Time (in seconds) to wait between each request retry.",
         ),
     },
     description="This resource helps manage Census connectors",
 )
 def census_resource(context) -> CensusResource:
-    """This resource allows users to programatically interface with the Census REST API to launch
+    """
+    This resource allows users to programatically interface with the Census REST API to launch
     syncs and monitor their progress. This currently implements only a subset of the functionality
     exposed by the API.
 
     **Examples:**
 
     .. code-block:: python
```

### Comparing `dagster-census-0.19.6/dagster_census/utils.py` & `dagster-census-1.0.5/dagster_census/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from typing import Sequence
+from typing import List
 
 from dagster import AssetMaterialization
 
 from .types import CensusOutput
 
 
 def generate_materialization(
-    census_output: CensusOutput, asset_key_prefix: Sequence[str]
+    census_output: CensusOutput, asset_key_prefix: List[str]
 ) -> AssetMaterialization:
+
     sync_id = census_output.sync_run["sync_id"]
     source_name = census_output.source["name"]
     destination_name = census_output.destination["name"]
 
     metadata = {
         "sync_id": sync_id,
         "sync_run_id": census_output.sync_run["id"],
@@ -22,16 +23,14 @@
         "records_processed": census_output.sync_run["records_processed"],
         "records_updated": census_output.sync_run["records_updated"],
         "records_failed": census_output.sync_run["records_failed"],
         "records_invalid": census_output.sync_run["records_invalid"],
         "full_sync": census_output.sync_run["full_sync"],
     }
 
-    asset_key_name = [*asset_key_prefix, f"sync_{sync_id}"]
+    asset_key_name = asset_key_prefix + [f"sync_{sync_id}"]
 
     return AssetMaterialization(
         asset_key=asset_key_name,
-        description=(
-            f"Sync generated for Census sync {sync_id}: {source_name} to {destination_name}"
-        ),
+        description=f"Sync generated for Census sync {sync_id}: {source_name} to {destination_name}",
         metadata=metadata,
     )
```

### Comparing `dagster-census-0.19.6/dagster_census.egg-info/PKG-INFO` & `dagster-census-1.0.5/dagster_census.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: dagster-census
-Version: 0.19.6
+Version: 1.0.5
 Summary: Package for integrating Census with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-census
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-census-0.19.6/setup.py` & `dagster-census-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-from pathlib import Path
 from typing import Dict
 
 from setuptools import find_packages, setup
 
 
 def get_version() -> str:
     version: Dict[str, str] = {}
-    with open(Path(__file__).parent / "dagster_census/version.py", encoding="utf8") as fp:
-        exec(fp.read(), version)
+    with open("dagster_census/version.py", encoding="utf8") as fp:
+        exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
-ver = get_version()
-# dont pin dev installs to avoid pip dep resolver issues
-pin = "" if ver == "1!0+dev" else f"=={ver}"
-setup(
-    name="dagster-census",
-    version=ver,
-    author="Elementl",
-    author_email="hello@elementl.com",
-    license="Apache-2.0",
-    description="Package for integrating Census with Dagster.",
-    url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-census",
-    classifiers=[
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: OS Independent",
-    ],
-    packages=find_packages(exclude=["dagster_census_tests*"]),
-    install_requires=["dagster==1.3.6"],
-    zip_safe=False,
-)
+if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
+    setup(
+        name="dagster-census",
+        version=ver,
+        author="Elementl",
+        author_email="hello@elementl.com",
+        license="Apache-2.0",
+        description="Package for integrating Census with Dagster.",
+        url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-census",
+        classifiers=[
+            "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "License :: OSI Approved :: Apache Software License",
+            "Operating System :: OS Independent",
+        ],
+        packages=find_packages(exclude=["dagster_census_tests*"]),
+        install_requires=["dagster==1.0.5"],
+        zip_safe=False,
+    )
```

