# Comparing `tmp/wf_video_io-3.3.1.tar.gz` & `tmp/wf_video_io-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf_video_io-3.3.1.tar", max compression
+gzip compressed data, was "wf_video_io-3.3.2.tar", max compression
```

## Comparing `wf_video_io-3.3.1.tar` & `wf_video_io-3.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0     1088 2022-07-13 02:25:51.284383 wf_video_io-3.3.1/LICENSE
--rwxr-xr-x   0        0        0      278 2023-01-27 16:56:30.309581 wf_video_io-3.3.1/README.md
--rw-r--r--   0        0        0     1162 2023-05-25 15:19:43.551183 wf_video_io-3.3.1/pyproject.toml
--rwxr-xr-x   0        0        0       28 2022-07-13 02:25:51.323025 wf_video_io-3.3.1/video_io/__init__.py
--rw-r--r--   0        0        0       37 2022-10-13 19:42:09.408938 wf_video_io-3.3.1/video_io/client/__init__.py
--rwxr-xr-x   0        0        0    16067 2023-05-25 15:18:54.994835 wf_video_io-3.3.1/video_io/client/core.py
--rw-r--r--   0        0        0      265 2023-05-15 17:34:04.808749 wf_video_io-3.3.1/video_io/client/errors.py
--rw-r--r--   0        0        0     3385 2023-05-24 18:36:26.987342 wf_video_io-3.3.1/video_io/client/utils.py
--rw-r--r--   0        0        0     1742 2023-05-15 17:34:04.821553 wf_video_io-3.3.1/video_io/config.py
--rwxr-xr-x   0        0        0    47659 2023-05-15 17:34:04.959430 wf_video_io-3.3.1/video_io/core.py
--rw-r--r--   0        0        0      382 2023-05-15 17:34:04.811182 wf_video_io-3.3.1/video_io/log_retry.py
--rw-r--r--   0        0        0    10067 2023-05-15 17:34:04.860739 wf_video_io-3.3.1/video_io/utils.py
--rw-r--r--   0        0        0      585 2023-01-27 16:56:30.326420 wf_video_io-3.3.1/video_io/video_reader.py
--rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 wf_video_io-3.3.1/setup.py
--rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 wf_video_io-3.3.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1088 2022-07-13 02:25:51.284383 wf_video_io-3.3.2/LICENSE
+-rwxr-xr-x   0        0        0      278 2023-01-27 16:56:30.309581 wf_video_io-3.3.2/README.md
+-rw-r--r--   0        0        0     1162 2023-05-25 17:51:14.116034 wf_video_io-3.3.2/pyproject.toml
+-rwxr-xr-x   0        0        0       28 2022-07-13 02:25:51.323025 wf_video_io-3.3.2/video_io/__init__.py
+-rw-r--r--   0        0        0       37 2022-10-13 19:42:09.408938 wf_video_io-3.3.2/video_io/client/__init__.py
+-rwxr-xr-x   0        0        0    16757 2023-05-25 17:49:44.482339 wf_video_io-3.3.2/video_io/client/core.py
+-rw-r--r--   0        0        0      308 2023-05-25 17:31:09.138857 wf_video_io-3.3.2/video_io/client/errors.py
+-rw-r--r--   0        0        0     3385 2023-05-24 18:36:26.987342 wf_video_io-3.3.2/video_io/client/utils.py
+-rw-r--r--   0        0        0     1742 2023-05-15 17:34:04.821553 wf_video_io-3.3.2/video_io/config.py
+-rwxr-xr-x   0        0        0    47659 2023-05-15 17:34:04.959430 wf_video_io-3.3.2/video_io/core.py
+-rw-r--r--   0        0        0      382 2023-05-15 17:34:04.811182 wf_video_io-3.3.2/video_io/log_retry.py
+-rw-r--r--   0        0        0    10067 2023-05-15 17:34:04.860739 wf_video_io-3.3.2/video_io/utils.py
+-rw-r--r--   0        0        0      585 2023-01-27 16:56:30.326420 wf_video_io-3.3.2/video_io/video_reader.py
+-rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 wf_video_io-3.3.2/setup.py
+-rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 wf_video_io-3.3.2/PKG-INFO
```

### Comparing `wf_video_io-3.3.1/LICENSE` & `wf_video_io-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.1/pyproject.toml` & `wf_video_io-3.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "wf-video-io"
 dynamic = ["version"]
 
 [tool.poetry]
 name = "wf-video-io"
-version = "3.3.1"
+version = "3.3.2"
 description = "Library for working with video files and interacting with the wildflower video-service"
 authors = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>"]
 maintainers = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>", "Benjamin Jaffe-Talberg <ben.talberg@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "video_io"}]
```

### Comparing `wf_video_io-3.3.1/video_io/client/core.py` & `wf_video_io-3.3.2/video_io/client/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,29 @@
 import requests
 from requests.adapters import HTTPAdapter
 from typing import Optional
 import yaml
 
 import video_io.config
 from video_io.log_retry import LogRetry
