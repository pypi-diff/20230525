# Comparing `tmp/turbine-py-2.0.0.tar.gz` & `tmp/turbine-py-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbine-py-2.0.0.tar", last modified: Thu May 18 20:11:23 2023, max compression
+gzip compressed data, was "turbine-py-2.1.0.tar", last modified: Thu May 25 15:15:50 2023, max compression
```

## Comparing `turbine-py-2.0.0.tar` & `turbine-py-2.1.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.472128 turbine-py-2.0.0/
--rw-r--r--   0 root         (0) root         (0)      168 2023-05-18 20:11:11.000000 turbine-py-2.0.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      142 2023-05-18 20:11:11.000000 turbine-py-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8663 2023-05-18 20:11:23.472128 turbine-py-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8098 2023-05-18 20:11:11.000000 turbine-py-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.460128 turbine-py-2.0.0/pkg/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.460128 turbine-py-2.0.0/pkg/turbine/
--rw-r--r--   0 root         (0) root         (0)      125 2023-05-18 20:11:12.000000 turbine-py-2.0.0/pkg/turbine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2206 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.460128 turbine-py-2.0.0/pkg/turbine/src/
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.464128 turbine-py-2.0.0/pkg/turbine/src/function_deploy/
--rw-r--r--   0 root         (0) root         (0)      324 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/Dockerfile
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.464128 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/
--rw-r--r--   0 root         (0) root         (0)     2460 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/README.md
--rw-r--r--   0 root         (0) root         (0)      287 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3048 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/function_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.464128 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/proto_gen/
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/proto_gen/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1705 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2504 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/record.py
--rw-r--r--   0 root         (0) root         (0)      189 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.468128 turbine-py-2.0.0/pkg/turbine/src/turbine_app/
--rw-r--r--   0 root         (0) root         (0)      425 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1345 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/app.py
--rw-r--r--   0 root         (0) root         (0)     2293 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.468128 turbine-py-2.0.0/pkg/turbine/src/turbine_app/proto_gen/
--rw-r--r--   0 root         (0) root         (0)      816 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/proto_gen/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5680 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/proto_gen/turbine_pb2.py
--rw-r--r--   0 root         (0) root         (0)    15253 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/proto_gen/turbine_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    13062 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/proto_gen/validate_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/proto_gen/validate_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/resource.py
--rw-r--r--   0 root         (0) root         (0)     2052 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/types.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.472128 turbine-py-2.0.0/pkg/turbine_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8663 2023-05-18 20:11:23.000000 turbine-py-2.0.0/pkg/turbine_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1527 2023-05-18 20:11:23.000000 turbine-py-2.0.0/pkg/turbine_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:11:23.000000 turbine-py-2.0.0/pkg/turbine_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-18 20:11:23.000000 turbine-py-2.0.0/pkg/turbine_py.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      170 2023-05-18 20:11:23.000000 turbine-py-2.0.0/pkg/turbine_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-18 20:11:23.000000 turbine-py-2.0.0/pkg/turbine_py.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      361 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1278 2023-05-18 20:11:23.472128 turbine-py-2.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.472128 turbine-py-2.0.0/tests/
--rw-r--r--   0 root         (0) root         (0)     1849 2023-05-18 20:11:11.000000 turbine-py-2.0.0/tests/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:15:50.544363 turbine-py-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-05-25 15:15:38.000000 turbine-py-2.1.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      142 2023-05-25 15:15:38.000000 turbine-py-2.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8669 2023-05-25 15:15:50.544363 turbine-py-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8104 2023-05-25 15:15:38.000000 turbine-py-2.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:15:50.532363 turbine-py-2.1.0/pkg/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:15:50.532363 turbine-py-2.1.0/pkg/turbine/
+-rw-r--r--   0 root         (0) root         (0)      125 2023-05-25 15:15:39.000000 turbine-py-2.1.0/pkg/turbine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2206 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:15:50.532363 turbine-py-2.1.0/pkg/turbine/src/
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:15:50.532363 turbine-py-2.1.0/pkg/turbine/src/function_deploy/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/function_deploy/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/function_deploy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:15:50.536363 turbine-py-2.1.0/pkg/turbine/src/function_deploy/function_app/
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/function_deploy/function_app/README.md
+-rw-r--r--   0 root         (0) root         (0)      287 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/function_deploy/function_app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3048 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/function_deploy/function_app/function_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:15:50.536363 turbine-py-2.1.0/pkg/turbine/src/function_deploy/function_app/proto_gen/
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/function_deploy/function_app/proto_gen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2504 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/function_deploy/function_app/record.py
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/function_deploy/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:15:50.540363 turbine-py-2.1.0/pkg/turbine/src/turbine_app/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/turbine_app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1345 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/turbine_app/app.py
+-rw-r--r--   0 root         (0) root         (0)     2293 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/turbine_app/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:15:50.540363 turbine-py-2.1.0/pkg/turbine/src/turbine_app/proto_gen/
+-rw-r--r--   0 root         (0) root         (0)      816 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/turbine_app/proto_gen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/turbine_app/proto_gen/turbine_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    15253 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/turbine_app/proto_gen/turbine_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    13062 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/turbine_app/proto_gen/validate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/turbine_app/proto_gen/validate_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/turbine_app/resource.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/turbine_app/types.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pkg/turbine/src/turbine_app/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:15:50.544363 turbine-py-2.1.0/pkg/turbine_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8669 2023-05-25 15:15:50.000000 turbine-py-2.1.0/pkg/turbine_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-05-25 15:15:50.000000 turbine-py-2.1.0/pkg/turbine_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 15:15:50.000000 turbine-py-2.1.0/pkg/turbine_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-25 15:15:50.000000 turbine-py-2.1.0/pkg/turbine_py.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-25 15:15:50.000000 turbine-py-2.1.0/pkg/turbine_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-25 15:15:50.000000 turbine-py-2.1.0/pkg/turbine_py.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      361 2023-05-25 15:15:38.000000 turbine-py-2.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-05-25 15:15:50.544363 turbine-py-2.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:15:50.544363 turbine-py-2.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-05-25 15:15:38.000000 turbine-py-2.1.0/tests/test_cli.py
```

### Comparing `turbine-py-2.0.0/PKG-INFO` & `turbine-py-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbine-py
-Version: 2.0.0
+Version: 2.1.0
 Summary: Meroxa Turbine data application framework
 Home-page: https://meroxa.io/
 Author: Eric Cheatham
 Author-email: eric@meroxa.io
 License: MIT
 Project-URL: Source Code, https://github.com/meroxa/turbine-py/
 Project-URL: Issue Tracker, https://github.com/meroxa/turbine-py/issues
