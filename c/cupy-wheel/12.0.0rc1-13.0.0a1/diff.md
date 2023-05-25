# Comparing `tmp/cupy-wheel-12.0.0rc1.tar.gz` & `tmp/cupy-wheel-13.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cupy-wheel-12.0.0rc1.tar", last modified: Thu Mar  2 06:10:48 2023, max compression
+gzip compressed data, was "cupy-wheel-13.0.0a1.tar", last modified: Thu May 25 04:30:06 2023, max compression
```

## Comparing `cupy-wheel-12.0.0rc1.tar` & `cupy-wheel-13.0.0a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0     2053     2053        0 2023-03-02 06:10:47.990556 cupy-wheel-12.0.0rc1/
--rw-r--r--   0     2053     2053       58 2023-03-02 06:10:47.990556 cupy-wheel-12.0.0rc1/PKG-INFO
-drwxr-xr-x   0     2053     2053        0 2023-03-02 06:10:47.990556 cupy-wheel-12.0.0rc1/cupy_wheel.egg-info/
--rw-r--r--   0     2053     2053       58 2023-03-02 06:10:47.000000 cupy-wheel-12.0.0rc1/cupy_wheel.egg-info/PKG-INFO
--rw-r--r--   0     2053     2053      144 2023-03-02 06:10:47.000000 cupy-wheel-12.0.0rc1/cupy_wheel.egg-info/SOURCES.txt
--rw-r--r--   0     2053     2053        1 2023-03-02 06:10:47.000000 cupy-wheel-12.0.0rc1/cupy_wheel.egg-info/dependency_links.txt
--rw-r--r--   0     2053     2053        1 2023-03-02 06:10:47.000000 cupy-wheel-12.0.0rc1/cupy_wheel.egg-info/top_level.txt
--rw-r--r--   0     2053     2053       38 2023-03-02 06:10:47.990556 cupy-wheel-12.0.0rc1/setup.cfg
--rw-rw-r--   0     2053     2053     8241 2023-03-02 06:10:24.000000 cupy-wheel-12.0.0rc1/setup.py
+drwxr-xr-x   0     2758     2758        0 2023-05-25 04:30:06.237297 cupy-wheel-13.0.0a1/
+-rw-r--r--   0     2758     2758       57 2023-05-25 04:30:06.237297 cupy-wheel-13.0.0a1/PKG-INFO
+drwxr-xr-x   0     2758     2758        0 2023-05-25 04:30:06.237297 cupy-wheel-13.0.0a1/cupy_wheel.egg-info/
+-rw-r--r--   0     2758     2758       57 2023-05-25 04:30:06.000000 cupy-wheel-13.0.0a1/cupy_wheel.egg-info/PKG-INFO
+-rw-r--r--   0     2758     2758      144 2023-05-25 04:30:06.000000 cupy-wheel-13.0.0a1/cupy_wheel.egg-info/SOURCES.txt
+-rw-r--r--   0     2758     2758        1 2023-05-25 04:30:06.000000 cupy-wheel-13.0.0a1/cupy_wheel.egg-info/dependency_links.txt
+-rw-r--r--   0     2758     2758        1 2023-05-25 04:30:06.000000 cupy-wheel-13.0.0a1/cupy_wheel.egg-info/top_level.txt
+-rw-r--r--   0     2758     2758       38 2023-05-25 04:30:06.237297 cupy-wheel-13.0.0a1/setup.cfg
+-rw-rw-r--   0     2758     2758     8240 2023-05-25 03:52:58.000000 cupy-wheel-13.0.0a1/setup.py
```

### Comparing `cupy-wheel-12.0.0rc1/setup.py` & `cupy-wheel-13.0.0a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import sys
 from typing import Dict, List, Optional
 
 from setuptools import setup
 
 
-VERSION = '12.0.0rc1'
+VERSION = '13.0.0a1'
 
 # List of packages supported by this version of CuPy.
 PACKAGES = [
     'cupy-cuda102',
     'cupy-cuda110',
     'cupy-cuda111',
     'cupy-cuda11x',
```

