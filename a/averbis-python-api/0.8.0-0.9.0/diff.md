# Comparing `tmp/averbis-python-api-0.8.0.tar.gz` & `tmp/averbis-python-api-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "averbis-python-api-0.8.0.tar", last modified: Thu Apr 28 10:12:28 2022, max compression
+gzip compressed data, was "averbis-python-api-0.9.0.tar", last modified: Thu Jun 23 13:21:54 2022, max compression
```

## Comparing `averbis-python-api-0.8.0.tar` & `averbis-python-api-0.9.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 10:12:28.531380 averbis-python-api-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-04-28 10:12:16.000000 averbis-python-api-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9054 2022-04-28 10:12:28.531380 averbis-python-api-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8216 2022-04-28 10:12:16.000000 averbis-python-api-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 10:12:28.527380 averbis-python-api-0.8.0/averbis/
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-04-28 10:12:16.000000 averbis-python-api-0.8.0/averbis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-04-28 10:12:16.000000 averbis-python-api-0.8.0/averbis/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 10:12:28.527380 averbis-python-api-0.8.0/averbis/core/
--rw-r--r--   0 runner    (1001) docker     (121)     2278 2022-04-28 10:12:16.000000 averbis-python-api-0.8.0/averbis/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   109348 2022-04-28 10:12:16.000000 averbis-python-api-0.8.0/averbis/core/_rest_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 10:12:28.527380 averbis-python-api-0.8.0/averbis/highlighting/
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-04-28 10:12:16.000000 averbis-python-api-0.8.0/averbis/highlighting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7155 2022-04-28 10:12:16.000000 averbis-python-api-0.8.0/averbis/highlighting/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 10:12:28.527380 averbis-python-api-0.8.0/averbis_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9054 2022-04-28 10:12:28.000000 averbis-python-api-0.8.0/averbis_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-04-28 10:12:28.000000 averbis-python-api-0.8.0/averbis_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-28 10:12:28.000000 averbis-python-api-0.8.0/averbis_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-04-28 10:12:28.000000 averbis-python-api-0.8.0/averbis_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-04-28 10:12:28.000000 averbis-python-api-0.8.0/averbis_python_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-28 10:12:28.531380 averbis-python-api-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3554 2022-04-28 10:12:16.000000 averbis-python-api-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 10:12:28.531380 averbis-python-api-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-04-28 10:12:16.000000 averbis-python-api-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3570 2022-04-28 10:12:16.000000 averbis-python-api-0.8.0/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)    34936 2022-04-28 10:12:16.000000 averbis-python-api-0.8.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     9114 2022-04-28 10:12:16.000000 averbis-python-api-0.8.0/tests/test_document_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-04-28 10:12:16.000000 averbis-python-api-0.8.0/tests/test_highlighting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1406 2022-04-28 10:12:16.000000 averbis-python-api-0.8.0/tests/test_pear.py
--rw-r--r--   0 runner    (1001) docker     (121)    17809 2022-04-28 10:12:16.000000 averbis-python-api-0.8.0/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)    17574 2022-04-28 10:12:16.000000 averbis-python-api-0.8.0/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (121)    14103 2022-04-28 10:12:16.000000 averbis-python-api-0.8.0/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-04-28 10:12:16.000000 averbis-python-api-0.8.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 13:21:54.787974 averbis-python-api-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-06-23 13:21:46.000000 averbis-python-api-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     9054 2022-06-23 13:21:54.787974 averbis-python-api-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8216 2022-06-23 13:21:46.000000 averbis-python-api-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 13:21:54.787974 averbis-python-api-0.9.0/averbis/
+-rw-r--r--   0 runner    (1001) docker     (121)      988 2022-06-23 13:21:46.000000 averbis-python-api-0.9.0/averbis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      702 2022-06-23 13:21:46.000000 averbis-python-api-0.9.0/averbis/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 13:21:54.787974 averbis-python-api-0.9.0/averbis/core/
+-rw-r--r--   0 runner    (1001) docker     (121)     2338 2022-06-23 13:21:46.000000 averbis-python-api-0.9.0/averbis/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   117346 2022-06-23 13:21:46.000000 averbis-python-api-0.9.0/averbis/core/_rest_client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 13:21:54.787974 averbis-python-api-0.9.0/averbis/highlighting/
+-rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-06-23 13:21:46.000000 averbis-python-api-0.9.0/averbis/highlighting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7155 2022-06-23 13:21:46.000000 averbis-python-api-0.9.0/averbis/highlighting/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 13:21:54.787974 averbis-python-api-0.9.0/averbis_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9054 2022-06-23 13:21:54.000000 averbis-python-api-0.9.0/averbis_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      616 2022-06-23 13:21:54.000000 averbis-python-api-0.9.0/averbis_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-23 13:21:54.000000 averbis-python-api-0.9.0/averbis_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-06-23 13:21:54.000000 averbis-python-api-0.9.0/averbis_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-23 13:21:54.000000 averbis-python-api-0.9.0/averbis_python_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-23 13:21:54.787974 averbis-python-api-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3554 2022-06-23 13:21:46.000000 averbis-python-api-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 13:21:54.787974 averbis-python-api-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2022-06-23 13:21:46.000000 averbis-python-api-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4012 2022-06-23 13:21:46.000000 averbis-python-api-0.9.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35221 2022-06-23 13:21:46.000000 averbis-python-api-0.9.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9114 2022-06-23 13:21:46.000000 averbis-python-api-0.9.0/tests/test_document_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-06-23 13:21:46.000000 averbis-python-api-0.9.0/tests/test_highlighting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1406 2022-06-23 13:21:46.000000 averbis-python-api-0.9.0/tests/test_pear.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17809 2022-06-23 13:21:46.000000 averbis-python-api-0.9.0/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20214 2022-06-23 13:21:46.000000 averbis-python-api-0.9.0/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14103 2022-06-23 13:21:46.000000 averbis-python-api-0.9.0/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-06-23 13:21:46.000000 averbis-python-api-0.9.0/tests/utils.py
```

### Comparing `averbis-python-api-0.8.0/LICENSE` & `averbis-python-api-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `averbis-python-api-0.8.0/PKG-INFO` & `averbis-python-api-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: averbis-python-api
-Version: 0.8.0
+Version: 0.9.0
 Summary: Averbis REST API client for Python.
 Home-page: UNKNOWN
 Author: Averbis GmbH
 License: Apache License, Version 2.0. Copyright Averbis GmbH
 Project-URL: Bug Tracker, https://github.com/averbis/averbis-python-api/issues
 Project-URL: Source Code, https://github.com/averbis/averbis-python-api
 Platform: UNKNOWN
```

