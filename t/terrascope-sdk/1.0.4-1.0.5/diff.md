# Comparing `tmp/terrascope-sdk-1.0.4.tar.gz` & `tmp/terrascope-sdk-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/marticenicks/repos/terrascope_sdk/dist/.tmp-rm8lmc29/terrascope-sdk-1.0.4.tar", last modified: Mon Dec  5 13:29:53 2022, max compression
+gzip compressed data, was "/Users/marticenicks/repos/terrascope_sdk/dist/.tmp-hrh1dn2w/terrascope-sdk-1.0.5.tar", last modified: Tue Dec 13 12:19:03 2022, max compression
```

## Comparing `terrascope-sdk-1.0.4.tar` & `terrascope-sdk-1.0.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-05 13:29:53.000000 terrascope-sdk-1.0.4/
--rw-r--r--   0 marticenicks   (503) staff       (20)     1061 2022-09-20 12:17:07.000000 terrascope-sdk-1.0.4/LICENSE
--rw-r--r--   0 marticenicks   (503) staff       (20)     2561 2022-12-05 13:29:53.000000 terrascope-sdk-1.0.4/PKG-INFO
--rw-r--r--   0 marticenicks   (503) staff       (20)      845 2022-12-05 13:28:45.000000 terrascope-sdk-1.0.4/README.md
--rw-r--r--   0 marticenicks   (503) staff       (20)      990 2022-12-01 15:59:56.000000 terrascope-sdk-1.0.4/pyproject.toml
--rw-r--r--   0 marticenicks   (503) staff       (20)       38 2022-12-05 13:29:53.000000 terrascope-sdk-1.0.4/setup.cfg
-drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-05 13:29:52.000000 terrascope-sdk-1.0.4/terrascope/
--rw-r--r--   0 marticenicks   (503) staff       (20)        0 2022-08-23 12:05:34.000000 terrascope-sdk-1.0.4/terrascope/__init__.py
-drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-05 13:29:52.000000 terrascope-sdk-1.0.4/terrascope/sdk/
--rw-r--r--   0 marticenicks   (503) staff       (20)        0 2022-08-23 12:05:34.000000 terrascope-sdk-1.0.4/terrascope/sdk/__init__.py
-drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-05 13:29:53.000000 terrascope-sdk-1.0.4/terrascope/sdk/api/
--rw-r--r--   0 marticenicks   (503) staff       (20)        0 2022-08-23 12:05:34.000000 terrascope-sdk-1.0.4/terrascope/sdk/api/__init__.py
--rw-r--r--   0 marticenicks   (503) staff       (20)    27404 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.4/terrascope/sdk/api/algorithm.py
--rw-r--r--   0 marticenicks   (503) staff       (20)    27489 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.4/terrascope/sdk/api/analysis.py
--rw-r--r--   0 marticenicks   (503) staff       (20)    13852 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.4/terrascope/sdk/api/aoi.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     6456 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.4/terrascope/sdk/api/credit.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     3496 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.4/terrascope/sdk/api/data.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     2353 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.4/terrascope/sdk/api/permission.py
--rw-r--r--   0 marticenicks   (503) staff       (20)    15627 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.4/terrascope/sdk/api/result.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     2760 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.4/terrascope/sdk/api/toi.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     4178 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.4/terrascope/sdk/api/user.py
--rw-r--r--   0 marticenicks   (503) staff       (20)      851 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.4/terrascope/sdk/api/visualization.py
-drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-05 13:29:53.000000 terrascope-sdk-1.0.4/terrascope/sdk/builder/
--rw-r--r--   0 marticenicks   (503) staff       (20)        0 2022-11-03 15:49:18.000000 terrascope-sdk-1.0.4/terrascope/sdk/builder/__init__.py
--rw-r--r--   0 marticenicks   (503) staff       (20)    15382 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.4/terrascope/sdk/builder/algorithm.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     7091 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.4/terrascope/sdk/builder/analysis.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     6766 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.4/terrascope/sdk/builder/toi.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     5280 2022-12-02 18:44:12.000000 terrascope-sdk-1.0.4/terrascope/sdk/terrascope_sdk.py
-drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-05 13:29:53.000000 terrascope-sdk-1.0.4/terrascope/sdk/tools/
--rw-r--r--   0 marticenicks   (503) staff       (20)        0 2022-08-23 12:05:34.000000 terrascope-sdk-1.0.4/terrascope/sdk/tools/__init__.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     5752 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.4/terrascope/sdk/tools/io.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     1396 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.4/terrascope/sdk/tools/sdk_support.py
-drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-05 13:29:53.000000 terrascope-sdk-1.0.4/terrascope_sdk.egg-info/
--rw-r--r--   0 marticenicks   (503) staff       (20)     2561 2022-12-05 13:29:52.000000 terrascope-sdk-1.0.4/terrascope_sdk.egg-info/PKG-INFO
--rw-r--r--   0 marticenicks   (503) staff       (20)     1293 2022-12-05 13:29:52.000000 terrascope-sdk-1.0.4/terrascope_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 marticenicks   (503) staff       (20)        1 2022-12-05 13:29:52.000000 terrascope-sdk-1.0.4/terrascope_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 marticenicks   (503) staff       (20)      113 2022-12-05 13:29:52.000000 terrascope-sdk-1.0.4/terrascope_sdk.egg-info/requires.txt
--rw-r--r--   0 marticenicks   (503) staff       (20)       44 2022-12-05 13:29:52.000000 terrascope-sdk-1.0.4/terrascope_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-05 13:29:52.000000 terrascope-sdk-1.0.4/tests/
-drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-05 13:29:53.000000 terrascope-sdk-1.0.4/tests/integration/
--rw-r--r--   0 marticenicks   (503) staff       (20)    46388 2022-12-05 13:22:22.000000 terrascope-sdk-1.0.4/tests/integration/test_algorithm.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     1193 2022-11-03 15:49:18.000000 terrascope-sdk-1.0.4/tests/integration/test_algorithm_builder.py
--rw-r--r--   0 marticenicks   (503) staff       (20)    47447 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.4/tests/integration/test_analysis.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     1111 2022-11-03 15:49:18.000000 terrascope-sdk-1.0.4/tests/integration/test_analysis_builder.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     6127 2022-10-07 20:45:48.000000 terrascope-sdk-1.0.4/tests/integration/test_aoi.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     8417 2022-12-05 13:22:22.000000 terrascope-sdk-1.0.4/tests/integration/test_credit.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     1325 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.4/tests/integration/test_data.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     5982 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.4/tests/integration/test_permission.py
--rw-r--r--   0 marticenicks   (503) staff       (20)     7021 2022-11-03 15:49:18.000000 terrascope-sdk-1.0.4/tests/integration/test_result.py
--rw-r--r--   0 marticenicks   (503) staff       (20)      990 2022-11-03 15:49:18.000000 terrascope-sdk-1.0.4/tests/integration/test_sdk_support.py
--rw-r--r--   0 marticenicks   (503) staff       (20)    13125 2022-11-03 15:49:18.000000 terrascope-sdk-1.0.4/tests/integration/test_toi.py
--rw-r--r--   0 marticenicks   (503) staff       (20)      152 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.4/tests/integration/test_visualization.py
+drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/
+-rw-r--r--   0 marticenicks   (503) staff       (20)     1061 2022-09-20 12:17:07.000000 terrascope-sdk-1.0.5/LICENSE
+-rw-r--r--   0 marticenicks   (503) staff       (20)     2562 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/PKG-INFO
+-rw-r--r--   0 marticenicks   (503) staff       (20)      846 2022-12-05 14:48:31.000000 terrascope-sdk-1.0.5/README.md
+-rw-r--r--   0 marticenicks   (503) staff       (20)      990 2022-12-13 12:18:07.000000 terrascope-sdk-1.0.5/pyproject.toml
+-rw-r--r--   0 marticenicks   (503) staff       (20)       38 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/setup.cfg
+drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope/
+-rw-r--r--   0 marticenicks   (503) staff       (20)        0 2022-08-23 12:05:34.000000 terrascope-sdk-1.0.5/terrascope/__init__.py
+drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope/sdk/
+-rw-r--r--   0 marticenicks   (503) staff       (20)        0 2022-08-23 12:05:34.000000 terrascope-sdk-1.0.5/terrascope/sdk/__init__.py
+drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/
+-rw-r--r--   0 marticenicks   (503) staff       (20)        0 2022-08-23 12:05:34.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/__init__.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)    27404 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/algorithm.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)    27647 2022-12-13 12:13:36.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/analysis.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)    13852 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/aoi.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)     6456 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/credit.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)     3496 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/data.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)     2353 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/permission.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)    15627 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/result.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)     2760 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/toi.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)     4178 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/user.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)      851 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/api/visualization.py
+drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope/sdk/builder/
+-rw-r--r--   0 marticenicks   (503) staff       (20)        0 2022-11-03 15:49:18.000000 terrascope-sdk-1.0.5/terrascope/sdk/builder/__init__.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)    15398 2022-12-13 12:18:07.000000 terrascope-sdk-1.0.5/terrascope/sdk/builder/algorithm.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)     7091 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/builder/analysis.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)     6766 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/builder/toi.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)     5280 2022-12-05 14:48:26.000000 terrascope-sdk-1.0.5/terrascope/sdk/terrascope_sdk.py
+drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope/sdk/tools/
+-rw-r--r--   0 marticenicks   (503) staff       (20)        0 2022-08-23 12:05:34.000000 terrascope-sdk-1.0.5/terrascope/sdk/tools/__init__.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)     5752 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/tools/io.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)     1396 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/terrascope/sdk/tools/sdk_support.py
+drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope_sdk.egg-info/
+-rw-r--r--   0 marticenicks   (503) staff       (20)     2562 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 marticenicks   (503) staff       (20)     1293 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 marticenicks   (503) staff       (20)        1 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 marticenicks   (503) staff       (20)      113 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope_sdk.egg-info/requires.txt
+-rw-r--r--   0 marticenicks   (503) staff       (20)       44 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/terrascope_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/tests/
+drwxr-xr-x   0 marticenicks   (503) staff       (20)        0 2022-12-13 12:19:03.000000 terrascope-sdk-1.0.5/tests/integration/
+-rw-r--r--   0 marticenicks   (503) staff       (20)    46388 2022-12-05 14:48:26.000000 terrascope-sdk-1.0.5/tests/integration/test_algorithm.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)     1193 2022-11-03 15:49:18.000000 terrascope-sdk-1.0.5/tests/integration/test_algorithm_builder.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)    47447 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/tests/integration/test_analysis.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)     1111 2022-11-03 15:49:18.000000 terrascope-sdk-1.0.5/tests/integration/test_analysis_builder.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)     6127 2022-10-07 20:45:48.000000 terrascope-sdk-1.0.5/tests/integration/test_aoi.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)     8417 2022-12-05 13:22:22.000000 terrascope-sdk-1.0.5/tests/integration/test_credit.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)     1325 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/tests/integration/test_data.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)     5982 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/tests/integration/test_permission.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)     7021 2022-11-03 15:49:18.000000 terrascope-sdk-1.0.5/tests/integration/test_result.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)      990 2022-11-03 15:49:18.000000 terrascope-sdk-1.0.5/tests/integration/test_sdk_support.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)    13125 2022-11-03 15:49:18.000000 terrascope-sdk-1.0.5/tests/integration/test_toi.py
+-rw-r--r--   0 marticenicks   (503) staff       (20)      152 2022-11-16 12:53:16.000000 terrascope-sdk-1.0.5/tests/integration/test_visualization.py
```

### Comparing `terrascope-sdk-1.0.4/LICENSE` & `terrascope-sdk-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/PKG-INFO` & `terrascope-sdk-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrascope-sdk
-Version: 1.0.4
+Version: 1.0.5
 Summary: A software development kit for developing projects on TerraScope
 Author-email: "Martice E. Nicks III" <martice.nicks@orbitalinsight.com>
 License: Copyright 2022 Orbital Insight, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -38,15 +38,15 @@
 that are available. 
 
 Each API uses a client object which requires the following env variables to be set:
 
 ```shell
 TERRASCOPE_HOST=terrascope-api1.orbitalinsight.com
 TERRASCOPE_TOKEN=<TerraScope API Token>
-TERRASCOPE_TIMEOUT=<Int timeout in seconds> defalts to 60 seconds
+TERRASCOPE_TIMEOUT=<Int timeout in seconds> defaults to 60 seconds
 ```
 
 ## Authors and acknowledgment
 
 Orbital Insight
 
 ## License
