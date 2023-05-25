# Comparing `tmp/warpzone_sdk-6.0.6.tar.gz` & `tmp/warpzone_sdk-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warpzone_sdk-6.0.6.tar", max compression
+gzip compressed data, was "warpzone_sdk-7.0.0.tar", max compression
```

## Comparing `warpzone_sdk-6.0.6.tar` & `warpzone_sdk-7.0.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1121 2023-05-22 13:42:03.793304 warpzone_sdk-6.0.6/pyproject.toml
--rw-r--r--   0        0        0     1182 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/__init__.py
--rw-r--r--   0        0        0       21 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/blobstorage/__init__.py
--rw-r--r--   0        0        0     2874 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/blobstorage/client.py
--rw-r--r--   0        0        0       24 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/enums/__init__.py
--rw-r--r--   0        0        0      213 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/enums/topicenum.py
--rw-r--r--   0        0        0       27 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/__init__.py
--rw-r--r--   0        0        0     1501 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/functionize.py
--rw-r--r--   0        0        0     3035 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/integrations.py
--rw-r--r--   0        0        0     2223 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/monitor.py
--rw-r--r--   0        0        0     1486 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/process.py
--rw-r--r--   0        0        0       32 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/processors/__init__.py
--rw-r--r--   0        0        0     1910 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/processors/outputs.py
--rw-r--r--   0        0        0     1727 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/processors/triggers.py
--rw-r--r--   0        0        0     2268 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/signature.py
--rw-r--r--   0        0        0       80 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/types.py
--rw-r--r--   0        0        0     2108 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/healthchecks/__init__.py
--rw-r--r--   0        0        0     1112 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/healthchecks/model.py
--rw-r--r--   0        0        0       87 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/monitor/__init__.py
--rw-r--r--   0        0        0     1650 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/monitor/logs.py
--rw-r--r--   0        0        0     4781 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/monitor/traces.py
--rw-r--r--   0        0        0       21 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/servicebus/data/__init__.py
--rw-r--r--   0        0        0     5403 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/servicebus/data/client.py
--rw-r--r--   0        0        0       21 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/servicebus/events/__init__.py
--rw-r--r--   0        0        0     4250 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/servicebus/events/client.py
--rw-r--r--   0        0        0       47 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/tablestorage/__init__.py
--rw-r--r--   0        0        0     2882 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/tablestorage/client.py
--rw-r--r--   0        0        0     2509 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/tablestorage/client_async.py
--rw-r--r--   0        0        0      521 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/tablestorage/helpers.py
--rw-r--r--   0        0        0     2470 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/tablestorage/operations.py
--rw-r--r--   0        0        0      219 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/testing/__init__.py
--rw-r--r--   0        0        0     2790 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/testing/assertions.py
--rw-r--r--   0        0        0     3499 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/testing/data.py
--rw-r--r--   0        0        0       19 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/transform/__init__.py
--rw-r--r--   0        0        0     1641 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/transform/data.py
--rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 warpzone_sdk-6.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1121 2023-05-25 13:24:56.626896 warpzone_sdk-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1182 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/__init__.py
+-rw-r--r--   0        0        0       21 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/blobstorage/__init__.py
+-rw-r--r--   0        0        0     2874 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/blobstorage/client.py
+-rw-r--r--   0        0        0       24 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/enums/__init__.py
+-rw-r--r--   0        0        0      213 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/enums/topicenum.py
+-rw-r--r--   0        0        0       27 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/__init__.py
+-rw-r--r--   0        0        0     1501 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/functionize.py
+-rw-r--r--   0        0        0     3035 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/integrations.py
+-rw-r--r--   0        0        0     2223 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/monitor.py
+-rw-r--r--   0        0        0     1486 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/process.py
+-rw-r--r--   0        0        0       32 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/processors/__init__.py
+-rw-r--r--   0        0        0     1910 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/processors/outputs.py
+-rw-r--r--   0        0        0     1727 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/processors/triggers.py
+-rw-r--r--   0        0        0     2268 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/signature.py
+-rw-r--r--   0        0        0       80 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/function/types.py
+-rw-r--r--   0        0        0     2108 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/healthchecks/__init__.py
+-rw-r--r--   0        0        0     1112 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/healthchecks/model.py
+-rw-r--r--   0        0        0       87 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/monitor/__init__.py
+-rw-r--r--   0        0        0     1650 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/monitor/logs.py
+-rw-r--r--   0        0        0     4781 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/monitor/traces.py
+-rw-r--r--   0        0        0       21 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/servicebus/data/__init__.py
+-rw-r--r--   0        0        0     5636 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/servicebus/data/client.py
+-rw-r--r--   0        0        0       21 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/servicebus/events/__init__.py
+-rw-r--r--   0        0        0     4250 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/servicebus/events/client.py
+-rw-r--r--   0        0        0       47 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/tablestorage/__init__.py
+-rw-r--r--   0        0        0     2882 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/tablestorage/client.py
+-rw-r--r--   0        0        0     2509 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/tablestorage/client_async.py
+-rw-r--r--   0        0        0      521 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/tablestorage/helpers.py
+-rw-r--r--   0        0        0     2470 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/tablestorage/operations.py
+-rw-r--r--   0        0        0      219 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/testing/__init__.py
+-rw-r--r--   0        0        0     2939 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/testing/assertions.py
+-rw-r--r--   0        0        0     3661 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/testing/data.py
+-rw-r--r--   0        0        0       27 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/transform/__init__.py
+-rw-r--r--   0        0        0     1641 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/transform/data.py
+-rw-r--r--   0        0        0     1833 2023-05-25 13:24:56.630896 warpzone_sdk-7.0.0/warpzone/transform/schema.py
+-rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 warpzone_sdk-7.0.0/PKG-INFO
```

### Comparing `warpzone_sdk-6.0.6/pyproject.toml` & `warpzone_sdk-7.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "warpzone-sdk"
-version = "6.0.6"
+version = "7.0.0"
 description = "The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage"
 authors = ["Anders Launer Baek-Petersen <alp@energinet.dk>", "Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "warpzone" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `warpzone_sdk-6.0.6/warpzone/__init__.py` & `warpzone_sdk-7.0.0/warpzone/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.6/warpzone/blobstorage/client.py` & `warpzone_sdk-7.0.0/warpzone/blobstorage/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.6/warpzone/function/functionize.py` & `warpzone_sdk-7.0.0/warpzone/function/functionize.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.6/warpzone/function/integrations.py` & `warpzone_sdk-7.0.0/warpzone/function/integrations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.6/warpzone/function/monitor.py` & `warpzone_sdk-7.0.0/warpzone/function/monitor.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.6/warpzone/function/process.py` & `warpzone_sdk-7.0.0/warpzone/function/process.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.6/warpzone/function/processors/outputs.py` & `warpzone_sdk-7.0.0/warpzone/function/processors/outputs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.6/warpzone/function/processors/triggers.py` & `warpzone_sdk-7.0.0/warpzone/function/processors/triggers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.6/warpzone/function/signature.py` & `warpzone_sdk-7.0.0/warpzone/function/signature.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.6/warpzone/healthchecks/__init__.py` & `warpzone_sdk-7.0.0/warpzone/healthchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.6/warpzone/healthchecks/model.py` & `warpzone_sdk-7.0.0/warpzone/healthchecks/model.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.6/warpzone/monitor/logs.py` & `warpzone_sdk-7.0.0/warpzone/monitor/logs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.6/warpzone/monitor/traces.py` & `warpzone_sdk-7.0.0/warpzone/monitor/traces.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.6/warpzone/servicebus/data/client.py` & `warpzone_sdk-7.0.0/warpzone/servicebus/data/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pandas as pd
 
 from warpzone.blobstorage.client import BlobData, WarpzoneBlobClient
 from warpzone.enums.topicenum import Topic
 from warpzone.healthchecks import HealthCheckResult, check_health_of
 from warpzone.servicebus.events.client import EventMessage, WarpzoneEventClient
 from warpzone.transform import data
+from warpzone.transform.schema import calculate_schema_version, dataframe_schema_recast
 
 DATA_CONTAINER_NAME = "messages"
 BLOB_NAME_PARAM = "blob_name"
 TIMESTAMP_PARAM = "timestamp"
 TIMESTAMP_FORMAT = "%Y-%m-%dT%H:%M:%S%z"
 
 
@@ -34,20 +35,24 @@
         )
 
     @classmethod
     def from_pandas(
         cls,
         df: pd.DataFrame,
         subject: str,
-        schema: dict = None,
+        schema: dict,
         message_id: str = None,
         metadata: dict = None,
         timestamp: Optional[dt.datetime] = None,
     ):
