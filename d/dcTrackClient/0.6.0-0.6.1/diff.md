# Comparing `tmp/dctrackclient-0.6.0.tar.gz` & `tmp/dctrackclient-0.6.1.tar.gz`

## Comparing `dctrackclient-0.6.0.tar` & `dctrackclient-0.6.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    14009 2020-02-02 00:00:00.000000 dctrackclient-0.6.0/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.6.0/.gitignore
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 dctrackclient-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    17375 2020-02-02 00:00:00.000000 dctrackclient-0.6.0/../README.md
--rw-r--r--   0        0        0    17997 2020-02-02 00:00:00.000000 dctrackclient-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    14469 2020-02-02 00:00:00.000000 dctrackclient-0.6.1/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.6.1/.gitignore
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 dctrackclient-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    17764 2020-02-02 00:00:00.000000 dctrackclient-0.6.1/../README.md
+-rw-r--r--   0        0        0    18386 2020-02-02 00:00:00.000000 dctrackclient-0.6.1/PKG-INFO
```

### Comparing `dctrackclient-0.6.0/src/dcTrackClient/__init__.py` & `dctrackclient-0.6.1/src/dcTrackClient/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,18 @@
         """Get Model fields for the specified Model ID. usedCounts is an optional parameter that determines if the count of Items for the specified model is returned in the response. If set to "true" the counts will be included in the response, if omitted or set to "false" the item count will not be included in the response."""
         return self.__request('GET', '/api/v2/models/' + str(modelId) + '/?usedCounts=' + str(usedCounts) + '&')
 
     def createModel(self, returnDetails: bool, proceedOnWarning: bool, payload: dict):
         """Add a new Model. Returns JSON entity containing Make information that was passed in from the Request payload. "proceedOnWarning" relates to the warning messages that are thrown in dcTrack when you try to delete custom fields that are in use. The "proceedOnWarning" value can equal either "true" or "false." If "proceedOnWarning" equals "true," business warnings will be ignored. If "proceedOnWarning" equals "false," business warnings will not be ignored. Fields that are not in the payload will remain unchanged."""
         return self.__request('POST', '/api/v2/models/?returnDetails=' + str(returnDetails) + '&proceedOnWarning=' + str(proceedOnWarning) + '&', payload)
 
+    def updateModel(self, id: int, returnDetails: bool, proceedOnWarning: bool, payload: dict):
+        """Modify an existing Model. Fields that are not in the payload will remain unchanged. Returns a JSON entity containing Make information that was passed in from the Request payload."""
+        return self.__request('PUT', '/api/v2/models/' + str(id) + '/?returnDetails=' + str(returnDetails) + '&proceedOnWarning=' + str(proceedOnWarning) + '&', payload)
+
     def deleteModel(self, id: int):
         """Delete a Model using the Model ID."""
         return self.__request('DELETE', '/api/v2/models/' + str(id) + '/?')
 
     def searchModels(self, pageNumber: int, pageSize: int, payload: dict):
         """Search for models by user supplied search criteria. Returns a list of models with the "selectedColumns" returned in the payload. Search by Alias is not supported."""
         return self.__request('POST', '/api/v2/quicksearch/models/?pageNumber=' + str(pageNumber) + '&pageSize=' + str(pageSize) + '&', payload)
```

### Comparing `dctrackclient-0.6.0/pyproject.toml` & `dctrackclient-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "../README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dctrackclient-0.6.0/../README.md` & `dctrackclient-0.6.1/../README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API clients in Python and JavaScript
 
 ## Installation
 > dcTrackClient can be installed from the package manager of your choice.
 
 ### Python
 ```shell
-pip install dcTrackClient==0.6.0
+pip install dcTrackClient==0.6.1
 ```
 
 ### JavaScript
 ```shell
-npm i dctrackclient@0.6.0
+npm i dctrackclient@0.6.1
 ```
 
 ## Initialize a connection to the dcTrack API
 > Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
 
 ### Python
 ```py
@@ -314,14 +314,26 @@
 ```
 |Parameter|Type|
 |---|---|
 |returnDetails|boolean|
 |proceedOnWarning|boolean|
 |payload|object|
 
+## updateModel(id, returnDetails, proceedOnWarning, payload)
+> Modify an existing Model. Fields that are not in the payload will remain unchanged. Returns a JSON entity containing Make information that was passed in from the Request payload.
+```
+PUT api/v2/models/{id} payload
+```
+|Parameter|Type|
+|---|---|
+|id|number|
+|returnDetails|boolean|
+|proceedOnWarning|boolean|
+|payload|object|
+
 ## deleteModel(id)
 > Delete a Model using the Model ID.
 ```
 DELETE api/v2/models/{id}
 ```
 |Parameter|Type|
 |---|---|
```

### Comparing `dctrackclient-0.6.0/PKG-INFO` & `dctrackclient-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcTrackClient
-Version: 0.6.0
+Version: 0.6.1
 Summary: Sunbird dcTrack API client in Python
 Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
 Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
 Author-email: Nicolas Ventura <ventura@lbl.gov>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -20,20 +20,20 @@
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API clients in Python and JavaScript
 
 ## Installation
 > dcTrackClient can be installed from the package manager of your choice.
 
 ### Python
 ```shell
-pip install dcTrackClient==0.6.0
+pip install dcTrackClient==0.6.1
 ```
 
 ### JavaScript
 ```shell
-npm i dctrackclient@0.6.0
+npm i dctrackclient@0.6.1
 ```
 
 ## Initialize a connection to the dcTrack API
 > Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
 
 ### Python
 ```py
@@ -330,14 +330,26 @@
 ```
 |Parameter|Type|
 |---|---|
 |returnDetails|boolean|
 |proceedOnWarning|boolean|
 |payload|object|
 
+## updateModel(id, returnDetails, proceedOnWarning, payload)
+> Modify an existing Model. Fields that are not in the payload will remain unchanged. Returns a JSON entity containing Make information that was passed in from the Request payload.
+```
+PUT api/v2/models/{id} payload
+```
+|Parameter|Type|
+|---|---|
+|id|number|
+|returnDetails|boolean|
+|proceedOnWarning|boolean|
+|payload|object|
+
 ## deleteModel(id)
 > Delete a Model using the Model ID.
 ```
 DELETE api/v2/models/{id}
 ```
 |Parameter|Type|
 |---|---|
```

