# Comparing `tmp/quick_batch-0.1.0.tar.gz` & `tmp/quick_batch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_batch-0.1.0.tar", max compression
+gzip compressed data, was "quick_batch-0.1.1.tar", max compression
```

## Comparing `quick_batch-0.1.0.tar` & `quick_batch-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      155 2023-05-23 21:28:39.112895 quick_batch-0.1.0/README.md
--rw-r--r--   0        0        0      696 2023-05-23 22:25:09.227420 quick_batch-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-23 21:28:39.113594 quick_batch-0.1.0/quick_batch/README.md
--rw-r--r--   0        0        0      120 2023-05-23 21:28:39.113722 quick_batch-0.1.0/quick_batch/__init__.py
--rw-r--r--   0        0        0      906 2023-05-23 22:35:29.379320 quick_batch-0.1.0/quick_batch/main.py
--rw-r--r--   0        0        0      636 2023-05-23 21:28:39.113961 quick_batch-0.1.0/quick_batch/processor_app/Dockerfile
--rwxr-xr-x   0        0        0     1215 2023-05-23 21:28:39.114116 quick_batch-0.1.0/quick_batch/processor_app/processor_app/__init__.py
--rwxr-xr-x   0        0        0     1594 2023-05-23 21:28:39.114213 quick_batch-0.1.0/quick_batch/processor_app/processor_app/activate_process.py
--rwxr-xr-x   0        0        0     2234 2023-05-23 21:28:39.114323 quick_batch-0.1.0/quick_batch/processor_app/processor_app/api_connects.py
--rwxr-xr-x   0        0        0      409 2023-05-23 21:28:39.114415 quick_batch-0.1.0/quick_batch/processor_app/processor_app/run.py
--rwxr-xr-x   0        0        0       21 2023-05-23 21:28:39.114500 quick_batch-0.1.0/quick_batch/processor_app/requirements.txt
--rwxr-xr-x   0        0        0     5224 2023-05-23 21:28:39.114611 quick_batch-0.1.0/quick_batch/processor_app/wait-for-it.sh
--rw-r--r--   0        0        0      241 2023-05-23 21:28:39.114756 quick_batch-0.1.0/quick_batch/queue_app/Dockerfile
--rw-r--r--   0        0        0     1220 2023-05-23 21:28:39.114913 quick_batch-0.1.0/quick_batch/queue_app/queue_app/__init__.py
--rw-r--r--   0        0        0     2312 2023-05-23 21:28:39.115024 quick_batch-0.1.0/quick_batch/queue_app/queue_app/apis.py
--rw-r--r--   0        0        0     3250 2023-05-23 21:28:39.115129 quick_batch-0.1.0/quick_batch/queue_app/queue_app/queues_init.py
--rw-r--r--   0        0        0      424 2023-05-23 21:28:39.115220 quick_batch-0.1.0/quick_batch/queue_app/queue_app/run.py
--rwxr-xr-x   0        0        0       21 2023-05-23 21:28:39.115312 quick_batch-0.1.0/quick_batch/queue_app/requirements.txt
--rwxr-xr-x   0        0        0     5224 2023-05-23 21:28:39.115422 quick_batch-0.1.0/quick_batch/queue_app/wait-for-it.sh
--rw-r--r--   0        0        0      551 2023-05-23 21:28:39.115577 quick_batch-0.1.0/quick_batch/utilities/__init__.py
--rw-r--r--   0        0        0     2092 2023-05-23 21:28:39.115680 quick_batch-0.1.0/quick_batch/utilities/manage_containers.py
--rw-r--r--   0        0        0     2016 2023-05-23 21:28:39.115788 quick_batch-0.1.0/quick_batch/utilities/manage_images.py
--rw-r--r--   0        0        0     1788 2023-05-23 21:28:39.115881 quick_batch-0.1.0/quick_batch/utilities/manage_loggers.py
--rw-r--r--   0        0        0      551 2023-05-23 21:28:39.115972 quick_batch-0.1.0/quick_batch/utilities/manage_networks.py
--rw-r--r--   0        0        0     2487 2023-05-23 21:28:39.116062 quick_batch-0.1.0/quick_batch/utilities/manage_queue.py
--rw-r--r--   0        0        0     1394 2023-05-23 21:28:39.116156 quick_batch-0.1.0/quick_batch/utilities/manage_requirements.py
--rw-r--r--   0        0        0     4663 2023-05-23 21:28:39.116255 quick_batch-0.1.0/quick_batch/utilities/manage_services.py
--rw-r--r--   0        0        0     2395 2023-05-23 21:28:39.116371 quick_batch-0.1.0/quick_batch/utilities/manage_setup.py
--rw-r--r--   0        0        0      229 2023-05-23 21:28:39.116460 quick_batch-0.1.0/quick_batch/utilities/manage_swarm.py
--rw-r--r--   0        0        0     3720 2023-05-23 21:28:39.116564 quick_batch-0.1.0/quick_batch/utilities/param_checks.py
--rw-r--r--   0        0        0      832 1970-01-01 00:00:00.000000 quick_batch-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2919 2023-05-24 13:31:33.914938 quick_batch-0.1.1/README.md
+-rw-r--r--   0        0        0      658 2023-05-24 13:31:33.918938 quick_batch-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/README.md
+-rw-r--r--   0        0        0      120 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/__init__.py
+-rw-r--r--   0        0        0      906 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/main.py
+-rw-r--r--   0        0        0      636 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/processor_app/Dockerfile
+-rwxr-xr-x   0        0        0     1215 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/processor_app/processor_app/__init__.py
+-rwxr-xr-x   0        0        0     1594 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/processor_app/processor_app/activate_process.py
+-rwxr-xr-x   0        0        0     2234 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/processor_app/processor_app/api_connects.py
+-rwxr-xr-x   0        0        0      409 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/processor_app/processor_app/run.py
+-rwxr-xr-x   0        0        0       21 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/processor_app/requirements.txt
+-rwxr-xr-x   0        0        0     5224 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/processor_app/wait-for-it.sh
+-rw-r--r--   0        0        0      241 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/queue_app/Dockerfile
+-rw-r--r--   0        0        0     1220 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/queue_app/queue_app/__init__.py
+-rw-r--r--   0        0        0     2312 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/queue_app/queue_app/apis.py
+-rw-r--r--   0        0        0     3250 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/queue_app/queue_app/queues_init.py
+-rw-r--r--   0        0        0      424 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/queue_app/queue_app/run.py
+-rwxr-xr-x   0        0        0       21 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/queue_app/requirements.txt
+-rwxr-xr-x   0        0        0     5224 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/queue_app/wait-for-it.sh
+-rw-r--r--   0        0        0      551 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/utilities/__init__.py
+-rw-r--r--   0        0        0     2088 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/utilities/manage_containers.py
+-rw-r--r--   0        0        0     2016 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/utilities/manage_images.py
+-rw-r--r--   0        0        0     1788 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/utilities/manage_loggers.py
+-rw-r--r--   0        0        0      551 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/utilities/manage_networks.py
+-rw-r--r--   0        0        0     2487 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/utilities/manage_queue.py
+-rw-r--r--   0        0        0     1394 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/utilities/manage_requirements.py
+-rw-r--r--   0        0        0     4663 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/utilities/manage_services.py
+-rw-r--r--   0        0        0     2395 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/utilities/manage_setup.py
+-rw-r--r--   0        0        0      229 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/utilities/manage_swarm.py
+-rw-r--r--   0        0        0     3720 2023-05-24 13:31:33.918938 quick_batch-0.1.1/quick_batch/utilities/param_checks.py
+-rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 quick_batch-0.1.1/PKG-INFO
```

### Comparing `quick_batch-0.1.0/pyproject.toml` & `quick_batch-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 [tool.poetry]
 name = "quick_batch"
