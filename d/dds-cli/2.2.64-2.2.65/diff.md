# Comparing `tmp/dds_cli-2.2.64.tar.gz` & `tmp/dds_cli-2.2.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dds_cli-2.2.64.tar", last modified: Wed Apr 26 07:07:13 2023, max compression
+gzip compressed data, was "dds_cli-2.2.65.tar", last modified: Thu May 25 11:46:20 2023, max compression
```

## Comparing `dds_cli-2.2.64.tar` & `dds_cli-2.2.65.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:07:13.969940 dds_cli-2.2.64/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-26 07:06:39.000000 dds_cli-2.2.64/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-26 07:07:13.969940 dds_cli-2.2.64/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-04-26 07:06:39.000000 dds_cli-2.2.64/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:07:13.965940 dds_cli-2.2.64/dds_cli/
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76580 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/account_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/custom_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/data_getter.py
--rw-r--r--   0 runner    (1001) docker     (123)    22599 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/data_lister.py
--rw-r--r--   0 runner    (1001) docker     (123)    16136 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/data_putter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/data_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/file_compressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/file_encryptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10854 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/file_handler_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/file_handler_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/maintenance_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/motd_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/project_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/project_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/project_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/s3_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/text_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/unit_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14639 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13616 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:07:13.969940 dds_cli-2.2.64/dds_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-26 07:07:13.000000 dds_cli-2.2.64/dds_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-26 07:07:13.000000 dds_cli-2.2.64/dds_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:07:13.000000 dds_cli-2.2.64/dds_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-26 07:07:13.000000 dds_cli-2.2.64/dds_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:06:58.000000 dds_cli-2.2.64/dds_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-26 07:07:13.000000 dds_cli-2.2.64/dds_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 07:07:13.000000 dds_cli-2.2.64/dds_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-26 07:06:39.000000 dds_cli-2.2.64/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 07:07:13.969940 dds_cli-2.2.64/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-26 07:06:39.000000 dds_cli-2.2.64/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:07:13.969940 dds_cli-2.2.64/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:06:39.000000 dds_cli-2.2.64/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-26 07:06:39.000000 dds_cli-2.2.64/tests/test_account_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-26 07:06:39.000000 dds_cli-2.2.64/tests/test_data_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-04-26 07:06:39.000000 dds_cli-2.2.64/tests/test_file_compressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-04-26 07:06:39.000000 dds_cli-2.2.64/tests/test_file_encryptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-04-26 07:06:39.000000 dds_cli-2.2.64/tests/test_file_handler_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-26 07:06:39.000000 dds_cli-2.2.64/tests/test_maintenance_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-26 07:06:39.000000 dds_cli-2.2.64/tests/test_motd_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-04-26 07:06:39.000000 dds_cli-2.2.64/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:46:20.760563 dds_cli-2.2.65/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-25 11:45:46.000000 dds_cli-2.2.65/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-25 11:46:20.760563 dds_cli-2.2.65/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-25 11:45:46.000000 dds_cli-2.2.65/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:46:20.760563 dds_cli-2.2.65/dds_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76736 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/account_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/custom_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/data_getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22507 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/data_lister.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16330 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/data_putter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/data_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/file_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/file_encryptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/file_handler_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/file_handler_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/maintenance_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/motd_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/project_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/project_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/project_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/s3_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/text_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/unit_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13800 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 11:45:46.000000 dds_cli-2.2.65/dds_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:46:20.760563 dds_cli-2.2.65/dds_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-25 11:46:20.000000 dds_cli-2.2.65/dds_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-25 11:46:20.000000 dds_cli-2.2.65/dds_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:46:20.000000 dds_cli-2.2.65/dds_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 11:46:20.000000 dds_cli-2.2.65/dds_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:46:05.000000 dds_cli-2.2.65/dds_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-25 11:46:20.000000 dds_cli-2.2.65/dds_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 11:46:20.000000 dds_cli-2.2.65/dds_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-25 11:45:46.000000 dds_cli-2.2.65/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:46:20.760563 dds_cli-2.2.65/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-25 11:45:46.000000 dds_cli-2.2.65/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:46:20.760563 dds_cli-2.2.65/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:45:46.000000 dds_cli-2.2.65/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-25 11:45:46.000000 dds_cli-2.2.65/tests/test_account_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-25 11:45:46.000000 dds_cli-2.2.65/tests/test_data_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-05-25 11:45:46.000000 dds_cli-2.2.65/tests/test_file_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-05-25 11:45:46.000000 dds_cli-2.2.65/tests/test_file_encryptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-05-25 11:45:46.000000 dds_cli-2.2.65/tests/test_file_handler_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-05-25 11:45:46.000000 dds_cli-2.2.65/tests/test_maintenance_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-25 11:45:46.000000 dds_cli-2.2.65/tests/test_motd_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-05-25 11:45:46.000000 dds_cli-2.2.65/tests/test_utils.py
```

### Comparing `dds_cli-2.2.64/LICENSE` & `dds_cli-2.2.65/LICENSE`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.64/PKG-INFO` & `dds_cli-2.2.65/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dds_cli
-Version: 2.2.64
+Version: 2.2.65
 Summary: A command line tool to manage data and projects in the SciLifeLab Data Delivery System.
 Home-page: https://github.com/ScilifelabDataCentre/dds_cli
 Author: SciLifeLab Data Centre
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dds_cli Version: 2.2.64 Summary: A command line
+Metadata-Version: 2.1 Name: dds_cli Version: 2.2.65 Summary: A command line
 tool to manage data and projects in the SciLifeLab Data Delivery System. Home-
 page: https://github.com/ScilifelabDataCentre/dds_cli Author: SciLifeLab Data
 Centre License: MIT Classifier: Development Status :: 4 - Beta Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `dds_cli-2.2.64/README.md` & `dds_cli-2.2.65/README.md`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.64/dds_cli/__init__.py` & `dds_cli-2.2.65/dds_cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: skip-file
 """DDS CLI."""
 
 import datetime
 import os
 import pathlib
 import prompt_toolkit
 import rich.console
@@ -55,15 +56,15 @@
 class DDSEndpoint:
     """Defines all DDS urls."""
 
     # Base url - local or remote
     BASE_ENDPOINT_LOCAL = "http://127.0.0.1:5000/api/v1"
     BASE_ENDPOINT_DOCKER = "http://dds_backend:5000/api/v1"
     BASE_ENDPOINT_REMOTE = "https://delivery.scilifelab.se/api/v1"
-    BASE_ENDPOINT_REMOTE_TEST = "https://dds-dev.dckube.scilifelab.se/api/v1"
+    BASE_ENDPOINT_REMOTE_TEST = "https://dds-dev.dckube3.scilifelab.se/api/v1"
     if os.getenv("DDS_CLI_ENV") == "development":
         BASE_ENDPOINT = BASE_ENDPOINT_LOCAL
     elif os.getenv("DDS_CLI_ENV") == "docker-dev":
         BASE_ENDPOINT = BASE_ENDPOINT_DOCKER
     elif os.getenv("DDS_CLI_ENV") == "test-instance":
         BASE_ENDPOINT = BASE_ENDPOINT_REMOTE_TEST
     else:
```

### Comparing `dds_cli-2.2.64/dds_cli/__main__.py` & `dds_cli-2.2.65/dds_cli/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # IMPORTS ################################################################################ IMPORTS #
 ####################################################################################################
 
 # Standard library
 import concurrent.futures
 import itertools
 import logging
-import os
 import sys
 import typing
 
 # Installed
 import pathlib
 import rich_click as click
 import click_pathlib
@@ -67,44 +66,43 @@
 ####################################################################################################
 
 LOG = logging.getLogger("dds_cli")
 
 # Configuration for rich-click output
 click.rich_click.MAX_WIDTH = 100
 
-
 ## # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 #                                                                                                  #
 #                          MMMM   MMMM      AAAA      II   NNNN    NN                              #
 #                          MM MM MM MM     AA  AA     II   NN NN   NN                              #
 #                          MM  MMM  MM    AA    AA    II   NN  NN  NN                              #
 #                          MM   M   MM   AAAAAAAAAA   II   NN   NN NN                              #
 #                          MM       MM   AA      AA   II   NN    NNNN                              #
 #                                                                                                  #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # ##
 
 
-dds_url = dds_cli.DDSEndpoint.BASE_ENDPOINT
+DDS_URL = dds_cli.DDSEndpoint.BASE_ENDPOINT
+DDS_URL_BASE = DDS_URL[: DDS_URL.index("/", 8)]
+
 # Print header to STDERR
 dds_cli.utils.stderr_console.print(
     "[green]     ︵",
     "\n[green] ︵ (  )   ︵",
     "\n[green](  ) ) (  (  )[/]   [bold]SciLifeLab Data Delivery System",
-    "\n[green] ︶  (  ) ) ([/]    [blue][link={0}]{0}/[/link]".format(
-        dds_url[: dds_url.index("/", 8)]
-    ),
+    f"\n[green] ︶  (  ) ) ([/]    [blue][link={DDS_URL_BASE}]{DDS_URL_BASE}/[/link]",
     f"\n[green]      ︶ (  )[/]    [dim]CLI Version {dds_cli.__version__}",
     "\n[green]          ︶",
     highlight=False,
 )
 
 if len(sys.argv) == 1 or (len(sys.argv) > 1 and sys.argv[1] != "motd"):
     motds = dds_cli.motd_manager.MotdManager.list_all_active_motds(table=False)
     if motds:
-        dds_cli.utils.stderr_console.print(f"[bold]Important information:[/bold]")
+        dds_cli.utils.stderr_console.print("[bold]Important information:[/bold]")
         for motd in motds:
             dds_cli.utils.stderr_console.print(f"{motd['Created']} - {motd['Message']} \n")
 
 
 # -- dds -- #
 @click.group()
 @click.option(
@@ -376,15 +374,18 @@
     ),
 )
 @click.option(
     "--allow-group",
     is_flag=True,
     required=False,
     default=False,
-    help="[Not recommended, use with care] Allow read permissions to group. Sets 640 permission instead of 600, allowing others to access your authenticated session token.",
+    help=(
+        "[Not recommended, use with care] Allow read permissions to group. Sets 640 permission instead of 600, "
+        "allowing others to access your authenticated session token."
+    ),
 )
 @click.pass_obj
 def login(click_ctx, totp, allow_group):
     """Start or renew an authenticated session.
 
     Creates or renews the authentication token stored in the '.dds_cli_token' file.
 
@@ -400,15 +401,15 @@
     if no_prompt:
         LOG.warning("The --no-prompt flag is ignored for `dds auth login`")
     try:
         with dds_cli.auth.Auth(
             token_path=click_ctx.get("TOKEN_PATH"), totp=totp, allow_group=allow_group
         ):
             # Authentication token renewed in the init method.
-            LOG.info(f"[green] :white_check_mark: Authentication successful![/green]")
+            LOG.info("[green] :white_check_mark: Authentication successful![/green]")
     except (
         dds_cli.exceptions.APIError,
         dds_cli.exceptions.AuthenticationError,
         dds_cli.exceptions.DDSCLIException,
         dds_cli.exceptions.ApiResponseError,
         dds_cli.exceptions.ApiRequestError,
     ) as err:
@@ -558,15 +559,15 @@
     """
     try:
         with dds_cli.account_manager.AccountManager(
             no_prompt=click_ctx.get("NO_PROMPT", False),
             token_path=click_ctx.get("TOKEN_PATH"),
         ) as lister:
             if invites:
-                lister.list_invites(unit=unit, invites=invites)
+                lister.list_invites(invites=invites)
             else:
                 lister.list_users(unit=unit)
 
     except (
         dds_cli.exceptions.AuthenticationError,
         dds_cli.exceptions.ApiResponseError,
         dds_cli.exceptions.ApiRequestError,
@@ -579,15 +580,15 @@
 # -- dds user find -- #
 # TODO: Move this to dds unit?
 @user_group_command.command(name="find")
 @username_option(
     required=True, help_message="[Super Admins only] The username of the account you want to check."
 )
 @click.pass_obj
-def list_users(click_ctx, username):
+def find_users(click_ctx, username):
     """Check if a username is registered to an account in the DDS."""
     try:
         with dds_cli.account_manager.AccountManager(
             no_prompt=click_ctx.get("NO_PROMPT", False),
             token_path=click_ctx.get("TOKEN_PATH"),
         ) as lister:
             lister.find_user(user_to_find=username)
@@ -617,15 +618,15 @@
     required=True,
     type=click.Choice(
         choices=["Super Admin", "Unit Admin", "Unit Personnel", "Project Owner", "Researcher"],
         case_sensitive=False,
     ),
     help=(
         "Type of account. To include a space in the chosen role, use quotes "
-        '(e.g. "Unit Personnel") or escape the space (e.g. Unit\ Personnel)'
+        r'(e.g. "Unit Personnel") or escape the space (e.g. Unit\ Personnel)'
     ),
 )
 @click.option(
     "--unit",
     required=False,
     help="[Super Admins only]  To specify which unit the user should belong to.",
 )
