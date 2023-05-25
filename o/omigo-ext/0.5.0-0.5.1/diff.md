# Comparing `tmp/omigo_ext-0.5.0.tar.gz` & `tmp/omigo_ext-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omigo_ext-0.5.0.tar", last modified: Sat Mar 25 01:56:51 2023, max compression
+gzip compressed data, was "omigo_ext-0.5.1.tar", last modified: Thu May 25 19:10:22 2023, max compression
```

## Comparing `omigo_ext-0.5.0.tar` & `omigo_ext-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:56:51.114439 omigo_ext-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-25 01:56:51.114439 omigo_ext-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 01:56:18.000000 omigo_ext-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-25 01:56:18.000000 omigo_ext-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-03-25 01:56:51.114439 omigo_ext-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:56:51.110439 omigo_ext-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:56:51.114439 omigo_ext-0.5.0/src/omigo_ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 01:56:18.000000 omigo_ext-0.5.0/src/omigo_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-25 01:56:18.000000 omigo_ext-0.5.0/src/omigo_ext/etl_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-03-25 01:56:18.000000 omigo_ext-0.5.0/src/omigo_ext/graph_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-03-25 01:56:18.000000 omigo_ext-0.5.0/src/omigo_ext/graphviz_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-03-25 01:56:18.000000 omigo_ext-0.5.0/src/omigo_ext/kafka_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-03-25 01:56:18.000000 omigo_ext-0.5.0/src/omigo_ext/multithread_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-03-25 01:56:18.000000 omigo_ext-0.5.0/src/omigo_ext/ws_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:56:51.114439 omigo_ext-0.5.0/src/omigo_ext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-25 01:56:51.000000 omigo_ext-0.5.0/src/omigo_ext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-25 01:56:51.000000 omigo_ext-0.5.0/src/omigo_ext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:56:51.000000 omigo_ext-0.5.0/src/omigo_ext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-25 01:56:51.000000 omigo_ext-0.5.0/src/omigo_ext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-25 01:56:51.000000 omigo_ext-0.5.0/src/omigo_ext.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:10:22.486436 omigo_ext-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-25 19:10:22.486436 omigo_ext-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:39.000000 omigo_ext-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 19:09:39.000000 omigo_ext-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-25 19:10:22.486436 omigo_ext-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:10:22.482436 omigo_ext-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:10:22.486436 omigo_ext-0.5.1/src/omigo_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:39.000000 omigo_ext-0.5.1/src/omigo_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-25 19:09:39.000000 omigo_ext-0.5.1/src/omigo_ext/etl_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-05-25 19:09:39.000000 omigo_ext-0.5.1/src/omigo_ext/graph_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-25 19:09:39.000000 omigo_ext-0.5.1/src/omigo_ext/graphviz_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-25 19:09:39.000000 omigo_ext-0.5.1/src/omigo_ext/kafka_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-25 19:09:39.000000 omigo_ext-0.5.1/src/omigo_ext/multithread_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-05-25 19:09:39.000000 omigo_ext-0.5.1/src/omigo_ext/ws_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:10:22.486436 omigo_ext-0.5.1/src/omigo_ext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-25 19:10:22.000000 omigo_ext-0.5.1/src/omigo_ext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-25 19:10:22.000000 omigo_ext-0.5.1/src/omigo_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:10:22.000000 omigo_ext-0.5.1/src/omigo_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-25 19:10:22.000000 omigo_ext-0.5.1/src/omigo_ext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 19:10:22.000000 omigo_ext-0.5.1/src/omigo_ext.egg-info/top_level.txt
```

### Comparing `omigo_ext-0.5.0/setup.cfg` & `omigo_ext-0.5.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = omigo_ext
-version = 0.5.0
+version = 0.5.1
 author = amit jaiswal
 author_email = amit.jaiswal@gmail.com
 description = Extensions for omigo_core package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CrowdStrike/omigo-data-analytics
 project_urls =
```

### Comparing `omigo_ext-0.5.0/src/omigo_ext/etl_ext.py` & `omigo_ext-0.5.1/src/omigo_ext/etl_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.0/src/omigo_ext/graph_ext.py` & `omigo_ext-0.5.1/src/omigo_ext/graph_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.0/src/omigo_ext/graphviz_ext.py` & `omigo_ext-0.5.1/src/omigo_ext/graphviz_ext.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,17 @@
     props["style"] = "filled"
     props["shape"] = "rectangle"
 
     # return
     return props
 
 # TODO: Use graphviz apis instead of constructing strings
-def __get_graphviz_data__(vertex_map, edges_maps, node_props, edge_props, vertex_id_col, edge_src_col, edge_dest_col, vertex_display_id_col, style_func, max_len):
+def __get_graphviz_data__(vertex_map, edges_maps, node_props, edge_props, vertex_id_col, edge_src_col, edge_dest_col, vertex_display_id_col, style_func, max_len,
+    display_vertex_keys, display_edge_keys):
+
     # check for custom display
     if (style_func is None):
         style_func = __default_dot_style_func__
 
     # initialize the digraph structure
     digraph_arr = []
     digraph_arr.append("digraph G {")
