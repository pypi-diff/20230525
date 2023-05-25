# Comparing `tmp/uptime_kuma_api-1.0.0.tar.gz` & `tmp/uptime_kuma_api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uptime_kuma_api-1.0.0.tar", last modified: Thu May 25 19:36:58 2023, max compression
+gzip compressed data, was "uptime_kuma_api-1.0.1.tar", last modified: Thu May 25 21:54:28 2023, max compression
```

## Comparing `uptime_kuma_api-1.0.0.tar` & `uptime_kuma_api-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-05-25 19:36:58.984835 uptime_kuma_api-1.0.0/
--rw-r--r--   0 lucas     (1000) users      (985)     1067 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.0/LICENSE
--rw-r--r--   0 lucas     (1000) users      (985)     3186 2023-05-25 19:36:58.984835 uptime_kuma_api-1.0.0/PKG-INFO
--rw-r--r--   0 lucas     (1000) users      (985)     2057 2023-05-20 17:41:15.000000 uptime_kuma_api-1.0.0/README.md
--rw-r--r--   0 lucas     (1000) users      (985)       38 2023-05-25 19:36:58.984835 uptime_kuma_api-1.0.0/setup.cfg
--rw-r--r--   0 lucas     (1000) users      (985)     1818 2023-05-25 17:51:04.000000 uptime_kuma_api-1.0.0/setup.py
-drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-05-25 19:36:58.981501 uptime_kuma_api-1.0.0/uptime_kuma_api/
--rw-r--r--   0 lucas     (1000) users      (985)      592 2023-05-19 12:02:01.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/__init__.py
--rw-r--r--   0 lucas     (1000) users      (985)      142 2023-05-20 18:50:23.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/__version__.py
--rw-r--r--   0 lucas     (1000) users      (985)   149300 2023-05-25 19:16:46.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/api.py
--rw-r--r--   0 lucas     (1000) users      (985)      326 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/auth_method.py
--rw-r--r--   0 lucas     (1000) users      (985)      169 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/docker_type.py
--rw-r--r--   0 lucas     (1000) users      (985)    29259 2023-05-20 13:03:51.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/docstrings.py
--rw-r--r--   0 lucas     (1000) users      (985)      650 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/event.py
--rw-r--r--   0 lucas     (1000) users      (985)      252 2023-05-19 12:02:01.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/exceptions.py
--rw-r--r--   0 lucas     (1000) users      (985)      324 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/incident_style.py
--rw-r--r--   0 lucas     (1000) users      (985)      515 2023-05-01 18:17:19.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/maintenance_strategy.py
--rw-r--r--   0 lucas     (1000) users      (985)      226 2023-05-19 12:02:01.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/monitor_status.py
--rw-r--r--   0 lucas     (1000) users      (985)      828 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/monitor_type.py
--rw-r--r--   0 lucas     (1000) users      (985)    14475 2023-05-20 12:16:15.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/notification_providers.py
--rw-r--r--   0 lucas     (1000) users      (985)      336 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/proxy_protocol.py
-drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-05-25 19:36:58.984835 uptime_kuma_api-1.0.0/uptime_kuma_api.egg-info/
--rw-r--r--   0 lucas     (1000) users      (985)     3186 2023-05-25 19:36:58.000000 uptime_kuma_api-1.0.0/uptime_kuma_api.egg-info/PKG-INFO
--rw-r--r--   0 lucas     (1000) users      (985)      665 2023-05-25 19:36:58.000000 uptime_kuma_api-1.0.0/uptime_kuma_api.egg-info/SOURCES.txt
--rw-r--r--   0 lucas     (1000) users      (985)        1 2023-05-25 19:36:58.000000 uptime_kuma_api-1.0.0/uptime_kuma_api.egg-info/dependency_links.txt
--rw-r--r--   0 lucas     (1000) users      (985)       41 2023-05-25 19:36:58.000000 uptime_kuma_api-1.0.0/uptime_kuma_api.egg-info/requires.txt
--rw-r--r--   0 lucas     (1000) users      (985)       16 2023-05-25 19:36:58.000000 uptime_kuma_api-1.0.0/uptime_kuma_api.egg-info/top_level.txt
+drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-05-25 21:54:28.427329 uptime_kuma_api-1.0.1/
+-rw-r--r--   0 lucas     (1000) users      (985)     1067 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.1/LICENSE
+-rw-r--r--   0 lucas     (1000) users      (985)     3186 2023-05-25 21:54:28.427329 uptime_kuma_api-1.0.1/PKG-INFO
+-rw-r--r--   0 lucas     (1000) users      (985)     2057 2023-05-20 17:41:15.000000 uptime_kuma_api-1.0.1/README.md
+-rw-r--r--   0 lucas     (1000) users      (985)       38 2023-05-25 21:54:28.427329 uptime_kuma_api-1.0.1/setup.cfg
+-rw-r--r--   0 lucas     (1000) users      (985)     1818 2023-05-25 17:51:04.000000 uptime_kuma_api-1.0.1/setup.py
+drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-05-25 21:54:28.427329 uptime_kuma_api-1.0.1/uptime_kuma_api/
+-rw-r--r--   0 lucas     (1000) users      (985)      592 2023-05-19 12:02:01.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/__init__.py
+-rw-r--r--   0 lucas     (1000) users      (985)      142 2023-05-25 21:52:00.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/__version__.py
+-rw-r--r--   0 lucas     (1000) users      (985)   149456 2023-05-25 21:49:09.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/api.py
+-rw-r--r--   0 lucas     (1000) users      (985)      326 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/auth_method.py
+-rw-r--r--   0 lucas     (1000) users      (985)      169 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/docker_type.py
+-rw-r--r--   0 lucas     (1000) users      (985)    29259 2023-05-20 13:03:51.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/docstrings.py
+-rw-r--r--   0 lucas     (1000) users      (985)      650 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/event.py
+-rw-r--r--   0 lucas     (1000) users      (985)      252 2023-05-19 12:02:01.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/exceptions.py
+-rw-r--r--   0 lucas     (1000) users      (985)      324 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/incident_style.py
+-rw-r--r--   0 lucas     (1000) users      (985)      515 2023-05-01 18:17:19.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/maintenance_strategy.py
+-rw-r--r--   0 lucas     (1000) users      (985)      226 2023-05-19 12:02:01.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/monitor_status.py
+-rw-r--r--   0 lucas     (1000) users      (985)      828 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/monitor_type.py
+-rw-r--r--   0 lucas     (1000) users      (985)    14475 2023-05-20 12:16:15.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/notification_providers.py
+-rw-r--r--   0 lucas     (1000) users      (985)      336 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/proxy_protocol.py
+drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-05-25 21:54:28.427329 uptime_kuma_api-1.0.1/uptime_kuma_api.egg-info/
+-rw-r--r--   0 lucas     (1000) users      (985)     3186 2023-05-25 21:54:28.000000 uptime_kuma_api-1.0.1/uptime_kuma_api.egg-info/PKG-INFO
+-rw-r--r--   0 lucas     (1000) users      (985)      665 2023-05-25 21:54:28.000000 uptime_kuma_api-1.0.1/uptime_kuma_api.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas     (1000) users      (985)        1 2023-05-25 21:54:28.000000 uptime_kuma_api-1.0.1/uptime_kuma_api.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas     (1000) users      (985)       41 2023-05-25 21:54:28.000000 uptime_kuma_api-1.0.1/uptime_kuma_api.egg-info/requires.txt
+-rw-r--r--   0 lucas     (1000) users      (985)       16 2023-05-25 21:54:28.000000 uptime_kuma_api-1.0.1/uptime_kuma_api.egg-info/top_level.txt
```

### Comparing `uptime_kuma_api-1.0.0/LICENSE` & `uptime_kuma_api-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uptime_kuma_api-1.0.0/PKG-INFO` & `uptime_kuma_api-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uptime_kuma_api
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python wrapper for the Uptime Kuma WebSocket API
 Home-page: https://github.com/lucasheld/uptime-kuma-api
 Author: Lucas Held
 Author-email: lucasheld@hotmail.de
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `uptime_kuma_api-1.0.0/README.md` & `uptime_kuma_api-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `uptime_kuma_api-1.0.0/setup.py` & `uptime_kuma_api-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `uptime_kuma_api-1.0.0/uptime_kuma_api/__init__.py` & `uptime_kuma_api-1.0.1/uptime_kuma_api/__init__.py`

 * *Files identical despite different names*

