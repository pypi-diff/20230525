# Comparing `tmp/ASTOCache-1.0.1.tar.gz` & `tmp/ASTOCache-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASTOCache-1.0.1.tar", last modified: Tue May 23 06:19:35 2023, max compression
+gzip compressed data, was "ASTOCache-1.0.2.tar", last modified: Thu May 25 09:14:28 2023, max compression
```

## Comparing `ASTOCache-1.0.1.tar` & `ASTOCache-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-23 06:19:35.534864 ASTOCache-1.0.1/
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-23 06:19:35.534864 ASTOCache-1.0.1/ASTOCache/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     5600 2023-05-23 06:12:00.000000 ASTOCache-1.0.1/ASTOCache/__init__.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1270 2023-05-23 05:06:02.000000 ASTOCache-1.0.1/ASTOCache/logger.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-23 06:19:35.534864 ASTOCache-1.0.1/ASTOCache.egg-info/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      610 2023-05-23 06:19:35.000000 ASTOCache-1.0.1/ASTOCache.egg-info/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      263 2023-05-23 06:19:35.000000 ASTOCache-1.0.1/ASTOCache.egg-info/SOURCES.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2023-05-23 06:19:35.000000 ASTOCache-1.0.1/ASTOCache.egg-info/dependency_links.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       43 2023-05-23 06:19:35.000000 ASTOCache-1.0.1/ASTOCache.egg-info/requires.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       10 2023-05-23 06:19:35.000000 ASTOCache-1.0.1/ASTOCache.egg-info/top_level.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       78 2023-05-22 13:09:12.000000 ASTOCache-1.0.1/CHANGELOG.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1070 2023-05-22 13:12:22.000000 ASTOCache-1.0.1/LICENCE.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       25 2023-05-22 13:10:04.000000 ASTOCache-1.0.1/MANIFEST.in
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      610 2023-05-23 06:19:35.534864 ASTOCache-1.0.1/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      115 2023-05-22 13:06:57.000000 ASTOCache-1.0.1/README.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       38 2023-05-23 06:19:35.534864 ASTOCache-1.0.1/setup.cfg
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      632 2023-05-23 06:19:20.000000 ASTOCache-1.0.1/setup.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-25 09:14:28.453415 ASTOCache-1.0.2/
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-25 09:14:28.453415 ASTOCache-1.0.2/ASTOCache/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     5600 2023-05-23 06:12:00.000000 ASTOCache-1.0.2/ASTOCache/__init__.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1515 2023-05-25 09:11:11.000000 ASTOCache-1.0.2/ASTOCache/logger.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-25 09:14:28.453415 ASTOCache-1.0.2/ASTOCache.egg-info/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      610 2023-05-25 09:14:28.000000 ASTOCache-1.0.2/ASTOCache.egg-info/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      263 2023-05-25 09:14:28.000000 ASTOCache-1.0.2/ASTOCache.egg-info/SOURCES.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2023-05-25 09:14:28.000000 ASTOCache-1.0.2/ASTOCache.egg-info/dependency_links.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       43 2023-05-25 09:14:28.000000 ASTOCache-1.0.2/ASTOCache.egg-info/requires.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       10 2023-05-25 09:14:28.000000 ASTOCache-1.0.2/ASTOCache.egg-info/top_level.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       78 2023-05-22 13:09:12.000000 ASTOCache-1.0.2/CHANGELOG.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1070 2023-05-22 13:12:22.000000 ASTOCache-1.0.2/LICENCE.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       25 2023-05-22 13:10:04.000000 ASTOCache-1.0.2/MANIFEST.in
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      610 2023-05-25 09:14:28.453415 ASTOCache-1.0.2/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      115 2023-05-22 13:06:57.000000 ASTOCache-1.0.2/README.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       38 2023-05-25 09:14:28.453415 ASTOCache-1.0.2/setup.cfg
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      632 2023-05-25 09:14:23.000000 ASTOCache-1.0.2/setup.py
```

### Comparing `ASTOCache-1.0.1/ASTOCache/__init__.py` & `ASTOCache-1.0.2/ASTOCache/__init__.py`

 * *Files identical despite different names*

### Comparing `ASTOCache-1.0.1/ASTOCache/logger.py` & `ASTOCache-1.0.2/ASTOCache/logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 import inspect
 from fluent import asyncsender
 import os
 import msgpack
 from io import BytesIO
+import sys
+import traceback
 
 
 fluentd_host = os.environ.get("fluent_host", "")
 fluentd_port = int(os.environ.get("fluent_port", 0))
 component_name = os.environ.get("component_name", "")
 
 
 def overflow_handler(pendings):
     unpacker = msgpack.Unpacker(BytesIO(pendings))
     for unpacked in unpacker:
         print(unpacked)
 
 def log_emmiter(msg, typ='INFO'):
-    #eval file name to log to from typ
-    sender = asyncsender.FluentSender(component_name, host=fluentd_host, port=fluentd_port, buffer_overflow_handler=overflow_handler)
-    sender.emit(typ, {"message": f"{msg}"})
-    sender.close()
+    try:
+        #eval file name to log to from typ
+        sender = asyncsender.FluentSender(component_name, host=fluentd_host, port=fluentd_port, buffer_overflow_handler=overflow_handler)
+        sender.emit(typ, {"message": f"{msg}"})
+        sender.close()
+    except:
+        e = sys.exc_info()
+        traceback_output = "".join(traceback.format_exception(e[0], e[1], e[2]))
+        print("Error occured in caching logger", str(traceback_output))
 
 def logger(fn, typ='INFO'):
     from functools import wraps
     from datetime import datetime, timezone
 
     @wraps(fn)
     def inner(*args, **kwargs):
```

### Comparing `ASTOCache-1.0.1/ASTOCache.egg-info/PKG-INFO` & `ASTOCache-1.0.2/ASTOCache.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASTOCache
-Version: 1.0.1
+Version: 1.0.2
 Summary: Caching the JSON request payload and the value in RedisQ
 Home-page: UNKNOWN
 Author: Aditya Kumar Singh
 Author-email: aditya.singh@netcorecloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `ASTOCache-1.0.1/LICENCE.txt` & `ASTOCache-1.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `ASTOCache-1.0.1/PKG-INFO` & `ASTOCache-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASTOCache
-Version: 1.0.1
+Version: 1.0.2
 Summary: Caching the JSON request payload and the value in RedisQ
 Home-page: UNKNOWN
 Author: Aditya Kumar Singh
 Author-email: aditya.singh@netcorecloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `ASTOCache-1.0.1/setup.py` & `ASTOCache-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   'Operating System :: OS Independent',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='ASTOCache',
-  version='1.0.1',
+  version='1.0.2',
   description='Caching the JSON request payload and the value in RedisQ',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Aditya Kumar Singh',
   author_email='aditya.singh@netcorecloud.com',
   license='MIT', 
   classifiers=classifiers,
```