```

### Comparing `terrascope-sdk-1.0.4/README.md` & `terrascope-sdk-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 that are available. 
 
 Each API uses a client object which requires the following env variables to be set:
 
 ```shell
 TERRASCOPE_HOST=terrascope-api1.orbitalinsight.com
 TERRASCOPE_TOKEN=<TerraScope API Token>
-TERRASCOPE_TIMEOUT=<Int timeout in seconds> defalts to 60 seconds
+TERRASCOPE_TIMEOUT=<Int timeout in seconds> defaults to 60 seconds
 ```
 
 ## Authors and acknowledgment
 
 Orbital Insight
 
 ## License
```

### Comparing `terrascope-sdk-1.0.4/pyproject.toml` & `terrascope-sdk-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terrascope-sdk"
 
 
-version = "1.0.4"
+version = "1.0.5"
 
 
 authors = [
     { name = "Martice E. Nicks III", email = "martice.nicks@orbitalinsight.com" },
 ]
 description = "A software development kit for developing projects on TerraScope"
 readme = "README.md"
```

### Comparing `terrascope-sdk-1.0.4/terrascope/sdk/api/algorithm.py` & `terrascope-sdk-1.0.5/terrascope/sdk/api/algorithm.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/terrascope/sdk/api/analysis.py` & `terrascope-sdk-1.0.5/terrascope/sdk/api/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,14 +340,15 @@
         Retrieve the metadata for all analysis configurations that this user has access to and that match the provided
         search filters. By default, deactivated analysis_configs are not returned. Setting include_deactivated to true
         will also return any analysis_configs that had been deactivated.
 
         :param kwargs:
             - analysis_id: str
             - analysis_version_id: str