@@ -74,15 +74,15 @@
 This configuration file is where you begin your Turbine journey. Any time a Turbine app runs, this is the entry point for the entire application. When the project is created, the file will look like this:
 
 ```python
 # Dependencies of the example data app
 import hashlib
 import sys
 
-from turbine.runtime import RecordList, Runtime as Turbine
+from turbine.src.turbine_app import RecordList, TurbineApp
 
 def anonymize(records: RecordList) -> RecordList:
     for record in records:
         try:
             payload = record.value["payload"]
 
             # Hash the email
@@ -93,15 +93,15 @@
         except Exception as e:
             print("Error occurred while parsing records: " + str(e))
     return records
 
 
 class App:
     @staticmethod
-    async def run(turbine: Turbine):
+    async def run(turbine: TurbineApp):
       try:
         source = await turbine.resources("source_name")
 
         records = await source.records("collection_name")
 
         anonymized = await turbine.process(records, anonymize)
 
@@ -111,15 +111,15 @@
       except Exception as e:
           print(e, file=sys.stderr)
 ```
 
 Let's talk about the important parts of this code. Turbine apps have five functions that comprise the entire DSL. Outside of these functions, you can write whatever code you want to accomplish your tasks:
 
 ```python
-async def run(turbine: Turbine):
+async def run(turbine: TurbineApp):
 ```
 
 `run` is the main entry point for the application. This is where you can initialize the Turbine framework. This is also the place where, when you deploy your Turbine app to Meroxa, Meroxa will use this as the place to boot up the application.
 
 ```python
 source = await turbine.resources("source_name")
 ```
```

### Comparing `turbine-py-2.0.0/README.md` & `turbine-py-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 This configuration file is where you begin your Turbine journey. Any time a Turbine app runs, this is the entry point for the entire application. When the project is created, the file will look like this:
 
 ```python
 # Dependencies of the example data app
 import hashlib
 import sys
 
-from turbine.runtime import RecordList, Runtime as Turbine
+from turbine.src.turbine_app import RecordList, TurbineApp
 
 def anonymize(records: RecordList) -> RecordList:
     for record in records:
         try:
             payload = record.value["payload"]
 
             # Hash the email
@@ -76,15 +76,15 @@
         except Exception as e:
             print("Error occurred while parsing records: " + str(e))
     return records
 
 
 class App:
     @staticmethod
-    async def run(turbine: Turbine):
+    async def run(turbine: TurbineApp):
       try:
         source = await turbine.resources("source_name")
 
         records = await source.records("collection_name")
 
         anonymized = await turbine.process(records, anonymize)
 
@@ -94,15 +94,15 @@
       except Exception as e:
           print(e, file=sys.stderr)
 ```
 
 Let's talk about the important parts of this code. Turbine apps have five functions that comprise the entire DSL. Outside of these functions, you can write whatever code you want to accomplish your tasks:
 
 ```python
-async def run(turbine: Turbine):
+async def run(turbine: TurbineApp):
 ```
 
 `run` is the main entry point for the application. This is where you can initialize the Turbine framework. This is also the place where, when you deploy your Turbine app to Meroxa, Meroxa will use this as the place to boot up the application.
 
 ```python
 source = await turbine.resources("source_name")
 ```
