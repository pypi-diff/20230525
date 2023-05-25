# Comparing `tmp/dagster-msteams-0.19.6.tar.gz` & `tmp/dagster-msteams-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-msteams-0.19.6.tar", last modified: Thu May 25 17:27:00 2023, max compression
+gzip compressed data, was "dagster-msteams-1.0.5.tar", last modified: Fri Aug 26 13:46:46 2022, max compression
```

## Comparing `dagster-msteams-0.19.6.tar` & `dagster-msteams-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:27:00.518179 dagster-msteams-0.19.6/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-05-25 17:16:50.000000 dagster-msteams-0.19.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       66 2023-05-25 17:16:50.000000 dagster-msteams-0.19.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      690 2023-05-25 17:27:00.518179 dagster-msteams-0.19.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-05-25 17:16:50.000000 dagster-msteams-0.19.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:27:00.514179 dagster-msteams-0.19.6/dagster_msteams/
--rw-r--r--   0 root         (0) root         (0)      510 2023-05-25 17:16:50.000000 dagster-msteams-0.19.6/dagster_msteams/__init__.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-05-25 17:16:50.000000 dagster-msteams-0.19.6/dagster_msteams/card.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-05-25 17:16:50.000000 dagster-msteams-0.19.6/dagster_msteams/client.py
--rw-r--r--   0 root         (0) root         (0)     3899 2023-05-25 17:16:50.000000 dagster-msteams-0.19.6/dagster_msteams/hooks.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-25 17:16:50.000000 dagster-msteams-0.19.6/dagster_msteams/py.typed
--rw-r--r--   0 root         (0) root         (0)     3553 2023-05-25 17:16:50.000000 dagster-msteams-0.19.6/dagster_msteams/resources.py
--rw-r--r--   0 root         (0) root         (0)     5222 2023-05-25 17:16:50.000000 dagster-msteams-0.19.6/dagster_msteams/sensors.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-25 17:16:50.000000 dagster-msteams-0.19.6/dagster_msteams/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:27:00.518179 dagster-msteams-0.19.6/dagster_msteams.egg-info/
--rw-r--r--   0 root         (0) root         (0)      690 2023-05-25 17:27:00.000000 dagster-msteams-0.19.6/dagster_msteams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      491 2023-05-25 17:27:00.000000 dagster-msteams-0.19.6/dagster_msteams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:27:00.000000 dagster-msteams-0.19.6/dagster_msteams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:27:00.000000 dagster-msteams-0.19.6/dagster_msteams.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-25 17:27:00.000000 dagster-msteams-0.19.6/dagster_msteams.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-25 17:27:00.000000 dagster-msteams-0.19.6/dagster_msteams.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2023-05-25 17:27:00.518179 dagster-msteams-0.19.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1163 2023-05-25 17:16:50.000000 dagster-msteams-0.19.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:46.868890 dagster-msteams-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11356 2022-08-26 13:33:01.000000 dagster-msteams-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2022-08-26 13:33:01.000000 dagster-msteams-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      666 2022-08-26 13:46:46.868890 dagster-msteams-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2022-08-26 13:33:01.000000 dagster-msteams-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:46.868890 dagster-msteams-1.0.5/dagster_msteams/
+-rw-r--r--   0 root         (0) root         (0)      362 2022-08-26 13:33:01.000000 dagster-msteams-1.0.5/dagster_msteams/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      847 2022-08-26 13:33:01.000000 dagster-msteams-1.0.5/dagster_msteams/card.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2022-08-26 13:33:01.000000 dagster-msteams-1.0.5/dagster_msteams/client.py
+-rw-r--r--   0 root         (0) root         (0)     3931 2022-08-26 13:33:01.000000 dagster-msteams-1.0.5/dagster_msteams/hooks.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-msteams-1.0.5/dagster_msteams/py.typed
+-rw-r--r--   0 root         (0) root         (0)     2185 2022-08-26 13:33:01.000000 dagster-msteams-1.0.5/dagster_msteams/resources.py
+-rw-r--r--   0 root         (0) root         (0)     4842 2022-08-26 13:33:01.000000 dagster-msteams-1.0.5/dagster_msteams/sensors.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-msteams-1.0.5/dagster_msteams/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:46.868890 dagster-msteams-1.0.5/dagster_msteams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      666 2022-08-26 13:46:46.000000 dagster-msteams-1.0.5/dagster_msteams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      491 2022-08-26 13:46:46.000000 dagster-msteams-1.0.5/dagster_msteams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:46.000000 dagster-msteams-1.0.5/dagster_msteams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:46.000000 dagster-msteams-1.0.5/dagster_msteams.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       23 2022-08-26 13:46:46.000000 dagster-msteams-1.0.5/dagster_msteams.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2022-08-26 13:46:46.000000 dagster-msteams-1.0.5/dagster_msteams.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2022-08-26 13:46:46.872890 dagster-msteams-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1191 2022-08-26 13:33:01.000000 dagster-msteams-1.0.5/setup.py
```

### Comparing `dagster-msteams-0.19.6/LICENSE` & `dagster-msteams-1.0.5/LICENSE`

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

### Comparing `dagster-msteams-0.19.6/PKG-INFO` & `dagster-msteams-1.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: dagster-msteams
-Version: 0.19.6
+Version: 1.0.5
 Summary: A Microsoft Teams client resource for posting to Microsoft Teams
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-msteams
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
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-msteams-0.19.6/dagster_msteams/card.py` & `dagster-msteams-1.0.5/dagster_msteams/card.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Mapping
+from typing import Dict
 
 
 class Card:
     """Class to contruct a MS Teams Hero card for posting dagster messages."""
 
     def __init__(self):
         self.payload = {"type": "message", "attachments": []}