-        content = data.pandas_to_parquet(df, schema=schema)
+        if metadata is None:
+            metadata = {}
+        metadata["version"] = calculate_schema_version(schema)
+        df = dataframe_schema_recast(df, schema)
+        content = data.pandas_to_parquet(df)
         extension = "parquet"
         return cls(content, extension, subject, message_id, metadata, timestamp)
 
     def to_pandas(self) -> pd.DataFrame:
         return data.parquet_to_pandas(self.content)
```

### Comparing `warpzone_sdk-6.0.6/warpzone/servicebus/events/client.py` & `warpzone_sdk-7.0.0/warpzone/servicebus/events/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.6/warpzone/tablestorage/client.py` & `warpzone_sdk-7.0.0/warpzone/tablestorage/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.6/warpzone/tablestorage/client_async.py` & `warpzone_sdk-7.0.0/warpzone/tablestorage/client_async.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.6/warpzone/tablestorage/helpers.py` & `warpzone_sdk-7.0.0/warpzone/tablestorage/helpers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.6/warpzone/tablestorage/operations.py` & `warpzone_sdk-7.0.0/warpzone/tablestorage/operations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.6/warpzone/testing/assertions.py` & `warpzone_sdk-7.0.0/warpzone/testing/assertions.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,17 +50,19 @@
     if check_message_id:
         assert (
             left.message_id == right.message_id
         ), f"Message ids are different: {left.message_id} != {right.message_id}"
 
     if left.extension == "parquet":
         # for parquet files, check if the resulting pandas DataFrames are equal
