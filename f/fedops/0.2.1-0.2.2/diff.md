# Comparing `tmp/fedops-0.2.1.tar.gz` & `tmp/fedops-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedops-0.2.1.tar", last modified: Wed May 24 08:01:18 2023, max compression
+gzip compressed data, was "fedops-0.2.2.tar", last modified: Thu May 25 12:25:32 2023, max compression
```

## Comparing `fedops-0.2.1.tar` & `fedops-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-24 08:01:18.552314 fedops-0.2.1/
--rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-24 08:01:18.552169 fedops-0.2.1/PKG-INFO
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-24 08:01:18.548921 fedops-0.2.1/fedops/
--rw-r--r--   0 yangsemo   (501) staff       (20)      872 2023-05-23 04:42:21.000000 fedops-0.2.1/fedops/__init__.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-24 08:01:18.551071 fedops-0.2.1/fedops/client/
--rw-r--r--   0 yangsemo   (501) staff       (20)      987 2023-05-23 04:42:21.000000 fedops-0.2.1/fedops/client/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     6951 2023-05-24 08:00:46.000000 fedops-0.2.1/fedops/client/app.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     5010 2023-05-22 17:11:45.000000 fedops-0.2.1/fedops/client/app_test.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2817 2023-05-23 04:42:21.000000 fedops-0.2.1/fedops/client/client_api.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     6088 2023-05-23 04:42:21.000000 fedops-0.2.1/fedops/client/client_fl.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     3478 2023-05-23 04:42:21.000000 fedops-0.2.1/fedops/client/client_utils.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2561 2023-05-23 06:06:12.000000 fedops-0.2.1/fedops/client/client_wandb.py
--rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.2.1/fedops/client/test.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-24 08:01:18.551704 fedops-0.2.1/fedops/server/
--rw-r--r--   0 yangsemo   (501) staff       (20)      977 2023-05-23 04:42:21.000000 fedops-0.2.1/fedops/server/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     8963 2023-05-23 05:44:14.000000 fedops-0.2.1/fedops/server/app.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     1283 2023-05-22 17:11:45.000000 fedops-0.2.1/fedops/server/server_api.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     3229 2023-05-23 04:42:21.000000 fedops-0.2.1/fedops/server/server_utils.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-24 08:01:18.551917 fedops-0.2.1/fedops/utils/
--rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.2.1/fedops/utils/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)      832 2023-05-22 17:11:45.000000 fedops-0.2.1/fedops/utils/version.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-24 08:01:18.549629 fedops-0.2.1/fedops.egg-info/
--rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-24 08:01:18.000000 fedops-0.2.1/fedops.egg-info/PKG-INFO
--rw-r--r--   0 yangsemo   (501) staff       (20)      540 2023-05-24 08:01:18.000000 fedops-0.2.1/fedops.egg-info/SOURCES.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)        1 2023-05-24 08:01:18.000000 fedops-0.2.1/fedops.egg-info/dependency_links.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)      187 2023-05-24 08:01:18.000000 fedops-0.2.1/fedops.egg-info/requires.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)        7 2023-05-24 08:01:18.000000 fedops-0.2.1/fedops.egg-info/top_level.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)       38 2023-05-24 08:01:18.552355 fedops-0.2.1/setup.cfg
--rw-r--r--   0 yangsemo   (501) staff       (20)     1130 2023-05-24 08:00:51.000000 fedops-0.2.1/setup.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-25 12:25:32.402588 fedops-0.2.2/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-25 12:25:32.402404 fedops-0.2.2/PKG-INFO
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-25 12:25:32.398780 fedops-0.2.2/fedops/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      872 2023-05-23 04:42:21.000000 fedops-0.2.2/fedops/__init__.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-25 12:25:32.401167 fedops-0.2.2/fedops/client/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      987 2023-05-23 04:42:21.000000 fedops-0.2.2/fedops/client/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     6974 2023-05-25 12:21:10.000000 fedops-0.2.2/fedops/client/app.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     5010 2023-05-22 17:11:45.000000 fedops-0.2.2/fedops/client/app_test.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2817 2023-05-23 04:42:21.000000 fedops-0.2.2/fedops/client/client_api.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     6088 2023-05-23 04:42:21.000000 fedops-0.2.2/fedops/client/client_fl.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     3478 2023-05-23 04:42:21.000000 fedops-0.2.2/fedops/client/client_utils.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2430 2023-05-25 12:17:50.000000 fedops-0.2.2/fedops/client/client_wandb.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.2.2/fedops/client/test.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-25 12:25:32.401893 fedops-0.2.2/fedops/server/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      977 2023-05-23 04:42:21.000000 fedops-0.2.2/fedops/server/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     8963 2023-05-23 05:44:14.000000 fedops-0.2.2/fedops/server/app.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1283 2023-05-22 17:11:45.000000 fedops-0.2.2/fedops/server/server_api.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     3229 2023-05-23 04:42:21.000000 fedops-0.2.2/fedops/server/server_utils.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-25 12:25:32.402162 fedops-0.2.2/fedops/utils/
+-rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.2.2/fedops/utils/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)      832 2023-05-22 17:11:45.000000 fedops-0.2.2/fedops/utils/version.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-25 12:25:32.399510 fedops-0.2.2/fedops.egg-info/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-25 12:25:32.000000 fedops-0.2.2/fedops.egg-info/PKG-INFO
+-rw-r--r--   0 yangsemo   (501) staff       (20)      540 2023-05-25 12:25:32.000000 fedops-0.2.2/fedops.egg-info/SOURCES.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)        1 2023-05-25 12:25:32.000000 fedops-0.2.2/fedops.egg-info/dependency_links.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)      187 2023-05-25 12:25:32.000000 fedops-0.2.2/fedops.egg-info/requires.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)        7 2023-05-25 12:25:32.000000 fedops-0.2.2/fedops.egg-info/top_level.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)       38 2023-05-25 12:25:32.402628 fedops-0.2.2/setup.cfg
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1130 2023-05-25 11:32:29.000000 fedops-0.2.2/setup.py
```

### Comparing `fedops-0.2.1/PKG-INFO` & `fedops-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 0.2.1
+Version: 0.2.2
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-0.2.1/fedops/__init__.py` & `fedops-0.2.2/fedops/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.1/fedops/client/__init__.py` & `fedops-0.2.2/fedops/client/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.1/fedops/client/app.py` & `fedops-0.2.2/fedops/client/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,32 +6,33 @@
 from datetime import datetime
 
 from . import client_utils
 from . import client_fl
 from . import client_wandb
 from . import client_api
 
