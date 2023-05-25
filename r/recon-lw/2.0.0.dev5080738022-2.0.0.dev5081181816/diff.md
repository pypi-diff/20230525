# Comparing `tmp/recon_lw-2.0.0.dev5080738022.tar.gz` & `tmp/recon_lw-2.0.0.dev5081181816.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5080738022.tar", last modified: Thu May 25 13:49:50 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5081181816.tar", last modified: Thu May 25 14:32:20 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5080738022.tar` & `recon_lw-2.0.0.dev5081181816.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:49:50.000000 recon_lw-2.0.0.dev5080738022/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-25 13:49:03.000000 recon_lw-2.0.0.dev5080738022/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-25 13:49:50.000000 recon_lw-2.0.0.dev5080738022/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-25 13:49:03.000000 recon_lw-2.0.0.dev5080738022/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-25 13:49:24.000000 recon_lw-2.0.0.dev5080738022/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:49:50.000000 recon_lw-2.0.0.dev5080738022/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-25 13:49:03.000000 recon_lw-2.0.0.dev5080738022/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-25 13:49:03.000000 recon_lw-2.0.0.dev5080738022/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3717 2023-05-25 13:49:03.000000 recon_lw-2.0.0.dev5080738022/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-25 13:49:03.000000 recon_lw-2.0.0.dev5080738022/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-25 13:49:03.000000 recon_lw-2.0.0.dev5080738022/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    29715 2023-05-25 13:49:03.000000 recon_lw-2.0.0.dev5080738022/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-25 13:49:03.000000 recon_lw-2.0.0.dev5080738022/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:49:50.000000 recon_lw-2.0.0.dev5080738022/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-25 13:49:50.000000 recon_lw-2.0.0.dev5080738022/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-25 13:49:50.000000 recon_lw-2.0.0.dev5080738022/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 13:49:50.000000 recon_lw-2.0.0.dev5080738022/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-25 13:49:50.000000 recon_lw-2.0.0.dev5080738022/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-25 13:49:50.000000 recon_lw-2.0.0.dev5080738022/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-25 13:49:03.000000 recon_lw-2.0.0.dev5080738022/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 13:49:50.000000 recon_lw-2.0.0.dev5080738022/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-25 13:49:03.000000 recon_lw-2.0.0.dev5080738022/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:49:50.000000 recon_lw-2.0.0.dev5080738022/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-25 13:49:03.000000 recon_lw-2.0.0.dev5080738022/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 14:32:20.000000 recon_lw-2.0.0.dev5081181816/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-25 14:31:27.000000 recon_lw-2.0.0.dev5081181816/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-25 14:32:20.000000 recon_lw-2.0.0.dev5081181816/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-25 14:31:27.000000 recon_lw-2.0.0.dev5081181816/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-25 14:31:54.000000 recon_lw-2.0.0.dev5081181816/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 14:32:20.000000 recon_lw-2.0.0.dev5081181816/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-25 14:31:27.000000 recon_lw-2.0.0.dev5081181816/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-25 14:31:27.000000 recon_lw-2.0.0.dev5081181816/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3717 2023-05-25 14:31:27.000000 recon_lw-2.0.0.dev5081181816/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-25 14:31:27.000000 recon_lw-2.0.0.dev5081181816/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-25 14:31:27.000000 recon_lw-2.0.0.dev5081181816/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28436 2023-05-25 14:31:27.000000 recon_lw-2.0.0.dev5081181816/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-25 14:31:27.000000 recon_lw-2.0.0.dev5081181816/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 14:32:20.000000 recon_lw-2.0.0.dev5081181816/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-25 14:32:20.000000 recon_lw-2.0.0.dev5081181816/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-25 14:32:20.000000 recon_lw-2.0.0.dev5081181816/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 14:32:20.000000 recon_lw-2.0.0.dev5081181816/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-25 14:32:20.000000 recon_lw-2.0.0.dev5081181816/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-25 14:32:20.000000 recon_lw-2.0.0.dev5081181816/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-25 14:31:27.000000 recon_lw-2.0.0.dev5081181816/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 14:32:20.000000 recon_lw-2.0.0.dev5081181816/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-25 14:31:27.000000 recon_lw-2.0.0.dev5081181816/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 14:32:20.000000 recon_lw-2.0.0.dev5081181816/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-25 14:31:27.000000 recon_lw-2.0.0.dev5081181816/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5080738022/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5081181816/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5080738022/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5081181816/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5080738022/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5081181816/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5080738022/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5081181816/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5080738022/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5081181816/recon_lw/recon_ob.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,14 +114,15 @@
                 log_book["sessionId"] = mess["sessionId"]
                 log_book["book_id"] = book_id
                 log_book["operation"] = operation.__name__
                 log_book["operation_params"] = initial_parameters
                 log_book["source_msg_id"] = mess["messageId"]
                 if log_books_filter is None or log_books_filter(log_book):
                     log_books_collection.append(log_book)