+        left_pandas, right_pandas = left.to_pandas(), right.to_pandas()
         pd.testing.assert_frame_equal(
-            left=left.to_pandas(),
-            right=right.to_pandas(),
+            left=left_pandas,
+            right=right_pandas,
+            check_dtype=False if (left_pandas.empty and right_pandas.empty) else True,
         )
     elif left.extension == "json":
         # for json files, check if the parsed data is equal
         left_json, right_json = json.loads(left.content), json.loads(right.content)
         assert (
             left_json == right_json
         ), f"JSON is different: {left_json} != {right_json}"
```

### Comparing `warpzone_sdk-6.0.6/warpzone/testing/data.py` & `warpzone_sdk-7.0.0/warpzone/testing/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime as dt
 import os
 from pathlib import Path
 
 import pandas as pd
 
 from warpzone.servicebus.data.client import DataMessage
+from warpzone.transform.schema import generate_and_stringify_schema
 
 
 def get_filepath(filename: str, subfolder: str = "data"):
     return Path(os.environ["PYTEST_CURRENT_TEST"]).parent / subfolder / filename
 
 
 def parse_iso_datetime(values: pd.Series) -> pd.Series:
@@ -96,17 +97,20 @@
     message_id: str = None,
     metadata: dict = None,
     timestamp: dt.datetime = None,
     subfolder: str = "data",
 ) -> DataMessage:
     suffixes = Path(filename).suffixes
     if suffixes[0] == ".df":
+        df = read_pandas(filename, subfolder)
+        schema = generate_and_stringify_schema(df)
         return DataMessage.from_pandas(
-            df=read_pandas(filename, subfolder),
+            df=df,
             subject=subject,
+            schema=schema,
             message_id=message_id,
             metadata=metadata,
             timestamp=timestamp,
         )
     else:
         return DataMessage(
             content=read_bytes(filename, subfolder),
```

### Comparing `warpzone_sdk-6.0.6/warpzone/transform/data.py` & `warpzone_sdk-7.0.0/warpzone/transform/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.6/PKG-INFO` & `warpzone_sdk-7.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warpzone-sdk
-Version: 6.0.6
+Version: 7.0.0
 Summary: The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage
 Author: Anders Launer Baek-Petersen
 Author-email: alp@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

