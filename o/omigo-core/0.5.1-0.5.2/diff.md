# Comparing `tmp/omigo_core-0.5.1.tar.gz` & `tmp/omigo_core-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omigo_core-0.5.1.tar", last modified: Thu May 25 19:09:59 2023, max compression
+gzip compressed data, was "omigo_core-0.5.2.tar", last modified: Thu May 25 19:16:48 2023, max compression
```

## Comparing `omigo_core-0.5.1.tar` & `omigo_core-0.5.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:59.765351 omigo_core-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-25 19:09:59.765351 omigo_core-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:39.000000 omigo_core-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 19:09:39.000000 omigo_core-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-25 19:09:59.765351 omigo_core-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:59.761351 omigo_core-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:59.765351 omigo_core-0.5.1/src/omigo_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/file_io_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/file_paths_data_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/file_paths_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/file_paths_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/funclib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/local_fs_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/s3_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    17089 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/s3io_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)   213923 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)    28370 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/tsvutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18448 2023-05-25 19:09:39.000000 omigo_core-0.5.1/src/omigo_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:59.765351 omigo_core-0.5.1/src/omigo_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-25 19:09:59.000000 omigo_core-0.5.1/src/omigo_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-25 19:09:59.000000 omigo_core-0.5.1/src/omigo_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:09:59.000000 omigo_core-0.5.1/src/omigo_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-25 19:09:59.000000 omigo_core-0.5.1/src/omigo_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 19:09:59.000000 omigo_core-0.5.1/src/omigo_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:59.765351 omigo_core-0.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-25 19:09:39.000000 omigo_core-0.5.1/test/test_tsv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:48.455191 omigo_core-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-25 19:16:48.455191 omigo_core-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:29.000000 omigo_core-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 19:16:29.000000 omigo_core-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-25 19:16:48.455191 omigo_core-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:48.451190 omigo_core-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:48.451190 omigo_core-0.5.2/src/omigo_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/file_io_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/file_paths_data_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/file_paths_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/file_paths_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/funclib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/local_fs_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/s3_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17089 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/s3io_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)   213923 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28370 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/tsvutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18448 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:48.455191 omigo_core-0.5.2/src/omigo_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-25 19:16:48.000000 omigo_core-0.5.2/src/omigo_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-25 19:16:48.000000 omigo_core-0.5.2/src/omigo_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:16:48.000000 omigo_core-0.5.2/src/omigo_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-25 19:16:48.000000 omigo_core-0.5.2/src/omigo_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 19:16:48.000000 omigo_core-0.5.2/src/omigo_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:48.455191 omigo_core-0.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-25 19:16:29.000000 omigo_core-0.5.2/test/test_tsv.py
```

### Comparing `omigo_core-0.5.1/PKG-INFO` & `omigo_core-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omigo_core
-Version: 0.5.1
+Version: 0.5.2
 Summary: Data Analytics Library for Python
 Home-page: https://github.com/CrowdStrike/omigo-data-analytics
 Author: amit jaiswal
 Author-email: amit.jaiswal@gmail.com
 Project-URL: Bug Tracker, https://github.com/CrowdStrike/omigo-data-analytics/browse
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `omigo_core-0.5.1/setup.cfg` & `omigo_core-0.5.2/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = omigo_core
-version = 0.5.1
+version = 0.5.2
 author = amit jaiswal
 author_email = amit.jaiswal@gmail.com
 description = Data Analytics Library for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CrowdStrike/omigo-data-analytics
 project_urls =
```

### Comparing `omigo_core-0.5.1/src/omigo_core/etl.py` & `omigo_core-0.5.2/src/omigo_core/etl.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.1/src/omigo_core/file_io_wrapper.py` & `omigo_core-0.5.2/src/omigo_core/file_io_wrapper.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.1/src/omigo_core/file_paths_data_reader.py` & `omigo_core-0.5.2/src/omigo_core/file_paths_data_reader.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.1/src/omigo_core/file_paths_reader.py` & `omigo_core-0.5.2/src/omigo_core/file_paths_reader.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.1/src/omigo_core/file_paths_util.py` & `omigo_core-0.5.2/src/omigo_core/file_paths_util.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.1/src/omigo_core/funclib.py` & `omigo_core-0.5.2/src/omigo_core/funclib.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.1/src/omigo_core/local_fs_wrapper.py` & `omigo_core-0.5.2/src/omigo_core/local_fs_wrapper.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.1/src/omigo_core/s3_wrapper.py` & `omigo_core-0.5.2/src/omigo_core/s3_wrapper.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.1/src/omigo_core/s3io_wrapper.py` & `omigo_core-0.5.2/src/omigo_core/s3io_wrapper.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.1/src/omigo_core/tsv.py` & `omigo_core-0.5.2/src/omigo_core/tsv.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.1/src/omigo_core/tsvutils.py` & `omigo_core-0.5.2/src/omigo_core/tsvutils.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.1/src/omigo_core/utils.py` & `omigo_core-0.5.2/src/omigo_core/utils.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.1/src/omigo_core.egg-info/PKG-INFO` & `omigo_core-0.5.2/src/omigo_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omigo-core
-Version: 0.5.1
+Version: 0.5.2
 Summary: Data Analytics Library for Python
 Home-page: https://github.com/CrowdStrike/omigo-data-analytics
 Author: amit jaiswal
 Author-email: amit.jaiswal@gmail.com
 Project-URL: Bug Tracker, https://github.com/CrowdStrike/omigo-data-analytics/browse
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `omigo_core-0.5.1/src/omigo_core.egg-info/SOURCES.txt` & `omigo_core-0.5.2/src/omigo_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

