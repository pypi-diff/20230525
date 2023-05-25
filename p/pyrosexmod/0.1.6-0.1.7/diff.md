# Comparing `tmp/pyrosexmod-0.1.6.tar.gz` & `tmp/pyrosexmod-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrosexmod-0.1.6.tar", last modified: Thu May 25 11:26:24 2023, max compression
+gzip compressed data, was "pyrosexmod-0.1.7.tar", last modified: Thu May 25 11:31:36 2023, max compression
```

## Comparing `pyrosexmod-0.1.6.tar` & `pyrosexmod-0.1.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:26:24.473373 pyrosexmod-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-25 11:26:08.000000 pyrosexmod-0.1.6/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-25 11:26:08.000000 pyrosexmod-0.1.6/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-25 11:26:08.000000 pyrosexmod-0.1.6/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 11:26:24.473373 pyrosexmod-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-25 11:26:08.000000 pyrosexmod-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:26:24.469372 pyrosexmod-0.1.6/pyrosexmod/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 11:26:08.000000 pyrosexmod-0.1.6/pyrosexmod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:26:24.473373 pyrosexmod-0.1.6/pyrosexmod/filters/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 11:26:08.000000 pyrosexmod-0.1.6/pyrosexmod/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 11:26:08.000000 pyrosexmod-0.1.6/pyrosexmod/filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:26:24.473373 pyrosexmod-0.1.6/pyrosexmod/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 11:26:08.000000 pyrosexmod-0.1.6/pyrosexmod/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-25 11:26:08.000000 pyrosexmod-0.1.6/pyrosexmod/helpers/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:26:24.473373 pyrosexmod-0.1.6/pyrosexmod/listen/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 11:26:08.000000 pyrosexmod-0.1.6/pyrosexmod/listen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-25 11:26:08.000000 pyrosexmod-0.1.6/pyrosexmod/listen/listen.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-25 11:26:08.000000 pyrosexmod-0.1.6/pyrosexmod/teledl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:26:24.473373 pyrosexmod-0.1.6/pyrosexmod/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 11:26:08.000000 pyrosexmod-0.1.6/pyrosexmod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-25 11:26:08.000000 pyrosexmod-0.1.6/pyrosexmod/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:26:24.473373 pyrosexmod-0.1.6/pyrosexmod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 11:26:24.000000 pyrosexmod-0.1.6/pyrosexmod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 11:26:24.000000 pyrosexmod-0.1.6/pyrosexmod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:26:24.000000 pyrosexmod-0.1.6/pyrosexmod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 11:26:24.000000 pyrosexmod-0.1.6/pyrosexmod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 11:26:24.000000 pyrosexmod-0.1.6/pyrosexmod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:26:24.473373 pyrosexmod-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-25 11:26:08.000000 pyrosexmod-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:31:36.253238 pyrosexmod-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-25 11:31:24.000000 pyrosexmod-0.1.7/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-25 11:31:24.000000 pyrosexmod-0.1.7/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-25 11:31:24.000000 pyrosexmod-0.1.7/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 11:31:36.253238 pyrosexmod-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-25 11:31:24.000000 pyrosexmod-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:31:36.249238 pyrosexmod-0.1.7/pyrosexmod/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 11:31:24.000000 pyrosexmod-0.1.7/pyrosexmod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:31:36.249238 pyrosexmod-0.1.7/pyrosexmod/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 11:31:24.000000 pyrosexmod-0.1.7/pyrosexmod/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 11:31:24.000000 pyrosexmod-0.1.7/pyrosexmod/filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:31:36.249238 pyrosexmod-0.1.7/pyrosexmod/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 11:31:24.000000 pyrosexmod-0.1.7/pyrosexmod/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-25 11:31:24.000000 pyrosexmod-0.1.7/pyrosexmod/helpers/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:31:36.253238 pyrosexmod-0.1.7/pyrosexmod/listen/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 11:31:24.000000 pyrosexmod-0.1.7/pyrosexmod/listen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-25 11:31:24.000000 pyrosexmod-0.1.7/pyrosexmod/listen/listen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-25 11:31:24.000000 pyrosexmod-0.1.7/pyrosexmod/teledl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:31:36.253238 pyrosexmod-0.1.7/pyrosexmod/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 11:31:24.000000 pyrosexmod-0.1.7/pyrosexmod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-25 11:31:24.000000 pyrosexmod-0.1.7/pyrosexmod/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:31:36.249238 pyrosexmod-0.1.7/pyrosexmod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 11:31:36.000000 pyrosexmod-0.1.7/pyrosexmod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 11:31:36.000000 pyrosexmod-0.1.7/pyrosexmod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:31:36.000000 pyrosexmod-0.1.7/pyrosexmod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 11:31:36.000000 pyrosexmod-0.1.7/pyrosexmod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 11:31:36.000000 pyrosexmod-0.1.7/pyrosexmod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:31:36.253238 pyrosexmod-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-25 11:31:24.000000 pyrosexmod-0.1.7/setup.py
```

### Comparing `pyrosexmod-0.1.6/COPYING` & `pyrosexmod-0.1.7/COPYING`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.1.6/COPYING.lesser` & `pyrosexmod-0.1.7/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.1.6/NOTICE` & `pyrosexmod-0.1.7/NOTICE`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.1.6/PKG-INFO` & `pyrosexmod-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrosexmod
-Version: 0.1.6
+Version: 0.1.7
 Summary: A monkeypatcher add-on for Pyrosex
 Home-page: https://github.com/OTHFamily/pyrosexmod
 Author: OTH
 Author-email: oth@pyrosex.org
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `pyrosexmod-0.1.6/README.md` & `pyrosexmod-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.1.6/pyrosexmod/helpers/helpers.py` & `pyrosexmod-0.1.7/pyrosexmod/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.1.6/pyrosexmod/listen/listen.py` & `pyrosexmod-0.1.7/pyrosexmod/listen/listen.py`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.1.6/pyrosexmod/teledl.py` & `pyrosexmod-0.1.7/pyrosexmod/teledl.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 
 async def download(link: str) -> str:
     loop = asyncio.get_running_loop()
     
     def video_dl():
         ydl_optssx = {
-            "outtmpl": "downloads/%(id)s.%(ext)s",
+            "outtmpl": "downloads/%(id)s.mp4",
             "nooverwrites": True,
             "no_warnings": False,
             "ignoreerrors": True,
         }
         x = youtube_dl.YoutubeDL(ydl_optssx)
         info = x.extract_info(link, False)
         xyz = os.path.join(
-            "downloads", f"{info['id']}.{info['ext']}"
+            "downloads", f"{info['id']}.mp4"
         )
         if os.path.exists(xyz):
             return xyz
         x.download([link])
         return xyz
 
     return  await loop.run_in_executor(None, video_dl)
```

### Comparing `pyrosexmod-0.1.6/pyrosexmod.egg-info/PKG-INFO` & `pyrosexmod-0.1.7/pyrosexmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrosexmod
-Version: 0.1.6
+Version: 0.1.7
 Summary: A monkeypatcher add-on for Pyrosex
 Home-page: https://github.com/OTHFamily/pyrosexmod
 Author: OTH
 Author-email: oth@pyrosex.org
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `pyrosexmod-0.1.6/setup.py` & `pyrosexmod-0.1.7/setup.py`

 * *Files identical despite different names*

