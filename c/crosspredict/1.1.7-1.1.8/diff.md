# Comparing `tmp/crosspredict-1.1.7.tar.gz` & `tmp/crosspredict-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosspredict-1.1.7.tar", last modified: Thu Apr 13 14:28:36 2023, max compression
+gzip compressed data, was "crosspredict-1.1.8.tar", last modified: Thu May 25 11:28:22 2023, max compression
```

## Comparing `crosspredict-1.1.7.tar` & `crosspredict-1.1.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.817636 crosspredict-1.1.7/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     1074 2022-09-26 07:29:13.000000 crosspredict-1.1.7/LICENSE
--rw-r--r--   0 vboyadzhi   (503) staff       (20)       58 2022-09-26 07:29:13.000000 crosspredict-1.1.7/MANIFEST.in
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     5584 2023-04-13 14:28:36.817513 crosspredict-1.1.7/PKG-INFO
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     5151 2022-09-26 07:59:16.000000 crosspredict-1.1.7/README.md
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.808367 crosspredict-1.1.7/crosspredict/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)       44 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/__init__.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.809363 crosspredict-1.1.7/crosspredict/__pycache__/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      206 2022-09-26 08:25:52.000000 crosspredict-1.1.7/crosspredict/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     4094 2022-09-26 08:26:01.000000 crosspredict-1.1.7/crosspredict/__pycache__/iterator.cpython-39.pyc
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.810357 crosspredict-1.1.7/crosspredict/crossval/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      241 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/crossval/__init__.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.811351 crosspredict-1.1.7/crosspredict/crossval/__pycache__/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      380 2022-09-26 08:25:52.000000 crosspredict-1.1.7/crosspredict/crossval/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     3213 2022-09-26 08:26:02.000000 crosspredict-1.1.7/crosspredict/crossval/__pycache__/_catboost.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     7803 2022-10-01 14:55:03.000000 crosspredict-1.1.7/crosspredict/crossval/__pycache__/_crossval.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     2885 2022-09-26 08:57:16.000000 crosspredict-1.1.7/crosspredict/crossval/__pycache__/_lightgbm.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     1763 2022-09-26 08:26:01.000000 crosspredict-1.1.7/crosspredict/crossval/__pycache__/_xgboost.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     3869 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/crossval/_catboost.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)    12175 2023-04-13 13:11:46.000000 crosspredict-1.1.7/crosspredict/crossval/_crossval.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     3848 2022-09-26 08:57:01.000000 crosspredict-1.1.7/crosspredict/crossval/_lightgbm.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     2331 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/crossval/_xgboost.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     4965 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/iterator.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.811673 crosspredict-1.1.7/crosspredict/nodes/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      215 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/nodes/__init__.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)    12522 2023-04-13 13:11:46.000000 crosspredict-1.1.7/crosspredict/nodes/_nodes.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     1580 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/parameters.yml
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.813274 crosspredict-1.1.7/crosspredict/report_binary/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      138 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/report_binary/__init__.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.814702 crosspredict-1.1.7/crosspredict/report_binary/__pycache__/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      323 2022-09-26 08:27:01.000000 crosspredict-1.1.7/crosspredict/report_binary/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     8585 2022-09-26 08:27:01.000000 crosspredict-1.1.7/crosspredict/report_binary/__pycache__/_curves.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     9111 2022-09-26 08:27:01.000000 crosspredict-1.1.7/crosspredict/report_binary/__pycache__/_report_binary.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     7896 2023-04-13 13:11:46.000000 crosspredict-1.1.7/crosspredict/report_binary/_curves.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)    12423 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/report_binary/_report_binary.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.815164 crosspredict-1.1.7/crosspredict/target_encoder/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      174 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/target_encoder/__init__.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     2836 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/target_encoder/_crosstargetencoder.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     3471 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/target_encoder/_target_encoder.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.809037 crosspredict-1.1.7/crosspredict.egg-info/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     5584 2023-04-13 14:28:36.000000 crosspredict-1.1.7/crosspredict.egg-info/PKG-INFO
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     1470 2023-04-13 14:28:36.000000 crosspredict-1.1.7/crosspredict.egg-info/SOURCES.txt
--rw-r--r--   0 vboyadzhi   (503) staff       (20)        1 2023-04-13 14:28:36.000000 crosspredict-1.1.7/crosspredict.egg-info/dependency_links.txt
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      247 2023-04-13 14:28:36.000000 crosspredict-1.1.7/crosspredict.egg-info/requires.txt
--rw-r--r--   0 vboyadzhi   (503) staff       (20)       19 2023-04-13 14:28:36.000000 crosspredict-1.1.7/crosspredict.egg-info/top_level.txt
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      246 2022-09-26 08:59:16.000000 crosspredict-1.1.7/requirements.txt
--rw-r--r--   0 vboyadzhi   (503) staff       (20)       38 2023-04-13 14:28:36.817679 crosspredict-1.1.7/setup.cfg
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     1272 2023-04-13 13:12:24.000000 crosspredict-1.1.7/setup.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.817190 crosspredict-1.1.7/tests/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)        0 2022-09-26 07:29:13.000000 crosspredict-1.1.7/tests/__init__.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      556 2022-09-26 07:29:13.000000 crosspredict-1.1.7/tests/conftest.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     7765 2022-09-26 08:47:46.000000 crosspredict-1.1.7/tests/test_binary.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     2518 2022-09-26 07:29:13.000000 crosspredict-1.1.7/tests/test_iterator.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:22.439760 crosspredict-1.1.8/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     1074 2022-09-26 07:29:13.000000 crosspredict-1.1.8/LICENSE
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)       58 2022-09-26 07:29:13.000000 crosspredict-1.1.8/MANIFEST.in
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     5584 2023-05-25 11:28:22.438939 crosspredict-1.1.8/PKG-INFO
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     5151 2022-09-26 07:59:16.000000 crosspredict-1.1.8/README.md
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:21.688412 crosspredict-1.1.8/crosspredict/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)       44 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/__init__.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:21.691027 crosspredict-1.1.8/crosspredict/__pycache__/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      206 2022-09-26 08:25:52.000000 crosspredict-1.1.8/crosspredict/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     4094 2022-09-26 08:26:01.000000 crosspredict-1.1.8/crosspredict/__pycache__/iterator.cpython-39.pyc
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:22.383877 crosspredict-1.1.8/crosspredict/crossval/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      241 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/crossval/__init__.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:22.387813 crosspredict-1.1.8/crosspredict/crossval/__pycache__/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      380 2022-09-26 08:25:52.000000 crosspredict-1.1.8/crosspredict/crossval/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     3213 2022-09-26 08:26:02.000000 crosspredict-1.1.8/crosspredict/crossval/__pycache__/_catboost.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     7886 2023-05-25 11:27:14.000000 crosspredict-1.1.8/crosspredict/crossval/__pycache__/_crossval.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     2885 2022-09-26 08:57:16.000000 crosspredict-1.1.8/crosspredict/crossval/__pycache__/_lightgbm.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     1763 2022-09-26 08:26:01.000000 crosspredict-1.1.8/crosspredict/crossval/__pycache__/_xgboost.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     3869 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/crossval/_catboost.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)    11738 2023-05-25 11:26:23.000000 crosspredict-1.1.8/crosspredict/crossval/_crossval.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     3848 2022-09-26 08:57:01.000000 crosspredict-1.1.8/crosspredict/crossval/_lightgbm.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     2331 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/crossval/_xgboost.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     4965 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/iterator.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:22.388913 crosspredict-1.1.8/crosspredict/nodes/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      215 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/nodes/__init__.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)    12522 2023-04-13 13:11:46.000000 crosspredict-1.1.8/crosspredict/nodes/_nodes.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     1580 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/parameters.yml
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:22.435022 crosspredict-1.1.8/crosspredict/report_binary/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      138 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/report_binary/__init__.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:22.436123 crosspredict-1.1.8/crosspredict/report_binary/__pycache__/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      323 2022-09-26 08:27:01.000000 crosspredict-1.1.8/crosspredict/report_binary/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     8606 2023-05-25 10:01:03.000000 crosspredict-1.1.8/crosspredict/report_binary/__pycache__/_curves.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     9111 2022-09-26 08:27:01.000000 crosspredict-1.1.8/crosspredict/report_binary/__pycache__/_report_binary.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     7896 2023-04-13 13:11:46.000000 crosspredict-1.1.8/crosspredict/report_binary/_curves.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)    12423 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/report_binary/_report_binary.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:22.436968 crosspredict-1.1.8/crosspredict/target_encoder/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      174 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/target_encoder/__init__.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     2836 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/target_encoder/_crosstargetencoder.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     3471 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/target_encoder/_target_encoder.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:21.690551 crosspredict-1.1.8/crosspredict.egg-info/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     5584 2023-05-25 11:28:21.000000 crosspredict-1.1.8/crosspredict.egg-info/PKG-INFO
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     1470 2023-05-25 11:28:21.000000 crosspredict-1.1.8/crosspredict.egg-info/SOURCES.txt
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)        1 2023-05-25 11:28:21.000000 crosspredict-1.1.8/crosspredict.egg-info/dependency_links.txt
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      247 2023-05-25 11:28:21.000000 crosspredict-1.1.8/crosspredict.egg-info/requires.txt
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)       19 2023-05-25 11:28:21.000000 crosspredict-1.1.8/crosspredict.egg-info/top_level.txt
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      246 2022-09-26 08:59:16.000000 crosspredict-1.1.8/requirements.txt
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)       38 2023-05-25 11:28:22.439974 crosspredict-1.1.8/setup.cfg
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     1272 2023-05-25 11:28:06.000000 crosspredict-1.1.8/setup.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:22.437784 crosspredict-1.1.8/tests/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)        0 2022-09-26 07:29:13.000000 crosspredict-1.1.8/tests/__init__.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      556 2022-09-26 07:29:13.000000 crosspredict-1.1.8/tests/conftest.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     7765 2022-09-26 08:47:46.000000 crosspredict-1.1.8/tests/test_binary.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     2518 2022-09-26 07:29:13.000000 crosspredict-1.1.8/tests/test_iterator.py
```

### Comparing `crosspredict-1.1.7/LICENSE` & `crosspredict-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/PKG-INFO` & `crosspredict-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosspredict
-Version: 1.1.7
+Version: 1.1.8
 Summary: package for easy crossvalidation
 Home-page: UNKNOWN
 Author: Vladislav Boyadzhi
 Author-email: vladislav.boyadzhi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crosspredict-1.1.7/README.md` & `crosspredict-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/crosspredict/__pycache__/iterator.cpython-39.pyc` & `crosspredict-1.1.8/crosspredict/__pycache__/iterator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/crosspredict/crossval/__pycache__/_catboost.cpython-39.pyc` & `crosspredict-1.1.8/crosspredict/crossval/__pycache__/_catboost.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/crosspredict/crossval/__pycache__/_crossval.cpython-39.pyc` & `crosspredict-1.1.8/crosspredict/crossval/__pycache__/_crossval.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Oct  1 14:54:19 2022 UTC, .py size: 11711 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 9b54 3863 bf2d 0000  a........T8c.-..
+00000000: 610d 0d0a 0000 0000 df45 6f64 da2d 0000  a........Eod.-..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 5a06 6400 6403 6c07 5a07 6400 6403 6c08  Z.d.d.l.Z.d.d.l.
 00000060: 5a09 6400 6403 6c0a 5a0a 6400 6403 6c0b  Z.d.d.l.Z.d.d.l.
 00000070: 6d0c 5a0d 0100 6400 6403 6c0e 5a0f 6400  m.Z...d.d.l.Z.d.
@@ -106,20 +106,20 @@
 00000690: 645f 6e61 6d65 721d 0000 00da 0c65 7661  d_namer......eva
 000006a0: 6c73 5f72 6573 756c 7472 3000 0000 721e  ls_resultr0...r.
 000006b0: 0000 00da 0c76 6572 626f 7365 5f65 7661  .....verbose_eva
 000006c0: 6c72 2900 0000 7229 0000 0072 2a00 0000  lr)...r)...r*...
 000006d0: da05 7472 6169 6e3c 0000 0073 0200 0000  ..train<...s....
 000006e0: 000d 7a16 4372 6f73 734d 6f64 656c 4661  ..z.CrossModelFa
 000006f0: 6272 6963 2e74 7261 696e 6302 0000 0000  bric.trainc.....
-00000700: 0000 0000 0000 0015 0000 000d 0000 0043  ...............C
-00000710: 0000 0073 d002 0000 7400 a001 7402 a101  ...s....t...t...
+00000700: 0000 0000 0000 0016 0000 000d 0000 0043  ...............C
+00000710: 0000 0073 e602 0000 7400 a001 7402 a101  ...s....t...t...
 00000720: 7d02 6900 7d03 6700 7d04 7c02 a003 7c00  }.i.}.g.}.|...|.
 00000730: 6a04 a101 0100 7c00 6a05 6a06 7c01 6401  j.....|.j.j.|.d.
 00000740: 8d01 0100 7407 7c00 6a05 a008 7c01 a101  ....t.|.j...|...
-00000750: 8301 4400 9001 5dd2 5c02 7d05 5c02 7d06  ..D...].\.}.\.}.
+00000750: 8301 4400 9001 5dce 5c02 7d05 5c02 7d06  ..D...].\.}.\.}.
 00000760: 7d07 7c00 6a09 6400 7501 728e 7c00 6a09  }.|.j.d.u.r.|.j.
 00000770: 6a0a 7c05 7c06 7c07 6402 8d03 5c02 7d08  j.|.|.|.d...\.}.
 00000780: 7d09 740b 6a0c 7c06 7c08 6702 6403 6404  }.t.j.|.|.g.d.d.
 00000790: 8d02 7d06 740b 6a0c 7c07 7c09 6702 6403  ..}.t.j.|.|.g.d.
 000007a0: 6404 8d02 7d07 7c06 7c00 6a0d 1900 7c07  d...}.|.|.j...|.
 000007b0: 7c00 6a0d 1900 0200 7d0a 7d0b 7c06 7c00  |.j.....}.}.|.|.
 000007c0: 6a0e 1900 7c07 7c00 6a0e 1900 0200 7d0c  j...|.|.j.....}.
@@ -132,357 +132,362 @@
 00000830: 6a13 7c00 6a04 7c0e 6409 7c0f 640a 7c00  j.|.j.|.d.|.d.|.
 00000840: 6a14 7c10 7c00 6a10 7c00 6a15 640b 640c  j.|.|.j.|.j.d.d.
 00000850: 8d0a 7d11 6e1a 7c00 6a13 7c00 6a04 7c0e  ..}.n.|.j.|.j.|.
 00000860: 7c00 6a14 7c00 6a10 640b 640d 8d05 7d11  |.j.|.j.d.d...}.
 00000870: 7c11 7c00 6a16 7c05 3c00 7c00 6a12 723c  |.|.j.|.<.|.j.r<
 00000880: 7c00 6a04 640e 1900 640f 7600 9001 7290  |.j.d...d.v...r.
 00000890: 7c10 640a 1900 7c00 6a04 640e 1900 1900  |.d...|.j.d.....
