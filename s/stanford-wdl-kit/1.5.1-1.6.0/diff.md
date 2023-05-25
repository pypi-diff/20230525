# Comparing `tmp/stanford-wdl-kit-1.5.1.tar.gz` & `tmp/stanford-wdl-kit-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stanford-wdl-kit-1.5.1.tar", last modified: Thu Mar  9 19:32:37 2023, max compression
+gzip compressed data, was "stanford-wdl-kit-1.6.0.tar", last modified: Thu May 25 20:09:58 2023, max compression
```

## Comparing `stanford-wdl-kit-1.5.1.tar` & `stanford-wdl-kit-1.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 cloudsdk  (1000) cloudsdk  (1000)        0 2023-03-09 19:32:37.484300 stanford-wdl-kit-1.5.1/
--rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)     1696 2023-03-09 19:32:37.484300 stanford-wdl-kit-1.5.1/PKG-INFO
-drwxr-xr-x   0 cloudsdk  (1000) cloudsdk  (1000)        0 2023-03-09 19:32:37.484300 stanford-wdl-kit-1.5.1/gcp/
--rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)    19960 2023-03-09 19:29:34.000000 stanford-wdl-kit-1.5.1/gcp/bigquery.py
--rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)    13561 2023-03-09 19:29:34.000000 stanford-wdl-kit-1.5.1/gcp/cloudsql.py
--rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)     7917 2023-03-09 19:29:34.000000 stanford-wdl-kit-1.5.1/gcp/gcs.py
--rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)       38 2023-03-09 19:32:37.484300 stanford-wdl-kit-1.5.1/setup.cfg
--rwxr-xr-x   0 cloudsdk  (1000) cloudsdk  (1000)     4132 2023-03-09 19:32:37.000000 stanford-wdl-kit-1.5.1/setup.py
-drwxr-xr-x   0 cloudsdk  (1000) cloudsdk  (1000)        0 2023-03-09 19:32:37.484300 stanford-wdl-kit-1.5.1/stanford_wdl_kit.egg-info/
--rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)     1696 2023-03-09 19:32:37.000000 stanford-wdl-kit-1.5.1/stanford_wdl_kit.egg-info/PKG-INFO
--rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)      444 2023-03-09 19:32:37.000000 stanford-wdl-kit-1.5.1/stanford_wdl_kit.egg-info/SOURCES.txt
--rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)        1 2023-03-09 19:32:37.000000 stanford-wdl-kit-1.5.1/stanford_wdl_kit.egg-info/dependency_links.txt
--rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)      198 2023-03-09 19:32:37.000000 stanford-wdl-kit-1.5.1/stanford_wdl_kit.egg-info/entry_points.txt
--rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)        1 2023-03-09 19:32:37.000000 stanford-wdl-kit-1.5.1/stanford_wdl_kit.egg-info/namespace_packages.txt
--rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)      455 2023-03-09 19:32:37.000000 stanford-wdl-kit-1.5.1/stanford_wdl_kit.egg-info/requires.txt
--rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)       10 2023-03-09 19:32:37.000000 stanford-wdl-kit-1.5.1/stanford_wdl_kit.egg-info/top_level.txt
--rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)        1 2023-03-09 19:32:37.000000 stanford-wdl-kit-1.5.1/stanford_wdl_kit.egg-info/zip-safe
-drwxr-xr-x   0 cloudsdk  (1000) cloudsdk  (1000)        0 2023-03-09 19:32:37.484300 stanford-wdl-kit-1.5.1/utils/
--rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)    29915 2023-03-09 19:29:34.000000 stanford-wdl-kit-1.5.1/utils/backup.py
--rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)     3074 2023-03-09 19:29:34.000000 stanford-wdl-kit-1.5.1/utils/mailer.py
--rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)     2623 2023-03-09 19:29:34.000000 stanford-wdl-kit-1.5.1/utils/slacker.py
--rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)     2783 2023-03-09 19:29:34.000000 stanford-wdl-kit-1.5.1/utils/yaml2wdl.py
+drwxr-xr-x   0 cloudsdk  (1000) cloudsdk  (1000)        0 2023-05-25 20:09:58.248603 stanford-wdl-kit-1.6.0/
+-rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)     1696 2023-05-25 20:09:58.248603 stanford-wdl-kit-1.6.0/PKG-INFO
+drwxr-xr-x   0 cloudsdk  (1000) cloudsdk  (1000)        0 2023-05-25 20:09:58.248603 stanford-wdl-kit-1.6.0/gcp/
+-rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)    19960 2023-05-25 20:06:52.000000 stanford-wdl-kit-1.6.0/gcp/bigquery.py
+-rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)    13561 2023-05-25 20:06:52.000000 stanford-wdl-kit-1.6.0/gcp/cloudsql.py
+-rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)     7917 2023-05-25 20:06:52.000000 stanford-wdl-kit-1.6.0/gcp/gcs.py
+-rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)       38 2023-05-25 20:09:58.248603 stanford-wdl-kit-1.6.0/setup.cfg
+-rwxr-xr-x   0 cloudsdk  (1000) cloudsdk  (1000)     4132 2023-05-25 20:09:57.000000 stanford-wdl-kit-1.6.0/setup.py
+drwxr-xr-x   0 cloudsdk  (1000) cloudsdk  (1000)        0 2023-05-25 20:09:58.248603 stanford-wdl-kit-1.6.0/stanford_wdl_kit.egg-info/
+-rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)     1696 2023-05-25 20:09:58.000000 stanford-wdl-kit-1.6.0/stanford_wdl_kit.egg-info/PKG-INFO
+-rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)      444 2023-05-25 20:09:58.000000 stanford-wdl-kit-1.6.0/stanford_wdl_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)        1 2023-05-25 20:09:58.000000 stanford-wdl-kit-1.6.0/stanford_wdl_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)      198 2023-05-25 20:09:58.000000 stanford-wdl-kit-1.6.0/stanford_wdl_kit.egg-info/entry_points.txt
+-rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)        1 2023-05-25 20:09:58.000000 stanford-wdl-kit-1.6.0/stanford_wdl_kit.egg-info/namespace_packages.txt
+-rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)      455 2023-05-25 20:09:58.000000 stanford-wdl-kit-1.6.0/stanford_wdl_kit.egg-info/requires.txt
+-rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)       10 2023-05-25 20:09:58.000000 stanford-wdl-kit-1.6.0/stanford_wdl_kit.egg-info/top_level.txt
+-rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)        1 2023-05-25 20:09:58.000000 stanford-wdl-kit-1.6.0/stanford_wdl_kit.egg-info/zip-safe
+drwxr-xr-x   0 cloudsdk  (1000) cloudsdk  (1000)        0 2023-05-25 20:09:58.248603 stanford-wdl-kit-1.6.0/utils/
+-rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)    29915 2023-05-25 20:06:52.000000 stanford-wdl-kit-1.6.0/utils/backup.py
+-rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)     3074 2023-05-25 20:06:52.000000 stanford-wdl-kit-1.6.0/utils/mailer.py
+-rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)     2623 2023-05-25 20:06:52.000000 stanford-wdl-kit-1.6.0/utils/slacker.py
+-rw-r--r--   0 cloudsdk  (1000) cloudsdk  (1000)     2783 2023-05-25 20:06:52.000000 stanford-wdl-kit-1.6.0/utils/yaml2wdl.py
```

### Comparing `stanford-wdl-kit-1.5.1/PKG-INFO` & `stanford-wdl-kit-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stanford-wdl-kit
-Version: 1.5.1
+Version: 1.6.0
 Summary: A WDL toolkit with a focus on ETL and Cloud integration
 Home-page: https://github.com/susom/wdl-kit
 Author: Darren Guan, Joe Mesterhazy, Tyler Tollefson, Smita Limaye, Jay Chen
 Author-email: dguan2@stanford.edu, jmesterh@stanford.edu, tjt8712@stanford.edu, slimaye@stanford.edu, jchen313@stanford.edu
 Maintainer: Research IT: Technology & Digital Solutions, Stanford Medicine
 Maintainer-email: rit-oss-admin@stanford.edu
 License: Apache License, Version 2.0
