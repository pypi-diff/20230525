# Comparing `tmp/phc-0.9.1.tar.gz` & `tmp/phc-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/phc-0.9.1.tar", last modified: Tue Dec 17 11:11:19 2019, max compression
+gzip compressed data, was "dist/phc-0.9.2.tar", last modified: Wed Feb 19 18:01:57 2020, max compression
```

## Comparing `phc-0.9.1.tar` & `phc-0.9.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-17 11:11:19.000000 phc-0.9.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2019-12-17 11:10:23.000000 phc-0.9.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     4606 2019-12-17 11:11:19.000000 phc-0.9.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3083 2019-12-17 11:10:23.000000 phc-0.9.1/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-17 11:11:19.000000 phc-0.9.1/phc/
--rw-rw-r--   0 travis    (2000) travis    (2000)      456 2019-12-17 11:10:23.000000 phc-0.9.1/phc/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3663 2019-12-17 11:10:23.000000 phc-0.9.1/phc/api_response.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8927 2019-12-17 11:10:23.000000 phc-0.9.1/phc/base_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      870 2019-12-17 11:10:23.000000 phc-0.9.1/phc/errors.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-17 11:11:19.000000 phc-0.9.1/phc/services/
--rw-rw-r--   0 travis    (2000) travis    (2000)      656 2019-12-17 11:10:23.000000 phc-0.9.1/phc/services/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      688 2019-12-17 11:10:23.000000 phc-0.9.1/phc/services/accounts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12855 2019-12-17 11:10:23.000000 phc-0.9.1/phc/services/analytics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3132 2019-12-17 11:10:23.000000 phc-0.9.1/phc/services/cohorts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2159 2019-12-17 11:10:23.000000 phc-0.9.1/phc/services/fhir.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8189 2019-12-17 11:10:23.000000 phc-0.9.1/phc/services/files.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7262 2019-12-17 11:10:23.000000 phc-0.9.1/phc/services/genomics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3456 2019-12-17 11:10:23.000000 phc-0.9.1/phc/services/projects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1935 2019-12-17 11:10:23.000000 phc-0.9.1/phc/session.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-17 11:11:19.000000 phc-0.9.1/phc/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)      466 2019-12-17 11:10:23.000000 phc-0.9.1/phc/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      841 2019-12-17 11:10:23.000000 phc-0.9.1/phc/util/data_lake_query.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5613 2019-12-17 11:10:23.000000 phc-0.9.1/phc/util/patient_filter_query_builder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2019-12-17 11:10:23.000000 phc-0.9.1/phc/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-17 11:11:19.000000 phc-0.9.1/phc.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4606 2019-12-17 11:11:19.000000 phc-0.9.1/phc.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      563 2019-12-17 11:11:19.000000 phc-0.9.1/phc.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-12-17 11:11:19.000000 phc-0.9.1/phc.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       50 2019-12-17 11:11:19.000000 phc-0.9.1/phc.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        4 2019-12-17 11:11:19.000000 phc-0.9.1/phc.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       32 2019-12-17 11:10:23.000000 phc-0.9.1/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-12-17 11:11:19.000000 phc-0.9.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1426 2019-12-17 11:10:23.000000 phc-0.9.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-19 18:01:57.000000 phc-0.9.2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       24 2020-02-19 18:01:01.000000 phc-0.9.2/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4606 2020-02-19 18:01:57.000000 phc-0.9.2/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3083 2020-02-19 18:01:01.000000 phc-0.9.2/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-19 18:01:57.000000 phc-0.9.2/phc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      456 2020-02-19 18:01:01.000000 phc-0.9.2/phc/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3663 2020-02-19 18:01:01.000000 phc-0.9.2/phc/api_response.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9105 2020-02-19 18:01:01.000000 phc-0.9.2/phc/base_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      870 2020-02-19 18:01:01.000000 phc-0.9.2/phc/errors.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-19 18:01:57.000000 phc-0.9.2/phc/services/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      656 2020-02-19 18:01:01.000000 phc-0.9.2/phc/services/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      688 2020-02-19 18:01:01.000000 phc-0.9.2/phc/services/accounts.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12855 2020-02-19 18:01:01.000000 phc-0.9.2/phc/services/analytics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3132 2020-02-19 18:01:01.000000 phc-0.9.2/phc/services/cohorts.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2287 2020-02-19 18:01:01.000000 phc-0.9.2/phc/services/fhir.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8189 2020-02-19 18:01:01.000000 phc-0.9.2/phc/services/files.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7262 2020-02-19 18:01:01.000000 phc-0.9.2/phc/services/genomics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3456 2020-02-19 18:01:01.000000 phc-0.9.2/phc/services/projects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1935 2020-02-19 18:01:01.000000 phc-0.9.2/phc/session.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-19 18:01:57.000000 phc-0.9.2/phc/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      466 2020-02-19 18:01:01.000000 phc-0.9.2/phc/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      841 2020-02-19 18:01:01.000000 phc-0.9.2/phc/util/data_lake_query.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5613 2020-02-19 18:01:01.000000 phc-0.9.2/phc/util/patient_filter_query_builder.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-02-19 18:01:01.000000 phc-0.9.2/phc/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-19 18:01:57.000000 phc-0.9.2/phc.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4606 2020-02-19 18:01:57.000000 phc-0.9.2/phc.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      578 2020-02-19 18:01:57.000000 phc-0.9.2/phc.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-19 18:01:57.000000 phc-0.9.2/phc.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       50 2020-02-19 18:01:57.000000 phc-0.9.2/phc.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        4 2020-02-19 18:01:57.000000 phc-0.9.2/phc.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      179 2020-02-19 18:01:01.000000 phc-0.9.2/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       32 2020-02-19 18:01:01.000000 phc-0.9.2/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-02-19 18:01:57.000000 phc-0.9.2/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1426 2020-02-19 18:01:01.000000 phc-0.9.2/setup.py
```

### Comparing `phc-0.9.1/PKG-INFO` & `phc-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phc
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python interface for the PHC.
 Home-page: https://lifeomic.github.io/phc-sdk-py
 Author: LifeOmic Development
 Author-email: development@lifeomic.com
 License: MIT
 Description: # PHC SDK for Python
