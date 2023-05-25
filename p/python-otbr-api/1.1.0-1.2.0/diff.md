# Comparing `tmp/python-otbr-api-1.1.0.tar.gz` & `tmp/python-otbr-api-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-otbr-api-1.1.0.tar", last modified: Wed May 10 18:04:51 2023, max compression
+gzip compressed data, was "python-otbr-api-1.2.0.tar", last modified: Thu May 25 07:56:15 2023, max compression
```

## Comparing `python-otbr-api-1.1.0.tar` & `python-otbr-api-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:04:51.804274 python-otbr-api-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-10 18:04:30.000000 python-otbr-api-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-10 18:04:51.804274 python-otbr-api-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-10 18:04:30.000000 python-otbr-api-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-10 18:04:30.000000 python-otbr-api-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:04:51.804274 python-otbr-api-1.1.0/python_otbr_api/
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-05-10 18:04:30.000000 python-otbr-api-1.1.0/python_otbr_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-10 18:04:30.000000 python-otbr-api-1.1.0/python_otbr_api/mdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-10 18:04:30.000000 python-otbr-api-1.1.0/python_otbr_api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-10 18:04:30.000000 python-otbr-api-1.1.0/python_otbr_api/pskc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:04:30.000000 python-otbr-api-1.1.0/python_otbr_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-10 18:04:30.000000 python-otbr-api-1.1.0/python_otbr_api/tlv_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:04:51.804274 python-otbr-api-1.1.0/python_otbr_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-10 18:04:51.000000 python-otbr-api-1.1.0/python_otbr_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-10 18:04:51.000000 python-otbr-api-1.1.0/python_otbr_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:04:51.000000 python-otbr-api-1.1.0/python_otbr_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 18:04:51.000000 python-otbr-api-1.1.0/python_otbr_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 18:04:51.000000 python-otbr-api-1.1.0/python_otbr_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:04:51.000000 python-otbr-api-1.1.0/python_otbr_api.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-10 18:04:51.804274 python-otbr-api-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:56:15.204285 python-otbr-api-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-25 07:55:54.000000 python-otbr-api-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 07:56:15.204285 python-otbr-api-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 07:55:54.000000 python-otbr-api-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-25 07:55:54.000000 python-otbr-api-1.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:56:15.200285 python-otbr-api-1.2.0/python_otbr_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-25 07:55:54.000000 python-otbr-api-1.2.0/python_otbr_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-25 07:55:54.000000 python-otbr-api-1.2.0/python_otbr_api/mdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-25 07:55:54.000000 python-otbr-api-1.2.0/python_otbr_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-25 07:55:54.000000 python-otbr-api-1.2.0/python_otbr_api/pskc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:55:54.000000 python-otbr-api-1.2.0/python_otbr_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-25 07:55:54.000000 python-otbr-api-1.2.0/python_otbr_api/tlv_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:56:15.204285 python-otbr-api-1.2.0/python_otbr_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 07:56:15.000000 python-otbr-api-1.2.0/python_otbr_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-25 07:56:15.000000 python-otbr-api-1.2.0/python_otbr_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:56:15.000000 python-otbr-api-1.2.0/python_otbr_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 07:56:15.000000 python-otbr-api-1.2.0/python_otbr_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 07:56:15.000000 python-otbr-api-1.2.0/python_otbr_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:56:14.000000 python-otbr-api-1.2.0/python_otbr_api.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-25 07:56:15.204285 python-otbr-api-1.2.0/setup.cfg
```

### Comparing `python-otbr-api-1.1.0/LICENSE` & `python-otbr-api-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-otbr-api-1.1.0/pyproject.toml` & `python-otbr-api-1.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=65.6", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name         = "python-otbr-api"
-version      = "1.1.0"
+version      = "1.2.0"
 license      = {text = "MIT"}
 description  = "API to interact with an OTBR via its REST API"
 readme       = "README.md"
 authors      = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
 requires-python = ">=3.9.0"
```

### Comparing `python-otbr-api-1.1.0/python_otbr_api/__init__.py` & `python-otbr-api-1.2.0/python_otbr_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,17 @@
         )
 
         if response.status == HTTPStatus.CONFLICT:
             raise ThreadNetworkActiveError
         if response.status != HTTPStatus.ACCEPTED:
             raise OTBRError(f"unexpected http status {response.status}")
 
-    async def set_channel(self, channel: int) -> None:
+    async def set_channel(
+        self, channel: int, delay: int = PENDING_DATASET_DELAY_TIMER
+    ) -> None:
         """Change the channel
 
         The channel is changed by creating a new pending dataset based on the active
         dataset.
         """
         if not 11 <= channel <= 26:
             raise OTBRError(f"invalid channel {channel}")
@@ -158,15 +160,15 @@
             raise OTBRError("router has no active dataset")
 
         if dataset.active_timestamp and dataset.active_timestamp.seconds is not None:
             dataset.active_timestamp.seconds += 1
         else:
             dataset.active_timestamp = Timestamp(False, 1, 0)
         dataset.channel = channel
-        dataset.delay = PENDING_DATASET_DELAY_TIMER
+        dataset.delay = delay
 
         await self.create_pending_dataset(dataset)
 
     async def get_extended_address(self) -> bytes:
         """Get extended address (EUI-64).
 
         Raises if the http status is not 200 or if the response is invalid.
```

### Comparing `python-otbr-api-1.1.0/python_otbr_api/mdns.py` & `python-otbr-api-1.2.0/python_otbr_api/mdns.py`

 * *Files identical despite different names*

### Comparing `python-otbr-api-1.1.0/python_otbr_api/models.py` & `python-otbr-api-1.2.0/python_otbr_api/models.py`

 * *Files identical despite different names*

### Comparing `python-otbr-api-1.1.0/python_otbr_api/pskc.py` & `python-otbr-api-1.2.0/python_otbr_api/pskc.py`

 * *Files identical despite different names*

### Comparing `python-otbr-api-1.1.0/python_otbr_api/tlv_parser.py` & `python-otbr-api-1.2.0/python_otbr_api/tlv_parser.py`

 * *Files identical despite different names*