+
 class FLClientTask():
     def __init__(self, config, fl_task):
         self.app = FastAPI()
-        
+
         self.x_train = fl_task[0]
         self.x_test = fl_task[1]
         self.y_train = fl_task[2]
         self.y_test = fl_task[3]
         self.y_label_counter = fl_task[4]
         self.model = fl_task[5]
         self.model_name = fl_task[6]
         self.task_id = config['task']['name']
         self.dataset = config['data']['name']
         self.label_count = config['data']['label_count']
         self.validation_split = config['data']['validation_split']
         self.wandb_key = config['wandb']['api_key']
         self.wandb_account = config['wandb']['account']
-        
+
         self.status = client_utils.FLClientStatus()
 
     async def fl_client_start(self):
         logging.info('FL learning ready')
 
         logging.info(f'fl_task_id: {self.task_id}')
         logging.info(f'dataset: {self.dataset}')
@@ -81,14 +82,17 @@
             # FL client end time
             fl_end_time = time.time() - fl_start_time
 
             # Wandb log(Client round end time)
             wandb_run.log({"operation_time": fl_end_time, "next_gl_model_v": self.status.FL_next_gl_model},
                           step=self.status.FL_next_gl_model)
 
+            # close wandb
+            wandb_run.finish()
+
             client_all_time_result = {"fl_task_id": self.task_id, "client_mac": self.status.FL_client_mac,
                                       "operation_time": fl_end_time,
                                       "next_gl_model_v": self.status.FL_next_gl_model, "wandb_name": wandb_name}
             json_result = json.dumps(client_all_time_result)
             logging.info(f'client_operation_time - {json_result}')
 
             # Send client_time_result to client_performance pod
