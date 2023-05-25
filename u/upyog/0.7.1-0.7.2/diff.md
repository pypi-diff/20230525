# Comparing `tmp/upyog-0.7.1.tar.gz` & `tmp/upyog-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upyog-0.7.1.tar", last modified: Wed May 17 16:23:48 2023, max compression
+gzip compressed data, was "upyog-0.7.2.tar", last modified: Thu May 25 07:50:05 2023, max compression
```

## Comparing `upyog-0.7.1.tar` & `upyog-0.7.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.477124 upyog-0.7.1/
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3412 2023-05-17 16:23:22.000000 upyog-0.7.1/CHANGELOG.md
--rw-r--r--   0 rahulsomani   (501) staff       (20)      133 2022-01-27 18:07:46.000000 upyog-0.7.1/MANIFEST.in
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-05-17 16:23:48.477207 upyog-0.7.1/PKG-INFO
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)      618 2022-01-15 04:03:41.000000 upyog-0.7.1/README.md
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.468932 upyog-0.7.1/assets/
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.470354 upyog-0.7.1/assets/fonts/
--rw-rwxrwx   0 rahulsomani   (501) staff       (20)    28432 2022-01-27 13:15:35.000000 upyog-0.7.1/assets/fonts/EuroStyleNormal.ttf
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)     1384 2023-05-17 16:23:48.477600 upyog-0.7.1/setup.cfg
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)      251 2022-01-17 09:53:10.000000 upyog-0.7.1/setup.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.471089 upyog-0.7.1/upyog/
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)       28 2022-10-28 02:44:32.000000 upyog-0.7.1/upyog/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      644 2023-01-24 04:50:27.000000 upyog-0.7.1/upyog/all.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.472406 upyog-0.7.1/upyog/ann/
--rw-r--r--   0 rahulsomani   (501) staff       (20)        0 2022-01-22 05:11:22.000000 upyog-0.7.1/upyog/ann/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     4426 2022-01-22 20:02:13.000000 upyog-0.7.1/upyog/ann/annoy.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3066 2023-04-16 03:50:08.000000 upyog-0.7.1/upyog/cli.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.473948 upyog-0.7.1/upyog/image/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      141 2022-09-04 09:39:14.000000 upyog-0.7.1/upyog/image/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3340 2023-04-21 18:57:17.000000 upyog-0.7.1/upyog/image/cli.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     2286 2022-09-01 09:27:43.000000 upyog-0.7.1/upyog/image/composition.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)    17228 2023-03-06 08:32:51.000000 upyog-0.7.1/upyog/image/draw.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1526 2023-04-15 11:13:07.000000 upyog-0.7.1/upyog/image/io.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1442 2023-02-28 09:04:05.000000 upyog-0.7.1/upyog/image/pil_operators.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1518 2023-05-17 11:01:32.000000 upyog-0.7.1/upyog/image/utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     7939 2023-02-28 09:16:20.000000 upyog-0.7.1/upyog/image/visualiser.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1306 2023-05-17 15:42:19.000000 upyog-0.7.1/upyog/imports.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.475291 upyog-0.7.1/upyog/ml/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      211 2023-05-17 15:36:44.000000 upyog-0.7.1/upyog/ml/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1419 2023-05-17 11:40:18.000000 upyog-0.7.1/upyog/ml/coreml_utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1626 2023-05-17 15:35:49.000000 upyog-0.7.1/upyog/ml/eval_dataset.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      438 2023-05-17 15:42:14.000000 upyog-0.7.1/upyog/ml/imports.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3662 2023-05-17 16:21:13.000000 upyog-0.7.1/upyog/ml/model_utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1707 2023-05-17 11:41:09.000000 upyog-0.7.1/upyog/ml/preprocessing.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1230 2023-05-17 11:25:25.000000 upyog-0.7.1/upyog/ml/utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1138 2023-05-17 11:07:07.000000 upyog-0.7.1/upyog/ml/visualise.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1198 2022-06-01 05:03:09.000000 upyog-0.7.1/upyog/nb2script.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.476066 upyog-0.7.1/upyog/os/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      137 2022-10-26 00:24:39.000000 upyog-0.7.1/upyog/os/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     6159 2023-04-16 07:09:32.000000 upyog-0.7.1/upyog/os/cli.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-08-03 15:10:12.000000 upyog-0.7.1/upyog/os/patch_pathlib.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3356 2022-10-26 00:24:37.000000 upyog-0.7.1/upyog/os/read_files.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3459 2023-05-17 10:58:12.000000 upyog-0.7.1/upyog/os/utils.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.476968 upyog-0.7.1/upyog/utils/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      118 2022-10-28 03:18:43.000000 upyog-0.7.1/upyog/utils/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-04-05 12:59:08.000000 upyog-0.7.1/upyog/utils/boxes.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)    14495 2023-01-11 07:05:00.000000 upyog-0.7.1/upyog/utils/download.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1324 2023-01-12 17:22:00.000000 upyog-0.7.1/upyog/utils/prettify_df.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     2992 2023-04-16 03:45:58.000000 upyog-0.7.1/upyog/utils/utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      556 2022-08-08 14:04:02.000000 upyog-0.7.1/upyog/utils/zip_utils.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.472107 upyog-0.7.1/upyog.egg-info/
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-05-17 16:23:48.000000 upyog-0.7.1/upyog.egg-info/PKG-INFO
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1022 2023-05-17 16:23:48.000000 upyog-0.7.1/upyog.egg-info/SOURCES.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2023-05-17 16:23:48.000000 upyog-0.7.1/upyog.egg-info/dependency_links.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)      454 2023-05-17 16:23:48.000000 upyog-0.7.1/upyog.egg-info/entry_points.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2022-01-17 09:58:14.000000 upyog-0.7.1/upyog.egg-info/not-zip-safe
--rw-r--r--   0 rahulsomani   (501) staff       (20)      179 2023-05-17 16:23:48.000000 upyog-0.7.1/upyog.egg-info/requires.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)       12 2023-05-17 16:23:48.000000 upyog-0.7.1/upyog.egg-info/top_level.txt
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.060754 upyog-0.7.2/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3488 2023-05-25 07:49:57.000000 upyog-0.7.2/CHANGELOG.md
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      133 2022-01-27 18:07:46.000000 upyog-0.7.2/MANIFEST.in
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-05-25 07:50:05.060864 upyog-0.7.2/PKG-INFO
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)      618 2022-01-15 04:03:41.000000 upyog-0.7.2/README.md
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.051037 upyog-0.7.2/assets/
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.052800 upyog-0.7.2/assets/fonts/
+-rw-rwxrwx   0 rahulsomani   (501) staff       (20)    28432 2022-01-27 13:15:35.000000 upyog-0.7.2/assets/fonts/EuroStyleNormal.ttf
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)     1384 2023-05-25 07:50:05.061343 upyog-0.7.2/setup.cfg
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)      251 2022-01-17 09:53:10.000000 upyog-0.7.2/setup.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.053967 upyog-0.7.2/upyog/
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)       28 2022-10-28 02:44:32.000000 upyog-0.7.2/upyog/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      644 2023-01-24 04:50:27.000000 upyog-0.7.2/upyog/all.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.055839 upyog-0.7.2/upyog/ann/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)        0 2022-01-22 05:11:22.000000 upyog-0.7.2/upyog/ann/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     4426 2022-01-22 20:02:13.000000 upyog-0.7.2/upyog/ann/annoy.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3066 2023-04-16 03:50:08.000000 upyog-0.7.2/upyog/cli.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.057289 upyog-0.7.2/upyog/image/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      141 2022-09-04 09:39:14.000000 upyog-0.7.2/upyog/image/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3340 2023-04-21 18:57:17.000000 upyog-0.7.2/upyog/image/cli.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     2286 2022-09-01 09:27:43.000000 upyog-0.7.2/upyog/image/composition.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)    17235 2023-05-23 10:33:14.000000 upyog-0.7.2/upyog/image/draw.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1526 2023-04-15 11:13:07.000000 upyog-0.7.2/upyog/image/io.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1442 2023-02-28 09:04:05.000000 upyog-0.7.2/upyog/image/pil_operators.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1518 2023-05-17 11:01:32.000000 upyog-0.7.2/upyog/image/utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     7939 2023-02-28 09:16:20.000000 upyog-0.7.2/upyog/image/visualiser.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1306 2023-05-17 15:42:19.000000 upyog-0.7.2/upyog/imports.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.058594 upyog-0.7.2/upyog/ml/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      211 2023-05-17 15:36:44.000000 upyog-0.7.2/upyog/ml/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1419 2023-05-17 11:40:18.000000 upyog-0.7.2/upyog/ml/coreml_utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1803 2023-05-25 07:42:54.000000 upyog-0.7.2/upyog/ml/eval_dataset.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      523 2023-05-25 07:42:28.000000 upyog-0.7.2/upyog/ml/imports.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3662 2023-05-17 16:21:13.000000 upyog-0.7.2/upyog/ml/model_utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1707 2023-05-17 11:41:09.000000 upyog-0.7.2/upyog/ml/preprocessing.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     2066 2023-05-25 07:35:59.000000 upyog-0.7.2/upyog/ml/utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1138 2023-05-17 11:07:07.000000 upyog-0.7.2/upyog/ml/visualise.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1198 2022-06-01 05:03:09.000000 upyog-0.7.2/upyog/nb2script.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.059522 upyog-0.7.2/upyog/os/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      137 2022-10-26 00:24:39.000000 upyog-0.7.2/upyog/os/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     6159 2023-04-16 07:09:32.000000 upyog-0.7.2/upyog/os/cli.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-08-03 15:10:12.000000 upyog-0.7.2/upyog/os/patch_pathlib.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     4424 2023-05-25 07:33:09.000000 upyog-0.7.2/upyog/os/read_files.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3459 2023-05-17 10:58:12.000000 upyog-0.7.2/upyog/os/utils.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.060570 upyog-0.7.2/upyog/utils/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      118 2022-10-28 03:18:43.000000 upyog-0.7.2/upyog/utils/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-04-05 12:59:08.000000 upyog-0.7.2/upyog/utils/boxes.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)    14495 2023-01-11 07:05:00.000000 upyog-0.7.2/upyog/utils/download.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1324 2023-01-12 17:22:00.000000 upyog-0.7.2/upyog/utils/prettify_df.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     2992 2023-04-16 03:45:58.000000 upyog-0.7.2/upyog/utils/utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      556 2022-08-08 14:04:02.000000 upyog-0.7.2/upyog/utils/zip_utils.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-25 07:50:05.055267 upyog-0.7.2/upyog.egg-info/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-05-25 07:50:04.000000 upyog-0.7.2/upyog.egg-info/PKG-INFO
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1022 2023-05-25 07:50:05.000000 upyog-0.7.2/upyog.egg-info/SOURCES.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2023-05-25 07:50:04.000000 upyog-0.7.2/upyog.egg-info/dependency_links.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      454 2023-05-25 07:50:04.000000 upyog-0.7.2/upyog.egg-info/entry_points.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2022-01-17 09:58:14.000000 upyog-0.7.2/upyog.egg-info/not-zip-safe
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      179 2023-05-25 07:50:04.000000 upyog-0.7.2/upyog.egg-info/requires.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)       12 2023-05-25 07:50:04.000000 upyog-0.7.2/upyog.egg-info/top_level.txt
```

### Comparing `upyog-0.7.1/CHANGELOG.md` & `upyog-0.7.2/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-## Unreleased
+## 0.7.2 -- 25 May 2023
+* Font path bugfix...
+* Port over more ML utilities to `upyog.ml`
 
 ## 0.7.1 -- 17 May 2023
 * Rename `InferenceDataset` to `ImageInferenceDataset`
 * Clean up imports
 * Add some more ML functionality from private packages
 
 ## 0.7.0 -- 17 May 2023