+            - subject_id: str
             - search_text: str
             - tag: str
             - min_created_on: Datetime
             - max_created_on: Datetime
             - include_algorithm_details: bool
             - include_all_versions: bool
             - pagination: Pagination
@@ -363,14 +364,16 @@
             )))
 
         for key in kwargs.keys():
             if key == 'analysis_id':
                 request_fragments.append(AnalysisConfigListRequest(analysis_id=kwargs[key]))
             if key == 'analysis_version_id':
                 request_fragments.append(AnalysisConfigListRequest(analysis_version_id=kwargs[key]))
+            if key == 'subject_id':
+                request_fragments.append(AnalysisConfigListRequest(subject_id=kwargs[key]))
             if key == 'search_text':
                 request_fragments.append(AnalysisConfigListRequest(search_text=kwargs[key]))
             if key == 'tag':
                 request_fragments.append(AnalysisConfigListRequest(tag=kwargs[key]))
             if key == 'min_created_on':
                 min_created_on = Timestamp()
                 min_created_on.FromDatetime(kwargs[key])
```

### Comparing `terrascope-sdk-1.0.4/terrascope/sdk/api/aoi.py` & `terrascope-sdk-1.0.5/terrascope/sdk/api/aoi.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/terrascope/sdk/api/credit.py` & `terrascope-sdk-1.0.5/terrascope/sdk/api/credit.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/terrascope/sdk/api/data.py` & `terrascope-sdk-1.0.5/terrascope/sdk/api/data.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/terrascope/sdk/api/permission.py` & `terrascope-sdk-1.0.5/terrascope/sdk/api/permission.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/terrascope/sdk/api/result.py` & `terrascope-sdk-1.0.5/terrascope/sdk/api/result.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/terrascope/sdk/api/toi.py` & `terrascope-sdk-1.0.5/terrascope/sdk/api/toi.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/terrascope/sdk/api/user.py` & `terrascope-sdk-1.0.5/terrascope/sdk/api/user.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/terrascope/sdk/api/visualization.py` & `terrascope-sdk-1.0.5/terrascope/sdk/api/visualization.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/terrascope/sdk/builder/algorithm.py` & `terrascope-sdk-1.0.5/terrascope/sdk/builder/algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,17 +225,17 @@
     def container_parameters_resource_request(self, **kwargs):
         if 'resource_request' not in self.container_parameters['container_parameters'].keys():
             self.container_parameters['container_parameters']['resource_request'] = {}
 
         if 'gpu' in kwargs.keys():
             self.container_parameters['container_parameters']['resource_request']['gpu'] = kwargs['gpu']
         if 'memory_gb' in kwargs.keys():
