# Comparing `tmp/gcp_pilot-1.8.0.tar.gz` & `tmp/gcp_pilot-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp_pilot-1.8.0.tar", max compression
+gzip compressed data, was "gcp_pilot-1.9.0.tar", max compression
```

## Comparing `gcp_pilot-1.8.0.tar` & `gcp_pilot-1.9.0.tar`

### file list

```diff
@@ -1,42 +1,41 @@
--rw-r--r--   0        0        0    11358 2023-02-10 16:02:48.492471 gcp_pilot-1.8.0/LICENSE.md
--rw-r--r--   0        0        0     7867 2023-02-10 16:02:48.492471 gcp_pilot-1.8.0/README.md
--rw-r--r--   0        0        0        0 2023-02-10 16:02:48.492471 gcp_pilot-1.8.0/gcp_pilot/__init__.py
--rw-r--r--   0        0        0     8623 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/api_gateway.py
--rw-r--r--   0        0        0     4319 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/api_key.py
--rw-r--r--   0        0        0     1267 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/app_engine.py
--rw-r--r--   0        0        0    17403 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/base.py
--rw-r--r--   0        0        0     9221 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/big_query.py
--rw-r--r--   0        0        0    11272 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/build.py
--rw-r--r--   0        0        0    10536 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/calendar.py
--rw-r--r--   0        0        0     9129 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/chats.py
--rw-r--r--   0        0        0    10520 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/datastore.py
--rw-r--r--   0        0        0     6219 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/directory.py
--rw-r--r--   0        0        0     5234 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/dns.py
--rw-r--r--   0        0        0     3479 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/error_reporting.py
--rw-r--r--   0        0        0     1208 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/factories/__init__.py
--rw-r--r--   0        0        0     2770 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/factories/identity_platform.py
--rw-r--r--   0        0        0     7203 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/functions.py
--rw-r--r--   0        0        0    19431 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/healthcare.py
--rw-r--r--   0        0        0     9218 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/iam.py
--rw-r--r--   0        0        0     1740 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/iap.py
--rw-r--r--   0        0        0    13147 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/identity_platform.py
--rw-r--r--   0        0        0     1503 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/logging.py
--rw-r--r--   0        0        0     1689 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/mocker.py
--rw-r--r--   0        0        0     1799 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/monitoring.py
--rw-r--r--   0        0        0     2102 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/people.py
--rw-r--r--   0        0        0    16264 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/pubsub.py
--rw-r--r--   0        0        0    18277 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/resource.py
--rw-r--r--   0        0        0     8177 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/run.py
--rw-r--r--   0        0        0     5190 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/scheduler.py
--rw-r--r--   0        0        0     3428 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/secret_manager.py
--rw-r--r--   0        0        0     2221 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/service_usage.py
--rw-r--r--   0        0        0      928 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/sheets.py
--rw-r--r--   0        0        0     2021 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/source.py
--rw-r--r--   0        0        0     1459 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/speech.py
--rw-r--r--   0        0        0     5099 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/sql.py
--rw-r--r--   0        0        0     4838 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/storage.py
--rw-r--r--   0        0        0     3896 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/gcp_pilot/tasks.py
--rw-r--r--   0        0        0     2749 2023-02-10 16:02:48.496471 gcp_pilot-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     9464 1970-01-01 00:00:00.000000 gcp_pilot-1.8.0/setup.py
--rw-r--r--   0        0        0     9811 1970-01-01 00:00:00.000000 gcp_pilot-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/LICENSE.md
+-rw-r--r--   0        0        0     7867 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/__init__.py
+-rw-r--r--   0        0        0     8623 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/api_gateway.py
+-rw-r--r--   0        0        0     4319 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/api_key.py
+-rw-r--r--   0        0        0     1267 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/app_engine.py
+-rw-r--r--   0        0        0    17403 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/base.py
+-rw-r--r--   0        0        0     9263 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/big_query.py
+-rw-r--r--   0        0        0    11272 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/build.py
+-rw-r--r--   0        0        0    10536 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/calendar.py
+-rw-r--r--   0        0        0     9129 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/chats.py
+-rw-r--r--   0        0        0    10520 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/datastore.py
+-rw-r--r--   0        0        0     6219 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/directory.py
+-rw-r--r--   0        0        0     5234 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/dns.py
+-rw-r--r--   0        0        0     3479 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/error_reporting.py
+-rw-r--r--   0        0        0     1208 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/factories/__init__.py
+-rw-r--r--   0        0        0     2770 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/factories/identity_platform.py
+-rw-r--r--   0        0        0     7203 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/functions.py
+-rw-r--r--   0        0        0    19431 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/healthcare.py
+-rw-r--r--   0        0        0     9218 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/iam.py
+-rw-r--r--   0        0        0     1740 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/iap.py
+-rw-r--r--   0        0        0    13147 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/identity_platform.py
+-rw-r--r--   0        0        0     1503 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/logging.py
+-rw-r--r--   0        0        0     1689 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/mocker.py
+-rw-r--r--   0        0        0     1799 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/monitoring.py
+-rw-r--r--   0        0        0     2102 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/people.py
+-rw-r--r--   0        0        0    16264 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/pubsub.py
+-rw-r--r--   0        0        0    18277 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/resource.py
+-rw-r--r--   0        0        0     8177 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/run.py
+-rw-r--r--   0        0        0     5190 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/scheduler.py
+-rw-r--r--   0        0        0     3428 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/secret_manager.py
+-rw-r--r--   0        0        0     2221 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/service_usage.py
+-rw-r--r--   0        0        0     1072 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/sheets.py
+-rw-r--r--   0        0        0     2021 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/source.py
+-rw-r--r--   0        0        0     1459 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/speech.py
+-rw-r--r--   0        0        0     5099 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/sql.py
+-rw-r--r--   0        0        0     4838 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/storage.py
+-rw-r--r--   0        0        0     3896 2023-03-01 18:50:28.461306 gcp_pilot-1.9.0/gcp_pilot/tasks.py
+-rw-r--r--   0        0        0     2756 2023-03-01 18:50:28.465306 gcp_pilot-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     9811 1970-01-01 00:00:00.000000 gcp_pilot-1.9.0/PKG-INFO
```

### Comparing `gcp_pilot-1.8.0/LICENSE.md` & `gcp_pilot-1.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/README.md` & `gcp_pilot-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/api_gateway.py` & `gcp_pilot-1.9.0/gcp_pilot/api_gateway.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/api_key.py` & `gcp_pilot-1.9.0/gcp_pilot/api_key.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/app_engine.py` & `gcp_pilot-1.9.0/gcp_pilot/app_engine.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/base.py` & `gcp_pilot-1.9.0/gcp_pilot/base.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/big_query.py` & `gcp_pilot-1.9.0/gcp_pilot/big_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         table = self.get_table(
             table_name=table_name,
             project_id=project_id,
             dataset_name=dataset_name,
         )
         errors = self.client.insert_rows(table=table, rows=rows)
         if errors:
