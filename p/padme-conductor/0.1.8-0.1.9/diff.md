# Comparing `tmp/padme-conductor-0.1.8.tar.gz` & `tmp/padme-conductor-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "padme-conductor-0.1.8.tar", last modified: Thu May 25 20:53:33 2023, max compression
+gzip compressed data, was "padme-conductor-0.1.9.tar", last modified: Thu May 25 20:58:36 2023, max compression
```

## Comparing `padme-conductor-0.1.8.tar` & `padme-conductor-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-05-25 20:53:33.811158 padme-conductor-0.1.8/
--rw-r--r--   0 martin    (1000) martin    (1000)     1069 2023-03-30 09:44:42.000000 padme-conductor-0.1.8/LICENSE
--rw-r--r--   0 martin    (1000) martin    (1000)       26 2023-03-30 09:44:42.000000 padme-conductor-0.1.8/MANIFEST.in
--rw-r--r--   0 martin    (1000) martin    (1000)     5346 2023-05-25 20:53:33.811158 padme-conductor-0.1.8/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)     4856 2023-05-25 20:50:07.000000 padme-conductor-0.1.8/README.md
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-05-25 20:53:33.801158 padme-conductor-0.1.8/padme_conductor/
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-05-25 20:53:33.811158 padme-conductor-0.1.8/padme_conductor/Plugins/
--rw-r--r--   0 martin    (1000) martin    (1000)      338 2023-03-30 09:44:42.000000 padme-conductor-0.1.8/padme_conductor/Plugins/DatabasePlugin.py
--rw-r--r--   0 martin    (1000) martin    (1000)      781 2023-03-30 09:46:10.000000 padme-conductor-0.1.8/padme_conductor/Plugins/FHIR.py
--rw-r--r--   0 martin    (1000) martin    (1000)      774 2023-03-30 09:44:42.000000 padme-conductor-0.1.8/padme_conductor/Plugins/MinIO.py
--rw-r--r--   0 martin    (1000) martin    (1000)      902 2023-03-30 09:44:42.000000 padme-conductor-0.1.8/padme_conductor/Plugins/SQL.py
--rw-r--r--   0 martin    (1000) martin    (1000)      226 2023-03-30 09:44:42.000000 padme-conductor-0.1.8/padme_conductor/Plugins/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1000)      513 2023-03-30 09:45:50.000000 padme-conductor-0.1.8/padme_conductor/Query.py
--rw-r--r--   0 martin    (1000) martin    (1000)      122 2023-03-30 09:44:42.000000 padme-conductor-0.1.8/padme_conductor/Separation.py
--rw-r--r--   0 martin    (1000) martin    (1000)     2101 2023-03-30 09:44:42.000000 padme-conductor-0.1.8/padme_conductor/TrainLogger.py
--rw-r--r--   0 martin    (1000) martin    (1000)      705 2023-03-30 09:44:42.000000 padme-conductor-0.1.8/padme_conductor/_TrainTagFormatter.py
--rw-r--r--   0 martin    (1000) martin    (1000)      356 2023-03-30 09:44:42.000000 padme-conductor-0.1.8/padme_conductor/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1000)      545 2023-03-30 09:44:42.000000 padme-conductor-0.1.8/padme_conductor/constants.py
--rw-r--r--   0 martin    (1000) martin    (1000)     7105 2023-03-30 09:44:42.000000 padme-conductor-0.1.8/padme_conductor/padme_conductor.py
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-05-25 20:53:33.801158 padme-conductor-0.1.8/padme_conductor.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1000)     5346 2023-05-25 20:53:33.000000 padme-conductor-0.1.8/padme_conductor.egg-info/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)      637 2023-05-25 20:53:33.000000 padme-conductor-0.1.8/padme_conductor.egg-info/SOURCES.txt
--rw-r--r--   0 martin    (1000) martin    (1000)        1 2023-05-25 20:53:33.000000 padme-conductor-0.1.8/padme_conductor.egg-info/dependency_links.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       23 2023-05-25 20:53:33.000000 padme-conductor-0.1.8/padme_conductor.egg-info/requires.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       16 2023-05-25 20:53:33.000000 padme-conductor-0.1.8/padme_conductor.egg-info/top_level.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       96 2023-03-30 09:44:42.000000 padme-conductor-0.1.8/pyproject.toml
--rw-r--r--   0 martin    (1000) martin    (1000)       38 2023-05-25 20:53:33.811158 padme-conductor-0.1.8/setup.cfg
--rw-r--r--   0 martin    (1000) martin    (1000)      723 2023-05-25 20:51:45.000000 padme-conductor-0.1.8/setup.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-05-25 20:58:36.821156 padme-conductor-0.1.9/
+-rw-r--r--   0 martin    (1000) martin    (1000)     1069 2023-03-30 09:44:42.000000 padme-conductor-0.1.9/LICENSE
+-rw-r--r--   0 martin    (1000) martin    (1000)       26 2023-03-30 09:44:42.000000 padme-conductor-0.1.9/MANIFEST.in
+-rw-r--r--   0 martin    (1000) martin    (1000)     5406 2023-05-25 20:58:36.821156 padme-conductor-0.1.9/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)     4916 2023-05-25 20:58:25.000000 padme-conductor-0.1.9/README.md
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-05-25 20:58:36.811156 padme-conductor-0.1.9/padme_conductor/
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-05-25 20:58:36.821156 padme-conductor-0.1.9/padme_conductor/Plugins/
+-rw-r--r--   0 martin    (1000) martin    (1000)      338 2023-03-30 09:44:42.000000 padme-conductor-0.1.9/padme_conductor/Plugins/DatabasePlugin.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      781 2023-03-30 09:46:10.000000 padme-conductor-0.1.9/padme_conductor/Plugins/FHIR.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      774 2023-03-30 09:44:42.000000 padme-conductor-0.1.9/padme_conductor/Plugins/MinIO.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      902 2023-03-30 09:44:42.000000 padme-conductor-0.1.9/padme_conductor/Plugins/SQL.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      226 2023-03-30 09:44:42.000000 padme-conductor-0.1.9/padme_conductor/Plugins/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      513 2023-03-30 09:45:50.000000 padme-conductor-0.1.9/padme_conductor/Query.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      122 2023-03-30 09:44:42.000000 padme-conductor-0.1.9/padme_conductor/Separation.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     2101 2023-03-30 09:44:42.000000 padme-conductor-0.1.9/padme_conductor/TrainLogger.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      705 2023-03-30 09:44:42.000000 padme-conductor-0.1.9/padme_conductor/_TrainTagFormatter.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      356 2023-03-30 09:44:42.000000 padme-conductor-0.1.9/padme_conductor/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      545 2023-03-30 09:44:42.000000 padme-conductor-0.1.9/padme_conductor/constants.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     7105 2023-03-30 09:44:42.000000 padme-conductor-0.1.9/padme_conductor/padme_conductor.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-05-25 20:58:36.811156 padme-conductor-0.1.9/padme_conductor.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1000)     5406 2023-05-25 20:58:36.000000 padme-conductor-0.1.9/padme_conductor.egg-info/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)      637 2023-05-25 20:58:36.000000 padme-conductor-0.1.9/padme_conductor.egg-info/SOURCES.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)        1 2023-05-25 20:58:36.000000 padme-conductor-0.1.9/padme_conductor.egg-info/dependency_links.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       23 2023-05-25 20:58:36.000000 padme-conductor-0.1.9/padme_conductor.egg-info/requires.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       16 2023-05-25 20:58:36.000000 padme-conductor-0.1.9/padme_conductor.egg-info/top_level.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       96 2023-03-30 09:44:42.000000 padme-conductor-0.1.9/pyproject.toml
+-rw-r--r--   0 martin    (1000) martin    (1000)       38 2023-05-25 20:58:36.821156 padme-conductor-0.1.9/setup.cfg
+-rw-r--r--   0 martin    (1000) martin    (1000)      723 2023-05-25 20:56:53.000000 padme-conductor-0.1.9/setup.py
```

### Comparing `padme-conductor-0.1.8/LICENSE` & `padme-conductor-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `padme-conductor-0.1.8/PKG-INFO` & `padme-conductor-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: padme-conductor
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library which supports the creation of so-called Trains for the Personal Health Train infrastructure.
 Home-page: https://github.com/sawelt/padme-conductor
 Author: Martin Goerz, Sascha Welten
 Author-email: welten@dbis.rwth-aachen.de
 License: UNKNOWN
 Keywords: Personal Health Train,PADME
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PADME Conductor Library
 
 <p align="center">
-    <img src="./logo.svg" width=220>
+    <img src="https://raw.githubusercontent.com/sawelt/padme-conductor/main/logo.svg" width=220>
 </p>
 
 A library to simplify the interactions with the Personal Health Train (PHT) and its Stations.
 
 
 ## Connection Parameters
```

