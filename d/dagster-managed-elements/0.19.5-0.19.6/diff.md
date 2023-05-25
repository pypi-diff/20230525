# Comparing `tmp/dagster-managed-elements-0.19.5.tar.gz` & `tmp/dagster-managed-elements-0.19.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-managed-elements-0.19.5.tar", last modified: Thu May 18 20:48:48 2023, max compression
+gzip compressed data, was "dagster-managed-elements-0.19.6.tar", last modified: Thu May 25 17:26:50 2023, max compression
```

## Comparing `dagster-managed-elements-0.19.5.tar` & `dagster-managed-elements-0.19.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:48.685663 dagster-managed-elements-0.19.5/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-05-18 20:38:07.000000 dagster-managed-elements-0.19.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       76 2023-05-18 20:38:07.000000 dagster-managed-elements-0.19.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      686 2023-05-18 20:48:48.685663 dagster-managed-elements-0.19.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-18 20:38:07.000000 dagster-managed-elements-0.19.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:48.681663 dagster-managed-elements-0.19.5/dagster_managed_elements/
--rw-r--r--   0 root         (0) root         (0)      202 2023-05-18 20:38:07.000000 dagster-managed-elements-0.19.5/dagster_managed_elements/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6327 2023-05-18 20:38:07.000000 dagster-managed-elements-0.19.5/dagster_managed_elements/cli.py
--rw-r--r--   0 root         (0) root         (0)     9573 2023-05-18 20:38:07.000000 dagster-managed-elements-0.19.5/dagster_managed_elements/types.py
--rw-r--r--   0 root         (0) root         (0)     3357 2023-05-18 20:38:07.000000 dagster-managed-elements-0.19.5/dagster_managed_elements/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-18 20:38:07.000000 dagster-managed-elements-0.19.5/dagster_managed_elements/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:48.685663 dagster-managed-elements-0.19.5/dagster_managed_elements.egg-info/
--rw-r--r--   0 root         (0) root         (0)      686 2023-05-18 20:48:48.000000 dagster-managed-elements-0.19.5/dagster_managed_elements.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      558 2023-05-18 20:48:48.000000 dagster-managed-elements-0.19.5/dagster_managed_elements.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:48:48.000000 dagster-managed-elements-0.19.5/dagster_managed_elements.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      126 2023-05-18 20:48:48.000000 dagster-managed-elements-0.19.5/dagster_managed_elements.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:48:48.000000 dagster-managed-elements-0.19.5/dagster_managed_elements.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 20:48:48.000000 dagster-managed-elements-0.19.5/dagster_managed_elements.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-05-18 20:48:48.000000 dagster-managed-elements-0.19.5/dagster_managed_elements.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      171 2023-05-18 20:48:48.689664 dagster-managed-elements-0.19.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1518 2023-05-18 20:38:07.000000 dagster-managed-elements-0.19.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:26:50.694131 dagster-managed-elements-0.19.6/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-05-25 17:16:50.000000 dagster-managed-elements-0.19.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       76 2023-05-25 17:16:50.000000 dagster-managed-elements-0.19.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      686 2023-05-25 17:26:50.694131 dagster-managed-elements-0.19.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-25 17:16:50.000000 dagster-managed-elements-0.19.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:26:50.694131 dagster-managed-elements-0.19.6/dagster_managed_elements/
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-25 17:16:50.000000 dagster-managed-elements-0.19.6/dagster_managed_elements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6327 2023-05-25 17:16:50.000000 dagster-managed-elements-0.19.6/dagster_managed_elements/cli.py
+-rw-r--r--   0 root         (0) root         (0)     9573 2023-05-25 17:16:50.000000 dagster-managed-elements-0.19.6/dagster_managed_elements/types.py
+-rw-r--r--   0 root         (0) root         (0)     3357 2023-05-25 17:16:50.000000 dagster-managed-elements-0.19.6/dagster_managed_elements/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-25 17:16:50.000000 dagster-managed-elements-0.19.6/dagster_managed_elements/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:26:50.694131 dagster-managed-elements-0.19.6/dagster_managed_elements.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      686 2023-05-25 17:26:50.000000 dagster-managed-elements-0.19.6/dagster_managed_elements.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      558 2023-05-25 17:26:50.000000 dagster-managed-elements-0.19.6/dagster_managed_elements.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:26:50.000000 dagster-managed-elements-0.19.6/dagster_managed_elements.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2023-05-25 17:26:50.000000 dagster-managed-elements-0.19.6/dagster_managed_elements.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:26:50.000000 dagster-managed-elements-0.19.6/dagster_managed_elements.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 17:26:50.000000 dagster-managed-elements-0.19.6/dagster_managed_elements.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-25 17:26:50.000000 dagster-managed-elements-0.19.6/dagster_managed_elements.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      171 2023-05-25 17:26:50.698131 dagster-managed-elements-0.19.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-05-25 17:16:50.000000 dagster-managed-elements-0.19.6/setup.py
```

### Comparing `dagster-managed-elements-0.19.5/LICENSE` & `dagster-managed-elements-0.19.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.5/PKG-INFO` & `dagster-managed-elements-0.19.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-managed-elements
-Version: 0.19.5
+Version: 0.19.6
 Summary: Package for Managed elements with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-managed-elements
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-managed-elements-0.19.5/dagster_managed_elements/cli.py` & `dagster-managed-elements-0.19.6/dagster_managed_elements/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.5/dagster_managed_elements/types.py` & `dagster-managed-elements-0.19.6/dagster_managed_elements/types.py`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.5/dagster_managed_elements/utils.py` & `dagster-managed-elements-0.19.6/dagster_managed_elements/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.5/dagster_managed_elements.egg-info/PKG-INFO` & `dagster-managed-elements-0.19.6/dagster_managed_elements.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-managed-elements
-Version: 0.19.5
+Version: 0.19.6
 Summary: Package for Managed elements with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-managed-elements
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-managed-elements-0.19.5/dagster_managed_elements.egg-info/SOURCES.txt` & `dagster-managed-elements-0.19.6/dagster_managed_elements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.5/setup.py` & `dagster-managed-elements-0.19.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_managed_elements_tests*"]),
-    install_requires=["dagster==1.3.5", "requests", "click_spinner"],
+    install_requires=["dagster==1.3.6", "requests", "click_spinner"],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "dagster-managed-elements = dagster_managed_elements.cli:main",
             "dagster-me = dagster_managed_elements.cli:main",
         ]
     },
```

