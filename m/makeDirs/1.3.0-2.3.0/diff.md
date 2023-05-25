# Comparing `tmp/makedirs-1.3.0.tar.gz` & `tmp/makedirs-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makedirs-1.3.0.tar", last modified: Fri May  5 11:51:08 2023, max compression
+gzip compressed data, was "makedirs-2.3.0.tar", last modified: Fri May  5 11:49:49 2023, max compression
```

## Comparing `makedirs-1.3.0.tar` & `makedirs-2.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 11:51:08.483147 makedirs-1.3.0/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 makedirs-1.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 makedirs-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0      385 2023-05-05 11:51:08.483147 makedirs-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 makedirs-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 11:51:08.468125 makedirs-1.3.0/makedirs.egg-info/
--rw-rw-rw-   0        0        0      385 2023-05-05 11:51:08.000000 makedirs-1.3.0/makedirs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-05-05 11:51:08.000000 makedirs-1.3.0/makedirs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 11:51:08.000000 makedirs-1.3.0/makedirs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 11:51:08.000000 makedirs-1.3.0/makedirs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 11:51:08.471129 makedirs-1.3.0/mkdirs/
-drwxrwxrwx   0        0        0        0 2023-05-05 11:51:08.475139 makedirs-1.3.0/mkdirs/Function/
--rw-rw-rw-   0        0        0   470528 2023-04-28 06:08:00.000000 makedirs-1.3.0/mkdirs/Function/MkdirFunction.pyd
--rw-rw-rw-   0        0        0        0 2023-03-01 06:05:54.000000 makedirs-1.3.0/mkdirs/Function/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 11:51:08.481147 makedirs-1.3.0/mkdirs/Ui/
--rw-rw-rw-   0        0        0    40448 2023-04-28 06:06:05.000000 makedirs-1.3.0/mkdirs/Ui/MaskWin.pyd
--rw-rw-rw-   0        0        0        0 2023-03-01 06:05:54.000000 makedirs-1.3.0/mkdirs/Ui/__init__.py
--rw-rw-rw-   0        0        0    71680 2023-04-28 06:08:08.000000 makedirs-1.3.0/mkdirs/Ui/mkdirUi.pyd
--rw-rw-rw-   0        0        0        0 2023-03-01 06:05:54.000000 makedirs-1.3.0/mkdirs/__init__.py
--rw-rw-rw-   0        0        0   149504 2023-05-05 09:15:01.000000 makedirs-1.3.0/mkdirs/mkdir.pyd
--rw-rw-rw-   0        0        0      135 2023-05-05 11:51:08.485144 makedirs-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1030 2023-05-05 11:50:56.000000 makedirs-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:49:49.420139 makedirs-2.3.0/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 makedirs-2.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 makedirs-2.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      385 2023-05-05 11:49:49.420139 makedirs-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 makedirs-2.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 11:49:49.401779 makedirs-2.3.0/makedirs.egg-info/
+-rw-rw-rw-   0        0        0      385 2023-05-05 11:49:49.000000 makedirs-2.3.0/makedirs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-05-05 11:49:49.000000 makedirs-2.3.0/makedirs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 11:49:49.000000 makedirs-2.3.0/makedirs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 11:49:49.000000 makedirs-2.3.0/makedirs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 11:49:49.404770 makedirs-2.3.0/mkdirs/
+drwxrwxrwx   0        0        0        0 2023-05-05 11:49:49.409141 makedirs-2.3.0/mkdirs/Function/
+-rw-rw-rw-   0        0        0   470528 2023-04-28 06:08:00.000000 makedirs-2.3.0/mkdirs/Function/MkdirFunction.pyd
+-rw-rw-rw-   0        0        0        0 2023-03-01 06:05:54.000000 makedirs-2.3.0/mkdirs/Function/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:49:49.418139 makedirs-2.3.0/mkdirs/Ui/
+-rw-rw-rw-   0        0        0    40448 2023-04-28 06:06:05.000000 makedirs-2.3.0/mkdirs/Ui/MaskWin.pyd
+-rw-rw-rw-   0        0        0        0 2023-03-01 06:05:54.000000 makedirs-2.3.0/mkdirs/Ui/__init__.py
+-rw-rw-rw-   0        0        0    71680 2023-04-28 06:08:08.000000 makedirs-2.3.0/mkdirs/Ui/mkdirUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-03-01 06:05:54.000000 makedirs-2.3.0/mkdirs/__init__.py
+-rw-rw-rw-   0        0        0   149504 2023-05-05 09:15:01.000000 makedirs-2.3.0/mkdirs/mkdir.pyd
+-rw-rw-rw-   0        0        0      135 2023-05-05 11:49:49.421140 makedirs-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1030 2023-05-05 11:49:47.000000 makedirs-2.3.0/setup.py
```

### Comparing `makedirs-1.3.0/LICENSE.txt` & `makedirs-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `makedirs-1.3.0/setup.py` & `makedirs-2.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
-MAJOR = 1
+MAJOR = 2
 MINOR = 3
 PATCH = 0
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
```

