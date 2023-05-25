# Comparing `tmp/Candataloader-1.1.0.tar.gz` & `tmp/Candataloader-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Candataloader-1.1.0.tar", last modified: Wed May 24 13:52:47 2023, max compression
+gzip compressed data, was "dist/Candataloader-1.1.1.tar", last modified: Wed May 24 14:03:11 2023, max compression
```

## Comparing `Candataloader-1.1.0.tar` & `Candataloader-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-24 13:52:47.000000 Candataloader-1.1.0/
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 03:35:39.000000 Candataloader-1.1.0/README.md
-drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-24 13:52:47.000000 Candataloader-1.1.0/Candataloader/
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 03:31:46.000000 Candataloader-1.1.0/Candataloader/__init__.py
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)     1172 2023-05-24 13:40:09.000000 Candataloader-1.1.0/Candataloader/download.py
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       38 2023-05-24 13:52:47.000000 Candataloader-1.1.0/setup.cfg
-drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-24 13:52:47.000000 Candataloader-1.1.0/Candataloader.egg-info/
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        9 2023-05-24 13:52:47.000000 Candataloader-1.1.0/Candataloader.egg-info/requires.txt
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        1 2023-05-24 13:52:47.000000 Candataloader-1.1.0/Candataloader.egg-info/dependency_links.txt
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      254 2023-05-24 13:52:47.000000 Candataloader-1.1.0/Candataloader.egg-info/SOURCES.txt
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       14 2023-05-24 13:52:47.000000 Candataloader-1.1.0/Candataloader.egg-info/top_level.txt
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      254 2023-05-24 13:52:47.000000 Candataloader-1.1.0/Candataloader.egg-info/PKG-INFO
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      317 2023-05-24 13:49:33.000000 Candataloader-1.1.0/setup.py
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      254 2023-05-24 13:52:47.000000 Candataloader-1.1.0/PKG-INFO
+drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-24 14:03:11.000000 Candataloader-1.1.1/
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 03:35:39.000000 Candataloader-1.1.1/README.md
+drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-24 14:03:11.000000 Candataloader-1.1.1/Candataloader/
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 03:31:46.000000 Candataloader-1.1.1/Candataloader/__init__.py
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)     1172 2023-05-24 13:40:09.000000 Candataloader-1.1.1/Candataloader/download.py
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       38 2023-05-24 14:03:11.000000 Candataloader-1.1.1/setup.cfg
+drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-24 14:03:11.000000 Candataloader-1.1.1/Candataloader.egg-info/
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        1 2023-05-24 14:03:11.000000 Candataloader-1.1.1/Candataloader.egg-info/dependency_links.txt
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      218 2023-05-24 14:03:11.000000 Candataloader-1.1.1/Candataloader.egg-info/SOURCES.txt
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       23 2023-05-24 14:03:11.000000 Candataloader-1.1.1/Candataloader.egg-info/top_level.txt
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      227 2023-05-24 14:03:11.000000 Candataloader-1.1.1/Candataloader.egg-info/PKG-INFO
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      299 2023-05-24 14:02:11.000000 Candataloader-1.1.1/setup.py
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      227 2023-05-24 14:03:11.000000 Candataloader-1.1.1/PKG-INFO
```

### Comparing `Candataloader-1.1.0/Candataloader/download.py` & `Candataloader-1.1.1/Candataloader/download.py`

 * *Files identical despite different names*

