# Comparing `tmp/pyrosexmod-0.0.5.tar.gz` & `tmp/pyrosexmod-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrosexmod-0.0.5.tar", last modified: Thu May 25 07:57:45 2023, max compression
+gzip compressed data, was "pyrosexmod-0.0.6.tar", last modified: Thu May 25 08:05:45 2023, max compression
```

## Comparing `pyrosexmod-0.0.5.tar` & `pyrosexmod-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:57:45.049990 pyrosexmod-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-25 07:57:32.000000 pyrosexmod-0.0.5/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-25 07:57:32.000000 pyrosexmod-0.0.5/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-25 07:57:32.000000 pyrosexmod-0.0.5/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 07:57:45.049990 pyrosexmod-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-25 07:57:32.000000 pyrosexmod-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:57:45.045990 pyrosexmod-0.0.5/pyrosexmod/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 07:57:32.000000 pyrosexmod-0.0.5/pyrosexmod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:57:45.049990 pyrosexmod-0.0.5/pyrosexmod/filters/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 07:57:32.000000 pyrosexmod-0.0.5/pyrosexmod/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 07:57:32.000000 pyrosexmod-0.0.5/pyrosexmod/filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:57:45.049990 pyrosexmod-0.0.5/pyrosexmod/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 07:57:32.000000 pyrosexmod-0.0.5/pyrosexmod/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-25 07:57:32.000000 pyrosexmod-0.0.5/pyrosexmod/helpers/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:57:45.049990 pyrosexmod-0.0.5/pyrosexmod/listen/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 07:57:32.000000 pyrosexmod-0.0.5/pyrosexmod/listen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-25 07:57:32.000000 pyrosexmod-0.0.5/pyrosexmod/listen/listen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-25 07:57:32.000000 pyrosexmod-0.0.5/pyrosexmod/teledl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:57:45.049990 pyrosexmod-0.0.5/pyrosexmod/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 07:57:32.000000 pyrosexmod-0.0.5/pyrosexmod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-25 07:57:32.000000 pyrosexmod-0.0.5/pyrosexmod/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:57:45.049990 pyrosexmod-0.0.5/pyrosexmod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 07:57:45.000000 pyrosexmod-0.0.5/pyrosexmod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 07:57:45.000000 pyrosexmod-0.0.5/pyrosexmod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:57:45.000000 pyrosexmod-0.0.5/pyrosexmod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 07:57:45.000000 pyrosexmod-0.0.5/pyrosexmod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 07:57:45.000000 pyrosexmod-0.0.5/pyrosexmod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:57:45.049990 pyrosexmod-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-25 07:57:32.000000 pyrosexmod-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:05:45.020124 pyrosexmod-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-25 08:05:30.000000 pyrosexmod-0.0.6/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-25 08:05:30.000000 pyrosexmod-0.0.6/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-25 08:05:30.000000 pyrosexmod-0.0.6/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 08:05:45.020124 pyrosexmod-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-25 08:05:30.000000 pyrosexmod-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:05:45.016124 pyrosexmod-0.0.6/pyrosexmod/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 08:05:30.000000 pyrosexmod-0.0.6/pyrosexmod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:05:45.020124 pyrosexmod-0.0.6/pyrosexmod/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 08:05:30.000000 pyrosexmod-0.0.6/pyrosexmod/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 08:05:30.000000 pyrosexmod-0.0.6/pyrosexmod/filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:05:45.020124 pyrosexmod-0.0.6/pyrosexmod/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 08:05:30.000000 pyrosexmod-0.0.6/pyrosexmod/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-25 08:05:30.000000 pyrosexmod-0.0.6/pyrosexmod/helpers/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:05:45.020124 pyrosexmod-0.0.6/pyrosexmod/listen/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 08:05:30.000000 pyrosexmod-0.0.6/pyrosexmod/listen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-25 08:05:30.000000 pyrosexmod-0.0.6/pyrosexmod/listen/listen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-25 08:05:30.000000 pyrosexmod-0.0.6/pyrosexmod/teledl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:05:45.020124 pyrosexmod-0.0.6/pyrosexmod/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 08:05:30.000000 pyrosexmod-0.0.6/pyrosexmod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-25 08:05:30.000000 pyrosexmod-0.0.6/pyrosexmod/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:05:45.020124 pyrosexmod-0.0.6/pyrosexmod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 08:05:45.000000 pyrosexmod-0.0.6/pyrosexmod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 08:05:45.000000 pyrosexmod-0.0.6/pyrosexmod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 08:05:45.000000 pyrosexmod-0.0.6/pyrosexmod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 08:05:45.000000 pyrosexmod-0.0.6/pyrosexmod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 08:05:45.000000 pyrosexmod-0.0.6/pyrosexmod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 08:05:45.020124 pyrosexmod-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-25 08:05:30.000000 pyrosexmod-0.0.6/setup.py
```

### Comparing `pyrosexmod-0.0.5/COPYING` & `pyrosexmod-0.0.6/COPYING`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.5/COPYING.lesser` & `pyrosexmod-0.0.6/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.5/NOTICE` & `pyrosexmod-0.0.6/NOTICE`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.5/PKG-INFO` & `pyrosexmod-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrosexmod
-Version: 0.0.5
+Version: 0.0.6
 Summary: A monkeypatcher add-on for Pyrosex
 Home-page: https://github.com/OTHFamily/pyrosexmod
 Author: OTH
 Author-email: oth@pyrosex.org
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `pyrosexmod-0.0.5/README.md` & `pyrosexmod-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.5/pyrosexmod/helpers/helpers.py` & `pyrosexmod-0.0.6/pyrosexmod/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.5/pyrosexmod/listen/listen.py` & `pyrosexmod-0.0.6/pyrosexmod/listen/listen.py`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.5/pyrosexmod/teledl.py` & `pyrosexmod-0.0.6/pyrosexmod/teledl.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,70 @@
 import os
 import yt_dlp
 import asyncio
 from typing import Union
 
 