-version = "0.1.0"
-description = "ultra simple python + docker scaling for quick batch processing"
+version = "0.1.1"
+description = "ultra simple command line tool for docker-scaling batch processing"
 authors = ["Jeremy Watt <jermwatt@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jermwatt/quick_batch"
 license = "MIT"
-# packages = [{include = "quick_batch"}]
 
 [tool.poetry.scripts]
 quick_batch = "quick_batch.main:main"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `quick_batch-0.1.0/quick_batch/main.py` & `quick_batch-0.1.1/quick_batch/main.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.0/quick_batch/processor_app/Dockerfile` & `quick_batch-0.1.1/quick_batch/processor_app/Dockerfile`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.0/quick_batch/processor_app/processor_app/__init__.py` & `quick_batch-0.1.1/quick_batch/processor_app/processor_app/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.0/quick_batch/processor_app/processor_app/activate_process.py` & `quick_batch-0.1.1/quick_batch/processor_app/processor_app/activate_process.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.0/quick_batch/processor_app/processor_app/api_connects.py` & `quick_batch-0.1.1/quick_batch/processor_app/processor_app/api_connects.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.0/quick_batch/processor_app/wait-for-it.sh` & `quick_batch-0.1.1/quick_batch/processor_app/wait-for-it.sh`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.0/quick_batch/queue_app/queue_app/__init__.py` & `quick_batch-0.1.1/quick_batch/queue_app/queue_app/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.0/quick_batch/queue_app/queue_app/apis.py` & `quick_batch-0.1.1/quick_batch/queue_app/queue_app/apis.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.0/quick_batch/queue_app/queue_app/queues_init.py` & `quick_batch-0.1.1/quick_batch/queue_app/queue_app/queues_init.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.0/quick_batch/queue_app/wait-for-it.sh` & `quick_batch-0.1.1/quick_batch/queue_app/wait-for-it.sh`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.0/quick_batch/utilities/__init__.py` & `quick_batch-0.1.1/quick_batch/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.0/quick_batch/utilities/manage_containers.py` & `quick_batch-0.1.1/quick_batch/utilities/manage_containers.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
         container.remove(force=True)
 
 
 # start queue_app docker container with interactive terminal
 @log_exceptions
 def startup_queue_app_container(client, config_path, input_path):
     queue_container = client.containers.run(
-        image='quick_batch_queue_app',
-        network='quick_batch_network',
+        image='quickbatch_queue_app',
+        network='quickbatch_network',
         detach=True,
         name='queue_app',
         tty=True,
         stdin_open=True,
         ports={'80/tcp': 80},
         volumes={
             queue_path + '/queue_app':
@@ -36,16 +36,16 @@
 
 
 # start queue_app docker container with interactive terminal
 @log_exceptions
 def startup_processor_app(client, config_path, input_path, output_path):
     # start processor_app docker container with interactive terminal
     processor_container = client.containers.run(
-        image='quick_batch_processor_app',
-        network='quick_batch_network',
+        image='quickbatch_processor_app',
+        network='quickbatch_network',
         detach=True,
         name='processor_app',
         tty=True,
         stdin_open=True,
         ports={'80/tcp': None},
         volumes={
             processor_path + '/processor_app':
```

### Comparing `quick_batch-0.1.0/quick_batch/utilities/manage_images.py` & `quick_batch-0.1.1/quick_batch/utilities/manage_images.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.0/quick_batch/utilities/manage_loggers.py` & `quick_batch-0.1.1/quick_batch/utilities/manage_loggers.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.0/quick_batch/utilities/manage_networks.py` & `quick_batch-0.1.1/quick_batch/utilities/manage_networks.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.0/quick_batch/utilities/manage_queue.py` & `quick_batch-0.1.1/quick_batch/utilities/manage_queue.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.0/quick_batch/utilities/manage_requirements.py` & `quick_batch-0.1.1/quick_batch/utilities/manage_requirements.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.0/quick_batch/utilities/manage_services.py` & `quick_batch-0.1.1/quick_batch/utilities/manage_services.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.0/quick_batch/utilities/manage_setup.py` & `quick_batch-0.1.1/quick_batch/utilities/manage_setup.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.0/quick_batch/utilities/param_checks.py` & `quick_batch-0.1.1/quick_batch/utilities/param_checks.py`

 * *Files identical despite different names*

