# Comparing `tmp/dash-connectivity-viewer-2.0.8.tar.gz` & `tmp/dash-connectivity-viewer-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-connectivity-viewer-2.0.8.tar", last modified: Tue May 23 21:40:20 2023, max compression
+gzip compressed data, was "dash-connectivity-viewer-2.0.9.tar", last modified: Wed May 24 00:06:06 2023, max compression
```

## Comparing `dash-connectivity-viewer-2.0.8.tar` & `dash-connectivity-viewer-2.0.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-23 21:40:20.171553 dash-connectivity-viewer-2.0.8/
--rw-r--r--   0 caseysm    (501) staff       (20)     1842 2023-05-09 18:49:42.000000 dash-connectivity-viewer-2.0.8/LICENSE.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       71 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.8/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)      525 2023-05-23 21:40:20.171285 dash-connectivity-viewer-2.0.8/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      216 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.8/README.md
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-23 21:40:20.078952 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/
--rw-r--r--   0 caseysm    (501) staff       (20)       22 2023-05-23 21:40:05.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/__init__.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-23 21:40:20.105138 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/
--rw-r--r--   0 caseysm    (501) staff       (20)      568 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    24594 2023-05-13 00:17:14.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5453 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3461 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6156 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py
--rw-r--r--   0 caseysm    (501) staff       (20)       82 2023-03-18 18:57:32.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/external_stylesheets.py
--rw-r--r--   0 caseysm    (501) staff       (20)    20408 2023-05-14 19:13:50.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/layout.py
--rw-r--r--   0 caseysm    (501) staff       (20)     4439 2023-05-12 23:41:48.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-23 21:40:20.128114 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/
--rw-r--r--   0 caseysm    (501) staff       (20)      711 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    14472 2023-05-14 19:13:28.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1347 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)      210 2023-02-08 23:15:09.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/ct_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)    14841 2023-05-14 19:13:16.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/layout.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-23 21:40:20.153782 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/
--rw-r--r--   0 caseysm    (501) staff       (20)       17 2023-04-13 06:43:13.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5184 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     2914 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/dash_url_helper.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-23 21:40:20.155417 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/data/
--rw-r--r--   0 caseysm    (501) staff       (20)      144 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/data/height_bounds_v1.npy
--rw-r--r--   0 caseysm    (501) staff       (20)      168 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/data/layer_bounds_v1.npy
--rw-r--r--   0 caseysm    (501) staff       (20)    10170 2023-05-18 22:41:24.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/dataframe_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)      294 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/external_stylesheets.py
--rw-r--r--   0 caseysm    (501) staff       (20)    13477 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/link_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3942 2023-05-14 20:42:12.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/lookup_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)    11370 2023-05-12 23:38:23.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/neuron_data_base.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3825 2023-05-23 21:02:51.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/schema_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3950 2023-05-14 19:10:55.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/table_lookup.py
--rw-r--r--   0 caseysm    (501) staff       (20)      762 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/transform_utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-23 21:40:20.169647 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/connectivity_table/
--rw-r--r--   0 caseysm    (501) staff       (20)      591 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/connectivity_table/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    13817 2023-05-14 19:07:55.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/connectivity_table/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)      523 2023-02-08 23:15:09.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/connectivity_table/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     9093 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/connectivity_table/layout.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-23 21:40:20.080234 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)      525 2023-05-23 21:40:20.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)     1990 2023-05-23 21:40:20.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-05-23 21:40:20.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      180 2023-05-23 21:40:20.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       25 2023-05-23 21:40:20.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer.egg-info/top_level.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      179 2023-05-18 22:42:04.000000 dash-connectivity-viewer-2.0.8/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-05-23 21:40:20.171610 dash-connectivity-viewer-2.0.8/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1153 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.8/setup.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-24 00:06:06.334181 dash-connectivity-viewer-2.0.9/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1842 2023-05-09 18:49:42.000000 dash-connectivity-viewer-2.0.9/LICENSE.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       71 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.9/MANIFEST.in
+-rw-r--r--   0 caseysm    (501) staff       (20)      525 2023-05-24 00:06:06.333987 dash-connectivity-viewer-2.0.9/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)      216 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.9/README.md
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-24 00:06:06.302705 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/
+-rw-r--r--   0 caseysm    (501) staff       (20)       22 2023-05-24 00:05:12.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/__init__.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-24 00:06:06.314741 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_connectivity/
+-rw-r--r--   0 caseysm    (501) staff       (20)      568 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_connectivity/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    24643 2023-05-24 00:03:45.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_connectivity/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     5453 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_connectivity/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3461 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     6156 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py
+-rw-r--r--   0 caseysm    (501) staff       (20)       82 2023-03-18 18:57:32.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_connectivity/external_stylesheets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    20408 2023-05-14 19:13:50.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_connectivity/layout.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     4439 2023-05-12 23:41:48.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-24 00:06:06.320667 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_table/
+-rw-r--r--   0 caseysm    (501) staff       (20)      711 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_table/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    14472 2023-05-14 19:13:28.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_table/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     1347 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_table/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      210 2023-02-08 23:15:09.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_table/ct_utils.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    14841 2023-05-14 19:13:16.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_table/layout.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-24 00:06:06.328259 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/
+-rw-r--r--   0 caseysm    (501) staff       (20)       17 2023-04-13 06:43:13.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     5233 2023-05-23 23:46:19.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     2914 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/dash_url_helper.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-24 00:06:06.330619 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/data/
+-rw-r--r--   0 caseysm    (501) staff       (20)      144 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/data/height_bounds_v1.npy
+-rw-r--r--   0 caseysm    (501) staff       (20)      168 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/data/layer_bounds_v1.npy
+-rw-r--r--   0 caseysm    (501) staff       (20)    10170 2023-05-18 22:41:24.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/dataframe_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      294 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/external_stylesheets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    13477 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/link_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3942 2023-05-14 20:42:12.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/lookup_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    11370 2023-05-12 23:38:23.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/neuron_data_base.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3825 2023-05-23 21:02:51.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/schema_utils.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3950 2023-05-14 19:10:55.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/table_lookup.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      762 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/transform_utils.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-24 00:06:06.333666 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/connectivity_table/
+-rw-r--r--   0 caseysm    (501) staff       (20)      591 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/connectivity_table/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    13817 2023-05-14 19:07:55.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/connectivity_table/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      523 2023-02-08 23:15:09.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/connectivity_table/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     9093 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/connectivity_table/layout.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-24 00:06:06.303488 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer.egg-info/
+-rw-r--r--   0 caseysm    (501) staff       (20)      525 2023-05-24 00:06:06.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)     1990 2023-05-24 00:06:06.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-05-24 00:06:06.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      180 2023-05-24 00:06:06.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer.egg-info/requires.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       25 2023-05-24 00:06:06.000000 dash-connectivity-viewer-2.0.9/dash_connectivity_viewer.egg-info/top_level.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      179 2023-05-18 22:42:04.000000 dash-connectivity-viewer-2.0.9/requirements.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-05-24 00:06:06.334251 dash-connectivity-viewer-2.0.9/setup.cfg
+-rw-r--r--   0 caseysm    (501) staff       (20)     1153 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.9/setup.py
```

### Comparing `dash-connectivity-viewer-2.0.8/LICENSE.txt` & `dash-connectivity-viewer-2.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/PKG-INFO` & `dash-connectivity-viewer-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-connectivity-viewer
-Version: 2.0.8
+Version: 2.0.9
 Summary: Dash connectivity viewer for CAVE data
 Home-page: https://github.com/ceesem/dash-connectivity-viewer
 Author: Casey Schneider-Mizell
 Author-email: caseysm@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/__init__.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_connectivity/__init__.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/callbacks.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_connectivity/callbacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,14 +209,15 @@
     )
     def define_table_columns(_, datastack, cell_type_table):
         client = make_client(datastack, c.server_address)
         if cell_type_table == "" or cell_type_table is None:
             return [{"name": i, "id": i} for i in c.table_columns], []
 
         _, val_cols = get_table_info(cell_type_table, client, allow_types=ALLOW_COLUMN_TYPES_DISCRETE)