```

### Comparing `phc-0.9.1/README.md` & `phc-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `phc-0.9.1/phc/api_response.py` & `phc-0.9.2/phc/api_response.py`

 * *Files identical despite different names*

### Comparing `phc-0.9.1/phc/base_client.py` & `phc-0.9.2/phc/base_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,26 +80,28 @@
         self,
         api_path: str,
         http_verb: str = "POST",
         upload_file: [str, bytes] = None,
         json: dict = None,
         data: str = None,
         headers: dict = {},
+        params: dict = {},
     ) -> Union[asyncio.Future, ApiResponse]:
         if self.session.is_expired() and self.session.refresh_token:
             self._refresh_token()
 
         return self._api_call_impl(
             self.session.api_url,
             api_path,
             http_verb,
             upload_file,
             json,
             data,
             headers,
+            params,
         )
 
     def _fhir_call(
         self,
         api_path: str,
         http_verb: str = "POST",
         upload_file: [str, bytes] = None,
@@ -164,14 +166,15 @@
         url: str,
         api_path: str,
         http_verb: str = "POST",
         upload_file: [str, bytes] = None,
         json: dict = None,
         data: str = None,
         headers: dict = {},
+        params: dict = {},
     ) -> Union[asyncio.Future, ApiResponse]:
         """Sends an API request
 
         Arguments:
             api_path {str} -- The root API path
 
         Keyword Arguments:
@@ -187,14 +190,15 @@
 
         if self.session.is_expired() and not self.session.refresh_token:
             raise RequestError("The session token has expired.")
 
         has_json = json is not None
         has_data = data is not None
         has_file = upload_file is not None
+        has_params = params is not None
 
         if has_json and has_data:
             raise Exception(
                 '"json" and "data" cannot be supplied as request body.'
             )
 
         req_args = {"headers": self._get_headers(has_json, headers)}
@@ -203,14 +207,17 @@
 
         elif has_data:
             req_args["data"] = data
 
         elif has_file:
             req_args["file"] = upload_file
 
+        if has_params:
+            req_args["params"] = params
+
         api_url = urljoin(url, api_path)
 
         future = asyncio.ensure_future(
             self._send(http_verb=http_verb, api_url=api_url, req_args=req_args),
             loop=self._event_loop,
         )
```

### Comparing `phc-0.9.1/phc/errors.py` & `phc-0.9.2/phc/errors.py`

 * *Files identical despite different names*

### Comparing `phc-0.9.1/phc/services/__init__.py` & `phc-0.9.2/phc/services/__init__.py`

 * *Files identical despite different names*

### Comparing `phc-0.9.1/phc/services/accounts.py` & `phc-0.9.2/phc/services/accounts.py`

 * *Files identical despite different names*

### Comparing `phc-0.9.1/phc/services/analytics.py` & `phc-0.9.2/phc/services/analytics.py`

 * *Files identical despite different names*

### Comparing `phc-0.9.1/phc/services/cohorts.py` & `phc-0.9.2/phc/services/cohorts.py`

 * *Files identical despite different names*

### Comparing `phc-0.9.1/phc/services/fhir.py` & `phc-0.9.2/phc/services/fhir.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,17 @@
         The PHC session
     run_async: bool
         True to return promises, False to return results (default is False)
     timeout: int
         Operation timeout (default is 30)
     """
 
