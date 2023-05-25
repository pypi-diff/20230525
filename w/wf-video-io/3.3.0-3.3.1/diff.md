# Comparing `tmp/wf_video_io-3.3.0.tar.gz` & `tmp/wf_video_io-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf_video_io-3.3.0.tar", max compression
+gzip compressed data, was "wf_video_io-3.3.1.tar", max compression
```

## Comparing `wf_video_io-3.3.0.tar` & `wf_video_io-3.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0     1088 2022-07-13 02:25:51.284383 wf_video_io-3.3.0/LICENSE
--rwxr-xr-x   0        0        0      278 2023-01-27 16:56:30.309581 wf_video_io-3.3.0/README.md
--rw-r--r--   0        0        0     1162 2023-05-24 18:48:33.803582 wf_video_io-3.3.0/pyproject.toml
--rwxr-xr-x   0        0        0       28 2022-07-13 02:25:51.323025 wf_video_io-3.3.0/video_io/__init__.py
--rw-r--r--   0        0        0       37 2022-10-13 19:42:09.408938 wf_video_io-3.3.0/video_io/client/__init__.py
--rwxr-xr-x   0        0        0    15566 2023-05-24 18:27:45.399757 wf_video_io-3.3.0/video_io/client/core.py
--rw-r--r--   0        0        0      265 2023-05-15 17:34:04.808749 wf_video_io-3.3.0/video_io/client/errors.py
--rw-r--r--   0        0        0     3385 2023-05-24 18:36:26.987342 wf_video_io-3.3.0/video_io/client/utils.py
--rw-r--r--   0        0        0     1742 2023-05-15 17:34:04.821553 wf_video_io-3.3.0/video_io/config.py
--rwxr-xr-x   0        0        0    47659 2023-05-15 17:34:04.959430 wf_video_io-3.3.0/video_io/core.py
--rw-r--r--   0        0        0      382 2023-05-15 17:34:04.811182 wf_video_io-3.3.0/video_io/log_retry.py
--rw-r--r--   0        0        0    10067 2023-05-15 17:34:04.860739 wf_video_io-3.3.0/video_io/utils.py
--rw-r--r--   0        0        0      585 2023-01-27 16:56:30.326420 wf_video_io-3.3.0/video_io/video_reader.py
--rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 wf_video_io-3.3.0/setup.py
--rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 wf_video_io-3.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1088 2022-07-13 02:25:51.284383 wf_video_io-3.3.1/LICENSE
+-rwxr-xr-x   0        0        0      278 2023-01-27 16:56:30.309581 wf_video_io-3.3.1/README.md
+-rw-r--r--   0        0        0     1162 2023-05-25 15:19:43.551183 wf_video_io-3.3.1/pyproject.toml
+-rwxr-xr-x   0        0        0       28 2022-07-13 02:25:51.323025 wf_video_io-3.3.1/video_io/__init__.py
+-rw-r--r--   0        0        0       37 2022-10-13 19:42:09.408938 wf_video_io-3.3.1/video_io/client/__init__.py
+-rwxr-xr-x   0        0        0    16067 2023-05-25 15:18:54.994835 wf_video_io-3.3.1/video_io/client/core.py
+-rw-r--r--   0        0        0      265 2023-05-15 17:34:04.808749 wf_video_io-3.3.1/video_io/client/errors.py
+-rw-r--r--   0        0        0     3385 2023-05-24 18:36:26.987342 wf_video_io-3.3.1/video_io/client/utils.py
+-rw-r--r--   0        0        0     1742 2023-05-15 17:34:04.821553 wf_video_io-3.3.1/video_io/config.py
+-rwxr-xr-x   0        0        0    47659 2023-05-15 17:34:04.959430 wf_video_io-3.3.1/video_io/core.py
+-rw-r--r--   0        0        0      382 2023-05-15 17:34:04.811182 wf_video_io-3.3.1/video_io/log_retry.py
+-rw-r--r--   0        0        0    10067 2023-05-15 17:34:04.860739 wf_video_io-3.3.1/video_io/utils.py
+-rw-r--r--   0        0        0      585 2023-01-27 16:56:30.326420 wf_video_io-3.3.1/video_io/video_reader.py
+-rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 wf_video_io-3.3.1/setup.py
+-rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 wf_video_io-3.3.1/PKG-INFO
```

### Comparing `wf_video_io-3.3.0/LICENSE` & `wf_video_io-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.0/pyproject.toml` & `wf_video_io-3.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "wf-video-io"
 dynamic = ["version"]
 
 [tool.poetry]
 name = "wf-video-io"
-version = "3.3.0"
+version = "3.3.1"
 description = "Library for working with video files and interacting with the wildflower video-service"
 authors = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>"]
 maintainers = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>", "Benjamin Jaffe-Talberg <ben.talberg@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "video_io"}]
```

### Comparing `wf_video_io-3.3.0/video_io/client/core.py` & `wf_video_io-3.3.1/video_io/client/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 from pathlib import Path
 from typing import List, Dict
 
 from cachetools import TTLCache
 import requests
 from requests.adapters import HTTPAdapter