### Comparing `averbis-python-api-0.8.0/README.rst` & `averbis-python-api-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `averbis-python-api-0.8.0/averbis/__init__.py` & `averbis-python-api-0.9.0/averbis/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2021 Averbis GmbH.
+# Copyright (c) 2022 Averbis GmbH.
 #
 # This file is part of Averbis Python API.
 # See https://www.averbis.com for further info.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
@@ -13,19 +13,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #
-from .core import Client, Project, Pipeline, Result, Terminology, DocumentCollection, Pear, Process
+from .core import Client, Project, Pipeline, Result, Terminology, DocumentCollection, Pear, Process, \
+    EvaluationConfiguration
 
 __all__ = [
     "Client",
     "Project",
     "Pipeline",
     "Result",
     "Terminology",
+    "EvaluationConfiguration",
     "DocumentCollection",
     "Pear",
     "Process",
 ]
```

### Comparing `averbis-python-api-0.8.0/averbis/__version__.py` & `averbis-python-api-0.9.0/averbis/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #
-__version__ = "0.8.0"
+__version__ = "0.9.0"
```

### Comparing `averbis-python-api-0.8.0/averbis/core/__init__.py` & `averbis-python-api-0.9.0/averbis/core/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     Client,
     Result,
     Pipeline,
     Project,
     DocumentCollection,
     Pear,
     Process,
+    EvaluationConfiguration,
     DOCUMENT_IMPORTER_CAS,
     DOCUMENT_IMPORTER_SOLR,
     DOCUMENT_IMPORTER_TEXT,
     HEADER_CONTENT_TYPE,
     HEADER_ACCEPT,
     MEDIA_TYPE_ANY,
     MEDIA_TYPE_APPLICATION_JSON,
@@ -58,14 +59,15 @@
     "Client",
     "Result",
     "Pipeline",
     "Project",
     "DocumentCollection",
     "Pear",
     "Process",
+    "EvaluationConfiguration",
     "DOCUMENT_IMPORTER_CAS",
     "DOCUMENT_IMPORTER_SOLR",
     "DOCUMENT_IMPORTER_TEXT",
     "HEADER_CONTENT_TYPE",
     "HEADER_ACCEPT",
     "MEDIA_TYPE_ANY",
     "MEDIA_TYPE_APPLICATION_JSON",
```

### Comparing `averbis-python-api-0.8.0/averbis/core/_rest_client.py` & `averbis-python-api-0.9.0/averbis/core/_rest_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -830,14 +830,38 @@
             pipeline=pipeline,
             preceding_process_name=self.name,
         )
 
         return document_collection.get_process(process_name=process_name)
 
     @experimental_api
+    def evaluate_against(
+        self,
+        reference_process: "Process",
+        process_name: str,
+        evaluation_configurations: List["EvaluationConfiguration"],
+        number_of_pipeline_instances: int = 1,
+    ) -> "Process":
+        """
+        HIGHLY EXPERIMENTAL API - may soon change or disappear.
+
+        Starts the evaluation of this process in comparison to the given one as a new process.
+        Returns the new evaluation process.
+        """
+        # noinspection PyProtectedMember
+        return self.project.client._evaluate(
+            self.project,
+            self,
+            reference_process,
+            process_name,
+            evaluation_configurations,
+            number_of_pipeline_instances,
+        )
+
+    @experimental_api
     def rerun(self):
         """
         HIGHLY EXPERIMENTAL API - may soon change or disappear.
 
         Triggers a rerun if the process is IDLE.
         All current results will be deleted and the documents will be reprocessed.
         """