```

### Comparing `stanford-wdl-kit-1.5.1/gcp/bigquery.py` & `stanford-wdl-kit-1.6.0/gcp/bigquery.py`

 * *Files identical despite different names*

### Comparing `stanford-wdl-kit-1.5.1/gcp/cloudsql.py` & `stanford-wdl-kit-1.6.0/gcp/cloudsql.py`

 * *Files identical despite different names*

### Comparing `stanford-wdl-kit-1.5.1/gcp/gcs.py` & `stanford-wdl-kit-1.6.0/gcp/gcs.py`

 * *Files identical despite different names*

### Comparing `stanford-wdl-kit-1.5.1/setup.py` & `stanford-wdl-kit-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'stanford-wdl-kit',
-        version = '1.5.1',
+        version = '1.6.0',
         description = 'A WDL toolkit with a focus on ETL and Cloud integration',
         long_description = '# WDL-kit\n## A WDL toolkit with a focus on ETL and Cloud integration\n\nWDL-kit is a collection of dockerized utilities to simplify the creation of ETL-like workflows in the Workflow Definition Language. \n\n## Features\n\n* YAML-to-WDL\n  \n  Converts .yaml files into .wdl tasks. This is primarily a workaround for the WDL language not supporting multi-line strings, which is problematic for SQL ETL workflows. \n\n* Google Cloud\n\n  Wrappers for BigQuery, Google Cloud Storage, etc. \n\n* Slack\n\n  Wrapper for sending Slack messages\n\n* MailGun\n\n  Wrapper for sending mail via MailGun',
         long_description_content_type = 'text/markdown',
         classifiers = [
             'Programming Language :: Python',
             'Programming Language :: Python :: Implementation :: PyPy',
             'Programming Language :: Python :: 3',
```

### Comparing `stanford-wdl-kit-1.5.1/stanford_wdl_kit.egg-info/PKG-INFO` & `stanford-wdl-kit-1.6.0/stanford_wdl_kit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stanford-wdl-kit
-Version: 1.5.1
+Version: 1.6.0
 Summary: A WDL toolkit with a focus on ETL and Cloud integration
 Home-page: https://github.com/susom/wdl-kit
 Author: Darren Guan, Joe Mesterhazy, Tyler Tollefson, Smita Limaye, Jay Chen
 Author-email: dguan2@stanford.edu, jmesterh@stanford.edu, tjt8712@stanford.edu, slimaye@stanford.edu, jchen313@stanford.edu
 Maintainer: Research IT: Technology & Digital Solutions, Stanford Medicine
 Maintainer-email: rit-oss-admin@stanford.edu
 License: Apache License, Version 2.0
```

### Comparing `stanford-wdl-kit-1.5.1/utils/backup.py` & `stanford-wdl-kit-1.6.0/utils/backup.py`

 * *Files identical despite different names*

### Comparing `stanford-wdl-kit-1.5.1/utils/mailer.py` & `stanford-wdl-kit-1.6.0/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `stanford-wdl-kit-1.5.1/utils/slacker.py` & `stanford-wdl-kit-1.6.0/utils/slacker.py`

 * *Files identical despite different names*

### Comparing `stanford-wdl-kit-1.5.1/utils/yaml2wdl.py` & `stanford-wdl-kit-1.6.0/utils/yaml2wdl.py`

 * *Files identical despite different names*