```

### Comparing `turbine-py-2.0.0/pkg/turbine/cli.py` & `turbine-py-2.1.0/pkg/turbine/cli.py`

 * *Files identical despite different names*

### Comparing `turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/README.md` & `turbine-py-2.1.0/pkg/turbine/src/function_deploy/function_app/README.md`

 * *Files identical despite different names*

### Comparing `turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/function_server.py` & `turbine-py-2.1.0/pkg/turbine/src/function_deploy/function_app/function_server.py`

 * *Files identical despite different names*

### Comparing `turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2.py` & `turbine-py-2.1.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2.py`

 * *Files identical despite different names*

### Comparing `turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2.pyi` & `turbine-py-2.1.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2_grpc.py` & `turbine-py-2.1.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/record.py` & `turbine-py-2.1.0/pkg/turbine/src/function_deploy/function_app/record.py`

 * *Files identical despite different names*

### Comparing `turbine-py-2.0.0/pkg/turbine/src/turbine_app/app.py` & `turbine-py-2.1.0/pkg/turbine/src/turbine_app/app.py`

 * *Files identical despite different names*

### Comparing `turbine-py-2.0.0/pkg/turbine/src/turbine_app/client.py` & `turbine-py-2.1.0/pkg/turbine/src/turbine_app/client.py`

 * *Files identical despite different names*

### Comparing `turbine-py-2.0.0/pkg/turbine/src/turbine_app/proto_gen/__init__.py` & `turbine-py-2.1.0/pkg/turbine/src/turbine_app/proto_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `turbine-py-2.0.0/pkg/turbine/src/turbine_app/proto_gen/turbine_pb2.py` & `turbine-py-2.1.0/pkg/turbine/src/turbine_app/proto_gen/turbine_pb2.py`

 * *Files identical despite different names*

### Comparing `turbine-py-2.0.0/pkg/turbine/src/turbine_app/proto_gen/turbine_pb2_grpc.py` & `turbine-py-2.1.0/pkg/turbine/src/turbine_app/proto_gen/turbine_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `turbine-py-2.0.0/pkg/turbine/src/turbine_app/proto_gen/validate_pb2.py` & `turbine-py-2.1.0/pkg/turbine/src/turbine_app/proto_gen/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `turbine-py-2.0.0/pkg/turbine/src/turbine_app/resource.py` & `turbine-py-2.1.0/pkg/turbine/src/turbine_app/resource.py`

 * *Files identical despite different names*

### Comparing `turbine-py-2.0.0/pkg/turbine/src/turbine_app/types.py` & `turbine-py-2.1.0/pkg/turbine/src/turbine_app/types.py`

 * *Files identical despite different names*

### Comparing `turbine-py-2.0.0/pkg/turbine/src/turbine_app/utils.py` & `turbine-py-2.1.0/pkg/turbine/src/turbine_app/utils.py`

 * *Files identical despite different names*

### Comparing `turbine-py-2.0.0/pkg/turbine_py.egg-info/PKG-INFO` & `turbine-py-2.1.0/pkg/turbine_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbine-py
-Version: 2.0.0
+Version: 2.1.0
 Summary: Meroxa Turbine data application framework
 Home-page: https://meroxa.io/
 Author: Eric Cheatham
 Author-email: eric@meroxa.io
 License: MIT
 Project-URL: Source Code, https://github.com/meroxa/turbine-py/
 Project-URL: Issue Tracker, https://github.com/meroxa/turbine-py/issues
@@ -74,15 +74,15 @@
 This configuration file is where you begin your Turbine journey. Any time a Turbine app runs, this is the entry point for the entire application. When the project is created, the file will look like this:
 
 ```python
 # Dependencies of the example data app
 import hashlib
 import sys
 
-from turbine.runtime import RecordList, Runtime as Turbine
+from turbine.src.turbine_app import RecordList, TurbineApp
 
 def anonymize(records: RecordList) -> RecordList:
     for record in records:
         try:
             payload = record.value["payload"]
 
             # Hash the email
@@ -93,15 +93,15 @@
         except Exception as e:
             print("Error occurred while parsing records: " + str(e))
     return records
 
 
 class App:
     @staticmethod
-    async def run(turbine: Turbine):
+    async def run(turbine: TurbineApp):
       try:
         source = await turbine.resources("source_name")
 
         records = await source.records("collection_name")
 
         anonymized = await turbine.process(records, anonymize)
 
@@ -111,15 +111,15 @@
       except Exception as e:
           print(e, file=sys.stderr)
 ```
 
 Let's talk about the important parts of this code. Turbine apps have five functions that comprise the entire DSL. Outside of these functions, you can write whatever code you want to accomplish your tasks:
 
 ```python
-async def run(turbine: Turbine):
+async def run(turbine: TurbineApp):
 ```
 
 `run` is the main entry point for the application. This is where you can initialize the Turbine framework. This is also the place where, when you deploy your Turbine app to Meroxa, Meroxa will use this as the place to boot up the application.
 
 ```python
 source = await turbine.resources("source_name")
 ```
```

### Comparing `turbine-py-2.0.0/pkg/turbine_py.egg-info/SOURCES.txt` & `turbine-py-2.1.0/pkg/turbine_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `turbine-py-2.0.0/setup.cfg` & `turbine-py-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `turbine-py-2.0.0/tests/test_cli.py` & `turbine-py-2.1.0/tests/test_cli.py`

 * *Files identical despite different names*