@@ -902,14 +926,15 @@
         Returns an analysis as a UIMA CAS.
         """
         if self.project.client.get_build_info()["specVersion"].startswith("5."):
             raise OperationNotSupported(
                 "Text analysis export is not supported for platform version 5.x, it is only supported from 6.x onwards."
             )
         document_collection = self.project.get_document_collection(self.document_source_name)
+        # noinspection PyProtectedMember
         document_identifier = document_collection._get_document_identifier(document_name)
         # noinspection PyProtectedMember
         type_system = load_typesystem(
             self.project.client._export_analysis_result_typesystem(
                 self.project.name, self.document_source_name, document_identifier, self
             )
         )
@@ -1400,24 +1425,100 @@
         """
         # noinspection PyProtectedMember
         zip_file = self.client._create_zip_io(source, path_in_zip)
         # noinspection PyProtectedMember
         return self.client._upload_resources(zip_file, project_name=self.name)["files"]
 
 
+class EvaluationConfiguration:
+    def __init__(
+        self,
+        comparison_annotation_type_name: str,
+        features_to_compare: List[str],
+        reference_annotation_type_name: str = None,
+    ):
+        """
+        Configuration for the evaluation of one annotation type
+
+        :param comparison_annotation_type_name:   fully qualified name of the annotation that will be compared;
+            can also be a rule of format fully_qualified_name[feature1=value1&amp;&amp;feature2=value2...]
+            can be extended by another rule of the same type, meaning that an annotation must be contained, e.g:
+            fully_qualified_name[feature1=value1&amp;&amp;feature2=value2...] >
+            fully_qualified_name[feature1=value1&amp;&amp;feature2=value2...]
+        :param reference_annotation_type_name:   fully qualified name of the annotation in the reference text analysis
+            result that other annotations should be compared to; can also be a rule (see annotation_type_name above).
+            If not given, the same annotation as the comparison annotation is used
+        :param features_to_compare:   The list of features that should be used in the comparison, e.g., begin, end,
+            uniqueID.
+        """
+        self.partialMatchCriteria: Union[str, None] = None
+        self.partialMatchArguments: List[str] = []
+        # Features to be excluded from deep feature structure comparisons. These are regular
+        # expressions which match against the fully qualified feature name (type:feature).
+        self.excludeFeaturePatterns: List[str] = []
+        # Regular expression specifying character sequences that should be ignored when
+        # values of string features are compared
+        self.stringFeatureComparisonIgnorePattern = None
+        self.compareAnnotationRule = comparison_annotation_type_name
+        if reference_annotation_type_name:
+            self.goldAnnotationRule = reference_annotation_type_name
+        if reference_annotation_type_name is None:
+            self.goldAnnotationRule = comparison_annotation_type_name
+        self.featuresToBeCompared = features_to_compare
+        self.allowMultipleMatches = False
+        self.stringFeatureComparisonIgnoreCase = False
+        self.forceComparisonWhenGoldstandardMissing = False
+
+    def add_feature(self, feature_name: str) -> "EvaluationConfiguration":
+        self.featuresToBeCompared.append(feature_name)
+        return self
+
+    def use_overlap_partial_match(self) -> "EvaluationConfiguration":
+        """
+        Overlapping annotations are used to calculate partial positives.  Normally, these will replace a FalsePositive
+        or FalseNegative if a partial match is identified.
+        """
+        self.partialMatchCriteria = "OVERLAP_MATCH"
+        return self
+
+    def use_range_variance_partial_match(
+        self, range_variance: int
+    ) -> "EvaluationConfiguration":
+        """
+        Annotations that are offset by the given variance are used to calculate partial positives.
+        Normally, these will replace a FalsePositive or FalseNegative if a partial match is identified.
+        """
+        self.partialMatchCriteria = "RANGE_VARIANCE_MATCH"
+        self.partialMatchArguments = [str(range_variance)]
+        return self
+
+    def use_enclosing_annotation_partial_match(
+        self, enclosing_annotation_type_name: str
+    ) -> "EvaluationConfiguration":
+        """
+        Annotations that are covered by the given annotation type are used to calculate partial positives.
+        Normally, these will replace a FalsePositive or FalseNegative if a partial match is identified.
+        """
+        self.partialMatchCriteria = "ENCLOSING_ANNOTATION_MATCH"
+        self.partialMatchArguments = [enclosing_annotation_type_name]
+        return self
+
+
 class Client:
     def __init__(
         self,
         url_or_id: str,
         api_token: str = None,
         verify_ssl: Union[str, bool] = True,
         settings: Union[str, Path, dict] = None,
         username: str = None,
         password: str = None,
         timeout: float = None,
+        polling_timeout: int = 30,
+        poll_delay: int = 5,
     ):
         """
         A Client is the base object for all calls within the Averbis Python API.
 
         The Client can be initialized by passing the required parameters (e.g. URL and API Token) or
         by creating a client-settings.json file in which the information is stored.
         The client-settings.json allows specifying different profiles for different servers.
@@ -1427,16 +1528,21 @@
         :param api_token:  The API Token enabling users to perform requests in the platform
         :param verify_ssl: Whether the SSL verifcation should be activated (default=True)
         :param settings:   Either a dictionary containing settings information or a path to the settings file.
                            As fallback, a "client-settings.json" file is searched in the current directory and in $HOME/.averbis/
         :param username:   If no API token is provided, then a username can be provided together with a password to generate a new API token
         :param password:   If no API token is provided, then a username can be provided together with a password to generate a new API token
         :param timeout:    An optional global timeout (in seconds) specifiying how long the Client is waiting for a server response (default=None).
+
+        :param polling_timeout: Timeout (in seconds) after which polling for specific status requests is no longer tried.
+        :param poll_delay: Time (in seconds) between requests to server for specific status.
         """
 
