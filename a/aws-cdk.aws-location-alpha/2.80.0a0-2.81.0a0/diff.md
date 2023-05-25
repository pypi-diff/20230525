# Comparing `tmp/aws-cdk.aws-location-alpha-2.80.0a0.tar.gz` & `tmp/aws-cdk.aws-location-alpha-2.81.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src119495194/src/packages/@aws-cdk/aws-location-alpha/dist/python/aws-cdk.aws-location-alpha-2.80.0a0.tar", last modified: Fri May 19 21:06:05 2023, max compression
+gzip compressed data, was "/codebuild/output/src215479335/src/packages/@aws-cdk/aws-location-alpha/dist/python/aws-cdk.aws-location-alpha-2.81.0a0.tar", last modified: Thu May 25 16:41:58 2023, max compression
```

## Comparing `aws-cdk.aws-location-alpha-2.80.0a0.tar` & `aws-cdk.aws-location-alpha-2.81.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:06:05.000000 aws-cdk.aws-location-alpha-2.80.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-05-19 21:05:57.000000 aws-cdk.aws-location-alpha-2.80.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-19 21:05:57.000000 aws-cdk.aws-location-alpha-2.80.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-19 21:05:57.000000 aws-cdk.aws-location-alpha-2.80.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3088 2023-05-19 21:06:05.000000 aws-cdk.aws-location-alpha-2.80.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2085 2023-05-19 21:05:57.000000 aws-cdk.aws-location-alpha-2.80.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-05-19 21:05:57.000000 aws-cdk.aws-location-alpha-2.80.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 21:06:05.000000 aws-cdk.aws-location-alpha-2.80.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1877 2023-05-19 21:05:57.000000 aws-cdk.aws-location-alpha-2.80.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:06:05.000000 aws-cdk.aws-location-alpha-2.80.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:06:05.000000 aws-cdk.aws-location-alpha-2.80.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:06:05.000000 aws-cdk.aws-location-alpha-2.80.0a0/src/aws_cdk/aws_location_alpha/
--rw-r--r--   0 root         (0) root         (0)    18770 2023-05-19 21:05:57.000000 aws-cdk.aws-location-alpha-2.80.0a0/src/aws_cdk/aws_location_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:06:05.000000 aws-cdk.aws-location-alpha-2.80.0a0/src/aws_cdk/aws_location_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      443 2023-05-19 21:05:57.000000 aws-cdk.aws-location-alpha-2.80.0a0/src/aws_cdk/aws_location_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25461 2023-05-19 21:05:57.000000 aws-cdk.aws-location-alpha-2.80.0a0/src/aws_cdk/aws_location_alpha/_jsii/aws-location-alpha@2.80.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 21:05:57.000000 aws-cdk.aws-location-alpha-2.80.0a0/src/aws_cdk/aws_location_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:06:05.000000 aws-cdk.aws-location-alpha-2.80.0a0/src/aws_cdk.aws_location_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3088 2023-05-19 21:06:05.000000 aws-cdk.aws-location-alpha-2.80.0a0/src/aws_cdk.aws_location_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      541 2023-05-19 21:06:05.000000 aws-cdk.aws-location-alpha-2.80.0a0/src/aws_cdk.aws_location_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 21:06:05.000000 aws-cdk.aws-location-alpha-2.80.0a0/src/aws_cdk.aws_location_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-19 21:06:05.000000 aws-cdk.aws-location-alpha-2.80.0a0/src/aws_cdk.aws_location_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 21:06:05.000000 aws-cdk.aws-location-alpha-2.80.0a0/src/aws_cdk.aws_location_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:41:58.000000 aws-cdk.aws-location-alpha-2.81.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-05-25 16:41:47.000000 aws-cdk.aws-location-alpha-2.81.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-25 16:41:47.000000 aws-cdk.aws-location-alpha-2.81.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-25 16:41:47.000000 aws-cdk.aws-location-alpha-2.81.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3088 2023-05-25 16:41:58.000000 aws-cdk.aws-location-alpha-2.81.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2085 2023-05-25 16:41:47.000000 aws-cdk.aws-location-alpha-2.81.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-05-25 16:41:47.000000 aws-cdk.aws-location-alpha-2.81.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 16:41:58.000000 aws-cdk.aws-location-alpha-2.81.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1877 2023-05-25 16:41:47.000000 aws-cdk.aws-location-alpha-2.81.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:41:58.000000 aws-cdk.aws-location-alpha-2.81.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:41:58.000000 aws-cdk.aws-location-alpha-2.81.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:41:58.000000 aws-cdk.aws-location-alpha-2.81.0a0/src/aws_cdk/aws_location_alpha/
+-rw-r--r--   0 root         (0) root         (0)    18770 2023-05-25 16:41:47.000000 aws-cdk.aws-location-alpha-2.81.0a0/src/aws_cdk/aws_location_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:41:58.000000 aws-cdk.aws-location-alpha-2.81.0a0/src/aws_cdk/aws_location_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-05-25 16:41:47.000000 aws-cdk.aws-location-alpha-2.81.0a0/src/aws_cdk/aws_location_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25459 2023-05-25 16:41:47.000000 aws-cdk.aws-location-alpha-2.81.0a0/src/aws_cdk/aws_location_alpha/_jsii/aws-location-alpha@2.81.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 16:41:47.000000 aws-cdk.aws-location-alpha-2.81.0a0/src/aws_cdk/aws_location_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:41:58.000000 aws-cdk.aws-location-alpha-2.81.0a0/src/aws_cdk.aws_location_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3088 2023-05-25 16:41:58.000000 aws-cdk.aws-location-alpha-2.81.0a0/src/aws_cdk.aws_location_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      541 2023-05-25 16:41:58.000000 aws-cdk.aws-location-alpha-2.81.0a0/src/aws_cdk.aws_location_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 16:41:58.000000 aws-cdk.aws-location-alpha-2.81.0a0/src/aws_cdk.aws_location_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-25 16:41:58.000000 aws-cdk.aws-location-alpha-2.81.0a0/src/aws_cdk.aws_location_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-25 16:41:58.000000 aws-cdk.aws-location-alpha-2.81.0a0/src/aws_cdk.aws_location_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-location-alpha-2.80.0a0/LICENSE` & `aws-cdk.aws-location-alpha-2.81.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-location-alpha-2.80.0a0/PKG-INFO` & `aws-cdk.aws-location-alpha-2.81.0a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-location-alpha
-Version: 2.80.0a0
+Version: 2.81.0a0
 Summary: The CDK Construct Library for AWS::Location
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-location-alpha-2.80.0a0/README.md` & `aws-cdk.aws-location-alpha-2.81.0a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-location-alpha-2.80.0a0/setup.py` & `aws-cdk.aws-location-alpha-2.81.0a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-location-alpha",
-    "version": "2.80.0.a0",
+    "version": "2.81.0.a0",
     "description": "The CDK Construct Library for AWS::Location",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "aws_cdk.aws_location_alpha",
         "aws_cdk.aws_location_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_location_alpha._jsii": [
-            "aws-location-alpha@2.80.0-alpha.0.jsii.tgz"
+            "aws-location-alpha@2.81.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_location_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.80.0",
+        "aws-cdk-lib==2.81.0",
         "constructs>=10.0.0, <11.0.0",
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

### Comparing `aws-cdk.aws-location-alpha-2.80.0a0/src/aws_cdk/aws_location_alpha/__init__.py` & `aws-cdk.aws-location-alpha-2.81.0a0/src/aws_cdk/aws_location_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-location-alpha-2.80.0a0/src/aws_cdk.aws_location_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-location-alpha-2.81.0a0/src/aws_cdk.aws_location_alpha.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-location-alpha
-Version: 2.80.0a0
+Version: 2.81.0a0
 Summary: The CDK Construct Library for AWS::Location
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-location-alpha-2.80.0a0/src/aws_cdk.aws_location_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-location-alpha-2.81.0a0/src/aws_cdk.aws_location_alpha.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_location_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_location_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_location_alpha.egg-info/requires.txt
 src/aws_cdk.aws_location_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_location_alpha/__init__.py
 src/aws_cdk/aws_location_alpha/py.typed
 src/aws_cdk/aws_location_alpha/_jsii/__init__.py
-src/aws_cdk/aws_location_alpha/_jsii/aws-location-alpha@2.80.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_location_alpha/_jsii/aws-location-alpha@2.81.0-alpha.0.jsii.tgz
```

