# Comparing `tmp/common-task-system-client-1.1.1.tar.gz` & `tmp/common-task-system-client-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-task-system-client-1.1.1.tar", last modified: Fri Apr 21 05:43:09 2023, max compression
+gzip compressed data, was "common-task-system-client-1.1.2.tar", last modified: Thu May  4 09:47:26 2023, max compression
```

## Comparing `common-task-system-client-1.1.1.tar` & `common-task-system-client-1.1.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.946641 common-task-system-client-1.1.1/
--rw-rw-rw-   0        0        0     1085 2023-02-20 07:10:46.000000 common-task-system-client-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      302 2023-04-21 05:43:09.946641 common-task-system-client-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-02-20 07:10:46.000000 common-task-system-client-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.925353 common-task-system-client-1.1.1/common_task_system_client.egg-info/
--rw-rw-rw-   0        0        0      302 2023-04-21 05:43:09.000000 common-task-system-client-1.1.1/common_task_system_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1499 2023-04-21 05:43:09.000000 common-task-system-client-1.1.1/common_task_system_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 05:43:09.000000 common-task-system-client-1.1.1/common_task_system_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-21 05:43:09.000000 common-task-system-client-1.1.1/common_task_system_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-21 05:43:09.000000 common-task-system-client-1.1.1/common_task_system_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 05:43:09.946641 common-task-system-client-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      424 2023-04-21 03:23:50.000000 common-task-system-client-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.927354 common-task-system-client-1.1.1/task_system_client/
--rw-rw-rw-   0        0        0        0 2023-02-20 07:12:05.000000 common-task-system-client-1.1.1/task_system_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.929866 common-task-system-client-1.1.1/task_system_client/callback/
--rw-rw-rw-   0        0        0       42 2023-03-17 05:21:49.000000 common-task-system-client-1.1.1/task_system_client/callback/__init__.py
--rw-rw-rw-   0        0        0      490 2023-03-17 06:56:57.000000 common-task-system-client-1.1.1/task_system_client/callback/base.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.931126 common-task-system-client-1.1.1/task_system_client/callback/callbacks/
--rw-rw-rw-   0        0        0        0 2023-03-17 03:52:57.000000 common-task-system-client-1.1.1/task_system_client/callback/callbacks/__init__.py
--rw-rw-rw-   0        0        0      701 2023-03-23 01:18:51.000000 common-task-system-client-1.1.1/task_system_client/callback/callbacks/upload_log.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.932641 common-task-system-client-1.1.1/task_system_client/executor/
--rw-rw-rw-   0        0        0      193 2023-03-14 03:27:53.000000 common-task-system-client-1.1.1/task_system_client/executor/__init__.py
--rw-rw-rw-   0        0        0      390 2023-03-24 06:53:45.000000 common-task-system-client-1.1.1/task_system_client/executor/base.py
--rw-rw-rw-   0        0        0     1913 2023-04-18 05:09:27.000000 common-task-system-client-1.1.1/task_system_client/executor/executor.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.934638 common-task-system-client-1.1.1/task_system_client/handler/
--rw-rw-rw-   0        0        0      277 2023-04-21 03:33:18.000000 common-task-system-client-1.1.1/task_system_client/handler/__init__.py
--rw-rw-rw-   0        0        0      166 2023-04-21 03:13:13.000000 common-task-system-client-1.1.1/task_system_client/handler/base.py
--rw-rw-rw-   0        0        0      694 2023-04-21 03:22:51.000000 common-task-system-client-1.1.1/task_system_client/handler/exception.py
--rw-rw-rw-   0        0        0      382 2023-03-16 03:20:59.000000 common-task-system-client-1.1.1/task_system_client/main.py
--rw-rw-rw-   0        0        0     1888 2023-04-21 05:42:56.000000 common-task-system-client-1.1.1/task_system_client/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.936639 common-task-system-client-1.1.1/task_system_client/subscriber/
--rw-rw-rw-   0        0        0      541 2023-04-21 03:36:06.000000 common-task-system-client-1.1.1/task_system_client/subscriber/__init__.py
--rw-rw-rw-   0        0        0     3327 2023-04-21 03:13:46.000000 common-task-system-client-1.1.1/task_system_client/subscriber/base.py
--rw-rw-rw-   0        0        0     4530 2023-04-21 03:28:45.000000 common-task-system-client-1.1.1/task_system_client/subscriber/threaded.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.938641 common-task-system-client-1.1.1/task_system_client/task_center/
--rw-rw-rw-   0        0        0      130 2023-02-22 05:09:58.000000 common-task-system-client-1.1.1/task_system_client/task_center/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.939638 common-task-system-client-1.1.1/task_system_client/task_center/dispatch/
--rw-rw-rw-   0        0        0      286 2023-02-27 02:22:48.000000 common-task-system-client-1.1.1/task_system_client/task_center/dispatch/__init__.py
--rw-rw-rw-   0        0        0      857 2023-03-17 09:28:16.000000 common-task-system-client-1.1.1/task_system_client/task_center/dispatch/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.943639 common-task-system-client-1.1.1/task_system_client/task_center/subscription/
--rw-rw-rw-   0        0        0      487 2023-02-27 02:22:30.000000 common-task-system-client-1.1.1/task_system_client/task_center/subscription/__init__.py
--rw-rw-rw-   0        0        0     1378 2023-04-21 05:30:08.000000 common-task-system-client-1.1.1/task_system_client/task_center/subscription/base.py
--rw-rw-rw-   0        0        0     1382 2023-04-21 05:13:58.000000 common-task-system-client-1.1.1/task_system_client/task_center/subscription/http.py
--rw-rw-rw-   0        0        0      547 2023-02-27 03:21:04.000000 common-task-system-client-1.1.1/task_system_client/task_center/subscription/redis.py
--rw-rw-rw-   0        0        0      655 2023-02-27 03:14:11.000000 common-task-system-client-1.1.1/task_system_client/task_center/subscription/sql.py
--rw-rw-rw-   0        0        0     2107 2023-04-18 05:09:27.000000 common-task-system-client-1.1.1/task_system_client/task_center/task.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:43:09.945639 common-task-system-client-1.1.1/task_system_client/utils/
--rw-rw-rw-   0        0        0        0 2023-02-20 09:58:14.000000 common-task-system-client-1.1.1/task_system_client/utils/__init__.py
--rw-rw-rw-   0        0        0      428 2023-02-22 03:46:05.000000 common-task-system-client-1.1.1/task_system_client/utils/class_loader.py
--rw-rw-rw-   0        0        0     2627 2023-02-27 01:52:51.000000 common-task-system-client-1.1.1/task_system_client/utils/db_utils.py
--rw-rw-rw-   0        0        0     1068 2023-03-14 03:24:44.000000 common-task-system-client-1.1.1/task_system_client/utils/module_loading.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:47:26.441415 common-task-system-client-1.1.2/
+-rw-rw-rw-   0        0        0     1085 2023-02-20 07:10:46.000000 common-task-system-client-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      302 2023-05-04 09:47:26.441415 common-task-system-client-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-02-20 07:10:46.000000 common-task-system-client-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 09:47:26.424708 common-task-system-client-1.1.2/common_task_system_client.egg-info/
+-rw-rw-rw-   0        0        0      302 2023-05-04 09:47:26.000000 common-task-system-client-1.1.2/common_task_system_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1499 2023-05-04 09:47:26.000000 common-task-system-client-1.1.2/common_task_system_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 09:47:26.000000 common-task-system-client-1.1.2/common_task_system_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-04 09:47:26.000000 common-task-system-client-1.1.2/common_task_system_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-04 09:47:26.000000 common-task-system-client-1.1.2/common_task_system_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 09:47:26.442416 common-task-system-client-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      424 2023-05-04 09:46:00.000000 common-task-system-client-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:47:26.427144 common-task-system-client-1.1.2/task_system_client/
+-rw-rw-rw-   0        0        0        0 2023-02-20 07:12:05.000000 common-task-system-client-1.1.2/task_system_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:47:26.429153 common-task-system-client-1.1.2/task_system_client/callback/
+-rw-rw-rw-   0        0        0       42 2023-03-17 05:21:49.000000 common-task-system-client-1.1.2/task_system_client/callback/__init__.py
+-rw-rw-rw-   0        0        0      490 2023-03-17 06:56:57.000000 common-task-system-client-1.1.2/task_system_client/callback/base.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:47:26.430433 common-task-system-client-1.1.2/task_system_client/callback/callbacks/
+-rw-rw-rw-   0        0        0        0 2023-03-17 03:52:57.000000 common-task-system-client-1.1.2/task_system_client/callback/callbacks/__init__.py
+-rw-rw-rw-   0        0        0      701 2023-03-23 01:18:51.000000 common-task-system-client-1.1.2/task_system_client/callback/callbacks/upload_log.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:47:26.431472 common-task-system-client-1.1.2/task_system_client/executor/
+-rw-rw-rw-   0        0        0      193 2023-03-14 03:27:53.000000 common-task-system-client-1.1.2/task_system_client/executor/__init__.py
+-rw-rw-rw-   0        0        0      390 2023-03-24 06:53:45.000000 common-task-system-client-1.1.2/task_system_client/executor/base.py
+-rw-rw-rw-   0        0        0     1913 2023-04-18 05:09:27.000000 common-task-system-client-1.1.2/task_system_client/executor/executor.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:47:26.432476 common-task-system-client-1.1.2/task_system_client/handler/
+-rw-rw-rw-   0        0        0      277 2023-04-21 03:33:18.000000 common-task-system-client-1.1.2/task_system_client/handler/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-04-21 03:13:13.000000 common-task-system-client-1.1.2/task_system_client/handler/base.py
+-rw-rw-rw-   0        0        0      732 2023-04-21 08:24:39.000000 common-task-system-client-1.1.2/task_system_client/handler/exception.py
+-rw-rw-rw-   0        0        0      382 2023-03-16 03:20:59.000000 common-task-system-client-1.1.2/task_system_client/main.py
+-rw-rw-rw-   0        0        0     1888 2023-04-21 05:42:56.000000 common-task-system-client-1.1.2/task_system_client/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:47:26.434596 common-task-system-client-1.1.2/task_system_client/subscriber/
+-rw-rw-rw-   0        0        0      541 2023-04-21 03:36:06.000000 common-task-system-client-1.1.2/task_system_client/subscriber/__init__.py
+-rw-rw-rw-   0        0        0     3327 2023-04-21 03:13:46.000000 common-task-system-client-1.1.2/task_system_client/subscriber/base.py
+-rw-rw-rw-   0        0        0     4530 2023-04-21 03:28:45.000000 common-task-system-client-1.1.2/task_system_client/subscriber/threaded.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:47:26.435630 common-task-system-client-1.1.2/task_system_client/task_center/
+-rw-rw-rw-   0        0        0      130 2023-02-22 05:09:58.000000 common-task-system-client-1.1.2/task_system_client/task_center/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:47:26.436629 common-task-system-client-1.1.2/task_system_client/task_center/dispatch/
+-rw-rw-rw-   0        0        0      286 2023-02-27 02:22:48.000000 common-task-system-client-1.1.2/task_system_client/task_center/dispatch/__init__.py
+-rw-rw-rw-   0        0        0      857 2023-03-17 09:28:16.000000 common-task-system-client-1.1.2/task_system_client/task_center/dispatch/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:47:26.439398 common-task-system-client-1.1.2/task_system_client/task_center/subscription/
+-rw-rw-rw-   0        0        0      487 2023-02-27 02:22:30.000000 common-task-system-client-1.1.2/task_system_client/task_center/subscription/__init__.py
+-rw-rw-rw-   0        0        0     1378 2023-04-21 05:30:08.000000 common-task-system-client-1.1.2/task_system_client/task_center/subscription/base.py
+-rw-rw-rw-   0        0        0     1382 2023-04-21 05:13:58.000000 common-task-system-client-1.1.2/task_system_client/task_center/subscription/http.py
+-rw-rw-rw-   0        0        0      547 2023-02-27 03:21:04.000000 common-task-system-client-1.1.2/task_system_client/task_center/subscription/redis.py
+-rw-rw-rw-   0        0        0      655 2023-02-27 03:14:11.000000 common-task-system-client-1.1.2/task_system_client/task_center/subscription/sql.py
+-rw-rw-rw-   0        0        0     2140 2023-05-04 09:45:53.000000 common-task-system-client-1.1.2/task_system_client/task_center/task.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:47:26.440415 common-task-system-client-1.1.2/task_system_client/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-20 09:58:14.000000 common-task-system-client-1.1.2/task_system_client/utils/__init__.py
+-rw-rw-rw-   0        0        0      428 2023-02-22 03:46:05.000000 common-task-system-client-1.1.2/task_system_client/utils/class_loader.py
+-rw-rw-rw-   0        0        0     2627 2023-02-27 01:52:51.000000 common-task-system-client-1.1.2/task_system_client/utils/db_utils.py
+-rw-rw-rw-   0        0        0     1068 2023-03-14 03:24:44.000000 common-task-system-client-1.1.2/task_system_client/utils/module_loading.py
```

### Comparing `common-task-system-client-1.1.1/LICENSE` & `common-task-system-client-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.1/common_task_system_client.egg-info/SOURCES.txt` & `common-task-system-client-1.1.2/common_task_system_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.1/task_system_client/callback/callbacks/upload_log.py` & `common-task-system-client-1.1.2/task_system_client/callback/callbacks/upload_log.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.1/task_system_client/executor/executor.py` & `common-task-system-client-1.1.2/task_system_client/executor/executor.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.1/task_system_client/handler/exception.py` & `common-task-system-client-1.1.2/task_system_client/handler/exception.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,12 +19,13 @@
                 break
 
     def __str__(self):
         return self.name
 
 
 class HttpExceptionUpload(ExceptionHandler):