```

### Comparing `upyog-0.7.1/PKG-INFO` & `upyog-0.7.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upyog
-Version: 0.7.1
+Version: 0.7.2
 Summary: Myriad Utilities
 Author: Rahul Somani
 Author-email: rsomani95@gmail.com
 License: MIT
 Keywords: utilities
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

### Comparing `upyog-0.7.1/README.md` & `upyog-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/assets/fonts/EuroStyleNormal.ttf` & `upyog-0.7.2/assets/fonts/EuroStyleNormal.ttf`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/setup.cfg` & `upyog-0.7.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = upyog
-version = 0.7.1
+version = 0.7.2
 author = Rahul Somani
 author_email = rsomani95@gmail.com
 description = Myriad Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = utilities
 license = MIT
```

### Comparing `upyog-0.7.1/upyog/all.py` & `upyog-0.7.2/upyog/all.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/ann/annoy.py` & `upyog-0.7.2/upyog/ann/annoy.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/cli.py` & `upyog-0.7.2/upyog/cli.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/image/cli.py` & `upyog-0.7.2/upyog/image/cli.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/image/composition.py` & `upyog-0.7.2/upyog/image/composition.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/image/draw.py` & `upyog-0.7.2/upyog/image/draw.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
     else:
         return get_fallback_font()
 
 
 # DEFAULT_FONT_PATH = str(
 #     Path(__file__).parent.parent.parent / "assets" / "fonts" / "EuroStyleNormal.ttf"
 # )
