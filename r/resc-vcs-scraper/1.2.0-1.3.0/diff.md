# Comparing `tmp/resc_vcs_scraper-1.2.0.tar.gz` & `tmp/resc_vcs_scraper-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_vcs_scraper-1.2.0.tar", last modified: Fri Apr 14 15:09:35 2023, max compression
+gzip compressed data, was "resc_vcs_scraper-1.3.0.tar", last modified: Thu May 25 09:50:43 2023, max compression
```

## Comparing `resc_vcs_scraper-1.2.0.tar` & `resc_vcs_scraper-1.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:35.232214 resc_vcs_scraper-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-14 15:09:35.232214 resc_vcs_scraper-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-14 15:09:35.232214 resc_vcs_scraper-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:35.228213 resc_vcs_scraper-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:35.228213 resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-14 15:09:35.000000 resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-14 15:09:35.000000 resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:09:35.000000 resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-14 15:09:35.000000 resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:09:35.000000 resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-14 15:09:35.000000 resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 15:09:35.000000 resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:35.228213 resc_vcs_scraper-1.2.0/src/vcs_scraper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/dict_remapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/environment_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:35.228213 resc_vcs_scraper-1.2.0/src/vcs_scraper/project_collector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/project_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/project_collector/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:35.228213 resc_vcs_scraper-1.2.0/src/vcs_scraper/repository_collector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/repository_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/repository_collector/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:35.232214 resc_vcs_scraper-1.2.0/src/vcs_scraper/static/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/static/logging.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:35.232214 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/azure_devops_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/azure_devops_data_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/bitbucket_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/bitbucket_data_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/github_public_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/vcs_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/vcs_connector_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-14 15:09:31.000000 resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_instances_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.207305 resc_vcs_scraper-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-25 09:50:43.207305 resc_vcs_scraper-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-25 09:50:43.207305 resc_vcs_scraper-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.203304 resc_vcs_scraper-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.203304 resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-25 09:50:43.000000 resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-25 09:50:43.000000 resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:50:43.000000 resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 09:50:43.000000 resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:50:43.000000 resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-25 09:50:43.000000 resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 09:50:43.000000 resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.207305 resc_vcs_scraper-1.3.0/src/vcs_scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/dict_remapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/environment_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.207305 resc_vcs_scraper-1.3.0/src/vcs_scraper/project_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/project_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/project_collector/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.207305 resc_vcs_scraper-1.3.0/src/vcs_scraper/repository_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/repository_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/repository_collector/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.207305 resc_vcs_scraper-1.3.0/src/vcs_scraper/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/static/logging.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.207305 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/azure_devops_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/azure_devops_data_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/bitbucket_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/bitbucket_data_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/github_public_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/vcs_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/vcs_connector_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_instances_parser.py
```

### Comparing `resc_vcs_scraper-1.2.0/PKG-INFO` & `resc_vcs_scraper-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_vcs_scraper
-Version: 1.2.0
+Version: 1.3.0
 Summary: Repository Scanner - Version Control System - Scraper
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_vcs_scraper-1.2.0/setup.cfg` & `resc_vcs_scraper-1.3.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = resc_vcs_scraper
 description = Repository Scanner - Version Control System - Scraper
-version = 1.2.0
+version = 1.3.0
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/PKG-INFO` & `resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc-vcs-scraper
-Version: 1.2.0
+Version: 1.3.0
 Summary: Repository Scanner - Version Control System - Scraper
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_vcs_scraper-1.2.0/src/resc_vcs_scraper.egg-info/SOURCES.txt` & `resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.2.0/src/vcs_scraper/common.py` & `resc_vcs_scraper-1.3.0/src/vcs_scraper/common.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.2.0/src/vcs_scraper/configuration.py` & `resc_vcs_scraper-1.3.0/src/vcs_scraper/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.2.0/src/vcs_scraper/dict_remapper.py` & `resc_vcs_scraper-1.3.0/src/vcs_scraper/dict_remapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.2.0/src/vcs_scraper/environment_wrapper.py` & `resc_vcs_scraper-1.3.0/src/vcs_scraper/environment_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.2.0/src/vcs_scraper/model.py` & `resc_vcs_scraper-1.3.0/src/vcs_scraper/model.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.2.0/src/vcs_scraper/project_collector/common.py` & `resc_vcs_scraper-1.3.0/src/vcs_scraper/project_collector/common.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.2.0/src/vcs_scraper/repository_collector/common.py` & `resc_vcs_scraper-1.3.0/src/vcs_scraper/repository_collector/common.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.2.0/src/vcs_scraper/static/logging.ini` & `resc_vcs_scraper-1.3.0/src/vcs_scraper/static/logging.ini`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/azure_devops_connector.py` & `resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/azure_devops_connector.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/azure_devops_data_mapper.py` & `resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/azure_devops_data_mapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/bitbucket_connector.py` & `resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/bitbucket_connector.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/bitbucket_data_mapper.py` & `resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/bitbucket_data_mapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/github_public_connector.py` & `resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/github_public_connector.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/vcs_connector.py` & `resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/vcs_connector.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_connectors/vcs_connector_factory.py` & `resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/vcs_connector_factory.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.2.0/src/vcs_scraper/vcs_instances_parser.py` & `resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_instances_parser.py`

 * *Files identical despite different names*