-            self.container_parameters['container_parameters']['resource_request']['gpu'] = kwargs['memory_gb']
+            self.container_parameters['container_parameters']['resource_request']['memory_gb'] = kwargs['memory_gb']
         if 'cpu_millicore' in kwargs.keys():
-            self.container_parameters['container_parameters']['resource_request']['gpu'] = kwargs['cpu_millicore']
+            self.container_parameters['container_parameters']['resource_request']['cpu_millicore'] = kwargs['cpu_millicore']
 
     # Parameters
     def parameter_add(self, **kwargs):
         assert 'description' in kwargs.keys()
         entry = {}
         if 'name' in kwargs.keys():
             entry['name'] = kwargs['name']
```

### Comparing `terrascope-sdk-1.0.4/terrascope/sdk/builder/analysis.py` & `terrascope-sdk-1.0.5/terrascope/sdk/builder/analysis.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/terrascope/sdk/builder/toi.py` & `terrascope-sdk-1.0.5/terrascope/sdk/builder/toi.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/terrascope/sdk/terrascope_sdk.py` & `terrascope-sdk-1.0.5/terrascope/sdk/terrascope_sdk.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/terrascope/sdk/tools/io.py` & `terrascope-sdk-1.0.5/terrascope/sdk/tools/io.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/terrascope/sdk/tools/sdk_support.py` & `terrascope-sdk-1.0.5/terrascope/sdk/tools/sdk_support.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/terrascope_sdk.egg-info/PKG-INFO` & `terrascope-sdk-1.0.5/terrascope_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrascope-sdk
-Version: 1.0.4
+Version: 1.0.5
 Summary: A software development kit for developing projects on TerraScope
 Author-email: "Martice E. Nicks III" <martice.nicks@orbitalinsight.com>
 License: Copyright 2022 Orbital Insight, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -38,15 +38,15 @@
 that are available. 
 
 Each API uses a client object which requires the following env variables to be set:
 
 ```shell
 TERRASCOPE_HOST=terrascope-api1.orbitalinsight.com
 TERRASCOPE_TOKEN=<TerraScope API Token>
-TERRASCOPE_TIMEOUT=<Int timeout in seconds> defalts to 60 seconds
+TERRASCOPE_TIMEOUT=<Int timeout in seconds> defaults to 60 seconds
 ```
 
 ## Authors and acknowledgment
 
 Orbital Insight
 
 ## License
