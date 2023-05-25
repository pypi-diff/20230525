# Comparing `tmp/pybuilder-integration-97.tar.gz` & `tmp/pybuilder-integration-98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybuilder-integration-97.tar", last modified: Wed May 24 17:50:25 2023, max compression
+gzip compressed data, was "pybuilder-integration-98.tar", last modified: Thu May 25 16:44:18 2023, max compression
```

## Comparing `pybuilder-integration-97.tar` & `pybuilder-integration-98.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:50:25.246833 pybuilder-integration-97/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-24 17:50:25.246833 pybuilder-integration-97/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:50:25.246833 pybuilder-integration-97/pybuilder_integration/
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-24 17:49:42.000000 pybuilder-integration-97/pybuilder_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-05-24 17:49:42.000000 pybuilder-integration-97/pybuilder_integration/artifact_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-24 17:49:42.000000 pybuilder-integration-97/pybuilder_integration/cloudwatchlogs_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-24 17:49:42.000000 pybuilder-integration-97/pybuilder_integration/directory_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-24 17:49:42.000000 pybuilder-integration-97/pybuilder_integration/exec_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-24 17:49:42.000000 pybuilder-integration-97/pybuilder_integration/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    12758 2023-05-24 17:49:42.000000 pybuilder-integration-97/pybuilder_integration/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-24 17:49:42.000000 pybuilder-integration-97/pybuilder_integration/tool_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:50:25.246833 pybuilder-integration-97/pybuilder_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-24 17:50:25.000000 pybuilder-integration-97/pybuilder_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-24 17:50:25.000000 pybuilder-integration-97/pybuilder_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:50:25.000000 pybuilder-integration-97/pybuilder_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:50:25.000000 pybuilder-integration-97/pybuilder_integration.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-24 17:50:25.000000 pybuilder-integration-97/pybuilder_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 17:50:25.000000 pybuilder-integration-97/pybuilder_integration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:50:25.000000 pybuilder-integration-97/pybuilder_integration.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 17:50:25.246833 pybuilder-integration-97/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1682 2023-05-24 17:50:22.000000 pybuilder-integration-97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:44:18.206133 pybuilder-integration-98/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-25 16:44:18.206133 pybuilder-integration-98/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:44:18.206133 pybuilder-integration-98/pybuilder_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-25 16:43:29.000000 pybuilder-integration-98/pybuilder_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-05-25 16:43:29.000000 pybuilder-integration-98/pybuilder_integration/artifact_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-25 16:43:29.000000 pybuilder-integration-98/pybuilder_integration/cloudwatchlogs_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-25 16:43:29.000000 pybuilder-integration-98/pybuilder_integration/directory_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-25 16:43:29.000000 pybuilder-integration-98/pybuilder_integration/exec_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-25 16:43:29.000000 pybuilder-integration-98/pybuilder_integration/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-05-25 16:43:29.000000 pybuilder-integration-98/pybuilder_integration/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-25 16:43:29.000000 pybuilder-integration-98/pybuilder_integration/tool_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:44:18.206133 pybuilder-integration-98/pybuilder_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-25 16:44:18.000000 pybuilder-integration-98/pybuilder_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-25 16:44:18.000000 pybuilder-integration-98/pybuilder_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:44:18.000000 pybuilder-integration-98/pybuilder_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:44:18.000000 pybuilder-integration-98/pybuilder_integration.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 16:44:18.000000 pybuilder-integration-98/pybuilder_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 16:44:18.000000 pybuilder-integration-98/pybuilder_integration.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:44:18.000000 pybuilder-integration-98/pybuilder_integration.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 16:44:18.206133 pybuilder-integration-98/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1682 2023-05-25 16:44:16.000000 pybuilder-integration-98/setup.py
```

### Comparing `pybuilder-integration-97/PKG-INFO` & `pybuilder-integration-98/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuilder-integration
-Version: 97
+Version: 98
 Summary: A pybuilder plugin that runs integration tests (Tavern & Cypress) against a target.
 Home-page: https://github.com/rspitler/pybuilder-integration
 Author: 
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
```

### Comparing `pybuilder-integration-97/pybuilder_integration/__init__.py` & `pybuilder-integration-98/pybuilder_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-97/pybuilder_integration/artifact_manager.py` & `pybuilder-integration-98/pybuilder_integration/artifact_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
                                          args=args,
                                          failure_message=f"Failed to find bucket",
                                          log_file_name='s3-head-bucket',
                                          project=project,
                                          reactor=reactor,
                                          logger=logger,
                                          raise_exception=True,
-                                         report=True)
+                                         report=False)
 
 
 artifact_managers: Dict[str, S3ArtifactManager] = {}
 manager = S3ArtifactManager()
 artifact_managers[manager.identifier] = manager
```

### Comparing `pybuilder-integration-97/pybuilder_integration/cloudwatchlogs_utility.py` & `pybuilder-integration-98/pybuilder_integration/cloudwatchlogs_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-97/pybuilder_integration/directory_utility.py` & `pybuilder-integration-98/pybuilder_integration/directory_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-97/pybuilder_integration/exec_utility.py` & `pybuilder-integration-98/pybuilder_integration/exec_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-97/pybuilder_integration/properties.py` & `pybuilder-integration-98/pybuilder_integration/properties.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-97/pybuilder_integration/tasks.py` & `pybuilder-integration-98/pybuilder_integration/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     executable = os.path.join(work_dir, "node_modules/cypress/bin/cypress")
     results_file, run_name = get_test_report_file(project=project, test_dir=work_dir, tool="cypress")
     # Run the actual tests against the baseURL provided by ${integration_target}
     test_report_folder = directory_utility.prepare_reports_directory(project)
     args = ["run", "--config",
             f"baseUrl={target_url},"
             f"videosFolder={test_report_folder}/videos,"
-            f"screenshotsFolder={test_report_folder}/screenshots"
+            f"screenshotsFolder={test_report_folder}/screenshots",
             "--reporter-options",
             f"mochaFile={results_file}"]
     if project.get_property("record_cypress", True):
         args.append('--record')
     _add_config_file(logger, project, args, environment, work_dir)
     environment_variables = project.get_property(ENVIRONMENT_VARIABLES, {})
     logger.info(f"Running cypress on host: {target_url}")
```

### Comparing `pybuilder-integration-97/pybuilder_integration/tool_utility.py` & `pybuilder-integration-98/pybuilder_integration/tool_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-97/pybuilder_integration.egg-info/PKG-INFO` & `pybuilder-integration-98/pybuilder_integration.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuilder-integration
-Version: 97
+Version: 98
 Summary: A pybuilder plugin that runs integration tests (Tavern & Cypress) against a target.
 Home-page: https://github.com/rspitler/pybuilder-integration
 Author: 
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
```

### Comparing `pybuilder-integration-97/pybuilder_integration.egg-info/SOURCES.txt` & `pybuilder-integration-98/pybuilder_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-97/setup.py` & `pybuilder-integration-98/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'pybuilder-integration',
-        version = '97',
+        version = '98',
         description = 'A pybuilder plugin that runs integration tests (Tavern & Cypress) against a target.',
         long_description = 'A pybuilder plugin that runs integration tests against a target.  This is intended to be a broader scope than unit-tests encompassing dependant functionality.',
         long_description_content_type = None,
         classifiers = [
             'Development Status :: 3 - Alpha',
             'Programming Language :: Python'
         ],
```

