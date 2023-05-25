# Comparing `tmp/BaseNN-0.0.9.tar.gz` & `tmp/BaseNN-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseNN-0.0.9.tar", last modified: Thu Mar 23 08:18:26 2023, max compression
+gzip compressed data, was "dist/BaseNN-0.1.0.tar", last modified: Wed May 24 09:09:25 2023, max compression
```

## Comparing `BaseNN-0.0.9.tar` & `BaseNN-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-23 08:18:26.000000 BaseNN-0.0.9/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-23 08:18:26.000000 BaseNN-0.0.9/BaseNN/
--rw-rw-r--   0 user      (1001) user      (1001)    25552 2023-03-23 08:17:43.000000 BaseNN-0.0.9/BaseNN/BaseNN.py
--rw-rw-r--   0 user      (1001) user      (1001)      206 2023-03-17 08:45:06.000000 BaseNN-0.0.9/BaseNN/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-23 08:18:26.000000 BaseNN-0.0.9/BaseNN/examples/
--rw-rw-r--   0 user      (1001) user      (1001)     8847 2023-03-23 08:10:20.000000 BaseNN-0.0.9/BaseNN/examples/BaseNN_demo.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-26 07:13:38.000000 BaseNN-0.0.9/BaseNN/examples/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2023-02-09 06:29:12.000000 BaseNN-0.0.9/BaseNN/examples/lstmdemo.py
--rw-rw-r--   0 user      (1001) user      (1001)     1256 2023-03-23 08:17:57.000000 BaseNN-0.0.9/BaseNN/version.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-23 08:18:26.000000 BaseNN-0.0.9/BaseNN.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-03-23 08:18:26.000000 BaseNN-0.0.9/BaseNN.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      356 2023-03-23 08:18:26.000000 BaseNN-0.0.9/BaseNN.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-03-23 08:18:26.000000 BaseNN-0.0.9/BaseNN.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       49 2023-03-23 08:18:26.000000 BaseNN-0.0.9/BaseNN.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1001) user      (1001)       69 2023-03-23 08:18:26.000000 BaseNN-0.0.9/BaseNN.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        7 2023-03-23 08:18:26.000000 BaseNN-0.0.9/BaseNN.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-18 03:21:26.000000 BaseNN-0.0.9/BaseNN.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-03-23 08:18:26.000000 BaseNN-0.0.9/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-03-23 08:18:26.000000 BaseNN-0.0.9/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     3827 2023-03-23 08:17:52.000000 BaseNN-0.0.9/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-24 09:09:25.000000 BaseNN-0.1.0/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-24 09:09:25.000000 BaseNN-0.1.0/BaseNN/
+-rw-rw-r--   0 user      (1001) user      (1001)    37357 2023-05-24 07:46:21.000000 BaseNN-0.1.0/BaseNN/BaseNN.py
+-rw-rw-r--   0 user      (1001) user      (1001)      270 2023-05-24 09:07:14.000000 BaseNN-0.1.0/BaseNN/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-24 09:09:25.000000 BaseNN-0.1.0/BaseNN/examples/
+-rw-rw-r--   0 user      (1001) user      (1001)    22819 2023-05-24 08:46:31.000000 BaseNN-0.1.0/BaseNN/examples/BaseNN_demo.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-26 07:13:38.000000 BaseNN-0.1.0/BaseNN/examples/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)     3059 2023-04-13 07:47:30.000000 BaseNN-0.1.0/BaseNN/examples/pkl2pth.py
+-rw-r--r--   0 user      (1001) user      (1001)     4409 2023-05-22 08:15:12.000000 BaseNN-0.1.0/BaseNN/load_data.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1256 2023-05-24 09:08:59.000000 BaseNN-0.1.0/BaseNN/version.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-24 09:09:25.000000 BaseNN-0.1.0/BaseNN.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-24 09:09:25.000000 BaseNN-0.1.0/BaseNN.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      375 2023-05-24 09:09:25.000000 BaseNN-0.1.0/BaseNN.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-05-24 09:09:25.000000 BaseNN-0.1.0/BaseNN.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       49 2023-05-24 09:09:25.000000 BaseNN-0.1.0/BaseNN.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       80 2023-05-24 09:09:25.000000 BaseNN-0.1.0/BaseNN.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        7 2023-05-24 09:09:25.000000 BaseNN-0.1.0/BaseNN.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-18 03:21:26.000000 BaseNN-0.1.0/BaseNN.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-24 09:09:25.000000 BaseNN-0.1.0/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-05-24 09:09:25.000000 BaseNN-0.1.0/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     3827 2023-05-24 09:08:45.000000 BaseNN-0.1.0/setup.py
```

### Comparing `BaseNN-0.0.9/BaseNN/version.py` & `BaseNN-0.1.0/BaseNN/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-__version__='0.0.9'
+__version__='0.1.0'
 __path__=os.path.abspath(os.getcwd())
 
 def parse_version_info(version_str):
     version_info = []
     for x in version_str.split('.'):
         if x.isdigit():
             version_info.append(int(x))
```

### Comparing `BaseNN-0.0.9/setup.py` & `BaseNN-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     packages = list(gen_packages_items())
     return packages
 
 
 setup(
     name='BaseNN',
-    version='0.0.9',
+    version='0.1.0',
     description='BaseNN can easily build neural networks layer by layer and deeply explore the neural network principle.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
     include_package_data=True,
```

