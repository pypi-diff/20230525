# Comparing `tmp/quick_batch-0.1.2.tar.gz` & `tmp/quick_batch-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_batch-0.1.2.tar", max compression
+gzip compressed data, was "quick_batch-0.1.3.tar", max compression
```

## Comparing `quick_batch-0.1.2.tar` & `quick_batch-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     3112 2023-05-24 23:40:19.638964 quick_batch-0.1.2/README.md
--rw-r--r--   0        0        0      658 2023-05-24 23:40:19.642964 quick_batch-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/README.md
--rw-r--r--   0        0        0      120 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/__init__.py
--rw-r--r--   0        0        0      906 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/main.py
--rw-r--r--   0        0        0      288 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/processor_app/Dockerfile
--rwxr-xr-x   0        0        0     1215 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/processor_app/processor_app/__init__.py
--rwxr-xr-x   0        0        0     1594 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/processor_app/processor_app/activate_process.py
--rwxr-xr-x   0        0        0     2234 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/processor_app/processor_app/api_connects.py
--rwxr-xr-x   0        0        0      409 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/processor_app/processor_app/run.py
--rwxr-xr-x   0        0        0       21 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/processor_app/requirements.txt
--rwxr-xr-x   0        0        0     5224 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/processor_app/wait-for-it.sh
--rw-r--r--   0        0        0      241 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/queue_app/Dockerfile
--rw-r--r--   0        0        0     1220 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/queue_app/queue_app/__init__.py
--rw-r--r--   0        0        0     2312 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/queue_app/queue_app/apis.py
--rw-r--r--   0        0        0     3250 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/queue_app/queue_app/queues_init.py
--rw-r--r--   0        0        0      424 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/queue_app/queue_app/run.py
--rwxr-xr-x   0        0        0       21 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/queue_app/requirements.txt
--rwxr-xr-x   0        0        0     5224 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/queue_app/wait-for-it.sh
--rw-r--r--   0        0        0      551 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/utilities/__init__.py
--rw-r--r--   0        0        0     2088 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/utilities/manage_containers.py
--rw-r--r--   0        0        0     3959 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/utilities/manage_images.py
--rw-r--r--   0        0        0     1788 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/utilities/manage_loggers.py
--rw-r--r--   0        0        0      551 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/utilities/manage_networks.py
--rw-r--r--   0        0        0     2487 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/utilities/manage_queue.py
--rw-r--r--   0        0        0     1394 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/utilities/manage_requirements.py
--rw-r--r--   0        0        0     4663 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/utilities/manage_services.py
--rw-r--r--   0        0        0     2395 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/utilities/manage_setup.py
--rw-r--r--   0        0        0      229 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/utilities/manage_swarm.py
--rw-r--r--   0        0        0     3720 2023-05-24 23:40:19.642964 quick_batch-0.1.2/quick_batch/utilities/param_checks.py
--rw-r--r--   0        0        0     3786 1970-01-01 00:00:00.000000 quick_batch-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3112 2023-05-25 03:45:25.046437 quick_batch-0.1.3/README.md
+-rw-r--r--   0        0        0      658 2023-05-25 03:45:25.046437 quick_batch-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 03:45:25.046437 quick_batch-0.1.3/quick_batch/README.md
+-rw-r--r--   0        0        0      120 2023-05-25 03:45:25.046437 quick_batch-0.1.3/quick_batch/__init__.py
+-rw-r--r--   0        0        0      906 2023-05-25 03:45:25.046437 quick_batch-0.1.3/quick_batch/main.py
+-rw-r--r--   0        0        0      368 2023-05-25 03:45:25.046437 quick_batch-0.1.3/quick_batch/processor_app/Dockerfile
+-rwxr-xr-x   0        0        0     1215 2023-05-25 03:45:25.046437 quick_batch-0.1.3/quick_batch/processor_app/processor_app/__init__.py
+-rwxr-xr-x   0        0        0     1594 2023-05-25 03:45:25.046437 quick_batch-0.1.3/quick_batch/processor_app/processor_app/activate_process.py
+-rwxr-xr-x   0        0        0     2234 2023-05-25 03:45:25.046437 quick_batch-0.1.3/quick_batch/processor_app/processor_app/api_connects.py
+-rwxr-xr-x   0        0        0      409 2023-05-25 03:45:25.046437 quick_batch-0.1.3/quick_batch/processor_app/processor_app/run.py
+-rwxr-xr-x   0        0        0       21 2023-05-25 03:45:25.046437 quick_batch-0.1.3/quick_batch/processor_app/requirements.txt
+-rwxr-xr-x   0        0        0     5224 2023-05-25 03:45:25.046437 quick_batch-0.1.3/quick_batch/processor_app/wait-for-it.sh
+-rw-r--r--   0        0        0      241 2023-05-25 03:45:25.046437 quick_batch-0.1.3/quick_batch/queue_app/Dockerfile
+-rw-r--r--   0        0        0     1220 2023-05-25 03:45:25.046437 quick_batch-0.1.3/quick_batch/queue_app/queue_app/__init__.py
+-rw-r--r--   0        0        0     2312 2023-05-25 03:45:25.050437 quick_batch-0.1.3/quick_batch/queue_app/queue_app/apis.py
+-rw-r--r--   0        0        0     3250 2023-05-25 03:45:25.050437 quick_batch-0.1.3/quick_batch/queue_app/queue_app/queues_init.py
+-rw-r--r--   0        0        0      424 2023-05-25 03:45:25.050437 quick_batch-0.1.3/quick_batch/queue_app/queue_app/run.py
+-rwxr-xr-x   0        0        0       21 2023-05-25 03:45:25.050437 quick_batch-0.1.3/quick_batch/queue_app/requirements.txt
+-rwxr-xr-x   0        0        0     5224 2023-05-25 03:45:25.050437 quick_batch-0.1.3/quick_batch/queue_app/wait-for-it.sh
+-rw-r--r--   0        0        0      551 2023-05-25 03:45:25.050437 quick_batch-0.1.3/quick_batch/utilities/__init__.py
+-rw-r--r--   0        0        0     2088 2023-05-25 03:45:25.050437 quick_batch-0.1.3/quick_batch/utilities/manage_containers.py
+-rw-r--r--   0        0        0     3959 2023-05-25 03:45:25.050437 quick_batch-0.1.3/quick_batch/utilities/manage_images.py
+-rw-r--r--   0        0        0     1788 2023-05-25 03:45:25.050437 quick_batch-0.1.3/quick_batch/utilities/manage_loggers.py
+-rw-r--r--   0        0        0      551 2023-05-25 03:45:25.050437 quick_batch-0.1.3/quick_batch/utilities/manage_networks.py
+-rw-r--r--   0        0        0     2487 2023-05-25 03:45:25.050437 quick_batch-0.1.3/quick_batch/utilities/manage_queue.py
+-rw-r--r--   0        0        0     1394 2023-05-25 03:45:25.050437 quick_batch-0.1.3/quick_batch/utilities/manage_requirements.py
+-rw-r--r--   0        0        0     4663 2023-05-25 03:45:25.050437 quick_batch-0.1.3/quick_batch/utilities/manage_services.py
+-rw-r--r--   0        0        0     2395 2023-05-25 03:45:25.050437 quick_batch-0.1.3/quick_batch/utilities/manage_setup.py
+-rw-r--r--   0        0        0      229 2023-05-25 03:45:25.050437 quick_batch-0.1.3/quick_batch/utilities/manage_swarm.py
+-rw-r--r--   0        0        0     3720 2023-05-25 03:45:25.050437 quick_batch-0.1.3/quick_batch/utilities/param_checks.py
+-rw-r--r--   0        0        0     3786 1970-01-01 00:00:00.000000 quick_batch-0.1.3/PKG-INFO
```

### Comparing `quick_batch-0.1.2/README.md` & `quick_batch-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/pyproject.toml` & `quick_batch-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quick_batch"
-version = "0.1.2"
+version = "0.1.3"
 description = "ultra simple command line tool for docker-scaling batch processing"
 authors = ["Jeremy Watt <jermwatt@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jermwatt/quick_batch"
 license = "MIT"
 
 [tool.poetry.scripts]
```

### Comparing `quick_batch-0.1.2/quick_batch/main.py` & `quick_batch-0.1.3/quick_batch/main.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/quick_batch/processor_app/processor_app/__init__.py` & `quick_batch-0.1.3/quick_batch/processor_app/processor_app/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/quick_batch/processor_app/processor_app/activate_process.py` & `quick_batch-0.1.3/quick_batch/processor_app/processor_app/activate_process.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/quick_batch/processor_app/processor_app/api_connects.py` & `quick_batch-0.1.3/quick_batch/processor_app/processor_app/api_connects.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/quick_batch/processor_app/wait-for-it.sh` & `quick_batch-0.1.3/quick_batch/processor_app/wait-for-it.sh`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/quick_batch/queue_app/queue_app/__init__.py` & `quick_batch-0.1.3/quick_batch/queue_app/queue_app/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/quick_batch/queue_app/queue_app/apis.py` & `quick_batch-0.1.3/quick_batch/queue_app/queue_app/apis.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/quick_batch/queue_app/queue_app/queues_init.py` & `quick_batch-0.1.3/quick_batch/queue_app/queue_app/queues_init.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/quick_batch/queue_app/wait-for-it.sh` & `quick_batch-0.1.3/quick_batch/queue_app/wait-for-it.sh`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/quick_batch/utilities/__init__.py` & `quick_batch-0.1.3/quick_batch/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/quick_batch/utilities/manage_containers.py` & `quick_batch-0.1.3/quick_batch/utilities/manage_containers.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/quick_batch/utilities/manage_images.py` & `quick_batch-0.1.3/quick_batch/utilities/manage_images.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/quick_batch/utilities/manage_loggers.py` & `quick_batch-0.1.3/quick_batch/utilities/manage_loggers.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/quick_batch/utilities/manage_networks.py` & `quick_batch-0.1.3/quick_batch/utilities/manage_networks.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/quick_batch/utilities/manage_queue.py` & `quick_batch-0.1.3/quick_batch/utilities/manage_queue.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/quick_batch/utilities/manage_requirements.py` & `quick_batch-0.1.3/quick_batch/utilities/manage_requirements.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/quick_batch/utilities/manage_services.py` & `quick_batch-0.1.3/quick_batch/utilities/manage_services.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/quick_batch/utilities/manage_setup.py` & `quick_batch-0.1.3/quick_batch/utilities/manage_setup.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/quick_batch/utilities/param_checks.py` & `quick_batch-0.1.3/quick_batch/utilities/param_checks.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.2/PKG-INFO` & `quick_batch-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick-batch
-Version: 0.1.2
+Version: 0.1.3
 Summary: ultra simple command line tool for docker-scaling batch processing
 Home-page: https://github.com/jermwatt/quick_batch
 License: MIT
 Author: Jeremy Watt
 Author-email: jermwatt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