-000008a0: 7c03 7c05 3c00 6e34 7c00 6a04 640e 1900  |.|.<.n4|.j.d...
-000008b0: 6410 7600 9001 72c4 6411 6412 8400 6413  d.v...r.d.d...d.
-000008c0: 7c10 640a 1900 7c00 6a04 640e 1900 1900  |.d...|.j.d.....
-000008d0: 1400 4400 8301 7c03 7c05 3c00 7417 a018  ..D...|.|.<.t...
-000008e0: 7c10 640a 1900 7c00 6a04 640e 1900 1900  |.d...|.j.d.....
-000008f0: a101 7d12 7c04 a019 7c12 a101 0100 7c02  ..}.|...|.....|.
-00000900: a003 6414 7c05 7c00 6a05 6a11 1600 9b00  ..d.|.|.j.j.....
-00000910: 6415 7c00 6a04 640e 1900 9b00 6416 7c12  d.|.j.d.....d.|.
-00000920: 9b00 9d06 a101 0100 713c 7c00 6a12 9002  ........q<|.j...
-00000930: 72cc 740b a01a 741b 6417 6412 8400 7c03  r.t...t.d.d...|.
-00000940: a01c a100 4400 8301 8301 a101 7c00 5f1d  ....D.......|._.
-00000950: 7c00 6a1d a01e a100 6a1f 6403 6404 8d01  |.j.....j.d.d...
-00000960: 6406 6b02 7d13 7417 a020 7c00 6a1d 7c13  d.k.}.t.. |.j.|.
-00000970: 1900 6a21 6403 6404 8d01 6a22 a101 7c00  ..j!d.d...j"..|.
-00000980: 5f23 7c00 6a1d 7c13 1900 6a21 6403 6404  _#|.j.|...j!d.d.
-00000990: 8d01 7c00 6a23 1900 7c00 5f24 7c00 6a1d  ..|.j#..|._$|.j.
-000009a0: 7c13 1900 6a25 6403 6404 8d01 7c00 6a23  |...j%d.d...|.j#
-000009b0: 1900 7c00 5f25 7c00 6a24 0b00 7426 7c00  ..|._%|.j$..t&|.
-000009c0: 6a25 7c00 6a24 7c04 7427 7c00 6a23 8301  j%|.j$|.t'|.j#..
-000009d0: 6418 9c06 7d14 7c02 a003 7c14 a101 0100  d...}.|...|.....
-000009e0: 7c14 5300 7c00 5300 2919 4ea9 01da 0264  |.S.|.S.).N....d
-000009f0: 66a9 03da 0466 6f6c 6472 3900 0000 da04  f....foldr9.....
-00000a00: 7465 7374 e901 0000 00a9 01da 0461 7869  test.........axi
-00000a10: 7329 0372 2e00 0000 722f 0000 0072 3000  s).r....r/...r0.
-00000a20: 0000 7201 0000 007a 0d52 4550 4541 5420  ..r....z.REPEAT 
-00000a30: 464f 4c44 5320 7a06 2053 5441 5254 7239  FOLDS z. STARTr9
-00000a40: 0000 00da 0465 7661 6c46 290a 721a 0000  .....evalF).r...
-00000a50: 0072 3300 0000 7234 0000 00da 0976 616c  .r3...r4.....val
-00000a60: 6964 5f73 6574 7236 0000 0072 1d00 0000  id_setr6...r....
-00000a70: 7237 0000 0072 3000 0000 721e 0000 0072  r7...r0...r....r
-00000a80: 3800 0000 2905 721a 0000 0072 3300 0000  8...).r....r3...
-00000a90: 721d 0000 0072 3000 0000 7238 0000 0072  r....r0...r8...r
-00000aa0: 0b00 0000 a903 da03 6175 6372 1800 0000  ........aucr....
-00000ab0: 7219 0000 00a9 0c72 1000 0000 7211 0000  r......r....r...
-00000ac0: 0072 1200 0000 7213 0000 0072 0c00 0000  .r....r....r....
-00000ad0: 720d 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
-00000ae0: 1400 0000 7215 0000 0072 1600 0000 7217  ....r....r....r.
-00000af0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000b00: 0200 0000 0400 0000 5300 0000 7314 0000  ........S...s...
-00000b10: 0067 007c 005d 0c7d 0164 007c 0114 0091  .g.|.].}.d.|....
-00000b20: 0271 0453 0029 01e9 ffff ffff 7229 0000  .q.S.)......r)..
-00000b30: 0029 02da 022e 30da 0178 7229 0000 0072  .)....0..xr)...r
-00000b40: 2900 0000 722a 0000 00da 0a3c 6c69 7374  )...r*.....<list
-00000b50: 636f 6d70 3e84 0000 00f3 0000 0000 7a28  comp>.........z(
-00000b60: 4372 6f73 734d 6f64 656c 4661 6272 6963  CrossModelFabric
-00000b70: 2e66 6974 2e3c 6c6f 6361 6c73 3e2e 3c6c  .fit.<locals>.<l
-00000b80: 6973 7463 6f6d 703e 7247 0000 007a 1609  istcomp>rG...z..
-00000b90: 4352 4f53 5356 414c 4944 4154 494f 4e20  CROSSVALIDATION 
-00000ba0: 464f 4c44 207a 1120 454e 4453 2077 6974  FOLD z. ENDS wit
-00000bb0: 6820 6265 7374 2060 7a04 6020 3d20 6301  h best `z.` = c.
-00000bc0: 0000 0000 0000 0000 0000 0003 0000 0006  ................
-00000bd0: 0000 0053 0000 0073 1e00 0000 6700 7c00  ...S...s....g.|.
-00000be0: 5d16 5c02 7d01 7d02 7c01 7400 a001 7c02  ].\.}.}.|.t...|.
-00000bf0: a101 6602 9102 7104 5300 7229 0000 0029  ..f...q.S.r)...)
-00000c00: 02da 0270 64da 0653 6572 6965 7329 0372  ...pd..Series).r
-00000c10: 4800 0000 da01 6bda 0176 7229 0000 0072  H.....k..vr)...r
-00000c20: 2900 0000 722a 0000 0072 4a00 0000 8e00  )...r*...rJ.....
-00000c30: 0000 724b 0000 0029 06da 046c 6f73 73da  ..rK...)...loss.
-00000c40: 0673 7461 7475 7372 2700 0000 7225 0000  .statusr'...r%..
-00000c50: 005a 0a73 636f 7265 735f 616c 6c5a 096e  .Z.scores_allZ.n
-00000c60: 756d 5f62 6f6f 7374 2928 da07 6c6f 6767  um_boost)(..logg
-00000c70: 696e 67da 0967 6574 4c6f 6767 6572 da08  ing..getLogger..
-00000c80: 5f5f 6e61 6d65 5f5f da04 696e 666f 721a  __name__..infor.
-00000c90: 0000 0072 0a00 0000 da03 6669 74da 0965  ...r......fit..e
-00000ca0: 6e75 6d65 7261 7465 da05 7370 6c69 7472  numerate..splitr
-00000cb0: 2200 0000 da09 7472 616e 7366 6f72 6d72  ".....transformr
-00000cc0: 4c00 0000 da06 636f 6e63 6174 721b 0000  L.....concatr...
-00000cd0: 0072 2000 0000 7232 0000 0072 1c00 0000  .r ...r2...r....
-00000ce0: da08 6e5f 7370 6c69 7473 721f 0000 0072  ..n_splitsr....r
-00000cf0: 3900 0000 721d 0000 0072 1e00 0000 7223  9...r....r....r#
-00000d00: 0000 00da 026e 70da 036d 6178 da06 6170  .....np..max..ap
-00000d10: 7065 6e64 da09 4461 7461 4672 616d 65da  pend..DataFrame.
-00000d20: 0464 6963 74da 0569 7465 6d73 7224 0000  .dict..itemsr$..
-00000d30: 00da 0669 736e 756c 6cda 0373 756d da06  ...isnull..sum..
-00000d40: 6172 676d 6178 da04 6d65 616e da06 7661  argmax..mean..va
-00000d50: 6c75 6573 7226 0000 0072 2500 0000 7227  luesr&...r%...r'
-00000d60: 0000 0072 0400 0000 da03 696e 7429 1572  ...r......int).r
-00000d70: 2800 0000 723b 0000 00da 036c 6f67 7224  (...r;.....logr$
-00000d80: 0000 005a 0a73 636f 7265 735f 6176 6772  ...Z.scores_avgr
-00000d90: 3d00 0000 7239 0000 00da 0376 616c da0d  =...r9.....val..
-00000da0: 656e 636f 6465 645f 7472 6169 6eda 0c65  encoded_train..e
-00000db0: 6e63 6f64 6564 5f74 6573 74da 0758 5f74  ncoded_test..X_t
-00000dc0: 7261 696e da05 585f 7661 6cda 0779 5f74  rain..X_val..y_t
-00000dd0: 7261 696e da05 795f 7661 6c5a 0664 7472  rain..y_valZ.dtr
-00000de0: 6169 6e5a 0664 7661 6c69 6472 3700 0000  ainZ.dvalidr7...
-00000df0: da05 6d6f 6465 6c5a 0862 6573 745f 6175  ..modelZ.best_au
-00000e00: 63da 046d 6173 6bda 0672 6573 756c 7472  c..mask..resultr
-00000e10: 2900 0000 7229 0000 0072 2a00 0000 7256  )...r)...r*...rV
-00000e20: 0000 004b 0000 0073 9e00 0000 0001 0a01  ...K...s........
-00000e30: 0401 0401 0c02 0e02 1e01 0a01 0601 06ff  ................
-00000e40: 0a02 1201 1202 1601 1602 0401 0201 0201  ................
-00000e50: 04fd 0604 0801 04ff 0603 1201 1a03 0401  ................
-00000e60: 0801 0401 0401 0201 0201 0201 0201 0401  ................
-00000e70: 0201 0401 0401 02f6 080c 0801 0201 0401  ................
-00000e80: 0401 02fc 0606 0a01 0602 1001 1801 1003  ................
-00000e90: 2402 1801 0a02 0401 22ff 0603 0801 0401  $.......".......
-00000ea0: 14ff 0602 1601 0401 12ff 0602 0a01 02ff  ................
-00000eb0: 0401 04ff 0603 1a03 0601 0201 0401 0401  ................
-00000ec0: 0201 08fb 0607 0a01 0401 7a14 4372 6f73  ..........z.Cros
-00000ed0: 734d 6f64 656c 4661 6272 6963 2e66 6974  sModelFabric.fit
-00000ee0: 6302 0000 0000 0000 0000 0000 000f 0000  c...............
-00000ef0: 0008 0000 0043 0000 0073 fc00 0000 7c01  .....C...s....|.
-00000f00: 7c00 6a00 1900 7d02 7c01 7c00 6a01 1900  |.j...}.|.|.j...
-00000f10: 7d03 7402 6a03 7c01 6a04 7405 a006 7c01  }.t.j.|.j.t...|.
-00000f20: 6a07 6401 1900 a101 6402 8d02 7d04 7408  j.d.....d...}.t.
-00000f30: 7c00 6a09 a00a 7c01 a101 8301 4400 5db6  |.j...|.....D.].
-00000f40: 5c02 7d05 5c02 7d06 7d07 7c00 6a0b 6400  \.}.\.}.}.|.j.d.
-00000f50: 7501 7290 7c00 6a0b 6a0c 7c05 7c06 7c07  u.r.|.j.j.|.|.|.
-00000f60: 6403 8d03 5c02 7d08 7d09 7402 6a0d 7c06  d...\.}.}.t.j.|.
-00000f70: 7c08 6702 6404 6405 8d02 7d06 7402 6a0d  |.g.d.d...}.t.j.
-00000f80: 7c07 7c09 6702 6404 6405 8d02 7d07 7c06  |.|.g.d.d...}.|.
-00000f90: 7c00 6a00 1900 7c07 7c00 6a00 1900 0200  |.j...|.|.j.....
-00000fa0: 7d0a 7d0b 7c06 7c00 6a01 1900 7c07 7c00  }.}.|.|.j...|.|.
-00000fb0: 6a01 1900 0200 7d0c 7d0d 7c00 6a0e 7c05  j.....}.}.|.j.|.
-00000fc0: 1900 7d0e 7c04 6a0f 7c0b 6a04 0500 1900  ..}.|.j.|.j.....
-00000fd0: 7c0e 6a10 7c0b 7c0e a000 a100 1900 7c00  |.j.|.|.......|.
-00000fe0: 6a11 6406 8d02 7c00 6a09 6a12 1b00 3700  j.d...|.j.j...7.
-00000ff0: 0300 3c00 7140 7c04 5300 2907 4e72 0100  ..<.q@|.S.).Nr..
-00001000: 0000 a902 da05 696e 6465 7872 2e00 0000  ......indexr....
-00001010: 723c 0000 0072 3f00 0000 7240 0000 00a9  r<...r?...r@....
-00001020: 01da 0d6e 756d 5f69 7465 7261 7469 6f6e  ...num_iteration
-00001030: 2913 721b 0000 0072 2000 0000 724c 0000  ).r....r ...rL..
-00001040: 0072 4d00 0000 7274 0000 0072 5c00 0000  .rM...rt...r\...
-00001050: da05 7a65 726f 73da 0573 6861 7065 7257  ..zeros..shaperW
-00001060: 0000 0072 0a00 0000 7258 0000 0072 2200  ...r....rX...r".
-00001070: 0000 7259 0000 0072 5a00 0000 7223 0000  ..rY...rZ...r#..
-00001080: 00da 036c 6f63 da07 7072 6564 6963 7472  ...loc..predictr
-00001090: 2600 0000 da09 6e5f 7265 7065 6174 7329  &.....n_repeats)
-000010a0: 0f72 2800 0000 723b 0000 0072 4900 0000  .r(...r;...rI...
-000010b0: da01 7972 7a00 0000 723d 0000 0072 3900  ..yrz...r=...r9.
-000010c0: 0000 7269 0000 0072 6a00 0000 726b 0000  ..ri...rj...rk..
-000010d0: 0072 6c00 0000 726d 0000 0072 6e00 0000  .rl...rm...rn...
-000010e0: 726f 0000 0072 7000 0000 7229 0000 0072  ro...rp...r)...r
-000010f0: 2900 0000 722a 0000 0072 5900 0000 a300  )...r*...rY.....
-00001100: 0000 732a 0000 0000 010a 010a 011c 021c  ..s*............
-00001110: 010a 0106 0106 ff0a 0212 0112 0216 0116  ................
-00001120: 030a 010c 010e 0104 ff04 0106 ff02 ff08  ................
-00001130: 047a 1a43 726f 7373 4d6f 6465 6c46 6162  .z.CrossModelFab
-00001140: 7269 632e 7472 616e 7366 6f72 6d63 0200  ric.transformc..
-00001150: 0000 0000 0000 0000 0000 0700 0000 0600  ................
-00001160: 0000 4300 0000 7390 0000 0074 006a 017c  ..C...s....t.j.|
-00001170: 016a 0274 03a0 047c 016a 0564 0119 00a1  .j.t...|.j.d....
-00001180: 0164 028d 027d 0274 067c 006a 07a0 08a1  .d...}.t.|.j....
-00001190: 0083 017d 037c 006a 0964 0075 0172 527c  ...}.|.j.d.u.rR|
-000011a0: 006a 09a0 0a7c 01a1 017d 0474 006a 0b7c  .j...|...}.t.j.|
-000011b0: 017c 0467 0264 0364 048d 027d 017c 006a  .|.g.d.d...}.|.j
-000011c0: 07a0 08a1 0044 005d 2e7d 057c 006a 077c  .....D.].}.|.j.|
-000011d0: 0519 007d 067c 027c 066a 0a7c 017c 06a0  ...}.|.|.j.|.|..
-000011e0: 0ca1 0019 007c 006a 0d64 058d 027c 031b  .....|.j.d...|..
-000011f0: 0037 007d 0271 5c7c 0253 0029 064e 7201  .7.}.q\|.S.).Nr.
-00001200: 0000 0072 7300 0000 723f 0000 0072 4000  ...rs...r?...r@.
-00001210: 0000 7275 0000 0029 0e72 4c00 0000 724d  ..ru...).rL...rM
-00001220: 0000 0072 7400 0000 725c 0000 0072 7700  ...rt...r\...rw.
-00001230: 0000 7278 0000 00da 036c 656e 7223 0000  ..rx.....lenr#..
-00001240: 00da 046b 6579 7372 2200 0000 727a 0000  ...keysr"...rz..
-00001250: 0072 5a00 0000 721b 0000 0072 2600 0000  .rZ...r....r&...
-00001260: 2907 7228 0000 0072 3e00 0000 727a 0000  ).r(...r>...rz..
-00001270: 005a 0a6d 6f64 656c 735f 6c65 6e72 6b00  .Z.models_lenrk.
-00001280: 0000 723d 0000 0072 7000 0000 7229 0000  ..r=...rp...r)..
-00001290: 0072 2900 0000 722a 0000 0072 7a00 0000  .r)...r*...rz...
-000012a0: ba00 0000 7312 0000 0000 011c 010e 010a  ....s...........
-000012b0: 010c 0112 020e 010a 0122 027a 1843 726f  .........".z.Cro
-000012c0: 7373 4d6f 6465 6c46 6162 7269 632e 7072  ssModelFabric.pr
-000012d0: 6564 6963 7463 0300 0000 0000 0000 0000  edictc..........
-000012e0: 0000 0300 0000 0300 0000 4300 0000 7338  ..........C...s8
-000012f0: 0000 007c 006a 0064 0119 0064 0276 0072  ...|.j.d...d.v.r
-00001300: 1c7c 01a0 017c 02a1 0164 0319 0053 007c  .|...|...d...S.|
-00001310: 006a 0064 0119 0064 0476 0072 347c 01a0  .j.d...d.v.r4|..
-00001320: 017c 02a1 0153 0064 0053 0029 054e 720b  .|...S.d.S.).Nr.
-00001330: 0000 0072 4400 0000 723f 0000 0072 4600  ...rD...r?...rF.
-00001340: 0000 2902 721a 0000 00da 0b73 6861 705f  ..).r......shap_
-00001350: 7661 6c75 6573 2903 7228 0000 00da 0965  values).r(.....e
-00001360: 7870 6c61 696e 6572 da09 6466 5f73 616d  xplainer..df_sam
-00001370: 706c 6572 2900 0000 7229 0000 0072 2a00  pler)...r)...r*.
-00001380: 0000 da10 5f67 6574 5f73 6861 705f 7661  ...._get_shap_va
-00001390: 6c75 6573 c700 0000 7308 0000 0000 010e  lues....s.......
-000013a0: 010e 010e 037a 2143 726f 7373 4d6f 6465  .....z!CrossMode
-000013b0: 6c46 6162 7269 632e 5f67 6574 5f73 6861  lFabric._get_sha
-000013c0: 705f 7661 6c75 6573 e9f4 0100 00a9 02e9  p_values........
-000013d0: 0a00 0000 7285 0000 0072 3a00 0000 6304  ....r....r:...c.
-000013e0: 0000 0000 0000 0000 0000 001b 0000 0008  ................
-000013f0: 0000 0043 0000 0073 ce01 0000 7400 6a01  ...C...s....t.j.
-00001400: 7c03 6401 8d01 7d04 7402 a003 7404 a101  |.d...}.t...t...
-00001410: 7d05 7405 6a06 6402 6701 6403 8d01 7d06  }.t.j.d.g.d...}.
-00001420: 7c01 7c00 6a07 1900 7d07 7c01 7c00 6a08  |.|.j...}.|.|.j.
-00001430: 1900 7d08 7409 7c00 6a0a a00b 7c01 a101  ..}.t.|.j...|...
-00001440: 8301 4400 5dfa 5c02 7d09 5c02 7d0a 7d0b  ..D.].\.}.\.}.}.
-00001450: 7c00 6a0c 6404 7501 7298 7c00 6a0c 6a0d  |.j.d.u.r.|.j.j.
-00001460: 7c09 7c0a 7c0b 6405 8d03 5c02 7d0c 7d0d  |.|.|.d...\.}.}.
-00001470: 7405 6a0e 7c0a 7c0c 6702 6406 6407 8d02  t.j.|.|.g.d.d...
-00001480: 7d0a 7405 6a0e 7c0b 7c0d 6702 6406 6407  }.t.j.|.|.g.d.d.
-00001490: 8d02 7d0b 7c0a 7c00 6a07 1900 7c0b 7c00  ..}.|.|.j...|.|.
-000014a0: 6a07 1900 0200 7d0e 7d0f 7c0a 7c00 6a08  j.....}.}.|.|.j.
-000014b0: 1900 7c0b 7c00 6a08 1900 0200 7d10 7d11  ..|.|.j.....}.}.
-000014c0: 7c00 6a0f 7c09 1900 7d12 7410 a011 7c12  |.j.|...}.t...|.
-000014d0: a101 7d13 7c0f 7c12 a007 a100 1900 6a12  ..}.|.|.......j.
-000014e0: 7c02 6408 6409 640a 8d03 7d14 7c00 a013  |.d.d.d...}.|...
-000014f0: 7c13 7c14 a102 7d15 7405 6a06 7414 7c12  |.|...}.t.j.t.|.
-00001500: a007 a100 7415 6a16 7415 a017 7c15 a101  ....t.j.t...|...
-00001510: 6408 6407 8d02 8302 6402 640b 7418 7c09  d.d.....d.d.t.|.
-00001520: 8301 1700 6702 6403 8d02 7d16 7405 6a19  ....g.d...}.t.j.
-00001530: 7c06 7c16 640c 6402 640d 8d04 7d06 7148  |.|.d.d.d...}.qH
-00001540: 7c06 a01a 6402 a101 6a1b 640e 640f 6702  |...d...j.d.d.g.
-00001550: 6406 6407 8d02 6a1c 640e 6410 6411 8d02  d.d...j.d.d.d...
-00001560: 7d17 7c17 6404 6412 8502 1900 6a1d 7d18  }.|.d.d.....j.}.
-00001570: 7c06 6a1e 7c06 6402 1900 a01f 7c18 a101  |.j.|.d.....|...
-00001580: 1900 7d19 7405 6a20 7c19 6402 6701 6413  ..}.t.j |.d.g.d.
-00001590: 6414 8400 7c19 6a21 6a22 a023 a100 4400  d...|.j!j".#..D.
-000015a0: 8301 6415 8d03 7d1a 7424 6a25 6416 6402  ..d...}.t$j%d.d.
-000015b0: 7c1a 7415 6a16 7c18 6417 8d05 0100 7c04  |.t.j.|.d.....|.
-000015c0: 7c17 a026 a100 6602 5300 2918 75f1 0000  |..&..f.S.).u...
-000015d0: 000a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-000015e0: 6d20 6466 3a0a 2020 2020 2020 2020 3a70  m df:.        :p
-000015f0: 6172 616d 206e 5f73 616d 706c 6573 3a20  aram n_samples: 
-00001600: d0ba d0be d0bb d0b8 d187 d0b5 d181 d182  ................
-00001610: d0b2 d0be 20d0 b7d0 b0d0 bfd0 b8d1 81d0  .... ...........
-00001620: b5d0 b920 d0ba d0be d182 d0be d180 d0be  ... ............
-00001630: d0b5 20d0 b1d1 83d0 b4d0 b5d1 8220 d181  .. .......... ..
-00001640: d0b5 d0bc d0bf d0bb d0b8 d180 d0be d0b2  ................
-00001650: d0b0 d182 d18c d181 d18f 20d0 b220 d0ba  .......... .. ..
-00001660: d0b0 d0b6 d0b4 d0be d0bc 20d1 82d0 b5d1  .......... .....
-00001670: 81d1 82d0 bed0 b2d0 bed0 bc20 d184 d0be  ........... ....
-00001680: d0bb d0b4 d0b5 20d0 b4d0 bbd1 8f20 d0b0  ...... ...... ..
-00001690: d0bd d0b0 d0bb d0b8 d0b7 d18b 2073 6861  ............ sha
-000016a0: 7020 7661 6c75 6573 0a20 2020 2020 2020  p values.       
-000016b0: 203a 7265 7475 726e 3a0a 2020 2020 2020   :return:.      
-000016c0: 2020 2901 da07 6669 6773 697a 65da 0766    )...figsize..f
-000016d0: 6561 7475 7265 a901 da07 636f 6c75 6d6e  eature....column
-000016e0: 734e 723c 0000 0072 3f00 0000 7240 0000  sNr<...r?...r@..
-000016f0: 0072 0100 0000 54a9 03da 016e 7221 0000  .r....T....nr!..
-00001700: 00da 0772 6570 6c61 6365 da05 7368 6170  ...replace..shap
-00001710: 5fda 056f 7574 6572 a902 da03 686f 77da  _..outer....how.
-00001720: 026f 6e72 6500 0000 7227 0000 0046 2901  .onre...r'...F).
-00001730: da09 6173 6365 6e64 696e 67e9 1e00 0000  ..ascending.....
-00001740: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001750: 0004 0000 0053 0000 0073 1800 0000 6700  .....S...s....g.
-00001760: 7c00 5d10 7d01 7c01 6400 7601 7204 7c01  |.].}.|.d.v.r.|.
-00001770: 9102 7104 5300 2901 2901 7287 0000 0072  ..q.S.).).r....r
-00001780: 2900 0000 2902 7248 0000 0072 8700 0000  )...).rH...r....
-00001790: 7229 0000 0072 2900 0000 722a 0000 0072  r)...r)...r*...r
-000017a0: 4a00 0000 f700 0000 7302 0000 0006 017a  J.......s......z
-000017b0: 2943 726f 7373 4d6f 6465 6c46 6162 7269  )CrossModelFabri
-000017c0: 632e 7368 6170 2e3c 6c6f 6361 6c73 3e2e  c.shap.<locals>.
-000017d0: 3c6c 6973 7463 6f6d 703e 2902 da07 6964  <listcomp>)...id
-000017e0: 5f76 6172 73da 0a76 616c 7565 5f76 6172  _vars..value_var
-000017f0: 73da 0576 616c 7565 2905 7249 0000 0072  s..value).rI...r
-00001800: 7c00 0000 722e 0000 00da 0965 7374 696d  |...r......estim
-00001810: 6174 6f72 da05 6f72 6465 7229 27da 0370  ator..order)'..p
-00001820: 6c74 da06 6669 6775 7265 7252 0000 0072  lt..figurerR...r
-00001830: 5300 0000 7254 0000 0072 4c00 0000 725f  S...rT...rL...r_
-00001840: 0000 0072 1b00 0000 7220 0000 0072 5700  ...r....r ...rW.
-00001850: 0000 720a 0000 0072 5800 0000 7222 0000  ..r....rX...r"..
-00001860: 0072 5900 0000 725a 0000 0072 2300 0000  .rY...rZ...r#...
-00001870: da04 7368 6170 da0d 5472 6565 4578 706c  ..shap..TreeExpl
-00001880: 6169 6e65 72da 0673 616d 706c 6572 8200  ainer..sampler..
-00001890: 0000 da03 7a69 7072 5c00 0000 7265 0000  ....zipr\...re..
-000018a0: 00da 0361 6273 da03 7374 72da 056d 6572  ...abs..str..mer
-000018b0: 6765 da09 7365 745f 696e 6465 78da 0361  ge..set_index..a
-000018c0: 6767 da0b 736f 7274 5f76 616c 7565 7372  gg..sort_valuesr
-000018d0: 7400 0000 7279 0000 00da 0469 7369 6eda  t...ry.....isin.
-000018e0: 046d 656c 7472 8900 0000 7266 0000 00da  .meltr....rf....
-000018f0: 0674 6f6c 6973 74da 0373 6e73 5a07 6261  .tolist..snsZ.ba
-00001900: 7270 6c6f 74da 0b72 6573 6574 5f69 6e64  rplot..reset_ind
-00001910: 6578 291b 7228 0000 0072 3b00 0000 da09  ex).r(...r;.....
-00001920: 6e5f 7361 6d70 6c65 7372 8600 0000 da03  n_samplesr......
-00001930: 6669 6772 6800 0000 da0b 7368 6170 5f64  figrh.....shap_d
-00001940: 665f 6669 6e72 4900 0000 727c 0000 0072  f_finrI...r|...r
-00001950: 3d00 0000 7239 0000 0072 6900 0000 726a  =...r9...ri...rj
-00001960: 0000 0072 6b00 0000 726c 0000 0072 6d00  ...rk...rl...rm.
-00001970: 0000 726e 0000 0072 6f00 0000 7270 0000  ..rn...ro...rp..
-00001980: 0072 8000 0000 7281 0000 0072 7f00 0000  .r....r....r....
-00001990: da07 7368 6170 5f64 665a 1273 6861 705f  ..shap_dfZ.shap_
-000019a0: 6665 6174 7572 655f 7374 6174 735a 0963  feature_statsZ.c
-000019b0: 6f6c 735f 6265 7374 5a0d 6265 7374 5f66  ols_bestZ.best_f
-000019c0: 6561 7475 7265 735a 1262 6573 745f 6665  eaturesZ.best_fe
-000019d0: 6174 7572 6573 5f6d 656c 7472 2900 0000  atures_meltr)...
-000019e0: 7229 0000 0072 2a00 0000 729b 0000 00cf  r)...r*...r.....
-000019f0: 0000 0073 5800 0000 0007 0c01 0a01 0e02  ...sX...........
-00001a00: 0a01 0a02 1c01 0a01 0601 06ff 0a02 1201  ................
-00001a10: 1202 1601 1602 0a01 0a01 0c01 06ff 0602  ................
-00001a20: 0c01 1001 0aff 0601 0eff 0602 0801 04ff  ................
-00001a30: 0803 0a01 08ff 0601 04ff 0602 0e02 1401  ................
-00001a40: 0401 0c01 0aff 04ff 0604 0a01 06ff 0602  ................
-00001a50: 7a15 4372 6f73 734d 6f64 656c 4661 6272  z.CrossModelFabr
-00001a60: 6963 2e73 6861 70a9 0172 3e00 0000 6303  ic.shap..r>...c.
-00001a70: 0000 0000 0000 0000 0000 000c 0000 0007  ................
-00001a80: 0000 0043 0000 0073 d400 0000 7400 a001  ...C...s....t...
-00001a90: a100 7d03 7402 a003 7404 a101 7d04 7405  ..}.t...t...}.t.
-00001aa0: 6a06 6401 6701 6402 8d01 7d05 7c00 6a07  j.d.g.d...}.|.j.
-00001ab0: 6400 7501 724a 7c00 6a07 6a08 7c01 6403  d.u.rJ|.j.j.|.d.
-00001ac0: 8d01 7d06 7405 6a09 7c01 7c06 6702 6404  ..}.t.j.|.|.g.d.
-00001ad0: 6405 8d02 7d01 7c00 6a0a 6406 1900 7d07  d...}.|.j.d...}.
-00001ae0: 740b a00c 7c07 a101 7d08 7c01 7c07 a00d  t...|...}.|.|...
-00001af0: a100 1900 6a0e 7c02 6406 6407 6408 8d03  ....j.|.d.d.d...
-00001b00: 7d09 7c00 a00f 7c08 7c09 a102 7d0a 7405  }.|...|.|...}.t.
-00001b10: 6a06 7410 7c07 a00d a100 7411 6a12 7411  j.t.|.....t.j.t.
-00001b20: a013 7c0a a101 6406 6405 8d02 8302 6401  ..|...d.d.....d.
-00001b30: 6409 6702 6402 8d02 7d0b 7405 6a14 7c05  d.g.d...}.t.j.|.
-00001b40: 7c0b 640a 6401 640b 8d04 7d05 740b 6a15  |.d.d.d...}.t.j.
-00001b50: 7c0a 7c09 640c 640d 8d03 0100 7c03 5300  |.|.d.d.....|.S.
-00001b60: 290e 4e72 8700 0000 7288 0000 0072 ae00  ).Nr....r....r..
-00001b70: 0000 723f 0000 0072 4000 0000 7201 0000  ..r?...r@...r...
-00001b80: 0054 728a 0000 0072 8d00 0000 728e 0000  .Tr....r....r...
-00001b90: 0072 8f00 0000 4629 01da 0473 686f 7729  .r....F)...show)
-00001ba0: 1672 9900 0000 729a 0000 0072 5200 0000  .r....r....rR...
-00001bb0: 7253 0000 0072 5400 0000 724c 0000 0072  rS...rT...rL...r
-00001bc0: 5f00 0000 7222 0000 0072 7a00 0000 725a  _...r"...rz...rZ
-00001bd0: 0000 0072 2300 0000 729b 0000 0072 9c00  ...r#...r....r..
-00001be0: 0000 721b 0000 0072 9d00 0000 7282 0000  ..r....r....r...
-00001bf0: 0072 9e00 0000 725c 0000 0072 6500 0000  .r....r\...re...
-00001c00: 729f 0000 0072 a100 0000 5a0c 7375 6d6d  r....r....Z.summ
-00001c10: 6172 795f 706c 6f74 290c 7228 0000 0072  ary_plot).r(...r
-00001c20: 3e00 0000 72aa 0000 0072 ab00 0000 7268  >...r....r....rh
-00001c30: 0000 0072 ac00 0000 726b 0000 0072 7000  ...r....rk...rp.
-00001c40: 0000 7280 0000 0072 8100 0000 727f 0000  ..r....r....r...
-00001c50: 0072 ad00 0000 7229 0000 0072 2900 0000  .r....r)...r)...
-00001c60: 722a 0000 00da 1173 6861 705f 7375 6d6d  r*.....shap_summ
-00001c70: 6172 795f 706c 6f74 fe00 0000 7328 0000  ary_plot....s(..
-00001c80: 0000 0108 010a 010e 010a 010e 0112 030a  ................
-00001c90: 010a 010c 0106 ff06 020c 0110 010a ff06  ................
-00001ca0: 0106 ff06 0212 0210 017a 2243 726f 7373  .........z"Cross
-00001cb0: 4d6f 6465 6c46 6162 7269 632e 7368 6170  ModelFabric.shap
-00001cc0: 5f73 756d 6d61 7279 5f70 6c6f 7429 0672  _summary_plot).r
-00001cd0: 0700 0000 7208 0000 0072 0900 0000 5472  ....r....r....Tr
-00001ce0: 0100 0000 4e29 0272 8300 0000 7284 0000  ....N).r....r...
-00001cf0: 0029 0172 8300 0000 2911 7254 0000 00da  .).r....).rT....
-00001d00: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00001d10: 7561 6c6e 616d 655f 5f72 0500 0000 722b  ualname__r....r+
-00001d20: 0000 0072 0300 0000 722d 0000 0072 3200  ...r....r-...r2.
-00001d30: 0000 7239 0000 0072 5600 0000 7259 0000  ..r9...rV...rY..
-00001d40: 0072 7a00 0000 7282 0000 0072 4c00 0000  .rz...r....rL...
-00001d50: 725f 0000 0072 9b00 0000 72b0 0000 0072  r_...r....r....r
-00001d60: 2900 0000 7229 0000 0072 2900 0000 722a  )...r)...r)...r*
-00001d70: 0000 0072 0600 0000 0c00 0000 732a 0000  ...r........s*..
-00001d80: 0008 0600 0100 0100 0100 0100 0100 f602  ................
-00001d90: 0102 ff0c 2702 010a 0302 010a 0302 010a  ....'...........
-00001da0: 0e08 5808 1708 0d08 0812 2f72 0600 0000  ..X......./r....
-00001db0: 2913 da03 6162 6372 0200 0000 7203 0000  )...abcr....r...
-00001dc0: 00da 0868 7970 6572 6f70 7472 0400 0000  ...hyperoptr....
-00001dd0: da05 6e75 6d70 7972 5c00 0000 7252 0000  ..numpyr\...rR..
-00001de0: 00da 0670 616e 6461 7372 4c00 0000 729b  ...pandasrL...r.
-00001df0: 0000 00da 116d 6174 706c 6f74 6c69 622e  .....matplotlib.
-00001e00: 7079 706c 6f74 da06 7079 706c 6f74 7299  pyplot..pyplotr.
-00001e10: 0000 005a 0773 6561 626f 726e 72a8 0000  ...Z.seabornr...
-00001e20: 00da 1563 726f 7373 7072 6564 6963 742e  ...crosspredict.
-00001e30: 6974 6572 6174 6f72 7205 0000 0072 0600  iteratorr....r..
-00001e40: 0000 7229 0000 0072 2900 0000 7229 0000  ..r)...r)...r)..
-00001e50: 0072 2a00 0000 da08 3c6d 6f64 756c 653e  .r*.....<module>
-00001e60: 0100 0000 7312 0000 0010 010c 0108 0108  ....s...........
-00001e70: 0108 0108 010c 0108 010c 03              ...........
+000008a0: 7c03 7c05 3c00 6e30 7c00 6a04 640e 1900  |.|.<.n0|.j.d...
+000008b0: 6410 7600 9001 72c0 6411 6412 8400 7c10  d.v...r.d.d...|.
+000008c0: 640a 1900 7c00 6a04 640e 1900 1900 4400  d...|.j.d.....D.
+000008d0: 8301 7c03 7c05 3c00 7417 a018 7c10 640a  ..|.|.<.t...|.d.
+000008e0: 1900 7c00 6a04 640e 1900 1900 a101 7d12  ..|.j.d.......}.
+000008f0: 7c04 a019 7c12 a101 0100 7c02 a003 6413  |...|.....|...d.
+00000900: 7c05 7c00 6a05 6a11 1600 9b00 6414 7c00  |.|.j.j.....d.|.
+00000910: 6a04 640e 1900 9b00 6415 7c12 9b00 9d06  j.d.....d.|.....
+00000920: a101 0100 713c 7c00 6a12 9002 72e2 740b  ....q<|.j...r.t.
+00000930: a01a 741b 6416 6412 8400 7c03 a01c a100  ..t.d.d...|.....
+00000940: 4400 8301 8301 a101 7c00 5f1d 7c00 6a1d  D.......|._.|.j.
+00000950: a01e a100 6a1f 6403 6404 8d01 6406 6b02  ....j.d.d...d.k.
+00000960: 7d13 7417 a020 7c00 6a1d 7c13 1900 6a21  }.t.. |.j.|...j!
+00000970: 6403 6404 8d01 6a22 a101 7c00 5f23 7c00  d.d...j"..|._#|.
+00000980: 6a1d 7c13 1900 6a21 6403 6404 8d01 7c00  j.|...j!d.d...|.
+00000990: 6a23 1900 7c00 5f24 7c00 6a24 7d14 7c00  j#..|._$|.j$}.|.
+000009a0: 6a04 640e 1900 640f 7600 9002 729e 7c00  j.d...d.v...r.|.
+000009b0: 6a24 0b00 7d14 7c00 6a1d 7c13 1900 6a25  j$..}.|.j.|...j%
+000009c0: 6403 6404 8d01 7c00 6a23 1900 7c00 5f25  d.d...|.j#..|._%
+000009d0: 7c14 7426 7c00 6a25 7c00 6a24 7c04 7427  |.t&|.j%|.j$|.t'
+000009e0: 7c00 6a23 8301 6417 9c06 7d15 7c02 a003  |.j#..d...}.|...
+000009f0: 7c15 a101 0100 7c15 5300 7c00 5300 2918  |.....|.S.|.S.).
+00000a00: 4ea9 01da 0264 66a9 03da 0466 6f6c 6472  N....df....foldr
+00000a10: 3900 0000 da04 7465 7374 e901 0000 00a9  9.....test......
+00000a20: 01da 0461 7869 7329 0372 2e00 0000 722f  ...axis).r....r/
+00000a30: 0000 0072 3000 0000 7201 0000 007a 0d52  ...r0...r....z.R
+00000a40: 4550 4541 5420 464f 4c44 5320 7a06 2053  EPEAT FOLDS z. S
+00000a50: 5441 5254 7239 0000 00da 0465 7661 6c46  TARTr9.....evalF
+00000a60: 290a 721a 0000 0072 3300 0000 7234 0000  ).r....r3...r4..
+00000a70: 00da 0976 616c 6964 5f73 6574 7236 0000  ...valid_setr6..
+00000a80: 0072 1d00 0000 7237 0000 0072 3000 0000  .r....r7...r0...
+00000a90: 721e 0000 0072 3800 0000 2905 721a 0000  r....r8...).r...
+00000aa0: 0072 3300 0000 721d 0000 0072 3000 0000  .r3...r....r0...
+00000ab0: 7238 0000 0072 0b00 0000 da03 6175 6329  r8...r......auc)
+00000ac0: 0e72 1800 0000 7219 0000 0072 1000 0000  .r....r....r....
+00000ad0: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+00000ae0: 0c00 0000 720d 0000 0072 0e00 0000 720f  ....r....r....r.
+00000af0: 0000 0072 1400 0000 7215 0000 0072 1600  ...r....r....r..
+00000b00: 0000 7217 0000 0063 0100 0000 0000 0000  ..r....c........
+00000b10: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
+00000b20: 7314 0000 0067 007c 005d 0c7d 0164 007c  s....g.|.].}.d.|
+00000b30: 0114 0091 0271 0453 0029 01e9 ffff ffff  .....q.S.)......
+00000b40: 7229 0000 0029 02da 022e 30da 0178 7229  r)...)....0..xr)
+00000b50: 0000 0072 2900 0000 722a 0000 00da 0a3c  ...r)...r*.....<
+00000b60: 6c69 7374 636f 6d70 3e85 0000 00f3 0000  listcomp>.......
+00000b70: 0000 7a28 4372 6f73 734d 6f64 656c 4661  ..z(CrossModelFa
+00000b80: 6272 6963 2e66 6974 2e3c 6c6f 6361 6c73  bric.fit.<locals
+00000b90: 3e2e 3c6c 6973 7463 6f6d 703e 7a16 0943  >.<listcomp>z..C
+00000ba0: 524f 5353 5641 4c49 4441 5449 4f4e 2046  ROSSVALIDATION F
+00000bb0: 4f4c 4420 7a11 2045 4e44 5320 7769 7468  OLD z. ENDS with
+00000bc0: 2062 6573 7420 607a 0460 203d 2063 0100   best `z.` = c..
+00000bd0: 0000 0000 0000 0000 0000 0300 0000 0600  ................
+00000be0: 0000 5300 0000 731e 0000 0067 007c 005d  ..S...s....g.|.]
+00000bf0: 165c 027d 017d 027c 0174 00a0 017c 02a1  .\.}.}.|.t...|..
+00000c00: 0166 0291 0271 0453 0072 2900 0000 2902  .f...q.S.r)...).
+00000c10: da02 7064 da06 5365 7269 6573 2903 7246  ..pd..Series).rF
+00000c20: 0000 00da 016b da01 7672 2900 0000 7229  .....k..vr)...r)
+00000c30: 0000 0072 2a00 0000 7248 0000 008f 0000  ...r*...rH......
+00000c40: 0072 4900 0000 2906 da04 6c6f 7373 da06  .rI...)...loss..
+00000c50: 7374 6174 7573 7227 0000 0072 2500 0000  statusr'...r%...
+00000c60: 5a0a 7363 6f72 6573 5f61 6c6c 5a09 6e75  Z.scores_allZ.nu
+00000c70: 6d5f 626f 6f73 7429 28da 076c 6f67 6769  m_boost)(..loggi
+00000c80: 6e67 da09 6765 744c 6f67 6765 72da 085f  ng..getLogger.._
+00000c90: 5f6e 616d 655f 5fda 0469 6e66 6f72 1a00  _name__..infor..
+00000ca0: 0000 720a 0000 00da 0366 6974 da09 656e  ..r......fit..en
+00000cb0: 756d 6572 6174 65da 0573 706c 6974 7222  umerate..splitr"
+00000cc0: 0000 00da 0974 7261 6e73 666f 726d 724a  .....transformrJ
+00000cd0: 0000 00da 0663 6f6e 6361 7472 1b00 0000  .....concatr....
+00000ce0: 7220 0000 0072 3200 0000 721c 0000 00da  r ...r2...r.....
+00000cf0: 086e 5f73 706c 6974 7372 1f00 0000 7239  .n_splitsr....r9
+00000d00: 0000 0072 1d00 0000 721e 0000 0072 2300  ...r....r....r#.
+00000d10: 0000 da02 6e70 da03 6d61 78da 0661 7070  ....np..max..app
+00000d20: 656e 64da 0944 6174 6146 7261 6d65 da04  end..DataFrame..
+00000d30: 6469 6374 da05 6974 656d 7372 2400 0000  dict..itemsr$...
+00000d40: da06 6973 6e75 6c6c da03 7375 6dda 0661  ..isnull..sum..a
+00000d50: 7267 6d61 78da 046d 6561 6eda 0676 616c  rgmax..mean..val
+00000d60: 7565 7372 2600 0000 7225 0000 0072 2700  uesr&...r%...r'.
+00000d70: 0000 7204 0000 00da 0369 6e74 2916 7228  ..r......int).r(
+00000d80: 0000 0072 3b00 0000 da03 6c6f 6772 2400  ...r;.....logr$.
+00000d90: 0000 5a0a 7363 6f72 6573 5f61 7667 723d  ..Z.scores_avgr=
+00000da0: 0000 0072 3900 0000 da03 7661 6cda 0d65  ...r9.....val..e
+00000db0: 6e63 6f64 6564 5f74 7261 696e da0c 656e  ncoded_train..en
+00000dc0: 636f 6465 645f 7465 7374 da07 585f 7472  coded_test..X_tr
+00000dd0: 6169 6eda 0558 5f76 616c da07 795f 7472  ain..X_val..y_tr
+00000de0: 6169 6eda 0579 5f76 616c 5a06 6474 7261  ain..y_valZ.dtra
+00000df0: 696e 5a06 6476 616c 6964 7237 0000 00da  inZ.dvalidr7....
+00000e00: 056d 6f64 656c 5a08 6265 7374 5f61 7563  .modelZ.best_auc
+00000e10: da04 6d61 736b 724e 0000 00da 0672 6573  ..maskrN.....res
+00000e20: 756c 7472 2900 0000 7229 0000 0072 2a00  ultr)...r)...r*.
+00000e30: 0000 7254 0000 004b 0000 0073 9800 0000  ..rT...K...s....
+00000e40: 0001 0a01 0401 0401 0c02 0e02 1e01 0a01  ................
+00000e50: 0601 06ff 0a02 1201 1202 1601 1602 0401  ................
+00000e60: 0201 0201 04fd 0604 0801 04ff 0603 1201  ................
+00000e70: 1a03 0401 0801 0401 0401 0201 0201 0201  ................
+00000e80: 0201 0401 0201 0401 0401 02f6 080c 0801  ................
+00000e90: 0201 0401 0401 02fc 0606 0a01 0602 1001  ................
+00000ea0: 1801 1004 2002 1801 0a02 0401 22ff 0603  .... ......."...
+00000eb0: 0801 0401 14ff 0602 1601 1c01 1a01 0601  ................
+00000ec0: 1001 0803 1a03 0201 0201 0401 0401 0201  ................
+00000ed0: 08fb 0607 0a01 0401 7a14 4372 6f73 734d  ........z.CrossM
+00000ee0: 6f64 656c 4661 6272 6963 2e66 6974 6302  odelFabric.fitc.
+00000ef0: 0000 0000 0000 0000 0000 000f 0000 0008  ................
+00000f00: 0000 0043 0000 0073 fc00 0000 7c01 7c00  ...C...s....|.|.
+00000f10: 6a00 1900 7d02 7c01 7c00 6a01 1900 7d03  j...}.|.|.j...}.
+00000f20: 7402 6a03 7c01 6a04 7405 a006 7c01 6a07  t.j.|.j.t...|.j.
+00000f30: 6401 1900 a101 6402 8d02 7d04 7408 7c00  d.....d...}.t.|.
+00000f40: 6a09 a00a 7c01 a101 8301 4400 5db6 5c02  j...|.....D.].\.
+00000f50: 7d05 5c02 7d06 7d07 7c00 6a0b 6400 7501  }.\.}.}.|.j.d.u.
+00000f60: 7290 7c00 6a0b 6a0c 7c05 7c06 7c07 6403  r.|.j.j.|.|.|.d.
+00000f70: 8d03 5c02 7d08 7d09 7402 6a0d 7c06 7c08  ..\.}.}.t.j.|.|.
+00000f80: 6702 6404 6405 8d02 7d06 7402 6a0d 7c07  g.d.d...}.t.j.|.
+00000f90: 7c09 6702 6404 6405 8d02 7d07 7c06 7c00  |.g.d.d...}.|.|.
+00000fa0: 6a00 1900 7c07 7c00 6a00 1900 0200 7d0a  j...|.|.j.....}.
+00000fb0: 7d0b 7c06 7c00 6a01 1900 7c07 7c00 6a01  }.|.|.j...|.|.j.
+00000fc0: 1900 0200 7d0c 7d0d 7c00 6a0e 7c05 1900  ....}.}.|.j.|...
+00000fd0: 7d0e 7c04 6a0f 7c0b 6a04 0500 1900 7c0e  }.|.j.|.j.....|.
+00000fe0: 6a10 7c0b 7c0e a000 a100 1900 7c00 6a11  j.|.|.......|.j.
+00000ff0: 6406 8d02 7c00 6a09 6a12 1b00 3700 0300  d...|.j.j...7...
+00001000: 3c00 7140 7c04 5300 2907 4e72 0100 0000  <.q@|.S.).Nr....
+00001010: a902 da05 696e 6465 7872 2e00 0000 723c  ....indexr....r<
+00001020: 0000 0072 3f00 0000 7240 0000 00a9 01da  ...r?...r@......
+00001030: 0d6e 756d 5f69 7465 7261 7469 6f6e 2913  .num_iteration).
+00001040: 721b 0000 0072 2000 0000 724a 0000 0072  r....r ...rJ...r
+00001050: 4b00 0000 7272 0000 0072 5a00 0000 da05  K...rr...rZ.....
+00001060: 7a65 726f 73da 0573 6861 7065 7255 0000  zeros..shaperU..
+00001070: 0072 0a00 0000 7256 0000 0072 2200 0000  .r....rV...r"...
+00001080: 7257 0000 0072 5800 0000 7223 0000 00da  rW...rX...r#....
+00001090: 036c 6f63 da07 7072 6564 6963 7472 2600  .loc..predictr&.
+000010a0: 0000 da09 6e5f 7265 7065 6174 7329 0f72  ....n_repeats).r
+000010b0: 2800 0000 723b 0000 0072 4700 0000 da01  (...r;...rG.....
+000010c0: 7972 7800 0000 723d 0000 0072 3900 0000  yrx...r=...r9...
+000010d0: 7267 0000 0072 6800 0000 7269 0000 0072  rg...rh...ri...r
+000010e0: 6a00 0000 726b 0000 0072 6c00 0000 726d  j...rk...rl...rm
+000010f0: 0000 0072 6e00 0000 7229 0000 0072 2900  ...rn...r)...r).
+00001100: 0000 722a 0000 0072 5700 0000 a600 0000  ..r*...rW.......
+00001110: 732a 0000 0000 010a 010a 011c 021c 010a  s*..............
+00001120: 0106 0106 ff0a 0212 0112 0216 0116 030a  ................
+00001130: 010c 010e 0104 ff04 0106 ff02 ff08 037a  ...............z
+00001140: 1a43 726f 7373 4d6f 6465 6c46 6162 7269  .CrossModelFabri
+00001150: 632e 7472 616e 7366 6f72 6d63 0200 0000  c.transformc....
+00001160: 0000 0000 0000 0000 0700 0000 0600 0000  ................
+00001170: 4300 0000 7390 0000 0074 006a 017c 016a  C...s....t.j.|.j
+00001180: 0274 03a0 047c 016a 0564 0119 00a1 0164  .t...|.j.d.....d
+00001190: 028d 027d 0274 067c 006a 07a0 08a1 0083  ...}.t.|.j......
+000011a0: 017d 037c 006a 0964 0075 0172 527c 006a  .}.|.j.d.u.rR|.j
+000011b0: 09a0 0a7c 01a1 017d 0474 006a 0b7c 017c  ...|...}.t.j.|.|
+000011c0: 0467 0264 0364 048d 027d 017c 006a 07a0  .g.d.d...}.|.j..
+000011d0: 08a1 0044 005d 2e7d 057c 006a 077c 0519  ...D.].}.|.j.|..
+000011e0: 007d 067c 027c 066a 0a7c 017c 06a0 0ca1  .}.|.|.j.|.|....
+000011f0: 0019 007c 006a 0d64 058d 027c 031b 0037  ...|.j.d...|...7
+00001200: 007d 0271 5c7c 0253 0029 064e 7201 0000  .}.q\|.S.).Nr...
+00001210: 0072 7100 0000 723f 0000 0072 4000 0000  .rq...r?...r@...
+00001220: 7273 0000 0029 0e72 4a00 0000 724b 0000  rs...).rJ...rK..
+00001230: 0072 7200 0000 725a 0000 0072 7500 0000  .rr...rZ...ru...
+00001240: 7276 0000 00da 036c 656e 7223 0000 00da  rv.....lenr#....
+00001250: 046b 6579 7372 2200 0000 7278 0000 0072  .keysr"...rx...r
+00001260: 5800 0000 721b 0000 0072 2600 0000 2907  X...r....r&...).
+00001270: 7228 0000 0072 3e00 0000 7278 0000 005a  r(...r>...rx...Z
+00001280: 0a6d 6f64 656c 735f 6c65 6e72 6900 0000  .models_lenri...
+00001290: 723d 0000 0072 6e00 0000 7229 0000 0072  r=...rn...r)...r
+000012a0: 2900 0000 722a 0000 0072 7800 0000 bc00  )...r*...rx.....
+000012b0: 0000 7312 0000 0000 011c 010e 010a 010c  ..s.............
+000012c0: 0112 020e 010a 0122 027a 1843 726f 7373  .......".z.Cross
+000012d0: 4d6f 6465 6c46 6162 7269 632e 7072 6564  ModelFabric.pred
+000012e0: 6963 7463 0300 0000 0000 0000 0000 0000  ictc............
+000012f0: 0300 0000 0300 0000 4300 0000 7338 0000  ........C...s8..
+00001300: 007c 006a 0064 0119 0064 0276 0072 1c7c  .|.j.d...d.v.r.|
+00001310: 01a0 017c 02a1 0164 0319 0053 007c 006a  ...|...d...S.|.j
+00001320: 0064 0119 0064 0476 0072 347c 01a0 017c  .d...d.v.r4|...|
+00001330: 02a1 0153 0064 0053 0029 054e 720b 0000  ...S.d.S.).Nr...
+00001340: 0029 0372 4400 0000 7218 0000 0072 1900  .).rD...r....r..
+00001350: 0000 723f 0000 0029 0c72 1000 0000 7211  ..r?...).r....r.
+00001360: 0000 0072 1200 0000 7213 0000 0072 0c00  ...r....r....r..
+00001370: 0000 720d 0000 0072 0e00 0000 720f 0000  ..r....r....r...
+00001380: 0072 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
+00001390: 7217 0000 0029 0272 1a00 0000 da0b 7368  r....).r......sh
+000013a0: 6170 5f76 616c 7565 7329 0372 2800 0000  ap_values).r(...
+000013b0: da09 6578 706c 6169 6e65 72da 0964 665f  ..explainer..df_
+000013c0: 7361 6d70 6c65 7229 0000 0072 2900 0000  sampler)...r)...
+000013d0: 722a 0000 00da 105f 6765 745f 7368 6170  r*....._get_shap
+000013e0: 5f76 616c 7565 73c9 0000 0073 0800 0000  _values....s....
+000013f0: 0001 0e01 0e01 0e03 7a21 4372 6f73 734d  ........z!CrossM
+00001400: 6f64 656c 4661 6272 6963 2e5f 6765 745f  odelFabric._get_
+00001410: 7368 6170 5f76 616c 7565 73e9 f401 0000  shap_values.....
+00001420: a902 e90a 0000 0072 8300 0000 723a 0000  .......r....r:..
+00001430: 0063 0400 0000 0000 0000 0000 0000 1b00  .c..............
+00001440: 0000 0800 0000 4300 0000 73ce 0100 0074  ......C...s....t
+00001450: 006a 017c 0364 018d 017d 0474 02a0 0374  .j.|.d...}.t...t
+00001460: 04a1 017d 0574 056a 0664 0267 0164 038d  ...}.t.j.d.g.d..
+00001470: 017d 067c 017c 006a 0719 007d 077c 017c  .}.|.|.j...}.|.|
+00001480: 006a 0819 007d 0874 097c 006a 0aa0 0b7c  .j...}.t.|.j...|
+00001490: 01a1 0183 0144 005d fa5c 027d 095c 027d  .....D.].\.}.\.}
+000014a0: 0a7d 0b7c 006a 0c64 0475 0172 987c 006a  .}.|.j.d.u.r.|.j
+000014b0: 0c6a 0d7c 097c 0a7c 0b64 058d 035c 027d  .j.|.|.|.d...\.}
+000014c0: 0c7d 0d74 056a 0e7c 0a7c 0c67 0264 0664  .}.t.j.|.|.g.d.d
+000014d0: 078d 027d 0a74 056a 0e7c 0b7c 0d67 0264  ...}.t.j.|.|.g.d
+000014e0: 0664 078d 027d 0b7c 0a7c 006a 0719 007c  .d...}.|.|.j...|
+000014f0: 0b7c 006a 0719 0002 007d 0e7d 0f7c 0a7c  .|.j.....}.}.|.|
+00001500: 006a 0819 007c 0b7c 006a 0819 0002 007d  .j...|.|.j.....}
+00001510: 107d 117c 006a 0f7c 0919 007d 1274 10a0  .}.|.j.|...}.t..
+00001520: 117c 12a1 017d 137c 0f7c 12a0 07a1 0019  .|...}.|.|......
+00001530: 006a 127c 0264 0864 0964 0a8d 037d 147c  .j.|.d.d.d...}.|
+00001540: 00a0 137c 137c 14a1 027d 1574 056a 0674  ...|.|...}.t.j.t
+00001550: 147c 12a0 07a1 0074 156a 1674 15a0 177c  .|.....t.j.t...|
+00001560: 15a1 0164 0864 078d 0283 0264 0264 0b74  ...d.d.....d.d.t
+00001570: 187c 0983 0117 0067 0264 038d 027d 1674  .|.....g.d...}.t
+00001580: 056a 197c 067c 1664 0c64 0264 0d8d 047d  .j.|.|.d.d.d...}
+00001590: 0671 487c 06a0 1a64 02a1 016a 1b64 0e64  .qH|...d...j.d.d
+000015a0: 0f67 0264 0664 078d 026a 1c64 0e64 1064  .g.d.d...j.d.d.d
+000015b0: 118d 027d 177c 1764 0464 1285 0219 006a  ...}.|.d.d.....j
+000015c0: 1d7d 187c 066a 1e7c 0664 0219 00a0 1f7c  .}.|.j.|.d.....|
+000015d0: 18a1 0119 007d 1974 056a 207c 1964 0267  .....}.t.j |.d.g
+000015e0: 0164 1364 1484 007c 196a 216a 22a0 23a1  .d.d...|.j!j".#.
+000015f0: 0044 0083 0164 158d 037d 1a74 246a 2564  .D...d...}.t$j%d
+00001600: 1664 027c 1a74 156a 167c 1864 178d 0501  .d.|.t.j.|.d....
+00001610: 007c 047c 17a0 26a1 0066 0253 0029 1875  .|.|..&..f.S.).u
+00001620: f100 0000 0a0a 2020 2020 2020 2020 3a70  ......        :p
+00001630: 6172 616d 2064 663a 0a20 2020 2020 2020  aram df:.       
+00001640: 203a 7061 7261 6d20 6e5f 7361 6d70 6c65   :param n_sample
+00001650: 733a 20d0 bad0 bed0 bbd0 b8d1 87d0 b5d1  s: .............
+00001660: 81d1 82d0 b2d0 be20 d0b7 d0b0 d0bf d0b8  ....... ........
+00001670: d181 d0b5 d0b9 20d0 bad0 bed1 82d0 bed1  ...... .........
+00001680: 80d0 bed0 b520 d0b1 d183 d0b4 d0b5 d182  ..... ..........
+00001690: 20d1 81d0 b5d0 bcd0 bfd0 bbd0 b8d1 80d0   ...............
+000016a0: bed0 b2d0 b0d1 82d1 8cd1 81d1 8f20 d0b2  ............. ..
+000016b0: 20d0 bad0 b0d0 b6d0 b4d0 bed0 bc20 d182   ............ ..
+000016c0: d0b5 d181 d182 d0be d0b2 d0be d0bc 20d1  .............. .
+000016d0: 84d0 bed0 bbd0 b4d0 b520 d0b4 d0bb d18f  ......... ......
+000016e0: 20d0 b0d0 bdd0 b0d0 bbd0 b8d0 b7d1 8b20   .............. 
+000016f0: 7368 6170 2076 616c 7565 730a 2020 2020  shap values.    
+00001700: 2020 2020 3a72 6574 7572 6e3a 0a20 2020      :return:.   
+00001710: 2020 2020 2029 01da 0766 6967 7369 7a65       )...figsize
+00001720: da07 6665 6174 7572 65a9 01da 0763 6f6c  ..feature....col
+00001730: 756d 6e73 4e72 3c00 0000 723f 0000 0072  umnsNr<...r?...r
+00001740: 4000 0000 7201 0000 0054 a903 da01 6e72  @...r....T....nr
+00001750: 2100 0000 da07 7265 706c 6163 65da 0573  !.....replace..s
+00001760: 6861 705f da05 6f75 7465 72a9 02da 0368  hap_..outer....h
+00001770: 6f77 da02 6f6e 7263 0000 0072 2700 0000  ow..onrc...r'...
+00001780: 4629 01da 0961 7363 656e 6469 6e67 e91e  F)...ascending..
+00001790: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+000017a0: 0200 0000 0400 0000 5300 0000 7318 0000  ........S...s...
+000017b0: 0067 007c 005d 107d 017c 0164 0076 0172  .g.|.].}.|.d.v.r
+000017c0: 047c 0191 0271 0453 0029 0129 0172 8500  .|...q.S.).).r..
+000017d0: 0000 7229 0000 0029 0272 4600 0000 7285  ..r)...).rF...r.
+000017e0: 0000 0072 2900 0000 7229 0000 0072 2a00  ...r)...r)...r*.
+000017f0: 0000 7248 0000 00f9 0000 0073 0200 0000  ..rH.......s....
+00001800: 0601 7a29 4372 6f73 734d 6f64 656c 4661  ..z)CrossModelFa
+00001810: 6272 6963 2e73 6861 702e 3c6c 6f63 616c  bric.shap.<local
+00001820: 733e 2e3c 6c69 7374 636f 6d70 3e29 02da  s>.<listcomp>)..
+00001830: 0769 645f 7661 7273 da0a 7661 6c75 655f  .id_vars..value_
+00001840: 7661 7273 da05 7661 6c75 6529 0572 4700  vars..value).rG.
+00001850: 0000 727a 0000 0072 2e00 0000 da09 6573  ..rz...r......es
+00001860: 7469 6d61 746f 72da 056f 7264 6572 2927  timator..order)'
+00001870: da03 706c 74da 0666 6967 7572 6572 5000  ..plt..figurerP.
+00001880: 0000 7251 0000 0072 5200 0000 724a 0000  ..rQ...rR...rJ..
+00001890: 0072 5d00 0000 721b 0000 0072 2000 0000  .r]...r....r ...
+000018a0: 7255 0000 0072 0a00 0000 7256 0000 0072  rU...r....rV...r
+000018b0: 2200 0000 7257 0000 0072 5800 0000 7223  "...rW...rX...r#
+000018c0: 0000 00da 0473 6861 70da 0d54 7265 6545  .....shap..TreeE
+000018d0: 7870 6c61 696e 6572 da06 7361 6d70 6c65  xplainer..sample
+000018e0: 7280 0000 00da 037a 6970 725a 0000 0072  r......ziprZ...r
+000018f0: 6300 0000 da03 6162 73da 0373 7472 da05  c.....abs..str..
+00001900: 6d65 7267 65da 0973 6574 5f69 6e64 6578  merge..set_index
+00001910: da03 6167 67da 0b73 6f72 745f 7661 6c75  ..agg..sort_valu
+00001920: 6573 7272 0000 0072 7700 0000 da04 6973  esrr...rw.....is
+00001930: 696e da04 6d65 6c74 7287 0000 0072 6400  in..meltr....rd.
+00001940: 0000 da06 746f 6c69 7374 da03 736e 735a  ....tolist..snsZ
+00001950: 0762 6172 706c 6f74 da0b 7265 7365 745f  .barplot..reset_
+00001960: 696e 6465 7829 1b72 2800 0000 723b 0000  index).r(...r;..
+00001970: 00da 096e 5f73 616d 706c 6573 7284 0000  ...n_samplesr...
+00001980: 00da 0366 6967 7266 0000 00da 0b73 6861  ...figrf.....sha
+00001990: 705f 6466 5f66 696e 7247 0000 0072 7a00  p_df_finrG...rz.
+000019a0: 0000 723d 0000 0072 3900 0000 7267 0000  ..r=...r9...rg..
+000019b0: 0072 6800 0000 7269 0000 0072 6a00 0000  .rh...ri...rj...
+000019c0: 726b 0000 0072 6c00 0000 726d 0000 0072  rk...rl...rm...r
+000019d0: 6e00 0000 727e 0000 0072 7f00 0000 727d  n...r~...r....r}
+000019e0: 0000 00da 0773 6861 705f 6466 5a12 7368  .....shap_dfZ.sh
+000019f0: 6170 5f66 6561 7475 7265 5f73 7461 7473  ap_feature_stats
+00001a00: 5a09 636f 6c73 5f62 6573 745a 0d62 6573  Z.cols_bestZ.bes
+00001a10: 745f 6665 6174 7572 6573 5a12 6265 7374  t_featuresZ.best
+00001a20: 5f66 6561 7475 7265 735f 6d65 6c74 7229  _features_meltr)
+00001a30: 0000 0072 2900 0000 722a 0000 0072 9900  ...r)...r*...r..
+00001a40: 0000 d100 0000 7358 0000 0000 070c 010a  ......sX........
+00001a50: 010e 020a 010a 021c 010a 0106 0106 ff0a  ................
+00001a60: 0212 0112 0216 0116 020a 010a 010c 0106  ................
+00001a70: ff06 020c 0110 010a ff06 010e ff06 0208  ................
+00001a80: 0104 ff08 030a 0108 ff06 0104 ff06 020e  ................
+00001a90: 0214 0104 010c 010a ff04 ff06 040a 0106  ................
+00001aa0: ff06 027a 1543 726f 7373 4d6f 6465 6c46  ...z.CrossModelF
+00001ab0: 6162 7269 632e 7368 6170 a901 723e 0000  abric.shap..r>..
+00001ac0: 0063 0300 0000 0000 0000 0000 0000 0c00  .c..............
+00001ad0: 0000 0700 0000 4300 0000 73d4 0000 0074  ......C...s....t
+00001ae0: 00a0 01a1 007d 0374 02a0 0374 04a1 017d  .....}.t...t...}
+00001af0: 0474 056a 0664 0167 0164 028d 017d 057c  .t.j.d.g.d...}.|
+00001b00: 006a 0764 0075 0172 4a7c 006a 076a 087c  .j.d.u.rJ|.j.j.|
+00001b10: 0164 038d 017d 0674 056a 097c 017c 0667  .d...}.t.j.|.|.g
+00001b20: 0264 0464 058d 027d 017c 006a 0a64 0619  .d.d...}.|.j.d..
+00001b30: 007d 0774 0ba0 0c7c 07a1 017d 087c 017c  .}.t...|...}.|.|
+00001b40: 07a0 0da1 0019 006a 0e7c 0264 0664 0764  .......j.|.d.d.d
+00001b50: 088d 037d 097c 00a0 0f7c 087c 09a1 027d  ...}.|...|.|...}
+00001b60: 0a74 056a 0674 107c 07a0 0da1 0074 116a  .t.j.t.|.....t.j
+00001b70: 1274 11a0 137c 0aa1 0164 0664 058d 0283  .t...|...d.d....
+00001b80: 0264 0164 0967 0264 028d 027d 0b74 056a  .d.d.g.d...}.t.j
+00001b90: 147c 057c 0b64 0a64 0164 0b8d 047d 0574  .|.|.d.d.d...}.t
+00001ba0: 0b6a 157c 0a7c 0964 0c64 0d8d 0301 007c  .j.|.|.d.d.....|
+00001bb0: 0353 0029 0e4e 7285 0000 0072 8600 0000  .S.).Nr....r....
+00001bc0: 72ac 0000 0072 3f00 0000 7240 0000 0072  r....r?...r@...r
+00001bd0: 0100 0000 5472 8800 0000 728b 0000 0072  ....Tr....r....r
+00001be0: 8c00 0000 728d 0000 0046 2901 da04 7368  ....r....F)...sh
+00001bf0: 6f77 2916 7297 0000 0072 9800 0000 7250  ow).r....r....rP
+00001c00: 0000 0072 5100 0000 7252 0000 0072 4a00  ...rQ...rR...rJ.
+00001c10: 0000 725d 0000 0072 2200 0000 7278 0000  ..r]...r"...rx..
+00001c20: 0072 5800 0000 7223 0000 0072 9900 0000  .rX...r#...r....
+00001c30: 729a 0000 0072 1b00 0000 729b 0000 0072  r....r....r....r
+00001c40: 8000 0000 729c 0000 0072 5a00 0000 7263  ....r....rZ...rc
+00001c50: 0000 0072 9d00 0000 729f 0000 005a 0c73  ...r....r....Z.s
+00001c60: 756d 6d61 7279 5f70 6c6f 7429 0c72 2800  ummary_plot).r(.
+00001c70: 0000 723e 0000 0072 a800 0000 72a9 0000  ..r>...r....r...
+00001c80: 0072 6600 0000 72aa 0000 0072 6900 0000  .rf...r....ri...
+00001c90: 726e 0000 0072 7e00 0000 727f 0000 0072  rn...r~...r....r
+00001ca0: 7d00 0000 72ab 0000 0072 2900 0000 7229  }...r....r)...r)
+00001cb0: 0000 0072 2a00 0000 da11 7368 6170 5f73  ...r*.....shap_s
+00001cc0: 756d 6d61 7279 5f70 6c6f 7400 0100 0073  ummary_plot....s
+00001cd0: 2800 0000 0001 0801 0a01 0e01 0a01 0e01  (...............
+00001ce0: 1203 0a01 0a01 0c01 06ff 0602 0c01 1001  ................
+00001cf0: 0aff 0601 06ff 0602 1202 1001 7a22 4372  ............z"Cr
+00001d00: 6f73 734d 6f64 656c 4661 6272 6963 2e73  ossModelFabric.s
+00001d10: 6861 705f 7375 6d6d 6172 795f 706c 6f74  hap_summary_plot
+00001d20: 2906 7207 0000 0072 0800 0000 7209 0000  ).r....r....r...
+00001d30: 0054 7201 0000 004e 2902 7281 0000 0072  .Tr....N).r....r
+00001d40: 8200 0000 2901 7281 0000 0029 1172 5200  ....).r....).rR.
+00001d50: 0000 da0a 5f5f 6d6f 6475 6c65 5f5f da0c  ....__module__..
+00001d60: 5f5f 7175 616c 6e61 6d65 5f5f 7205 0000  __qualname__r...
+00001d70: 0072 2b00 0000 7203 0000 0072 2d00 0000  .r+...r....r-...
+00001d80: 7232 0000 0072 3900 0000 7254 0000 0072  r2...r9...rT...r
+00001d90: 5700 0000 7278 0000 0072 8000 0000 724a  W...rx...r....rJ
+00001da0: 0000 0072 5d00 0000 7299 0000 0072 ae00  ...r]...r....r..
+00001db0: 0000 7229 0000 0072 2900 0000 7229 0000  ..r)...r)...r)..
+00001dc0: 0072 2a00 0000 7206 0000 000c 0000 0073  .r*...r........s
+00001dd0: 2a00 0000 0806 0001 0001 0001 0001 0001  *...............
+00001de0: 00f6 0201 02ff 0c27 0201 0a03 0201 0a03  .......'........
+00001df0: 0201 0a0e 085b 0816 080d 0808 122f 7206  .....[......./r.
+00001e00: 0000 0029 13da 0361 6263 7202 0000 0072  ...)...abcr....r
+00001e10: 0300 0000 da08 6879 7065 726f 7074 7204  ......hyperoptr.
+00001e20: 0000 00da 056e 756d 7079 725a 0000 0072  .....numpyrZ...r
+00001e30: 5000 0000 da06 7061 6e64 6173 724a 0000  P.....pandasrJ..
+00001e40: 0072 9900 0000 da11 6d61 7470 6c6f 746c  .r......matplotl
+00001e50: 6962 2e70 7970 6c6f 74da 0670 7970 6c6f  ib.pyplot..pyplo
+00001e60: 7472 9700 0000 5a07 7365 6162 6f72 6e72  tr....Z.seabornr
+00001e70: a600 0000 da15 6372 6f73 7370 7265 6469  ......crosspredi
+00001e80: 6374 2e69 7465 7261 746f 7272 0500 0000  ct.iteratorr....
+00001e90: 7206 0000 0072 2900 0000 7229 0000 0072  r....r)...r)...r
+00001ea0: 2900 0000 722a 0000 00da 083c 6d6f 6475  )...r*.....<modu
+00001eb0: 6c65 3e01 0000 0073 1200 0000 1001 0c01  le>....s........
+00001ec0: 0801 0801 0801 0801 0c01 0801 0c03       ..............
```

### Comparing `crosspredict-1.1.7/crosspredict/crossval/__pycache__/_lightgbm.cpython-39.pyc` & `crosspredict-1.1.8/crosspredict/crossval/__pycache__/_lightgbm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/crosspredict/crossval/__pycache__/_xgboost.cpython-39.pyc` & `crosspredict-1.1.8/crosspredict/crossval/__pycache__/_xgboost.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/crosspredict/crossval/_catboost.py` & `crosspredict-1.1.8/crosspredict/crossval/_catboost.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/crosspredict/crossval/_crossval.py` & `crosspredict-1.1.8/crosspredict/crossval/_crossval.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,35 +126,27 @@
                 # Построение прогнозов при разном виде взаимодействия
                 if self.params['metric'] in ('auc'):
                     scores[fold] = evals_result['eval'][self.params['metric']]
                 elif self.params['metric'] in (
                 'binary_logloss', 'binary', 'l1', 'mean_absolute_error', 'mae', 'regression_l1', 'l2',
                 'mean_squared_error', 'mse', 'regression_l2', 'regression', 'rmse',
                 'root_mean_squared_error', 'l2_root'):