@@ -11,18 +11,18 @@
     def type(self):
         return self.payload["type"]
 
     @property
     def attachments(self):
         return self.payload["attachments"]
 
-    def _create_attachment(self, text_message: str) -> Mapping:
+    def _create_attachment(self, text_message: str) -> Dict:
         content = {
             "title": "Dagster Pipeline Alert",
-            "text": text_message,
+            "subtitle": text_message,
         }
         content_type = "application/vnd.microsoft.card.hero"
         return {"contentType": content_type, "content": content}
 
     def add_attachment(self, text_message: str):
         hero_card_attachment = self._create_attachment(text_message)
         self.payload["attachments"].append(hero_card_attachment)
```

### Comparing `dagster-msteams-0.19.6/dagster_msteams/client.py` & `dagster-msteams-1.0.5/dagster_msteams/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from typing import Mapping, Optional
+from typing import Dict, Optional
 
 from requests import codes, exceptions, post
 
 
 class TeamsClient:
     """MS Teams web client responsible for connecting to a channel using the webhook URL
-    and posting informaton in the form of cards.
-    """
+    and posting informaton in the form of cards."""
 
     def __init__(
         self,
         hook_url: str,
         http_proxy: Optional[str] = None,
         https_proxy: Optional[str] = None,
         timeout: Optional[float] = 60,
@@ -25,20 +24,20 @@
             self._proxy = {}
             if http_proxy:
                 self._proxy["http"] = http_proxy
             if https_proxy:
                 self._proxy["https"] = https_proxy
         self._headers = {"Content-Type": "application/json"}
 
-    def post_message(self, payload: Mapping) -> bool:  # pragma: no cover
+    def post_message(self, payload: Dict) -> bool:  # pragma: no cover
         response = post(
             self._hook_url,
             json=payload,
             headers=self._headers,
             proxies=self._proxy,
             timeout=self._timeout,
             verify=self._verify,
         )
-        if response.status_code == codes["ok"] and response.text == "1":
+        if response.status_code == codes.ok and response.text == "1":  # pylint: disable=no-member
             return True
         else:
             raise exceptions.RequestException(response.text)
```

### Comparing `dagster-msteams-0.19.6/dagster_msteams/hooks.py` & `dagster-msteams-1.0.5/dagster_msteams/hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Callable, Optional
 
+from dagster_msteams.card import Card
+
 from dagster._core.definitions import failure_hook, success_hook
 from dagster._core.execution.context.hook import HookContext
 
-from dagster_msteams.card import Card
-
 
 def _default_status_message(context: HookContext, status: str) -> str:
     return f"Op {context.op.name} on job {context.job_name} {status}!\nRun ID: {context.run_id}"
 
 
 def _default_failure_message(context: HookContext) -> str:
     return _default_status_message(context, status="failed")
@@ -60,15 +60,15 @@
         if dagit_base_url:
             text += "<a href='{base_url}/instance/runs/{run_id}'>View in Dagit</a>".format(
                 base_url=dagit_base_url,
                 run_id=context.run_id,
             )
         card = Card()
         card.add_attachment(text_message=text)
-        context.resources.msteams.post_message(payload=card.payload)
+        context.resources.msteams.post_message(payload=card.payload)  # type: ignore
 
     return _hook
 
 
 def teams_on_success(
     message_fn: Callable[[HookContext], str] = _default_success_message,
     dagit_base_url: Optional[str] = None,
@@ -111,10 +111,10 @@
         if dagit_base_url:
             text += "<a href='{base_url}/instance/runs/{run_id}'>View in Dagit</a>".format(
                 base_url=dagit_base_url,
                 run_id=context.run_id,
             )
         card = Card()
         card.add_attachment(text_message=text)
-        context.resources.msteams.post_message(payload=card.payload)
+        context.resources.msteams.post_message(payload=card.payload)  # type: ignore
 
     return _hook
```

### Comparing `dagster-msteams-0.19.6/dagster_msteams/sensors.py` & `dagster-msteams-1.0.5/dagster_msteams/sensors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import TYPE_CHECKING, Callable, Optional, Sequence, Union
+from typing import TYPE_CHECKING, Callable, List, Optional, Union
+
+from dagster_msteams.card import Card
+from dagster_msteams.client import TeamsClient
 
 from dagster import DefaultSensorStatus
-from dagster._core.definitions import GraphDefinition, JobDefinition
+from dagster._core.definitions import GraphDefinition, PipelineDefinition
 from dagster._core.definitions.run_status_sensor_definition import (
     RunFailureSensorContext,
     run_failure_sensor,
 )
 from dagster._core.definitions.unresolved_asset_job_definition import UnresolvedAssetJobDefinition
 
-from dagster_msteams.card import Card
-from dagster_msteams.client import TeamsClient
-
 if TYPE_CHECKING:
-    from dagster._core.definitions.selector import JobSelector, RepositorySelector
+    from dagster._core.host_representation.selector import JobSelector, RepositorySelector
 
 
 def _default_failure_message(context: RunFailureSensorContext) -> str:
     return "\n".join(
         [
             f"Job {context.dagster_run.job_name} failed!",
             f"Run ID: {context.dagster_run.run_id}",
@@ -32,25 +32,24 @@
     https_proxy: Optional[str] = None,
     timeout: Optional[float] = 60,
     verify: Optional[bool] = None,
     name: Optional[str] = None,
     dagit_base_url: Optional[str] = None,
     default_status: DefaultSensorStatus = DefaultSensorStatus.STOPPED,
     monitored_jobs: Optional[
-        Sequence[
+        List[
             Union[
-                JobDefinition,
+                PipelineDefinition,
                 GraphDefinition,
                 UnresolvedAssetJobDefinition,
                 "RepositorySelector",
                 "JobSelector",
             ]
         ]
     ] = None,
-    monitor_all_repositories: bool = False,
 ):
     """Create a sensor on run failures that will message the given MS Teams webhook URL.
 
     Args:
         hook_url (str): MS Teams incoming webhook URL.
         message_fn (Optional(Callable[[RunFailureSensorContext], str])): Function which
             takes in the ``RunFailureSensorContext`` and outputs the message you want to send.
