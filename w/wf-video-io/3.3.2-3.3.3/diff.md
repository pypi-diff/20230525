# Comparing `tmp/wf_video_io-3.3.2.tar.gz` & `tmp/wf_video_io-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf_video_io-3.3.2.tar", max compression
+gzip compressed data, was "wf_video_io-3.3.3.tar", max compression
```

## Comparing `wf_video_io-3.3.2.tar` & `wf_video_io-3.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0     1088 2022-07-13 02:25:51.284383 wf_video_io-3.3.2/LICENSE
--rwxr-xr-x   0        0        0      278 2023-01-27 16:56:30.309581 wf_video_io-3.3.2/README.md
--rw-r--r--   0        0        0     1162 2023-05-25 17:51:14.116034 wf_video_io-3.3.2/pyproject.toml
--rwxr-xr-x   0        0        0       28 2022-07-13 02:25:51.323025 wf_video_io-3.3.2/video_io/__init__.py
--rw-r--r--   0        0        0       37 2022-10-13 19:42:09.408938 wf_video_io-3.3.2/video_io/client/__init__.py
--rwxr-xr-x   0        0        0    16757 2023-05-25 17:49:44.482339 wf_video_io-3.3.2/video_io/client/core.py
--rw-r--r--   0        0        0      308 2023-05-25 17:31:09.138857 wf_video_io-3.3.2/video_io/client/errors.py
--rw-r--r--   0        0        0     3385 2023-05-24 18:36:26.987342 wf_video_io-3.3.2/video_io/client/utils.py
--rw-r--r--   0        0        0     1742 2023-05-15 17:34:04.821553 wf_video_io-3.3.2/video_io/config.py
--rwxr-xr-x   0        0        0    47659 2023-05-15 17:34:04.959430 wf_video_io-3.3.2/video_io/core.py
--rw-r--r--   0        0        0      382 2023-05-15 17:34:04.811182 wf_video_io-3.3.2/video_io/log_retry.py
--rw-r--r--   0        0        0    10067 2023-05-15 17:34:04.860739 wf_video_io-3.3.2/video_io/utils.py
--rw-r--r--   0        0        0      585 2023-01-27 16:56:30.326420 wf_video_io-3.3.2/video_io/video_reader.py
--rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 wf_video_io-3.3.2/setup.py
--rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 wf_video_io-3.3.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1088 2022-07-13 02:25:51.284383 wf_video_io-3.3.3/LICENSE
+-rwxr-xr-x   0        0        0      278 2023-01-27 16:56:30.309581 wf_video_io-3.3.3/README.md
+-rw-r--r--   0        0        0     1162 2023-05-25 18:28:16.480641 wf_video_io-3.3.3/pyproject.toml
+-rwxr-xr-x   0        0        0       28 2022-07-13 02:25:51.323025 wf_video_io-3.3.3/video_io/__init__.py
+-rw-r--r--   0        0        0       37 2022-10-13 19:42:09.408938 wf_video_io-3.3.3/video_io/client/__init__.py
+-rwxr-xr-x   0        0        0    17296 2023-05-25 18:23:09.180053 wf_video_io-3.3.3/video_io/client/core.py
+-rw-r--r--   0        0        0      308 2023-05-25 17:31:09.138857 wf_video_io-3.3.3/video_io/client/errors.py
+-rw-r--r--   0        0        0     3385 2023-05-25 18:28:00.924148 wf_video_io-3.3.3/video_io/client/utils.py
+-rw-r--r--   0        0        0     1742 2023-05-15 17:34:04.821553 wf_video_io-3.3.3/video_io/config.py
+-rwxr-xr-x   0        0        0    47659 2023-05-15 17:34:04.959430 wf_video_io-3.3.3/video_io/core.py
+-rw-r--r--   0        0        0      382 2023-05-15 17:34:04.811182 wf_video_io-3.3.3/video_io/log_retry.py
+-rw-r--r--   0        0        0    10067 2023-05-15 17:34:04.860739 wf_video_io-3.3.3/video_io/utils.py
+-rw-r--r--   0        0        0      585 2023-01-27 16:56:30.326420 wf_video_io-3.3.3/video_io/video_reader.py
+-rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 wf_video_io-3.3.3/setup.py
+-rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 wf_video_io-3.3.3/PKG-INFO
```

### Comparing `wf_video_io-3.3.2/LICENSE` & `wf_video_io-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.2/pyproject.toml` & `wf_video_io-3.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "wf-video-io"
 dynamic = ["version"]
 
 [tool.poetry]
 name = "wf-video-io"
-version = "3.3.2"
+version = "3.3.3"
 description = "Library for working with video files and interacting with the wildflower video-service"
 authors = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>"]
 maintainers = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>", "Benjamin Jaffe-Talberg <ben.talberg@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "video_io"}]
```

### Comparing `wf_video_io-3.3.2/video_io/client/core.py` & `wf_video_io-3.3.3/video_io/client/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 )
 
 
 logger = logging.getLogger(__name__)
 
 
 UPLOAD_FAILED_REASON_BAD_VIDEO = "BAD_VIDEO"
