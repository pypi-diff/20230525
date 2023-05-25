# Comparing `tmp/pycliwrapper-0.1.tar.gz` & `tmp/pycliwrapper-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycliwrapper-0.1.tar", last modified: Thu May 25 14:27:31 2023, max compression
+gzip compressed data, was "pycliwrapper-0.2.tar", last modified: Thu May 25 14:39:30 2023, max compression
```

## Comparing `pycliwrapper-0.1.tar` & `pycliwrapper-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-25 14:27:31.760919 pycliwrapper-0.1/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      718 2023-05-25 14:27:31.760919 pycliwrapper-0.1/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      299 2023-05-25 14:23:47.000000 pycliwrapper-0.1/README.md
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-25 14:27:31.760919 pycliwrapper-0.1/pycliwrapper.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      718 2023-05-25 14:27:31.000000 pycliwrapper-0.1/pycliwrapper.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      162 2023-05-25 14:27:31.000000 pycliwrapper-0.1/pycliwrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-05-25 14:27:31.000000 pycliwrapper-0.1/pycliwrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-05-25 14:27:31.000000 pycliwrapper-0.1/pycliwrapper.egg-info/top_level.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-05-25 14:27:31.760919 pycliwrapper-0.1/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      643 2023-05-25 14:23:47.000000 pycliwrapper-0.1/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-25 14:39:30.066398 pycliwrapper-0.2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      718 2023-05-25 14:39:30.066398 pycliwrapper-0.2/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      299 2023-05-25 14:23:47.000000 pycliwrapper-0.2/README.md
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-25 14:39:30.066398 pycliwrapper-0.2/pycliwrapper.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      718 2023-05-25 14:39:29.000000 pycliwrapper-0.2/pycliwrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      162 2023-05-25 14:39:29.000000 pycliwrapper-0.2/pycliwrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-05-25 14:39:29.000000 pycliwrapper-0.2/pycliwrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-05-25 14:39:29.000000 pycliwrapper-0.2/pycliwrapper.egg-info/top_level.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-05-25 14:39:30.066398 pycliwrapper-0.2/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      628 2023-05-25 14:39:00.000000 pycliwrapper-0.2/setup.py
```

### Comparing `pycliwrapper-0.1/PKG-INFO` & `pycliwrapper-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycliwrapper
-Version: 0.1
+Version: 0.2
 Summary: Wrap any CLI tool to Python like syntax
 Home-page: UNKNOWN
 Author: Jordi Deu-Pons
 License: Apache License 2.0
 Keywords: cli,wrapper
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycliwrapper-0.1/pycliwrapper.egg-info/PKG-INFO` & `pycliwrapper-0.2/pycliwrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycliwrapper
-Version: 0.1
+Version: 0.2
 Summary: Wrap any CLI tool to Python like syntax
 Home-page: UNKNOWN
 Author: Jordi Deu-Pons
 License: Apache License 2.0
 Keywords: cli,wrapper
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycliwrapper-0.1/setup.py` & `pycliwrapper-0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from setuptools import setup
-from pycliwrapper import __version__
+
+__version__ = "0.2"
 
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(
@@ -17,8 +18,8 @@
     keywords=["cli", "wrapper"],
     install_requires=[],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Intended Audience :: Developers"
     ]
-)
+)
```