-                    scores[fold] = [-1 * x for x in -1 * evals_result['eval'][self.params['metric']]]
+                    scores[fold] = [-1 * x for x in evals_result['eval'][self.params['metric']]]
 
                 best_auc = np.max(evals_result['eval'][self.params['metric']])
                 scores_avg.append(best_auc)
 
                 log.info(
                     f'\tCROSSVALIDATION FOLD {fold % self.iterator.n_splits} ENDS with best `{self.params["metric"]}` = {best_auc}')
 
         if self.valid:
             self.scores = pd.DataFrame(
                 dict([(k, pd.Series(v)) for k, v in scores.items()]))
             mask = self.scores.isnull().sum(axis=1) == 0
-            if self.params['metric'] in ('auc'):
-                self.num_boost_optimal = np.argmax(self.scores[mask].mean(axis=1).values)
-
-            elif self.params['metric'] in (
-                'binary_logloss', 'binary', 'l1', 'mean_absolute_error', 'mae', 'regression_l1', 'l2',
-                'mean_squared_error', 'mse', 'regression_l2', 'regression', 'rmse',
-                'root_mean_squared_error', 'l2_root'):
-                self.num_boost_optimal = np.argmin(self.scores[mask].mean(axis=1).values)
-
+            self.num_boost_optimal = np.argmax(self.scores[mask].mean(axis=1).values)
             self.score_max = self.scores[mask].mean(axis=1)[self.num_boost_optimal]
             loss = self.score_max
             if self.params['metric'] in ('auc'):
                 loss = -self.score_max
 
             # self.score_max = np.mean(scores_avg)
             self.std = self.scores[mask].std(axis=1)[self.num_boost_optimal]
