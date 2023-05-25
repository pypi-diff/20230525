# Comparing `tmp/aiorobonect-0.1.8.tar.gz` & `tmp/aiorobonect-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorobonect-0.1.8.tar", last modified: Sat May 20 15:57:04 2023, max compression
+gzip compressed data, was "aiorobonect-0.1.9.tar", last modified: Sat May 20 16:21:07 2023, max compression
```

## Comparing `aiorobonect-0.1.8.tar` & `aiorobonect-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:57:04.060212 aiorobonect-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-20 15:56:44.000000 aiorobonect-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-20 15:57:04.060212 aiorobonect-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-20 15:56:44.000000 aiorobonect-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:57:04.056212 aiorobonect-0.1.8/aiorobonect/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-20 15:56:44.000000 aiorobonect-0.1.8/aiorobonect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-20 15:56:44.000000 aiorobonect-0.1.8/aiorobonect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-20 15:56:44.000000 aiorobonect-0.1.8/aiorobonect/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-20 15:56:44.000000 aiorobonect-0.1.8/aiorobonect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:57:04.056212 aiorobonect-0.1.8/aiorobonect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-20 15:57:04.000000 aiorobonect-0.1.8/aiorobonect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-20 15:57:04.000000 aiorobonect-0.1.8/aiorobonect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 15:57:04.000000 aiorobonect-0.1.8/aiorobonect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-20 15:57:04.000000 aiorobonect-0.1.8/aiorobonect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 15:57:04.000000 aiorobonect-0.1.8/aiorobonect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 15:57:04.060212 aiorobonect-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-20 15:56:47.000000 aiorobonect-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:21:07.226376 aiorobonect-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-20 16:20:46.000000 aiorobonect-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-20 16:21:07.226376 aiorobonect-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-20 16:20:46.000000 aiorobonect-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:21:07.226376 aiorobonect-0.1.9/aiorobonect/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-20 16:20:46.000000 aiorobonect-0.1.9/aiorobonect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-20 16:20:46.000000 aiorobonect-0.1.9/aiorobonect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-20 16:20:46.000000 aiorobonect-0.1.9/aiorobonect/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-20 16:20:46.000000 aiorobonect-0.1.9/aiorobonect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:21:07.226376 aiorobonect-0.1.9/aiorobonect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-20 16:21:07.000000 aiorobonect-0.1.9/aiorobonect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-20 16:21:07.000000 aiorobonect-0.1.9/aiorobonect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 16:21:07.000000 aiorobonect-0.1.9/aiorobonect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-20 16:21:07.000000 aiorobonect-0.1.9/aiorobonect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 16:21:07.000000 aiorobonect-0.1.9/aiorobonect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 16:21:07.226376 aiorobonect-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-20 16:20:49.000000 aiorobonect-0.1.9/setup.py
```

### Comparing `aiorobonect-0.1.8/LICENSE` & `aiorobonect-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.1.8/PKG-INFO` & `aiorobonect-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.1.8
+Version: 0.1.9
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-0.1.8/README.md` & `aiorobonect-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.1.8/aiorobonect/client.py` & `aiorobonect-0.1.9/aiorobonect/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,10 +81,9 @@
         return result
 
     async def state(self) -> list[dict]:
         """Send status command to mower."""
         self.session_start()
         result = await self.async_cmd("status")
         self.sleeping = result.get("status").get("status") == 17
-        print(result.json)
         await self.session_close()
         return result
```

### Comparing `aiorobonect-0.1.8/aiorobonect.egg-info/PKG-INFO` & `aiorobonect-0.1.9/aiorobonect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.1.8
+Version: 0.1.9
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-0.1.8/setup.py` & `aiorobonect-0.1.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=[val.strip() for val in open("requirements.txt")],
-    version="v0.1.8",
+    version="v0.1.9",
 )
```