@@ -995,16 +996,17 @@
             token_path=click_ctx.get("TOKEN_PATH"),
         ) as creator:
             emails_roles = []
             if owner or researcher:
                 email_overlap = set(owner) & set(researcher)
                 if email_overlap:
                     LOG.info(
-                        f"The email(s) {email_overlap} specified as both owner and researcher! "
-                        "Please specify a unique role for each email."
+                        "The email(s) %s specified as both owner and researcher! "
+                        "Please specify a unique role for each email.",
+                        email_overlap,
                     )
                     sys.exit(1)
                 if owner:
                     emails_roles.extend([{"email": x, "role": "Project Owner"} for x in owner])
                 if researcher:
                     emails_roles.extend([{"email": x, "role": "Researcher"} for x in researcher])
 
@@ -1683,15 +1685,16 @@
     if get_all and (source or source_path_file):
         LOG.error(
             "Flag '--get-all' cannot be used together with options '--source'/'--source-path-fail'."
         )
         sys.exit(1)
     elif not get_all and not (source or source_path_file):
         LOG.error(
-            "Specify either '--source' or '--source-path-file' to download specific directories/files, or '--get-all' to download all project contents."
+            "Specify either '--source' or '--source-path-file' to download specific directories/files, "
+            "or '--get-all' to download all project contents."
         )
         sys.exit(1)
 
     try:
         # Begin delivery
         with dds_cli.data_getter.DataGetter(
             project=project,
@@ -1722,15 +1725,15 @@
                 with concurrent.futures.ThreadPoolExecutor() as texec:
                     task_dwnld = progress.add_task(
                         "Download", total=len(getter.filehandler.data), step="summary"
                     )
 
                     # Schedule the first num_threads futures for upload
                     for file in itertools.islice(iterator, num_threads):
-                        LOG.debug(f"Starting: {rich.markup.escape(str(file))}")
+                        LOG.debug("Starting: %s", rich.markup.escape(str(file)))
                         # Execute download
                         download_threads[
                             texec.submit(getter.download_and_verify, file=file, progress=progress)
                         ] = file
 
                     while download_threads:
                         # Wait for the next future to complete
@@ -1738,36 +1741,38 @@
                             download_threads, return_when=concurrent.futures.FIRST_COMPLETED
                         )
 
                         new_tasks = 0
 
                         for dfut in ddone:
                             downloaded_file = download_threads.pop(dfut)
-                            LOG.debug(
-                                f"Future done: {rich.markup.escape(str(downloaded_file))}",
-                            )
+                            LOG.debug("Future done: %s", rich.markup.escape(str(downloaded_file)))
 
                             # Get result
                             try:
                                 file_downloaded = dfut.result()
                                 LOG.debug(
-                                    f"Download of {rich.markup.escape(str(downloaded_file))} successful: {file_downloaded}"
+                                    "Download of %s successful: %s",
+                                    rich.markup.escape(str(downloaded_file)),
+                                    file_downloaded,
                                 )
                             except concurrent.futures.BrokenExecutor as err:
                                 LOG.critical(
-                                    f"Download of file {rich.markup.escape(str(downloaded_file))} failed! Error: {err}"
+                                    "Download of file %s failed! Error: %s",
+                                    rich.markup.escape(str(downloaded_file)),
+                                    err,
                                 )
                                 continue
 
                             new_tasks += 1
                             progress.advance(task_dwnld)
 
                         # Schedule the next set of futures for download
                         for next_file in itertools.islice(iterator, new_tasks):
-                            LOG.debug(f"Starting: {rich.markup.escape(str(next_file))}")
+                            LOG.debug("Starting: %s", rich.markup.escape(str(next_file)))
                             # Execute download
                             download_threads[
                                 texec.submit(
                                     getter.download_and_verify,
                                     file=next_file,
                                     progress=progress,
                                 )
@@ -1864,15 +1869,15 @@
             "'--rm-all' / '--file' / '--folder'."
         )
         sys.exit(1)
 
     # Warn if trying to remove all contents
     if rm_all:
         if no_prompt:
-            LOG.warning(f"Deleting all files within project '{project}'")
+            LOG.warning("Deleting all files within project '%s'", project)
         else:
             if not rich.prompt.Confirm.ask(
                 f"Are you sure you want to delete all files within project '{project}'?"
             ):
                 LOG.info("Probably for the best. Exiting.")
                 sys.exit(0)
 
@@ -2099,28 +2104,28 @@
         with dds_cli.data_lister.DataLister(
             show_usage=True,
             no_prompt=click_ctx.get("NO_PROMPT", False),
             json=True,
             token_path=click_ctx.get("TOKEN_PATH"),
         ) as lister:
             # Get projects, only active by default
-            projects: typing.List = lister.list_projects(show_all=(stat_type == "all"))
+            projects: typing.List = lister.list_projects(show_all=stat_type == "all")
 
             if stat_type == "size":
                 # Calculate total amount of saved data in active projects
                 title_bold_part: str = "Bytes"
                 title_rest: str = "currently stored in DDS"
-                value: int = sum([x["Size"] for x in projects])
+                value: int = sum(x["Size"] for x in projects)
             else:
                 # Get number of projects
                 title_bold_part: str = "Active" if stat_type == "active" else "Total"
                 title_rest: str = "projects"
                 value: int = len(projects)
 
-            LOG.info(f"[bold]{title_bold_part}[/bold] {title_rest}: {value}")
+            LOG.info("[bold]%s[/bold] %s: %s", title_bold_part, title_rest, value)
     except (
         dds_cli.exceptions.APIError,
         dds_cli.exceptions.AuthenticationError,
         dds_cli.exceptions.ApiResponseError,
         dds_cli.exceptions.ApiRequestError,
     ) as err:
         LOG.error(err)
```

### Comparing `dds_cli-2.2.64/dds_cli/account_manager.py` & `dds_cli-2.2.65/dds_cli/account_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """Admin class, adds ."""
 
 ####################################################################################################
 # IMPORTS ################################################################################ IMPORTS #
 ###################################################################################################
 
 # Standard library
-from email import header
 import logging
 
 # Installed
 import rich.markup
-from rich.table import Table
 
 # Own modules
 import dds_cli
 import dds_cli.auth
 import dds_cli.base
 import dds_cli.exceptions
 import dds_cli.utils
@@ -135,19 +133,24 @@
         for field in response.get("info", []):
             if isinstance(response["info"][field], str):
                 response["info"][field] = rich.markup.escape(response["info"][field])
 
         info = response.get("info")
         if info:
             LOG.info(
-                f"Username:          {info['username']} \
-                \nRole:              {info['role']} \
-                \nName:              {info['name']} \
-                \nPrimary Email:     {info['email_primary']} \
-                \nAssociated Emails: {', '.join(str(x) for x in info['emails_all'])}"
+                "Username:          %s \n"
+                "Role:              %s \n"
+                "Name:              %s \n"
+                "Primary Email:     %s \n"
+                "Associated Emails: %s \n",
+                info["username"],
+                info["role"],
+                info["name"],
+                info["email_primary"],
+                ", ".join(str(x) for x in info["emails_all"]),
             )
 
     def user_activation(self, email, action):
         """Deactivate/Reactivate users"""
         json = {"email": email, "action": action}
         response_json, _ = dds_cli.utils.perform_request(
             dds_cli.DDSEndpoint.USER_ACTIVATION,
@@ -169,15 +172,15 @@
             headers=self.token,
             params={"project": project},
             json=json,
             error_message=f"Failed to fix project access for user '{email}'",
         )
 
         if project_errors:
-            LOG.warning(f"Could not fix user '{email}' access to the following projects:")
+            LOG.warning("Could not fix user '%s' access to the following projects:", email)
             msg = project_errors
         else:
             msg = response_json.get(
                 "message",
                 (
                     f"Project access fixed for user '{email}'. "
                     "They should now have access to all project data."
@@ -193,15 +196,15 @@
             method="get",
             headers=self.token,
             json={"unit": unit},
             error_message="Failed getting unit users from API",
         )
 
         if response.get("empty"):
-            LOG.info(f"There are no Unit Admins or Unit Personnel connected to unit '{unit}'")
+            LOG.info("There are no Unit Admins or Unit Personnel connected to unit '%s'", unit)
             return
 
         users, keys = dds_cli.utils.get_required_in_response(
             keys=["users", "keys"], response=response
         )
 
         # Sort users according to name
@@ -222,28 +225,28 @@
             rows=users,
             caption=caption,
         )
 
         # Print out table
         dds_cli.utils.print_or_page(item=table)
 
-    def list_invites(self, unit: str = None, invites: bool = None) -> None:
+    def list_invites(self, invites: bool = None) -> None:
         """List all unit users within a specific unit."""
         response, _ = dds_cli.utils.perform_request(
             endpoint=dds_cli.DDSEndpoint.LIST_INVITED_USERS,
             method="get",
             headers=self.token,
             error_message="Failed getting invites from API",
         )
         title = "Current invites"
         caption = "All invited users where you have access"
         invites = response.get("invites")
 
         if not invites:
-            LOG.info(f"There are no current invites")
+            LOG.info("There are no current invites")
             return
 
         table = dds_cli.utils.create_table(
             title=title,
             columns=response.get("keys"),
             rows=invites,
             caption=caption,
@@ -265,9 +268,9 @@
         exists = response.get("exists")
         if exists is None:
             raise dds_cli.exceptions.ApiResponseError(
                 message="No information returned from API. Could not determine if user account exists."
             )
 
         LOG.info(
-            f"Account exists: {'[blue][bold]Yes[/bold][/blue]' if exists else '[red][bold]No[/bold][/red]'}"
+            "Account exists: [bold]%s[/bold]", "[blue]Yes[/blue]" if exists else "[red]No[/red]"
         )
```

### Comparing `dds_cli-2.2.64/dds_cli/auth.py` & `dds_cli-2.2.65/dds_cli/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Data Delivery System authentication manager."""
 # Standard library
 import logging
 import getpass
 
 # Installed
-import rich
+from rich.prompt import Prompt
 
 # Own modules
 import dds_cli
 from dds_cli import base
 from dds_cli import exceptions
 from dds_cli import user
 import dds_cli.utils
@@ -44,45 +44,49 @@
             force_renew_token=force_renew_token,
             token_path=token_path,
             totp=totp,
             allow_group=allow_group,
         )
 
     def check(self):
+        """Check if token exists and return info."""
         token_file = user.TokenFile(token_path=self.token_path)
         if token_file.file_exists():
             token = token_file.read_token()
             if token:
                 token_file.token_report(token=token)
         else:
             LOG.info(
-                "[red]No saved token found, or token has expired. Authenticate yourself with `dds auth login` to use this functionality![/red]"
+                "[red]No saved token found, or token has expired. "
+                "Authenticate yourself with `dds auth login` to use this functionality![/red]"
             )
 
     def logout(self):
+        """Logout user by removing authenticated token."""
         token_file = user.TokenFile(token_path=self.token_path)
         if token_file.file_exists():
             token_file.delete_token()
             LOG.info("[green] :white_check_mark: Successfully logged out![/green]")
         else:
             LOG.info("[green]Already logged out![/green]")
 
     def twofactor(self, auth_method: str = None):
+        """Perform 2FA for user."""
         if auth_method == "totp":
             response_json, _ = dds_cli.utils.perform_request(
                 endpoint=dds_cli.DDSEndpoint.USER_ACTIVATE_TOTP,
                 headers=self.token,
                 method="post",
             )
         else:
             # Need to authenticate again since TOTP might have been lost
             LOG.info(
                 "Activating authentication via email, please (re-)enter your username and password:"
             )
-            username: str = rich.prompt.Prompt.ask("DDS username")
+            username: str = Prompt.ask("DDS username")
             password: str = getpass.getpass(prompt="DDS password: ")
 
             if password == "":
                 raise exceptions.AuthenticationError(
                     message="Non-empty password needed to be able to authenticate."
                 )
 
@@ -91,14 +95,15 @@
                 method="post",
                 auth=(username, password),
             )
 
         LOG.info(response_json.get("message"))
 
     def deactivate(self, username: str = None):
+        """Deactivate TOTP for user."""
         response_json, _ = dds_cli.utils.perform_request(
             endpoint=dds_cli.DDSEndpoint.TOTP_DEACTIVATE,
             headers=self.token,
             json={"username": username},
             method="put",
         )
         LOG.info(response_json.get("message"))
```

### Comparing `dds_cli-2.2.64/dds_cli/base.py` & `dds_cli-2.2.65/dds_cli/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,18 @@
 
 ###############################################################################
 # IMPORTS ########################################################### IMPORTS #
 ###############################################################################
 
 # Standard library
 import logging
-import os
 import pathlib
 import typing
 
 # Installed
-import http
-import time
-import simplejson
 from rich.progress import Progress, SpinnerColumn
 
 # Own modules
 import dds_cli.directory
 import dds_cli.timestamp
 import dds_cli.utils
 
@@ -67,15 +63,15 @@
         self.no_prompt = no_prompt
         self.token_path = token_path
 
         if self.method_check:
             # Get attempted operation e.g. put/ls/rm/get
             if self.method not in DDS_METHODS:
                 raise exceptions.InvalidMethodError(attempted_method=self.method)
-            LOG.debug(f"Attempted operation: {self.method}")
+            LOG.debug("Attempted operation: %s", self.method)
 
             # Use user defined destination if any specified
             if self.method in DDS_DIR_REQUIRED_METHODS:
                 default_dir = pathlib.Path(
                     f"DataDelivery_{dds_cli.timestamp.TimeStamp().timestamp}_{self.project}"
                 )
                 if mount_dir:
@@ -110,33 +106,33 @@
         # files within project
         if self.method in DDS_KEYS_REQUIRED_METHODS:
             if self.method == "put":
                 self.s3connector = self.__get_safespring_keys()
 
             self.keys = self.__get_project_keys()
 
-            self.status = dict()
+            self.status: typing.Dict = {}
             self.filehandler = None
 
     def __enter__(self):
         """Return self when using context manager."""
         return self
 
-    def __exit__(self, exc_type, exc_value, tb, max_fileerrs: int = 40):
+    def __exit__(self, exception_type, exception_value, traceback, max_fileerrs: int = 40):
         """Finish and print out delivery summary.
 
         This is not entered if there's an error during __init__.
         """
         if self.method in ["put", "get", "rm"]:
             if self.method != "rm":
                 self.__printout_delivery_summary()
 
         # Exception is not handled
-        if exc_type is not None:
-            LOG.debug(f"Exception: {exc_type} with value {exc_value}")
+        if exception_type is not None:
+            LOG.debug("Exception: %s with value %s", exception_type, exception_value)
             return False
 
         return True
 
     # Private methods ############################### Private methods #
     def __get_safespring_keys(self):
         """Get safespring keys."""
@@ -184,15 +180,15 @@
             raise exceptions.NoKeyError(f"Project access denied: No {key_type} key.")
 
         return project_public[key_type]
 
     def __printout_delivery_summary(self):
         """Print out the delivery summary if any files were cancelled."""
         if self.stop_doing:
-            LOG.info(f"{'Upload' if self.method == 'put' else 'Download'} cancelled.\n")
+            LOG.info("%s cancelled.\n", "Upload" if self.method == "put" else "Download")
             return
 
         # TODO: Look into a better summary print out - old deleted for now
         any_failed = self.__collect_all_failed()
         true_failed = [entry for entry in any_failed if entry["message"] != "File already uploaded"]
         nr_uploaded = len(any_failed) - len(true_failed)
 
@@ -206,39 +202,41 @@
                     "Errors occurred during upload.\n"
                     "If you wish to retry the upload, re-run the 'dds data put' command again, "
                     "specifying the same options as you did now. To also overwrite the files "
                     "that were uploaded, also add the '--overwrite' flag at the end of the command.\n\n"
                     f"Please verify that the following error log has been generated: {self.failed_delivery_log}\n"
                     "[red][bold]Do not[/bold][/red] delete this file; The Data Centre may need it during DDS support."
                 )
-            else:
-                # TODO: --destination should be able to >at least< overwrite the files in the
-                # previously created download location.
-                raise exceptions.DownloadError(
-                    "Errors occurred during download.\n"
-                    "If you wish to retry the download, re-run the `dds data get` command again, "
-                    "specifying the same options as you did now. A new directory will "
-                    "automatically be created and all files will be downloaded again.\n\n"
-                    f"See {self.failed_delivery_log} for more information."
-                )
 
-        elif nr_uploaded:
+            # TODO: --destination should be able to >at least< overwrite the files in the
+            # previously created download location.
+            raise exceptions.DownloadError(
+                "Errors occurred during download.\n"
+                "If you wish to retry the download, re-run the `dds data get` command again, "
+                "specifying the same options as you did now. A new directory will "
+                "automatically be created and all files will be downloaded again.\n\n"
+                f"See {self.failed_delivery_log} for more information."
+            )
+
+        if nr_uploaded:
             # Raise exception in order to give exit code 1
             LOG.warning(
-                f"{nr_uploaded} files have already been uploaded to this project.\nUpload [bold]partially[/bold] completed!\n"
+                "%s files have already been uploaded to this project.\n"
+                "Upload [bold]partially[/bold] completed!\n",
+                nr_uploaded,
             )
 
         else:
             # Printout if no cancelled/failed files
             dds_cli.utils.console.print(
                 f"\n{'Upload' if self.method == 'put' else 'Download'} completed!\n"
             )
 
         if self.method == "get" and len(self.filehandler.data) > len(any_failed):
-            LOG.info(f"Any downloaded files are located: {self.filehandler.local_destination}.")
+            LOG.info("Any downloaded files are located at: %s.", self.filehandler.local_destination)
 
     def __collect_all_failed(self, sort: bool = True) -> list:
         """Put cancelled files from status in to failed dict and sort the output."""
         # Transform all items to string
         self.filehandler.data = {
             str(file): {str(x): str(y) for x, y in info.items()}
             for file, info in list(self.filehandler.data.items())
```

### Comparing `dds_cli-2.2.64/dds_cli/custom_decorators.py` & `dds_cli-2.2.65/dds_cli/custom_decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,21 +48,21 @@
         if self.status[file]["cancel"]:
             message = f"File already cancelled, stopping file {escape(file)}"
             LOG.warning(message)
             return False
 
         # Mark as started
         self.status[file]["started"] = True
-        LOG.debug(f"File {escape(str(file))} started {func.__name__}")
+        LOG.debug("File '%s' started: %s", escape(str(file)), func.__name__)
 
         # Run function
         ok_to_proceed, message = func(self, file=file, *args, **kwargs)
         # Cancel file(s) if something failed
         if not ok_to_proceed:
-            LOG.warning(f"{func.__name__} failed: {message}")
+            LOG.warning("%s failed: %s", func.__name__, message)
             self.status[file].update({"cancel": True, "message": message})
             if self.status[file].get("failed_op") is None:
                 self.status[file]["failed_op"] = "crypto"
 
             if self.break_on_fail:
                 message = f"'--break-on-fail'. File causing failure: '{file}'. "
                 LOG.warning(message)
@@ -87,36 +87,40 @@
 def update_status(func):
     """Decorator for updating the status of files."""
 
     @functools.wraps(func)
     def wrapped(self, file, *args, **kwargs):
         # TODO (ina): add processing?
         if func.__name__ not in ["put", "add_file_db", "get", "update_db"]:
-            raise Exception(f"The function {func.__name__} cannot be used with this decorator.")
+            raise dds_cli.exceptions.DDSCLIException(
+                f"The function {func.__name__} cannot be used with this decorator."
+            )
         if func.__name__ not in self.status[file]:
-            raise Exception(f"No status found for function {func.__name__}.")
+            raise dds_cli.exceptions.DDSCLIException(
+                f"No status found for function {func.__name__}."
+            )
 
         # Update status to started
         self.status[file][func.__name__].update({"started": True})
-        LOG.debug(f"File {escape(str(file))} status updated to {func.__name__}: started")
+        LOG.debug("File '%s' status updated to %s: started", escape(str(file)), func.__name__)
 
         # Run function
         ok_to_continue, message, *_ = func(self, file=file, *args, **kwargs)
 
         # ok_to_continue = False
         if not ok_to_continue:
             # Save info about which operation failed
 
             self.status[file]["failed_op"] = func.__name__
-            LOG.warning(f"{func.__name__} failed: {message}")
+            LOG.warning("%s failed: %s", func.__name__, message)
 
         else:
             # Update status to done
             self.status[file][func.__name__].update({"done": True})
-            LOG.debug(f"File {escape(str(file))} status updated to {func.__name__}: done")
+            LOG.debug("File %s status updated to %s: done", escape(str(file)), func.__name__)
 
         return ok_to_continue, message
 
     return wrapped
 
 
 def subpath_required(func):
@@ -133,28 +137,26 @@
         # Create path
         if not full_subpath.exists():
             try:
                 full_subpath.mkdir(parents=True, exist_ok=True)
             except OSError as err:
                 return False, str(err)
 
-            LOG.debug(f"New directory created: {full_subpath}")
+            LOG.debug("New directory created: '%s'", full_subpath)
 
         return func(self, file=file, *args, **kwargs)
 
     return check_and_create
 
 
 def removal_spinner(func):
     """Spinner for the rm command"""
 
     @functools.wraps(func)
     def create_and_remove_task(self, *args, **kwargs):
-        message = ""
-
         with Progress(
             "[bold]{task.description}",
             SpinnerColumn(spinner_name="dots12", style="white"),
             console=dds_cli.utils.stderr_console,
         ) as progress:
             # Determine spinner text
             if func.__name__ == "remove_all":
@@ -182,15 +184,15 @@
             table_len = self.failed_table.renderable.row_count
 
             if table_len + 5 > dds_cli.utils.console.height:
                 with dds_cli.utils.console.pager():
                     dds_cli.utils.console.print(self.failed_table)
             else:
                 dds_cli.utils.console.print(self.failed_table)
-            LOG.warning(f"Finished {description_lc} with errors, see table above")
+            LOG.warning("Finished %s with errors, see table above", description_lc)
         elif self.failed_files is not None:
             self.failed_files["result"] = f"Finished {description_lc} with errors"
             dds_cli.utils.console.print(self.failed_files)
         else:
             dds_cli.utils.console.print(f"Successfully finished {description_lc}")
 
     return create_and_remove_task
```

### Comparing `dds_cli-2.2.64/dds_cli/data_getter.py` & `dds_cli-2.2.65/dds_cli/data_getter.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 # Standard library
 import logging
 import pathlib
 
 # Installed
 import requests
-import simplejson
 from rich.markup import escape
 from rich.progress import Progress, SpinnerColumn
 
 # Own modules
 from dds_cli import DDSEndpoint, FileSegment
 from dds_cli import file_handler_remote as fhr
 from dds_cli import data_remover as dr
@@ -97,15 +96,15 @@
                     ":warning-emoji: Some specified files were not found in the system "
                     "and '--break-on-fail' flag used. :warning-emoji:"
                     f"Files not found: {self.filehandler.failed}"
                 )
 
             if not self.filehandler.data:
                 if self.temporary_directory and self.temporary_directory.is_dir():
-                    LOG.debug(f"Deleting temporary folder {self.temporary_directory}.")
+                    LOG.debug("Deleting temporary folder '%s'.", self.temporary_directory)
                     dds_cli.utils.delete_folder(self.temporary_directory)
                 raise dds_cli.exceptions.DownloadError("No files to download.")
 
             self.status = self.filehandler.create_download_status_dict()
 
             progress.remove_task(wait_task)
 
@@ -130,21 +129,21 @@
         # Update progress task for decryption
         progress.reset(
             task,
             description=txt.TextHandler.task_name(file=escape(str(file)), step="decrypt"),
             total=file_info["size_original"],
         )
 
-        LOG.debug(f"File {escape(str(file))} downloaded: {file_downloaded}")
+        LOG.debug("File '%s' downloaded: %s", escape(str(file)), file_downloaded)
 
         if file_downloaded:
             db_updated, message = self.update_db(file=file)
-            LOG.debug(f"Database updated: {db_updated}")
+            LOG.debug("Database updated: %s", db_updated)
 
-            LOG.debug(f"Beginning decryption of file {escape(str(file))}...")
+            LOG.debug("Beginning decryption of file '%s'...", escape(str(file)))
             file_saved = False
             with fe.Decryptor(
                 project_keys=self.keys,
                 peer_public=file_info["public_key"],
                 key_salt=file_info["salt"],
             ) as decryptor:
                 streamed_chunks = decryptor.decrypt_file(infile=file_info["path_downloaded"])
@@ -156,15 +155,15 @@
                 )
 
                 file_saved, message = stream_to_file_func(
                     chunks=streamed_chunks,
                     outfile=file,
                 )
 
-            LOG.debug(f"file saved? {file_saved}")
+            LOG.debug("File saved? %s", file_saved)
             if file_saved:
                 # TODO (ina): decide on checksum verification method --
                 # this checks original, the other is generated from compressed
                 all_ok, message = (
                     fe.Encryptor.verify_checksum(file=file, correct_checksum=file_info["checksum"])
                     if self.verify_checksum
                     else (True, "")
@@ -180,14 +179,15 @@
         """Download files from the cloud."""
         downloaded = False
         error = ""
         file_local = self.filehandler.data[file]["path_downloaded"]
         file_remote = self.filehandler.data[file]["url"]
 
         try:
+            # TODO: Set timeout? (pylint)
             with requests.get(file_remote, stream=True) as req:
                 req.raise_for_status()
                 with file_local.open(mode="wb") as new_file:
                     for chunk in req.iter_content(chunk_size=FileSegment.SEGMENT_SIZE_CIPHER):
                         progress.update(task, advance=len(chunk))
                         new_file.write(chunk)
         except (
@@ -210,15 +210,14 @@
 
         return downloaded, error
 
     @update_status
     def update_db(self, file):
         """Update file info in db."""
         updated_in_db = False
-        error = ""
 
         # Get file info
         fileinfo = self.filehandler.data[file]
         filename = {"name": fileinfo["name_in_db"]}
         params = {"project": self.project}
 
         # Send file info to API
```

### Comparing `dds_cli-2.2.64/dds_cli/data_lister.py` & `dds_cli-2.2.65/dds_cli/data_lister.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,19 @@
 ###############################################################################
 # IMPORTS ########################################################### IMPORTS #
 ###############################################################################
 
 # Standard library
 from dataclasses import dataclass
 import logging
-import os
 from typing import Tuple, Union, List
 import datetime
 import pathlib
 
 # Installed
-import requests
-import simplejson
 from rich.padding import Padding
 from rich.markup import escape
 from rich.table import Table
 from rich.tree import Tree
 import pytz
 import tzlocal
 
@@ -97,37 +94,37 @@
         if not project_info:
             raise exceptions.NoDataError("No project info was retrieved. No files to list.")
         for project in project_info:
             try:
                 last_updated = pytz.timezone("UTC").localize(
                     datetime.datetime.strptime(project["Last updated"], "%a, %d %b %Y %H:%M:%S GMT")
                 )
-            except ValueError as err:
+            except ValueError as exc:
                 raise exceptions.ApiResponseError(
                     f"Time zone mismatch: Incorrect zone '{project['Last updated'].split()[-1]}'"
-                )
-            else:
-                project["Last updated"] = last_updated.astimezone(tzlocal.get_localzone()).strftime(
-                    "%a, %d %b %Y %H:%M:%S %Z"
-                )
+                ) from exc
+
+            project["Last updated"] = last_updated.astimezone(tzlocal.get_localzone()).strftime(
+                "%a, %d %b %Y %H:%M:%S %Z"
+            )
 
         # Sort projects according to chosen or default, first ID
         sorted_projects = self.__sort_projects(projects=project_info, sort_by=sort_by)
 
         if not self.json:
             self.__print_project_table(sorted_projects, usage_info, total_size, always_show)
 
         # Return the list of projects
         return sorted_projects
 
     def list_files(self, folder: str = None, show_size: bool = False):
         """Create a tree displaying the files within the project."""
-        LOG.info(f"Listing files for project '{self.project}'")
+        LOG.info("Listing files for project '%s'", self.project)
         if folder:
-            LOG.info(f"Showing files in folder '{escape(str(folder))}'")
+            LOG.info("Showing files in folder '%s'", escape(str(folder)))
 
         if folder is None:
             folder = ""
         # Make call to API
         response, _ = dds_cli.utils.perform_request(
             DDSEndpoint.LIST_FILES,
             method="get",
@@ -152,55 +149,55 @@
         tree_title = escape(str(folder)) or f"Files / directories in project: [green]{self.project}"
         tree = Tree(f"[bold magenta]{tree_title}")
 
         if not sorted_files_folders:
             raise exceptions.NoDataError(f"Could not find folder: '{escape(folder)}'")
 
         # Get max length of file name
-        max_string = max([len(x["name"]) for x in sorted_files_folders])
+        max_string = max(len(x["name"]) for x in sorted_files_folders)
 
         # Get max length of size string
         max_size = max(
-            [
+            (
                 len(
                     dds_cli.utils.format_api_response(
                         response=x["size"], key="Size", binary=self.binary
                     ).split(" ", maxsplit=1)[0]
                 )
                 for x in sorted_files_folders
                 if show_size and "size" in x
-            ],
+            ),
             default=0,
         )
 
         # Visible folders
         visible_folders = []
 
         # Add items to tree
-        for x in sorted_files_folders:
+        for item in sorted_files_folders:
             # Check if string is folder
-            is_folder = x.pop("folder")
+            is_folder = item.pop("folder")
 
             # Att 1 for folders due to trailing /
             tab = th.TextHandler.format_tabs(
-                string_len=len(x["name"]) + (1 if is_folder else 0),
+                string_len=len(item["name"]) + (1 if is_folder else 0),
                 max_string_len=max_string,
             )
 
             # Add formatting if folder and set string name
             line = ""
             if is_folder:
                 line = "[bold deep_sky_blue3]"
-                visible_folders.append(x["name"])
-            line += escape(x["name"]) + ("/" if is_folder else "")
+                visible_folders.append(item["name"])
+            line += escape(item["name"]) + ("/" if is_folder else "")
 
             # Add size to line if option specified
-            if show_size and "size" in x:
+            if show_size and "size" in item:
                 size = dds_cli.utils.format_api_response(
-                    response=x["size"], key="Size", binary=self.binary
+                    response=item["size"], key="Size", binary=self.binary
                 )
                 line += f"{tab}{size.split()[0]}"
 
                 # Define space between number and size format
                 tabs_bf_format = th.TextHandler.format_tabs(
                     string_len=len(size), max_string_len=max_size, tab_len=2
                 )
@@ -253,44 +250,47 @@
             Recurses through the project directories.
 
             Constructs a file tree by subsequent calls to the API
             """
             tree = FileTree([], f"{basename}/")
             try:
                 sorted_files_folders = __api_call_list_files(folder)
-            except exceptions.NoDataError as e:
+            except exceptions.NoDataError as exc:
                 if folder is None:
                     raise exceptions.NoDataError(
                         "No files or folders found for the specified project"
-                    )
-                else:
-                    raise exceptions.NoDataError(f"Could not find folder: '{escape(folder)}'")
+                    ) from exc
+
+                raise exceptions.NoDataError(f"Could not find folder: '{escape(folder)}'") from exc
 
             # Get max length of file name
