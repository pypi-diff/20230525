# Comparing `tmp/cdk8s-plus-26-2.4.0.tar.gz` & `tmp/cdk8s-plus-26-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-plus-26-2.4.0.tar", last modified: Tue May 23 17:09:07 2023, max compression
+gzip compressed data, was "cdk8s-plus-26-2.4.1.tar", last modified: Thu May 25 02:31:48 2023, max compression
```

## Comparing `cdk8s-plus-26-2.4.0.tar` & `cdk8s-plus-26-2.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:09:07.661118 cdk8s-plus-26-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-23 17:08:55.000000 cdk8s-plus-26-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 17:08:55.000000 cdk8s-plus-26-2.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 17:08:55.000000 cdk8s-plus-26-2.4.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-23 17:09:07.661118 cdk8s-plus-26-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-23 17:08:55.000000 cdk8s-plus-26-2.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-23 17:08:55.000000 cdk8s-plus-26-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:09:07.661118 cdk8s-plus-26-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-23 17:08:55.000000 cdk8s-plus-26-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:09:07.653118 cdk8s-plus-26-2.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:09:07.657118 cdk8s-plus-26-2.4.0/src/cdk8s_plus_26/
--rw-r--r--   0 runner    (1001) docker     (123)  1161508 2023-05-23 17:08:55.000000 cdk8s-plus-26-2.4.0/src/cdk8s_plus_26/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:09:07.657118 cdk8s-plus-26-2.4.0/src/cdk8s_plus_26/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-23 17:08:55.000000 cdk8s-plus-26-2.4.0/src/cdk8s_plus_26/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1287683 2023-05-23 17:08:55.000000 cdk8s-plus-26-2.4.0/src/cdk8s_plus_26/_jsii/cdk8s-plus-26@2.4.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:09:07.661118 cdk8s-plus-26-2.4.0/src/cdk8s_plus_26/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)  2771385 2023-05-23 17:08:55.000000 cdk8s-plus-26-2.4.0/src/cdk8s_plus_26/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:08:55.000000 cdk8s-plus-26-2.4.0/src/cdk8s_plus_26/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:09:07.657118 cdk8s-plus-26-2.4.0/src/cdk8s_plus_26.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-23 17:09:07.000000 cdk8s-plus-26-2.4.0/src/cdk8s_plus_26.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-23 17:09:07.000000 cdk8s-plus-26-2.4.0/src/cdk8s_plus_26.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:09:07.000000 cdk8s-plus-26-2.4.0/src/cdk8s_plus_26.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-23 17:09:07.000000 cdk8s-plus-26-2.4.0/src/cdk8s_plus_26.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 17:09:07.000000 cdk8s-plus-26-2.4.0/src/cdk8s_plus_26.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:31:48.934883 cdk8s-plus-26-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-25 02:31:32.000000 cdk8s-plus-26-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 02:31:32.000000 cdk8s-plus-26-2.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 02:31:32.000000 cdk8s-plus-26-2.4.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-25 02:31:48.934883 cdk8s-plus-26-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-25 02:31:32.000000 cdk8s-plus-26-2.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-25 02:31:32.000000 cdk8s-plus-26-2.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 02:31:48.934883 cdk8s-plus-26-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-25 02:31:32.000000 cdk8s-plus-26-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:31:48.922882 cdk8s-plus-26-2.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:31:48.926883 cdk8s-plus-26-2.4.1/src/cdk8s_plus_26/
+-rw-r--r--   0 runner    (1001) docker     (123)  1161508 2023-05-25 02:31:32.000000 cdk8s-plus-26-2.4.1/src/cdk8s_plus_26/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:31:48.926883 cdk8s-plus-26-2.4.1/src/cdk8s_plus_26/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-25 02:31:32.000000 cdk8s-plus-26-2.4.1/src/cdk8s_plus_26/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1287675 2023-05-25 02:31:32.000000 cdk8s-plus-26-2.4.1/src/cdk8s_plus_26/_jsii/cdk8s-plus-26@2.4.1.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:31:48.930883 cdk8s-plus-26-2.4.1/src/cdk8s_plus_26/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)  2771385 2023-05-25 02:31:32.000000 cdk8s-plus-26-2.4.1/src/cdk8s_plus_26/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 02:31:32.000000 cdk8s-plus-26-2.4.1/src/cdk8s_plus_26/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:31:48.926883 cdk8s-plus-26-2.4.1/src/cdk8s_plus_26.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-25 02:31:48.000000 cdk8s-plus-26-2.4.1/src/cdk8s_plus_26.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-25 02:31:48.000000 cdk8s-plus-26-2.4.1/src/cdk8s_plus_26.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 02:31:48.000000 cdk8s-plus-26-2.4.1/src/cdk8s_plus_26.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-25 02:31:48.000000 cdk8s-plus-26-2.4.1/src/cdk8s_plus_26.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 02:31:48.000000 cdk8s-plus-26-2.4.1/src/cdk8s_plus_26.egg-info/top_level.txt
```

### Comparing `cdk8s-plus-26-2.4.0/LICENSE` & `cdk8s-plus-26-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-26-2.4.0/PKG-INFO` & `cdk8s-plus-26-2.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-26
-Version: 2.4.0
+Version: 2.4.1
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-26 synthesizes Kubernetes manifests for Kubernetes 1.26.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-plus-26-2.4.0/README.md` & `cdk8s-plus-26-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-26-2.4.0/setup.py` & `cdk8s-plus-26-2.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-plus-26",
-    "version": "2.4.0",
+    "version": "2.4.1",
     "description": "cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-26 synthesizes Kubernetes manifests for Kubernetes 1.26.0",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-plus.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -23,25 +23,25 @@
     "packages": [
         "cdk8s_plus_26",
         "cdk8s_plus_26._jsii",
         "cdk8s_plus_26.k8s"
     ],
     "package_data": {
         "cdk8s_plus_26._jsii": [
-            "cdk8s-plus-26@2.4.0.jsii.tgz"
+            "cdk8s-plus-26@2.4.1.jsii.tgz"
         ],
         "cdk8s_plus_26": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdk8s>=2.7.72, <3.0.0",
-        "constructs>=10.2.30, <11.0.0",
-        "jsii>=1.81.0, <2.0.0",
+        "cdk8s>=2.7.75, <3.0.0",
+        "constructs>=10.2.32, <11.0.0",
+        "jsii>=1.82.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk8s-plus-26-2.4.0/src/cdk8s_plus_26/__init__.py` & `cdk8s-plus-26-2.4.1/src/cdk8s_plus_26/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-26-2.4.0/src/cdk8s_plus_26/k8s/__init__.py` & `cdk8s-plus-26-2.4.1/src/cdk8s_plus_26/k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-26-2.4.0/src/cdk8s_plus_26.egg-info/PKG-INFO` & `cdk8s-plus-26-2.4.1/src/cdk8s_plus_26.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-26
-Version: 2.4.0
+Version: 2.4.1
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-26 synthesizes Kubernetes manifests for Kubernetes 1.26.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