@@ -50,15 +52,21 @@
         mp_props.append("{}".format(vertex_display_id_val))
 
         # iterate over all properties of the vertex
         if (node_props is not None and len(node_props) > 0):
             for k1 in node_props:
                 # get the value and generate key-value string
                 v1 = str(mp[k1]) if (k1 in mp.keys()) else ""
-                kv_str = "[{} = {}]".format(k1, v1)
+
+                # decide whether to display keys
+                kv_str = None
+                if (display_vertex_keys is None or k1 in display_vertex_keys):
+                    kv_str = "[{} = {}]".format(k1, v1)
+                else:
+                    kv_str = "[{}]".format(v1)
 
                 # truncate the value if it exceeds a specific threshold
                 if (max_len is not None and len(kv_str) > max_len):
                     if (max_len > 3):
                         kv_str = kv_str[0:(max_len - 3)] + "..."
                     else:
                         kv_str = kv_str[0:max_len]
@@ -93,16 +101,22 @@
         if (edge_props is not None and len(edge_props) > 0):
             ed_props = []
 
             # iterate over all edge properties
             for k1 in edge_props:
                 # get the value and generate key-value string
                 v1 = str(mp[k1]) if (k1 in mp.keys()) else ""
+
                 if (v1 != ""):
-                    kv_str = "[{}]".format(v1)
+                    # decide whether to display keys
+                    kv_str = None
+                    if (display_edge_keys is None or k1 in display_edge_keys):
+                        kv_str = "[{} = {}]".format(k1, v1)
+                    else:
+                        kv_str = "[{}]".format(v1)
 
                     # truncate the value if it exceeds a specific threshold
                     if (max_len is not None and len(kv_str) > max_len):
                         if (max_len > 3):
                             kv_str = kv_str[0:(max_len - 3)] + "..."
                         else:
                             kv_str = kv_str[0:max_len]
@@ -124,15 +138,15 @@
     # debug
     utils.debug(digraph_str)
 
     # return
     return digraph_str
 
 def get_graphviz_data(vtsv, etsv, vertex_id_col, src_edge_col, dest_edge_col, vertex_display_id_col = None, node_props = None, edge_props = None, style_func = None,
-    max_len = None, create_missing_vertices = False):
+    max_len = None, create_missing_vertices = False, display_vertex_keys = None, display_edge_keys = None):
 
     # default for vertex display
     if (vertex_display_id_col is None):
         vertex_display_id_col = vertex_id_col
 
     # do some validation on vertices and edges
     vertex_ids = set(vtsv.col_as_array_uniq(vertex_id_col))
@@ -179,18 +193,20 @@
 
     # create edges map
     edges_maps = {}
     for mp in etsv.to_maps():
         edges_maps[(mp[src_edge_col], mp[dest_edge_col])] = mp
 
     # get the graphviz output
-    return __get_graphviz_data__(vertex_map, edges_maps, node_props, edge_props, vertex_id_col, src_edge_col, dest_edge_col, vertex_display_id_col, style_func, max_len)
+    return __get_graphviz_data__(vertex_map, edges_maps, node_props, edge_props, vertex_id_col, src_edge_col, dest_edge_col, vertex_display_id_col, style_func, max_len,
+        display_vertex_keys, display_edge_keys)
 
 def plot_graph(vtsv, etsv, vertex_id_col, src_edge_col, dest_edge_col, vertex_display_id_col = None, node_props = None, edge_props = None, style_func = None,
-    max_len = None, create_missing_vertices = False):
+    max_len = None, create_missing_vertices = False, display_vertex_keys = None, display_edge_keys = None):
 
     digraph_str = get_graphviz_data(vtsv, etsv, vertex_id_col, src_edge_col, dest_edge_col, vertex_display_id_col = vertex_display_id_col, node_props = node_props,
-        edge_props = edge_props, style_func = style_func, max_len = max_len, create_missing_vertices = create_missing_vertices)
+        edge_props = edge_props, style_func = style_func, max_len = max_len, create_missing_vertices = create_missing_vertices, display_vertex_keys = display_vertex_keys,
+        display_edge_keys = display_edge_keys)
 
     # return
     return graphviz.Source(digraph_str)
```

### Comparing `omigo_ext-0.5.0/src/omigo_ext/kafka_ext.py` & `omigo_ext-0.5.1/src/omigo_ext/kafka_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.0/src/omigo_ext/multithread_ext.py` & `omigo_ext-0.5.1/src/omigo_ext/multithread_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.0/src/omigo_ext/ws_ext.py` & `omigo_ext-0.5.1/src/omigo_ext/ws_ext.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
             result_mp["response:selective_execution"] = "1"
 
             # some debugging
             if (str(resp_status_code).startswith("5")):
                 utils.error("__call_web_service_exp_func_inner__: Got status code: {}: mp: {}".format(resp_status_code, mp))
         else:
             # for some reason, this row is not meant to be executed. Ignore.
-            resp_str, resp_status_code, resp_err = "", 0, ""
+            resp_str, resp_status_code, resp_err = "", 200, ""
             result_mp["response:success"] = "0"
             result_mp["response:selective_execution"] = "0"
 
         # fill rest of the result map.
         result_mp["response:url_encoded"] = str(utils.url_encode(resp_str))
         result_mp["response:status_code"] = str(resp_status_code)
         result_mp["response:error"] = str(resp_err)
```

