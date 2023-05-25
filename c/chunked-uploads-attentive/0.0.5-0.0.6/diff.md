# Comparing `tmp/chunked-uploads-attentive-0.0.5.tar.gz` & `tmp/chunked-uploads-attentive-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chunked-uploads-attentive-0.0.5.tar", last modified: Sat May 13 13:39:54 2023, max compression
+gzip compressed data, was "chunked-uploads-attentive-0.0.6.tar", last modified: Thu May 25 05:43:48 2023, max compression
```

## Comparing `chunked-uploads-attentive-0.0.5.tar` & `chunked-uploads-attentive-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 13:39:54.438647 chunked-uploads-attentive-0.0.5/
--rw-rw-rw-   0        0        0      478 2023-05-13 13:39:54.437647 chunked-uploads-attentive-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-13 13:39:54.438647 chunked-uploads-attentive-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      893 2023-05-13 13:38:48.000000 chunked-uploads-attentive-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-13 13:39:54.400646 chunked-uploads-attentive-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-13 13:39:54.410646 chunked-uploads-attentive-0.0.5/src/chunked_uploads_attentive.egg-info/
--rw-rw-rw-   0        0        0      478 2023-05-13 13:39:54.000000 chunked-uploads-attentive-0.0.5/src/chunked_uploads_attentive.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      527 2023-05-13 13:39:54.000000 chunked-uploads-attentive-0.0.5/src/chunked_uploads_attentive.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 13:39:54.000000 chunked-uploads-attentive-0.0.5/src/chunked_uploads_attentive.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-13 13:39:54.000000 chunked-uploads-attentive-0.0.5/src/chunked_uploads_attentive.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-13 13:39:54.000000 chunked-uploads-attentive-0.0.5/src/chunked_uploads_attentive.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-13 13:39:54.435650 chunked-uploads-attentive-0.0.5/src/uploads/
--rw-rw-rw-   0        0        0        0 2023-03-21 15:09:06.000000 chunked-uploads-attentive-0.0.5/src/uploads/__init__.py
--rw-rw-rw-   0        0        0      325 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.5/src/uploads/admin.py
--rw-rw-rw-   0        0        0      152 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.5/src/uploads/apps.py
--rw-rw-rw-   0        0        0      300 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.5/src/uploads/constants.py
--rw-rw-rw-   0        0        0      262 2023-02-13 12:36:18.000000 chunked-uploads-attentive-0.0.5/src/uploads/exceptions.py
--rw-rw-rw-   0        0        0     3853 2023-05-07 19:41:00.000000 chunked-uploads-attentive-0.0.5/src/uploads/models.py
--rw-rw-rw-   0        0        0      384 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.5/src/uploads/response.py
--rw-rw-rw-   0        0        0      578 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.5/src/uploads/serializers.py
--rw-rw-rw-   0        0        0     2417 2023-05-07 19:40:59.000000 chunked-uploads-attentive-0.0.5/src/uploads/settings.py
--rw-rw-rw-   0        0        0       63 2023-03-21 15:09:06.000000 chunked-uploads-attentive-0.0.5/src/uploads/tests.py
--rw-rw-rw-   0        0        0    12227 2023-05-12 19:57:30.000000 chunked-uploads-attentive-0.0.5/src/uploads/views.py
+drwxrwxrwx   0        0        0        0 2023-05-25 05:43:48.476237 chunked-uploads-attentive-0.0.6/
+-rw-rw-rw-   0        0        0      478 2023-05-25 05:43:48.476237 chunked-uploads-attentive-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-25 05:43:48.476237 chunked-uploads-attentive-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      925 2023-05-25 05:43:44.000000 chunked-uploads-attentive-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 05:43:48.439888 chunked-uploads-attentive-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 05:43:48.460600 chunked-uploads-attentive-0.0.6/src/chunked_uploads_attentive.egg-info/
+-rw-rw-rw-   0        0        0      478 2023-05-25 05:43:48.000000 chunked-uploads-attentive-0.0.6/src/chunked_uploads_attentive.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2023-05-25 05:43:48.000000 chunked-uploads-attentive-0.0.6/src/chunked_uploads_attentive.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 05:43:48.000000 chunked-uploads-attentive-0.0.6/src/chunked_uploads_attentive.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-25 05:43:48.000000 chunked-uploads-attentive-0.0.6/src/chunked_uploads_attentive.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 05:43:48.000000 chunked-uploads-attentive-0.0.6/src/chunked_uploads_attentive.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 05:43:48.476237 chunked-uploads-attentive-0.0.6/src/uploads/
+-rw-rw-rw-   0        0        0        0 2023-03-21 15:09:06.000000 chunked-uploads-attentive-0.0.6/src/uploads/__init__.py
+-rw-rw-rw-   0        0        0      325 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.6/src/uploads/admin.py
+-rw-rw-rw-   0        0        0      152 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.6/src/uploads/apps.py
+-rw-rw-rw-   0        0        0      300 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.6/src/uploads/constants.py
+-rw-rw-rw-   0        0        0      262 2023-02-13 12:36:18.000000 chunked-uploads-attentive-0.0.6/src/uploads/exceptions.py
+-rw-rw-rw-   0        0        0     3853 2023-05-07 19:41:00.000000 chunked-uploads-attentive-0.0.6/src/uploads/models.py
+-rw-rw-rw-   0        0        0      384 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.6/src/uploads/response.py
+-rw-rw-rw-   0        0        0      578 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.6/src/uploads/serializers.py
+-rw-rw-rw-   0        0        0     2417 2023-05-07 19:40:59.000000 chunked-uploads-attentive-0.0.6/src/uploads/settings.py
+-rw-rw-rw-   0        0        0       63 2023-03-21 15:09:06.000000 chunked-uploads-attentive-0.0.6/src/uploads/tests.py
+-rw-rw-rw-   0        0        0    12227 2023-05-12 19:57:30.000000 chunked-uploads-attentive-0.0.6/src/uploads/views.py
```

### Comparing `chunked-uploads-attentive-0.0.5/setup.py` & `chunked-uploads-attentive-0.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Chunked Upload of files on gcs using Django'
 LONG_DESCRIPTION = 'A package that allows to transfer files and resume in case of data failure'
 
 # Setting up
 setup(
     name="chunked-uploads-attentive",
     version=VERSION,
     author="Ayion",
     author_email="<ayan@attentive.ai>",
     description=DESCRIPTION,
     package_dir={'':'src'},
     packages=['uploads'],
-    install_requires=['django', 'djangorestframework'],
+    install_requires=['django', 'djangorestframework','google','google-cloud-storage'],
     keywords=['python', 'file', 'transfer', 'chunk', 'chunks', 'upload'],
     license='MIT',
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `chunked-uploads-attentive-0.0.5/src/chunked_uploads_attentive.egg-info/SOURCES.txt` & `chunked-uploads-attentive-0.0.6/src/chunked_uploads_attentive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chunked-uploads-attentive-0.0.5/src/uploads/models.py` & `chunked-uploads-attentive-0.0.6/src/uploads/models.py`

 * *Files identical despite different names*

### Comparing `chunked-uploads-attentive-0.0.5/src/uploads/serializers.py` & `chunked-uploads-attentive-0.0.6/src/uploads/serializers.py`

 * *Files identical despite different names*

### Comparing `chunked-uploads-attentive-0.0.5/src/uploads/settings.py` & `chunked-uploads-attentive-0.0.6/src/uploads/settings.py`

 * *Files identical despite different names*

### Comparing `chunked-uploads-attentive-0.0.5/src/uploads/views.py` & `chunked-uploads-attentive-0.0.6/src/uploads/views.py`

 * *Files identical despite different names*