### Comparing `padme-conductor-0.1.8/README.md` & `padme-conductor-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # PADME Conductor Library
 
 <p align="center">
-    <img src="./logo.svg" width=220>
+    <img src="https://raw.githubusercontent.com/sawelt/padme-conductor/main/logo.svg" width=220>
 </p>
 
 A library to simplify the interactions with the Personal Health Train (PHT) and its Stations.
 
 
 ## Connection Parameters
```

### Comparing `padme-conductor-0.1.8/padme_conductor/Plugins/FHIR.py` & `padme-conductor-0.1.9/padme_conductor/Plugins/FHIR.py`

 * *Files identical despite different names*

### Comparing `padme-conductor-0.1.8/padme_conductor/Plugins/MinIO.py` & `padme-conductor-0.1.9/padme_conductor/Plugins/MinIO.py`

 * *Files identical despite different names*

### Comparing `padme-conductor-0.1.8/padme_conductor/Plugins/SQL.py` & `padme-conductor-0.1.9/padme_conductor/Plugins/SQL.py`

 * *Files identical despite different names*

### Comparing `padme-conductor-0.1.8/padme_conductor/Query.py` & `padme-conductor-0.1.9/padme_conductor/Query.py`

 * *Files identical despite different names*

### Comparing `padme-conductor-0.1.8/padme_conductor/TrainLogger.py` & `padme-conductor-0.1.9/padme_conductor/TrainLogger.py`

 * *Files identical despite different names*

### Comparing `padme-conductor-0.1.8/padme_conductor/_TrainTagFormatter.py` & `padme-conductor-0.1.9/padme_conductor/_TrainTagFormatter.py`

 * *Files identical despite different names*

### Comparing `padme-conductor-0.1.8/padme_conductor/constants.py` & `padme-conductor-0.1.9/padme_conductor/constants.py`

 * *Files identical despite different names*

### Comparing `padme-conductor-0.1.8/padme_conductor/padme_conductor.py` & `padme-conductor-0.1.9/padme_conductor/padme_conductor.py`

 * *Files identical despite different names*

### Comparing `padme-conductor-0.1.8/padme_conductor.egg-info/PKG-INFO` & `padme-conductor-0.1.9/padme_conductor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: padme-conductor
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library which supports the creation of so-called Trains for the Personal Health Train infrastructure.
 Home-page: https://github.com/sawelt/padme-conductor
 Author: Martin Goerz, Sascha Welten
 Author-email: welten@dbis.rwth-aachen.de
 License: UNKNOWN
 Keywords: Personal Health Train,PADME
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PADME Conductor Library
 
 <p align="center">
-    <img src="./logo.svg" width=220>
+    <img src="https://raw.githubusercontent.com/sawelt/padme-conductor/main/logo.svg" width=220>
 </p>
 
 A library to simplify the interactions with the Personal Health Train (PHT) and its Stations.
 
 
 ## Connection Parameters
```

### Comparing `padme-conductor-0.1.8/padme_conductor.egg-info/SOURCES.txt` & `padme-conductor-0.1.9/padme_conductor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `padme-conductor-0.1.8/setup.py` & `padme-conductor-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="padme-conductor",
-    version="0.1.8",
+    version="0.1.9",
     description="A library which supports the creation of so-called Trains for the Personal Health Train infrastructure.",
     py_modules=["padme_conductor"],
     packages=find_packages(),
     author="Martin Goerz, Sascha Welten",
     author_email="welten@dbis.rwth-aachen.de",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

