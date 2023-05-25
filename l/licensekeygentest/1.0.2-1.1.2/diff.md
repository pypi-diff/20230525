# Comparing `tmp/licensekeygentest-1.0.2.tar.gz` & `tmp/licensekeygentest-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "licensekeygentest-1.0.2.tar", last modified: Wed May 24 13:49:59 2023, max compression
+gzip compressed data, was "licensekeygentest-1.1.2.tar", last modified: Thu May 25 09:12:27 2023, max compression
```

## Comparing `licensekeygentest-1.0.2.tar` & `licensekeygentest-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-24 13:49:59.749889 licensekeygentest-1.0.2/
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     1063 2023-05-23 11:20:36.000000 licensekeygentest-1.0.2/LICENSE
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      699 2023-05-24 13:49:59.749889 licensekeygentest-1.0.2/PKG-INFO
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      152 2023-05-23 11:20:36.000000 licensekeygentest-1.0.2/README.md
-drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-24 13:49:59.741889 licensekeygentest-1.0.2/licensekeygentest/
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       43 2023-05-23 11:20:36.000000 licensekeygentest-1.0.2/licensekeygentest/__init__.py
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     2238 2023-05-24 13:48:02.000000 licensekeygentest-1.0.2/licensekeygentest/main.py
-drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-24 13:49:59.741889 licensekeygentest-1.0.2/licensekeygentest.egg-info/
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      699 2023-05-24 13:49:59.000000 licensekeygentest-1.0.2/licensekeygentest.egg-info/PKG-INFO
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      286 2023-05-24 13:49:59.000000 licensekeygentest-1.0.2/licensekeygentest.egg-info/SOURCES.txt
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)        1 2023-05-24 13:49:59.000000 licensekeygentest-1.0.2/licensekeygentest.egg-info/dependency_links.txt
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)        9 2023-05-24 13:49:59.000000 licensekeygentest-1.0.2/licensekeygentest.egg-info/requires.txt
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       18 2023-05-24 13:49:59.000000 licensekeygentest-1.0.2/licensekeygentest.egg-info/top_level.txt
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       38 2023-05-24 13:49:59.749889 licensekeygentest-1.0.2/setup.cfg
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     1063 2023-05-24 13:48:37.000000 licensekeygentest-1.0.2/setup.py
+drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-25 09:12:27.019629 licensekeygentest-1.1.2/
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     1063 2023-05-23 11:20:36.000000 licensekeygentest-1.1.2/LICENSE
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      699 2023-05-25 09:12:27.019629 licensekeygentest-1.1.2/PKG-INFO
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      152 2023-05-23 11:20:36.000000 licensekeygentest-1.1.2/README.md
+drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-25 09:12:27.015629 licensekeygentest-1.1.2/licensekeygentest/
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       43 2023-05-23 11:20:36.000000 licensekeygentest-1.1.2/licensekeygentest/__init__.py
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     3806 2023-05-25 09:08:10.000000 licensekeygentest-1.1.2/licensekeygentest/main.py
+drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-25 09:12:27.019629 licensekeygentest-1.1.2/licensekeygentest.egg-info/
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      699 2023-05-25 09:12:26.000000 licensekeygentest-1.1.2/licensekeygentest.egg-info/PKG-INFO
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      286 2023-05-25 09:12:26.000000 licensekeygentest-1.1.2/licensekeygentest.egg-info/SOURCES.txt
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)        1 2023-05-25 09:12:26.000000 licensekeygentest-1.1.2/licensekeygentest.egg-info/dependency_links.txt
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)        9 2023-05-25 09:12:26.000000 licensekeygentest-1.1.2/licensekeygentest.egg-info/requires.txt
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       18 2023-05-25 09:12:26.000000 licensekeygentest-1.1.2/licensekeygentest.egg-info/top_level.txt
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       38 2023-05-25 09:12:27.019629 licensekeygentest-1.1.2/setup.cfg
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     1063 2023-05-25 09:12:07.000000 licensekeygentest-1.1.2/setup.py
```

### Comparing `licensekeygentest-1.0.2/LICENSE` & `licensekeygentest-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `licensekeygentest-1.0.2/PKG-INFO` & `licensekeygentest-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensekeygentest
-Version: 1.0.2
+Version: 1.1.2
 Summary: POC for license validation checks
 Author: Rahul R
 Author-email: <rahulranjan25.RR@gmail.com>
 Keywords: python,authentication,licensing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `licensekeygentest-1.0.2/licensekeygentest.egg-info/PKG-INFO` & `licensekeygentest-1.1.2/licensekeygentest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensekeygentest
-Version: 1.0.2
+Version: 1.1.2
 Summary: POC for license validation checks
 Author: Rahul R
 Author-email: <rahulranjan25.RR@gmail.com>
 Keywords: python,authentication,licensing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `licensekeygentest-1.0.2/setup.py` & `licensekeygentest-1.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.2'
+VERSION = '1.1.2'
 DESCRIPTION = 'POC for license validation checks'
 LONG_DESCRIPTION = 'A POC package that allows lisencing of python libraries.'
 
 # Setting up
 setup(
     name="licensekeygentest",
     version=VERSION,
```