-            max_string = max([len(x["name"]) for x in sorted_files_folders])
+            max_string = max(len(x["name"]) for x in sorted_files_folders)
 
             # Get max length of size string
             max_size = max(
-                [
+                (
                     len(x["size"].split(" ")[0])
                     for x in sorted_files_folders
                     if show_size and "size" in x
-                ],
+                ),
                 default=0,
             )
+
             # Rich outputs precisely one line per file/folder
-            for f in sorted_files_folders:
-                is_folder = f.pop("folder")
+            for item in sorted_files_folders:
+                is_folder = item.pop("folder")
 
                 if not is_folder:
-                    tree.subtrees.append((escape(f["name"]), f.get("size") if show_size else None))
+                    tree.subtrees.append(
+                        (escape(item["name"]), item.get("size") if show_size else None)
+                    )
                 else:
                     subtree, _max_string, _max_size = __construct_file_tree(
-                        pathlib.Path(folder, f["name"]).as_posix() if folder else f["name"],
-                        f"[bold deep_sky_blue3]{escape(f['name'])}",
+                        pathlib.Path(folder, item["name"]).as_posix() if folder else item["name"],
+                        f"[bold deep_sky_blue3]{escape(item['name'])}",
                     )
                     # Due to indentation, the filename strings of
                     # subdirectories are 4 characters deeper than
                     # their parent directories
                     max_string = max(max_string, _max_string + 4)
                     max_size = max(max_size, _max_size)
                     tree.subtrees.append(subtree)
@@ -301,31 +301,31 @@
             """
             Recurses through the project directories.
 
             Constructs a file tree by subsequent calls to the API
             """
             try:
                 sorted_files_folders = __api_call_list_files(folder)
-            except exceptions.NoDataError as e:
+            except exceptions.NoDataError as exc:
                 if folder is None:
                     raise exceptions.NoDataError(
                         "No files or folders found for the specified project"
-                    )
-                else:
-                    raise exceptions.NoDataError(f"Could not find folder: '{folder}'")
+                    ) from exc
+
+                raise exceptions.NoDataError(f"Could not find folder: '{folder}'") from exc
 
             tree = {}
 
-            for f in sorted_files_folders:
-                is_folder = f.pop("folder")
-                name = f["name"]
+            for item in sorted_files_folders:
+                is_folder = item.pop("folder")
+                name = item["name"]
                 if not is_folder:
                     tree[name] = {"name": name, "is_folder": False, "children": {}}
                     if show_size:
-                        tree[f["name"]]["size"] = f.get("size")
+                        tree[item["name"]]["size"] = item.get("size")
                 else:
                     children = __construct_file_dict_tree(
                         pathlib.Path(folder, name).as_posix() if folder else name,
                     )
                     tree[name] = {"name": name, "is_folder": True, "children": children}
 
             return tree
@@ -360,46 +360,46 @@
                     tree.add(line)
 
             return tree, tree_length
 
         if self.json:
             tree_dict = __construct_file_dict_tree(None)
             return tree_dict
-        else:
-            # We use two tree walks, one for file search and one for Rich tree
-            # constructing, since it is difficult to compute the correct size
-            # indentation without the whole tree
-            file_tree, max_string, max_size = __construct_file_tree(
-                None, f"[bold magenta]Files & directories in project: [green]{self.project}"
-            )
 
-            tree, tree_length = __construct_rich_tree(file_tree, max_string, max_size, 0)
+        # We use two tree walks, one for file search and one for Rich tree
+        # constructing, since it is difficult to compute the correct size
+        # indentation without the whole tree
+        file_tree, max_string, max_size = __construct_file_tree(
+            None, f"[bold magenta]Files & directories in project: [green]{self.project}"
+        )
 
-            # The first header is not accounted for by the recursion
-            tree_length += 1
+        tree, tree_length = __construct_rich_tree(file_tree, max_string, max_size, 0)
 
-            # Check if the tree is too large to be printed directly
-            # and use a pager if that is the case
-            if tree_length > dds_cli.utils.console.height:
-                with dds_cli.utils.console.pager():
-                    dds_cli.utils.console.print(
-                        Padding(
-                            tree,
-                            1,
-                        )
-                    )
-            else:
+        # The first header is not accounted for by the recursion
+        tree_length += 1
+
+        # Check if the tree is too large to be printed directly
+        # and use a pager if that is the case
+        if tree_length > dds_cli.utils.console.height:
+            with dds_cli.utils.console.pager():
                 dds_cli.utils.console.print(
                     Padding(
                         tree,
                         1,
                     )
                 )
+        else:
+            dds_cli.utils.console.print(
+                Padding(
+                    tree,
+                    1,
+                )
+            )
 
-            return None
+        return None
 
     def list_users(self):
         """Get a list of user(s) involved in a project."""
         # Get user list from API
         resp_json, _ = dds_cli.utils.perform_request(
             DDSEndpoint.LIST_PROJ_USERS,
             method="get",
@@ -434,15 +434,15 @@
         }
 
         # Get lower case option
         sort_by = sort_by.lower()
 
         # Check if sorting column allowed
         if sort_by in ["usage", "cost"] and not self.show_usage:
-            LOG.warning(f"Can only sort by {sort_by} when using the --usage flag.")
+            LOG.warning("Can only sort by %s when using the --usage flag.", sort_by)
             sort_by = "updated"
 
         # Sort according to ID
         sorted_projects = sorted(projects, key=lambda i: i["Project ID"])
 
         # Sort again according to chosen of default option
         sort_by = sorting_dict.get(sort_by)
```

### Comparing `dds_cli-2.2.64/dds_cli/data_putter.py` & `dds_cli-2.2.65/dds_cli/data_putter.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import pathlib
 
 # Installed
 import boto3
 import botocore
 from rich.markup import escape
 from rich.progress import Progress, SpinnerColumn, BarColumn
-import simplejson
 
 # Own modules
 from dds_cli import base
 from dds_cli import exceptions
 from dds_cli import data_remover as dr
 from dds_cli import DDSEndpoint
 from dds_cli import file_encryptor as fe
@@ -89,15 +88,15 @@
                 upload_task = progress.add_task(
                     description="Upload",
                     total=len(putter.filehandler.data),
                 )
 
                 # Schedule the first num_threads futures for upload
                 for file in itertools.islice(iterator, num_threads):
-                    LOG.debug(f"Starting: {escape(file)}")
+                    LOG.debug("Starting: '%s'", escape(file))
                     upload_threads[
                         texec.submit(
                             putter.protect_and_upload,
                             file=file,
                             progress=progress,
                         )
                     ] = file
@@ -113,37 +112,41 @@
 
                         # Number of new upload tasks that can be started
                         new_tasks = 0
 
                         # Get result from future and schedule database update
                         for fut in done:
                             uploaded_file = upload_threads.pop(fut)
-                            LOG.debug(f"Future done for file: {escape(uploaded_file)}")
+                            LOG.debug("Future done for file: %s", escape(uploaded_file))
 
                             # Get result
                             try:
                                 file_uploaded = fut.result()
                                 LOG.debug(
-                                    f"Upload of {escape(str(uploaded_file))} successful: {file_uploaded}"
+                                    "Upload of '%s' successful: %s",
+                                    escape(str(uploaded_file)),
+                                    file_uploaded,
                                 )
                             except concurrent.futures.BrokenExecutor as err:
                                 LOG.error(
-                                    f"Upload of file {escape(uploaded_file)} failed! Error: {err}"
+                                    "Upload of file '%s' failed! Error: %s",
+                                    escape(uploaded_file),
+                                    err,
                                 )
                                 continue
 
                             # Increase the main progress bar
                             progress.advance(upload_task)
 
                             # New available threads
                             new_tasks += 1
 
                         # Schedule the next set of futures for upload
                         for next_file in itertools.islice(iterator, new_tasks):
-                            LOG.debug(f"Starting: {escape(next_file)}")
+                            LOG.debug("Starting: '%s'", escape(next_file))
                             upload_threads[
                                 texec.submit(
                                     putter.protect_and_upload,
                                     file=next_file,
                                     progress=progress,
                                 )
                             ] = next_file
@@ -246,15 +249,15 @@
             )
 
             # Remove spinner
             progress.remove_task(wait_task)
 
         if not self.filehandler.data:
             if self.temporary_directory and self.temporary_directory.is_dir():
-                LOG.debug(f"Deleting temporary folder {self.temporary_directory}.")
+                LOG.debug("Deleting temporary folder %s.", self.temporary_directory)
                 dds_cli.utils.delete_folder(self.temporary_directory)
             raise exceptions.UploadError(
                 "The specified data has already been uploaded. If you wish to redo the upload, "
                 "use the '--overwrite' flag. Please use with caution as previously uploaded data "
                 "with matching file paths will be overwritten."
             )
 
@@ -287,24 +290,26 @@
                 progress=(progress, task),
             )
 
             # Get hex version of public key -- saved in db
             file_public_key = encryptor.get_public_component_hex(private_key=encryptor.my_private)
             salt = encryptor.salt
 