+    name = 'http_exception_upload'
 
     def process(self, e):
         return requests.post(settings.EXCEPTION_REPORT_URL, json={
-            'error': str(e),
+            'content': str(e),
         }).text
```

### Comparing `common-task-system-client-1.1.1/task_system_client/settings.py` & `common-task-system-client-1.1.2/task_system_client/settings.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.1/task_system_client/subscriber/__init__.py` & `common-task-system-client-1.1.2/task_system_client/subscriber/__init__.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.1/task_system_client/subscriber/base.py` & `common-task-system-client-1.1.2/task_system_client/subscriber/base.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.1/task_system_client/subscriber/threaded.py` & `common-task-system-client-1.1.2/task_system_client/subscriber/threaded.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.1/task_system_client/task_center/dispatch/dispatcher.py` & `common-task-system-client-1.1.2/task_system_client/task_center/dispatch/dispatcher.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.1/task_system_client/task_center/subscription/base.py` & `common-task-system-client-1.1.2/task_system_client/task_center/subscription/base.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.1/task_system_client/task_center/subscription/http.py` & `common-task-system-client-1.1.2/task_system_client/task_center/subscription/http.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.1/task_system_client/task_center/subscription/redis.py` & `common-task-system-client-1.1.2/task_system_client/task_center/subscription/redis.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.1/task_system_client/task_center/subscription/sql.py` & `common-task-system-client-1.1.2/task_system_client/task_center/subscription/sql.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.1/task_system_client/task_center/task.py` & `common-task-system-client-1.1.2/task_system_client/task_center/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     def __init__(self, schedule):
         self.schedule_id = schedule['id']
         self.schedule_time = datetime.strptime(schedule['schedule_time'], '%Y-%m-%d %H:%M:%S')
         self.callback = schedule['callback']
         self.task = Task(schedule['task'])
         self.queue = schedule.get('queue', None)
         self.config = schedule.get('config') or {}
+        self.content = schedule
 
     def __str__(self):
         return 'TaskSchedule(id=%s, time=%s, task=%s)' % (
             self.schedule_id, self.schedule_time, self.task
         )
 
     __repr__ = __str__
```

### Comparing `common-task-system-client-1.1.1/task_system_client/utils/db_utils.py` & `common-task-system-client-1.1.2/task_system_client/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.1/task_system_client/utils/module_loading.py` & `common-task-system-client-1.1.2/task_system_client/utils/module_loading.py`

 * *Files identical despite different names*

