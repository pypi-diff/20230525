# Comparing `tmp/recon_lw-2.0.0.dev5081361559.tar.gz` & `tmp/recon_lw-2.0.0.dev5081971643.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5081361559.tar", last modified: Thu May 25 14:50:11 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5081971643.tar", last modified: Thu May 25 15:50:48 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5081361559.tar` & `recon_lw-2.0.0.dev5081971643.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 14:50:11.000000 recon_lw-2.0.0.dev5081361559/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-25 14:49:24.000000 recon_lw-2.0.0.dev5081361559/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-25 14:50:11.000000 recon_lw-2.0.0.dev5081361559/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-25 14:49:24.000000 recon_lw-2.0.0.dev5081361559/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-25 14:49:46.000000 recon_lw-2.0.0.dev5081361559/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 14:50:11.000000 recon_lw-2.0.0.dev5081361559/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-25 14:49:24.000000 recon_lw-2.0.0.dev5081361559/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-25 14:49:24.000000 recon_lw-2.0.0.dev5081361559/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3717 2023-05-25 14:49:24.000000 recon_lw-2.0.0.dev5081361559/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-25 14:49:24.000000 recon_lw-2.0.0.dev5081361559/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-25 14:49:24.000000 recon_lw-2.0.0.dev5081361559/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    28380 2023-05-25 14:49:24.000000 recon_lw-2.0.0.dev5081361559/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-25 14:49:24.000000 recon_lw-2.0.0.dev5081361559/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 14:50:11.000000 recon_lw-2.0.0.dev5081361559/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-25 14:50:11.000000 recon_lw-2.0.0.dev5081361559/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-25 14:50:11.000000 recon_lw-2.0.0.dev5081361559/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 14:50:11.000000 recon_lw-2.0.0.dev5081361559/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-25 14:50:11.000000 recon_lw-2.0.0.dev5081361559/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-25 14:50:11.000000 recon_lw-2.0.0.dev5081361559/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-25 14:49:24.000000 recon_lw-2.0.0.dev5081361559/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 14:50:11.000000 recon_lw-2.0.0.dev5081361559/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-25 14:49:24.000000 recon_lw-2.0.0.dev5081361559/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 14:50:11.000000 recon_lw-2.0.0.dev5081361559/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-25 14:49:24.000000 recon_lw-2.0.0.dev5081361559/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 15:50:48.000000 recon_lw-2.0.0.dev5081971643/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-25 15:49:59.000000 recon_lw-2.0.0.dev5081971643/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-25 15:50:48.000000 recon_lw-2.0.0.dev5081971643/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-25 15:49:59.000000 recon_lw-2.0.0.dev5081971643/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-25 15:50:29.000000 recon_lw-2.0.0.dev5081971643/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 15:50:48.000000 recon_lw-2.0.0.dev5081971643/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-25 15:49:59.000000 recon_lw-2.0.0.dev5081971643/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-25 15:49:59.000000 recon_lw-2.0.0.dev5081971643/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3717 2023-05-25 15:49:59.000000 recon_lw-2.0.0.dev5081971643/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-25 15:49:59.000000 recon_lw-2.0.0.dev5081971643/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-25 15:49:59.000000 recon_lw-2.0.0.dev5081971643/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28525 2023-05-25 15:49:59.000000 recon_lw-2.0.0.dev5081971643/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-25 15:49:59.000000 recon_lw-2.0.0.dev5081971643/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 15:50:48.000000 recon_lw-2.0.0.dev5081971643/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-25 15:50:48.000000 recon_lw-2.0.0.dev5081971643/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-25 15:50:48.000000 recon_lw-2.0.0.dev5081971643/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 15:50:48.000000 recon_lw-2.0.0.dev5081971643/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-25 15:50:48.000000 recon_lw-2.0.0.dev5081971643/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-25 15:50:48.000000 recon_lw-2.0.0.dev5081971643/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-25 15:49:59.000000 recon_lw-2.0.0.dev5081971643/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 15:50:48.000000 recon_lw-2.0.0.dev5081971643/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-25 15:49:59.000000 recon_lw-2.0.0.dev5081971643/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 15:50:48.000000 recon_lw-2.0.0.dev5081971643/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-25 15:49:59.000000 recon_lw-2.0.0.dev5081971643/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5081361559/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5081971643/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5081361559/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5081971643/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5081361559/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5081971643/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5081361559/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5081971643/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5081361559/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5081971643/recon_lw/recon_ob.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,16 @@
     for tupl in operations_batch:
         dbg_event["attachedMessageIds"].append(tupl[2]["messageId"])
     events.append(dbg_event)
 
     if len(obs) > 1 and aggregate_batch_updates:
         skip_top = 0
         for i in range(len(obs) - 1):
+            if obs[i]["operation"] in ["ob_change_status", "ob_clean_book", "ob_aggr_clean_book", "ob_top_clean_book"]:
+                continue
             if obs[i]["aggr_seq"]["top_delta"] == 1:
                 skip_top += 1
             obs[i]["aggr_seq"]["top_delta"] = 0
             obs[i]["aggr_seq"]["top_v"] = -1
             obs[i]["aggr_seq"]["top_v2"] = -1
 
         obs[-1]["aggr_seq"]["top_delta"] = 1
```

### Comparing `recon_lw-2.0.0.dev5081361559/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5081971643/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5081361559/setup.py` & `recon_lw-2.0.0.dev5081971643/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5081361559/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5081971643/test/test_recon_ob.py`

 * *Files identical despite different names*