@@ -187,15 +179,14 @@
             y_train, y_val = train[self.col_target], val[self.col_target]
 
             # Подготовка данных в нужном формате
             model = self.models[fold]
             predict.loc[X_val.index] += \
                 model.predict(X_val[model.feature_name()],
                               num_iteration=self.num_boost_optimal) / self.iterator.n_repeats
-
         return predict
 
     def predict(self, test):
         predict = pd.Series(index=test.index, data=np.zeros(test.shape[0]))
         models_len = len(self.models.keys())
         if self.cross_target_encoder is not None:
             encoded_test = self.cross_target_encoder.predict(test)
```

### Comparing `crosspredict-1.1.7/crosspredict/crossval/_lightgbm.py` & `crosspredict-1.1.8/crosspredict/crossval/_lightgbm.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/crosspredict/crossval/_xgboost.py` & `crosspredict-1.1.8/crosspredict/crossval/_xgboost.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/crosspredict/iterator.py` & `crosspredict-1.1.8/crosspredict/iterator.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/crosspredict/nodes/_nodes.py` & `crosspredict-1.1.8/crosspredict/nodes/_nodes.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/crosspredict/parameters.yml` & `crosspredict-1.1.8/crosspredict/parameters.yml`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/crosspredict/report_binary/__pycache__/_curves.cpython-39.pyc` & `crosspredict-1.1.8/crosspredict/report_binary/__pycache__/_curves.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Sep 26 07:29:13 2022 UTC, .py size: 7860 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 c954 3163 b41e 0000  a........T1c....
+00000000: 610d 0d0a 0000 0000 92ff 3764 d81e 0000  a.........7d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 0401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a05 0100 6400 6402 6c06  d.l.m.Z...d.d.l.
 00000050: 5a07 6400 6402 6c08 5a09 6400 6402 6c0a  Z.d.d.l.Z.d.d.l.
 00000060: 5a0b 6400 6402 6c0c 5a0c 6400 6403 6c0d  Z.d.d.l.Z.d.d.l.
 00000070: 6d0e 5a0e 0100 6400 6404 6c0d 6d0f 5a0f  m.Z...d.d.l.m.Z.
@@ -241,297 +241,298 @@
 00000f00: da05 636f 756e 74a9 0672 3000 0000 7246  ..count..r0...rF
 00000f10: 0000 0072 4700 0000 7240 0000 0072 3e00  ...rG...r@...r>.
 00000f20: 0000 724e 0000 0072 5400 0000 7217 0000  ..rN...rT...r...
 00000f30: 0072 1800 0000 7248 0000 0054 0000 0073  .r....rH...T...s
 00000f40: 0800 0000 0001 1201 0601 0601 7a15 4765  ............z.Ge
 00000f50: 6e47 494e 4943 7572 7665 2e5f 5f69 6e69  nGINICurve.__ini
 00000f60: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
-00000f70: 0200 0000 0500 0000 0300 0000 7356 0000  ............sV..
+00000f70: 0200 0000 0500 0000 0300 0000 7366 0000  ............sf..
 00000f80: 007c 01a0 0088 006a 01a1 01a0 02a1 0088  .|.....j........
 00000f90: 005f 037c 017c 0188 006a 0419 00a0 05a1  ._.|.|...j......
-00000fa0: 000f 0019 00a0 0088 006a 01a1 01a0 0687  .........j......
-00000fb0: 0066 0164 0164 0284 08a1 0188 005f 0788  .f.d.d......._..
-00000fc0: 006a 076a 0888 006a 036a 0964 038d 0188  .j.j...j.j.d....
-00000fd0: 005f 0788 0053 0029 044e 6301 0000 0000  ._...S.).Nc.....
-00000fe0: 0000 0000 0000 0001 0000 0006 0000 0013  ................
-00000ff0: 0000 0073 3c00 0000 7400 7c00 8800 6a01  ...s<...t.|...j.
-00001000: 1900 a002 a100 8301 6401 6b04 7238 6402  ........d.k.r8d.
-00001010: 6403 7403 7c00 8800 6a01 1900 7c00 8800  d.t.|...j...|...
-00001020: 6a04 1900 8302 1400 6401 1800 1400 5300  j.......d.....S.
-00001030: 6400 5300 2904 4ee9 0100 0000 e964 0000  d.S.).N......d..
-00001040: 00e9 0200 0000 2905 721e 0000 0072 4700  ......).r....rG.
-00001050: 0000 da06 756e 6971 7565 7207 0000 0072  ....uniquer....r
-00001060: 4600 0000 7216 0000 00a9 0172 3000 0000  F...r......r0...
-00001070: 7217 0000 0072 1800 0000 7219 0000 005d  r....r....r....]
-00001080: 0000 0073 0a00 0000 0201 0cff 0201 02ff  ...s............
-00001090: 2601 7a22 4765 6e47 494e 4943 7572 7665  &.z"GenGINICurve
-000010a0: 2e66 6974 2e3c 6c6f 6361 6c73 3e2e 3c6c  .fit.<locals>.<l
-000010b0: 616d 6264 613e 2901 721f 0000 0029 0ada  ambda>).r....)..
-000010c0: 0767 726f 7570 6279 7268 0000 00da 0473  .groupbyrh.....s
-000010d0: 697a 6572 6900 0000 7246 0000 0072 5a00  izeri...rF...rZ.
-000010e0: 0000 da05 6170 706c 7972 6700 0000 da07  ....applyrg.....
-000010f0: 7265 696e 6465 7872 1f00 0000 724a 0000  reindexr....rJ..
-00001100: 0072 1700 0000 726f 0000 0072 1800 0000  .r....ro...r....
-00001110: 724c 0000 005a 0000 0073 0c00 0000 0001  rL...Z...s......
-00001120: 1201 1c01 0aff 0603 1401 7a10 4765 6e47  ..........z.GenG
-00001130: 494e 4943 7572 7665 2e66 6974 6303 0000  INICurve.fitc...
-00001140: 0000 0000 0000 0000 0005 0000 0007 0000  ................
-00001150: 004b 0000 0073 5e00 0000 7c03 6401 1900  .K...s^...|.d...
-00001160: 7d04 7c01 7c00 5f00 7c04 7c00 5f01 7c00  }.|.|._.|.|._.|.
-00001170: 6a02 7c00 6a03 7c01 6402 6403 8d03 0100  j.|.j.|.d.d.....
-00001180: 7c00 6a04 7c00 6a05 6601 7c04 7c00 6a06  |.j.|.j.f.|.|.j.
-00001190: 6404 6405 6406 9c04 7c03 a401 8e01 0100  d.d.d...|.......
-000011a0: 7c02 725a 7c01 6a07 7c02 6407 6408 6409  |.rZ|.j.|.d.d.d.
-000011b0: 8d03 0100 7c00 5300 290a 4e72 3f00 0000  ....|.S.).Nr?...
-000011c0: 720c 0000 0072 3700 0000 5a04 4749 4e49  r....r7...Z.GINI
-000011d0: 5429 0472 1000 0000 723e 0000 0072 3200  T).r....r>...r2.
-000011e0: 0000 723d 0000 0072 5d00 0000 725e 0000  ..r=...r]...r^..
-000011f0: 0072 5f00 0000 2908 7210 0000 0072 3f00  .r_...).r....r?.
-00001200: 0000 7236 0000 0072 6900 0000 7241 0000  ..r6...ri...rA..
-00001210: 0072 6700 0000 723e 0000 0072 6300 0000  .rg...r>...rc...
-00001220: 2905 7230 0000 0072 1000 0000 724d 0000  ).r0...r....rM..
-00001230: 0072 4e00 0000 723f 0000 0072 1700 0000  .rN...r?...r....
-00001240: 7217 0000 0072 1800 0000 723b 0000 0062  r....r....r;...b
-00001250: 0000 0073 1000 0000 0001 0801 0601 0601  ...s............
-00001260: 1201 2001 0401 1001 7a11 4765 6e47 494e  .. .....z.GenGIN
-00001270: 4943 7572 7665 2e70 6c6f 7429 014e 2902  ICurve.plot).N).
-00001280: 4e4e 7264 0000 0072 1700 0000 7217 0000  NNrd...r....r...
-00001290: 0072 5400 0000 7218 0000 0072 6600 0000  .rT...r....rf...
-000012a0: 5300 0000 7306 0000 0008 010e 0608 0872  S...s..........r
-000012b0: 6600 0000 6300 0000 0000 0000 0000 0000  f...c...........
-000012c0: 0000 0000 0004 0000 0000 0000 0073 3000  .............s0.
-000012d0: 0000 6500 5a01 6400 5a02 6408 8700 6601  ..e.Z.d.Z.d...f.
-000012e0: 6402 6403 8409 5a03 6404 6405 8400 5a04  d.d...Z.d.d...Z.
-000012f0: 6409 6406 6407 8401 5a05 8700 0400 5a06  d.d.d...Z.....Z.
-00001300: 5300 290a da0c 4765 6e52 6973 6b43 7572  S.)...GenRiskCur
-00001310: 7665 4e63 0500 0000 0000 0000 0000 0000  veNc............
-00001320: 0600 0000 0500 0000 0b00 0000 7322 0000  ............s"..
-00001330: 0074 0083 006a 017c 017c 027c 0464 018d  .t...j.|.|.|.d..
-00001340: 0301 007c 037c 005f 0264 007c 005f 0364  ...|.|._.d.|._.d
-00001350: 0053 0072 5000 0000 2904 7251 0000 0072  .S.rP...).rQ...r
-00001360: 4800 0000 7268 0000 00da 0472 6973 6b72  H...rh.....riskr
-00001370: 6a00 0000 7254 0000 0072 1700 0000 7218  j...rT...r....r.
-00001380: 0000 0072 4800 0000 6e00 0000 7306 0000  ...rH...n...s...
-00001390: 0000 0112 0106 017a 1547 656e 5269 736b  .......z.GenRisk
-000013a0: 4375 7276 652e 5f5f 696e 6974 5f5f 6302  Curve.__init__c.
-000013b0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-000013c0: 0000 0043 0000 0073 2200 0000 7c01 a000  ...C...s"...|...
-000013d0: 7c00 6a01 a101 7c00 6a02 1900 a003 6401  |.j...|.j.....d.
-000013e0: 6402 6702 a101 7c00 5f04 7c00 5300 2903  d.g...|._.|.S.).
-000013f0: 4e72 6900 0000 da04 6d65 616e 2905 7270  Nri.....mean).rp
-00001400: 0000 0072 6800 0000 7247 0000 00da 0361  ...rh...rG.....a
-00001410: 6767 7275 0000 0072 4a00 0000 7217 0000  ggru...rJ...r...
-00001420: 0072 1700 0000 7218 0000 0072 4c00 0000  .r....r....rL...
-00001430: 7300 0000 7304 0000 0000 011e 017a 1047  s...s........z.G
-00001440: 656e 5269 736b 4375 7276 652e 6669 7463  enRiskCurve.fitc
-00001450: 0500 0000 0000 0000 0000 0000 0700 0000  ................
-00001460: 0700 0000 4b00 0000 7368 0000 007c 0564  ....K...sh...|.d
-00001470: 0119 007d 067c 017c 005f 007c 067c 005f  ...}.|.|._.|.|._
-00001480: 017c 0364 0075 0072 2064 027d 037c 006a  .|.d.u.r d.}.|.j
-00001490: 027c 006a 0364 0319 007c 0164 0464 058d  .|.j.d...|.d.d..
-000014a0: 0301 007c 006a 047c 006a 0364 0619 007c  ...|.j.|.j.d...|
-000014b0: 067c 037c 0464 0764 088d 0501 007c 0272  .|.|.d.d.....|.r
-000014c0: 647c 016a 057c 0264 0964 0a64 0b8d 0301  d|.j.|.d.d.d....
-000014d0: 007c 0053 0029 0c4e 723f 0000 00fa 0b4d  .|.S.).Nr?.....M
-000014e0: 6561 6e20 5461 7267 6574 7269 0000 0072  ean Targetri...r
-000014f0: 0c00 0000 7237 0000 0072 7600 0000 54a9  ....r7...rv...T.
-00001500: 0372 3200 0000 723e 0000 0072 3d00 0000  .r2...r>...r=...
-00001510: 725d 0000 0072 5e00 0000 725f 0000 0029  r]...r^...r_...)
-00001520: 0672 1000 0000 723f 0000 0072 3600 0000  .r....r?...r6...
-00001530: 7275 0000 0072 4100 0000 7263 0000 0029  ru...rA...rc...)
-00001540: 0772 3000 0000 7210 0000 0072 4d00 0000  .r0...r....rM...
-00001550: 7232 0000 0072 3e00 0000 724e 0000 0072  r2...r>...rN...r
-00001560: 3f00 0000 7217 0000 0072 1700 0000 7218  ?...r....r....r.
-00001570: 0000 0072 3b00 0000 7700 0000 7314 0000  ...r;...w...s...
-00001580: 0000 0108 0106 0106 0108 0104 0116 011a  ................
-00001590: 0104 0110 017a 1147 656e 5269 736b 4375  .....z.GenRiskCu
-000015a0: 7276 652e 706c 6f74 2901 4e29 044e 4e4e  rve.plot).N).NNN
-000015b0: 4e72 6400 0000 7217 0000 0072 1700 0000  Nrd...r....r....
-000015c0: 7254 0000 0072 1800 0000 7274 0000 006d  rT...r....rt...m
-000015d0: 0000 0073 0600 0000 0801 0e05 0804 7274  ...s..........rt
-000015e0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000015f0: 0000 0000 0500 0000 0000 0000 7330 0000  ............s0..
-00001600: 0065 005a 0164 005a 0264 0887 0066 0164  .e.Z.d.Z.d...f.d
-00001610: 0264 0384 095a 0364 0464 0584 005a 0464  .d...Z.d.d...Z.d
-00001620: 0964 0664 0784 015a 0587 0004 005a 0653  .d.d...Z.....Z.S
-00001630: 0029 0ada 0d4d 6561 6e50 726f 6243 7572  .)...MeanProbCur
-00001640: 7665 4e63 0400 0000 0000 0000 0000 0000  veNc............
-00001650: 0500 0000 0500 0000 0b00 0000 7328 0000  ............s(..
-00001660: 0074 0083 006a 017c 017c 027c 0364 018d  .t...j.|.|.|.d..
-00001670: 0301 0064 007c 005f 0264 007c 005f 0364  ...d.|._.d.|._.d
-00001680: 007c 005f 0464 0053 0072 5000 0000 2905  .|._.d.S.rP...).
-00001690: 7251 0000 0072 4800 0000 da0a 7064 5f64  rQ...rH.....pd_d
-000016a0: 6563 696c 6573 da07 7064 5f62 696e 73da  eciles..pd_bins.
-000016b0: 096d 6561 6e5f 7072 6f62 7253 0000 0072  .mean_probrS...r
-000016c0: 5400 0000 7217 0000 0072 1800 0000 7248  T...r....r....rH
-000016d0: 0000 0085 0000 0073 0800 0000 0001 1201  .......s........
-000016e0: 0601 0601 7a16 4d65 616e 5072 6f62 4375  ....z.MeanProbCu
-000016f0: 7276 652e 5f5f 696e 6974 5f5f 6302 0000  rve.__init__c...
-00001700: 0000 0000 0000 0000 0002 0000 0007 0000  ................
-00001710: 0043 0000 0073 4c00 0000 7400 6a01 7c01  .C...sL...t.j.|.
-00001720: 7c00 6a02 1900 7403 a004 6401 6402 6403  |.j...t...d.d.d.
-00001730: a103 6404 6405 6406 8d04 5c02 7c00 5f05  ..d.d.d...\.|._.
-00001740: 7c00 5f06 7c01 a007 7c00 6a05 a101 7c00  |._.|...|.j...|.
-00001750: 6a08 1900 a009 6407 6408 6702 a101 7c00  j.....d.d.g...|.
-00001760: 5f0a 7c00 5300 2909 4e72 0100 0000 670b  _.|.S.).Nr....g.
-00001770: 7a6f 0c01 00f0 3f67 9a99 9999 9999 b93f  zo....?g.......?
-00001780: da04 6472 6f70 5429 03da 0171 da0a 6475  ..dropT)...q..du
-00001790: 706c 6963 6174 6573 da07 7265 7462 696e  plicates..retbin
-000017a0: 7372 6900 0000 7276 0000 0029 0bda 0270  sri...rv...)...p
-000017b0: 64da 0471 6375 7472 4600 0000 7221 0000  d..qcutrF...r!..
-000017c0: 0072 2200 0000 727b 0000 0072 7c00 0000  .r"...r{...r|...
-000017d0: 7270 0000 0072 4700 0000 7277 0000 0072  rp...rG...rw...r
-000017e0: 7d00 0000 724a 0000 0072 1700 0000 7217  }...rJ...r....r.
-000017f0: 0000 0072 1800 0000 724c 0000 008b 0000  ...r....rL......
-00001800: 0073 1600 0000 0001 1001 06ff 0201 04ff  .s..............
-00001810: 0e02 0a01 04ff 0401 06ff 0602 7a11 4d65  ............z.Me
-00001820: 616e 5072 6f62 4375 7276 652e 6669 7463  anProbCurve.fitc
-00001830: 0600 0000 0000 0000 0000 0000 0700 0000  ................
-00001840: 0700 0000 4b00 0000 7360 0000 007c 017c  ....K...s`...|.|
-00001850: 005f 007c 027c 005f 017c 0464 0075 0072  ._.|.|._.|.d.u.r
-00001860: 1864 017d 047c 006a 027c 006a 0364 0219  .d.}.|.j.|.j.d..
-00001870: 007c 0164 0364 048d 0301 007c 006a 047c  .|.d.d.....|.j.|
-00001880: 006a 0364 0519 007c 027c 047c 0564 0664  .j.d...|.|.|.d.d
-00001890: 078d 0501 007c 0372 5c7c 016a 057c 0364  .....|.r\|.j.|.d
-000018a0: 0864 0964 0a8d 0301 007c 0053 0029 0b4e  .d.d.....|.S.).N
-000018b0: 7278 0000 0072 6900 0000 720c 0000 0072  rx...ri...r....r
-000018c0: 3700 0000 7276 0000 0054 7279 0000 0072  7...rv...Try...r
-000018d0: 5d00 0000 725e 0000 0072 5f00 0000 2906  ]...r^...r_...).
-000018e0: 7210 0000 0072 3f00 0000 7236 0000 0072  r....r?...r6...r
-000018f0: 7d00 0000 7241 0000 0072 6300 0000 2907  }...rA...rc...).
-00001900: 7230 0000 0072 1000 0000 723f 0000 0072  r0...r....r?...r
-00001910: 4d00 0000 7232 0000 0072 3e00 0000 724e  M...r2...r>...rN
-00001920: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
-00001930: 0000 723b 0000 0092 0000 0073 1200 0000  ..r;.......s....
-00001940: 0001 0601 0601 0801 0401 1601 1a01 0401  ................
-00001950: 1001 7a12 4d65 616e 5072 6f62 4375 7276  ..z.MeanProbCurv
-00001960: 652e 706c 6f74 2901 4e29 054e 4e4e 4e4e  e.plot).N).NNNNN
-00001970: 7264 0000 0072 1700 0000 7217 0000 0072  rd...r....r....r
-00001980: 5400 0000 7218 0000 0072 7a00 0000 8400  T...r....rz.....
-00001990: 0000 7306 0000 0008 010e 0608 0772 7a00  ..s..........rz.
-000019a0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000019b0: 0000 0004 0000 0000 0000 0073 3000 0000  ...........s0...
-000019c0: 6500 5a01 6400 5a02 6408 8700 6601 6402  e.Z.d.Z.d...f.d.
-000019d0: 6403 8409 5a03 6404 6405 8400 5a04 6409  d...Z.d.d...Z.d.
-000019e0: 6406 6407 8401 5a05 8700 0400 5a06 5300  d.d...Z.....Z.S.
-000019f0: 290a da0b 526f 6341 7563 4375 7276 654e  )...RocAucCurveN
-00001a00: 6304 0000 0000 0000 0000 0000 0005 0000  c...............
-00001a10: 0005 0000 000b 0000 0073 2800 0000 7400  .........s(...t.
-00001a20: 8300 6a01 7c01 7c02 7c03 6401 8d03 0100  ..j.|.|.|.d.....
-00001a30: 6400 7c00 5f02 6400 7c00 5f03 6400 7c00  d.|._.d.|._.d.|.
-00001a40: 5f04 6400 5300 7250 0000 0029 0572 5100  _.d.S.rP...).rQ.
-00001a50: 0000 7248 0000 00da 0366 7072 da03 7470  ..rH.....fpr..tp
-00001a60: 72da 0772 6f63 5f61 7563 7253 0000 0072  r..roc_aucrS...r
-00001a70: 5400 0000 7217 0000 0072 1800 0000 7248  T...r....r....rH
-00001a80: 0000 009f 0000 0073 0800 0000 0001 1201  .......s........
-00001a90: 0601 0601 7a14 526f 6341 7563 4375 7276  ....z.RocAucCurv
-00001aa0: 652e 5f5f 696e 6974 5f5f 6302 0000 0000  e.__init__c.....
-00001ab0: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
-00001ac0: 0000 0073 3400 0000 7400 7c01 7c00 6a01  ...s4...t.|.|.j.
-00001ad0: 1900 7c01 7c00 6a02 1900 8302 5c03 7c00  ..|.|.j.....\.|.
-00001ae0: 5f03 7c00 5f04 7d02 7405 7c00 6a03 7c00  _.|._.}.t.|.j.|.
-00001af0: 6a04 8302 7c00 5f06 7c00 5300 7249 0000  j...|._.|.S.rI..
-00001b00: 0029 0772 0400 0000 7247 0000 0072 4600  .).r....rG...rF.
-00001b10: 0000 7285 0000 0072 8600 0000 7206 0000  ..r....r....r...
-00001b20: 0072 8700 0000 a903 7230 0000 0072 4b00  .r......r0...rK.
-00001b30: 0000 da01 5f72 1700 0000 7217 0000 0072  ...._r....r....r
-00001b40: 1800 0000 724c 0000 00a5 0000 0073 0a00  ....rL.......s..
-00001b50: 0000 0001 0201 10ff 0e02 1001 7a0f 526f  ............z.Ro
-00001b60: 6341 7563 4375 7276 652e 6669 7463 0300  cAucCurve.fitc..
-00001b70: 0000 0000 0000 0000 0000 0500 0000 0600  ................
-00001b80: 0000 4b00 0000 736a 0000 007c 0164 0075  ..K...sj...|.d.u
-00001b90: 0072 1474 00a0 01a1 005c 027d 047d 017c  .r.t.....\.}.}.|
-00001ba0: 017c 005f 0274 037c 006a 047c 006a 057c  .|._.t.|.j.|.j.|
-00001bb0: 006a 0664 0114 007c 006a 0764 028d 047c  .j.d...|.j.d...|
-00001bc0: 005f 087c 0272 4c7c 016a 097c 0264 0364  ._.|.rL|.j.|.d.d
-00001bd0: 0464 058d 0301 007c 006a 086a 0a66 007c  .d.....|.j.j.f.|
-00001be0: 017c 006a 0764 069c 027c 03a4 018e 0101  .|.j.d...|......
-00001bf0: 007c 0053 0029 074e 726c 0000 0029 0472  .|.S.).Nrl...).r
-00001c00: 8500 0000 7286 0000 0072 8700 0000 da0e  ....r....r......
-00001c10: 6573 7469 6d61 746f 725f 6e61 6d65 725d  estimator_namer]
-00001c20: 0000 0072 5e00 0000 725f 0000 00a9 0272  ...r^...r_.....r
-00001c30: 1000 0000 723e 0000 0029 0b72 2700 0000  ....r>...).r'...
-00001c40: da08 7375 6270 6c6f 7473 7210 0000 0072  ..subplotsr....r
-00001c50: 0900 0000 7285 0000 0072 8600 0000 7287  ....r....r....r.
-00001c60: 0000 0072 3e00 0000 da03 7669 7a72 6300  ...r>.....vizrc.
-00001c70: 0000 723b 0000 00a9 0572 3000 0000 7210  ..r;.....r0...r.
-00001c80: 0000 0072 4d00 0000 724e 0000 00da 0366  ...rM...rN.....f
-00001c90: 6967 7217 0000 0072 1700 0000 7218 0000  igr....r....r...
-00001ca0: 0072 3b00 0000 ab00 0000 731a 0000 0000  .r;.......s.....
-00001cb0: 0108 010c 0106 0202 0104 0104 0108 0104  ................
-00001cc0: fc08 0604 0110 021a 017a 1052 6f63 4175  .........z.RocAu
-00001cd0: 6343 7572 7665 2e70 6c6f 7429 014e 2902  cCurve.plot).N).
-00001ce0: 4e4e 7264 0000 0072 1700 0000 7217 0000  NNrd...r....r...
-00001cf0: 0072 5400 0000 7218 0000 0072 8400 0000  .rT...r....r....
-00001d00: 9e00 0000 7306 0000 0008 010e 0608 0672  ....s..........r
-00001d10: 8400 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00001d20: 0000 0000 0004 0000 0000 0000 0073 3000  .............s0.
-00001d30: 0000 6500 5a01 6400 5a02 6408 8700 6601  ..e.Z.d.Z.d...f.
-00001d40: 6402 6403 8409 5a03 6404 6405 8400 5a04  d.d...Z.d.d...Z.
-00001d50: 6409 6406 6407 8401 5a05 8700 0400 5a06  d.d.d...Z.....Z.
-00001d60: 5300 290a da14 5072 6563 6973 696f 6e52  S.)...PrecisionR
-00001d70: 6563 616c 6c43 7572 7665 4e63 0400 0000  ecallCurveNc....
-00001d80: 0000 0000 0000 0000 0500 0000 0500 0000  ................
-00001d90: 0b00 0000 7328 0000 0074 0083 006a 017c  ....s(...t...j.|
-00001da0: 017c 027c 0364 018d 0301 0064 007c 005f  .|.|.d.....d.|._
-00001db0: 0264 007c 005f 0364 007c 005f 0464 0053  .d.|._.d.|._.d.S
-00001dc0: 0072 5000 0000 2905 7251 0000 0072 4800  .rP...).rQ...rH.
-00001dd0: 0000 da09 7072 6563 6973 696f 6eda 0672  ....precision..r
-00001de0: 6563 616c 6cda 1161 7665 7261 6765 5f70  ecall..average_p
-00001df0: 7265 6369 7369 6f6e 7253 0000 0072 5400  recisionrS...rT.
-00001e00: 0000 7217 0000 0072 1800 0000 7248 0000  ..r....r....rH..
-00001e10: 00be 0000 0073 0800 0000 0001 1201 0601  .....s..........
-00001e20: 0601 7a1d 5072 6563 6973 696f 6e52 6563  ..z.PrecisionRec
-00001e30: 616c 6c43 7572 7665 2e5f 5f69 6e69 745f  allCurve.__init_
-00001e40: 5f63 0200 0000 0000 0000 0000 0000 0300  _c..............
-00001e50: 0000 0400 0000 4300 0000 733c 0000 0074  ......C...s<...t
-00001e60: 007c 017c 006a 0119 007c 017c 006a 0219  .|.|.j...|.|.j..
-00001e70: 0083 025c 037c 005f 037c 005f 047d 0274  ...\.|._.|._.}.t
-00001e80: 057c 017c 006a 0119 007c 017c 006a 0219  .|.|.j...|.|.j..
-00001e90: 0083 027c 005f 067c 0053 0072 4900 0000  ...|._.|.S.rI...
-00001ea0: 2907 7205 0000 0072 4700 0000 7246 0000  ).r....rG...rF..
-00001eb0: 0072 9100 0000 7292 0000 0072 0800 0000  .r....r....r....
-00001ec0: 7293 0000 0072 8800 0000 7217 0000 0072  r....r....r....r
-00001ed0: 1700 0000 7218 0000 0072 4c00 0000 c400  ....r....rL.....
-00001ee0: 0000 730e 0000 0000 0102 0110 ff0e 0202  ..s.............
-00001ef0: 0110 ff06 027a 1850 7265 6369 7369 6f6e  .....z.Precision
-00001f00: 5265 6361 6c6c 4375 7276 652e 6669 7463  RecallCurve.fitc
-00001f10: 0300 0000 0000 0000 0000 0000 0500 0000  ................
-00001f20: 0600 0000 4b00 0000 7366 0000 007c 0164  ....K...sf...|.d
-00001f30: 0075 0072 1474 00a0 01a1 005c 027d 047d  .u.r.t.....\.}.}
-00001f40: 017c 017c 005f 0274 037c 006a 047c 006a  .|.|._.t.|.j.|.j
-00001f50: 057c 006a 067c 006a 0764 018d 047c 005f  .|.j.|.j.d...|._
-00001f60: 087c 0272 487c 016a 097c 0264 0264 0364  .|.rH|.j.|.d.d.d
-00001f70: 048d 0301 007c 006a 086a 0a66 007c 017c  .....|.j.j.f.|.|
-00001f80: 006a 0764 059c 027c 03a4 018e 0101 007c  .j.d...|.......|
-00001f90: 0053 0029 064e 2904 7291 0000 0072 9200  .S.).N).r....r..
-00001fa0: 0000 7293 0000 0072 8a00 0000 725d 0000  ..r....r....r]..
-00001fb0: 0072 5e00 0000 725f 0000 0072 8b00 0000  .r^...r_...r....
-00001fc0: 290b 7227 0000 0072 8c00 0000 7210 0000  ).r'...r....r...
-00001fd0: 0072 0a00 0000 7291 0000 0072 9200 0000  .r....r....r....
-00001fe0: 7293 0000 0072 3e00 0000 728d 0000 0072  r....r>...r....r
-00001ff0: 6300 0000 723b 0000 0072 8e00 0000 7217  c...r;...r....r.
-00002000: 0000 0072 1700 0000 7218 0000 0072 3b00  ...r....r....r;.
-00002010: 0000 cb00 0000 7316 0000 0000 0208 010c  ......s.........
-00002020: 0106 0202 0108 0108 fe08 0504 0110 021a  ................
-00002030: 017a 1950 7265 6369 7369 6f6e 5265 6361  .z.PrecisionReca
-00002040: 6c6c 4375 7276 652e 706c 6f74 2901 4e29  llCurve.plot).N)
-00002050: 024e 4e72 6400 0000 7217 0000 0072 1700  .NNrd...r....r..
-00002060: 0000 7254 0000 0072 1800 0000 7290 0000  ..rT...r....r...
-00002070: 00bd 0000 0073 0600 0000 0801 0e06 0807  .....s..........
-00002080: 7290 0000 0029 1dda 0361 6263 7202 0000  r....)...abcr...
-00002090: 0072 0300 0000 da11 6d61 7470 6c6f 746c  .r......matplotl
-000020a0: 6962 2e70 7970 6c6f 74da 0670 7970 6c6f  ib.pyplot..pyplo
-000020b0: 7472 2700 0000 da06 7061 6e64 6173 7282  tr'.....pandasr.
-000020c0: 0000 00da 0773 6561 626f 726e 7223 0000  .....seabornr#..
-000020d0: 00da 056e 756d 7079 7221 0000 0072 5600  ...numpyr!...rV.
-000020e0: 0000 5a0f 736b 6c65 6172 6e2e 6d65 7472  ..Z.sklearn.metr
-000020f0: 6963 7372 0400 0000 7205 0000 0072 0600  icsr....r....r..
-00002100: 0000 7207 0000 0072 0800 0000 7209 0000  ..r....r....r...
-00002110: 0072 0a00 0000 720b 0000 0072 4500 0000  .r....r....rE...
-00002120: 724f 0000 0072 6600 0000 7274 0000 0072  rO...rf...rt...r
-00002130: 7a00 0000 7284 0000 0072 9000 0000 7217  z...r....r....r.
-00002140: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
-00002150: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00002160: 7324 0000 0010 010c 0108 0108 0108 0108  s$..............
-00002170: 010c 010c 0110 010c 0110 030e 1e12 1210  ................
-00002180: 1510 1a10 1710 1a10 1f                   .........
+00000fa0: 000f 007c 0188 006a 0619 00a0 05a1 000f  ...|...j........
+00000fb0: 0040 0019 00a0 0088 006a 01a1 01a0 0787  .@.......j......
+00000fc0: 0066 0164 0164 0284 08a1 0188 005f 0888  .f.d.d......._..
+00000fd0: 006a 086a 0988 006a 036a 0a64 038d 0188  .j.j...j.j.d....
+00000fe0: 005f 0888 0053 0029 044e 6301 0000 0000  ._...S.).Nc.....
+00000ff0: 0000 0000 0000 0001 0000 0006 0000 0013  ................
+00001000: 0000 0073 3c00 0000 7400 7c00 8800 6a01  ...s<...t.|...j.
+00001010: 1900 a002 a100 8301 6401 6b04 7238 6402  ........d.k.r8d.
+00001020: 6403 7403 7c00 8800 6a01 1900 7c00 8800  d.t.|...j...|...
+00001030: 6a04 1900 8302 1400 6401 1800 1400 5300  j.......d.....S.
+00001040: 6400 5300 2904 4ee9 0100 0000 e964 0000  d.S.).N......d..
+00001050: 00e9 0200 0000 2905 721e 0000 0072 4700  ......).r....rG.
+00001060: 0000 da06 756e 6971 7565 7207 0000 0072  ....uniquer....r
+00001070: 4600 0000 7216 0000 00a9 0172 3000 0000  F...r......r0...
+00001080: 7217 0000 0072 1800 0000 7219 0000 005d  r....r....r....]
+00001090: 0000 0073 0a00 0000 0201 0cff 0201 02ff  ...s............
+000010a0: 2601 7a22 4765 6e47 494e 4943 7572 7665  &.z"GenGINICurve
+000010b0: 2e66 6974 2e3c 6c6f 6361 6c73 3e2e 3c6c  .fit.<locals>.<l
+000010c0: 616d 6264 613e 2901 721f 0000 0029 0bda  ambda>).r....)..
+000010d0: 0767 726f 7570 6279 7268 0000 00da 0473  .groupbyrh.....s
+000010e0: 697a 6572 6900 0000 7246 0000 0072 5a00  izeri...rF...rZ.
+000010f0: 0000 7247 0000 00da 0561 7070 6c79 7267  ..rG.....applyrg
+00001100: 0000 00da 0772 6569 6e64 6578 721f 0000  .....reindexr...
+00001110: 0072 4a00 0000 7217 0000 0072 6f00 0000  .rJ...r....ro...
+00001120: 7218 0000 0072 4c00 0000 5a00 0000 730c  r....rL...Z...s.
+00001130: 0000 0000 0112 012c 010a ff06 0314 017a  .......,.......z
+00001140: 1047 656e 4749 4e49 4375 7276 652e 6669  .GenGINICurve.fi
+00001150: 7463 0300 0000 0000 0000 0000 0000 0500  tc..............
+00001160: 0000 0700 0000 4b00 0000 735e 0000 007c  ......K...s^...|
+00001170: 0364 0119 007d 047c 017c 005f 007c 047c  .d...}.|.|._.|.|
+00001180: 005f 017c 006a 027c 006a 037c 0164 0264  ._.|.j.|.j.|.d.d
+00001190: 038d 0301 007c 006a 047c 006a 0566 017c  .....|.j.|.j.f.|
+000011a0: 047c 006a 0664 0464 0564 069c 047c 03a4  .|.j.d.d.d...|..
+000011b0: 018e 0101 007c 0272 5a7c 016a 077c 0264  .....|.rZ|.j.|.d
+000011c0: 0764 0864 098d 0301 007c 0053 0029 0a4e  .d.d.....|.S.).N
+000011d0: 723f 0000 0072 0c00 0000 7237 0000 005a  r?...r....r7...Z
+000011e0: 0447 494e 4954 2904 7210 0000 0072 3e00  .GINIT).r....r>.
+000011f0: 0000 7232 0000 0072 3d00 0000 725d 0000  ..r2...r=...r]..
+00001200: 0072 5e00 0000 725f 0000 0029 0872 1000  .r^...r_...).r..
+00001210: 0000 723f 0000 0072 3600 0000 7269 0000  ..r?...r6...ri..
+00001220: 0072 4100 0000 7267 0000 0072 3e00 0000  .rA...rg...r>...
+00001230: 7263 0000 0029 0572 3000 0000 7210 0000  rc...).r0...r...
+00001240: 0072 4d00 0000 724e 0000 0072 3f00 0000  .rM...rN...r?...
+00001250: 7217 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00001260: 3b00 0000 6200 0000 7310 0000 0000 0108  ;...b...s.......
+00001270: 0106 0106 0112 0120 0104 0110 017a 1147  ....... .....z.G
+00001280: 656e 4749 4e49 4375 7276 652e 706c 6f74  enGINICurve.plot
+00001290: 2901 4e29 024e 4e72 6400 0000 7217 0000  ).N).NNrd...r...
+000012a0: 0072 1700 0000 7254 0000 0072 1800 0000  .r....rT...r....
+000012b0: 7266 0000 0053 0000 0073 0600 0000 0801  rf...S...s......
+000012c0: 0e06 0808 7266 0000 0063 0000 0000 0000  ....rf...c......
+000012d0: 0000 0000 0000 0000 0000 0400 0000 0000  ................
+000012e0: 0000 7330 0000 0065 005a 0164 005a 0264  ..s0...e.Z.d.Z.d
+000012f0: 0887 0066 0164 0264 0384 095a 0364 0464  ...f.d.d...Z.d.d
+00001300: 0584 005a 0464 0964 0664 0784 015a 0587  ...Z.d.d.d...Z..
+00001310: 0004 005a 0653 0029 0ada 0c47 656e 5269  ...Z.S.)...GenRi
+00001320: 736b 4375 7276 654e 6305 0000 0000 0000  skCurveNc.......
+00001330: 0000 0000 0006 0000 0005 0000 000b 0000  ................
+00001340: 0073 2200 0000 7400 8300 6a01 7c01 7c02  .s"...t...j.|.|.
+00001350: 7c04 6401 8d03 0100 7c03 7c00 5f02 6400  |.d.....|.|._.d.
+00001360: 7c00 5f03 6400 5300 7250 0000 0029 0472  |._.d.S.rP...).r
+00001370: 5100 0000 7248 0000 0072 6800 0000 da04  Q...rH...rh.....
+00001380: 7269 736b 726a 0000 0072 5400 0000 7217  riskrj...rT...r.
+00001390: 0000 0072 1800 0000 7248 0000 006e 0000  ...r....rH...n..
+000013a0: 0073 0600 0000 0001 1201 0601 7a15 4765  .s..........z.Ge
+000013b0: 6e52 6973 6b43 7572 7665 2e5f 5f69 6e69  nRiskCurve.__ini
+000013c0: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
+000013d0: 0200 0000 0400 0000 4300 0000 7322 0000  ........C...s"..
+000013e0: 007c 01a0 007c 006a 01a1 017c 006a 0219  .|...|.j...|.j..
+000013f0: 00a0 0364 0164 0267 02a1 017c 005f 047c  ...d.d.g...|._.|
+00001400: 0053 0029 034e 7269 0000 00da 046d 6561  .S.).Nri.....mea
+00001410: 6e29 0572 7000 0000 7268 0000 0072 4700  n).rp...rh...rG.
+00001420: 0000 da03 6167 6772 7500 0000 724a 0000  ....aggru...rJ..
+00001430: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00001440: 724c 0000 0073 0000 0073 0400 0000 0001  rL...s...s......
+00001450: 1e01 7a10 4765 6e52 6973 6b43 7572 7665  ..z.GenRiskCurve
+00001460: 2e66 6974 6305 0000 0000 0000 0000 0000  .fitc...........
+00001470: 0007 0000 0007 0000 004b 0000 0073 6800  .........K...sh.
+00001480: 0000 7c05 6401 1900 7d06 7c01 7c00 5f00  ..|.d...}.|.|._.
+00001490: 7c06 7c00 5f01 7c03 6400 7500 7220 6402  |.|._.|.d.u.r d.
+000014a0: 7d03 7c00 6a02 7c00 6a03 6403 1900 7c01  }.|.j.|.j.d...|.
+000014b0: 6404 6405 8d03 0100 7c00 6a04 7c00 6a03  d.d.....|.j.|.j.
+000014c0: 6406 1900 7c06 7c03 7c04 6407 6408 8d05  d...|.|.|.d.d...
+000014d0: 0100 7c02 7264 7c01 6a05 7c02 6409 640a  ..|.rd|.j.|.d.d.
+000014e0: 640b 8d03 0100 7c00 5300 290c 4e72 3f00  d.....|.S.).Nr?.
+000014f0: 0000 fa0b 4d65 616e 2054 6172 6765 7472  ....Mean Targetr
+00001500: 6900 0000 720c 0000 0072 3700 0000 7276  i...r....r7...rv
+00001510: 0000 0054 a903 7232 0000 0072 3e00 0000  ...T..r2...r>...
+00001520: 723d 0000 0072 5d00 0000 725e 0000 0072  r=...r]...r^...r
+00001530: 5f00 0000 2906 7210 0000 0072 3f00 0000  _...).r....r?...
+00001540: 7236 0000 0072 7500 0000 7241 0000 0072  r6...ru...rA...r
+00001550: 6300 0000 2907 7230 0000 0072 1000 0000  c...).r0...r....
+00001560: 724d 0000 0072 3200 0000 723e 0000 0072  rM...r2...r>...r
+00001570: 4e00 0000 723f 0000 0072 1700 0000 7217  N...r?...r....r.
+00001580: 0000 0072 1800 0000 723b 0000 0077 0000  ...r....r;...w..
+00001590: 0073 1400 0000 0001 0801 0601 0601 0801  .s..............
+000015a0: 0401 1601 1a01 0401 1001 7a11 4765 6e52  ..........z.GenR
+000015b0: 6973 6b43 7572 7665 2e70 6c6f 7429 014e  iskCurve.plot).N
+000015c0: 2904 4e4e 4e4e 7264 0000 0072 1700 0000  ).NNNNrd...r....
+000015d0: 7217 0000 0072 5400 0000 7218 0000 0072  r....rT...r....r
+000015e0: 7400 0000 6d00 0000 7306 0000 0008 010e  t...m...s.......
+000015f0: 0508 0472 7400 0000 6300 0000 0000 0000  ...rt...c.......
+00001600: 0000 0000 0000 0000 0005 0000 0000 0000  ................
+00001610: 0073 3000 0000 6500 5a01 6400 5a02 6408  .s0...e.Z.d.Z.d.
+00001620: 8700 6601 6402 6403 8409 5a03 6404 6405  ..f.d.d...Z.d.d.
+00001630: 8400 5a04 6409 6406 6407 8401 5a05 8700  ..Z.d.d.d...Z...
+00001640: 0400 5a06 5300 290a da0d 4d65 616e 5072  ..Z.S.)...MeanPr
+00001650: 6f62 4375 7276 654e 6304 0000 0000 0000  obCurveNc.......
+00001660: 0000 0000 0005 0000 0005 0000 000b 0000  ................
+00001670: 0073 2800 0000 7400 8300 6a01 7c01 7c02  .s(...t...j.|.|.
+00001680: 7c03 6401 8d03 0100 6400 7c00 5f02 6400  |.d.....d.|._.d.
+00001690: 7c00 5f03 6400 7c00 5f04 6400 5300 7250  |._.d.|._.d.S.rP
+000016a0: 0000 0029 0572 5100 0000 7248 0000 00da  ...).rQ...rH....
+000016b0: 0a70 645f 6465 6369 6c65 73da 0770 645f  .pd_deciles..pd_
+000016c0: 6269 6e73 da09 6d65 616e 5f70 726f 6272  bins..mean_probr
+000016d0: 5300 0000 7254 0000 0072 1700 0000 7218  S...rT...r....r.
+000016e0: 0000 0072 4800 0000 8500 0000 7308 0000  ...rH.......s...
+000016f0: 0000 0112 0106 0106 017a 164d 6561 6e50  .........z.MeanP
+00001700: 726f 6243 7572 7665 2e5f 5f69 6e69 745f  robCurve.__init_
+00001710: 5f63 0200 0000 0000 0000 0000 0000 0200  _c..............
+00001720: 0000 0700 0000 4300 0000 734c 0000 0074  ......C...sL...t
+00001730: 006a 017c 017c 006a 0219 0074 03a0 0464  .j.|.|.j...t...d
+00001740: 0164 0264 03a1 0364 0464 0564 068d 045c  .d.d...d.d.d...\
+00001750: 027c 005f 057c 005f 067c 01a0 077c 006a  .|._.|._.|...|.j
+00001760: 05a1 017c 006a 0819 00a0 0964 0764 0867  ...|.j.....d.d.g
+00001770: 02a1 017c 005f 0a7c 0053 0029 094e 7201  ...|._.|.S.).Nr.
+00001780: 0000 0067 0b7a 6f0c 0100 f03f 679a 9999  ...g.zo....?g...
+00001790: 9999 99b9 3fda 0464 726f 7054 2903 da01  ....?..dropT)...
+000017a0: 71da 0a64 7570 6c69 6361 7465 73da 0772  q..duplicates..r
+000017b0: 6574 6269 6e73 7269 0000 0072 7600 0000  etbinsri...rv...
+000017c0: 290b da02 7064 da04 7163 7574 7246 0000  )...pd..qcutrF..
+000017d0: 0072 2100 0000 7222 0000 0072 7b00 0000  .r!...r"...r{...
+000017e0: 727c 0000 0072 7000 0000 7247 0000 0072  r|...rp...rG...r
+000017f0: 7700 0000 727d 0000 0072 4a00 0000 7217  w...r}...rJ...r.
+00001800: 0000 0072 1700 0000 7218 0000 0072 4c00  ...r....r....rL.
+00001810: 0000 8b00 0000 7316 0000 0000 0110 0106  ......s.........
+00001820: ff02 0104 ff0e 020a 0104 ff04 0106 ff06  ................
+00001830: 027a 114d 6561 6e50 726f 6243 7572 7665  .z.MeanProbCurve
+00001840: 2e66 6974 6306 0000 0000 0000 0000 0000  .fitc...........
+00001850: 0007 0000 0007 0000 004b 0000 0073 6000  .........K...s`.
+00001860: 0000 7c01 7c00 5f00 7c02 7c00 5f01 7c04  ..|.|._.|.|._.|.
+00001870: 6400 7500 7218 6401 7d04 7c00 6a02 7c00  d.u.r.d.}.|.j.|.
+00001880: 6a03 6402 1900 7c01 6403 6404 8d03 0100  j.d...|.d.d.....
+00001890: 7c00 6a04 7c00 6a03 6405 1900 7c02 7c04  |.j.|.j.d...|.|.
+000018a0: 7c05 6406 6407 8d05 0100 7c03 725c 7c01  |.d.d.....|.r\|.
+000018b0: 6a05 7c03 6408 6409 640a 8d03 0100 7c00  j.|.d.d.d.....|.
+000018c0: 5300 290b 4e72 7800 0000 7269 0000 0072  S.).Nrx...ri...r
+000018d0: 0c00 0000 7237 0000 0072 7600 0000 5472  ....r7...rv...Tr
+000018e0: 7900 0000 725d 0000 0072 5e00 0000 725f  y...r]...r^...r_
+000018f0: 0000 0029 0672 1000 0000 723f 0000 0072  ...).r....r?...r
+00001900: 3600 0000 727d 0000 0072 4100 0000 7263  6...r}...rA...rc
+00001910: 0000 0029 0772 3000 0000 7210 0000 0072  ...).r0...r....r
+00001920: 3f00 0000 724d 0000 0072 3200 0000 723e  ?...rM...r2...r>
+00001930: 0000 0072 4e00 0000 7217 0000 0072 1700  ...rN...r....r..
+00001940: 0000 7218 0000 0072 3b00 0000 9200 0000  ..r....r;.......
+00001950: 7312 0000 0000 0106 0106 0108 0104 0116  s...............
+00001960: 011a 0104 0110 017a 124d 6561 6e50 726f  .......z.MeanPro
+00001970: 6243 7572 7665 2e70 6c6f 7429 014e 2905  bCurve.plot).N).
+00001980: 4e4e 4e4e 4e72 6400 0000 7217 0000 0072  NNNNNrd...r....r
+00001990: 1700 0000 7254 0000 0072 1800 0000 727a  ....rT...r....rz
+000019a0: 0000 0084 0000 0073 0600 0000 0801 0e06  .......s........
+000019b0: 0807 727a 0000 0063 0000 0000 0000 0000  ..rz...c........
+000019c0: 0000 0000 0000 0000 0400 0000 0000 0000  ................
+000019d0: 7330 0000 0065 005a 0164 005a 0264 0887  s0...e.Z.d.Z.d..
+000019e0: 0066 0164 0264 0384 095a 0364 0464 0584  .f.d.d...Z.d.d..
+000019f0: 005a 0464 0964 0664 0784 015a 0587 0004  .Z.d.d.d...Z....
+00001a00: 005a 0653 0029 0ada 0b52 6f63 4175 6343  .Z.S.)...RocAucC
+00001a10: 7572 7665 4e63 0400 0000 0000 0000 0000  urveNc..........
+00001a20: 0000 0500 0000 0500 0000 0b00 0000 7328  ..............s(
+00001a30: 0000 0074 0083 006a 017c 017c 027c 0364  ...t...j.|.|.|.d
+00001a40: 018d 0301 0064 007c 005f 0264 007c 005f  .....d.|._.d.|._
+00001a50: 0364 007c 005f 0464 0053 0072 5000 0000  .d.|._.d.S.rP...
+00001a60: 2905 7251 0000 0072 4800 0000 da03 6670  ).rQ...rH.....fp
+00001a70: 72da 0374 7072 da07 726f 635f 6175 6372  r..tpr..roc_aucr
+00001a80: 5300 0000 7254 0000 0072 1700 0000 7218  S...rT...r....r.
+00001a90: 0000 0072 4800 0000 9f00 0000 7308 0000  ...rH.......s...
+00001aa0: 0000 0112 0106 0106 017a 1452 6f63 4175  .........z.RocAu
+00001ab0: 6343 7572 7665 2e5f 5f69 6e69 745f 5f63  cCurve.__init__c
+00001ac0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00001ad0: 0400 0000 4300 0000 7334 0000 0074 007c  ....C...s4...t.|
+00001ae0: 017c 006a 0119 007c 017c 006a 0219 0083  .|.j...|.|.j....
+00001af0: 025c 037c 005f 037c 005f 047d 0274 057c  .\.|._.|._.}.t.|
+00001b00: 006a 037c 006a 0483 027c 005f 067c 0053  .j.|.j...|._.|.S
+00001b10: 0072 4900 0000 2907 7204 0000 0072 4700  .rI...).r....rG.
+00001b20: 0000 7246 0000 0072 8500 0000 7286 0000  ..rF...r....r...
+00001b30: 0072 0600 0000 7287 0000 00a9 0372 3000  .r....r......r0.
+00001b40: 0000 724b 0000 00da 015f 7217 0000 0072  ..rK....._r....r
+00001b50: 1700 0000 7218 0000 0072 4c00 0000 a500  ....r....rL.....
+00001b60: 0000 730a 0000 0000 0102 0110 ff0e 0210  ..s.............
+00001b70: 017a 0f52 6f63 4175 6343 7572 7665 2e66  .z.RocAucCurve.f
+00001b80: 6974 6303 0000 0000 0000 0000 0000 0005  itc.............
+00001b90: 0000 0006 0000 004b 0000 0073 6a00 0000  .......K...sj...
+00001ba0: 7c01 6400 7500 7214 7400 a001 a100 5c02  |.d.u.r.t.....\.
+00001bb0: 7d04 7d01 7c01 7c00 5f02 7403 7c00 6a04  }.}.|.|._.t.|.j.
+00001bc0: 7c00 6a05 7c00 6a06 6401 1400 7c00 6a07  |.j.|.j.d...|.j.
+00001bd0: 6402 8d04 7c00 5f08 7c02 724c 7c01 6a09  d...|._.|.rL|.j.
+00001be0: 7c02 6403 6404 6405 8d03 0100 7c00 6a08  |.d.d.d.....|.j.
+00001bf0: 6a0a 6600 7c01 7c00 6a07 6406 9c02 7c03  j.f.|.|.j.d...|.
+00001c00: a401 8e01 0100 7c00 5300 2907 4e72 6c00  ......|.S.).Nrl.
+00001c10: 0000 2904 7285 0000 0072 8600 0000 7287  ..).r....r....r.
+00001c20: 0000 00da 0e65 7374 696d 6174 6f72 5f6e  .....estimator_n
+00001c30: 616d 6572 5d00 0000 725e 0000 0072 5f00  amer]...r^...r_.
+00001c40: 0000 a902 7210 0000 0072 3e00 0000 290b  ....r....r>...).
+00001c50: 7227 0000 00da 0873 7562 706c 6f74 7372  r'.....subplotsr
+00001c60: 1000 0000 7209 0000 0072 8500 0000 7286  ....r....r....r.
+00001c70: 0000 0072 8700 0000 723e 0000 00da 0376  ...r....r>.....v
+00001c80: 697a 7263 0000 0072 3b00 0000 a905 7230  izrc...r;.....r0
+00001c90: 0000 0072 1000 0000 724d 0000 0072 4e00  ...r....rM...rN.
+00001ca0: 0000 da03 6669 6772 1700 0000 7217 0000  ....figr....r...
+00001cb0: 0072 1800 0000 723b 0000 00ab 0000 0073  .r....r;.......s
+00001cc0: 1a00 0000 0001 0801 0c01 0602 0201 0401  ................
+00001cd0: 0401 0801 04fc 0806 0401 1002 1a01 7a10  ..............z.
+00001ce0: 526f 6341 7563 4375 7276 652e 706c 6f74  RocAucCurve.plot
+00001cf0: 2901 4e29 024e 4e72 6400 0000 7217 0000  ).N).NNrd...r...
+00001d00: 0072 1700 0000 7254 0000 0072 1800 0000  .r....rT...r....
+00001d10: 7284 0000 009e 0000 0073 0600 0000 0801  r........s......
+00001d20: 0e06 0806 7284 0000 0063 0000 0000 0000  ....r....c......
+00001d30: 0000 0000 0000 0000 0000 0400 0000 0000  ................
+00001d40: 0000 7330 0000 0065 005a 0164 005a 0264  ..s0...e.Z.d.Z.d
+00001d50: 0887 0066 0164 0264 0384 095a 0364 0464  ...f.d.d...Z.d.d
+00001d60: 0584 005a 0464 0964 0664 0784 015a 0587  ...Z.d.d.d...Z..
+00001d70: 0004 005a 0653 0029 0ada 1450 7265 6369  ...Z.S.)...Preci
+00001d80: 7369 6f6e 5265 6361 6c6c 4375 7276 654e  sionRecallCurveN
+00001d90: 6304 0000 0000 0000 0000 0000 0005 0000  c...............
+00001da0: 0005 0000 000b 0000 0073 2800 0000 7400  .........s(...t.
+00001db0: 8300 6a01 7c01 7c02 7c03 6401 8d03 0100  ..j.|.|.|.d.....
+00001dc0: 6400 7c00 5f02 6400 7c00 5f03 6400 7c00  d.|._.d.|._.d.|.
+00001dd0: 5f04 6400 5300 7250 0000 0029 0572 5100  _.d.S.rP...).rQ.
+00001de0: 0000 7248 0000 00da 0970 7265 6369 7369  ..rH.....precisi
+00001df0: 6f6e da06 7265 6361 6c6c da11 6176 6572  on..recall..aver
+00001e00: 6167 655f 7072 6563 6973 696f 6e72 5300  age_precisionrS.
+00001e10: 0000 7254 0000 0072 1700 0000 7218 0000  ..rT...r....r...
+00001e20: 0072 4800 0000 be00 0000 7308 0000 0000  .rH.......s.....
+00001e30: 0112 0106 0106 017a 1d50 7265 6369 7369  .......z.Precisi
+00001e40: 6f6e 5265 6361 6c6c 4375 7276 652e 5f5f  onRecallCurve.__
+00001e50: 696e 6974 5f5f 6302 0000 0000 0000 0000  init__c.........
+00001e60: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
+00001e70: 3c00 0000 7400 7c01 7c00 6a01 1900 7c01  <...t.|.|.j...|.
+00001e80: 7c00 6a02 1900 8302 5c03 7c00 5f03 7c00  |.j.....\.|._.|.
+00001e90: 5f04 7d02 7405 7c01 7c00 6a01 1900 7c01  _.}.t.|.|.j...|.
+00001ea0: 7c00 6a02 1900 8302 7c00 5f06 7c00 5300  |.j.....|._.|.S.
+00001eb0: 7249 0000 0029 0772 0500 0000 7247 0000  rI...).r....rG..
+00001ec0: 0072 4600 0000 7291 0000 0072 9200 0000  .rF...r....r....
+00001ed0: 7208 0000 0072 9300 0000 7288 0000 0072  r....r....r....r
+00001ee0: 1700 0000 7217 0000 0072 1800 0000 724c  ....r....r....rL
+00001ef0: 0000 00c4 0000 0073 0e00 0000 0001 0201  .......s........
+00001f00: 10ff 0e02 0201 10ff 0602 7a18 5072 6563  ..........z.Prec
+00001f10: 6973 696f 6e52 6563 616c 6c43 7572 7665  isionRecallCurve
+00001f20: 2e66 6974 6303 0000 0000 0000 0000 0000  .fitc...........
+00001f30: 0005 0000 0006 0000 004b 0000 0073 6600  .........K...sf.
+00001f40: 0000 7c01 6400 7500 7214 7400 a001 a100  ..|.d.u.r.t.....
+00001f50: 5c02 7d04 7d01 7c01 7c00 5f02 7403 7c00  \.}.}.|.|._.t.|.
+00001f60: 6a04 7c00 6a05 7c00 6a06 7c00 6a07 6401  j.|.j.|.j.|.j.d.
+00001f70: 8d04 7c00 5f08 7c02 7248 7c01 6a09 7c02  ..|._.|.rH|.j.|.
+00001f80: 6402 6403 6404 8d03 0100 7c00 6a08 6a0a  d.d.d.....|.j.j.
+00001f90: 6600 7c01 7c00 6a07 6405 9c02 7c03 a401  f.|.|.j.d...|...
+00001fa0: 8e01 0100 7c00 5300 2906 4e29 0472 9100  ....|.S.).N).r..
+00001fb0: 0000 7292 0000 0072 9300 0000 728a 0000  ..r....r....r...
+00001fc0: 0072 5d00 0000 725e 0000 0072 5f00 0000  .r]...r^...r_...
+00001fd0: 728b 0000 0029 0b72 2700 0000 728c 0000  r....).r'...r...
+00001fe0: 0072 1000 0000 720a 0000 0072 9100 0000  .r....r....r....
+00001ff0: 7292 0000 0072 9300 0000 723e 0000 0072  r....r....r>...r
+00002000: 8d00 0000 7263 0000 0072 3b00 0000 728e  ....rc...r;...r.
+00002010: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00002020: 0000 723b 0000 00cb 0000 0073 1600 0000  ..r;.......s....
+00002030: 0002 0801 0c01 0602 0201 0801 08fe 0805  ................
+00002040: 0401 1002 1a01 7a19 5072 6563 6973 696f  ......z.Precisio
+00002050: 6e52 6563 616c 6c43 7572 7665 2e70 6c6f  nRecallCurve.plo
+00002060: 7429 014e 2902 4e4e 7264 0000 0072 1700  t).N).NNrd...r..
+00002070: 0000 7217 0000 0072 5400 0000 7218 0000  ..r....rT...r...
+00002080: 0072 9000 0000 bd00 0000 7306 0000 0008  .r........s.....
+00002090: 010e 0608 0772 9000 0000 291d da03 6162  .....r....)...ab
+000020a0: 6372 0200 0000 7203 0000 00da 116d 6174  cr....r......mat
+000020b0: 706c 6f74 6c69 622e 7079 706c 6f74 da06  plotlib.pyplot..
+000020c0: 7079 706c 6f74 7227 0000 00da 0670 616e  pyplotr'.....pan
+000020d0: 6461 7372 8200 0000 da07 7365 6162 6f72  dasr......seabor
+000020e0: 6e72 2300 0000 da05 6e75 6d70 7972 2100  nr#.....numpyr!.
+000020f0: 0000 7256 0000 005a 0f73 6b6c 6561 726e  ..rV...Z.sklearn
+00002100: 2e6d 6574 7269 6373 7204 0000 0072 0500  .metricsr....r..
+00002110: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
+00002120: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00002130: 7245 0000 0072 4f00 0000 7266 0000 0072  rE...rO...rf...r
+00002140: 7400 0000 727a 0000 0072 8400 0000 7290  t...rz...r....r.
+00002150: 0000 0072 1700 0000 7217 0000 0072 1700  ...r....r....r..
+00002160: 0000 7218 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00002170: 3e01 0000 0073 2400 0000 1001 0c01 0801  >....s$.........
+00002180: 0801 0801 0801 0c01 0c01 1001 0c01 1003  ................
+00002190: 0e1e 1212 1015 101a 1017 101a 101f       ..............
```

