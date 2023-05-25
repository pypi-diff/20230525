# Comparing `tmp/dartrig-0.1.0.tar.gz` & `tmp/dartrig-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dartrig-0.1.0.tar", last modified: Thu May 25 14:35:11 2023, max compression
+gzip compressed data, was "dist/dartrig-0.1.1.tar", last modified: Thu May 25 14:48:04 2023, max compression
```

## Comparing `dartrig-0.1.0.tar` & `dartrig-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-25 14:35:11.000000 dartrig-0.1.0/
--rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-05-25 14:35:11.000000 dartrig-0.1.0/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.1.0/LICENSE
--rw-r--r--   0 nezah      (501) staff       (20)     1061 2023-04-11 08:24:52.000000 dartrig-0.1.0/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      692 2023-05-25 14:35:10.000000 dartrig-0.1.0/setup.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-25 14:35:11.000000 dartrig-0.1.0/dartrig/
--rw-r--r--   0 nezah      (501) staff       (20)    13097 2023-05-25 14:35:10.000000 dartrig-0.1.0/dartrig/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)      682 2023-03-18 12:39:55.000000 dartrig-0.1.0/dartrig/annotations.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-25 14:35:11.000000 dartrig-0.1.0/dartrig.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-05-25 14:35:11.000000 dartrig-0.1.0/dartrig.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      223 2023-05-25 14:35:11.000000 dartrig-0.1.0/dartrig.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)       30 2023-05-25 14:35:11.000000 dartrig-0.1.0/dartrig.egg-info/requires.txt
--rw-r--r--   0 nezah      (501) staff       (20)        8 2023-05-25 14:35:11.000000 dartrig-0.1.0/dartrig.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-25 14:35:11.000000 dartrig-0.1.0/dartrig.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-25 14:35:11.000000 dartrig-0.1.0/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-25 14:48:04.000000 dartrig-0.1.1/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-05-25 14:48:04.000000 dartrig-0.1.1/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.1.1/LICENSE
+-rw-r--r--   0 nezah      (501) staff       (20)     1061 2023-04-11 08:24:52.000000 dartrig-0.1.1/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      692 2023-05-25 14:48:00.000000 dartrig-0.1.1/setup.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-25 14:48:04.000000 dartrig-0.1.1/dartrig/
+-rw-r--r--   0 nezah      (501) staff       (20)    13097 2023-05-25 14:35:10.000000 dartrig-0.1.1/dartrig/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)      682 2023-03-18 12:39:55.000000 dartrig-0.1.1/dartrig/annotations.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-25 14:48:04.000000 dartrig-0.1.1/dartrig.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-05-25 14:48:04.000000 dartrig-0.1.1/dartrig.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      223 2023-05-25 14:48:04.000000 dartrig-0.1.1/dartrig.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       30 2023-05-25 14:48:04.000000 dartrig-0.1.1/dartrig.egg-info/requires.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        8 2023-05-25 14:48:04.000000 dartrig-0.1.1/dartrig.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-25 14:48:04.000000 dartrig-0.1.1/dartrig.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-25 14:48:04.000000 dartrig-0.1.1/setup.cfg
```

### Comparing `dartrig-0.1.0/PKG-INFO` & `dartrig-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartrig
-Version: 0.1.0
+Version: 0.1.1
 Summary: dartrig api wrapper
 Home-page: https://github.com/cheddars/dart_rigger
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dartrig-0.1.0/LICENSE` & `dartrig-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.0/README.md` & `dartrig-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.0/setup.py` & `dartrig-0.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="dartrig",
-    version="0.1.0",
+    version="0.1.1",
     install_requires=[
         'requests',
         'bs4',
         'adt_cache==0.0.9'
     ],
     license='MIT',
     author="cheddars",
```

### Comparing `dartrig-0.1.0/dartrig/__init__.py` & `dartrig-0.1.1/dartrig/__init__.py`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.0/dartrig/annotations.py` & `dartrig-0.1.1/dartrig/annotations.py`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.0/dartrig.egg-info/PKG-INFO` & `dartrig-0.1.1/dartrig.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartrig
-Version: 0.1.0
+Version: 0.1.1
 Summary: dartrig api wrapper
 Home-page: https://github.com/cheddars/dart_rigger
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

