# Comparing `tmp/qoa4ml-0.0.8.tar.gz` & `tmp/qoa4ml-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/tringuyen/workplace/Study/PhD/Gitlab/qoa4ml/dev/package/dist/tmpfw9d8ucm/qoa4ml-0.0.8.tar", last modified: Wed Mar 23 14:33:34 2022, max compression
+gzip compressed data, was "/Users/tringuyen/workplace/Study/PhD/Gitlab/qoa4ml/dev/package/dist/tmp8wasmwge/qoa4ml-0.0.9.tar", last modified: Wed Mar 23 15:38:02 2022, max compression
```

## Comparing `qoa4ml-0.0.8.tar` & `qoa4ml-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:33:34.511565 qoa4ml-0.0.8/
--rw-r--r--   0 tringuyen   (501) wheel        (0)       90 2022-03-23 14:33:16.000000 qoa4ml-0.0.8/CHANGELOG.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.0.8/LICENCE.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       30 2022-03-23 13:04:50.000000 qoa4ml-0.0.8/MANIFEST.in
--rw-r--r--   0 tringuyen   (501) wheel        (0)      385 2022-03-23 14:33:34.511219 qoa4ml-0.0.8/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)       40 2022-03-23 13:08:51.000000 qoa4ml-0.0.8/README.md
--rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-03-23 13:35:28.000000 qoa4ml-0.0.8/pyproject.toml
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:33:34.503222 qoa4ml-0.0.8/qoa4ml/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-18 16:53:28.000000 qoa4ml-0.0.8/qoa4ml/__init__.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:33:34.505958 qoa4ml-0.0.8/qoa4ml/collector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.0.8/qoa4ml/collector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1903 2022-03-23 11:58:56.000000 qoa4ml-0.0.8/qoa4ml/collector/qmqp_collector.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:33:34.507792 qoa4ml-0.0.8/qoa4ml/connector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.0.8/qoa4ml/connector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1794 2022-03-23 10:27:57.000000 qoa4ml-0.0.8/qoa4ml/connector/amqp_client.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.0.8/qoa4ml/connector/mess_logging.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.0.8/qoa4ml/connector/mqtt_client.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.0.8/qoa4ml/connector/prom_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     3240 2022-03-23 11:09:47.000000 qoa4ml-0.0.8/qoa4ml/probes.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:33:34.510296 qoa4ml-0.0.8/qoa4ml/qoa4ml.egg-info/
--rw-r--r--   0 tringuyen   (501) wheel        (0)      554 2022-03-23 13:59:35.000000 qoa4ml-0.0.8/qoa4ml/qoa4ml.egg-info/SOURCES.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2022-03-23 13:59:35.000000 qoa4ml-0.0.8/qoa4ml/qoa4ml.egg-info/dependency_links.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       14 2022-03-23 13:59:35.000000 qoa4ml-0.0.8/qoa4ml/qoa4ml.egg-info/requires.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2022-03-23 13:59:35.000000 qoa4ml-0.0.8/qoa4ml/qoa4ml.egg-info/top_level.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4039 2022-03-23 12:05:46.000000 qoa4ml-0.0.8/qoa4ml/reports.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)      893 2022-03-23 14:32:35.000000 qoa4ml-0.0.8/qoa4ml/utils.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:33:34.505375 qoa4ml-0.0.8/qoa4ml.egg-info/
--rw-r--r--   0 tringuyen   (501) wheel        (0)      385 2022-03-23 14:33:34.000000 qoa4ml-0.0.8/qoa4ml.egg-info/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)      667 2022-03-23 14:33:34.000000 qoa4ml-0.0.8/qoa4ml.egg-info/SOURCES.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2022-03-23 14:33:34.000000 qoa4ml-0.0.8/qoa4ml.egg-info/dependency_links.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       14 2022-03-23 14:33:34.000000 qoa4ml-0.0.8/qoa4ml.egg-info/requires.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2022-03-23 14:33:34.000000 qoa4ml-0.0.8/qoa4ml.egg-info/top_level.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2022-03-23 14:33:34.511670 qoa4ml-0.0.8/setup.cfg
--rw-r--r--   0 tringuyen   (501) wheel        (0)      518 2022-03-23 14:33:08.000000 qoa4ml-0.0.8/setup.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2022-03-23 15:38:02.771130 qoa4ml-0.0.9/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       90 2022-03-23 14:33:16.000000 qoa4ml-0.0.9/CHANGELOG.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.0.9/LICENCE.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       30 2022-03-23 13:04:50.000000 qoa4ml-0.0.9/MANIFEST.in
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      385 2022-03-23 15:38:02.770846 qoa4ml-0.0.9/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       40 2022-03-23 13:08:51.000000 qoa4ml-0.0.9/README.md
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-03-23 13:35:28.000000 qoa4ml-0.0.9/pyproject.toml
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2022-03-23 15:38:02.764143 qoa4ml-0.0.9/qoa4ml/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-18 16:53:28.000000 qoa4ml-0.0.9/qoa4ml/__init__.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2022-03-23 15:38:02.766490 qoa4ml-0.0.9/qoa4ml/collector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.0.9/qoa4ml/collector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1903 2022-03-23 11:58:56.000000 qoa4ml-0.0.9/qoa4ml/collector/qmqp_collector.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2022-03-23 15:38:02.768303 qoa4ml-0.0.9/qoa4ml/connector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.0.9/qoa4ml/connector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1794 2022-03-23 10:27:57.000000 qoa4ml-0.0.9/qoa4ml/connector/amqp_client.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.0.9/qoa4ml/connector/mess_logging.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.0.9/qoa4ml/connector/mqtt_client.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.0.9/qoa4ml/connector/prom_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     3240 2022-03-23 11:09:47.000000 qoa4ml-0.0.9/qoa4ml/probes.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2022-03-23 15:38:02.770238 qoa4ml-0.0.9/qoa4ml/qoa4ml.egg-info/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      554 2022-03-23 13:59:35.000000 qoa4ml-0.0.9/qoa4ml/qoa4ml.egg-info/SOURCES.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2022-03-23 13:59:35.000000 qoa4ml-0.0.9/qoa4ml/qoa4ml.egg-info/dependency_links.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       14 2022-03-23 13:59:35.000000 qoa4ml-0.0.9/qoa4ml/qoa4ml.egg-info/requires.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2022-03-23 13:59:35.000000 qoa4ml-0.0.9/qoa4ml/qoa4ml.egg-info/top_level.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4039 2022-03-23 12:05:46.000000 qoa4ml-0.0.9/qoa4ml/reports.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1281 2022-03-23 15:36:03.000000 qoa4ml-0.0.9/qoa4ml/utils.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2022-03-23 15:38:02.766029 qoa4ml-0.0.9/qoa4ml.egg-info/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      385 2022-03-23 15:38:02.000000 qoa4ml-0.0.9/qoa4ml.egg-info/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      667 2022-03-23 15:38:02.000000 qoa4ml-0.0.9/qoa4ml.egg-info/SOURCES.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2022-03-23 15:38:02.000000 qoa4ml-0.0.9/qoa4ml.egg-info/dependency_links.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       14 2022-03-23 15:38:02.000000 qoa4ml-0.0.9/qoa4ml.egg-info/requires.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2022-03-23 15:38:02.000000 qoa4ml-0.0.9/qoa4ml.egg-info/top_level.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2022-03-23 15:38:02.771231 qoa4ml-0.0.9/setup.cfg
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      518 2022-03-23 15:37:47.000000 qoa4ml-0.0.9/setup.py
```

### Comparing `qoa4ml-0.0.8/LICENCE.txt` & `qoa4ml-0.0.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.8/qoa4ml/collector/qmqp_collector.py` & `qoa4ml-0.0.9/qoa4ml/collector/qmqp_collector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.8/qoa4ml/connector/amqp_client.py` & `qoa4ml-0.0.9/qoa4ml/connector/amqp_client.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.8/qoa4ml/connector/mess_logging.py` & `qoa4ml-0.0.9/qoa4ml/connector/mess_logging.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.8/qoa4ml/connector/mqtt_client.py` & `qoa4ml-0.0.9/qoa4ml/connector/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.8/qoa4ml/connector/prom_connector.py` & `qoa4ml-0.0.9/qoa4ml/connector/prom_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.8/qoa4ml/probes.py` & `qoa4ml-0.0.9/qoa4ml/probes.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.8/qoa4ml/qoa4ml.egg-info/SOURCES.txt` & `qoa4ml-0.0.9/qoa4ml/qoa4ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.8/qoa4ml/reports.py` & `qoa4ml-0.0.9/qoa4ml/reports.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.8/qoa4ml/utils.py` & `qoa4ml-0.0.9/qoa4ml/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-import json, psutil
+from concurrent.futures import thread
+import json, psutil, time
+from qoa4ml.reports import Qoa_Client
+from threading import Thread
 
 def load_config(file_path:str)->dict:
     """
     file_path: file path to load config
     """
     with open(file_path, "r") as f:
         return json.load(f)
@@ -26,8 +29,20 @@
         return psutil.virtual_memory().free
     if key == "total":
         return psutil.virtual_memory().total
     if key == "active":
         return psutil.virtual_memory().active
     if key == "available":
         return psutil.virtual_memory().available
-    return psutil.virtual_memory().used
+    return psutil.virtual_memory().used
+
+
+sys_monitor_flag = False
+
+def system_report(client:Qoa_Client, interval:int):
+    while sys_monitor_flag:
+        print(interval)
+        time.sleep(1)
+
+
+def sys_monitor(client:Qoa_Client, interval:int):
+    sub_thread = Thread(target=system_report, args=(client,interval))
```

### Comparing `qoa4ml-0.0.8/qoa4ml.egg-info/SOURCES.txt` & `qoa4ml-0.0.9/qoa4ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.8/setup.py` & `qoa4ml-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='qoa4ml',
-    version='0.0.8',
+    version='0.0.9',
     description='Quality of Analysis for Machine Learning',
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     long_description_content_type='text/markdown',
     url='https://rdsea.github.io/',
     author='Aaltosea',
     email='tri.m.nguyen@aalto.fi',
     keyword='Monitoring Machine Learning',
```