-DEFAULT_FONT_PATH = str(Path(__file__) / "_Inter-Light.ttf")
+DEFAULT_FONT_PATH = str(Path(__file__).parent / "_Inter-Light.ttf")
 
 
 def get_fallback_font() -> ImageFont.FreeTypeFont:
     return get_font(DEFAULT_FONT_PATH, size=30)
 
 
 def _write_text(
```

### Comparing `upyog-0.7.1/upyog/image/io.py` & `upyog-0.7.2/upyog/image/io.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/image/pil_operators.py` & `upyog-0.7.2/upyog/image/pil_operators.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/image/utils.py` & `upyog-0.7.2/upyog/image/utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/image/visualiser.py` & `upyog-0.7.2/upyog/image/visualiser.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/imports.py` & `upyog-0.7.2/upyog/imports.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/ml/coreml_utils.py` & `upyog-0.7.2/upyog/ml/coreml_utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/ml/eval_dataset.py` & `upyog-0.7.2/upyog/ml/eval_dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from upyog.ml.imports import *
-from upyog.os import get_image_files
+from upyog.os import get_image_files, collate_image_filenames
 from upyog.image import load_image
 
 
-__all__ = ["ImageInferenceDataset"]
+__all__ = ["ImageInferenceDataset", "image_filename_collate_fn"]
 
 
 class ImageInferenceDataset(Dataset, ABC):
     """
     Base class that gathers files from a myriad number of folders / lists of
     filenames and stores them as `self.fnames`.
 
@@ -17,28 +17,28 @@
 
     def __init__(
         self,
         fnames: List[os.PathLike] = None,
         img_folders: Optional[List[os.PathLike]] = None,
         sort_fnames: bool = True,
     ):
-        self.fnames = []
-        if fnames:
-            assert isinstance(fnames, list)
-            self.fnames.extend(fnames)
-
-        if img_folders:
-            assert isinstance(img_folders, list)
-            assert [Path(f).exists() for f in img_folders]
-            for folder in img_folders:
-                self.fnames.extend(get_image_files(folder))
-
+        self.fnames = collate_image_filenames(fnames, img_folders)
         if sort_fnames:
             self.fnames.sort()
 
+        num_unique_files = len(set(self.fnames))
+        if not num_unique_files == len(self.fnames):
+            before = len(self.fnames)
+            logger.warning(f"Found {before} - {num_unique_files} duplicate filenames")
+
+            self.fnames = sorted(set(self.fnames))
+            after = len(self.fnames)
+
+            logger.info(f"Removed duplicate filenames. Total no. filenames: {before} -> {after}")
+
     def post_init(self):
         pass
 
     def __len__(self):
         return len(self.fnames)
 
     @abstractmethod
```

### Comparing `upyog-0.7.1/upyog/ml/model_utils.py` & `upyog-0.7.2/upyog/ml/model_utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/ml/preprocessing.py` & `upyog-0.7.2/upyog/ml/preprocessing.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/ml/visualise.py` & `upyog-0.7.2/upyog/ml/visualise.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/nb2script.py` & `upyog-0.7.2/upyog/nb2script.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/os/cli.py` & `upyog-0.7.2/upyog/os/cli.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/os/read_files.py` & `upyog-0.7.2/upyog/os/read_files.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from upyog.utils.utils import flatten
 
 
 """
 Taken from fastaiv1: https://github.com/fastai/fastai1/blob/a8327427ad5137c4899a1b4f74745193c9ea5be3/fastai/data_block.py#L22-L47
 """
 
-__all__ = ["PathLike", "get_files", "get_image_files", "get_video_files"]
+__all__ = ["PathLike", "get_files", "get_image_files", "get_video_files", "collate_image_filenames"]
 
 
 def get_files(
     path: PathLike,
     extensions: Collection[str] = None,
     recurse: bool = False,
     exclude: Optional[Collection[str]] = None,
@@ -105,7 +105,40 @@
     return get_files(
         path=path,
         include=include,
         exclude=exclude,
         recurse=recurse,
         extensions=_VIDEO_EXTENSIONS,
     )
+
+
+def collate_image_filenames(
+    filenames: List[os.PathLike] = None,
+    img_folders: Optional[List[os.PathLike]] = None,
+    sort: bool = True,
+    return_str: bool = False,
+) -> List[PathLike]:
+    """
+    Take a list of `fnames` and `img_folders`, and return a flattened list of
+    all image files in `img_folders` and `fnames` as a single list
+    """
+    all_files = []
+    if filenames is not None:
+        assert isinstance(filenames, list)
+        filenames = [Path(f) for f in filenames]
+        all_files.extend(filenames)
+
+    if img_folders is not None:
+        if isinstance(img_folders, (str, Path)):
+            img_folders = [img_folders]
+        for folder in img_folders:
+            if not Path(folder).exists():
+                raise FileNotFoundError(f"{folder} not found on disk.")
+        for folder in img_folders:
+            all_files.extend(get_image_files(folder))
+
+    if sort:
+        all_files = sorted(all_files)
+
+    if return_str:
+          return [str(f) for f in all_files]
+    else: return all_files
```

### Comparing `upyog-0.7.1/upyog/os/utils.py` & `upyog-0.7.2/upyog/os/utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/utils/download.py` & `upyog-0.7.2/upyog/utils/download.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/utils/prettify_df.py` & `upyog-0.7.2/upyog/utils/prettify_df.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/utils/utils.py` & `upyog-0.7.2/upyog/utils/utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog/utils/zip_utils.py` & `upyog-0.7.2/upyog/utils/zip_utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.1/upyog.egg-info/PKG-INFO` & `upyog-0.7.2/upyog.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upyog
-Version: 0.7.1
+Version: 0.7.2
 Summary: Myriad Utilities
 Author: Rahul Somani
 Author-email: rsomani95@gmail.com
 License: MIT
 Keywords: utilities
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

### Comparing `upyog-0.7.1/upyog.egg-info/SOURCES.txt` & `upyog-0.7.2/upyog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