+
         table_cons = c.table_columns + val_cols
         return (
             [{"name": i, "id": i} for i in table_cons],
             [{"label": k, "value": k} for k in val_cols],
         )
 
     @app.callback(
@@ -437,14 +438,16 @@
                 f"Input (n = {n_syn_post})",
                 1,
                 info_cache,
                 vplot,
                 syn_res,
             )
         except Exception as e:
+            if c.debug:
+                raise e
             return (
                 html.Div(str(e)),
                 "danger",
                 "",
                 [],
                 [],
                 "Output",
```

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/config.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_connectivity/config.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/layout.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_connectivity/layout.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/__init__.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_table/__init__.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/callbacks.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_table/callbacks.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/config.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_table/config.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/layout.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/cell_type_table/layout.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/config.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
         )
 
         # If None, the info service is used
         self.nucleus_table = config.get("nucleus_table", None)
         self.nucleus_id_column = config.get("nucleus_id_column", "id")
         self.nucleus_filter = config.get('nucleus_filter', {})
 
+        self.debug = config.get("debug", False)
+
         # Used to look up number of neurons per root id
         self.soma_table = self.nucleus_table
         self.soma_id_column = self.nucleus_id_column
 
         # Used to look up connectivity
         # If None, the info service is used
         self.synapse_table = config.get("synapse_table", None)
```

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/dash_url_helper.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/dash_url_helper.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/dataframe_utilities.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/dataframe_utilities.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/link_utilities.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/link_utilities.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/lookup_utilities.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/lookup_utilities.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/neuron_data_base.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/neuron_data_base.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/schema_utils.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/table_lookup.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/table_lookup.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/transform_utils.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/common/transform_utils.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/connectivity_table/__init__.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/connectivity_table/__init__.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/connectivity_table/callbacks.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/connectivity_table/callbacks.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/connectivity_table/config.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/connectivity_table/config.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/connectivity_table/layout.py` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer/connectivity_table/layout.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer.egg-info/PKG-INFO` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-connectivity-viewer
-Version: 2.0.8
+Version: 2.0.9
 Summary: Dash connectivity viewer for CAVE data
 Home-page: https://github.com/ceesem/dash-connectivity-viewer
 Author: Casey Schneider-Mizell
 Author-email: caseysm@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer.egg-info/SOURCES.txt` & `dash-connectivity-viewer-2.0.9/dash_connectivity_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.8/setup.py` & `dash-connectivity-viewer-2.0.9/setup.py`

 * *Files identical despite different names*