+UPLOAD_FAILED_REASON_BAD_PATH_TO_VIDEO = "BAD_PATH_TO_VIDEO"
 
 class VideoStorageClient:
     DEFAULT_CONNECTION_POOL_SIZE = 10
 
     def __init__(
         self,
         token=None,
@@ -238,30 +239,38 @@
         response = await self.upload_videos(paths=[path], local_cache_directory=local_cache_directory)
         return response[0]
 
     async def upload_videos(self, paths: List[str], local_cache_directory: str = None):
         if local_cache_directory is None:
             local_cache_directory = self.CACHE_DIRECTORY
 
-        all_results: list[None, dict] = [None] * len(paths)
-        all_file_details: list[dict] = []
+        bad_file_results: List[dict] = []
+        all_file_details: List[dict] = []
         for ii, path in enumerate(paths):
             full_path = local_cache_directory / path
             ptype, file_details = parse_path(path)
             if ptype == "file":
                 file_details["ptype"] = ptype
                 file_details["path"] = full_path
                 file_details["filepath"] = path
                 all_file_details.append(file_details)
             else:
-                all_results[ii] = {
-                    "error": f"Invalid path. '{path}' doesn't match pattern [environment_id]/[camera_id]/[year]/[month]/[day]/[hour]/[min]-[second].mp4"
-                }
-
-        return await self._upload_videos(all_file_details)
+                bad_file_results.append({
+                    "id": None,
+                    "path": path,
+                    "uploaded": False,
+                    "upload_failed_reason": UPLOAD_FAILED_REASON_BAD_PATH_TO_VIDEO,
+                    "upload_failed_error": f"Invalid path. '{path}' doesn't match pattern [environment_id]/[camera_id]/[year]/[month]/[day]/[hour]/[min]-[second].mp4",
+                    "disposition": None
+                })
+
+        upload_results = []
+        if len(all_file_details) > 0:
+            upload_results = await self._upload_videos(all_file_details)
+        return [*upload_results, *bad_file_results]
 
     def prepare_video(self, file_details: Dict) -> (Dict, BytesIO):
         path = file_details["path"]
 
         try:
             video_properties = get_video_file_details(path)
         except Exception as e:
@@ -302,21 +311,22 @@
 
         files = []
         videos = []
         results = []
         for details in file_details:
             try:
                 meta, fileio = self.prepare_video(details)
-            except BadVideoError:
+            except BadVideoError as e:
                 results.append(
                     {
                         "id": None,
                         "path": details['filepath'],
                         "uploaded": False,
                         "upload_failed_reason": UPLOAD_FAILED_REASON_BAD_VIDEO,
+                        "upload_failed_error": str(e),
                         "disposition": None
                     }
                 )
                 continue
 
             files.append(
                 (
@@ -336,14 +346,15 @@
 
             for ii, vr in enumerate(response.json()):
                 results.append(
                     {
                         "path": videos[ii]["meta"]["path"],
                         "uploaded": True,
                         "upload_failed_reason": None,
+                        "upload_failed_error": None,
                         "id": vr["id"],
                         "disposition": "ok"
                         if "disposition" not in vr
                         else vr["disposition"],
                     }
                 )
             return results
```

### Comparing `wf_video_io-3.3.2/video_io/client/utils.py` & `wf_video_io-3.3.3/video_io/client/utils.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.2/video_io/config.py` & `wf_video_io-3.3.3/video_io/config.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.2/video_io/core.py` & `wf_video_io-3.3.3/video_io/core.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.2/video_io/utils.py` & `wf_video_io-3.3.3/video_io/utils.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.2/video_io/video_reader.py` & `wf_video_io-3.3.3/video_io/video_reader.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.2/setup.py` & `wf_video_io-3.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'wf-cv-utils>=3.4.0',
  'wf-fastapi-auth0>=1.0',
  'wf-gqlpycgen>=0.7.4,<0.8.0',
  'wf-honeycomb-io>=2.0.0']
 
 setup_kwargs = {
     'name': 'wf-video-io',
-    'version': '3.3.2',
+    'version': '3.3.3',
     'description': 'Library for working with video files and interacting with the wildflower video-service',
     'long_description': '# video_io\n\nTools for accessing Wildflower video data\n\n## Test\n\nTests are written with *behave* and *pytest*. As of 11/10/2022, *behave* tests are not functional.\n\n__Run pytest tests__\n\n```pytest```\n\n## Task list\n* ~~Add ability to request concatenation of videos~~ (11/7/2022)\n',
     'author': 'Paul J DeCoursey',
     'author_email': 'paul@decoursey.net',
     'maintainer': 'Paul J DeCoursey',
     'maintainer_email': 'paul@decoursey.net',
     'url': 'None',
```

### Comparing `wf_video_io-3.3.2/PKG-INFO` & `wf_video_io-3.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-video-io
-Version: 3.3.2
+Version: 3.3.3
 Summary: Library for working with video files and interacting with the wildflower video-service
 License: MIT
 Author: Paul J DeCoursey
 Author-email: paul@decoursey.net
 Maintainer: Paul J DeCoursey
 Maintainer-email: paul@decoursey.net
 Requires-Python: >=3.8,<3.12
```