+        self._polling_timeout = polling_timeout
+        self._poll_delay = poll_delay
         self.__logger = logging.getLogger(self.__class__.__module__ + "." + self.__class__.__name__)
         self._api_token = api_token
         self._verify_ssl = verify_ssl
         self._timeout = timeout
 
         if isinstance(settings, dict):
             self._settings = settings
@@ -1719,24 +1825,40 @@
                  representation.
         """
         if not self._build_info:
             response = self.__request_with_json_response("get", f"/v1/buildInfo")
             self._build_info = response["payload"]
         return self._build_info
 
-    def create_project(self, name: str, description: str = "") -> Project:
+    def create_project(self, name: str, description: str = "", exist_ok=False) -> Project:
         """
         Creates a new project.
 
+        :param name: The name of the new project
+        :param description: The description of the new project
+        :param exist_ok: If exist_ok is False (the default), a ValueError is raised if the project already exists. If
+        exist_ok is True and the project exists, then the existing project is returned.
         :return: The project.
         """
-        response = self.__request_with_json_response(
-            "post", f"/v1/projects", params={"name": name, "description": description}
-        )
-        return Project(self, response["payload"]["name"])
+
+        if self.exists_project(name):
+            if exist_ok:
+                project = self.get_project(name)
+            else:
+                raise ValueError(
+                    f"This project '{name}' already exists. You can pass the flag exist_ok=True to create_project to obtain the existing project."
+                )
+        else:
+            response = self.__request_with_json_response(
+                "post",
+                f"/v1/projects",
+                params={"name": name, "description": description},
+            )
+            project = Project(self, response["payload"]["name"])
+        return project
 
     def get_project(self, name: str) -> Project:
         """
         Access an existing project.
 
         :return: The project.
         """
@@ -1775,23 +1897,26 @@
         Upload file to the global resources. Existing files with same path/name will be overwritten.
 
         :return: List of resources after upload.
         """
         zip_file = self._create_zip_io(source, path_in_zip)
         return self._upload_resources(zip_file)["files"]
 
-    @experimental_api
     def list_projects(self) -> dict:
         """
-        HIGHLY EXPERIMENTAL API - may soon change or disappear.
-
         Returns a list of the projects.
         """
 
