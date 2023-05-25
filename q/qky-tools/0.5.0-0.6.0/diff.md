# Comparing `tmp/qky-tools-0.5.0.tar.gz` & `tmp/qky-tools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qky-tools-0.5.0.tar", last modified: Wed May 24 00:07:22 2023, max compression
+gzip compressed data, was "qky-tools-0.6.0.tar", last modified: Thu May 25 03:12:07 2023, max compression
```

## Comparing `qky-tools-0.5.0.tar` & `qky-tools-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 00:07:22.381207 qky-tools-0.5.0/
--rw-rw-rw-   0        0        0     1088 2023-05-18 00:09:54.000000 qky-tools-0.5.0/LICENSE.txt
--rw-rw-rw-   0        0        0      690 2023-05-24 00:07:22.380209 qky-tools-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-18 00:10:33.000000 qky-tools-0.5.0/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 00:07:22.324359 qky-tools-0.5.0/qky_tools/
--rw-rw-rw-   0        0        0       84 2023-05-22 06:07:16.000000 qky-tools-0.5.0/qky_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 00:07:22.362257 qky-tools-0.5.0/qky_tools/db_tools/
--rw-rw-rw-   0        0        0     5338 2023-05-18 00:24:47.000000 qky-tools-0.5.0/qky_tools/db_tools/MySQL.py
--rw-rw-rw-   0        0        0       42 2023-05-22 06:05:29.000000 qky-tools-0.5.0/qky_tools/db_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 00:07:22.378244 qky-tools-0.5.0/qky_tools/req_tools/
--rw-rw-rw-   0        0        0       90 2023-05-22 06:06:52.000000 qky-tools-0.5.0/qky_tools/req_tools/__init__.py
--rw-rw-rw-   0        0        0     3678 2023-05-24 00:06:05.000000 qky-tools-0.5.0/qky_tools/req_tools/cacheReq.py
--rw-rw-rw-   0        0        0      191 2023-05-18 01:01:36.000000 qky-tools-0.5.0/qky_tools/req_tools/proxyReq.py
-drwxrwxrwx   0        0        0        0 2023-05-24 00:07:22.348323 qky-tools-0.5.0/qky_tools.egg-info/
--rw-rw-rw-   0        0        0      690 2023-05-24 00:07:22.000000 qky-tools-0.5.0/qky_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-05-24 00:07:22.000000 qky-tools-0.5.0/qky_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 00:07:22.000000 qky-tools-0.5.0/qky_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-24 00:07:22.000000 qky-tools-0.5.0/qky_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-24 00:07:22.000000 qky-tools-0.5.0/qky_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 00:07:22.381207 qky-tools-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     3932 2023-05-24 00:07:14.000000 qky-tools-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 03:12:07.789606 qky-tools-0.6.0/
+-rw-rw-rw-   0        0        0     1088 2023-05-18 00:09:54.000000 qky-tools-0.6.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      690 2023-05-25 03:12:07.788609 qky-tools-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-18 00:10:33.000000 qky-tools-0.6.0/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 03:12:07.721696 qky-tools-0.6.0/qky_tools/
+-rw-rw-rw-   0        0        0       84 2023-05-22 06:07:16.000000 qky-tools-0.6.0/qky_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 03:12:07.762680 qky-tools-0.6.0/qky_tools/db_tools/
+-rw-rw-rw-   0        0        0     5338 2023-05-18 00:24:47.000000 qky-tools-0.6.0/qky_tools/db_tools/MySQL.py
+-rw-rw-rw-   0        0        0       42 2023-05-22 06:05:29.000000 qky-tools-0.6.0/qky_tools/db_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 03:12:07.785617 qky-tools-0.6.0/qky_tools/req_tools/
+-rw-rw-rw-   0        0        0       90 2023-05-22 06:06:52.000000 qky-tools-0.6.0/qky_tools/req_tools/__init__.py
+-rw-rw-rw-   0        0        0     3678 2023-05-24 00:06:05.000000 qky-tools-0.6.0/qky_tools/req_tools/cacheReq.py
+-rw-rw-rw-   0        0        0      191 2023-05-18 01:01:36.000000 qky-tools-0.6.0/qky_tools/req_tools/proxyReq.py
+drwxrwxrwx   0        0        0        0 2023-05-25 03:12:07.787611 qky-tools-0.6.0/qky_tools/str_tools/
+-rw-rw-rw-   0        0        0        0 2023-05-25 03:05:26.000000 qky-tools-0.6.0/qky_tools/str_tools/__init__.py
+-rw-rw-rw-   0        0        0      469 2023-05-25 03:11:40.000000 qky-tools-0.6.0/qky_tools/str_tools/chinese_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-25 03:12:07.748715 qky-tools-0.6.0/qky_tools.egg-info/
+-rw-rw-rw-   0        0        0      690 2023-05-25 03:12:07.000000 qky-tools-0.6.0/qky_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2023-05-25 03:12:07.000000 qky-tools-0.6.0/qky_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 03:12:07.000000 qky-tools-0.6.0/qky_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-25 03:12:07.000000 qky-tools-0.6.0/qky_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-25 03:12:07.000000 qky-tools-0.6.0/qky_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 03:12:07.789606 qky-tools-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     3946 2023-05-25 03:11:51.000000 qky-tools-0.6.0/setup.py
```

### Comparing `qky-tools-0.5.0/LICENSE.txt` & `qky-tools-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qky-tools-0.5.0/PKG-INFO` & `qky-tools-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qky-tools
-Version: 0.5.0
+Version: 0.6.0
 Summary: python tools collection
 Home-page: https://github.com/qiaokuoyuan/py-tools
 Author: qiaokuoyuan
 Author-email: 457361577@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qky-tools-0.5.0/qky_tools/db_tools/MySQL.py` & `qky-tools-0.6.0/qky_tools/db_tools/MySQL.py`

 * *Files identical despite different names*

### Comparing `qky-tools-0.5.0/qky_tools/req_tools/cacheReq.py` & `qky-tools-0.6.0/qky_tools/req_tools/cacheReq.py`

 * *Files identical despite different names*

### Comparing `qky-tools-0.5.0/qky_tools.egg-info/PKG-INFO` & `qky-tools-0.6.0/qky_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qky-tools
-Version: 0.5.0
+Version: 0.6.0
 Summary: python tools collection
 Home-page: https://github.com/qiaokuoyuan/py-tools
 Author: qiaokuoyuan
 Author-email: 457361577@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qky-tools-0.5.0/setup.py` & `qky-tools-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 # Package meta-data.
 NAME = 'qky-tools'
 DESCRIPTION = 'python tools collection'
 URL = 'https://github.com/qiaokuoyuan/py-tools'
 EMAIL = '457361577@qq.com'
 AUTHOR = 'qiaokuoyuan'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.5.0'
+VERSION = '0.6.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
-    'pymysql', 'nanoid'
+    'pymysql', 'nanoid','cachetools '
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

