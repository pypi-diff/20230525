# Comparing `tmp/cdklabs.appsync-utils-0.0.96.tar.gz` & `tmp/cdklabs.appsync-utils-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.appsync-utils-0.0.96.tar", last modified: Mon May 22 00:17:57 2023, max compression
+gzip compressed data, was "cdklabs.appsync-utils-0.0.97.tar", last modified: Thu May 25 00:18:29 2023, max compression
```

## Comparing `cdklabs.appsync-utils-0.0.96.tar` & `cdklabs.appsync-utils-0.0.97.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:17:57.081200 cdklabs.appsync-utils-0.0.96/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-22 00:17:43.000000 cdklabs.appsync-utils-0.0.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-22 00:17:43.000000 cdklabs.appsync-utils-0.0.96/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-22 00:17:43.000000 cdklabs.appsync-utils-0.0.96/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-05-22 00:17:57.081200 cdklabs.appsync-utils-0.0.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-05-22 00:17:43.000000 cdklabs.appsync-utils-0.0.96/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-22 00:17:43.000000 cdklabs.appsync-utils-0.0.96/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 00:17:57.081200 cdklabs.appsync-utils-0.0.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-22 00:17:43.000000 cdklabs.appsync-utils-0.0.96/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:17:57.077200 cdklabs.appsync-utils-0.0.96/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:17:57.077200 cdklabs.appsync-utils-0.0.96/src/awscdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:17:57.081200 cdklabs.appsync-utils-0.0.96/src/awscdk/appsync_utils/
--rw-r--r--   0 runner    (1001) docker     (123)   134850 2023-05-22 00:17:43.000000 cdklabs.appsync-utils-0.0.96/src/awscdk/appsync_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:17:57.081200 cdklabs.appsync-utils-0.0.96/src/awscdk/appsync_utils/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-22 00:17:43.000000 cdklabs.appsync-utils-0.0.96/src/awscdk/appsync_utils/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    82438 2023-05-22 00:17:43.000000 cdklabs.appsync-utils-0.0.96/src/awscdk/appsync_utils/_jsii/awscdk-appsync-utils@0.0.96.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 00:17:43.000000 cdklabs.appsync-utils-0.0.96/src/awscdk/appsync_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:17:57.081200 cdklabs.appsync-utils-0.0.96/src/cdklabs.appsync_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-05-22 00:17:57.000000 cdklabs.appsync-utils-0.0.96/src/cdklabs.appsync_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-22 00:17:57.000000 cdklabs.appsync-utils-0.0.96/src/cdklabs.appsync_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 00:17:57.000000 cdklabs.appsync-utils-0.0.96/src/cdklabs.appsync_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-22 00:17:57.000000 cdklabs.appsync-utils-0.0.96/src/cdklabs.appsync_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 00:17:57.000000 cdklabs.appsync-utils-0.0.96/src/cdklabs.appsync_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:18:29.296142 cdklabs.appsync-utils-0.0.97/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-25 00:18:16.000000 cdklabs.appsync-utils-0.0.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 00:18:16.000000 cdklabs.appsync-utils-0.0.97/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 00:18:16.000000 cdklabs.appsync-utils-0.0.97/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-05-25 00:18:29.296142 cdklabs.appsync-utils-0.0.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-05-25 00:18:16.000000 cdklabs.appsync-utils-0.0.97/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-25 00:18:16.000000 cdklabs.appsync-utils-0.0.97/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 00:18:29.296142 cdklabs.appsync-utils-0.0.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-25 00:18:16.000000 cdklabs.appsync-utils-0.0.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:18:29.292142 cdklabs.appsync-utils-0.0.97/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:18:29.292142 cdklabs.appsync-utils-0.0.97/src/awscdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:18:29.296142 cdklabs.appsync-utils-0.0.97/src/awscdk/appsync_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)   134850 2023-05-25 00:18:16.000000 cdklabs.appsync-utils-0.0.97/src/awscdk/appsync_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:18:29.296142 cdklabs.appsync-utils-0.0.97/src/awscdk/appsync_utils/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-25 00:18:16.000000 cdklabs.appsync-utils-0.0.97/src/awscdk/appsync_utils/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82437 2023-05-25 00:18:16.000000 cdklabs.appsync-utils-0.0.97/src/awscdk/appsync_utils/_jsii/awscdk-appsync-utils@0.0.97.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 00:18:16.000000 cdklabs.appsync-utils-0.0.97/src/awscdk/appsync_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:18:29.296142 cdklabs.appsync-utils-0.0.97/src/cdklabs.appsync_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-05-25 00:18:29.000000 cdklabs.appsync-utils-0.0.97/src/cdklabs.appsync_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-25 00:18:29.000000 cdklabs.appsync-utils-0.0.97/src/cdklabs.appsync_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 00:18:29.000000 cdklabs.appsync-utils-0.0.97/src/cdklabs.appsync_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-25 00:18:29.000000 cdklabs.appsync-utils-0.0.97/src/cdklabs.appsync_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 00:18:29.000000 cdklabs.appsync-utils-0.0.97/src/cdklabs.appsync_utils.egg-info/top_level.txt
```

### Comparing `cdklabs.appsync-utils-0.0.96/LICENSE` & `cdklabs.appsync-utils-0.0.97/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.appsync-utils-0.0.96/PKG-INFO` & `cdklabs.appsync-utils-0.0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.appsync-utils
-Version: 0.0.96
+Version: 0.0.97
 Summary: Utilities for creating appsync apis using aws-cdk
 Home-page: https://github.com/cdklabs/awscdk-appsync-utils.git
 Author: Mitchell Valine<mitchellvaline@yahoo.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/awscdk-appsync-utils.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.appsync-utils-0.0.96/README.md` & `cdklabs.appsync-utils-0.0.97/README.md`

 * *Files identical despite different names*

### Comparing `cdklabs.appsync-utils-0.0.96/setup.py` & `cdklabs.appsync-utils-0.0.97/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.appsync-utils",
-    "version": "0.0.96",
+    "version": "0.0.97",
     "description": "Utilities for creating appsync apis using aws-cdk",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/awscdk-appsync-utils.git",
     "long_description_content_type": "text/markdown",
     "author": "Mitchell Valine<mitchellvaline@yahoo.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "awscdk.appsync_utils",
         "awscdk.appsync_utils._jsii"
     ],
     "package_data": {
         "awscdk.appsync_utils._jsii": [
-            "awscdk-appsync-utils@0.0.96.jsii.tgz"
+            "awscdk-appsync-utils@0.0.97.jsii.tgz"
         ],
         "awscdk.appsync_utils": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.60.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.81.0, <2.0.0",
+        "jsii>=1.82.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdklabs.appsync-utils-0.0.96/src/awscdk/appsync_utils/__init__.py` & `cdklabs.appsync-utils-0.0.97/src/awscdk/appsync_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.appsync-utils-0.0.96/src/cdklabs.appsync_utils.egg-info/PKG-INFO` & `cdklabs.appsync-utils-0.0.97/src/cdklabs.appsync_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.appsync-utils
-Version: 0.0.96
+Version: 0.0.97
 Summary: Utilities for creating appsync apis using aws-cdk
 Home-page: https://github.com/cdklabs/awscdk-appsync-utils.git
 Author: Mitchell Valine<mitchellvaline@yahoo.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/awscdk-appsync-utils.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