-        response = self.__request_with_json_response("get", f"/experimental/projects")
+        try:
+            response = self.__request_with_json_response("get", f"/v1/projects")
+        except RequestException as e:
+            # in HD 6 below 6.11.0 the following url is used
+            if '405' not in e.args[0]:
+                raise e
+            response = self.__request_with_json_response("get", f"/experimental/projects")
         return response["payload"]
 
     @experimental_api
     def exists_project(self, name: str) -> bool:
         """
         HIGHLY EXPERIMENTAL API - may soon change or disappear.
 
@@ -2245,47 +2370,42 @@
         if build_version.startswith("5."):
             raise OperationNotSupported(
                 "Text analysis export is not supported for platform version 5.x, it is only supported from 6.x onwards."
             )
 
         process_name = self.__process_name(process)
 
-        if self._is_higher_equal_version(build_version, 6, 7):
+        try:
             return str(
                 self.__request_with_bytes_response(
                     "get",
                     f"/experimental/textanalysis/projects/{project}/documentCollections/{collection_name}"
                     f"/processes/{process_name}/textAnalysisResult",
                     headers={
                         HEADER_ACCEPT: MEDIA_TYPE_APPLICATION_XMI,
                     },
                     params={"documentName": document_name},
                 ),
                 ENCODING_UTF_8,
             )
 
-        return str(
-            self.__request_with_bytes_response(
-                "get",
-                f"/experimental/textanalysis/projects/{project}/documentCollections/{collection_name}"
-                f"/documents/{document_id}/processes/{process_name}/exportTextAnalysisResult",
-                headers={
-                    HEADER_ACCEPT: MEDIA_TYPE_APPLICATION_XMI,
-                },
-            ),
-            ENCODING_UTF_8,
-        )
+        except RequestException as e:
+            # in HD 6 below version 6.7 the endpoint is called with identifiers instead
+            return str(
+                self.__request_with_bytes_response(
+                    "get",
+                    f"/experimental/textanalysis/projects/{project}/documentCollections/{collection_name}"
+                    f"/documents/{document_id}/processes/{process_name}/exportTextAnalysisResult",
+                    headers={
+                        HEADER_ACCEPT: MEDIA_TYPE_APPLICATION_XMI,
+                    },
+                ),
+                ENCODING_UTF_8,
+            )
 
-    @staticmethod
-    def _is_higher_equal_version(version: str, compare_major: int, compare_minor: int) -> bool:
-        version_parts = version.split(".")
-        major = int(version_parts[0])
-        return major > compare_major or (
-            major == compare_major and int(version_parts[1]) >= compare_minor
-        )
 
     @experimental_api
     def _export_analysis_result_typesystem(
         self, project: str, collection_name: str, document_id: str, process: Union[Process, str]
     ) -> str:
         """
         HIGHLY EXPERIMENTAL API - may soon change or disappear.
@@ -2866,7 +2986,62 @@
             files["typesystemFile"] = (
                 "typesystem.xml",
                 typesystem.to_xml(),
                 MEDIA_TYPE_APPLICATION_XML,
             )
 
         return files
+
+    @experimental_api
+    def _evaluate(
+        self,
+        project: Project,
+        comparison_process: Process,
+        reference_process: Process,
+        process_name: str,
+        evaluation_configurations: List["EvaluationConfiguration"],
+        number_of_pipeline_instances: int,
+    ) -> Process:
+        """
+        HIGHLY EXPERIMENTAL API - may soon change or disappear.
+
+        Use {process}.evaluate_against() instead.
+        """
+        creation_response = self.__request_with_json_response(
+            "post",
+            f"/experimental/textanalysis/projects/{project.name}/documentCollections/{comparison_process.document_source_name}/evaluationProcesses",
+            params={
+                "comparisonProcessName": comparison_process.name,
+                "referenceProcessName": reference_process.name,
+                "processName": process_name,
+                "numberOfPipelineInstances": number_of_pipeline_instances,
+                "referenceDocumentCollectionName": reference_process.document_source_name,
+            },
+            json=[vars(evaluation_configuration) for evaluation_configuration in evaluation_configurations],
+            headers={
+                HEADER_CONTENT_TYPE: MEDIA_TYPE_APPLICATION_JSON,
+                HEADER_ACCEPT: MEDIA_TYPE_APPLICATION_JSON,
+            },
+        )
+        if creation_response["errorMessages"]:
+            raise Exception(
+                f"Error during evaluation process creation {creation_response['errorMessages']}"
+            )
+        self._ensure_process_created(project, process_name)
+
+        return Process(
+            project=project,
+            name=process_name,
+            document_source_name=comparison_process.document_source_name,
+        )
+
+    def _ensure_process_created(self, project: Project, process_name: str):
+        processes = self._list_processes(project)
+        total_time_slept = 0
+        while all(p.name != process_name for p in processes):
+            if total_time_slept > self._polling_timeout:
+                raise OperationTimeoutError(
+                    f"Process not found for ${total_time_slept}"
+                )
+            sleep(self._poll_delay)
+            total_time_slept += self._poll_delay
+            processes = self._list_processes(project)
```

### Comparing `averbis-python-api-0.8.0/averbis/highlighting/__init__.py` & `averbis-python-api-0.9.0/averbis/highlighting/__init__.py`

 * *Files identical despite different names*

### Comparing `averbis-python-api-0.8.0/averbis/highlighting/_utils.py` & `averbis-python-api-0.9.0/averbis/highlighting/_utils.py`

 * *Files identical despite different names*

### Comparing `averbis-python-api-0.8.0/averbis_python_api.egg-info/PKG-INFO` & `averbis-python-api-0.9.0/averbis_python_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: averbis-python-api
-Version: 0.8.0
+Version: 0.9.0
 Summary: Averbis REST API client for Python.
 Home-page: UNKNOWN
 Author: Averbis GmbH
 License: Apache License, Version 2.0. Copyright Averbis GmbH
 Project-URL: Bug Tracker, https://github.com/averbis/averbis-python-api/issues
 Project-URL: Source Code, https://github.com/averbis/averbis-python-api
 Platform: UNKNOWN