### Comparing `crosspredict-1.1.7/crosspredict/report_binary/__pycache__/_report_binary.cpython-39.pyc` & `crosspredict-1.1.8/crosspredict/report_binary/__pycache__/_report_binary.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/crosspredict/report_binary/_curves.py` & `crosspredict-1.1.8/crosspredict/report_binary/_curves.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/crosspredict/report_binary/_report_binary.py` & `crosspredict-1.1.8/crosspredict/report_binary/_report_binary.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/crosspredict/target_encoder/_crosstargetencoder.py` & `crosspredict-1.1.8/crosspredict/target_encoder/_crosstargetencoder.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/crosspredict/target_encoder/_target_encoder.py` & `crosspredict-1.1.8/crosspredict/target_encoder/_target_encoder.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/crosspredict.egg-info/PKG-INFO` & `crosspredict-1.1.8/crosspredict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosspredict
-Version: 1.1.7
+Version: 1.1.8
 Summary: package for easy crossvalidation
 Home-page: UNKNOWN
 Author: Vladislav Boyadzhi
 Author-email: vladislav.boyadzhi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crosspredict-1.1.7/crosspredict.egg-info/SOURCES.txt` & `crosspredict-1.1.8/crosspredict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/setup.py` & `crosspredict-1.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     with open('{0}/requirements.txt'.format(dir_path), 'r') as reqs:
         requirements = reqs.readlines()
     return requirements
 
 if __name__ == "__main__":
     setup(
         name="crosspredict",
-        version="1.1.7",
+        version="1.1.8",
         author="Vladislav Boyadzhi",
         author_email="vladislav.boyadzhi@gmail.com",
         description='package for easy crossvalidation',
         long_description=long_description,
         long_description_content_type="text/markdown",
         packages=find_packages(),
         classifiers=[
```

### Comparing `crosspredict-1.1.7/tests/conftest.py` & `crosspredict-1.1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/tests/test_binary.py` & `crosspredict-1.1.8/tests/test_binary.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.7/tests/test_iterator.py` & `crosspredict-1.1.8/tests/test_iterator.py`

 * *Files identical despite different names*