-from video_io.client.errors import SyncError
+from video_io.client.errors import SyncError, BadVideoError
 from video_io.client.utils import (
     client_token,
     parse_path,
     get_video_file_details,
     chunks,
     FPS_PATH,
 )
 
 
 logger = logging.getLogger(__name__)
 
 
+UPLOAD_FAILED_REASON_BAD_VIDEO = "BAD_VIDEO"
+
 class VideoStorageClient:
     DEFAULT_CONNECTION_POOL_SIZE = 10
 
     def __init__(
         self,
         token=None,
         cache_directory=video_io.config.VIDEO_STORAGE_LOCAL_CACHE_DIRECTORY,
@@ -255,15 +257,20 @@
                     "error": f"Invalid path. '{path}' doesn't match pattern [environment_id]/[camera_id]/[year]/[month]/[day]/[hour]/[min]-[second].mp4"
                 }
 
         return await self._upload_videos(all_file_details)
 
     def prepare_video(self, file_details: Dict) -> (Dict, BytesIO):
         path = file_details["path"]
-        video_properties = get_video_file_details(path)
+
+        try:
+            video_properties = get_video_file_details(path)
+        except Exception as e:
+            raise BadVideoError(f"Could not ffprobe video file {file_details['path']} - {e}")
+
         if file_details["ptype"] == "file":
             ts = f"{file_details['year']}-{file_details['month']}-{file_details['day']}T{file_details['hour']}:{file_details['file'][0:2]}:{file_details['file'][3:5]}.0000"
             meta = {
                 "timestamp": ts,
                 "meta": {
                     "environment_id": file_details["environment_id"],
                     "camera_id": file_details["camera_id"],
@@ -291,38 +298,52 @@
             "method": "POST",
             "url": f"{self.URL}/videos",
             "headers": self.headers,
         }
 
         files = []
         videos = []
+        results = []
         for details in file_details:
-            meta, fileio = self.prepare_video(details)
+            try:
+                meta, fileio = self.prepare_video(details)
+            except BadVideoError:
+                results.append(
+                    {
+                        "id": None,
+                        "path": details['filepath'],
+                        "uploaded": False,
+                        "upload_failed_reason": UPLOAD_FAILED_REASON_BAD_VIDEO,
+                        "disposition": None
+                    }
+                )
+                continue
+
             files.append(
                 (
                     "files",
                     fileio,
                 )
             )
             videos.append(meta)
 
-        results = []
         request["files"] = files
         request["data"] = {"videos": json.dumps(videos)}
         try:
             request = requests.Request(**request)
             r = request.prepare()
             response = self.request_session.send(r)
             response.raise_for_status()
 
             for ii, vr in enumerate(response.json()):
                 results.append(
                     {
                         "path": videos[ii]["meta"]["path"],
                         "uploaded": True,
+                        "upload_failed_reason": None,
                         "id": vr["id"],
                         "disposition": "ok"
                         if "disposition" not in vr
                         else vr["disposition"],
                     }
                 )
             return results
```

### Comparing `wf_video_io-3.3.1/video_io/client/utils.py` & `wf_video_io-3.3.2/video_io/client/utils.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.1/video_io/config.py` & `wf_video_io-3.3.2/video_io/config.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.1/video_io/core.py` & `wf_video_io-3.3.2/video_io/core.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.1/video_io/utils.py` & `wf_video_io-3.3.2/video_io/utils.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.1/video_io/video_reader.py` & `wf_video_io-3.3.2/video_io/video_reader.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.1/setup.py` & `wf_video_io-3.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'wf-cv-utils>=3.4.0',
  'wf-fastapi-auth0>=1.0',
  'wf-gqlpycgen>=0.7.4,<0.8.0',
  'wf-honeycomb-io>=2.0.0']
 
 setup_kwargs = {
     'name': 'wf-video-io',
-    'version': '3.3.1',
+    'version': '3.3.2',
     'description': 'Library for working with video files and interacting with the wildflower video-service',
     'long_description': '# video_io\n\nTools for accessing Wildflower video data\n\n## Test\n\nTests are written with *behave* and *pytest*. As of 11/10/2022, *behave* tests are not functional.\n\n__Run pytest tests__\n\n```pytest```\n\n## Task list\n* ~~Add ability to request concatenation of videos~~ (11/7/2022)\n',
     'author': 'Paul J DeCoursey',
     'author_email': 'paul@decoursey.net',
     'maintainer': 'Paul J DeCoursey',
     'maintainer_email': 'paul@decoursey.net',
     'url': 'None',
```

### Comparing `wf_video_io-3.3.1/PKG-INFO` & `wf_video_io-3.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-video-io
-Version: 3.3.1
+Version: 3.3.2
 Summary: Library for working with video files and interacting with the wildflower video-service
 License: MIT
 Author: Paul J DeCoursey
 Author-email: paul@decoursey.net
 Maintainer: Paul J DeCoursey
 Maintainer-email: paul@decoursey.net
 Requires-Python: >=3.8,<3.12
```