-    def execute_sql(self, project_id: str, statement: str) -> ApiResponse:
+    def execute_sql(
+        self, project_id: str, statement: str, scroll=""
+    ) -> ApiResponse:
         """Executes an SQL query against fhir-searh-service
 
         Parameters
         ----------
         project_id : str
             The project ID.
         statement : str
@@ -49,17 +51,20 @@
             [List] -- Dictionary with query response
         """
         return self._api_call(
             api_path=f"fhir-search/projects/{project_id}",
             http_verb="POST",
             data=statement,
             headers={"Content-Type": "text/plain"},
+            params={"scroll": scroll},
         )
 
-    def execute_es(self, project_id: str, query: dict) -> ApiResponse:
+    def execute_es(
+        self, project_id: str, query: dict, scroll=""
+    ) -> ApiResponse:
         """Executes an elasticsearch query against fhir-searh-service
 
         Parameters
         ----------
         project_id : str
             The project ID
         query : dict
@@ -70,8 +75,9 @@
         phc.ApiResponse
             The query response
         """
         return self._api_call(
             api_path=f"fhir-search/projects/{project_id}",
             http_verb="POST",
             json=query,
+            params={"scroll": scroll},
         )
```

### Comparing `phc-0.9.1/phc/services/files.py` & `phc-0.9.2/phc/services/files.py`

 * *Files identical despite different names*

### Comparing `phc-0.9.1/phc/services/genomics.py` & `phc-0.9.2/phc/services/genomics.py`

 * *Files identical despite different names*

### Comparing `phc-0.9.1/phc/services/projects.py` & `phc-0.9.2/phc/services/projects.py`

 * *Files identical despite different names*

### Comparing `phc-0.9.1/phc/session.py` & `phc-0.9.2/phc/session.py`

 * *Files identical despite different names*

### Comparing `phc-0.9.1/phc/util/data_lake_query.py` & `phc-0.9.2/phc/util/data_lake_query.py`

 * *Files identical despite different names*

### Comparing `phc-0.9.1/phc/util/patient_filter_query_builder.py` & `phc-0.9.2/phc/util/patient_filter_query_builder.py`

 * *Files identical despite different names*

### Comparing `phc-0.9.1/phc.egg-info/PKG-INFO` & `phc-0.9.2/phc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phc
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python interface for the PHC.
 Home-page: https://lifeomic.github.io/phc-sdk-py
 Author: LifeOmic Development
 Author-email: development@lifeomic.com
 License: MIT
 Description: # PHC SDK for Python
```

### Comparing `phc-0.9.1/setup.py` & `phc-0.9.2/setup.py`

 * *Files identical despite different names*

