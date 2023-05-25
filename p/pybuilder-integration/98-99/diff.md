# Comparing `tmp/pybuilder-integration-98.tar.gz` & `tmp/pybuilder-integration-99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybuilder-integration-98.tar", last modified: Thu May 25 16:44:18 2023, max compression
+gzip compressed data, was "pybuilder-integration-99.tar", last modified: Thu May 25 20:45:20 2023, max compression
```

## Comparing `pybuilder-integration-98.tar` & `pybuilder-integration-99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:44:18.206133 pybuilder-integration-98/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-25 16:44:18.206133 pybuilder-integration-98/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:44:18.206133 pybuilder-integration-98/pybuilder_integration/
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-25 16:43:29.000000 pybuilder-integration-98/pybuilder_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-05-25 16:43:29.000000 pybuilder-integration-98/pybuilder_integration/artifact_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-25 16:43:29.000000 pybuilder-integration-98/pybuilder_integration/cloudwatchlogs_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-25 16:43:29.000000 pybuilder-integration-98/pybuilder_integration/directory_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-25 16:43:29.000000 pybuilder-integration-98/pybuilder_integration/exec_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-25 16:43:29.000000 pybuilder-integration-98/pybuilder_integration/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-05-25 16:43:29.000000 pybuilder-integration-98/pybuilder_integration/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-25 16:43:29.000000 pybuilder-integration-98/pybuilder_integration/tool_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:44:18.206133 pybuilder-integration-98/pybuilder_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-25 16:44:18.000000 pybuilder-integration-98/pybuilder_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-25 16:44:18.000000 pybuilder-integration-98/pybuilder_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:44:18.000000 pybuilder-integration-98/pybuilder_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:44:18.000000 pybuilder-integration-98/pybuilder_integration.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 16:44:18.000000 pybuilder-integration-98/pybuilder_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 16:44:18.000000 pybuilder-integration-98/pybuilder_integration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:44:18.000000 pybuilder-integration-98/pybuilder_integration.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 16:44:18.206133 pybuilder-integration-98/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1682 2023-05-25 16:44:16.000000 pybuilder-integration-98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:45:20.212347 pybuilder-integration-99/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-25 20:45:20.212347 pybuilder-integration-99/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:45:20.212347 pybuilder-integration-99/pybuilder_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-25 20:44:45.000000 pybuilder-integration-99/pybuilder_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-05-25 20:44:45.000000 pybuilder-integration-99/pybuilder_integration/artifact_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-25 20:44:45.000000 pybuilder-integration-99/pybuilder_integration/cloudwatchlogs_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-25 20:44:45.000000 pybuilder-integration-99/pybuilder_integration/directory_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-25 20:44:45.000000 pybuilder-integration-99/pybuilder_integration/exec_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-25 20:44:45.000000 pybuilder-integration-99/pybuilder_integration/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-05-25 20:44:45.000000 pybuilder-integration-99/pybuilder_integration/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-25 20:44:45.000000 pybuilder-integration-99/pybuilder_integration/tool_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:45:20.212347 pybuilder-integration-99/pybuilder_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-25 20:45:20.000000 pybuilder-integration-99/pybuilder_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-25 20:45:20.000000 pybuilder-integration-99/pybuilder_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:45:20.000000 pybuilder-integration-99/pybuilder_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:45:20.000000 pybuilder-integration-99/pybuilder_integration.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 20:45:20.000000 pybuilder-integration-99/pybuilder_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 20:45:20.000000 pybuilder-integration-99/pybuilder_integration.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:45:20.000000 pybuilder-integration-99/pybuilder_integration.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 20:45:20.212347 pybuilder-integration-99/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1682 2023-05-25 20:45:18.000000 pybuilder-integration-99/setup.py
```

### Comparing `pybuilder-integration-98/PKG-INFO` & `pybuilder-integration-99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuilder-integration
-Version: 98
+Version: 99
 Summary: A pybuilder plugin that runs integration tests (Tavern & Cypress) against a target.
 Home-page: https://github.com/rspitler/pybuilder-integration
 Author: 
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
```

### Comparing `pybuilder-integration-98/pybuilder_integration/__init__.py` & `pybuilder-integration-99/pybuilder_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-98/pybuilder_integration/artifact_manager.py` & `pybuilder-integration-99/pybuilder_integration/artifact_manager.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-98/pybuilder_integration/cloudwatchlogs_utility.py` & `pybuilder-integration-99/pybuilder_integration/cloudwatchlogs_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-98/pybuilder_integration/directory_utility.py` & `pybuilder-integration-99/pybuilder_integration/directory_utility.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import shutil
 import tempfile
 
 
+
 def prepare_reports_directory(project):
     return prepare_directory("$dir_reports", project)
 
 
 def prepare_logs_directory(project):
     return prepare_directory("$dir_logs", project)
 
@@ -30,20 +31,24 @@
 def get_working_distribution_directory(project):
     dist_directory = prepare_dist_directory(project)
     return _ensure_directory_exists(f"{dist_directory}/working")
 
 
 def get_latest_distribution_directory(project):
     dist_directory = prepare_dist_directory(project)
-    return _ensure_directory_exists(f"{dist_directory}/LATEST")
+    from pybuilder_integration import ENVIRONMENT
+    environment = project.get_mandatory_property(ENVIRONMENT)
+    return _ensure_directory_exists(f"{dist_directory}/LATEST-{environment}")
 
 
 def get_latest_zipped_distribution_directory(project):
     dist_directory = prepare_dist_directory(project)
-    return _ensure_directory_exists(f"{dist_directory}/LATEST/zipped")
+    from pybuilder_integration import ENVIRONMENT
+    environment = project.get_mandatory_property(ENVIRONMENT)
+    return _ensure_directory_exists(f"{dist_directory}/LATEST-{environment}/zipped")
 
 
 def get_local_zip_artifact_path(tool, project, include_ending=False):
     artifact = f"{prepare_dist_directory(project)}/{tool}-{project.name}"
     if include_ending:
         return f"{artifact}.zip"
     return artifact
```

### Comparing `pybuilder-integration-98/pybuilder_integration/exec_utility.py` & `pybuilder-integration-99/pybuilder_integration/exec_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-98/pybuilder_integration/properties.py` & `pybuilder-integration-99/pybuilder_integration/properties.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-98/pybuilder_integration/tasks.py` & `pybuilder-integration-99/pybuilder_integration/tasks.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-98/pybuilder_integration/tool_utility.py` & `pybuilder-integration-99/pybuilder_integration/tool_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-98/pybuilder_integration.egg-info/PKG-INFO` & `pybuilder-integration-99/pybuilder_integration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuilder-integration
-Version: 98
+Version: 99
 Summary: A pybuilder plugin that runs integration tests (Tavern & Cypress) against a target.
 Home-page: https://github.com/rspitler/pybuilder-integration
 Author: 
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
```

### Comparing `pybuilder-integration-98/pybuilder_integration.egg-info/SOURCES.txt` & `pybuilder-integration-99/pybuilder_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-98/setup.py` & `pybuilder-integration-99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'pybuilder-integration',
-        version = '98',
+        version = '99',
         description = 'A pybuilder plugin that runs integration tests (Tavern & Cypress) against a target.',
         long_description = 'A pybuilder plugin that runs integration tests against a target.  This is intended to be a broader scope than unit-tests encompassing dependant functionality.',
         long_description_content_type = None,
         classifiers = [
             'Development Status :: 3 - Alpha',
             'Programming Language :: Python'
         ],
```