```

### Comparing `averbis-python-api-0.8.0/averbis_python_api.egg-info/SOURCES.txt` & `averbis-python-api-0.9.0/averbis_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `averbis-python-api-0.8.0/setup.py` & `averbis-python-api-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `averbis-python-api-0.8.0/tests/__init__.py` & `averbis-python-api-0.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `averbis-python-api-0.8.0/tests/fixtures.py` & `averbis-python-api-0.9.0/tests/fixtures.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,14 +76,23 @@
     requests_mock.get(
         f"{URL_BASE_ID + '/rest/v1'}/buildInfo",
         headers={"Content-Type": "application/json"},
         json={"payload": {"specVersion": "6.7.0", "buildNumber": ""}, "errorMessages": []},
     )
 
 
+@pytest.fixture()
+def requests_mock_id6_11(requests_mock):
+    requests_mock.get(
+        f"{URL_BASE_ID + '/rest/v1'}/buildInfo",
+        headers={"Content-Type": "application/json"},
+        json={"payload": {"specVersion": "6.11.0", "buildNumber": ""}, "errorMessages": []},
+    )
+
+
 ## Different clients based on the above platforms
 
 # Tests that should work for all platform versions
 @pytest.fixture(params=["5.33.0", "6.0.0"])
 def client(request, requests_mock):
     requests_mock.get(
         f"{API_BASE}/buildInfo",
@@ -101,11 +110,17 @@
 
 # Tests that should work in platform version 6
 @pytest.fixture()
 def client_version_6(requests_mock_id6):
     return Client(URL_BASE_ID, api_token=TEST_API_TOKEN)
 
 
-# Tests that should work in platform version 6.7
+# Tests that should work in version 6.7
 @pytest.fixture()
 def client_version_6_7(requests_mock_id6_7):
     return Client(URL_BASE_ID, api_token=TEST_API_TOKEN)
+
+
+# Tests that should work in version 6.11
+@pytest.fixture()
+def client_version_6_11(requests_mock_id6_11):
+    return Client(URL_BASE_ID, api_token=TEST_API_TOKEN)
```

### Comparing `averbis-python-api-0.8.0/tests/test_client.py` & `averbis-python-api-0.9.0/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,86 +154,133 @@
     build_info = client.get_build_info()
 
     assert build_info["specVersion"] == "5.33.0"
     assert build_info["buildNumber"] == ""
 
 
 def test_create_project(client, requests_mock):
-    def callback(request, _):
+    def create_project_callback(request, _):
         return {
             "payload": {
                 "id": 93498,
                 "name": request.qs["name"][0],
                 "description": request.qs["description"][0],
             },
             "errorMessages": [],
         }
 
     requests_mock.post(
-        f"{API_BASE}/projects", headers={"Content-Type": "application/json"}, json=callback
+        f"{API_BASE}/projects",
+        headers={"Content-Type": "application/json"},
+        json=create_project_callback,
     )
 
-    project = client.create_project(PROJECT_NAME, "Project for load testing")
+    existing_project_name = "test_project"
+    requests_mock.get(
+        f"{API_BASE}/projects",
+        headers={"Content-Type": "application/json"},
+        json={
+            "payload": [
+                {"name": existing_project_name, "description": ""},
+                {"name": "intern", "description": ""},
+            ],
+            "errorMessages": [],
+        },
+    )
 
+    project = client.create_project(PROJECT_NAME, "Project for load testing")
     assert project.name == PROJECT_NAME
 
+    with pytest.raises(ValueError):
+        client.create_project(existing_project_name)
+
+    project = client.create_project(existing_project_name, exist_ok=True)
+    assert project.name == existing_project_name
+
 
 def test_get_project(client):
     project = client.get_project(PROJECT_NAME)
 
     assert project.name == PROJECT_NAME
 
 
 def test_list_projects(client, requests_mock):
+
     def callback(request, _):
         return {
             "payload": [
                 {"name": "Jumble", "description": ""},
                 {"name": "Bumble", "description": ""},
             ],
             "errorMessages": [],
         }
 
     requests_mock.get(
+        f"{API_BASE}/projects", headers={"Content-Type": "application/json"}, status_code=405
+    )
+
+    requests_mock.get(
         f"{API_EXPERIMENTAL}/projects", headers={"Content-Type": "application/json"}, json=callback
     )
 
     project_list = client.list_projects()
 
     assert project_list[0]["name"] == "Jumble"
     assert project_list[1]["name"] == "Bumble"
 
 
