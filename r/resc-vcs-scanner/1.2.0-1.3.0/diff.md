# Comparing `tmp/resc_vcs_scanner-1.2.0.tar.gz` & `tmp/resc_vcs_scanner-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_vcs_scanner-1.2.0.tar", last modified: Fri Apr 14 15:09:49 2023, max compression
+gzip compressed data, was "resc_vcs_scanner-1.3.0.tar", last modified: Thu May 25 09:50:49 2023, max compression
```

## Comparing `resc_vcs_scanner-1.2.0.tar` & `resc_vcs_scanner-1.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:49.961434 resc_vcs_scanner-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-04-14 15:09:49.961434 resc_vcs_scanner-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-14 15:09:49.961434 resc_vcs_scanner-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:49.953434 resc_vcs_scanner-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:49.957434 resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-04-14 15:09:49.000000 resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 15:09:49.000000 resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:09:49.000000 resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-14 15:09:49.000000 resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:09:49.000000 resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 15:09:49.000000 resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 15:09:49.000000 resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:49.957434 resc_vcs_scanner-1.2.0/src/vcs_scanner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:49.957434 resc_vcs_scanner-1.2.0/src/vcs_scanner/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/helpers/env_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/helpers/environment_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/helpers/finding_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/input_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/output_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/resc_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:49.961434 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/celery_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14598 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/git_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/rws_api_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12159 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/secret_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/stdout_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:49.961434 resc_vcs_scanner-1.2.0/src/vcs_scanner/static/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-14 15:09:45.000000 resc_vcs_scanner-1.2.0/src/vcs_scanner/static/logging.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:49.854524 resc_vcs_scanner-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-05-25 09:50:49.854524 resc_vcs_scanner-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-25 09:50:49.854524 resc_vcs_scanner-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:49.850524 resc_vcs_scanner-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:49.850524 resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-05-25 09:50:49.000000 resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-25 09:50:49.000000 resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:50:49.000000 resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-25 09:50:49.000000 resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:50:49.000000 resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-25 09:50:49.000000 resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 09:50:49.000000 resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:49.854524 resc_vcs_scanner-1.3.0/src/vcs_scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:49.854524 resc_vcs_scanner-1.3.0/src/vcs_scanner/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/helpers/env_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/helpers/environment_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/helpers/finding_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/output_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/resc_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:49.854524 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/celery_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14598 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/git_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/rws_api_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12159 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/secret_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/stdout_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:49.854524 resc_vcs_scanner-1.3.0/src/vcs_scanner/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/static/logging.ini
```

### Comparing `resc_vcs_scanner-1.2.0/PKG-INFO` & `resc_vcs_scanner-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_vcs_scanner
-Version: 1.2.0
+Version: 1.3.0
 Summary: Repository Scanner - Version Control System - Scanner
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_vcs_scanner-1.2.0/setup.cfg` & `resc_vcs_scanner-1.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = resc_vcs_scanner
 description = Repository Scanner - Version Control System - Scanner
-version = 1.2.0
+version = 1.3.0
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/PKG-INFO` & `resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc-vcs-scanner
-Version: 1.2.0
+Version: 1.3.0
 Summary: Repository Scanner - Version Control System - Scanner
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_vcs_scanner-1.2.0/src/resc_vcs_scanner.egg-info/SOURCES.txt` & `resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.2.0/src/vcs_scanner/common.py` & `resc_vcs_scanner-1.3.0/src/vcs_scanner/common.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.2.0/src/vcs_scanner/helpers/env_default.py` & `resc_vcs_scanner-1.3.0/src/vcs_scanner/helpers/env_default.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.2.0/src/vcs_scanner/helpers/environment_wrapper.py` & `resc_vcs_scanner-1.3.0/src/vcs_scanner/helpers/environment_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.2.0/src/vcs_scanner/input_parser.py` & `resc_vcs_scanner-1.3.0/src/vcs_scanner/input_parser.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.2.0/src/vcs_scanner/model.py` & `resc_vcs_scanner-1.3.0/src/vcs_scanner/model.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.2.0/src/vcs_scanner/output_module.py` & `resc_vcs_scanner-1.3.0/src/vcs_scanner/output_module.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/celery_worker.py` & `resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/celery_worker.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/cli.py` & `resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/cli.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/configuration.py` & `resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/git_operation.py` & `resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/git_operation.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py` & `resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/rws_api_writer.py` & `resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/rws_api_writer.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/secret_scanner.py` & `resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/secret_scanner.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.2.0/src/vcs_scanner/secret_scanners/stdout_writer.py` & `resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/stdout_writer.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.2.0/src/vcs_scanner/static/logging.ini` & `resc_vcs_scanner-1.3.0/src/vcs_scanner/static/logging.ini`

 * *Files identical despite different names*

