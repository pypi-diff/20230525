# Comparing `tmp/large-image-source-dicom-1.21.1.dev4.tar.gz` & `tmp/large-image-source-dicom-1.21.1.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-dicom-1.21.1.dev4.tar", last modified: Wed May 24 20:08:37 2023, max compression
+gzip compressed data, was "large-image-source-dicom-1.21.1.dev6.tar", last modified: Thu May 25 01:22:01 2023, max compression
```

## Comparing `large-image-source-dicom-1.21.1.dev4.tar` & `large-image-source-dicom-1.21.1.dev6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-24 20:08:37.775359 large-image-source-dicom-1.21.1.dev4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-05-24 20:08:37.000000 large-image-source-dicom-1.21.1.dev4/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2023-05-24 20:08:37.775359 large-image-source-dicom-1.21.1.dev4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-05-24 20:08:37.000000 large-image-source-dicom-1.21.1.dev4/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-24 20:08:37.775359 large-image-source-dicom-1.21.1.dev4/large_image_source_dicom/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9934 2023-05-24 20:07:46.000000 large-image-source-dicom-1.21.1.dev4/large_image_source_dicom/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1163 2023-05-24 20:07:46.000000 large-image-source-dicom-1.21.1.dev4/large_image_source_dicom/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-24 20:08:37.775359 large-image-source-dicom-1.21.1.dev4/large_image_source_dicom.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2023-05-24 20:08:37.000000 large-image-source-dicom-1.21.1.dev4/large_image_source_dicom.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2023-05-24 20:08:37.000000 large-image-source-dicom-1.21.1.dev4/large_image_source_dicom.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-24 20:08:37.000000 large-image-source-dicom-1.21.1.dev4/large_image_source_dicom.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-05-24 20:08:37.000000 large-image-source-dicom-1.21.1.dev4/large_image_source_dicom.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-05-24 20:08:37.000000 large-image-source-dicom-1.21.1.dev4/large_image_source_dicom.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-05-24 20:08:37.000000 large-image-source-dicom-1.21.1.dev4/large_image_source_dicom.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-24 20:08:37.775359 large-image-source-dicom-1.21.1.dev4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2427 2023-05-24 20:07:46.000000 large-image-source-dicom-1.21.1.dev4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 01:22:01.563257 large-image-source-dicom-1.21.1.dev6/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-05-25 01:22:01.000000 large-image-source-dicom-1.21.1.dev6/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2023-05-25 01:22:01.563257 large-image-source-dicom-1.21.1.dev6/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-05-25 01:22:01.000000 large-image-source-dicom-1.21.1.dev6/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 01:22:01.559257 large-image-source-dicom-1.21.1.dev6/large_image_source_dicom/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9934 2023-05-25 01:21:02.000000 large-image-source-dicom-1.21.1.dev6/large_image_source_dicom/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1163 2023-05-25 01:21:02.000000 large-image-source-dicom-1.21.1.dev6/large_image_source_dicom/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 01:22:01.563257 large-image-source-dicom-1.21.1.dev6/large_image_source_dicom.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2023-05-25 01:22:01.000000 large-image-source-dicom-1.21.1.dev6/large_image_source_dicom.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2023-05-25 01:22:01.000000 large-image-source-dicom-1.21.1.dev6/large_image_source_dicom.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-25 01:22:01.000000 large-image-source-dicom-1.21.1.dev6/large_image_source_dicom.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-05-25 01:22:01.000000 large-image-source-dicom-1.21.1.dev6/large_image_source_dicom.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-05-25 01:22:01.000000 large-image-source-dicom-1.21.1.dev6/large_image_source_dicom.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-05-25 01:22:01.000000 large-image-source-dicom-1.21.1.dev6/large_image_source_dicom.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-25 01:22:01.563257 large-image-source-dicom-1.21.1.dev6/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2427 2023-05-25 01:21:02.000000 large-image-source-dicom-1.21.1.dev6/setup.py
```

### Comparing `large-image-source-dicom-1.21.1.dev4/LICENSE` & `large-image-source-dicom-1.21.1.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.21.1.dev4/PKG-INFO` & `large-image-source-dicom-1.21.1.dev6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-dicom
-Version: 1.21.1.dev4
+Version: 1.21.1.dev6
 Summary: A DICOM tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-dicom-1.21.1.dev4/README.rst` & `large-image-source-dicom-1.21.1.dev6/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.21.1.dev4/large_image_source_dicom/__init__.py` & `large-image-source-dicom-1.21.1.dev6/large_image_source_dicom/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.21.1.dev4/large_image_source_dicom/girder_source.py` & `large-image-source-dicom-1.21.1.dev6/large_image_source_dicom/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.21.1.dev4/large_image_source_dicom.egg-info/PKG-INFO` & `large-image-source-dicom-1.21.1.dev6/large_image_source_dicom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-dicom
-Version: 1.21.1.dev4
+Version: 1.21.1.dev6
 Summary: A DICOM tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-dicom-1.21.1.dev4/setup.py` & `large-image-source-dicom-1.21.1.dev6/setup.py`

 * *Files identical despite different names*

