# Comparing `tmp/pyrosexmod-0.0.8.tar.gz` & `tmp/pyrosexmod-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrosexmod-0.0.8.tar", last modified: Thu May 25 09:03:34 2023, max compression
+gzip compressed data, was "pyrosexmod-0.0.9.tar", last modified: Thu May 25 09:21:18 2023, max compression
```

## Comparing `pyrosexmod-0.0.8.tar` & `pyrosexmod-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:34.229347 pyrosexmod-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-25 09:03:15.000000 pyrosexmod-0.0.8/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-25 09:03:15.000000 pyrosexmod-0.0.8/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-25 09:03:15.000000 pyrosexmod-0.0.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 09:03:34.229347 pyrosexmod-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-25 09:03:15.000000 pyrosexmod-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:34.225347 pyrosexmod-0.0.8/pyrosexmod/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 09:03:15.000000 pyrosexmod-0.0.8/pyrosexmod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:34.229347 pyrosexmod-0.0.8/pyrosexmod/filters/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 09:03:15.000000 pyrosexmod-0.0.8/pyrosexmod/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 09:03:15.000000 pyrosexmod-0.0.8/pyrosexmod/filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:34.229347 pyrosexmod-0.0.8/pyrosexmod/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 09:03:15.000000 pyrosexmod-0.0.8/pyrosexmod/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-25 09:03:15.000000 pyrosexmod-0.0.8/pyrosexmod/helpers/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:34.229347 pyrosexmod-0.0.8/pyrosexmod/listen/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 09:03:15.000000 pyrosexmod-0.0.8/pyrosexmod/listen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-25 09:03:15.000000 pyrosexmod-0.0.8/pyrosexmod/listen/listen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-25 09:03:15.000000 pyrosexmod-0.0.8/pyrosexmod/teledl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:34.229347 pyrosexmod-0.0.8/pyrosexmod/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 09:03:15.000000 pyrosexmod-0.0.8/pyrosexmod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-25 09:03:15.000000 pyrosexmod-0.0.8/pyrosexmod/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:34.225347 pyrosexmod-0.0.8/pyrosexmod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 09:03:34.000000 pyrosexmod-0.0.8/pyrosexmod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 09:03:34.000000 pyrosexmod-0.0.8/pyrosexmod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:03:34.000000 pyrosexmod-0.0.8/pyrosexmod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 09:03:34.000000 pyrosexmod-0.0.8/pyrosexmod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 09:03:34.000000 pyrosexmod-0.0.8/pyrosexmod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:03:34.229347 pyrosexmod-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-25 09:03:15.000000 pyrosexmod-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:21:18.334339 pyrosexmod-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 09:21:18.330339 pyrosexmod-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:21:18.330339 pyrosexmod-0.0.9/pyrosexmod/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:21:18.330339 pyrosexmod-0.0.9/pyrosexmod/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:21:18.330339 pyrosexmod-0.0.9/pyrosexmod/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/helpers/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:21:18.330339 pyrosexmod-0.0.9/pyrosexmod/listen/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/listen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/listen/listen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/teledl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:21:18.330339 pyrosexmod-0.0.9/pyrosexmod/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:21:18.330339 pyrosexmod-0.0.9/pyrosexmod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 09:21:18.000000 pyrosexmod-0.0.9/pyrosexmod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 09:21:18.000000 pyrosexmod-0.0.9/pyrosexmod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:21:18.000000 pyrosexmod-0.0.9/pyrosexmod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 09:21:18.000000 pyrosexmod-0.0.9/pyrosexmod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 09:21:18.000000 pyrosexmod-0.0.9/pyrosexmod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:21:18.334339 pyrosexmod-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/setup.py
```

### Comparing `pyrosexmod-0.0.8/COPYING` & `pyrosexmod-0.0.9/COPYING`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.8/COPYING.lesser` & `pyrosexmod-0.0.9/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.8/NOTICE` & `pyrosexmod-0.0.9/NOTICE`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.8/PKG-INFO` & `pyrosexmod-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrosexmod
-Version: 0.0.8
+Version: 0.0.9
 Summary: A monkeypatcher add-on for Pyrosex
 Home-page: https://github.com/OTHFamily/pyrosexmod
 Author: OTH
 Author-email: oth@pyrosex.org
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `pyrosexmod-0.0.8/README.md` & `pyrosexmod-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.8/pyrosexmod/helpers/helpers.py` & `pyrosexmod-0.0.9/pyrosexmod/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.8/pyrosexmod/listen/listen.py` & `pyrosexmod-0.0.9/pyrosexmod/listen/listen.py`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.8/pyrosexmod/teledl.py` & `pyrosexmod-0.0.9/pyrosexmod/teledl.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,17 +48,37 @@
         x = ydl.extract_info(link, download=False)
         videoid = x["id"]
     return videoid
 
 
 async def download(
     link: str,
-    format_id: Union[bool, str],
+    video: Union[bool, str] = None,
+    format_id: Union[bool, str] = None,
 ) -> str:
     loop = asyncio.get_running_loop()
+    
+    def vid_dl():
+        ydl_optssx = {
+            "format": "(bestvideo[height<=?720][width<=?1280][ext=mp4])+(bestaudio[ext=m4a])",
+            "outtmpl": "downloads/%(id)s.%(ext)s",
+            "geo_bypass": True,
+            "nocheckcertificate": True,
+            "quiet": True,
+            "no_warnings": True,
+        }
+        x = yt_dlp.YoutubeDL(ydl_optssx)
+        info = x.extract_info(link, False)
+        xyz = os.path.join(
+            "downloads", f"{info['id']}.{info['ext']}"
+        )
+        if os.path.exists(xyz):
+            return xyz
+        x.download([link])
+        return xyz
 
     def video_dl():
         formats = f"{format_id}+140"
         ydl_optssx = {
             "format": formats,
             "outtmpl": "downloads/%(title)s",
             "geo_bypass": True,
@@ -73,8 +93,13 @@
         xyz = os.path.join(
             "downloads", f"{info['title']}.mp4"
         )
         if os.path.exists(xyz):
             return xyz
         x.download([link])
         return xyz
-    return await loop.run_in_executor(None, video_dl)
+
+    if video:
+        downloaded_file = await loop.run_in_executor(None, vid_dl)
+    else:
+        downloaded_file = await loop.run_in_executor(None, video_dl)
+    return downloaded_file
```

### Comparing `pyrosexmod-0.0.8/pyrosexmod.egg-info/PKG-INFO` & `pyrosexmod-0.0.9/pyrosexmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrosexmod
-Version: 0.0.8
+Version: 0.0.9
 Summary: A monkeypatcher add-on for Pyrosex
 Home-page: https://github.com/OTHFamily/pyrosexmod
 Author: OTH
 Author-email: oth@pyrosex.org
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `pyrosexmod-0.0.8/setup.py` & `pyrosexmod-0.0.9/setup.py`

 * *Files identical despite different names*