@@ -150,22 +154,22 @@
             # get the FL server IP
             self.status.FL_server_IP = client_api.ClientServerAPI(self.task_id).get_port()
 
             # start FL Client
             background_tasks.add_task(self.fl_client_start)
 
             return self.status
-        
+
         try:
             # create client api => to connect client manager
             uvicorn.run(self.app, host='0.0.0.0', port=8002)
 
         except Exception as e:
             # Handle any exceptions that occur during the execution
             logging.error(f'An error occurred during execution: {e}')
 
         finally:
             # FL client out
             client_api.ClientMangerAPI().get_client_out()
             logging.info(f'{self.status.FL_client_mac}-client close')
-            
+
```

### Comparing `fedops-0.2.1/fedops/client/app_test.py` & `fedops-0.2.2/fedops/client/app_test.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.1/fedops/client/client_api.py` & `fedops-0.2.2/fedops/client/client_api.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.1/fedops/client/client_fl.py` & `fedops-0.2.2/fedops/client/client_fl.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.1/fedops/client/client_utils.py` & `fedops-0.2.2/fedops/client/client_utils.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.1/fedops/client/client_wandb.py` & `fedops-0.2.2/fedops/client/client_wandb.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     try:
         # check client system resource usage from wandb
         api = wandb.Api()
         runs = api.runs(f"{wandb_account}/{fl_task_id}")
 
         sys_df = runs[0].history(stream="system")
 
-        col = ['system.network.sent', 'system.network.recv', 'system.disk', '_runtime', 'system.proc.memory.rssMB','system.proc.memory.availableMB', 'system.cpu', 'system.proc.cpu.threads', 'system.memory', 'system.proc.memory.percent', '_timestamp']
-        cols = [c.replace('\n', '') for c in col]
+        cols = ['system.network.sent', 'system.network.recv', 'system.disk', '_runtime', 'system.proc.memory.rssMB','system.proc.memory.availableMB', 'system.cpu', 'system.proc.cpu.threads', 'system.memory', 'system.proc.memory.percent', '_timestamp']
 
         sys_df = sys_df[cols]
 
         sys_df.rename(columns={
             "system.network.sent": "network_sent",
             "system.network.recv": "network_recv",
             "system.disk": "disk",
@@ -63,13 +62,10 @@
             sys_df_row['wandb_name'] = wandb_name
 
             sys_df_row_json = sys_df_row.to_json()
 
             # send client_system  to client_performance pod
             client_api.ClientServerAPI(fl_task_id).put_client_system(sys_df_row_json)
 
-        # close wandb
-        wandb.finish()
-
     except Exception as e:
         logging.error(f'wandb system load error: {e}')
-        wandb.finish() # close wandb
+
```

### Comparing `fedops-0.2.1/fedops/server/__init__.py` & `fedops-0.2.2/fedops/server/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.1/fedops/server/app.py` & `fedops-0.2.2/fedops/server/app.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.1/fedops/server/server_api.py` & `fedops-0.2.2/fedops/server/server_api.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.1/fedops/server/server_utils.py` & `fedops-0.2.2/fedops/server/server_utils.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.1/fedops/utils/version.py` & `fedops-0.2.2/fedops/utils/version.py`

 * *Files identical despite different names*

### Comparing `fedops-0.2.1/fedops.egg-info/PKG-INFO` & `fedops-0.2.2/fedops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 0.2.1
+Version: 0.2.2
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-0.2.1/fedops.egg-info/SOURCES.txt` & `fedops-0.2.2/fedops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fedops-0.2.1/setup.py` & `fedops-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fedops',
-    version='0.2.1',
+    version='0.2.2',
     author='Semo Yang',
     author_email='tpah20@gmail.com',
     description='FL Lifecycle Operations Management Platform',
     long_description='Long description of your library',
     url='https://github.com/gachon-CCLab/FedOps.git',
     packages=find_packages(),
     install_requires=[
```