@@ -60,23 +59,20 @@
         timeout: (Optional[float]): Connection timeout in seconds. Defaults to 60.
         verify: (Optional[bool]): Whether to verify the servers TLS certificate.
         name: (Optional[str]): The name of the sensor. Defaults to "teams_on_run_failure".
         dagit_base_url: (Optional[str]): The base url of your Dagit instance. Specify this to allow
             messages to include deeplinks to the failed run.
         default_status (DefaultSensorStatus): Whether the sensor starts as running or not. The default
             status can be overridden from Dagit or via the GraphQL API.
-        monitored_jobs (Optional[List[Union[JobDefinition, GraphDefinition, UnresolvedAssetJobDefinition, RepositorySelector, JobSelector]]]):
-            Jobs in the current repository that will be monitored by this sensor. Defaults to None,
-            which means the alert will be sent when any job in the repository matches the requested
-            run_status. To monitor jobs in external repositories, use RepositorySelector and JobSelector.
-        monitor_all_repositories (bool): If set to True, the sensor will monitor all runs in the
-            Dagster instance. If set to True, an error will be raised if you also specify
-            monitored_jobs or job_selection. Defaults to False.
+        monitored_jobs (Optional[List[Union[PipelineDefinition, GraphDefinition, UnresolvedAssetJobDefinition, RepositorySelector, JobSelector]]]):
+            Jobs in the current repository that will be monitored by this sensor. Defaults to None, which means the alert will
+            be sent when any job in the repository matches the requested run_status. To monitor jobs in external repositories, use RepositorySelector and JobSelector
 
     Examples:
