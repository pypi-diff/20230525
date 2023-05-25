# Comparing `tmp/tldrwl-0.0.8.tar.gz` & `tmp/tldrwl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldrwl-0.0.8.tar", last modified: Mon May 22 08:58:07 2023, max compression
+gzip compressed data, was "tldrwl-0.0.9.tar", last modified: Thu May 25 01:59:41 2023, max compression
```

## Comparing `tldrwl-0.0.8.tar` & `tldrwl-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 08:58:07.389024 tldrwl-0.0.8/
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)       25 2023-05-22 01:33:23.000000 tldrwl-0.0.8/MANIFEST.in
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)    16607 2023-05-22 08:58:07.389024 tldrwl-0.0.8/PKG-INFO
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)    16317 2023-05-22 08:13:51.000000 tldrwl-0.0.8/README.md
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      100 2023-05-22 06:20:03.000000 tldrwl-0.0.8/requirements.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)       38 2023-05-22 08:58:07.389024 tldrwl-0.0.8/setup.cfg
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      614 2023-05-22 08:57:57.000000 tldrwl-0.0.8/setup.py
-drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 08:58:07.389024 tldrwl-0.0.8/tldrwl/
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 00:53:22.000000 tldrwl-0.0.8/tldrwl/__init__.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1519 2023-05-22 08:55:18.000000 tldrwl-0.0.8/tldrwl/ai_interface.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1177 2023-05-22 05:37:32.000000 tldrwl-0.0.8/tldrwl/exception.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      679 2023-05-22 02:16:47.000000 tldrwl-0.0.8/tldrwl/register.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1148 2023-05-22 08:54:03.000000 tldrwl-0.0.8/tldrwl/summarize.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     5290 2023-05-22 08:54:27.000000 tldrwl-0.0.8/tldrwl/summarize_text.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     2149 2023-05-22 08:54:42.000000 tldrwl-0.0.8/tldrwl/summarize_webpage.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1772 2023-05-22 08:55:00.000000 tldrwl-0.0.8/tldrwl/summarize_youtube.py
-drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 08:58:07.389024 tldrwl-0.0.8/tldrwl.egg-info/
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)    16607 2023-05-22 08:58:07.000000 tldrwl-0.0.8/tldrwl.egg-info/PKG-INFO
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      378 2023-05-22 08:58:07.000000 tldrwl-0.0.8/tldrwl.egg-info/SOURCES.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)        1 2023-05-22 08:58:07.000000 tldrwl-0.0.8/tldrwl.egg-info/dependency_links.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      100 2023-05-22 08:58:07.000000 tldrwl-0.0.8/tldrwl.egg-info/requires.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)        7 2023-05-22 08:58:07.000000 tldrwl-0.0.8/tldrwl.egg-info/top_level.txt
+drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-25 01:59:41.574784 tldrwl-0.0.9/
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)       25 2023-05-22 01:33:23.000000 tldrwl-0.0.9/MANIFEST.in
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)    16607 2023-05-25 01:59:41.574784 tldrwl-0.0.9/PKG-INFO
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)    16317 2023-05-22 08:13:51.000000 tldrwl-0.0.9/README.md
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      100 2023-05-25 01:03:01.000000 tldrwl-0.0.9/requirements.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)       38 2023-05-25 01:59:41.574784 tldrwl-0.0.9/setup.cfg
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      614 2023-05-25 01:59:23.000000 tldrwl-0.0.9/setup.py
+drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-25 01:59:41.574784 tldrwl-0.0.9/tldrwl/
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 00:53:22.000000 tldrwl-0.0.9/tldrwl/__init__.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1840 2023-05-25 01:54:27.000000 tldrwl-0.0.9/tldrwl/__main__.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1519 2023-05-22 08:55:18.000000 tldrwl-0.0.9/tldrwl/ai_interface.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1177 2023-05-22 05:37:32.000000 tldrwl-0.0.9/tldrwl/exception.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      679 2023-05-22 02:16:47.000000 tldrwl-0.0.9/tldrwl/register.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1148 2023-05-25 01:52:32.000000 tldrwl-0.0.9/tldrwl/summarize.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     5290 2023-05-22 08:54:27.000000 tldrwl-0.0.9/tldrwl/summarize_text.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     2149 2023-05-22 08:54:42.000000 tldrwl-0.0.9/tldrwl/summarize_webpage.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1772 2023-05-22 08:55:00.000000 tldrwl-0.0.9/tldrwl/summarize_youtube.py
+drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-25 01:59:41.574784 tldrwl-0.0.9/tldrwl.egg-info/
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)    16607 2023-05-25 01:59:41.000000 tldrwl-0.0.9/tldrwl.egg-info/PKG-INFO
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      397 2023-05-25 01:59:41.000000 tldrwl-0.0.9/tldrwl.egg-info/SOURCES.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)        1 2023-05-25 01:59:41.000000 tldrwl-0.0.9/tldrwl.egg-info/dependency_links.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      100 2023-05-25 01:59:41.000000 tldrwl-0.0.9/tldrwl.egg-info/requires.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)        7 2023-05-25 01:59:41.000000 tldrwl-0.0.9/tldrwl.egg-info/top_level.txt
```

### Comparing `tldrwl-0.0.8/PKG-INFO` & `tldrwl-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tldrwl
-Version: 0.0.8
+Version: 0.0.9
 Summary: Too long, didn't read/watch/listen
 Home-page: https://github.com/jrodal98/tldrwl
 Author: Jacob Rodal
 Author-email: dev@jrodal.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `tldrwl-0.0.8/README.md` & `tldrwl-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.8/setup.py` & `tldrwl-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt") as f:
     install_requires = f.read().splitlines()
 
 setuptools.setup(
     name="tldrwl",
-    version="0.0.8",
+    version="0.0.9",
     author="Jacob Rodal",
     author_email="dev@jrodal.com",
     description="Too long, didn't read/watch/listen",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jrodal98/tldrwl",
     packages=setuptools.find_packages(),
```

### Comparing `tldrwl-0.0.8/tldrwl/ai_interface.py` & `tldrwl-0.0.9/tldrwl/ai_interface.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.8/tldrwl/exception.py` & `tldrwl-0.0.9/tldrwl/exception.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.8/tldrwl/register.py` & `tldrwl-0.0.9/tldrwl/register.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.8/tldrwl/summarize.py` & `tldrwl-0.0.9/tldrwl/summarize.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.8/tldrwl/summarize_text.py` & `tldrwl-0.0.9/tldrwl/summarize_text.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.8/tldrwl/summarize_webpage.py` & `tldrwl-0.0.9/tldrwl/summarize_webpage.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.8/tldrwl/summarize_youtube.py` & `tldrwl-0.0.9/tldrwl/summarize_youtube.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.8/tldrwl.egg-info/PKG-INFO` & `tldrwl-0.0.9/tldrwl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tldrwl
-Version: 0.0.8
+Version: 0.0.9
 Summary: Too long, didn't read/watch/listen
 Home-page: https://github.com/jrodal98/tldrwl
 Author: Jacob Rodal
 Author-email: dev@jrodal.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

