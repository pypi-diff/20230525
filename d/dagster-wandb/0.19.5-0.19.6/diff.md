# Comparing `tmp/dagster-wandb-0.19.5.tar.gz` & `tmp/dagster-wandb-0.19.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-wandb-0.19.5.tar", last modified: Thu May 18 20:45:53 2023, max compression
+gzip compressed data, was "dagster-wandb-0.19.6.tar", last modified: Thu May 25 17:25:06 2023, max compression
```

## Comparing `dagster-wandb-0.19.5.tar` & `dagster-wandb-0.19.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:53.005616 dagster-wandb-0.19.5/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-18 20:38:07.000000 dagster-wandb-0.19.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-18 20:38:07.000000 dagster-wandb-0.19.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      679 2023-05-18 20:45:53.005616 dagster-wandb-0.19.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-18 20:38:07.000000 dagster-wandb-0.19.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:53.005616 dagster-wandb-0.19.5/dagster_wandb/
--rw-r--r--   0 root         (0) root         (0)      613 2023-05-18 20:38:07.000000 dagster-wandb-0.19.5/dagster_wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33673 2023-05-18 20:38:07.000000 dagster-wandb-0.19.5/dagster_wandb/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:53.005616 dagster-wandb-0.19.5/dagster_wandb/launch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-wandb-0.19.5/dagster_wandb/launch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4425 2023-05-18 20:38:07.000000 dagster-wandb-0.19.5/dagster_wandb/launch/configs.py
--rw-r--r--   0 root         (0) root         (0)     5192 2023-05-18 20:38:07.000000 dagster-wandb-0.19.5/dagster_wandb/launch/ops.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-18 20:38:07.000000 dagster-wandb-0.19.5/dagster_wandb/py.typed
--rw-r--r--   0 root         (0) root         (0)     2157 2023-05-18 20:38:07.000000 dagster-wandb-0.19.5/dagster_wandb/resources.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-18 20:38:07.000000 dagster-wandb-0.19.5/dagster_wandb/types.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-18 20:38:07.000000 dagster-wandb-0.19.5/dagster_wandb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:53.005616 dagster-wandb-0.19.5/dagster_wandb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      679 2023-05-18 20:45:52.000000 dagster-wandb-0.19.5/dagster_wandb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      513 2023-05-18 20:45:52.000000 dagster-wandb-0.19.5/dagster_wandb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:45:52.000000 dagster-wandb-0.19.5/dagster_wandb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:45:52.000000 dagster-wandb-0.19.5/dagster_wandb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-18 20:45:52.000000 dagster-wandb-0.19.5/dagster_wandb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-18 20:45:52.000000 dagster-wandb-0.19.5/dagster_wandb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-18 20:45:53.009616 dagster-wandb-0.19.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1360 2023-05-18 20:38:07.000000 dagster-wandb-0.19.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:25:06.357621 dagster-wandb-0.19.6/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-25 17:16:50.000000 dagster-wandb-0.19.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-25 17:16:50.000000 dagster-wandb-0.19.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      679 2023-05-25 17:25:06.357621 dagster-wandb-0.19.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      150 2023-05-25 17:16:50.000000 dagster-wandb-0.19.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:25:06.353621 dagster-wandb-0.19.6/dagster_wandb/
+-rw-r--r--   0 root         (0) root         (0)      613 2023-05-25 17:16:50.000000 dagster-wandb-0.19.6/dagster_wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33673 2023-05-25 17:16:50.000000 dagster-wandb-0.19.6/dagster_wandb/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:25:06.357621 dagster-wandb-0.19.6/dagster_wandb/launch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:50.000000 dagster-wandb-0.19.6/dagster_wandb/launch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4425 2023-05-25 17:16:50.000000 dagster-wandb-0.19.6/dagster_wandb/launch/configs.py
+-rw-r--r--   0 root         (0) root         (0)     5192 2023-05-25 17:16:50.000000 dagster-wandb-0.19.6/dagster_wandb/launch/ops.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-25 17:16:50.000000 dagster-wandb-0.19.6/dagster_wandb/py.typed
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-05-25 17:16:50.000000 dagster-wandb-0.19.6/dagster_wandb/resources.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-25 17:16:50.000000 dagster-wandb-0.19.6/dagster_wandb/types.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-25 17:16:50.000000 dagster-wandb-0.19.6/dagster_wandb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:25:06.357621 dagster-wandb-0.19.6/dagster_wandb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      679 2023-05-25 17:25:06.000000 dagster-wandb-0.19.6/dagster_wandb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      513 2023-05-25 17:25:06.000000 dagster-wandb-0.19.6/dagster_wandb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:25:06.000000 dagster-wandb-0.19.6/dagster_wandb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:25:06.000000 dagster-wandb-0.19.6/dagster_wandb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-25 17:25:06.000000 dagster-wandb-0.19.6/dagster_wandb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-25 17:25:06.000000 dagster-wandb-0.19.6/dagster_wandb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-25 17:25:06.357621 dagster-wandb-0.19.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1360 2023-05-25 17:16:50.000000 dagster-wandb-0.19.6/setup.py
```

### Comparing `dagster-wandb-0.19.5/LICENSE` & `dagster-wandb-0.19.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.5/PKG-INFO` & `dagster-wandb-0.19.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-wandb
-Version: 0.19.5
+Version: 0.19.6
 Summary: Package for wandb Dagster components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-wandb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-wandb-0.19.5/dagster_wandb/__init__.py` & `dagster-wandb-0.19.6/dagster_wandb/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.5/dagster_wandb/io_manager.py` & `dagster-wandb-0.19.6/dagster_wandb/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.5/dagster_wandb/launch/configs.py` & `dagster-wandb-0.19.6/dagster_wandb/launch/configs.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.5/dagster_wandb/launch/ops.py` & `dagster-wandb-0.19.6/dagster_wandb/launch/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.5/dagster_wandb/resources.py` & `dagster-wandb-0.19.6/dagster_wandb/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.5/dagster_wandb/types.py` & `dagster-wandb-0.19.6/dagster_wandb/types.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.5/dagster_wandb.egg-info/PKG-INFO` & `dagster-wandb-0.19.6/dagster_wandb.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-wandb
-Version: 0.19.5
+Version: 0.19.6
 Summary: Package for wandb Dagster components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-wandb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-wandb-0.19.5/dagster_wandb.egg-info/SOURCES.txt` & `dagster-wandb-0.19.6/dagster_wandb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.5/setup.py` & `dagster-wandb-0.19.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,13 +30,13 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_wandb_tests*"]),
     install_requires=[
-        "dagster==1.3.5",
+        "dagster==1.3.6",
         "wandb>=0.13.5",
     ],
     extras_require={"dev": ["cloudpickle", "joblib", "callee", "dill"]},
     zip_safe=False,
 )
```