```

### Comparing `terrascope-sdk-1.0.4/terrascope_sdk.egg-info/SOURCES.txt` & `terrascope-sdk-1.0.5/terrascope_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/tests/integration/test_algorithm.py` & `terrascope-sdk-1.0.5/tests/integration/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/tests/integration/test_algorithm_builder.py` & `terrascope-sdk-1.0.5/tests/integration/test_algorithm_builder.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/tests/integration/test_analysis.py` & `terrascope-sdk-1.0.5/tests/integration/test_analysis.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/tests/integration/test_analysis_builder.py` & `terrascope-sdk-1.0.5/tests/integration/test_analysis_builder.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/tests/integration/test_aoi.py` & `terrascope-sdk-1.0.5/tests/integration/test_aoi.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/tests/integration/test_credit.py` & `terrascope-sdk-1.0.5/tests/integration/test_credit.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/tests/integration/test_data.py` & `terrascope-sdk-1.0.5/tests/integration/test_data.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/tests/integration/test_permission.py` & `terrascope-sdk-1.0.5/tests/integration/test_permission.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/tests/integration/test_result.py` & `terrascope-sdk-1.0.5/tests/integration/test_result.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/tests/integration/test_sdk_support.py` & `terrascope-sdk-1.0.5/tests/integration/test_sdk_support.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.4/tests/integration/test_toi.py` & `terrascope-sdk-1.0.5/tests/integration/test_toi.py`

 * *Files identical despite different names*

