# Comparing `tmp/aanalyticsact-0.0.0.8.tar.gz` & `tmp/aanalyticsact-0.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\aanalyticsact-0.0.0.8.tar", last modified: Mon Jan 17 15:42:22 2022, max compression
+gzip compressed data, was "dist\aanalyticsact-0.0.0.9.tar", last modified: Mon Jan 17 18:20:45 2022, max compression
```

## Comparing `aanalyticsact-0.0.0.8.tar` & `aanalyticsact-0.0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-01-17 15:42:22.490519 aanalyticsact-0.0.0.8/
--rw-rw-rw-   0        0        0     1365 2022-01-17 15:42:22.491521 aanalyticsact-0.0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      735 2021-09-15 04:51:09.000000 aanalyticsact-0.0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-01-17 15:42:22.451513 aanalyticsact-0.0.0.8/aanalyticsact/
--rw-rw-rw-   0        0        0      176 2022-01-17 15:38:59.000000 aanalyticsact-0.0.0.8/aanalyticsact/__init__.py
--rw-rw-rw-   0        0        0       23 2022-01-17 15:39:09.000000 aanalyticsact-0.0.0.8/aanalyticsact/__version__.py
--rw-rw-rw-   0        0        0     6271 2022-01-17 15:37:58.000000 aanalyticsact-0.0.0.8/aanalyticsact/actCreateSeg.py
--rw-rw-rw-   0        0        0     3237 2021-09-18 12:06:32.000000 aanalyticsact-0.0.0.8/aanalyticsact/actExecute.py
--rw-rw-rw-   0        0        0    11388 2022-01-17 15:36:39.000000 aanalyticsact-0.0.0.8/aanalyticsact/actModuler.py
--rw-rw-rw-   0        0        0     7234 2021-09-18 12:01:58.000000 aanalyticsact-0.0.0.8/aanalyticsact/actRunner.py
--rw-rw-rw-   0        0        0     3400 2022-01-17 15:37:46.000000 aanalyticsact-0.0.0.8/aanalyticsact/actUpdateSeg.py
-drwxrwxrwx   0        0        0        0 2022-01-17 15:42:22.488519 aanalyticsact-0.0.0.8/aanalyticsact.egg-info/
--rw-rw-rw-   0        0        0     1365 2022-01-17 15:42:22.000000 aanalyticsact-0.0.0.8/aanalyticsact.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2022-01-17 15:42:22.000000 aanalyticsact-0.0.0.8/aanalyticsact.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-17 15:42:22.000000 aanalyticsact-0.0.0.8/aanalyticsact.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2022-01-17 15:42:22.000000 aanalyticsact-0.0.0.8/aanalyticsact.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-01-17 15:42:22.494521 aanalyticsact-0.0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      689 2022-01-17 15:39:06.000000 aanalyticsact-0.0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-17 18:20:45.470867 aanalyticsact-0.0.0.9/
+-rw-rw-rw-   0        0        0     1419 2022-01-17 18:20:45.470867 aanalyticsact-0.0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      765 2022-01-17 15:45:46.000000 aanalyticsact-0.0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-01-17 18:20:45.454864 aanalyticsact-0.0.0.9/aanalyticsact/
+-rw-rw-rw-   0        0        0      176 2022-01-17 15:38:59.000000 aanalyticsact-0.0.0.9/aanalyticsact/__init__.py
+-rw-rw-rw-   0        0        0       23 2022-01-17 18:20:17.000000 aanalyticsact-0.0.0.9/aanalyticsact/__version__.py
+-rw-rw-rw-   0        0        0     6271 2022-01-17 15:37:58.000000 aanalyticsact-0.0.0.9/aanalyticsact/actCreateSeg.py
+-rw-rw-rw-   0        0        0     3237 2021-09-18 12:06:32.000000 aanalyticsact-0.0.0.9/aanalyticsact/actExecute.py
+-rw-rw-rw-   0        0        0    11388 2022-01-17 18:20:23.000000 aanalyticsact-0.0.0.9/aanalyticsact/actModuler.py
+-rw-rw-rw-   0        0        0     7234 2021-09-18 12:01:58.000000 aanalyticsact-0.0.0.9/aanalyticsact/actRunner.py
+-rw-rw-rw-   0        0        0     3506 2022-01-17 18:20:26.000000 aanalyticsact-0.0.0.9/aanalyticsact/actUpdateSeg.py
+drwxrwxrwx   0        0        0        0 2022-01-17 18:20:45.467866 aanalyticsact-0.0.0.9/aanalyticsact.egg-info/
+-rw-rw-rw-   0        0        0     1419 2022-01-17 18:20:45.000000 aanalyticsact-0.0.0.9/aanalyticsact.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2022-01-17 18:20:45.000000 aanalyticsact-0.0.0.9/aanalyticsact.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-17 18:20:45.000000 aanalyticsact-0.0.0.9/aanalyticsact.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2022-01-17 18:20:45.000000 aanalyticsact-0.0.0.9/aanalyticsact.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2022-01-17 18:20:45.472867 aanalyticsact-0.0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      689 2022-01-17 18:20:20.000000 aanalyticsact-0.0.0.9/setup.py
```

### Comparing `aanalyticsact-0.0.0.8/PKG-INFO` & `aanalyticsact-0.0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aanalyticsact
-Version: 0.0.0.8
+Version: 0.0.0.9
 Summary: adobe analytics library for Team ACT
 Home-page: https://github.com/SunkyeongLee/aanalyticsact
 Author: Sunkyeong Lee
 Author-email: sunkyong9768@gmail.com
 License: UNKNOWN
 Description: Adobe Analytics for Team ACT v.0.0.1
         ==============