+from typing import Optional
 import yaml
 
 import video_io.config
 from video_io.log_retry import LogRetry
 from video_io.client.errors import SyncError
 from video_io.client.utils import (
     client_token,
@@ -25,23 +26,26 @@
 )
 
 
 logger = logging.getLogger(__name__)
 
 
 class VideoStorageClient:
+    DEFAULT_CONNECTION_POOL_SIZE = 10
+
     def __init__(
         self,
         token=None,
         cache_directory=video_io.config.VIDEO_STORAGE_LOCAL_CACHE_DIRECTORY,
         url=video_io.config.VIDEO_STORAGE_URL,
         auth_domain=video_io.config.VIDEO_STORAGE_AUTH_DOMAIN,
         audience=video_io.config.VIDEO_STORAGE_AUDIENCE,
         client_id=video_io.config.VIDEO_STORAGE_CLIENT_ID,
         client_secret=video_io.config.HONEYCOMB_CLIENT_SECRET,
+        connection_pool_size: Optional[int] = None
     ):
         self.CACHE_DIRECTORY = cache_directory
         self.URL = url
 
         self.auth_domain = auth_domain
         self.audience = audience
         self.client_id = client_id
@@ -49,25 +53,31 @@
 
         self.headers = {}  # {"Content-Type": "application/json"}
 
         self.tokens = {}
         if token is not None:
             self.tokens["access_token"] = token
 
-        self.request_session = self.init_request_session()
+        self.request_session = self.init_request_session(connection_pool_size=connection_pool_size)
 
     @staticmethod
-    def init_request_session():
+    def init_request_session(connection_pool_size=None):
         retry_strategy = LogRetry(
             total=6,
             status_forcelist=[429, 500, 502, 503, 504],
             method_whitelist=["HEAD", "GET", "OPTIONS", "POST"],
             backoff_factor=0.5,
         )
-        adapter = HTTPAdapter(max_retries=retry_strategy)
+        _connection_pool_size = connection_pool_size
+        if _connection_pool_size is None:
+            _connection_pool_size = VideoStorageClient.DEFAULT_CONNECTION_POOL_SIZE
+
+        adapter = HTTPAdapter(max_retries=retry_strategy,
+                              pool_connections=_connection_pool_size,
+                              pool_maxsize=_connection_pool_size)
         request_session = requests.Session()
         request_session.mount("https://", adapter)
         request_session.mount("http://", adapter)
         return request_session
 
     def refresh_token(self):
         try:
@@ -219,18 +229,18 @@
                 start_date,
                 end_date,
                 e,
             )
             raise e
 
     async def upload_video(self, path: str, local_cache_directory: str = None):
-        response = await self.upload_videos(path=[path], local_cache_directory=local_cache_directory)
+        response = await self.upload_videos(paths=[path], local_cache_directory=local_cache_directory)
         return response[0]
 
-    async def upload_videos(self, paths: list[str], local_cache_directory: str = None):
+    async def upload_videos(self, paths: List[str], local_cache_directory: str = None):
         if local_cache_directory is None:
             local_cache_directory = self.CACHE_DIRECTORY
 
         all_results: list[None, dict] = [None] * len(paths)
         all_file_details: list[dict] = []
         for ii, path in enumerate(paths):
             full_path = local_cache_directory / path
```

### Comparing `wf_video_io-3.3.0/video_io/client/utils.py` & `wf_video_io-3.3.1/video_io/client/utils.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.0/video_io/config.py` & `wf_video_io-3.3.1/video_io/config.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.0/video_io/core.py` & `wf_video_io-3.3.1/video_io/core.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.0/video_io/utils.py` & `wf_video_io-3.3.1/video_io/utils.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.0/video_io/video_reader.py` & `wf_video_io-3.3.1/video_io/video_reader.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.0/setup.py` & `wf_video_io-3.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'wf-cv-utils>=3.4.0',
  'wf-fastapi-auth0>=1.0',
  'wf-gqlpycgen>=0.7.4,<0.8.0',
  'wf-honeycomb-io>=2.0.0']
 
 setup_kwargs = {
     'name': 'wf-video-io',
-    'version': '3.3.0',
+    'version': '3.3.1',
     'description': 'Library for working with video files and interacting with the wildflower video-service',
     'long_description': '# video_io\n\nTools for accessing Wildflower video data\n\n## Test\n\nTests are written with *behave* and *pytest*. As of 11/10/2022, *behave* tests are not functional.\n\n__Run pytest tests__\n\n```pytest```\n\n## Task list\n* ~~Add ability to request concatenation of videos~~ (11/7/2022)\n',
     'author': 'Paul J DeCoursey',
     'author_email': 'paul@decoursey.net',
     'maintainer': 'Paul J DeCoursey',
     'maintainer_email': 'paul@decoursey.net',
     'url': 'None',
```

### Comparing `wf_video_io-3.3.0/PKG-INFO` & `wf_video_io-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-video-io
-Version: 3.3.0
+Version: 3.3.1
 Summary: Library for working with video files and interacting with the wildflower video-service
 License: MIT
 Author: Paul J DeCoursey
 Author-email: paul@decoursey.net
 Maintainer: Paul J DeCoursey
 Maintainer-email: paul@decoursey.net
 Requires-Python: >=3.8,<3.12
```