-class Teledl:
-    async def formats(self, link: str):
-        if "&" in link:
-            link = link.split("&")[0]
-        ytdl_opts = {"quiet": True}
-        ydl = yt_dlp.YoutubeDL(ytdl_opts)
-        with ydl:
-            formats = []
-            r = ydl.extract_info(link, download=False)
-            for format in r["formats"]:
+async def formats(self, link: str):
+    if "&" in link:
+        link = link.split("&")[0]
+    ytdl_opts = {"quiet": True}
+    ydl = yt_dlp.YoutubeDL(ytdl_opts)
+    with ydl:
+        formats = []
+        r = ydl.extract_info(link, download=False)
+        for format in r["formats"]:
+            try:
+                str(format["format"])
+            except:
+                continue
+            if not "dash" in str(format["format"]).lower():
                 try:
-                    str(format["format"])
+                    format["format"]
+                    format["filesize"]
+                    format["format_id"]
+                    format["ext"]
+                    format["format_note"]
                 except:
                     continue
-                if not "dash" in str(format["format"]).lower():
-                    try:
-                        format["format"]
-                        format["filesize"]
-                        format["format_id"]
-                        format["ext"]
-                        format["format_note"]
-                    except:
-                        continue
-                    formats.append(
-                        {
-                            "format": format["format"],
-                            "filesize": format["filesize"],
-                            "format_id": format["format_id"],
-                            "ext": format["ext"],
-                            "format_note": format["format_note"],
-                            "url": link,
-                        }
-                    )
-        return formats, link
-    
-    
-    async def download(
-        self,
-        link: str,
-        format_id: Union[bool, str],
-    ) -> str:
-        loop = asyncio.get_running_loop()
-    
-        def video_dl():
-            formats = f"{format_id}+140"
-            ydl_optssx = {
-                "format": formats,
-                "outtmpl": "downloads/%(title)s",
-                "geo_bypass": True,
-                "nocheckcertificate": True,
-                "quiet": True,
-                "no_warnings": True,
-                "prefer_ffmpeg": True,
-                "merge_output_format": "mp4",
-            }
-            x = yt_dlp.YoutubeDL(ydl_optssx)
-            info = x.extract_info(link, False)
-            xyz = os.path.join(
-                "downloads", f"{info['title']}.mp4"
-            )
-            if os.path.exists(xyz):
-                return xyz
-            x.download([link])
+                formats.append(
+                    {
+                        "format": format["format"],
+                        "filesize": format["filesize"],
+                        "format_id": format["format_id"],
+                        "ext": format["ext"],
+                        "format_note": format["format_note"],
+                        "url": link,
+                    }
+                )
+    return formats, link
+
+
+async def download(
+    self,
+    link: str,
+    format_id: Union[bool, str],
+) -> str:
+    loop = asyncio.get_running_loop()
+
+    def video_dl():
+        formats = f"{format_id}+140"
+        ydl_optssx = {
+            "format": formats,
+            "outtmpl": "downloads/%(title)s",
+            "geo_bypass": True,
+            "nocheckcertificate": True,
+            "quiet": True,
+            "no_warnings": True,
+            "prefer_ffmpeg": True,
+            "merge_output_format": "mp4",
+        }
+        x = yt_dlp.YoutubeDL(ydl_optssx)
+        info = x.extract_info(link, False)
+        xyz = os.path.join(
+            "downloads", f"{info['title']}.mp4"
+        )
+        if os.path.exists(xyz):
             return xyz
-        return await loop.run_in_executor(None, video_dl)
+        x.download([link])
+        return xyz
+    return await loop.run_in_executor(None, video_dl)
```

### Comparing `pyrosexmod-0.0.5/pyrosexmod.egg-info/PKG-INFO` & `pyrosexmod-0.0.6/pyrosexmod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrosexmod
-Version: 0.0.5
+Version: 0.0.6
 Summary: A monkeypatcher add-on for Pyrosex
 Home-page: https://github.com/OTHFamily/pyrosexmod
 Author: OTH
 Author-email: oth@pyrosex.org
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `pyrosexmod-0.0.5/setup.py` & `pyrosexmod-0.0.6/setup.py`

 * *Files identical despite different names*