+                    obs.append(log_book)
                 #    log_event = recon_lw.create_event("OrderBook:" + mess["sessionId"],
                 #                                      "OrderBook",
                 #                                      event_sequence,
                 #                                      ok=True,
                 #                                      body=log_book,
                 #                                      parentId=parent_event["eventId"])
                 #    log_event["attachedMessageIds"] = [mess["messageId"]]
@@ -150,51 +151,25 @@
                                             "book_id": book_id},
                                       parentId=parent_event["eventId"])
     for tupl in operations_batch:
         dbg_event["attachedMessageIds"].append(tupl[2]["messageId"])
     events.append(dbg_event)
 
     if len(obs) > 1 and aggregate_batch_updates:
-        #same_side = all(
-        #    obs[i]["body"]["aggr_seq"]["affected_side"] == obs[0]["body"]["aggr_seq"]["affected_side"] for i in
-        #    range(1, len(obs)))
-        #same_level = all(
-        #    obs[i]["body"]["aggr_seq"]["affected_level"] == obs[0]["body"]["aggr_seq"]["affected_level"] for i in
-        #    range(1, len(obs)))
-        #l2 is not aggregated
-        #l1 is always aggregated regardless of side
-        same_level = False
-        same_side = True
-        if same_side and obs[0]["body"]["aggr_seq"]["affected_side"] != "na":
-            skip_top = 0
-            skip_aggr = 0
-            for i in range(len(obs) - 1):
-                if obs[i]["body"]["aggr_seq"]["top_delta"] == 1:
-                    skip_top += 1
-                obs[i]["body"]["aggr_seq"]["top_delta"] = 0
-                obs[i]["body"]["aggr_seq"]["top_v"] = -1
-                obs[i]["body"]["aggr_seq"]["top_v2"] = -1
-
-                if same_level and obs[0]["body"]["aggr_seq"]["affected_side"] != -1:
-                    if obs[i]["body"]["aggr_seq"]["limit_delta"] == 1:
-                        skip_aggr += 1
-                    obs[i]["body"]["aggr_seq"]["limit_delta"] = 0
-                    obs[i]["body"]["aggr_seq"]["limit_v"] = -1
-                    obs[i]["body"]["aggr_seq"]["limit_v2"] = -1
-
-            obs[-1]["body"]["aggr_seq"]["top_delta"] = 1
-            obs[-1]["body"]["aggr_seq"]["top_v"] -= skip_top
-            obs[-1]["body"]["aggr_seq"]["top_v2"] -= skip_top
-
-            if same_level and obs[0]["body"]["aggr_seq"]["affected_side"] != -1:
-                obs[-1]["body"]["aggr_seq"]["limit_delta"] = 1
-                obs[-1]["body"]["aggr_seq"]["limit_v"] -= skip_aggr
-                obs[-1]["body"]["aggr_seq"]["limit_v2"] -= skip_aggr
-
-    events.extend(obs)
+        skip_top = 0
+        for i in range(len(obs) - 1):
+            if obs[i]["body"]["aggr_seq"]["top_delta"] == 1:
+                skip_top += 1
+            obs[i]["body"]["aggr_seq"]["top_delta"] = 0
+            obs[i]["body"]["aggr_seq"]["top_v"] = -1
+            obs[i]["body"]["aggr_seq"]["top_v2"] = -1
+
+        obs[-1]["body"]["aggr_seq"]["top_delta"] = 1
+        obs[-1]["body"]["aggr_seq"]["top_v"] -= skip_top
+        obs[-1]["body"]["aggr_seq"]["top_v2"] -= skip_top
 
 
 def process_market_data_update(mess_batch, events,  books_cache, get_book_id_func ,update_book_rule,
                                check_book_rule, event_sequence, parent_event, initial_book_params, log_books_filter,
                                log_books_collection, aggregate_batch_updates):
     books_updates = {}
     for m in mess_batch:
```

### Comparing `recon_lw-2.0.0.dev5080738022/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5081181816/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5080738022/setup.py` & `recon_lw-2.0.0.dev5081181816/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5080738022/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5081181816/test/test_recon_ob.py`

 * *Files identical despite different names*