-        LOG.debug(f"Updating file processed size: {file_info['path_processed']}")
+        LOG.debug("Updating file processed size: %s", file_info["path_processed"])
 
         # Update file info incl size, public key, salt
         self.filehandler.data[file]["public_key"] = file_public_key
         self.filehandler.data[file]["salt"] = salt
         self.filehandler.data[file]["size_processed"] = file_info["path_processed"].stat().st_size
 
         if saved:
             LOG.debug(
-                f"File successfully encrypted: {escape(file)}. New location: {escape(str(file_info['path_processed']))}"
+                "File successfully encrypted: '%s'. New location: '%s'",
+                escape(file),
+                escape(str(file_info["path_processed"])),
             )
             # Update progress bar for upload
             progress.reset(
                 task,
                 description=txt.TextHandler.task_name(file=escape(file), step="put"),
                 total=self.filehandler.data[file]["size_processed"],
                 step="put",
@@ -316,22 +321,23 @@
             # Perform db update
             if file_uploaded:
                 db_updated, message = self.add_file_db(file=file)
 
                 if db_updated:
                     all_ok = True
                     LOG.debug(
-                        f"File successfully uploaded and added to the database: {escape(file)}"
+                        "File successfully uploaded and added to the database: '%s'", escape(file)
                     )
 
         if not saved or all_ok:
             # Delete temporary processed file locally
             LOG.debug(
-                f"Deleting file {escape(str(file_info['path_processed']))} - "
-                f"exists: {file_info['path_processed'].exists()}"
+                "Deleting file '%s' - exists: %s",
+                escape(str(file_info["path_processed"])),
+                file_info["path_processed"].exists(),
             )
             dr.DataRemover.delete_tempfile(file=file_info["path_processed"])
 
         # Remove progress bar task
         progress.remove_task(task)
 
         return all_ok, message
@@ -369,26 +375,25 @@
             botocore.client.ClientError,
             boto3.exceptions.Boto3Error,
             botocore.exceptions.BotoCoreError,
             FileNotFoundError,
             TypeError,
         ) as err:
             error = f"S3 upload of file '{escape(file)}' failed: {err}"
-            LOG.exception(f"{escape(file)}: {err}")
+            LOG.exception("'%s': %s", escape(file), err)
         else:
             uploaded = True
 
         return uploaded, error
 
     @update_status
     def add_file_db(self, file):
         """Make API request to add file to DB."""
         # Variables
         added_to_db = False
-        error = ""
 
         # Get file info and specify info required in db
         fileinfo = self.filehandler.data[file]
         params = {"project": self.project}
         file_info = {
             "name": pathlib.Path(file),
             "name_in_bucket": fileinfo["path_remote"],
```

### Comparing `dds_cli-2.2.64/dds_cli/data_remover.py` & `dds_cli-2.2.65/dds_cli/data_remover.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,38 +72,38 @@
         not_exists = resp_json["not_exists"]
         delete_failed = resp_json["not_removed"]
 
         # Create table if any files failed
         if not_exists or delete_failed:
             if self.no_prompt:
                 self.failed_files = {"Errors": []}
-                for x in not_exists:
-                    self.failed_files["Errors"].append({x: f"No such {level.lower()}"})
-                for x, y in delete_failed.items():
-                    self.failed_files["Errors"].append({x: y})
+                for non_ex_file in not_exists:
+                    self.failed_files["Errors"].append({non_ex_file: f"No such {level.lower()}"})
+                for failed_file, failure_info in delete_failed.items():
+                    self.failed_files["Errors"].append({failed_file: failure_info})
             else:
                 # Create table and add columns
                 table = rich.table.Table(
                     title=f"{level}s not deleted",
                     title_justify="left",
                     show_header=True,
                     header_style="bold",
                 )
                 columns = [level, "Error"]
-                for x in columns:
-                    table.add_column(x)
+                for col in columns:
+                    table.add_column(col)
 
                 # Add rows
-                for x in not_exists:
-                    table.add_row(rich.markup.escape(x), f"No such {level.lower()}")
+                for non_ex_file in not_exists:
+                    table.add_row(rich.markup.escape(non_ex_file), f"No such {level.lower()}")
 
-                for x, y in delete_failed.items():
+                for failed_file, failure_info in delete_failed.items():
                     table.add_row(
-                        f"[light_salmon3]{rich.markup.escape(x)}[/light_salmon3]",
-                        f"[light_salmon3]{rich.markup.escape(y)}[/light_salmon3]",
+                        f"[light_salmon3]{rich.markup.escape(failed_file)}[/light_salmon3]",
+                        f"[light_salmon3]{rich.markup.escape(failure_info)}[/light_salmon3]",
                     )
 
                 # Print out table
                 self.failed_table = rich.padding.Padding(table, 1)
 
     @staticmethod
     def delete_tempfile(file: pathlib.Path):
@@ -160,14 +160,16 @@
             headers=self.token,
             error_message=f"Failed to delete folder(s) from project '{self.project}'",
         )
 
         self.__create_failed_table(resp_json=response_json, level="Folder")
 
         if response_json.get("nr_deleted"):
-            LOG.info(f"{response_json['nr_deleted']} files were successfully deleted in {folder}.")
+            LOG.info(
+                "%s files were successfully deleted in %s.", response_json["nr_deleted"], folder
+            )
         # Print extra warning if s3 deletion succeeded, db failed
         if response_json.get("fail_type") == "db":
             LOG.error(
                 "Some files were deleted, but their database entries were not. "
                 + "Try to run the command again, and contact Data Centre if the problem persists."
             )
```

### Comparing `dds_cli-2.2.64/dds_cli/directory.py` & `dds_cli-2.2.65/dds_cli/directory.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,18 +38,19 @@
 
         if add_file_dir:
             dirs["FILES"] = path / pathlib.Path("files/")
 
         for directory in dirs.values():
             try:
                 directory.mkdir(parents=True, exist_ok=False)
-            except OSError as e:
-                if e.errno == errno.EEXIST:
+            except OSError as err:
+                if err.errno == errno.EEXIST:
                     sys.exit(
-                        f"Directory '{rich.markup.escape(str(directory))}' already exists. Please specify a path where a new folder can be created."
+                        f"Directory '{rich.markup.escape(str(directory))}' already exists. "
+                        "Please specify a path where a new folder can be created."
                     )
                 else:
                     sys.exit(
-                        f"The temporary directory '{rich.markup.escape(str(directory))}' could not be created: {e}"
+                        f"The temporary directory '{rich.markup.escape(str(directory))}' could not be created: {err}"
                     )
 
         self.directories = dirs
```

### Comparing `dds_cli-2.2.64/dds_cli/exceptions.py` & `dds_cli-2.2.65/dds_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.64/dds_cli/file_compressor.py` & `dds_cli-2.2.65/dds_cli/file_compressor.py`

 * *Files 17% similar despite different names*

```diff
@@ -70,17 +70,17 @@
             b"(\xb5/\xfd": "zst",
         }
         self.max_magic_len = max(len(x) for x in self.fmt_magic)
 
     def __enter__(self):
         return self
 
-    def __exit__(self, exc_type, exc_value, tb):
+    def __exit__(self, exc_type, exc_val, traceb):
         if exc_type is not None:
-            traceback.print_exception(exc_type, exc_value, tb)
+            traceback.print_exception(exc_type, exc_val, traceb)
             return False  # uncomment to pass exception through
 
         return True
 
     # Static methods ###################### Static methods #
     @staticmethod
     def compress_file(
@@ -103,15 +103,15 @@
                     #     chunk = compressor.read(chunk_size)
                     #     LOG.debug(type(chunk))
                     #     if not chunk:
                     #         break
                     #     yield
                     for chunk in iter(lambda: compressor.read(chunk_size), b""):
                         yield chunk
-        except Exception as err:
+        except Exception as err:  # pylint: disable=broad-exception-caught
             LOG.warning(str(err))
         else:
             LOG.debug("Compression finished.")
 
     @staticmethod
     def decompress_filechunks(chunks, outfile: pathlib.Path, **_):
         """Decompress file chunks"""
@@ -138,15 +138,15 @@
 
     # Public methods ###################### Public methods #
     def is_compressed(self, file):
         """Checks if a file is compressed or not."""
 
         compressed, error = (False, "")
         try:
-            with file.open(mode="rb") as f:
-                file_start = f.read(self.max_magic_len)
+            with file.open(mode="rb") as file_obj:
+                file_start = file_obj.read(self.max_magic_len)
                 if file_start.startswith(tuple(x for x in self.fmt_magic)):
                     compressed = True
         except OSError as err:
             error = str(err)
 
         return compressed, error
```

### Comparing `dds_cli-2.2.64/dds_cli/file_encryptor.py` & `dds_cli-2.2.65/dds_cli/file_encryptor.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             algorithm=hashes.SHA256(),
             length=32,
             salt=salt,
             info=b"",
             backend=backends.default_backend(),
         ).derive(shared_key)
 
-        LOG.debug(f"Salt: {salt}")
+        LOG.debug("Salt: %s", salt)
         return derived_shared_key, salt.hex().upper()
 
     @staticmethod
     def public_to_hex(public_key: x25519.X25519PublicKey):
         """Converts public key to hexstring."""
 
         # public = self.private.public_key()
@@ -104,17 +104,17 @@
         self.key, self.salt = self.generate_shared_key(
             my_private=self.my_private, peer_public=self.peer_public
         )
 
     def __enter__(self):
         return self
 
-    def __exit__(self, exc_type, exc_value, tb):
+    def __exit__(self, exc_type, exc_value, traceb):
         if exc_type is not None:
-            traceback.print_exception(exc_type, exc_value, tb)
+            traceback.print_exception(exc_type, exc_value, traceb)
             return False  # uncomment to pass exception through
 
         return True
 
     # Static methods ###################### Static methods #
     @staticmethod
     def verify_checksum(file: pathlib.Path, correct_checksum):
@@ -208,17 +208,17 @@
             peer_public=self.peer_public,
             salt=bytes.fromhex(key_salt),
         )
 
     def __enter__(self):
         return self
 
-    def __exit__(self, exc_type, exc_value, tb):
+    def __exit__(self, exc_type, exc_value, traceb):
         if exc_type is not None:
-            traceback.print_exception(exc_type, exc_value, tb)
+            traceback.print_exception(exc_type, exc_value, traceb)
             return False  # uncomment to pass exception through
 
         return True
 
     # Public methods ###################### Public methods #
     def decrypt_file(self, infile: pathlib.Path):
         """Decrypts the file"""
@@ -257,10 +257,10 @@
                     yield crypto_aead_chacha20poly1305_ietf_decrypt(
                         ciphertext=chunk, aad=aad, nonce=nonce, key=self.key
                     )
 
                 LOG.debug("Testing nonce...")
                 if last_nonce != nonce:
                     raise SystemExit("Nonces do not match!!")
-                LOG.debug(f"Last nonce should be: {last_nonce}, was: {nonce}")
-        except Exception as err:
+                LOG.debug("Last nonce should be: %s, was: %s", last_nonce, nonce)
+        except Exception as err:  # pylint: disable=broad-exception-caught
             LOG.warning(str(err))
```

### Comparing `dds_cli-2.2.64/dds_cli/file_handler.py` & `dds_cli-2.2.65/dds_cli/file_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 ###############################################################################
 # IMPORTS ########################################################### IMPORTS #
 ###############################################################################
 
 # Standard library
 import json
 import logging
-import os
 import pathlib
 import threading
 
 # Installed
 
 # Own modules
 import dds_cli.utils
@@ -88,19 +87,19 @@
         ok_to_remove = False
 
         # If file not ok to remove folder
         if not directory.is_dir():
             return ok_to_remove
 
         # Iterate through any existing subdirectories - recursive
-        LOG.debug(f"Any in directory? {any(directory.iterdir())}")
+        LOG.debug("Any in directory? %s", any(directory.iterdir()))
         if any(directory.iterdir()):
-            for p in directory.iterdir():
-                if p.is_dir():
-                    ok_to_remove = FileHandler.delete_tempdir(directory=p)
+            for item in directory.iterdir():
+                if item.is_dir():
+                    ok_to_remove = FileHandler.delete_tempdir(directory=item)
                     if ok_to_remove:
                         directory.rmdir()
         else:
             directory.rmdir()
             ok_to_remove = True
 
         return ok_to_remove
```

### Comparing `dds_cli-2.2.64/dds_cli/file_handler_local.py` & `dds_cli-2.2.65/dds_cli/file_handler_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 ###############################################################################
 # IMPORTS ########################################################### IMPORTS #
 ###############################################################################
 
 # Standard library
 import hashlib
-import http
 import logging
 import os
 import pathlib
 import typing
 import uuid
 import random
 
