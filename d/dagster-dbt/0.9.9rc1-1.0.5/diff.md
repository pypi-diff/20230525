# Comparing `tmp/dagster-dbt-0.9.9rc1.tar.gz` & `tmp/dagster-dbt-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-dbt-0.9.9rc1.tar", last modified: Thu Sep 17 21:07:46 2020, max compression
+gzip compressed data, was "dagster-dbt-1.0.5.tar", last modified: Fri Aug 26 13:46:02 2022, max compression
```

## Comparing `dagster-dbt-0.9.9rc1.tar` & `dagster-dbt-1.0.5.tar`

### file list

```diff
@@ -1,27 +1,40 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)      514 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      118 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/dagster_dbt/
--rw-r--r--   0 bobchen    (501) staff       (20)     1134 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     8550 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)    28581 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt/solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3950 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt/types.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3720 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt/utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/dagster_dbt.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      514 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/dagster_dbt.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      595 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/dagster_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/dagster_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/dagster_dbt.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       39 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/dagster_dbt.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       30 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/dagster_dbt.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/dagster_dbt_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    10353 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3661 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt_tests/test_resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4771 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt_tests/test_solids_i.py
--rw-r--r--   0 bobchen    (501) staff       (20)     9315 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt_tests/test_solids_ii.py
--rw-r--r--   0 bobchen    (501) staff       (20)      458 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt_tests/test_utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       89 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       38 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1100 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:02.224646 dagster-dbt-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       45 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      644 2022-08-26 13:46:02.224646 dagster-dbt-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      118 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:02.216646 dagster-dbt-1.0.5/dagster_dbt/
+-rw-r--r--   0 root         (0) root         (0)     1695 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24266 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/asset_defs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:02.216646 dagster-dbt-1.0.5/dagster_dbt/cli/
+-rw-r--r--   0 root         (0) root         (0)       88 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4053 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/cli/constants.py
+-rw-r--r--   0 root         (0) root         (0)    14754 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/cli/resources.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/cli/types.py
+-rw-r--r--   0 root         (0) root         (0)     5848 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:02.220646 dagster-dbt-1.0.5/dagster_dbt/cloud/
+-rw-r--r--   0 root         (0) root         (0)      130 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/cloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4738 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/cloud/ops.py
+-rw-r--r--   0 root         (0) root         (0)    24680 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/cloud/resources.py
+-rw-r--r--   0 root         (0) root         (0)     2715 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/cloud/types.py
+-rw-r--r--   0 root         (0) root         (0)     7438 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/dbt_resource.py
+-rw-r--r--   0 root         (0) root         (0)     3012 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/errors.py
+-rw-r--r--   0 root         (0) root         (0)     4398 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/ops.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:02.224646 dagster-dbt-1.0.5/dagster_dbt/rpc/
+-rw-r--r--   0 root         (0) root         (0)      180 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/rpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24560 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/rpc/resources.py
+-rw-r--r--   0 root         (0) root         (0)      938 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/rpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/rpc/utils.py
+-rw-r--r--   0 root         (0) root         (0)      631 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/types.py
+-rw-r--r--   0 root         (0) root         (0)     8391 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/dagster_dbt/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:02.216646 dagster-dbt-1.0.5/dagster_dbt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      644 2022-08-26 13:46:02.000000 dagster-dbt-1.0.5/dagster_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      817 2022-08-26 13:46:02.000000 dagster-dbt-1.0.5/dagster_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:02.000000 dagster-dbt-1.0.5/dagster_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:02.000000 dagster-dbt-1.0.5/dagster_dbt.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      121 2022-08-26 13:46:02.000000 dagster-dbt-1.0.5/dagster_dbt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-08-26 13:46:02.000000 dagster-dbt-1.0.5/dagster_dbt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2022-08-26 13:46:02.224646 dagster-dbt-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1623 2022-08-26 13:33:01.000000 dagster-dbt-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-dbt-0.9.9rc1/PKG-INFO` & `dagster-dbt-1.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-dbt
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: A Dagster integration for dbt
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-dbt
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Provides-Extra: test
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-dbt-0.9.9rc1/dagster_dbt.egg-info/PKG-INFO` & `dagster-dbt-1.0.5/dagster_dbt.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-dbt
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: A Dagster integration for dbt
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-dbt
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Provides-Extra: test
+License-File: LICENSE
+
+UNKNOWN
+
```