+
         .. code-block:: python
 
             teams_on_run_failure = make_teams_on_run_failure_sensor(
                 hook_url=os.getenv("TEAMS_WEBHOOK_URL")
             )
 
             @repository
@@ -95,29 +91,26 @@
                 hook_url=os.getenv("TEAMS_WEBHOOK_URL"),
                 message_fn=my_message_fn,
                 dagit_base_url="http://localhost:3000",
             )
 
 
     """
+
     teams_client = TeamsClient(
         hook_url=hook_url,
         http_proxy=http_proxy,
         https_proxy=https_proxy,
         timeout=timeout,
         verify=verify,
     )
 
-    @run_failure_sensor(
-        name=name,
-        default_status=default_status,
-        monitored_jobs=monitored_jobs,
-        monitor_all_repositories=monitor_all_repositories,
-    )
+    @run_failure_sensor(name=name, default_status=default_status, monitored_jobs=monitored_jobs)
     def teams_on_run_failure(context: RunFailureSensorContext):
+
         text = message_fn(context)
         if dagit_base_url:
             text += "<a href='{base_url}/instance/runs/{run_id}'>View in Dagit</a>".format(
                 base_url=dagit_base_url,
                 run_id=context.dagster_run.run_id,
             )
         card = Card()
```

### Comparing `dagster-msteams-0.19.6/dagster_msteams.egg-info/PKG-INFO` & `dagster-msteams-1.0.5/dagster_msteams.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: dagster-msteams
-Version: 0.19.6
+Version: 1.0.5
 Summary: A Microsoft Teams client resource for posting to Microsoft Teams
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-msteams
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
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-msteams-0.19.6/setup.py` & `dagster-msteams-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-from pathlib import Path
-
 from setuptools import find_packages, setup
 
 
 def get_version():
     version = {}
-    with open(Path(__file__).parent / "dagster_msteams/version.py", encoding="utf8") as fp:
-        exec(fp.read(), version)
+    with open("dagster_msteams/version.py", encoding="utf8") as fp:
+        exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
-setup(
-    name="dagster-msteams",
-    version=get_version(),
-    author="Elementl",
-    author_email="hello@elementl.com",
-    license="Apache-2.0",
-    description="A Microsoft Teams client resource for posting to Microsoft Teams",
-    url=(
-        "https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-msteams"
-    ),
-    classifiers=[
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: OS Independent",
-    ],
-    packages=find_packages(exclude=["dagster_msteams_tests*"]),
-    install_requires=[
-        "dagster",
-        "requests>=2,<3",
-    ],
-    zip_safe=False,
-)
+if __name__ == "__main__":
+    setup(
+        name="dagster-msteams",
+        version=get_version(),
+        author="Elementl",
+        author_email="hello@elementl.com",
+        license="Apache-2.0",
+        description="A Microsoft Teams client resource for posting to Microsoft Teams",
+        url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-msteams",
+        classifiers=[
+            "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "License :: OSI Approved :: Apache Software License",
+            "Operating System :: OS Independent",
+        ],
+        packages=find_packages(exclude=["dagster_msteams_tests*"]),
+        install_requires=[
+            "dagster",
+            "requests>=2,<3",
+        ],
+        zip_safe=False,
+    )
```

