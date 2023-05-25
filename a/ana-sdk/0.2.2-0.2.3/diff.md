# Comparing `tmp/ana_sdk-0.2.2.tar.gz` & `tmp/ana_sdk-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ana_sdk-0.2.2.tar", max compression
+gzip compressed data, was "ana_sdk-0.2.3.tar", max compression
```

## Comparing `ana_sdk-0.2.2.tar` & `ana_sdk-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.2.2/ana_sdk/__init__.py
--rw-r--r--   0        0        0    14685 2023-05-25 20:01:36.382463 ana_sdk-0.2.2/ana_sdk/ana.py
--rw-r--r--   0        0        0      177 2023-05-23 01:43:08.849263 ana_sdk-0.2.2/ana_sdk/clients/__init__.py
--rw-r--r--   0        0        0     4523 2023-05-23 02:57:33.535000 ana_sdk-0.2.2/ana_sdk/clients/ana_data_client.py
--rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.2.2/ana_sdk/clients/base_client.py
--rw-r--r--   0        0        0     4635 2023-05-23 01:51:45.997363 ana_sdk-0.2.2/ana_sdk/clients/dashboard_api_client.py
--rw-r--r--   0        0        0     1438 2023-05-23 03:23:45.283114 ana_sdk-0.2.2/ana_sdk/clients/oauth_client.py
--rw-r--r--   0        0        0     3320 2023-05-23 01:51:51.763464 ana_sdk-0.2.2/ana_sdk/clients/rpa_api_client.py
--rw-r--r--   0        0        0      333 2023-05-25 19:31:13.365688 ana_sdk-0.2.2/ana_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0     4162 2023-05-25 19:48:03.999218 ana_sdk-0.2.2/ana_sdk/result_factory.py
--rw-r--r--   0        0        0      463 2023-05-25 20:01:51.551945 ana_sdk-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.2.2/README.md
--rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.2.3/ana_sdk/__init__.py
+-rw-r--r--   0        0        0    14685 2023-05-25 20:01:36.382463 ana_sdk-0.2.3/ana_sdk/ana.py
+-rw-r--r--   0        0        0      177 2023-05-23 01:43:08.849263 ana_sdk-0.2.3/ana_sdk/clients/__init__.py
+-rw-r--r--   0        0        0     4523 2023-05-23 02:57:33.535000 ana_sdk-0.2.3/ana_sdk/clients/ana_data_client.py
+-rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.2.3/ana_sdk/clients/base_client.py
+-rw-r--r--   0        0        0     4635 2023-05-23 01:51:45.997363 ana_sdk-0.2.3/ana_sdk/clients/dashboard_api_client.py
+-rw-r--r--   0        0        0     1438 2023-05-23 03:23:45.283114 ana_sdk-0.2.3/ana_sdk/clients/oauth_client.py
+-rw-r--r--   0        0        0     3320 2023-05-23 01:51:51.763464 ana_sdk-0.2.3/ana_sdk/clients/rpa_api_client.py
+-rw-r--r--   0        0        0      744 2023-05-25 20:23:48.737805 ana_sdk-0.2.3/ana_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0     4340 2023-05-25 20:25:09.531740 ana_sdk-0.2.3/ana_sdk/result_factory.py
+-rw-r--r--   0        0        0      463 2023-05-25 20:25:29.635977 ana_sdk-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.2.3/README.md
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.2.3/PKG-INFO
```

### Comparing `ana_sdk-0.2.2/ana_sdk/ana.py` & `ana_sdk-0.2.3/ana_sdk/ana.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.2/ana_sdk/clients/ana_data_client.py` & `ana_sdk-0.2.3/ana_sdk/clients/ana_data_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.2/ana_sdk/clients/base_client.py` & `ana_sdk-0.2.3/ana_sdk/clients/base_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.2/ana_sdk/clients/dashboard_api_client.py` & `ana_sdk-0.2.3/ana_sdk/clients/dashboard_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.2/ana_sdk/clients/oauth_client.py` & `ana_sdk-0.2.3/ana_sdk/clients/oauth_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.2/ana_sdk/clients/rpa_api_client.py` & `ana_sdk-0.2.3/ana_sdk/clients/rpa_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.2/ana_sdk/result_factory.py` & `ana_sdk-0.2.3/ana_sdk/result_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from __future__ import annotations
 
 from abc import ABC
 from pathlib import Path
 
 import requests
 
-from .exceptions import ResultNotFoundError, NoResultHandlerImplementedError
+from .exceptions import (
+    ResultNotFoundError,
+    NoResultHandlerImplementedError,
+    TaskError,
+)
 
 
 class AbstractResultHandler(ABC):
     """
     Classe abstrata utilizada como interface para todos os manipuladores
     de resultado.
     """
@@ -134,14 +138,17 @@
         """
 
         result: dict = task_info.get("result")
         if not result:
             raise ResultNotFoundError()
         
         data: dict = result.get("data")
-
+        status: str = result.get("status")
+        if status in ("ERROR", "FAILURE"):
+            raise TaskError(result.get("error"))
+        
         if data and data.get("file"):
             return Report(result)
         elif data and data.get("response"):
             return Task(result)
         else:
             raise NoResultHandlerImplementedError()
```

### Comparing `ana_sdk-0.2.2/README.md` & `ana_sdk-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.2/PKG-INFO` & `ana_sdk-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ana-sdk
-Version: 0.2.2
+Version: 0.2.3
 Summary: SDK que visa fornecer uma interface para interagir com os serviços ANA.
 License: MIT
 Author: Jovane Mafort
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