### Comparing `uptime_kuma_api-1.0.0/uptime_kuma_api/api.py` & `uptime_kuma_api-1.0.1/uptime_kuma_api/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,36 +45,39 @@
             int_to_bool(d, keys)
     else:
         for key in keys:
             if key in data:
                 data[key] = True if data[key] == 1 else False
 
 
-def parse_value(data, key, type_) -> None:
+def parse_value(data, key, type_, default=None) -> None:
     if not data:
         return
     if isinstance(data, list):
         for d in data:
-            parse_value(d, key, type_)
+            parse_value(d, key, type_, default)
     else:
         if key in data:
-            data[key] = type_(data[key])
+            if data[key] is not None:
+                data[key] = type_(data[key])
+            elif default is not None:
+                data[key] = default
 
 
 # monitor
 def parse_monitor_status(data) -> None:
     parse_value(data, "status", MonitorStatus)
 
 
 def parse_monitor_type(data) -> None:
     parse_value(data, "type", MonitorType)
 
 
 def parse_auth_method(data) -> None:
-    parse_value(data, "authMethod", AuthMethod)
+    parse_value(data, "authMethod", AuthMethod, AuthMethod.NONE)
 
 
 # notification
 def parse_notification_type(data) -> None:
     parse_value(data, "type", NotificationType)
```

### Comparing `uptime_kuma_api-1.0.0/uptime_kuma_api/docstrings.py` & `uptime_kuma_api-1.0.1/uptime_kuma_api/docstrings.py`

 * *Files identical despite different names*

### Comparing `uptime_kuma_api-1.0.0/uptime_kuma_api/event.py` & `uptime_kuma_api-1.0.1/uptime_kuma_api/event.py`

 * *Files identical despite different names*

### Comparing `uptime_kuma_api-1.0.0/uptime_kuma_api/maintenance_strategy.py` & `uptime_kuma_api-1.0.1/uptime_kuma_api/maintenance_strategy.py`

 * *Files identical despite different names*

### Comparing `uptime_kuma_api-1.0.0/uptime_kuma_api/monitor_type.py` & `uptime_kuma_api-1.0.1/uptime_kuma_api/monitor_type.py`

 * *Files identical despite different names*

### Comparing `uptime_kuma_api-1.0.0/uptime_kuma_api/notification_providers.py` & `uptime_kuma_api-1.0.1/uptime_kuma_api/notification_providers.py`

 * *Files identical despite different names*

### Comparing `uptime_kuma_api-1.0.0/uptime_kuma_api.egg-info/PKG-INFO` & `uptime_kuma_api-1.0.1/uptime_kuma_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uptime-kuma-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python wrapper for the Uptime Kuma WebSocket API
 Home-page: https://github.com/lucasheld/uptime-kuma-api
 Author: Lucas Held
 Author-email: lucasheld@hotmail.de
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `uptime_kuma_api-1.0.0/uptime_kuma_api.egg-info/SOURCES.txt` & `uptime_kuma_api-1.0.1/uptime_kuma_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

