# Comparing `tmp/licensekeygentest-1.0.1.tar.gz` & `tmp/licensekeygentest-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "licensekeygentest-1.0.1.tar", last modified: Tue May 23 16:33:50 2023, max compression
+gzip compressed data, was "licensekeygentest-1.0.2.tar", last modified: Wed May 24 13:49:59 2023, max compression
```

## Comparing `licensekeygentest-1.0.1.tar` & `licensekeygentest-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-23 16:33:50.373928 licensekeygentest-1.0.1/
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     1063 2023-05-23 11:20:36.000000 licensekeygentest-1.0.1/LICENSE
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      699 2023-05-23 16:33:50.373928 licensekeygentest-1.0.1/PKG-INFO
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      152 2023-05-23 11:20:36.000000 licensekeygentest-1.0.1/README.md
-drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-23 16:33:50.369928 licensekeygentest-1.0.1/licensekeygentest/
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       43 2023-05-23 11:20:36.000000 licensekeygentest-1.0.1/licensekeygentest/__init__.py
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     2356 2023-05-23 16:31:06.000000 licensekeygentest-1.0.1/licensekeygentest/main.py
-drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-23 16:33:50.369928 licensekeygentest-1.0.1/licensekeygentest.egg-info/
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      699 2023-05-23 16:33:50.000000 licensekeygentest-1.0.1/licensekeygentest.egg-info/PKG-INFO
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      286 2023-05-23 16:33:50.000000 licensekeygentest-1.0.1/licensekeygentest.egg-info/SOURCES.txt
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)        1 2023-05-23 16:33:50.000000 licensekeygentest-1.0.1/licensekeygentest.egg-info/dependency_links.txt
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)        9 2023-05-23 16:33:50.000000 licensekeygentest-1.0.1/licensekeygentest.egg-info/requires.txt
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       18 2023-05-23 16:33:50.000000 licensekeygentest-1.0.1/licensekeygentest.egg-info/top_level.txt
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       38 2023-05-23 16:33:50.373928 licensekeygentest-1.0.1/setup.cfg
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     1063 2023-05-23 16:32:02.000000 licensekeygentest-1.0.1/setup.py
+drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-24 13:49:59.749889 licensekeygentest-1.0.2/
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     1063 2023-05-23 11:20:36.000000 licensekeygentest-1.0.2/LICENSE
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      699 2023-05-24 13:49:59.749889 licensekeygentest-1.0.2/PKG-INFO
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      152 2023-05-23 11:20:36.000000 licensekeygentest-1.0.2/README.md
+drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-24 13:49:59.741889 licensekeygentest-1.0.2/licensekeygentest/
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       43 2023-05-23 11:20:36.000000 licensekeygentest-1.0.2/licensekeygentest/__init__.py
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     2238 2023-05-24 13:48:02.000000 licensekeygentest-1.0.2/licensekeygentest/main.py
+drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-24 13:49:59.741889 licensekeygentest-1.0.2/licensekeygentest.egg-info/
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      699 2023-05-24 13:49:59.000000 licensekeygentest-1.0.2/licensekeygentest.egg-info/PKG-INFO
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      286 2023-05-24 13:49:59.000000 licensekeygentest-1.0.2/licensekeygentest.egg-info/SOURCES.txt
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)        1 2023-05-24 13:49:59.000000 licensekeygentest-1.0.2/licensekeygentest.egg-info/dependency_links.txt
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)        9 2023-05-24 13:49:59.000000 licensekeygentest-1.0.2/licensekeygentest.egg-info/requires.txt
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       18 2023-05-24 13:49:59.000000 licensekeygentest-1.0.2/licensekeygentest.egg-info/top_level.txt
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       38 2023-05-24 13:49:59.749889 licensekeygentest-1.0.2/setup.cfg
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     1063 2023-05-24 13:48:37.000000 licensekeygentest-1.0.2/setup.py
```

### Comparing `licensekeygentest-1.0.1/LICENSE` & `licensekeygentest-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `licensekeygentest-1.0.1/PKG-INFO` & `licensekeygentest-1.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensekeygentest
-Version: 1.0.1
+Version: 1.0.2
 Summary: POC for license validation checks
 Author: Rahul R
 Author-email: <rahulranjan25.RR@gmail.com>
 Keywords: python,authentication,licensing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `licensekeygentest-1.0.1/licensekeygentest/main.py` & `licensekeygentest-1.0.2/licensekeygentest/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 import threading, _thread
 import requests
 import json
 import time
 
 class library():
 
-  def __init__(self, license_key, email):
-    checkValidation = threading.Thread(target=self.validate, args=[license_key, email])
+  def __init__(self, license_key, email, debug=False):
+    checkValidation = threading.Thread(target=self.validate, args=[license_key, email, debug])
     checkValidation.start()
 
-  def validate(self, license_key, email):
+  def validate(self, license_key, email, debug):
     while (True):
       try:
         validation = requests.get(
           f"https://licensing.sr.flipr.ai/api/actions/validate/",
           headers={
             "Content-Type": "application/json",
             "Accept": "application/json"
           },
           data=json.dumps({
             "email": f"{email}",
             "key": f"{license_key}"
           })
         )
         validation_code = validation.json()
-        # CASE: DEBUG Only
-        print(f"[{validation.status_code}] Response >> Status:", validation_code)
+        if debug:
+          print(f"[{validation.status_code}] Response >> Status:", validation_code)
 
         if (validation.status_code != '200'):
+          if (validation.status_code/400 == 1):
+            _thread.interrupt_main()
+
           invalid_code =  validation_code == "SUSPENDED" or \
                           validation_code == "INVALID"   or \
                           validation_code == "EXPIRED"   or \
                           validation_code == "USER_SCOPE_MISMATCH"
 
           if invalid_code:
             _thread.interrupt_main()
@@ -51,15 +54,10 @@
         raise Exception("License validation request could not be made. Please make sure you are connected to the internet.\n")
 
 
   def some_other_process(self):
     counter = 0;
     while True:
       time.sleep(1)
-      print(f"Main thread counter: {counter}")
+      print(f"Main thread: {counter}")
       counter+=1
 
-
-testing = library(email="double.r4rahulandranjan.v1.2@gmail.com", 
-              license_key="ajOt0VLJjcOhN+5UFGo94Qs8lcBCxU9EMBLt1rDvNObDvBUlfx8flhs0mSeE/AQ0T1CGBhImtUeMoNm/Nnv3UQ==")
-
-testing.some_other_process()
```

### Comparing `licensekeygentest-1.0.1/licensekeygentest.egg-info/PKG-INFO` & `licensekeygentest-1.0.2/licensekeygentest.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensekeygentest
-Version: 1.0.1
+Version: 1.0.2
 Summary: POC for license validation checks
 Author: Rahul R
 Author-email: <rahulranjan25.RR@gmail.com>
 Keywords: python,authentication,licensing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `licensekeygentest-1.0.1/setup.py` & `licensekeygentest-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'POC for license validation checks'
 LONG_DESCRIPTION = 'A POC package that allows lisencing of python libraries.'
 
 # Setting up
 setup(
     name="licensekeygentest",
     version=VERSION,
```