@@ -50,17 +49,17 @@
         # Remove non existent files
         self.data_list = {x for x in self.data_list if x.exists()}
 
         non_existent_files = all_files.difference(self.data_list)
         if len(non_existent_files) > 0:
             # Issue warning that some of the files don't exist
             LOG.warning(
-                "The following files from '{}' does not exist: '{}'".format(
-                    user_input[1], "', '".join([str(x) for x in non_existent_files])
-                )
+                "The following files from '%s' does not exist: '%s'",
+                user_input[1],
+                "', '".join([str(x) for x in non_existent_files]),
             )
 
         # Get absolute paths for all data
         # os.path.expanduser(path): e.g. C:\Users\inaod568/repos/dds_cli
         # path.expanduser(), pathlib.Path: e.g. C:\Users\inaod568\repos\dds_cli
         self.data_list = [
             pathlib.Path(os.path.abspath(path.expanduser())) for path in self.data_list
@@ -79,15 +78,15 @@
     # Static methods ############## Static methods #
     @staticmethod
     def generate_bucket_filepath(filename="", folder=pathlib.Path("")):
         """Generates filename and new path which the file will be
         called in the bucket."""
 
         # Generate new file name
-        new_name = f"{'%020x' % random.randrange(16**20)}_{uuid.uuid5(uuid.NAMESPACE_X500, str(folder))}{uuid.uuid5(uuid.NAMESPACE_X500, filename)}"
+        new_name = f"{'%020x' % random.randrange(16**20)}_{uuid.uuid5(uuid.NAMESPACE_X500, str(folder))}{uuid.uuid5(uuid.NAMESPACE_X500, filename)}"  # pylint: disable=line-too-long,consider-using-f-string
         return new_name
 
     @staticmethod
     def read_file(file, chunk_size: int = FileSegment.SEGMENT_SIZE_RAW):
         """Read file in chunk_size sized chunks."""
 
         try:
@@ -97,16 +96,16 @@
         except OSError as err:
             LOG.warning(str(err))
 
     # Private methods ############ Private methods #
     def __collect_file_info_local(self, all_paths, folder=pathlib.Path(""), task_name=""):
         """Get info on each file in each path specified."""
         # Variables
-        file_info: typing.Dict = dict()
-        progress_tasks: typing.Dict = dict()
+        file_info: typing.Dict = {}
+        progress_tasks: typing.Dict = {}
 
         # Iterate though paths
         for path in all_paths:
             # Choose name for progress bar - unused?
             task_name = path.name if folder == pathlib.Path("") else task_name
             path_key = folder / path.name
             # Get info for all files
@@ -151,55 +150,58 @@
             else:
                 # Symlinks are also identified as files - if here and symlink --> broken
                 if path.is_symlink():
                     try:
                         resolved = path.resolve()
                     except RuntimeError:
                         LOG.warning(
-                            f"IGNORED: Link: {path} seems to contain infinite loop, will be ignored."
+                            "IGNORED: Link: '%s' seems to contain infinite loop, will be ignored.",
+                            path,
                         )
                     else:
                         LOG.warning(
-                            f"IGNORED: Link: {path} -> {resolved} seems to be broken, will be ignored."
+                            "IGNORED: Link: '%s' -> '%s' seems to be broken, will be ignored.",
+                            path,
+                            resolved,
                         )
                 else:
                     LOG.warning(
-                        f"IGNORED: Path of unsupported/unknown type: {path}, will be ignored."
+                        "IGNORED: Path of unsupported/unknown type: '%s', will be ignored.", path
                     )
 
         return file_info, progress_tasks
 
     # Public methods ############## Public methods #
     def create_upload_status_dict(self, existing_files, overwrite=False):
         """Create dict for tracking file delivery status"""
 
         LOG.debug("Creating the status dictionary.")
 
         status_dict = {}
-        for x in list(self.data):
-            in_db = bool(x in existing_files)
+        for item in list(self.data):
+            in_db = bool(item in existing_files)
             if in_db and not overwrite:
-                self.failed[x] = {
-                    **self.data.pop(x),
+                self.failed[item] = {
+                    **self.data.pop(item),
                     **{"message": "File already uploaded"},
                 }
             else:
                 if in_db:
                     if overwrite:
-                        self.data[x].update(
+                        self.data[item].update(
                             {
                                 "overwrite": True,
-                                "path_remote": existing_files[x],
+                                "path_remote": existing_files[item],
                             }
                         )
 
                 # filestream_funcname = (
                 #     "read_file" if self.data[x]["compressed"] else "compress_file"
                 # )
-                status_dict[x] = {
+                status_dict[item] = {
                     "cancel": False,
                     "started": False,
                     "message": "",
                     "failed_op": None,
                     # filestream_funcname: {"started": False, "done": False},
                     "put": {"started": False, "done": False},
                     "add_file_db": {"started": False, "done": False},
@@ -226,15 +228,15 @@
         )
         # API failure
         if "files" not in files_in_db:
             raise exceptions.NoDataError("Files not returned from API.")
 
         LOG.debug("Previous upload check finished.")
 
-        return dict() if files_in_db["files"] is None else files_in_db["files"]
+        return {} if files_in_db["files"] is None else files_in_db["files"]
 
     def create_encrypted_name(
         self, raw_file: pathlib.Path, subpath: str = pathlib.Path(""), no_compression: bool = True
     ):
         """Create new file name to save encrypted file."""
 
         # New local file name
```

### Comparing `dds_cli-2.2.64/dds_cli/file_handler_remote.py` & `dds_cli-2.2.65/dds_cli/file_handler_remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 ###############################################################################
 
 # Standard library
 import logging
 import pathlib
 
 # Installed
-import simplejson
 
 # Own modules
 from dds_cli import DDSEndpoint
 from dds_cli import file_handler as fh
 import dds_cli.utils
 
 ###############################################################################
@@ -93,15 +92,15 @@
         # Cancel download of those files or folders not found in the db
         self.failed = {
             x: {"error": "Not found in DB."}
             for x in all_paths
             if x not in files and x not in folder_contents
         }
 
-        LOG.debug(f"Not found: {self.failed}")
+        LOG.debug("Not found: %s", self.failed)
 
         # Save info on files in dict and return
         data = {
             self.local_destination
             / pathlib.Path(x): {
                 **y,
                 "name_in_db": x,
@@ -109,26 +108,26 @@
                 / pathlib.Path(y["subpath"])
                 / pathlib.Path(y["name_in_bucket"]),
             }
             for x, y in files.items()
         }
 
         # Save info on files in a specific folder and return
-        for x, y in folder_contents.items():
+        for _, folder_item in folder_contents.items():
             data.update(
                 {
                     self.local_destination
                     / pathlib.Path(j): {
                         **k,
                         "name_in_db": j,
                         "path_downloaded": self.local_destination
                         / pathlib.Path(k["subpath"])
                         / pathlib.Path(k["name_in_bucket"]),
                     }
-                    for j, k in y.items()
+                    for j, k in folder_item.items()
                 }
             )
 
         return data
 
     # Public methods ############ Public methods #
     def create_download_status_dict(self):
```

### Comparing `dds_cli-2.2.64/dds_cli/maintenance_manager.py` & `dds_cli-2.2.65/dds_cli/maintenance_manager.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.64/dds_cli/motd_manager.py` & `dds_cli-2.2.65/dds_cli/motd_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,19 +4,14 @@
 # IMPORTS ################################################################################ IMPORTS #
 ###################################################################################################
 
 # Standard library
 import logging
 
 # Installed
-import http
-import requests
-import rich.markup
-from rich.table import Table
-import simplejson
 
 # Own modules
 import dds_cli
 import dds_cli.auth
 import dds_cli.base
 import dds_cli.exceptions
 import dds_cli.utils
@@ -72,23 +67,23 @@
 
         response_message = response_json.get(
             "message", "No response. Cannot confirm MOTD creation."
         )
         LOG.info(response_message)
 
     @staticmethod
-    def list_all_active_motds(table=False):
+    def list_all_active_motds(table=False):  # pylint: disable=inconsistent-return-statements
         """Get all active MOTDs."""
         try:
             response, _ = dds_cli.utils.perform_request(
                 endpoint=dds_cli.DDSEndpoint.MOTD,
                 method="get",
                 error_message="Failed getting MOTDs from API",
             )
-        except:
+        except:  # pylint: disable=bare-except
             pass
         else:
             # Get items from response
             motd = response.get("motds")
             if not motd:
                 message = response.get("message", "No motds or info message returned from API.")
                 LOG.info(message)
```

### Comparing `dds_cli-2.2.64/dds_cli/options.py` & `dds_cli-2.2.65/dds_cli/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Click DDS options used multiple times in __main__.py."""
 
 # Imports
-import click
 import pathlib
+import click
 from dds_cli.utils import multiple_help_text
 
 
 # Args used multiple times
 def email_arg(required, email="email", metavar="[EMAIL]", nargs=1):
     """
     Email positional argument standard definition.
@@ -18,14 +18,18 @@
 
 # Options used multiple times
 
 
 def destination_option(
     help_message, option_type, long="--destination", short="-d", name="destination", required=False
 ):
+    """Destination option standard definition.
+
+    Use as decorator for commands.
+    """
     return click.option(
         long,
         short,
         name,
         required=required,
         type=option_type,
         multiple=False,
@@ -184,15 +188,18 @@
 
 
 def token_path_option(
     long="--token-path",
     short="-tp",
     name="token_path",
     required=False,
-    help_message="The path where the authentication token will be stored. For a normal use-case, this should not be needed.",
+    help_message=(
+        "The path where the authentication token will be stored. "
+        "For a normal use-case, this should not be needed."
+    ),
 ):
     """
     token path option standard definition.
 
     Use as decorator for commands.
     """
     return click.option(
```

### Comparing `dds_cli-2.2.64/dds_cli/project_creator.py` & `dds_cli-2.2.65/dds_cli/project_creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Data Delivery System Project Creator."""
 import logging
 
 # Installed
-import dds_cli
-import dds_cli.utils
 import rich.prompt
 
 # Own modules
+import dds_cli
+import dds_cli.utils
 from dds_cli import base
 from dds_cli import exceptions
-from dds_cli import utils
 from dds_cli import DDSEndpoint
 
 ###############################################################################
 # START LOGGING CONFIG ################################# START LOGGING CONFIG #
 ###############################################################################
 
 LOG = logging.getLogger(__name__)
@@ -69,15 +68,15 @@
         )
 
         warning_message = response_json.get("warning")
 
         if warning_message:
             if self.no_prompt:
                 LOG.warning(
-                    f"{warning_message}\n\n`--no-prompt` option used: Not creating project."
+                    "%s\n\n`--no-prompt` option used: Not creating project.", warning_message
                 )
                 proceed_creation = False
             else:
                 proceed_creation = rich.prompt.Confirm.ask(
                     f"[red][bold]WARNING!![/bold][/red] {warning_message}"
                     "\n\nAre you sure you wish to create this project anyway?"
                 )
```

### Comparing `dds_cli-2.2.64/dds_cli/project_info.py` & `dds_cli-2.2.65/dds_cli/project_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 """Data Delivery System Project info manager."""
+# Standard library
 import logging
+import sys
 
 # Installed
-import requests
-import simplejson
-import pytz
-import tzlocal
-import datetime
 import rich
-import sys
+
 
 # Own modules
 from dds_cli import base
 from dds_cli import exceptions
 from dds_cli import DDSEndpoint
 import dds_cli.utils
 
@@ -44,14 +41,15 @@
             method_check=False,
             token_path=token_path,
         )
         self.project = project
 
     # Public methods ###################### Public methods #
     def get_project_info(self):
+        """Collect project information from API."""
         # Get info about a project from API
         response, _ = dds_cli.utils.perform_request(
             DDSEndpoint.PROJ_INFO,
             method="get",
             headers=self.token,
             params={"project": self.project},
             error_message="Failed to get project information",
@@ -79,48 +77,58 @@
         )
         dds_cli.utils.console.print(table)
 
         # Print Title and Description below the table
         dds_cli.utils.console.print(f"[b]Project title:[/b]       {project_info['Title']}")
         dds_cli.utils.console.print(f"[b]Project description:[/b] {project_info['Description']}")
 
-    def update_info(self, title=None, description=None, pi=None):
+    def update_info(self, title=None, description=None, pi=None):  # pylint: disable=invalid-name
         """Update project info"""
 
         if all(item is None for item in [title, description, pi]):
             raise exceptions.NoDataError(
-                "Please specify which information you would like to change: '--title', '--description' or/and '--principal-investigator'."
+                "Please specify which information you would like to change: '--title', "
+                "'--description' or/and '--principal-investigator'."
             )
 
         # Get project info from API
         project_info = self.get_project_info()
 
         # Collect the items for change and ask for confirmation for each of them
         info_items = {}
         if title:
             info_items["title"] = title
             # Ask the user for confirmation
             if not rich.prompt.Confirm.ask(
-                f"You are about to change the [i]title[/i] for project '[b]{self.project}[/b]' \n[b][blue]from[/blue][/b]\t{project_info['Title']}\n[b][green]to[/green][/b]\t{info_items['title']} \nAre you sure?"
+                f"You are about to change the [i]title[/i] for project '[b]{self.project}[/b]'\n"
+                f"[b][blue]from[/blue][/b]\t{project_info['Title']}\n"
+                f"[b][green]to[/green][/b]\t{info_items['title']}\n"
+                "Are you sure?"
             ):
                 LOG.info("Probably for the best. Exiting.")
                 sys.exit(0)
         if description:
             info_items["description"] = description
             # Ask the user for confirmation
             if not rich.prompt.Confirm.ask(
-                f"You are about to change the [i]description[/i] for project '[b]{self.project}[/b]' \n[b][blue]from[/blue][/b]\t{project_info['Description']}\n[b][green]to[/green][/b]\t{info_items['description']} \nAre you sure?"
+                f"You are about to change the [i]description[/i] for project '[b]{self.project}[/b]' \n"
+                f"[b][blue]from[/blue][/b]\t{project_info['Description']}\n"
+                f"[b][green]to[/green][/b]\t{info_items['description']} \n"
+                "Are you sure?"
             ):
                 LOG.info("Probably for the best. Exiting.")
                 sys.exit(0)
         if pi:
             info_items["pi"] = pi
             # Ask the user for confirmation
             if not rich.prompt.Confirm.ask(
-                f"You are about to change the [i]PI[/i] for project '[b]{self.project}[/b]' \n[b][blue]from[/blue][/b]\t{project_info['PI']}\n[b][green]to[/green][/b]\t{info_items['pi']} \nAre you sure?"
+                f"You are about to change the [i]PI[/i] for project '[b]{self.project}[/b]' \n"
+                f"[b][blue]from[/blue][/b]\t{project_info['PI']}\n"
+                f"[b][green]to[/green][/b]\t{info_items['pi']} \n"
+                "Are you sure?"
             ):
                 LOG.info("Probably for the best. Exiting.")
                 sys.exit(0)
 
         # Run the request
         response_json, _ = dds_cli.utils.perform_request(
             endpoint=DDSEndpoint.PROJ_INFO,
```

### Comparing `dds_cli-2.2.64/dds_cli/project_status.py` & `dds_cli-2.2.65/dds_cli/project_status.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Data Delivery System Project Status manager."""
+import datetime
 import logging
+import typing
 
 # Installed
-import requests
-import simplejson
 import pytz
 import tzlocal
-import datetime
 
 # Own modules
 from dds_cli import base
 from dds_cli import exceptions
 from dds_cli import DDSEndpoint
 import dds_cli.utils
 
@@ -62,39 +61,39 @@
         status_out = f"Current status of {self.project}: {current_status}"
         deadline_out = ""
         if current_deadline:
             try:
                 date = pytz.timezone("UTC").localize(
                     datetime.datetime.strptime(current_deadline, "%a, %d %b %Y %H:%M:%S GMT")
                 )
-            except ValueError as err:
+            except ValueError as exc:
                 raise exceptions.ApiResponseError(
                     f"Time zone mismatch: Incorrect zone '{current_deadline.split()[-1]}'"
-                )
-            else:
-                current_deadline = date.astimezone(tzlocal.get_localzone()).strftime(
-                    "%a, %d %b %Y %H:%M:%S %Z"
-                )
+                ) from exc
+
+            current_deadline = date.astimezone(tzlocal.get_localzone()).strftime(
+                "%a, %d %b %Y %H:%M:%S %Z"
+            )
             deadline_out = f" with deadline {current_deadline}"
         dds_cli.utils.console.print(f"{status_out}{deadline_out}")
         if show_history:
             history = "Status history \n"
             for row in resp_json.get("history"):
                 try:
                     date = pytz.timezone("UTC").localize(
                         datetime.datetime.strptime(row[1], "%a, %d %b %Y %H:%M:%S GMT")
                     )
-                except ValueError as err:
+                except ValueError as exc:
                     raise exceptions.ApiResponseError(
                         f"Time zone mismatch: Incorrect zone '{row[1].split()[-1]}'"
-                    )
-                else:
-                    row[1] = date.astimezone(tzlocal.get_localzone()).strftime(
-                        "%a, %d %b %Y %H:%M:%S %Z"
-                    )
+                    ) from exc
+
+                row[1] = date.astimezone(tzlocal.get_localzone()).strftime(
+                    "%a, %d %b %Y %H:%M:%S %Z"
+                )
                 history += ", ".join(list(row)) + " \n"
             LOG.info(history)
 
     def update_status(self, new_status, deadline=None, is_aborted=False, no_mail=False):
         """Update project status"""
 
         extra_params = {"new_status": new_status, "send_email": not no_mail}
@@ -145,15 +144,15 @@
 
         num_busy: int = response_json.get("num")
         if num_busy is None:
             raise exceptions.ApiResponseError("No info about busy projects returned from API.")
 
         if num_busy:
             if not show:
-                LOG.info(f"There are {num_busy} busy projects at the moment.")
+                LOG.info("There are %s busy projects at the moment.", num_busy)
             else:
                 projects: typing.Dict = response_json.get("projects")
-                LOG.info(f"The following projects are busy:")
-                for p in projects:
-                    dds_cli.utils.console.print(f"{p}: updated on {projects[p]}")
+                LOG.info("The following projects are busy:")
+                for proj in projects:
+                    dds_cli.utils.console.print(f"{proj}: updated on {projects[proj]}")
         else:
-            LOG.info(f"There are no busy projects at the moment.")
+            LOG.info("There are no busy projects at the moment.")
```

### Comparing `dds_cli-2.2.64/dds_cli/s3_connector.py` & `dds_cli-2.2.65/dds_cli/s3_connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # Installed
 import boto3
 import botocore
 
 # Own modules
 import dds_cli.utils
 from dds_cli import DDSEndpoint
-from dds_cli import exceptions
 
 ###############################################################################
 # LOGGING ########################################################### LOGGING #
 ###############################################################################
 
 LOG = logging.getLogger(__name__)
 
@@ -53,18 +52,18 @@
     # @connect_cloud
     def __enter__(self):
         """Enter context."""
         self.resource = self.connect()
 
         return self
 
-    def __exit__(self, exc_type, exc_value, tb):
+    def __exit__(self, exc_type, exc_value, traceb):
         """Close context manager, incl. connection."""
         if exc_type is not None:
-            traceback.print_exception(exc_type, exc_value, tb)
+            traceback.print_exception(exc_type, exc_value, traceb)
             return False  # uncomment to pass exception through
 
         return True
 
     def connect(self):
         """Connect to S3 resource."""
         # Connect to service
@@ -74,18 +73,18 @@
             resource = session.resource(
                 service_name="s3",
                 endpoint_url=self.url,
                 aws_access_key_id=self.keys["access_key"],
                 aws_secret_access_key=self.keys["secret_key"],
             )
         except (boto3.exceptions.Boto3Error, botocore.exceptions.BotoCoreError) as err:
-            LOG.warning(f"S3 connection failed: {err}")
+            LOG.warning("S3 connection failed: %s", err)
             raise
-        else:
-            LOG.debug(f"Connected to S3.")
+
+        LOG.debug("Connected to S3.")
         return resource
 
     # Static methods ############ Static methods #
     @staticmethod
     def __get_s3_info(project_id, token):
         """Get information required to connect to cloud."""
         # Perform request to API
```

### Comparing `dds_cli-2.2.64/dds_cli/status.py` & `dds_cli-2.2.65/dds_cli/status.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         """Cancel upload all files."""
 
     @classmethod
     def cancel_one(cls):
         """Cancel the failed file."""
 
 
-class ProgressPercentage(object):
+class ProgressPercentage:
     """Updates the progress bar with the callback from boto3."""
 
     def __init__(self, progress, task):
         """Keep track of progress."""
         self.progress = progress
         self.task = task
```

### Comparing `dds_cli-2.2.64/dds_cli/text_handler.py` & `dds_cli-2.2.65/dds_cli/text_handler.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.64/dds_cli/timestamp.py` & `dds_cli-2.2.65/dds_cli/timestamp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""""""
+"""Timestamp module."""
 
 
 ###############################################################################
 # IMPORTS ########################################################### IMPORTS #
 ###############################################################################
 
 # Standard library
@@ -21,31 +21,33 @@
 
 ###############################################################################
 # CLASSES ########################################################### CLASSES #
 ###############################################################################
 
 
 class TimeStamp:
+    """Timestamp object."""
+
     def __init__(self):
         self.sep_date_time = "_"
         self.sep_time = "-"
 
         now = datetime.datetime.now()
         self.timestamp = ""
 
-        for t in (
+        for time_part in (
             now.year,
             self.sep_time,
             now.month,
             self.sep_time,
             now.day,
             self.sep_date_time,
             now.hour,
             self.sep_time,
             now.minute,
             self.sep_time,
             now.second,
         ):
-            if len(str(t)) == 1 and isinstance(t, int):
-                self.timestamp += f"0{t}"
+            if len(str(time_part)) == 1 and isinstance(time_part, int):
+                self.timestamp += f"0{time_part}"
             else:
-                self.timestamp += f"{t}"
+                self.timestamp += f"{time_part}"
```

### Comparing `dds_cli-2.2.64/dds_cli/unit_manager.py` & `dds_cli-2.2.65/dds_cli/unit_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,14 @@
 # IMPORTS ################################################################################ IMPORTS #
 ###################################################################################################
 
 # Standard library
 import logging
 
 # Installed
-import http
-import requests
-import rich.markup
-from rich.table import Table
-import simplejson
 
 # Own modules
 import dds_cli
 import dds_cli.auth
 import dds_cli.base
 import dds_cli.exceptions
 import dds_cli.utils
```

### Comparing `dds_cli-2.2.64/dds_cli/user.py` & `dds_cli-2.2.65/dds_cli/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,19 @@
 
 # Standard library
 import datetime
 import getpass
 import logging
 import os
 import pathlib
-import requests
-import simplejson
 import stat
 import subprocess
 
 # Installed
-import rich
+from rich.prompt import Prompt
 
 # Own modules
 import dds_cli
 from dds_cli import exceptions
 from dds_cli.utils import get_token_expiration_time, readable_timedelta
 import dds_cli.utils
 
@@ -95,86 +93,89 @@
             raise exceptions.AuthenticationError(
                 message=(
                     "Authentication not possible when running with --no-prompt. "
                     "Please run the `dds auth login` command and authenticate interactively."
                 )
             )
 
-        username = rich.prompt.Prompt.ask("DDS username")
+        username = Prompt.ask("DDS username")
         password = getpass.getpass(prompt="DDS password: ")
 
         if password == "":
             raise exceptions.AuthenticationError(
                 message="Non-empty password needed to be able to authenticate."
             )
 
         try:
             response_json, _ = dds_cli.utils.perform_request(
                 dds_cli.DDSEndpoint.ENCRYPTED_TOKEN,
                 method="get",
                 auth=(username, password),
                 error_message="Failed to authenticate user",
             )
-        except UnicodeEncodeError as err:
+        except UnicodeEncodeError as exc:
             raise dds_cli.exceptions.ApiRequestError(
                 message="The entered username or password seems to contain invalid characters. Please try again."
-            )
+            ) from exc
 
         # Token received from API needs to be completed with a mfa timestamp
         partial_auth_token = response_json.get("token")
         secondfactor_method = response_json.get("secondfactor_method")
 
         totp_enabled = secondfactor_method == "TOTP"
 
         # Verify Second Factor
         if totp:
             if not totp_enabled:
                 raise exceptions.AuthenticationError(
-                    "Authentication failed, you have not yet activated one-time authentication codes from authenticator app."
+                    "Authentication failed, you have not yet activated one-time "
+                    "authentication codes from authenticator app."
                 )
 
             response_json, _ = dds_cli.utils.perform_request(
                 dds_cli.DDSEndpoint.SECOND_FACTOR,
                 method="get",
                 headers={"Authorization": f"Bearer {partial_auth_token}"},
                 json={"TOTP": totp},
                 error_message="Failed to authenticate with one-time authentication code",
             )
 
         else:
-            LOG.debug(f"2FA method: {'TOTP' if totp_enabled else 'HOTP'}")
+            LOG.debug("2FA method: %s", "TOTP" if totp_enabled else "HOTP")
             if totp_enabled:
                 LOG.info(
                     "Please enter the one-time authentication code from your authenticator app."
                 )
                 nr_digits = 6
             else:
                 LOG.info(
                     "Please enter the one-time authentication code sent "
                     "to your email address (leave empty to exit):"
                 )
                 nr_digits = 8
 
             done = False
             while not done:
-                entered_one_time_code = rich.prompt.Prompt.ask("Authentication one-time code")
+                entered_one_time_code = Prompt.ask("Authentication one-time code")
                 if entered_one_time_code == "":
                     raise exceptions.AuthenticationError(
                         message="Exited due to no one-time authentication code entered."
                     )
 
                 if not entered_one_time_code.isdigit():
                     LOG.info(
                         "Please enter a valid one-time code. It should consist of only digits."
                     )
                     continue
                 if len(entered_one_time_code) != nr_digits:
                     LOG.info(
-                        f"Please enter a valid one-time code. It should consist of {nr_digits} digits "
-                        f"(you entered {len(entered_one_time_code)} digits)."
+                        "Please enter a valid one-time code. It should consist of %s digits "
+                        "(you entered %s digits).",
+                        nr_digits,
+                        len(entered_one_time_code),
                     )
                     continue
 
                 if totp_enabled:
                     json_request = {"TOTP": entered_one_time_code}
                 else:
                     json_request = {"HOTP": entered_one_time_code}
@@ -193,15 +194,15 @@
         # Get token from response
         token = response_json.get("token")
         if not token:
             raise exceptions.AuthenticationError(
                 message="Missing token in authentication response."
             )
 
-        LOG.debug(f"User {username} granted access to the DDS")
+        LOG.debug("User %s granted access to the DDS", username)
 
         return token
 
     @staticmethod
     def get_user_name_if_logged_in(token_path=None):
         """Returns a user name if logged in, otherwise None"""
 
@@ -215,15 +216,15 @@
                         dds_cli.DDSEndpoint.DISPLAY_USER_INFO,
                         method="get",
                         headers={"Authorization": f"Bearer {token}"},
                         error_message="Failed to get a username",
                     )
                     # Get response
                     username = response_json["info"]["username"]
-                except:
+                except:  # pylint: disable=bare-except
                     pass
         return username
 
 
 class TokenFile:
     """A class to manage the saved token."""
 
@@ -241,22 +242,23 @@
         Returns None if no valid token can be found.
 
         Debug, not warning. Run prior to logging configured.
         """
         LOG.debug("Attempting to retrieve token from file...")
 
         if not self.file_exists():
-            LOG.debug(f"Token file {self.token_file} does not exist.")
+            LOG.debug("Token file %s does not exist.", self.token_file)
             return None
 
         self.check_token_file_permissions()
 
         # Read token from file
-        with self.token_file.open(mode="r") as file:
+        with self.token_file.open(mode="r") as file:  # pylint: disable=unspecified-encoding
             token = file.read()
+            LOG.debug(type(token))
             if not token:
                 raise exceptions.TokenNotFoundError(message="Token file is empty.")
 
         if self.token_expired(token=token):
             LOG.debug("The token has expired, reauthentication required.")
             return None
 
@@ -271,15 +273,15 @@
         """Saves the token to the token file."""
 
         if not self.token_file.is_file():
             self.token_file.touch(mode=self.token_permission)
 
         self.check_token_file_permissions()
 
-        with self.token_file.open("w") as file:
+        with self.token_file.open("w") as file:  # pylint: disable=unspecified-encoding
             file.write(token)
 
         if os.name == "nt":
             cli_username = os.environ.get("USERNAME")
             try:
                 subprocess.check_call(
                     [
@@ -288,15 +290,15 @@
                         "/inheritance:r",
                         "/grant",
                         f"{cli_username}:(R,W)",
                     ],
                     stdout=subprocess.DEVNULL,
                     stderr=subprocess.DEVNULL,
                 )
-            except subprocess.CalledProcessError as exc:
+            except subprocess.CalledProcessError:
                 LOG.error("Failed to set token file permissions")
         LOG.debug("New token saved to file.")
 
     def delete_token(self):
         """Deletes the token file."""
 
         if self.file_exists():
@@ -310,19 +312,24 @@
         """
         if os.name != "nt":
             st_mode = os.stat(self.token_file).st_mode
             permissions_octal = oct(stat.S_IMODE(st_mode))
             permissions_readable = stat.filemode(st_mode)
             if permissions_octal not in ["0o600", "0o640"]:
                 raise exceptions.DDSCLIException(
-                    message=f"Token file permissions are not properly set, (got {permissions_readable} instead of required '-rw-------'). Please remove {self.token_file} and rerun the command."
+                    message=(
+                        f"Token file permissions are not properly set, (got {permissions_readable} "
+                        f"instead of required '-rw-------'). Please remove {self.token_file} and rerun the command."
+                    )
                 )
         else:
             LOG.info(
-                f"Storing the login information locally - please ensure no one else an access the file at {self.token_file}."
+                "Storing the login information locally - "
+                "please ensure no one else an access the file at '%s'.",
+                self.token_file,
             )
 
     def token_expired(self, token):
         """Check if the token has expired or is about to expire soon based on the UTC time.
 
         :param token: The DDS token that is obtained after successful basic and two-factor authentication.
             Token is already obtained before coming here, so not expected to be None.
@@ -332,18 +339,20 @@
         expiration_time = self.__token_dates(token=token)
         time_to_expire = expiration_time - datetime.datetime.utcnow()
 
         if expiration_time <= datetime.datetime.utcnow():
             LOG.debug("Token has expired. Now deleting it and fetching new token.")
             self.delete_token()
             return True
-        elif time_to_expire < dds_cli.TOKEN_EXPIRATION_WARNING_THRESHOLD:
+
+        if time_to_expire < dds_cli.TOKEN_EXPIRATION_WARNING_THRESHOLD:
             LOG.warning(
-                f"Saved token will expire in {readable_timedelta(time_to_expire)}, "
-                f"please consider renewing the session using the 'dds auth login' command."
+                "Saved token will expire in %s, "
+                "please consider renewing the session using the 'dds auth login' command.",
+                readable_timedelta(time_to_expire),
             )
 
         return False
 
     def token_report(self, token):
         """Produce report of token status.
 
@@ -365,18 +374,18 @@
             message = ""
         else:
             markup_color = "green"
             sign = ":white_check_mark:"
             message = "Token is OK!"
 
         if message:
-            LOG.info(f"[{markup_color}]{sign}  {message} {sign} [/{markup_color}]")
-        LOG.info(f"[{markup_color}]{sign}  {expiration_message} {sign} [/{markup_color}]")
+            LOG.info("[%s]%s  %s %s [/%s]", markup_color, sign, message, sign, markup_color)
+        LOG.info("[%s]%s  %s %s [/%s]", markup_color, sign, expiration_message, sign, markup_color)
 
     # Private methods ############################################################ Private methods #
-    def __token_dates(self, token):
+    def __token_dates(self, token):  # pylint: disable=inconsistent-return-statements
         """Returns the expiration time in UTC that is extracted from the token jose header."""
 
         expiration_time = get_token_expiration_time(token=token)
 
         if expiration_time:
             return datetime.datetime.fromisoformat(expiration_time)
```

### Comparing `dds_cli-2.2.64/dds_cli/utils.py` & `dds_cli-2.2.65/dds_cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """DDS CLI utils module."""
 
-import logging
 import numbers
 import pathlib
 import typing
+import http
+from typing import Dict, List, Union
 
 import requests
 import rich.console
 import simplejson
 from jwcrypto.common import InvalidJWEOperation
 from jwcrypto.jwe import InvalidJWEData
 from jwcrypto.jws import InvalidJWSObject
 from jwcrypto import jwt
-import http
 from rich.table import Table
-from typing import Dict, List, Union
 
 import dds_cli.exceptions
 from dds_cli import __version__, DDSEndpoint
 
 console = rich.console.Console()
 stderr_console = rich.console.Console(stderr=True)
 
@@ -45,15 +44,15 @@
     def format(num: Union[int, float], metric: bool = False, precision: int = 1) -> str:
         """Human-readable formatting of bytes, using binary (powers of 1024)
         or metric (powers of 1000) representation.
         """
         assert isinstance(num, (int, float)), "num must be an int or float"
         assert isinstance(metric, bool), "metric must be a bool"
         assert (
-            isinstance(precision, int) and precision >= 0 and precision <= 3
+            isinstance(precision, int) and 0 <= precision <= 3
         ), "precision must be an int (range 0-3)"
 
         unit_labels = HumanBytes.METRIC_LABELS if metric else HumanBytes.BINARY_LABELS
         last_label = unit_labels[-1]
         unit_step = 1000 if metric else 1024
         unit_step_thresh = unit_step - HumanBytes.PRECISION_OFFSETS[precision]
 
@@ -142,21 +141,24 @@
         )
     return tuple(response.get(x) for x in keys)
 
 
 def perform_request(
     endpoint,
     method,
-    headers={},
+    headers: typing.Dict = None,
     auth=None,
     params=None,
     json=None,
     error_message="API Request failed.",
     timeout=DDSEndpoint.TIMEOUT,
 ):
+    """Execute request to API."""
+    if not headers:
+        headers = {}
     version_header_name: str = "X-CLI-Version"
     request_method = None
     if method == "get":
         request_method = requests.get
     elif method == "put":
         request_method = requests.put
     elif method == "post":
@@ -164,17 +166,17 @@
     elif method == "delete":
         request_method = requests.delete
 
     def transform_paths(json_input):
         """Make paths serializable."""
         # Transform dict and list contents
         if isinstance(json_input, typing.Dict):
-            for x, y in json_input.items():
-                if isinstance(y, pathlib.Path):
-                    json_input[x] = y.as_posix()
+            for key, val in json_input.items():
+                if isinstance(val, pathlib.Path):
+                    json_input[key] = val.as_posix()
         elif isinstance(json_input, typing.List):
             json_input = [x.as_posix() if isinstance(x, pathlib.Path) else x for x in json_input]
         return json_input
 
     json = transform_paths(json_input=json)
     # Perform request.
     try:
@@ -265,15 +267,17 @@
         json_response = response.json()
     except simplejson.JSONDecodeError as err:
         raise SystemExit from err  # TODO: Change?
 
     return json_response
 
 
-def format_api_response(response, key: str, binary: bool = False, always_show: bool = False):
+def format_api_response(
+    response, key: str, binary: bool = False, always_show: bool = False
+):  # pylint: disable=unused-argument
     """Take a value e.g. bytes and reformat it to include a unit prefix."""
     formatted_response = response
     if isinstance(response, bool):
         formatted_response = ":white_heavy_check_mark:" if response else ":x:"
     elif isinstance(response, numbers.Number):
         if key in ["Size", "Usage"]:
             formatted_response = HumanBytes.format(num=response, metric=not binary)
@@ -330,16 +334,16 @@
     timespan["minutes"], _ = divmod(rem, 60)
     time_parts = ((name, round(value)) for name, value in timespan.items())
     time_parts = [
         f"{value} {name if value > 1 else name[:-1]}" for name, value in time_parts if value > 0
     ]
     if time_parts:
         return " ".join(time_parts)
-    else:
-        return "less than a minute"
+
+    return "less than a minute"
 
 
 def get_deletion_confirmation(action: str, project: str) -> bool:
     """Confirm that the user wants to perform deletion."""
     question = f"Are you sure you want to {action} {project}? All its contents "
     if action in ["delete", "abort"]:
         question = question + "and metainfo "
@@ -360,34 +364,35 @@
                 dds_cli.utils.console.print(item)
         else:
             raise dds_cli.exceptions.NoDataError("No users found.")
 
 
 # Adapted from <https://stackoverflow.com/a/49782093>.
 def delete_folder(folder):
+    """Delete local folder / directory."""
     folder = pathlib.Path(folder)
     for file_or_folder in folder.iterdir():
         if file_or_folder.is_dir():
             delete_folder(file_or_folder)
         else:
             file_or_folder.unlink()
     folder.rmdir()
 
 
 def __project_creation_error(response_json: Dict) -> str:
     """Parse response from project creation endpoint."""
-    message, title, description, pi, email = (
+    message, title, description, principal_investigator, email = (
         response_json.get("message"),
         response_json.get("title"),
         response_json.get("description"),
         response_json.get("pi"),
         response_json.get("email"),
     )
 
-    messages: List = [message, title, description, pi, email]
+    messages: List = [message, title, description, principal_investigator, email]
 
     error = next(message for message in messages if message)
 
     if isinstance(error, List):
         return error[0]
 
     return error
```

### Comparing `dds_cli-2.2.64/dds_cli.egg-info/PKG-INFO` & `dds_cli-2.2.65/dds_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dds-cli
-Version: 2.2.64
+Version: 2.2.65
 Summary: A command line tool to manage data and projects in the SciLifeLab Data Delivery System.
 Home-page: https://github.com/ScilifelabDataCentre/dds_cli
 Author: SciLifeLab Data Centre
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dds-cli Version: 2.2.64 Summary: A command line
+Metadata-Version: 2.1 Name: dds-cli Version: 2.2.65 Summary: A command line
 tool to manage data and projects in the SciLifeLab Data Delivery System. Home-
 page: https://github.com/ScilifelabDataCentre/dds_cli Author: SciLifeLab Data
 Centre License: MIT Classifier: Development Status :: 4 - Beta Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `dds_cli-2.2.64/dds_cli.egg-info/SOURCES.txt` & `dds_cli-2.2.65/dds_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.64/setup.py` & `dds_cli-2.2.65/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+"""Setup of DDS CLI."""
+# pylint: disable=unspecified-encoding, exec-used, consider-using-with, duplicate-code
+
 from setuptools import setup, find_packages
-import os
 
 version = {}
 with open("./dds_cli/version.py") as fp:
     exec(fp.read(), version)
 VERSION = version["__version__"]
 
 with open("README.md") as f:
@@ -25,15 +27,15 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     url="https://github.com/ScilifelabDataCentre/dds_cli",
     author="SciLifeLab Data Centre",
     license="MIT",
-    packages=find_packages(exclude=("docs")),
+    packages=find_packages(exclude="docs"),
     include_package_data=True,
     install_requires=requirements,
     setup_requires=["twine>=1.11.0", "setuptools>=38.6"],
     entry_points={
         "console_scripts": [
             "dds = dds_cli.__main__:dds_main",
         ],
```

### Comparing `dds_cli-2.2.64/tests/test_account_manager.py` & `dds_cli-2.2.65/tests/test_account_manager.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.64/tests/test_data_remover.py` & `dds_cli-2.2.65/tests/test_data_remover.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.64/tests/test_file_compressor.py` & `dds_cli-2.2.65/tests/test_file_compressor.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.64/tests/test_file_encryptor.py` & `dds_cli-2.2.65/tests/test_file_encryptor.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.64/tests/test_file_handler_local.py` & `dds_cli-2.2.65/tests/test_file_handler_local.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.64/tests/test_maintenance_manager.py` & `dds_cli-2.2.65/tests/test_maintenance_manager.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.64/tests/test_motd_manager.py` & `dds_cli-2.2.65/tests/test_motd_manager.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.64/tests/test_utils.py` & `dds_cli-2.2.65/tests/test_utils.py`

 * *Files identical despite different names*