-            raise Exception(f"Bigquery insert error: {errors}")
+            raise Exception(f"Bigquery insert error: {errors}")  # pylint: disable=broad-exception-raised
 
     def get_table(self, table_name: str, project_id: str | None = None, dataset_name: str | None = None) -> Table:
         dataset_ref = self._dataset_ref(project_id=project_id, dataset_name=dataset_name)
         table_ref = dataset_ref.table(table_id=table_name)
         return self.client.get_table(table_ref)
 
     def load(
```

### Comparing `gcp_pilot-1.8.0/gcp_pilot/build.py` & `gcp_pilot-1.9.0/gcp_pilot/build.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/calendar.py` & `gcp_pilot-1.9.0/gcp_pilot/calendar.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/chats.py` & `gcp_pilot-1.9.0/gcp_pilot/chats.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/datastore.py` & `gcp_pilot-1.9.0/gcp_pilot/datastore.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/directory.py` & `gcp_pilot-1.9.0/gcp_pilot/directory.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/dns.py` & `gcp_pilot-1.9.0/gcp_pilot/dns.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/error_reporting.py` & `gcp_pilot-1.9.0/gcp_pilot/error_reporting.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/exceptions.py` & `gcp_pilot-1.9.0/gcp_pilot/exceptions.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/factories/identity_platform.py` & `gcp_pilot-1.9.0/gcp_pilot/factories/identity_platform.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/functions.py` & `gcp_pilot-1.9.0/gcp_pilot/functions.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/healthcare.py` & `gcp_pilot-1.9.0/gcp_pilot/healthcare.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/iam.py` & `gcp_pilot-1.9.0/gcp_pilot/iam.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/iap.py` & `gcp_pilot-1.9.0/gcp_pilot/iap.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/identity_platform.py` & `gcp_pilot-1.9.0/gcp_pilot/identity_platform.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/logging.py` & `gcp_pilot-1.9.0/gcp_pilot/logging.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/mocker.py` & `gcp_pilot-1.9.0/gcp_pilot/mocker.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/monitoring.py` & `gcp_pilot-1.9.0/gcp_pilot/monitoring.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/people.py` & `gcp_pilot-1.9.0/gcp_pilot/people.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/pubsub.py` & `gcp_pilot-1.9.0/gcp_pilot/pubsub.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/resource.py` & `gcp_pilot-1.9.0/gcp_pilot/resource.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/run.py` & `gcp_pilot-1.9.0/gcp_pilot/run.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/scheduler.py` & `gcp_pilot-1.9.0/gcp_pilot/scheduler.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/secret_manager.py` & `gcp_pilot-1.9.0/gcp_pilot/secret_manager.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/service_usage.py` & `gcp_pilot-1.9.0/gcp_pilot/service_usage.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/sheets.py` & `gcp_pilot-1.9.0/gcp_pilot/sheets.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import gspread
 from google.auth.transport.requests import AuthorizedSession
+from gspread.client import extract_id_from_url
 
 from gcp_pilot.base import GoogleCloudPilotAPI
 
 
 class Spreadsheet(GoogleCloudPilotAPI):
     _scopes = [
         "https://www.googleapis.com/auth/spreadsheets",
         "https://www.googleapis.com/auth/drive",
     ]
 
     def __init__(self, sheet_id: str, **kwargs):
         super().__init__(**kwargs)
+        if sheet_id.startswith("https://"):
+            sheet_id = extract_id_from_url(sheet_id)
         self.sheet_id = sheet_id
         self.spreadsheet = self.client.open_by_key(self.sheet_id)
 
     def worksheet(self, name: str) -> gspread.Worksheet:
         return self.spreadsheet.worksheet(name)
 
     @classmethod
```

### Comparing `gcp_pilot-1.8.0/gcp_pilot/source.py` & `gcp_pilot-1.9.0/gcp_pilot/source.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/speech.py` & `gcp_pilot-1.9.0/gcp_pilot/speech.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/sql.py` & `gcp_pilot-1.9.0/gcp_pilot/sql.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/storage.py` & `gcp_pilot-1.9.0/gcp_pilot/storage.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/gcp_pilot/tasks.py` & `gcp_pilot-1.9.0/gcp_pilot/tasks.py`

 * *Files identical despite different names*

### Comparing `gcp_pilot-1.8.0/pyproject.toml` & `gcp_pilot-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gcp-pilot"
-version = "1.8.0"
+version = "1.9.0"
 description = "Google Cloud Platform Friendly Pilot"
 authors = ["Joao Daher <joao@daher.dev>"]
 repository = "https://github.com/flamingo-run/gcp-pilot"
 readme = "README.md"
 keywords = ["gcp", "google cloud python", "datastore orm"]
 packages = [
     { include = "gcp_pilot" },
@@ -69,15 +69,15 @@
 line_length = 120
 include_trailing_comma = true
 multi_line_output = 3
 src_paths = ["."]
 
 
 [tool.pylint.messages_control]
-disable = "C0114, C0115, C0116, W0212, W0511, W0613, W1203, W0221, R0901, R0903, R0913, R0801, R0401, R0902, R0914, E1101, R0912, C0204"
+disable = "C0114, C0115, C0116, W0212, W0511, W0613, W1203, W0221, R0901, R0903, R0913, R0801, R0401, R0902, R0914, E1101, R0912, C0204, R1735"
 
 [tool.pylint.format]
 max-line-length = "120"
 
 [tool.pylint.basic]
 good-names= "i, j, k, m, n, dt, db, id, pk, tz, qs, ex, _"
```

### Comparing `gcp_pilot-1.8.0/setup.py` & `gcp_pilot-1.9.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,247 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: gcp-pilot
+Version: 1.9.0
+Summary: Google Cloud Platform Friendly Pilot
+Home-page: https://github.com/flamingo-run/gcp-pilot
+Keywords: gcp,google cloud python,datastore orm
+Author: Joao Daher
+Author-email: joao@daher.dev
+Requires-Python: >=3.10,<3.12
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: bigquery
+Provides-Extra: build
+Provides-Extra: datastore
+Provides-Extra: dns
+Provides-Extra: healthcare
+Provides-Extra: iam
+Provides-Extra: monitoring
+Provides-Extra: pubsub
+Provides-Extra: secret
+Provides-Extra: sheets
+Provides-Extra: speech
+Provides-Extra: storage
+Provides-Extra: tasks
+Requires-Dist: factory_boy
+Requires-Dist: fhir.resources ; extra == "healthcare"
+Requires-Dist: google-api-python-client
+Requires-Dist: google-cloud-bigquery[storage] (>=3,<4) ; extra == "bigquery"
+Requires-Dist: google-cloud-build (>=3,<4) ; extra == "build"
+Requires-Dist: google-cloud-datastore (>=2,<3) ; extra == "datastore"
+Requires-Dist: google-cloud-dns (>=0,<1) ; extra == "dns"
+Requires-Dist: google-cloud-error-reporting ; extra == "monitoring"
+Requires-Dist: google-cloud-iam ; extra == "iam"
+Requires-Dist: google-cloud-logging (>=3,<4) ; extra == "monitoring"
+Requires-Dist: google-cloud-pubsub (>=2,<3) ; extra == "pubsub"
+Requires-Dist: google-cloud-scheduler (>=2,<3) ; extra == "tasks"
+Requires-Dist: google-cloud-secret-manager ; extra == "secret"
+Requires-Dist: google-cloud-speech (>=2,<3) ; extra == "speech"
+Requires-Dist: google-cloud-storage (>=2,<3) ; extra == "storage"
+Requires-Dist: google-cloud-tasks (>=2,<3) ; extra == "tasks"
+Requires-Dist: gspread (>=5,<6) ; extra == "sheets"
+Requires-Dist: pydantic ; extra == "datastore"
+Requires-Dist: pytz
+Requires-Dist: tenacity
+Project-URL: Repository, https://github.com/flamingo-run/gcp-pilot
+Description-Content-Type: text/markdown
+
+![Github CI](https://github.com/flamingo-run/gcp-pilot/workflows/Github%20CI/badge.svg)
+[![Coverage Status](https://coveralls.io/repos/github/flamingo-run/gcp-pilot/badge.svg)](https://coveralls.io/github/flamingo-run/gcp-pilot)
+[![python](https://img.shields.io/badge/python-3.11-blue.svg)]()
+
+# Google Cloud Pilot
+
+## Installation
+
+`pip install gcp-pilot`
+
+Some APIs need extra packages, thus you must use `extras` to add them:
+
+- Cloud Tasks: `pip install gcp-pilot[tasks]`
+- Cloud Build: `pip install gcp-pilot[build]`
+- Cloud Storage: `pip install gcp-pilot[storage]`
+- Big Query: `pip install gcp-pilot[bigquery]`
+- Speech: `pip install gcp-pilot[speech]`
+- Sheets: `pip install gcp-pilot[sheets]`
+- Pub/Sub: `pip install gcp-pilot[pubsub]`
+- Datastore: `pip install gcp-pilot[datastore]`
+- Cloud DNS: `pip install gcp-pilot[dns]`
+- Secret Manager: `pip install gcp-pilot[secret]`
+- Healthcare Engine: `pip install gcp-pilot[healthcare]`
+- IAM: `pip install gcp-pilot[iam]`
+
+
+## Usage
+
+```
+from gcp_pilot.resource import ResourceManager
+
+grm = ResourceManager()
+```
+
+## Default Values
+
+### Credentials
+
+`gcp-pilot` uses [ADC](https://cloud.google.com/docs/authentication/production#automatically) to detect credentials. This means that you must have one of the following setups:
+- Environment variable `GOOGLE_APPLICATION_CREDENTIALS` pointing to the JSON file with the credentials
+- Run inside GCP (Compute Engine, Cloud Run, GKE, AppEngine), so the machine's credentials will be used
+- Run locally after authenticating with `gcloud auth application-default login`
+
+You can also globally set a service account using the environment variable `DEFAULT_SERVICE_ACCOUNT`, which will require impersonation.
+
+### Project
+
+When creating a client, a default project is defined by using the project that the credentials belongs to.
+
+Clients that support managing resources from other projects can be overwritten per call.
+
+> Example: you create a `BigQuery` client using credentials from  `project_a`.
+All calls will query datasets from `project_a`, unless another project is passed as parameter when performing the call.
+
+You can also globally set a project using the environment variable `DEFAULT_PROJECT`
+
+### Location
+
+Very similar to default project, a default location is defined by using the project's location.
+The project's location will exist if you ever enabled AppEngine, so you had to set a location then.
+Otherwise, no default location will be set.
+
+You can also globally set a location using the environment variable `DEFAULT_LOCATION` and reduce the amount of API calls 
+when creating clients.
+
+## Why Use ``gcp-pilot``
+
+_"Since Google already has a [generic API client](https://github.com/googleapis/google-api-python-client) and so many [specific clients](https://github.com/googleapis?q=python&type=&language=), why should I use this library?"_
+
+Google's has 2 types of clients:
+- **dedicated**: custom-made for the APIs. They are excellent: they implement high level interaction with the API with friendly methods. The `gcp-pilot` can adds its value by handling authentication, friendly errors and parameter fallback.
+- **generic**: a single client that is capable of dynamically calling any REST API. They are a pain to use: very specific calls that must be translated from the documentation. The `gcp-pilot` comes in handy to add high-level interaction with friendly method such as `Calendar.create_event`, on top of all other vantages cited above.
+
+### Parameter Fallback
+
+Most API endpoints require `project_id` (sometimes even `project_number`) and `location`.
+
+So `gcp-pilot` automatically detects these values for you, based on your credentials (although it'll require extra permissions and API calls).
+
+If you use multiple projects, and your credentials is accessing other projects, you can still customize the parameters on each call to avoid the default fallback.
+
+
+### Friendly Errors
+
+Most APIs return a generic ``HttpException`` with am embedded payload with error output, and also there's a couple of different structures for these payloads.
+
+So `gcp-pilot` tries its best to convert these exceptions into more friendly ones, such as `NotFound`, `AlreadyExists` and `NotAllowed`.
+
+It'll be much easier to capture these exceptions and handle them by its type.
+
+
+### Identification Features
+
+- **Authentication**: each client uses [ADC](https://cloud.google.com/docs/authentication/production#automatically),
+which consists on trying to detect the service account with fallbacks: SDK > Environment Variable > Metadata
+- **Impersonation**: it's possible to create clients with ``impersonate_account`` parameter that [impersonates](https://cloud.google.com/iam/docs/impersonating-service-accounts#allow-impersonation) another account.
+- **Delegation**: services _(eg. Google Workspace)_ that requires specific subjects are automatically delegated, sometimes even performing additional credential signatures.
+- **Region**: most GCP services requires a location to work on *(some even require specific locations)*. If not provided, the clients use the project's default location, as defined by App Engine.
+- **Authorization**: OIDC authorization is automatically generated for services *(eg. CloudRun)* that require authentication to be used.
+
+### Auto-Authorization
+
+Some services require specific authorizations that should be setup prior to its usage, some examples:
+- [Pub/Sub] subscribe to a topic with authenticated push;
+- [Cloud Scheduler] schedule a job to trigger a Cloud Run service;
+- [Cloud Tasks] queue a task to trigger a Cloud Run service;
+
+In these cases, `gcp-pilot` tries its best to assure that the required permissions are properly set up
+before the actual request is made.
+
+### Integration
+
+Some services can be integrated, and `gcp-pilot` does just that in a seamless way by adding helper methods.
+
+Example: you can subscribe to Google Cloud Build's events to be notified by every build step.
+
+By using `CloudBuild.subscribe`, the `gcp-pilot` creates a subscription (and the topic, if needed) in the Google Pub/Sub service.
+
+## Supported APIs
+
+- IAM
+   - manage service accounts
+   - manage permissions
+   - encode & decode JWT tokens
+- Identity Platform
+  - sign in users
+  - sign up users
+  - reset password flow
+  - verify email flow
+- Credentials
+  - manage API Keys
+- Resource Manager
+   - manage projects
+   - manage permissions
+- Secret Manager
+  - manage secrets
+- Identity Aware Proxy
+   - generate OIDC token
+- Source Repositories
+   - manage repositories
+- Directory:
+  - manage users
+  - manage groups
+- People:
+  - get people
+- Cloud SQL
+   - manage instances
+   - manage databases
+   - manage users
+- Cloud Storage
+   - manage buckets
+   - manage files
+- Cloud Build
+   - manage triggers
+- Cloud Functions
+  - manager functions
+  - manage permissions
+- Cloud Scheduler
+   - manage schedules
+- Cloud Tasks
+   - manage tasks & queues
+- Cloud Run
+   - read services
+   - manage domain mappings [[1]](https://cloud.google.com/run/docs/mapping-custom-domains#adding_verified_domain_owners_to_other_users_or_service_accounts)
+- API Gateway
+  - manage APIs
+  - manage API Configs
+  - manage Gateways
+- Service Usage
+  - enable/disable APIs and Services
+- BigQuery
+   - manage datasets
+   - perform queries
+- Calendar
+   - manage events
+- Google Chats
+   - build complex messages
+   - call webhook
+   - interact as bot
+- Cloud Directory
+   - manage groups
+- Cloud DNS
+   - manage DNS zones
+   - manage zone's registers
+- Sheets
+   - manage spreadsheets (powered by gspread)
+- Speech
+   - recognize speech from audio
+- Datastore
+   - Object Mapping ("ORM-ish" management of documents)
+- Monitoring
+  - reporting errors
+  - logging
+  - manage custom services
+- Healthcare
+  - Manage datasets
+  - Manage stores
+  - Manage FHIR resources: _powered by [fhir-resources](https://github.com/nazrulworld/fhir.resources)_
 
-packages = \
-['gcp_pilot', 'gcp_pilot.factories']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['factory_boy', 'google-api-python-client', 'pytz', 'tenacity']
-
-extras_require = \
-{'bigquery': ['google-cloud-bigquery[storage]>=3,<4'],
- 'build': ['google-cloud-build>=3,<4'],
- 'datastore': ['google-cloud-datastore>=2,<3', 'pydantic'],
- 'dns': ['google-cloud-dns>=0,<1'],
- 'healthcare': ['fhir.resources'],
- 'iam': ['google-cloud-iam'],
- 'monitoring': ['google-cloud-logging>=3,<4', 'google-cloud-error-reporting'],
- 'pubsub': ['google-cloud-pubsub>=2,<3'],
- 'secret': ['google-cloud-secret-manager'],
- 'sheets': ['gspread>=5,<6'],
- 'speech': ['google-cloud-speech>=2,<3'],
- 'storage': ['google-cloud-storage>=2,<3'],
- 'tasks': ['google-cloud-tasks>=2,<3', 'google-cloud-scheduler>=2,<3']}
-
-setup_kwargs = {
-    'name': 'gcp-pilot',
-    'version': '1.8.0',
-    'description': 'Google Cloud Platform Friendly Pilot',
-    'long_description': '![Github CI](https://github.com/flamingo-run/gcp-pilot/workflows/Github%20CI/badge.svg)\n[![Coverage Status](https://coveralls.io/repos/github/flamingo-run/gcp-pilot/badge.svg)](https://coveralls.io/github/flamingo-run/gcp-pilot)\n[![python](https://img.shields.io/badge/python-3.11-blue.svg)]()\n\n# Google Cloud Pilot\n\n## Installation\n\n`pip install gcp-pilot`\n\nSome APIs need extra packages, thus you must use `extras` to add them:\n\n- Cloud Tasks: `pip install gcp-pilot[tasks]`\n- Cloud Build: `pip install gcp-pilot[build]`\n- Cloud Storage: `pip install gcp-pilot[storage]`\n- Big Query: `pip install gcp-pilot[bigquery]`\n- Speech: `pip install gcp-pilot[speech]`\n- Sheets: `pip install gcp-pilot[sheets]`\n- Pub/Sub: `pip install gcp-pilot[pubsub]`\n- Datastore: `pip install gcp-pilot[datastore]`\n- Cloud DNS: `pip install gcp-pilot[dns]`\n- Secret Manager: `pip install gcp-pilot[secret]`\n- Healthcare Engine: `pip install gcp-pilot[healthcare]`\n- IAM: `pip install gcp-pilot[iam]`\n\n\n## Usage\n\n```\nfrom gcp_pilot.resource import ResourceManager\n\ngrm = ResourceManager()\n```\n\n## Default Values\n\n### Credentials\n\n`gcp-pilot` uses [ADC](https://cloud.google.com/docs/authentication/production#automatically) to detect credentials. This means that you must have one of the following setups:\n- Environment variable `GOOGLE_APPLICATION_CREDENTIALS` pointing to the JSON file with the credentials\n- Run inside GCP (Compute Engine, Cloud Run, GKE, AppEngine), so the machine\'s credentials will be used\n- Run locally after authenticating with `gcloud auth application-default login`\n\nYou can also globally set a service account using the environment variable `DEFAULT_SERVICE_ACCOUNT`, which will require impersonation.\n\n### Project\n\nWhen creating a client, a default project is defined by using the project that the credentials belongs to.\n\nClients that support managing resources from other projects can be overwritten per call.\n\n> Example: you create a `BigQuery` client using credentials from  `project_a`.\nAll calls will query datasets from `project_a`, unless another project is passed as parameter when performing the call.\n\nYou can also globally set a project using the environment variable `DEFAULT_PROJECT`\n\n### Location\n\nVery similar to default project, a default location is defined by using the project\'s location.\nThe project\'s location will exist if you ever enabled AppEngine, so you had to set a location then.\nOtherwise, no default location will be set.\n\nYou can also globally set a location using the environment variable `DEFAULT_LOCATION` and reduce the amount of API calls \nwhen creating clients.\n\n## Why Use ``gcp-pilot``\n\n_"Since Google already has a [generic API client](https://github.com/googleapis/google-api-python-client) and so many [specific clients](https://github.com/googleapis?q=python&type=&language=), why should I use this library?"_\n\nGoogle\'s has 2 types of clients:\n- **dedicated**: custom-made for the APIs. They are excellent: they implement high level interaction with the API with friendly methods. The `gcp-pilot` can adds its value by handling authentication, friendly errors and parameter fallback.\n- **generic**: a single client that is capable of dynamically calling any REST API. They are a pain to use: very specific calls that must be translated from the documentation. The `gcp-pilot` comes in handy to add high-level interaction with friendly method such as `Calendar.create_event`, on top of all other vantages cited above.\n\n### Parameter Fallback\n\nMost API endpoints require `project_id` (sometimes even `project_number`) and `location`.\n\nSo `gcp-pilot` automatically detects these values for you, based on your credentials (although it\'ll require extra permissions and API calls).\n\nIf you use multiple projects, and your credentials is accessing other projects, you can still customize the parameters on each call to avoid the default fallback.\n\n\n### Friendly Errors\n\nMost APIs return a generic ``HttpException`` with am embedded payload with error output, and also there\'s a couple of different structures for these payloads.\n\nSo `gcp-pilot` tries its best to convert these exceptions into more friendly ones, such as `NotFound`, `AlreadyExists` and `NotAllowed`.\n\nIt\'ll be much easier to capture these exceptions and handle them by its type.\n\n\n### Identification Features\n\n- **Authentication**: each client uses [ADC](https://cloud.google.com/docs/authentication/production#automatically),\nwhich consists on trying to detect the service account with fallbacks: SDK > Environment Variable > Metadata\n- **Impersonation**: it\'s possible to create clients with ``impersonate_account`` parameter that [impersonates](https://cloud.google.com/iam/docs/impersonating-service-accounts#allow-impersonation) another account.\n- **Delegation**: services _(eg. Google Workspace)_ that requires specific subjects are automatically delegated, sometimes even performing additional credential signatures.\n- **Region**: most GCP services requires a location to work on *(some even require specific locations)*. If not provided, the clients use the project\'s default location, as defined by App Engine.\n- **Authorization**: OIDC authorization is automatically generated for services *(eg. CloudRun)* that require authentication to be used.\n\n### Auto-Authorization\n\nSome services require specific authorizations that should be setup prior to its usage, some examples:\n- [Pub/Sub] subscribe to a topic with authenticated push;\n- [Cloud Scheduler] schedule a job to trigger a Cloud Run service;\n- [Cloud Tasks] queue a task to trigger a Cloud Run service;\n\nIn these cases, `gcp-pilot` tries its best to assure that the required permissions are properly set up\nbefore the actual request is made.\n\n### Integration\n\nSome services can be integrated, and `gcp-pilot` does just that in a seamless way by adding helper methods.\n\nExample: you can subscribe to Google Cloud Build\'s events to be notified by every build step.\n\nBy using `CloudBuild.subscribe`, the `gcp-pilot` creates a subscription (and the topic, if needed) in the Google Pub/Sub service.\n\n## Supported APIs\n\n- IAM\n   - manage service accounts\n   - manage permissions\n   - encode & decode JWT tokens\n- Identity Platform\n  - sign in users\n  - sign up users\n  - reset password flow\n  - verify email flow\n- Credentials\n  - manage API Keys\n- Resource Manager\n   - manage projects\n   - manage permissions\n- Secret Manager\n  - manage secrets\n- Identity Aware Proxy\n   - generate OIDC token\n- Source Repositories\n   - manage repositories\n- Directory:\n  - manage users\n  - manage groups\n- People:\n  - get people\n- Cloud SQL\n   - manage instances\n   - manage databases\n   - manage users\n- Cloud Storage\n   - manage buckets\n   - manage files\n- Cloud Build\n   - manage triggers\n- Cloud Functions\n  - manager functions\n  - manage permissions\n- Cloud Scheduler\n   - manage schedules\n- Cloud Tasks\n   - manage tasks & queues\n- Cloud Run\n   - read services\n   - manage domain mappings [[1]](https://cloud.google.com/run/docs/mapping-custom-domains#adding_verified_domain_owners_to_other_users_or_service_accounts)\n- API Gateway\n  - manage APIs\n  - manage API Configs\n  - manage Gateways\n- Service Usage\n  - enable/disable APIs and Services\n- BigQuery\n   - manage datasets\n   - perform queries\n- Calendar\n   - manage events\n- Google Chats\n   - build complex messages\n   - call webhook\n   - interact as bot\n- Cloud Directory\n   - manage groups\n- Cloud DNS\n   - manage DNS zones\n   - manage zone\'s registers\n- Sheets\n   - manage spreadsheets (powered by gspread)\n- Speech\n   - recognize speech from audio\n- Datastore\n   - Object Mapping ("ORM-ish" management of documents)\n- Monitoring\n  - reporting errors\n  - logging\n  - manage custom services\n- Healthcare\n  - Manage datasets\n  - Manage stores\n  - Manage FHIR resources: _powered by [fhir-resources](https://github.com/nazrulworld/fhir.resources)_\n',
-    'author': 'Joao Daher',
-    'author_email': 'joao@daher.dev',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/flamingo-run/gcp-pilot',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.10,<3.12',
-}
-
-
-setup(**setup_kwargs)
```

