# Comparing `tmp/grid2fp-0.0.2.tar.gz` & `tmp/grid2fp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grid2fp-0.0.2.tar", last modified: Thu May 25 15:52:18 2023, max compression
+gzip compressed data, was "grid2fp-0.0.3.tar", last modified: Thu May 25 19:17:08 2023, max compression
```

## Comparing `grid2fp-0.0.2.tar` & `grid2fp-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:52:18.668267 grid2fp-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 15:51:53.000000 grid2fp-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-25 15:52:18.668267 grid2fp-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-25 15:51:53.000000 grid2fp-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:52:18.664267 grid2fp-0.0.2/grid2fp/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 15:51:53.000000 grid2fp-0.0.2/grid2fp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-25 15:51:53.000000 grid2fp-0.0.2/grid2fp/grid2fp.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-25 15:51:53.000000 grid2fp-0.0.2/grid2fp/grid_segment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:52:18.668267 grid2fp-0.0.2/grid2fp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-25 15:52:18.000000 grid2fp-0.0.2/grid2fp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-25 15:52:18.000000 grid2fp-0.0.2/grid2fp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:52:18.000000 grid2fp-0.0.2/grid2fp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 15:52:18.000000 grid2fp-0.0.2/grid2fp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 15:52:18.000000 grid2fp-0.0.2/grid2fp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:52:18.668267 grid2fp-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-25 15:51:53.000000 grid2fp-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:52:18.668267 grid2fp-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 15:51:53.000000 grid2fp-0.0.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-25 15:51:53.000000 grid2fp-0.0.2/test/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:17:08.956801 grid2fp-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 19:16:41.000000 grid2fp-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-25 19:17:08.956801 grid2fp-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-25 19:16:41.000000 grid2fp-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:17:08.956801 grid2fp-0.0.3/grid2fp/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 19:16:41.000000 grid2fp-0.0.3/grid2fp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-25 19:16:41.000000 grid2fp-0.0.3/grid2fp/grid2fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-25 19:16:41.000000 grid2fp-0.0.3/grid2fp/grid_segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:17:08.956801 grid2fp-0.0.3/grid2fp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-25 19:17:08.000000 grid2fp-0.0.3/grid2fp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-25 19:17:08.000000 grid2fp-0.0.3/grid2fp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:17:08.000000 grid2fp-0.0.3/grid2fp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 19:17:08.000000 grid2fp-0.0.3/grid2fp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 19:17:08.000000 grid2fp-0.0.3/grid2fp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 19:17:08.956801 grid2fp-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-25 19:16:41.000000 grid2fp-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:17:08.956801 grid2fp-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 19:16:41.000000 grid2fp-0.0.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-25 19:16:41.000000 grid2fp-0.0.3/test/test_integration.py
```

### Comparing `grid2fp-0.0.2/LICENSE` & `grid2fp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `grid2fp-0.0.2/PKG-INFO` & `grid2fp-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grid2fp
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to eat grid diagrams and generate its front projection.
 Home-page: https://github.com/Joecstarr/grid2fp
 Author: Casey Duckering
 Keywords: topology,Legendrian,Grid Diagram,knot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `grid2fp-0.0.2/README.md` & `grid2fp-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `grid2fp-0.0.2/grid2fp/grid2fp.py` & `grid2fp-0.0.3/grid2fp/grid2fp.py`

 * *Files identical despite different names*

### Comparing `grid2fp-0.0.2/grid2fp.egg-info/PKG-INFO` & `grid2fp-0.0.3/grid2fp.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grid2fp
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to eat grid diagrams and generate its front projection.
 Home-page: https://github.com/Joecstarr/grid2fp
 Author: Casey Duckering
 Keywords: topology,Legendrian,Grid Diagram,knot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `grid2fp-0.0.2/setup.py` & `grid2fp-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import logging
 
 logger = logging.getLogger(__name__)
 
-version = "0.0.2"
+version = "0.0.3"
 
 try:
     with open("README.md", "r") as f:
         long_desc = f.read()
 except:
     logger.warning("Could not open README.md.  long_description will be set to None.")
     long_desc = None
```

### Comparing `grid2fp-0.0.2/test/test_integration.py` & `grid2fp-0.0.3/test/test_integration.py`

 * *Files identical despite different names*