+def test_list_projects_v6_11(client_version_6_11, requests_mock):
+    def callback(request, _):
+        return {
+            "payload": [
+                {"name": "Jumble", "description": ""},
+                {"name": "Bumble", "description": ""},
+            ],
+            "errorMessages": [],
+        }
+
+    requests_mock.get(
+        f"{API_BASE}/projects", headers={"Content-Type": "application/json"}, json=callback
+    )
+
+    project_list = client_version_6_11.list_projects()
+
+    assert project_list[0]["name"] == "Jumble"
+    assert project_list[1]["name"] == "Bumble"
+
+
 def test_exists_project(client, requests_mock):
     def callback(request, _):
         return {
             "payload": [
                 {"name": "Jumble", "description": ""},
                 {"name": "Bumble", "description": ""},
             ],
             "errorMessages": [],
         }
 
     requests_mock.get(
-        f"{API_EXPERIMENTAL}/projects", headers={"Content-Type": "application/json"}, json=callback
+        f"{API_BASE}/projects", headers={"Content-Type": "application/json"}, status_code=405
     )
 
-    project_list = client.list_projects()
+    requests_mock.get(
+        f"{API_EXPERIMENTAL}/projects", headers={"Content-Type": "application/json"}, json=callback
+    )
 
     assert client.exists_project("Jumble") is True
     assert client.exists_project("Bumble") is True
     assert client.exists_project("Mumble") is False
 
 
 def test_delete_project(client_version_5):
     with pytest.raises(OperationNotSupported):
-        client._delete_project(PROJECT_NAME)
+        client_version_5._delete_project(PROJECT_NAME)
 
 
-def test_delete_project(client_version_6, requests_mock):
+def test_delete_project_v6(client_version_6, requests_mock):
     project = client_version_6.get_project(PROJECT_NAME)
     requests_mock.delete(
         f"{API_EXPERIMENTAL}/projects/{project.name}",
         headers={"Content-Type": "application/json"},
         json={"payload": None, "errorMessages": []},
     )
     response = project.delete()