@@ -16,15 +16,18 @@
         
           
         ## Functionalities
         
         
         * Retrieve Daily, Weekly, Monthly data and automatically dumps into the DB connected in their local machine.
         * Capable up to 2nd breakdown.
-        * Automatically retrieves data of all Reporting Suites.<br/><br/>
+        * Automatically retrieves data of all Reporting Suites.
+        * Update Segments
+        * Create Segments
+        
         
         More functionalities will be added in sooner time.<br/><br/>
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aanalyticsact-0.0.0.8/README.md` & `aanalyticsact-0.0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,10 +8,13 @@
 
   
 ## Functionalities
 
 
 * Retrieve Daily, Weekly, Monthly data and automatically dumps into the DB connected in their local machine.
 * Capable up to 2nd breakdown.
-* Automatically retrieves data of all Reporting Suites.<br/><br/>
+* Automatically retrieves data of all Reporting Suites.
+* Update Segments
+* Create Segments
+
 
 More functionalities will be added in sooner time.<br/><br/>
```

### Comparing `aanalyticsact-0.0.0.8/aanalyticsact/actCreateSeg.py` & `aanalyticsact-0.0.0.9/aanalyticsact/actCreateSeg.py`

 * *Files identical despite different names*

### Comparing `aanalyticsact-0.0.0.8/aanalyticsact/actExecute.py` & `aanalyticsact-0.0.0.9/aanalyticsact/actExecute.py`

 * *Files identical despite different names*

### Comparing `aanalyticsact-0.0.0.8/aanalyticsact/actModuler.py` & `aanalyticsact-0.0.0.9/aanalyticsact/actModuler.py`

 * *Files identical despite different names*

### Comparing `aanalyticsact-0.0.0.8/aanalyticsact/actRunner.py` & `aanalyticsact-0.0.0.9/aanalyticsact/actRunner.py`

 * *Files identical despite different names*

### Comparing `aanalyticsact-0.0.0.8/aanalyticsact/actUpdateSeg.py` & `aanalyticsact-0.0.0.9/aanalyticsact/actUpdateSeg.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,27 @@
 
 from copy import deepcopy
 import aanalytics2 as api2
 import json
 from itertools import *
 from sqlalchemy import create_engine
 import pandas as pd
-import actCreateSeg as cs
+from .actCreateSeg import *
 import time
 from ast import literal_eval
 
+
+def dataInitiator():
+    api2.configure()
+    logger = api2.Login() 
+    logger.connector.config
+
+
 def updateSegment(segmentID, jsonFile):
-    cs.dataInitiator()
+    dataInitiator()
     cid = "samsun0"
     ags = api2.Analytics(cid)
     ags.header
 
     createSeg = ags.updateSegment(segmentID, jsonFile)
     
     return createSeg
```

### Comparing `aanalyticsact-0.0.0.8/aanalyticsact.egg-info/PKG-INFO` & `aanalyticsact-0.0.0.9/aanalyticsact.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aanalyticsact
-Version: 0.0.0.8
+Version: 0.0.0.9
 Summary: adobe analytics library for Team ACT
 Home-page: https://github.com/SunkyeongLee/aanalyticsact
 Author: Sunkyeong Lee
 Author-email: sunkyong9768@gmail.com
 License: UNKNOWN
 Description: Adobe Analytics for Team ACT v.0.0.1
         ==============
@@ -16,15 +16,18 @@
         
           
         ## Functionalities
         
         
         * Retrieve Daily, Weekly, Monthly data and automatically dumps into the DB connected in their local machine.
         * Capable up to 2nd breakdown.
-        * Automatically retrieves data of all Reporting Suites.<br/><br/>
+        * Automatically retrieves data of all Reporting Suites.
+        * Update Segments
+        * Create Segments
+        
         
         More functionalities will be added in sooner time.<br/><br/>
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aanalyticsact-0.0.0.8/setup.py` & `aanalyticsact-0.0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aanalyticsact",
-    version="0.0.0.8",
+    version="0.0.0.9",
     author="Sunkyeong Lee",
     author_email="sunkyong9768@gmail.com",
     description="adobe analytics library for Team ACT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SunkyeongLee/aanalyticsact",
     packages=setuptools.find_packages(),
```

