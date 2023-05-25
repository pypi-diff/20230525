# Comparing `tmp/recon_lw-2.0.0.dev5068858351.tar.gz` & `tmp/recon_lw-2.0.0.dev5080448744.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5068858351.tar", last modified: Wed May 24 12:50:46 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5080448744.tar", last modified: Thu May 25 13:20:02 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5068858351.tar` & `recon_lw-2.0.0.dev5080448744.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 12:50:46.000000 recon_lw-2.0.0.dev5068858351/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-24 12:50:05.000000 recon_lw-2.0.0.dev5068858351/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-24 12:50:46.000000 recon_lw-2.0.0.dev5068858351/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-24 12:50:05.000000 recon_lw-2.0.0.dev5068858351/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-24 12:50:28.000000 recon_lw-2.0.0.dev5068858351/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 12:50:46.000000 recon_lw-2.0.0.dev5068858351/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-24 12:50:05.000000 recon_lw-2.0.0.dev5068858351/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-24 12:50:05.000000 recon_lw-2.0.0.dev5068858351/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-05-24 12:50:05.000000 recon_lw-2.0.0.dev5068858351/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-24 12:50:05.000000 recon_lw-2.0.0.dev5068858351/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-24 12:50:05.000000 recon_lw-2.0.0.dev5068858351/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    29106 2023-05-24 12:50:05.000000 recon_lw-2.0.0.dev5068858351/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-24 12:50:05.000000 recon_lw-2.0.0.dev5068858351/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 12:50:46.000000 recon_lw-2.0.0.dev5068858351/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-24 12:50:46.000000 recon_lw-2.0.0.dev5068858351/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-24 12:50:46.000000 recon_lw-2.0.0.dev5068858351/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 12:50:46.000000 recon_lw-2.0.0.dev5068858351/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-24 12:50:46.000000 recon_lw-2.0.0.dev5068858351/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-24 12:50:46.000000 recon_lw-2.0.0.dev5068858351/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-24 12:50:05.000000 recon_lw-2.0.0.dev5068858351/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 12:50:46.000000 recon_lw-2.0.0.dev5068858351/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-24 12:50:05.000000 recon_lw-2.0.0.dev5068858351/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 12:50:46.000000 recon_lw-2.0.0.dev5068858351/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-24 12:50:05.000000 recon_lw-2.0.0.dev5068858351/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:20:02.000000 recon_lw-2.0.0.dev5080448744/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-25 13:19:12.000000 recon_lw-2.0.0.dev5080448744/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-25 13:20:02.000000 recon_lw-2.0.0.dev5080448744/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-25 13:19:12.000000 recon_lw-2.0.0.dev5080448744/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-25 13:19:40.000000 recon_lw-2.0.0.dev5080448744/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:20:02.000000 recon_lw-2.0.0.dev5080448744/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-25 13:19:12.000000 recon_lw-2.0.0.dev5080448744/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-25 13:19:12.000000 recon_lw-2.0.0.dev5080448744/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3717 2023-05-25 13:19:12.000000 recon_lw-2.0.0.dev5080448744/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-25 13:19:12.000000 recon_lw-2.0.0.dev5080448744/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-25 13:19:12.000000 recon_lw-2.0.0.dev5080448744/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29706 2023-05-25 13:19:12.000000 recon_lw-2.0.0.dev5080448744/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-25 13:19:12.000000 recon_lw-2.0.0.dev5080448744/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:20:02.000000 recon_lw-2.0.0.dev5080448744/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-25 13:20:02.000000 recon_lw-2.0.0.dev5080448744/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-25 13:20:02.000000 recon_lw-2.0.0.dev5080448744/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 13:20:02.000000 recon_lw-2.0.0.dev5080448744/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-25 13:20:02.000000 recon_lw-2.0.0.dev5080448744/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-25 13:20:02.000000 recon_lw-2.0.0.dev5080448744/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-25 13:19:12.000000 recon_lw-2.0.0.dev5080448744/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 13:20:02.000000 recon_lw-2.0.0.dev5080448744/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-25 13:19:12.000000 recon_lw-2.0.0.dev5080448744/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:20:02.000000 recon_lw-2.0.0.dev5080448744/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-25 13:19:12.000000 recon_lw-2.0.0.dev5080448744/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5068858351/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5080448744/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5068858351/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5080448744/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5068858351/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5080448744/recon_lw/TimeCacheMatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         self._time_index = SortedKeyList(key=lambda t: recon_lw.time_stamp_key(t[0]))
         self._get_timestamp_key1_key2 = get_timestamp_key1_key2
         self._interpret_func = interpret_func
         self._create_event = create_event
         self._send_events = send_events
         self._horizon_delay_seconds = horizon_delay_seconds
         self._custom_settings = custom_settings
-        self._debug = True
+        self._debug = False
 
     def debug(self, body):
         ev = self._create_event("TCMDebug", "TCMDebug", True, body)
         self._send_events([ev])
 
     def process_objects_batch(self, batch: list) -> None:
         stream_time = None
```

### Comparing `recon_lw-2.0.0.dev5068858351/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5080448744/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5068858351/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5080448744/recon_lw/recon_ob.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,23 @@
 
 
 def process_operations_batch(operations_batch, events, book_id ,book, check_book_rule,
                              event_sequence, parent_event,  log_books_filter, log_books_collection,
                              aggregate_batch_updates):
 
     obs = []
+    debug_event = recon_lw.create_event("ROBDebug:" + parent_event["eventName"], "ROBDebug",
+                                          event_sequence,
+                                          ok=False,
+                                          body={"book_id": book_id,
+                                                "operations": [elem[0] for elem in operations_batch],
+                                                "times": [elem[1]["str_time_of_event"] for elem in operations_batch]},
+                                          parentId=parent_event["eventId"])
+    events.append(debug_event)
+
     for operation, parameters, mess in operations_batch:
         initial_book = copy.deepcopy(book)
         initial_parameters = copy.copy(parameters)
         parameters["order_book"] = book
         result, log_entries = operation(**parameters)
         if len(result) > 0:
             result["operation"] = operation.__name__
```

### Comparing `recon_lw-2.0.0.dev5068858351/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5080448744/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5068858351/setup.py` & `recon_lw-2.0.0.dev5080448744/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5068858351/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5080448744/test/test_recon_ob.py`

 * *Files identical despite different names*