@@ -707,50 +754,14 @@
 
 
 def test_analyse_html(client, requests_mock):
     requests_mock.post(
         f"{API_BASE}/textanalysis/projects/{PROJECT_NAME}/pipelines/discharge/analyseHtml",
         headers={"Content-Type": "application/json"},
         json={
-            "payload": [
-                {
-                    "begin": 28,
-                    "end": 40,
-                    "type": "de.averbis.types.health.Diagnosis",
-                    "coveredText": "Appendizitis",
-                    # ... truncated ...
-                },
-                {
-                    "begin": 0,
-                    "end": 41,
-                    "type": "de.averbis.types.health.PatientInformation",
-                    "coveredText": "Der Patient leidet an einer Appendizitis.",
-                    # ... truncated ...
-                },
-                # ... truncated ...
-            ],
-            "errorMessages": [],
-        },
-    )
-
-    response = client._analyse_html(
-        PROJECT_NAME,
-        "discharge",
-        "<html><body>Der Patient leidet an einer Appendizitis.</body></html>",
-        language="de",
-    )
-
-    assert response[0]["coveredText"] == "Appendizitis"
-
-
-def test_analyse_html(client, requests_mock):
-    requests_mock.post(
-        f"{API_BASE}/textanalysis/projects/{PROJECT_NAME}/pipelines/discharge/analyseHtml",
-        headers={"Content-Type": "application/json"},
-        json={
             "payload": [
                 {
                     "begin": 28,
                     "end": 40,
                     "type": "de.averbis.types.health.Diagnosis",
                     "coveredText": "Appendizitis",
                     # ... truncated ...
```

### Comparing `averbis-python-api-0.8.0/tests/test_document_collection.py` & `averbis-python-api-0.9.0/tests/test_document_collection.py`

 * *Files identical despite different names*

### Comparing `averbis-python-api-0.8.0/tests/test_highlighting.py` & `averbis-python-api-0.9.0/tests/test_highlighting.py`

 * *Files identical despite different names*

### Comparing `averbis-python-api-0.8.0/tests/test_pear.py` & `averbis-python-api-0.9.0/tests/test_pear.py`

 * *Files identical despite different names*

### Comparing `averbis-python-api-0.8.0/tests/test_pipeline.py` & `averbis-python-api-0.9.0/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `averbis-python-api-0.8.0/tests/test_process.py` & `averbis-python-api-0.9.0/tests/test_process.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,39 +19,37 @@
 #
 import tempfile
 from pathlib import Path
 
 from cassis import Cas, TypeSystem
 
 from averbis import Project, Pipeline
-from averbis.core import OperationNotSupported, MEDIA_TYPE_APPLICATION_XMI
+from averbis.core import OperationNotSupported, MEDIA_TYPE_APPLICATION_XMI, EvaluationConfiguration
 from tests.fixtures import *
 from tests.utils import *
 
 
 @pytest.fixture()
 def process(client) -> Process:
     project = client.get_project(PROJECT_NAME)
     return Process(project, "my_process", "my_doc_source", "my_pipeline")
 
 
 def test_delete(process, requests_mock):
-
     requests_mock.delete(
         f"{API_EXPERIMENTAL}/textanalysis/projects/{PROJECT_NAME}/"
         f"documentSources/{process.document_source_name}/processes/{process.name}",
         headers={"Content-Type": "application/json"},
         json={"payload": None, "errorMessages": []},
     )
 
     process.delete()
 
 
 def test_rerun(process, requests_mock):
-
     requests_mock.post(
         f"{API_EXPERIMENTAL}/textanalysis/projects/{PROJECT_NAME}/"
         f"documentSources/{process.document_source_name}/processes/{process.name}/reprocess",
         headers={"Content-Type": "application/json"},
         json={"payload": None, "errorMessages": []},
     )
 
@@ -239,15 +237,15 @@
     )
     process = collection.get_process(process_name)
 
     def callback(request, _content):
         page_size = int(request.qs["pageSize"][0])
         page = int(request.qs["page"][0])
         return_payload = [
-            {"documentName": f"Document ({page_size*(page-1)+k}).txt", "annotationDtos": []}
+            {"documentName": f"Document ({page_size * (page - 1) + k}).txt", "annotationDtos": []}
             for k in range(1, page_size + 1)
         ]
         return {
             "payload": {
                 "textAnalysisResultDtos": return_payload,
                 "projectName": project.name,
                 # Truncated
@@ -370,14 +368,21 @@
             "payload": [{"documentIdentifier": document_id, "documentName": document_name}],
             "errorMessages": [],
         },
     )
 
     requests_mock.get(
         f"{API_EXPERIMENTAL}/textanalysis/projects/{project.name}/documentCollections/{collection.name}"
+        f"/processes/{process.name}/textAnalysisResult",
+        headers={"Content-Type": "application/vnd.uima.cas+xmi"},
+        status_code=405
+    )
+
+    requests_mock.get(
+        f"{API_EXPERIMENTAL}/textanalysis/projects/{project.name}/documentCollections/{collection.name}"
         f"/documents/{document_id}/processes/{process.name}/exportTextAnalysisResult",
         headers={"Content-Type": "application/vnd.uima.cas+xmi"},
         text=expected_xmi,
     )
 
     cas = process.export_text_analysis_to_cas(document_name)
 
@@ -453,7 +458,56 @@
                 Path(tmp_file.name), document_name, mime_type=MEDIA_TYPE_APPLICATION_XMI
             )
         # should raise exception because mime type is not given
         with pytest.raises(Exception):
             process.import_text_analysis_result(
                 Path(tmp_file.name), document_name, typesystem=typesystem
             )
+
+
+def test_evaluate(client_version_6, requests_mock):
+    project = client_version_6.get_project(PROJECT_NAME)
+    collection = project.get_document_collection(COLLECTION_NAME)
+    comparison_process = Process(project, "comparison-process", collection.name)
+    reference_process = Process(project, "reference-process", collection.name)
+    evaluation_process_name = "evaluation_process"
+    requests_mock.post(
+        f"{API_EXPERIMENTAL}/textanalysis/projects/{project.name}/documentCollections/{collection.name}/evaluationProcesses",
+        headers={"Content-Type": "application/json"},
+        json={"payload": None, "errorMessages": []}
+    )
+    list_processes_payload = [{
+        "processName": evaluation_process_name,
+        "documentSourceName": collection.name
+    }]
+    requests_mock.get(
+        f"{API_EXPERIMENTAL}/textanalysis/projects/{project.name}/processes",
+        json={"payload": list_processes_payload, "errorMessages": []},
+    )
+    get_process_payload = {
+        "processName": evaluation_process_name,
+        "documentSourceName": collection.name,
+        "state": "IDLE",
+        "numberOfTotalDocuments": 3,
+        "numberOfSuccessfulDocuments": 3,
+        "numberOfUnsuccessfulDocuments": 0,
+        "errorMessages": [],
+        "comparisonProcessName": comparison_process.name,
+        "referenceProcessName": reference_process.name
+    }
+    requests_mock.get(
+        f"{API_EXPERIMENTAL}/textanalysis/projects/{project.name}/documentSources/{collection.name}/processes/{evaluation_process_name}",
+        json={"payload": get_process_payload, "errorMessages": []},
+    )
+
+    clinical_section_keyword_config = EvaluationConfiguration("de.averbis.types.health.ClinicalSectionKeyword",
+                                                                     ["begin", "end"])
+    medication_keyword_config = EvaluationConfiguration("de.averbis.types.health.Medication", ["begin", "end"])\
+        .add_feature("drugs")\
+        .use_range_variance_partial_match(3)
+    evaluation_process = comparison_process.evaluate_against(
+        reference_process,
+        evaluation_process_name,
+        [clinical_section_keyword_config, medication_keyword_config])
+
+    assert evaluation_process.name == evaluation_process_name
+    assert evaluation_process.document_source_name == collection.name
```

### Comparing `averbis-python-api-0.8.0/tests/test_project.py` & `averbis-python-api-0.9.0/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `averbis-python-api-0.8.0/tests/utils.py` & `averbis-python-api-0.9.0/tests/utils.py`

 * *Files identical despite different names*

