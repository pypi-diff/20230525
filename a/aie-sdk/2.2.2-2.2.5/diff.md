# Comparing `tmp/aie-sdk-2.2.2.tar.gz` & `tmp/aie-sdk-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aie-sdk-2.2.2.tar", last modified: Wed May 10 08:11:13 2023, max compression
+gzip compressed data, was "aie-sdk-2.2.5.tar", last modified: Thu May 25 12:36:32 2023, max compression
```

## Comparing `aie-sdk-2.2.2.tar` & `aie-sdk-2.2.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-10 08:11:13.761615 aie-sdk-2.2.2/
--rw-r--r--   0 songci     (502) staff       (20)     1068 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/LICENSE
--rw-r--r--   0 songci     (502) staff       (20)       21 2023-04-13 02:48:48.000000 aie-sdk-2.2.2/MANIFEST.in
--rw-r--r--   0 songci     (502) staff       (20)      429 2023-05-10 08:11:13.761139 aie-sdk-2.2.2/PKG-INFO
--rw-r--r--   0 songci     (502) staff       (20)      209 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/README.md
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-10 08:11:13.730507 aie-sdk-2.2.2/aie/
--rw-r--r--   0 songci     (502) staff       (20)     1128 2023-05-10 08:11:12.000000 aie-sdk-2.2.2/aie/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)     2302 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/aie_env.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-10 08:11:13.739431 aie-sdk-2.2.2/aie/aie_object/
--rw-r--r--   0 songci     (502) staff       (20)       46 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/aie_object/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)    16729 2023-05-10 08:11:11.000000 aie-sdk-2.2.2/aie/aie_object/classifier.py
--rw-r--r--   0 songci     (502) staff       (20)     5225 2023-05-10 08:11:04.000000 aie-sdk-2.2.2/aie/aie_object/collection.py
--rw-r--r--   0 songci     (502) staff       (20)     2996 2023-05-10 08:11:11.000000 aie-sdk-2.2.2/aie/aie_object/confusion_matrix.py
--rw-r--r--   0 songci     (502) staff       (20)    25064 2023-05-10 08:11:06.000000 aie-sdk-2.2.2/aie/aie_object/feature.py
--rw-r--r--   0 songci     (502) staff       (20)    27878 2023-05-10 08:11:07.000000 aie-sdk-2.2.2/aie/aie_object/feature_collection.py
--rw-r--r--   0 songci     (502) staff       (20)    22797 2023-05-10 08:11:08.000000 aie-sdk-2.2.2/aie/aie_object/filter.py
--rw-r--r--   0 songci     (502) staff       (20)    24135 2023-05-10 08:11:05.000000 aie-sdk-2.2.2/aie/aie_object/geometry.py
--rw-r--r--   0 songci     (502) staff       (20)    81753 2023-05-10 08:11:03.000000 aie-sdk-2.2.2/aie/aie_object/image.py
--rw-r--r--   0 songci     (502) staff       (20)    23330 2023-05-10 08:11:05.000000 aie-sdk-2.2.2/aie/aie_object/image_collection.py
--rw-r--r--   0 songci     (502) staff       (20)    29114 2023-05-10 08:11:10.000000 aie-sdk-2.2.2/aie/aie_object/kernel.py
--rw-r--r--   0 songci     (502) staff       (20)     1463 2023-05-10 08:11:12.000000 aie-sdk-2.2.2/aie/aie_object/model.py
--rw-r--r--   0 songci     (502) staff       (20)    13998 2023-05-10 08:11:09.000000 aie-sdk-2.2.2/aie/aie_object/reducer.py
--rw-r--r--   0 songci     (502) staff       (20)     2961 2023-05-10 08:11:09.000000 aie-sdk-2.2.2/aie/aie_object/terrain.py
--rw-r--r--   0 songci     (502) staff       (20)     2570 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/auth.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-10 08:11:13.747304 aie-sdk-2.2.2/aie/client/
--rw-r--r--   0 songci     (502) staff       (20)      275 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/client/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)     6490 2023-05-10 08:10:26.000000 aie-sdk-2.2.2/aie/client/client.py
--rw-r--r--   0 songci     (502) staff       (20)      775 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/client/constants.py
--rw-r--r--   0 songci     (502) staff       (20)     3278 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/client/dataset.py
--rw-r--r--   0 songci     (502) staff       (20)     1370 2022-11-21 11:41:47.000000 aie-sdk-2.2.2/aie/client/endpoints.py
--rw-r--r--   0 songci     (502) staff       (20)     7371 2023-05-10 08:10:26.000000 aie-sdk-2.2.2/aie/client/interactive_session.py
--rw-r--r--   0 songci     (502) staff       (20)     1647 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/client/maps.py
--rw-r--r--   0 songci     (502) staff       (20)    15854 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/client/mlproxy.py
--rw-r--r--   0 songci     (502) staff       (20)    18381 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/client/mlproxy_back.py
--rw-r--r--   0 songci     (502) staff       (20)     2543 2023-05-08 04:13:45.000000 aie-sdk-2.2.2/aie/client/task.py
--rw-r--r--   0 songci     (502) staff       (20)      232 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/customfunction_node.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-10 08:11:13.748984 aie-sdk-2.2.2/aie/error/
--rw-r--r--   0 songci     (502) staff       (20)      115 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/error/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)      849 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/error/aie_error.py
--rw-r--r--   0 songci     (502) staff       (20)     4264 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/export.py
--rw-r--r--   0 songci     (502) staff       (20)     1706 2023-04-10 02:23:35.000000 aie-sdk-2.2.2/aie/function_helper.py
--rw-r--r--   0 songci     (502) staff       (20)      500 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/function_node.py
--rw-r--r--   0 songci     (502) staff       (20)      907 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/g_var.py
--rw-r--r--   0 songci     (502) staff       (20)    11531 2022-12-09 06:48:05.000000 aie-sdk-2.2.2/aie/gen_python_functions.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-10 08:11:13.753688 aie-sdk-2.2.2/aie/map/
--rw-r--r--   0 songci     (502) staff       (20)       46 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/map/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)     2544 2022-12-01 11:50:21.000000 aie-sdk-2.2.2/aie/map/aie_color.py
--rw-r--r--   0 songci     (502) staff       (20)     8578 2022-12-01 11:50:21.000000 aie-sdk-2.2.2/aie/map/aie_layer.py
--rw-r--r--   0 songci     (502) staff       (20)     4947 2022-12-01 11:50:21.000000 aie-sdk-2.2.2/aie/map/aie_map.py
--rw-r--r--   0 songci     (502) staff       (20)     5860 2022-12-01 11:50:21.000000 aie-sdk-2.2.2/aie/map/color.csv
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-10 08:11:13.757385 aie-sdk-2.2.2/aie/serialize/
--rw-r--r--   0 songci     (502) staff       (20)      113 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/serialize/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)     4678 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/serialize/gen_visitor.py
--rw-r--r--   0 songci     (502) staff       (20)     3380 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/serialize/optimizer.py
--rw-r--r--   0 songci     (502) staff       (20)      724 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/serialize/serializer_impl.py
--rw-r--r--   0 songci     (502) staff       (20)      269 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/variable_node.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-10 08:11:13.760466 aie-sdk-2.2.2/aie_sdk.egg-info/
--rw-r--r--   0 songci     (502) staff       (20)      429 2023-05-10 08:11:13.000000 aie-sdk-2.2.2/aie_sdk.egg-info/PKG-INFO
--rw-r--r--   0 songci     (502) staff       (20)     1271 2023-05-10 08:11:13.000000 aie-sdk-2.2.2/aie_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 songci     (502) staff       (20)        1 2023-05-10 08:11:13.000000 aie-sdk-2.2.2/aie_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 songci     (502) staff       (20)       79 2023-05-10 08:11:13.000000 aie-sdk-2.2.2/aie_sdk.egg-info/requires.txt
--rw-r--r--   0 songci     (502) staff       (20)        4 2023-05-10 08:11:13.000000 aie-sdk-2.2.2/aie_sdk.egg-info/top_level.txt
--rw-r--r--   0 songci     (502) staff       (20)       38 2023-05-10 08:11:13.761754 aie-sdk-2.2.2/setup.cfg
--rw-r--r--   0 songci     (502) staff       (20)      891 2023-04-13 02:48:49.000000 aie-sdk-2.2.2/setup.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-25 12:36:32.959792 aie-sdk-2.2.5/
+-rw-r--r--   0 songci     (502) staff       (20)     1068 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/LICENSE
+-rw-r--r--   0 songci     (502) staff       (20)       21 2023-04-13 02:48:48.000000 aie-sdk-2.2.5/MANIFEST.in
+-rw-r--r--   0 songci     (502) staff       (20)      429 2023-05-25 12:36:32.959282 aie-sdk-2.2.5/PKG-INFO
+-rw-r--r--   0 songci     (502) staff       (20)      209 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/README.md
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-25 12:36:32.926748 aie-sdk-2.2.5/aie/
+-rw-r--r--   0 songci     (502) staff       (20)     1128 2023-05-25 12:36:32.000000 aie-sdk-2.2.5/aie/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)     2302 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/aie_env.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-25 12:36:32.936093 aie-sdk-2.2.5/aie/aie_object/
+-rw-r--r--   0 songci     (502) staff       (20)       46 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/aie_object/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)    16718 2023-05-25 12:36:30.000000 aie-sdk-2.2.5/aie/aie_object/classifier.py
+-rw-r--r--   0 songci     (502) staff       (20)     5220 2023-05-25 12:36:23.000000 aie-sdk-2.2.5/aie/aie_object/collection.py
+-rw-r--r--   0 songci     (502) staff       (20)     2989 2023-05-25 12:36:31.000000 aie-sdk-2.2.5/aie/aie_object/confusion_matrix.py
+-rw-r--r--   0 songci     (502) staff       (20)    25029 2023-05-25 12:36:26.000000 aie-sdk-2.2.5/aie/aie_object/feature.py
+-rw-r--r--   0 songci     (502) staff       (20)    27844 2023-05-25 12:36:27.000000 aie-sdk-2.2.5/aie/aie_object/feature_collection.py
+-rw-r--r--   0 songci     (502) staff       (20)    22776 2023-05-25 12:36:28.000000 aie-sdk-2.2.5/aie/aie_object/filter.py
+-rw-r--r--   0 songci     (502) staff       (20)    24100 2023-05-25 12:36:25.000000 aie-sdk-2.2.5/aie/aie_object/geometry.py
+-rw-r--r--   0 songci     (502) staff       (20)    81635 2023-05-25 12:36:23.000000 aie-sdk-2.2.5/aie/aie_object/image.py
+-rw-r--r--   0 songci     (502) staff       (20)    24036 2023-05-25 12:36:24.000000 aie-sdk-2.2.5/aie/aie_object/image_collection.py
+-rw-r--r--   0 songci     (502) staff       (20)    29090 2023-05-25 12:36:30.000000 aie-sdk-2.2.5/aie/aie_object/kernel.py
+-rw-r--r--   0 songci     (502) staff       (20)     1462 2023-05-25 12:36:31.000000 aie-sdk-2.2.5/aie/aie_object/model.py
+-rw-r--r--   0 songci     (502) staff       (20)    13971 2023-05-25 12:36:28.000000 aie-sdk-2.2.5/aie/aie_object/reducer.py
+-rw-r--r--   0 songci     (502) staff       (20)     2958 2023-05-25 12:36:29.000000 aie-sdk-2.2.5/aie/aie_object/terrain.py
+-rw-r--r--   0 songci     (502) staff       (20)     2570 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/auth.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-25 12:36:32.945643 aie-sdk-2.2.5/aie/client/
+-rw-r--r--   0 songci     (502) staff       (20)      275 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/client/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)     6639 2023-05-15 03:43:12.000000 aie-sdk-2.2.5/aie/client/client.py
+-rw-r--r--   0 songci     (502) staff       (20)      775 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/client/constants.py
+-rw-r--r--   0 songci     (502) staff       (20)     3278 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/client/dataset.py
+-rw-r--r--   0 songci     (502) staff       (20)     1370 2022-11-21 11:41:47.000000 aie-sdk-2.2.5/aie/client/endpoints.py
+-rw-r--r--   0 songci     (502) staff       (20)     8211 2023-05-15 03:43:12.000000 aie-sdk-2.2.5/aie/client/interactive_session.py
+-rw-r--r--   0 songci     (502) staff       (20)     1647 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/client/maps.py
+-rw-r--r--   0 songci     (502) staff       (20)    15854 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/client/mlproxy.py
+-rw-r--r--   0 songci     (502) staff       (20)    18381 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/client/mlproxy_back.py
+-rw-r--r--   0 songci     (502) staff       (20)     2543 2023-05-08 04:13:45.000000 aie-sdk-2.2.5/aie/client/task.py
+-rw-r--r--   0 songci     (502) staff       (20)      232 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/customfunction_node.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-25 12:36:32.947429 aie-sdk-2.2.5/aie/error/
+-rw-r--r--   0 songci     (502) staff       (20)      115 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/error/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)      849 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/error/aie_error.py
+-rw-r--r--   0 songci     (502) staff       (20)     4264 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/export.py
+-rw-r--r--   0 songci     (502) staff       (20)     1706 2023-04-10 02:23:35.000000 aie-sdk-2.2.5/aie/function_helper.py
+-rw-r--r--   0 songci     (502) staff       (20)      500 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/function_node.py
+-rw-r--r--   0 songci     (502) staff       (20)      907 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/g_var.py
+-rw-r--r--   0 songci     (502) staff       (20)    11531 2022-12-09 06:48:05.000000 aie-sdk-2.2.5/aie/gen_python_functions.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-25 12:36:32.951750 aie-sdk-2.2.5/aie/map/
+-rw-r--r--   0 songci     (502) staff       (20)       46 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/map/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)     2544 2022-12-01 11:50:21.000000 aie-sdk-2.2.5/aie/map/aie_color.py
+-rw-r--r--   0 songci     (502) staff       (20)     8578 2022-12-01 11:50:21.000000 aie-sdk-2.2.5/aie/map/aie_layer.py
+-rw-r--r--   0 songci     (502) staff       (20)     4947 2022-12-01 11:50:21.000000 aie-sdk-2.2.5/aie/map/aie_map.py
+-rw-r--r--   0 songci     (502) staff       (20)     5860 2022-12-01 11:50:21.000000 aie-sdk-2.2.5/aie/map/color.csv
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-25 12:36:32.955480 aie-sdk-2.2.5/aie/serialize/
+-rw-r--r--   0 songci     (502) staff       (20)      113 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/serialize/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)     4678 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/serialize/gen_visitor.py
+-rw-r--r--   0 songci     (502) staff       (20)     3380 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/serialize/optimizer.py
+-rw-r--r--   0 songci     (502) staff       (20)      724 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/serialize/serializer_impl.py
+-rw-r--r--   0 songci     (502) staff       (20)      269 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/variable_node.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-25 12:36:32.958589 aie-sdk-2.2.5/aie_sdk.egg-info/
+-rw-r--r--   0 songci     (502) staff       (20)      429 2023-05-25 12:36:32.000000 aie-sdk-2.2.5/aie_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 songci     (502) staff       (20)     1271 2023-05-25 12:36:32.000000 aie-sdk-2.2.5/aie_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 songci     (502) staff       (20)        1 2023-05-25 12:36:32.000000 aie-sdk-2.2.5/aie_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 songci     (502) staff       (20)       79 2023-05-25 12:36:32.000000 aie-sdk-2.2.5/aie_sdk.egg-info/requires.txt
+-rw-r--r--   0 songci     (502) staff       (20)        4 2023-05-25 12:36:32.000000 aie-sdk-2.2.5/aie_sdk.egg-info/top_level.txt
+-rw-r--r--   0 songci     (502) staff       (20)       38 2023-05-25 12:36:32.959934 aie-sdk-2.2.5/setup.cfg
+-rw-r--r--   0 songci     (502) staff       (20)      891 2023-04-13 02:48:49.000000 aie-sdk-2.2.5/setup.py
```

### Comparing `aie-sdk-2.2.2/LICENSE` & `aie-sdk-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/__init__.py` & `aie-sdk-2.2.5/aie/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-__version__ = "2.2.2"
+__version__ = "2.2.5"
 
 import sys
 import aie
 from .aie_env import AIEEnv
 from aie.map.aie_map import Map
 from aie.export import Export
 import types
```

### Comparing `aie-sdk-2.2.2/aie/aie_env.py` & `aie-sdk-2.2.5/aie/aie_env.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/aie_object/classifier.py` & `aie-sdk-2.2.5/aie/aie_object/classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from aie.customfunction_node import CustomFunctionNode
 from aie.function_helper import FunctionHelper
 from aie.error.aie_error import AIEError, AIEErrorCode
 
 
 class Classifier(FunctionNode):
     def __init__(self, preResult: str = "") -> aie.Classifier:
-
         if preResult is not None and not isinstance(preResult, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"preResult 只支持str类型参数, 传入类型为{type(preResult)}"
             )
 
         invoke_args = {
             "preResult": preResult,
@@ -30,15 +29,14 @@
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         super(Classifier, self).__init__("Classifier.constructors", invoke_args)
 
     def train(
         self, features: aie.FeatureCollection, classProperty: str, inputProperties: list
     ) -> aie.Classifier:
-
         if features is not None and not isinstance(features, aie.FeatureCollection):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"features 只支持aie.FeatureCollection类型参数, 传入类型为{type(features)}",
             )
 
         if classProperty is not None and not isinstance(classProperty, str):
@@ -77,15 +75,14 @@
         invoke_args["preResult"] = obj
         clf = FunctionHelper.apply("Classifier.train", "aie.Classifier", invoke_args)
 
         return clf
 
     @staticmethod
     def linearsvm() -> aie.Classifier:
-
         invoke_args = {}
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply(
             "Classifier.linearsvm", "aie.Classifier", invoke_args
         )
@@ -99,15 +96,14 @@
         gamma: [int, float] = None,
         coef0: [int, float] = 0.0,
         cost: [int, float] = 1.0,
         nu: [int, float] = 0.5,
         terminationEpsilon: [int, float] = 0.001,
         lossEpsilon: [int, float] = 0.1,
     ) -> aie.Classifier:
-
         if svmType is not None and not isinstance(svmType, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"svmType 只支持str类型参数, 传入类型为{type(svmType)}"
             )
 
         if kernelType is not None and not isinstance(kernelType, str):
             raise AIEError(
@@ -182,15 +178,14 @@
         maxDepth: int = 5,
         maxNodes: int = None,
         minLeafPopulation: int = 5,
         minWeightFraction: [int, float] = 0.0,
         minInfoGain: [int, float] = 0.0,
         seed: int = 0,
     ) -> aie.Classifier:
-
         if maxDepth is not None and not isinstance(maxDepth, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"maxDepth 只支持int类型参数, 传入类型为{type(maxDepth)}"
             )
 
         if maxNodes is not None and not isinstance(maxNodes, int):
             raise AIEError(
@@ -237,15 +232,14 @@
             "Classifier.decisionTree", "aie.Classifier", invoke_args
         )
 
     @staticmethod
     def cart(
         maxNodes: int = None, maxDepth: int = 20, minLeafPopulation: int = 5
     ) -> aie.Classifier:
-
         if maxNodes is not None and not isinstance(maxNodes, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"maxNodes 只支持int类型参数, 传入类型为{type(maxNodes)}"
             )
 
         if maxDepth is not None and not isinstance(maxDepth, int):
             raise AIEError(
@@ -272,15 +266,14 @@
     def randomForest(
         numTrees: int,
         maxDepth: int = 5,
         minLeafPopulation: int = 5,
         subsamplingRate: [int, float] = 1.0,
         seed: int = 0,
     ) -> aie.Classifier:
-
         if numTrees is not None and not isinstance(numTrees, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"numTrees 只支持int类型参数, 传入类型为{type(numTrees)}"
             )
 
         if maxDepth is not None and not isinstance(maxDepth, int):
             raise AIEError(
@@ -328,15 +321,14 @@
         numTrees: int,
         shrinkage: [int, float] = 0.005,
         samplingRate: [int, float] = 0.7,
         maxDepth: int = 20,
         maxNodes: int = None,
         minLeafPopulation: int = 5,
     ) -> aie.Classifier:
-
         if numTrees is not None and not isinstance(numTrees, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"numTrees 只支持int类型参数, 传入类型为{type(numTrees)}"
             )
 
         if shrinkage is not None and not isinstance(shrinkage, (int, float)):
             raise AIEError(
@@ -387,15 +379,14 @@
     @staticmethod
     def adaBoost(
         numTrees: int,
         maxDepth: int = 20,
         maxNodes: int = None,
         minLeafPopulation: int = 5,
     ) -> aie.Classifier:
-
         if numTrees is not None and not isinstance(numTrees, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"numTrees 只支持int类型参数, 传入类型为{type(numTrees)}"
             )
 
         if maxDepth is not None and not isinstance(maxDepth, int):
             raise AIEError(
@@ -427,15 +418,14 @@
 
         return FunctionHelper.apply(
             "Classifier.adaBoost", "aie.Classifier", invoke_args
         )
 
     @staticmethod
     def naiveBayes(smooth: [int, float] = 1.0) -> aie.Classifier:
-
         if smooth is not None and not isinstance(smooth, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"smooth 只支持(int,float)类型参数, 传入类型为{type(smooth)}",
             )
 
         invoke_args = {
@@ -445,15 +435,14 @@
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply(
             "Classifier.naiveBayes", "aie.Classifier", invoke_args
         )
 
     def confusionMatrix(self) -> aie.ConfusionMatrix:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply(
```

### Comparing `aie-sdk-2.2.2/aie/aie_object/collection.py` & `aie-sdk-2.2.5/aie/aie_object/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 class Collection(FunctionNode):
     @abc.abstractmethod
     def elementType(self):
         pass
 
     def filter(self, filter: Union[str, aie.Filter]) -> aie.Collection:
-
         if filter is not None and not isinstance(filter, (str, aie.Filter)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"filter 只支持(str,aie.Filter)类型参数, 传入类型为{type(filter)}",
             )
 
         invoke_args = {
@@ -39,15 +38,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数filter不能为空")
 
         return FunctionHelper.apply("Collection.filter", "aie.Collection", invoke_args)
 
     def filterBounds(
         self, geometry: Union[aie.Geometry, aie.Feature, aie.FeatureCollection]
     ) -> aie.Collection:
-
         if geometry is not None and not isinstance(
             geometry, (aie.Geometry, aie.Feature, aie.FeatureCollection)
         ):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"geometry 只支持(aie.Geometry,aie.Feature,aie.FeatureCollection)类型参数, 传入类型为{type(geometry)}",
             )
@@ -63,27 +61,25 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数geometry不能为空")
 
         return FunctionHelper.apply(
             "Collection.filterBounds", "aie.Collection", invoke_args
         )
 
     def first(self) -> object:
-
         invoke_args = {
             "collection": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Collection.first", "object", invoke_args)
 
     def limit(
         self, limit: int, property: str = None, ascending: bool = True
     ) -> aie.Collection:
-
         if limit is not None and not isinstance(limit, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"limit 只支持int类型参数, 传入类型为{type(limit)}"
             )
 
         if property is not None and not isinstance(property, str):
             raise AIEError(
@@ -107,15 +103,14 @@
 
         if "limit" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数limit不能为空")
 
         return FunctionHelper.apply("Collection.limit", "aie.Collection", invoke_args)
 
     def size(self) -> object:
-
         invoke_args = {
             "collection": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Collection.size", "object", invoke_args)
```

### Comparing `aie-sdk-2.2.2/aie/aie_object/confusion_matrix.py` & `aie-sdk-2.2.5/aie/aie_object/confusion_matrix.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from aie.customfunction_node import CustomFunctionNode
 from aie.function_helper import FunctionHelper
 from aie.error.aie_error import AIEError, AIEErrorCode
 
 
 class ConfusionMatrix(FunctionNode):
     def __init__(self, array: list) -> aie.ConfusionMatrix:
-
         if array is not None and not isinstance(array, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"array 只支持list类型参数, 传入类型为{type(array)}"
             )
 
         invoke_args = {
             "array": array,
@@ -33,37 +32,34 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数array不能为空")
 
         super(ConfusionMatrix, self).__init__(
             "ConfusionMatrix.constructors", invoke_args
         )
 
     def accuracy(self) -> object:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("ConfusionMatrix.accuracy", "object", invoke_args)
 
     def consumersAccuracy(self) -> object:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply(
             "ConfusionMatrix.consumersAccuracy", "object", invoke_args
         )
 
     def fscore(self, beta: [int, float] = 1.0) -> object:
-
         if beta is not None and not isinstance(beta, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"beta 只支持(int,float)类型参数, 传入类型为{type(beta)}"
             )
 
         invoke_args = {
             "input": self,
@@ -71,37 +67,34 @@
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("ConfusionMatrix.fscore", "object", invoke_args)
 
     def kappa(self) -> object:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("ConfusionMatrix.kappa", "object", invoke_args)
 
     def producersAccuracy(self) -> object:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply(
             "ConfusionMatrix.producersAccuracy", "object", invoke_args
         )
 
     def array(self) -> object:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("ConfusionMatrix.array", "object", invoke_args)
```

### Comparing `aie-sdk-2.2.2/aie/aie_object/feature.py` & `aie-sdk-2.2.5/aie/aie_object/feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,14 @@
         bbox = aie.client.InteractiveSession.getBounds(self)
         if bbox is not None and isinstance(bbox, list):
             bounds = [bbox[0], bbox[1], bbox[2], bbox[3]]
             return bounds
         raise AIEError(AIEErrorCode.ARGS_ERROR, f"获取Bounds失败. bbox: {bbox}")
 
     def get(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "input": self,
@@ -92,30 +91,28 @@
 
         if "property" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply("Feature.get", "object", invoke_args)
 
     def propertyNames(self) -> object:
-
         invoke_args = {
             "element": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Feature.propertyNames", "object", invoke_args)
 
     def select(
         self,
         propertySelectors: list,
         newProperties: list = None,
         retainGeometry: bool = True,
     ) -> object:
-
         if propertySelectors is not None and not isinstance(propertySelectors, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"propertySelectors 只支持list类型参数, 传入类型为{type(propertySelectors)}",
             )
 
         if newProperties is not None and not isinstance(newProperties, list):
@@ -141,15 +138,14 @@
 
         if "propertySelectors" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数propertySelectors不能为空")
 
         return FunctionHelper.apply("Feature.select", "object", invoke_args)
 
     def toArray(self, properties: list) -> object:
-
         if properties is not None and not isinstance(properties, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"properties 只支持list类型参数, 传入类型为{type(properties)}",
             )
 
         invoke_args = {
@@ -161,15 +157,14 @@
 
         if "properties" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数properties不能为空")
 
         return FunctionHelper.apply("Feature.toArray", "object", invoke_args)
 
     def toDictionary(self, properties: list = None) -> object:
-
         if properties is not None and not isinstance(properties, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"properties 只支持list类型参数, 传入类型为{type(properties)}",
             )
 
         invoke_args = {
@@ -178,15 +173,14 @@
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Feature.toDictionary", "object", invoke_args)
 
     def set(self, var_args: dict) -> aie.Feature:
-
         if var_args is not None and not isinstance(var_args, dict):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"var_args 只支持dict类型参数, 传入类型为{type(var_args)}"
             )
 
         invoke_args = {
             "element": self,
@@ -197,15 +191,14 @@
 
         if "var_args" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数var_args不能为空")
 
         return FunctionHelper.apply("Feature.set", "aie.Feature", invoke_args)
 
     def setGeometry(self, geometry: aie.Geometry) -> aie.Feature:
-
         if geometry is not None and not isinstance(geometry, aie.Geometry):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"geometry 只支持aie.Geometry类型参数, 传入类型为{type(geometry)}",
             )
 
         invoke_args = {
@@ -217,75 +210,68 @@
 
         if "geometry" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数geometry不能为空")
 
         return FunctionHelper.apply("Feature.setGeometry", "aie.Feature", invoke_args)
 
     def area(self) -> object:
-
         invoke_args = {
             "feature": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Feature.area", "object", invoke_args)
 
     def perimeter(self) -> object:
-
         invoke_args = {
             "feature": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Feature.perimeter", "object", invoke_args)
 
     def length(self) -> object:
-
         invoke_args = {
             "feature": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Feature.length", "object", invoke_args)
 
     def bounds(self) -> aie.Feature:
-
         invoke_args = {
             "feature": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Feature.bounds", "aie.Feature", invoke_args)
 
     def centroid(self) -> aie.Feature:
-
         invoke_args = {
             "feature": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Feature.centroid", "aie.Feature", invoke_args)
 
     def convexHull(self) -> aie.Feature:
-
         invoke_args = {
             "feature": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Feature.convexHull", "aie.Feature", invoke_args)
 
     def cutLines(self, distances: list) -> aie.Feature:
-
         if distances is not None and not isinstance(distances, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"distances 只支持list类型参数, 传入类型为{type(distances)}",
             )
 
         invoke_args = {
@@ -297,15 +283,14 @@
 
         if "distances" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数distances不能为空")
 
         return FunctionHelper.apply("Feature.cutLines", "aie.Feature", invoke_args)
 
     def simplify(self, tolerance: [int, float]) -> aie.Feature:
-
         if tolerance is not None and not isinstance(tolerance, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"tolerance 只支持(int,float)类型参数, 传入类型为{type(tolerance)}",
             )
 
         invoke_args = {
@@ -317,15 +302,14 @@
 
         if "tolerance" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数tolerance不能为空")
 
         return FunctionHelper.apply("Feature.simplify", "aie.Feature", invoke_args)
 
     def transform(self, proj: str) -> aie.Feature:
-
         if proj is not None and not isinstance(proj, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"proj 只支持str类型参数, 传入类型为{type(proj)}"
             )
 
         invoke_args = {
             "feature": self,
@@ -336,15 +320,14 @@
 
         if "proj" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数proj不能为空")
 
         return FunctionHelper.apply("Feature.transform", "aie.Feature", invoke_args)
 
     def containedIn(self, right: aie.Feature) -> object:
-
         if right is not None and not isinstance(right, aie.Feature):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"right 只支持aie.Feature类型参数, 传入类型为{type(right)}"
             )
 
         invoke_args = {
             "left": self,
@@ -355,15 +338,14 @@
 
         if "right" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply("Feature.containedIn", "object", invoke_args)
 
     def contains(self, right: aie.Feature) -> object:
-
         if right is not None and not isinstance(right, aie.Feature):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"right 只支持aie.Feature类型参数, 传入类型为{type(right)}"
             )
 
         invoke_args = {
             "left": self,
@@ -374,15 +356,14 @@
 
         if "right" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply("Feature.contains", "object", invoke_args)
 
     def difference(self, right: aie.Feature) -> aie.Feature:
-
         if right is not None and not isinstance(right, aie.Feature):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"right 只支持aie.Feature类型参数, 传入类型为{type(right)}"
             )
 
         invoke_args = {
             "left": self,
@@ -393,15 +374,14 @@
 
         if "right" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply("Feature.difference", "aie.Feature", invoke_args)
 
     def disjoint(self, right: aie.Feature) -> object:
-
         if right is not None and not isinstance(right, aie.Feature):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"right 只支持aie.Feature类型参数, 传入类型为{type(right)}"
             )
 
         invoke_args = {
             "left": self,
@@ -412,25 +392,23 @@
 
         if "right" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply("Feature.disjoint", "object", invoke_args)
 
     def dissolve(self) -> aie.Feature:
-
         invoke_args = {
             "feature": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Feature.dissolve", "aie.Feature", invoke_args)
 
     def distance(self, right: aie.Feature) -> object:
-
         if right is not None and not isinstance(right, aie.Feature):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"right 只支持aie.Feature类型参数, 传入类型为{type(right)}"
             )
 
         invoke_args = {
             "left": self,
@@ -441,15 +419,14 @@
 
         if "right" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply("Feature.distance", "object", invoke_args)
 
     def withinDistance(self, right: aie.Feature, distance: [int, float]) -> object:
-
         if right is not None and not isinstance(right, aie.Feature):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"right 只支持aie.Feature类型参数, 传入类型为{type(right)}"
             )
 
         if distance is not None and not isinstance(distance, (int, float)):
             raise AIEError(
@@ -470,15 +447,14 @@
 
         if "distance" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数distance不能为空")
 
         return FunctionHelper.apply("Feature.withinDistance", "object", invoke_args)
 
     def intersection(self, right: aie.Feature) -> aie.Feature:
-
         if right is not None and not isinstance(right, aie.Feature):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"right 只支持aie.Feature类型参数, 传入类型为{type(right)}"
             )
 
         invoke_args = {
             "left": self,
@@ -489,15 +465,14 @@
 
         if "right" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply("Feature.intersection", "aie.Feature", invoke_args)
 
     def intersects(self, right: aie.Feature) -> object:
-
         if right is not None and not isinstance(right, aie.Feature):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"right 只支持aie.Feature类型参数, 传入类型为{type(right)}"
             )
 
         invoke_args = {
             "left": self,
@@ -508,15 +483,14 @@
 
         if "right" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply("Feature.intersects", "object", invoke_args)
 
     def symmetricDifference(self, right: aie.Feature) -> aie.Feature:
-
         if right is not None and not isinstance(right, aie.Feature):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"right 只支持aie.Feature类型参数, 传入类型为{type(right)}"
             )
 
         invoke_args = {
             "left": self,
@@ -529,15 +503,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply(
             "Feature.symmetricDifference", "aie.Feature", invoke_args
         )
 
     def union(self, right: aie.Feature) -> aie.Feature:
-
         if right is not None and not isinstance(right, aie.Feature):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"right 只支持aie.Feature类型参数, 传入类型为{type(right)}"
             )
 
         invoke_args = {
             "left": self,
@@ -548,15 +521,14 @@
 
         if "right" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply("Feature.union", "aie.Feature", invoke_args)
 
     def buffer(self, distance: [int, float]) -> aie.Feature:
-
         if distance is not None and not isinstance(distance, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"distance 只支持(int,float)类型参数, 传入类型为{type(distance)}",
             )
 
         invoke_args = {
@@ -570,15 +542,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数distance不能为空")
 
         return FunctionHelper.apply("Feature.buffer", "aie.Feature", invoke_args)
 
     def copyProperties(
         self, source: aie.Feature, properties: list = None, exclude: list = None
     ) -> aie.Feature:
-
         if source is not None and not isinstance(source, aie.Feature):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"source 只支持aie.Feature类型参数, 传入类型为{type(source)}",
             )
 
         if properties is not None and not isinstance(properties, list):
@@ -605,41 +576,38 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数source不能为空")
 
         return FunctionHelper.apply(
             "Feature.copyProperties", "aie.Feature", invoke_args
         )
 
     def voronoiDiagram(self) -> aie.Feature:
-
         invoke_args = {
             "feature": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply(
             "Feature.voronoiDiagram", "aie.Feature", invoke_args
         )
 
     def delaunayTriangulation(self) -> aie.Feature:
-
         invoke_args = {
             "feature": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply(
             "Feature.delaunayTriangulation", "aie.Feature", invoke_args
         )
 
     def smooth(
         self, iterations: int, offset: [int, float], maxAngle: [int, float]
     ) -> aie.Feature:
-
         if iterations is not None and not isinstance(iterations, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"iterations 只支持int类型参数, 传入类型为{type(iterations)}",
             )
 
         if offset is not None and not isinstance(offset, (int, float)):
@@ -671,15 +639,14 @@
 
         if "maxAngle" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数maxAngle不能为空")
 
         return FunctionHelper.apply("Feature.smooth", "aie.Feature", invoke_args)
 
     def getNumber(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "input": self,
@@ -690,15 +657,14 @@
 
         if "property" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply("Feature.getNumber", "object", invoke_args)
 
     def getString(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "input": self,
@@ -709,15 +675,14 @@
 
         if "property" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply("Feature.getString", "object", invoke_args)
 
     def renamePropertyNames(self, var_args: dict) -> aie.Feature:
-
         if var_args is not None and not isinstance(var_args, dict):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"var_args 只支持dict类型参数, 传入类型为{type(var_args)}"
             )
 
         invoke_args = {
             "input": self,
```

### Comparing `aie-sdk-2.2.2/aie/aie_object/feature_collection.py` & `aie-sdk-2.2.5/aie/aie_object/feature_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,27 +62,25 @@
             return bounds
         raise AIEError(AIEErrorCode.ARGS_ERROR, f"获取Bounds失败. bbox: {bbox}")
 
     def elementType(self):
         return aie.Feature
 
     def propertyNames(self) -> object:
-
         invoke_args = {
             "element": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply(
             "FeatureCollection.propertyNames", "object", invoke_args
         )
 
     def aggregate_max(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -95,15 +93,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.aggregate_max", "object", invoke_args
         )
 
     def aggregate_min(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -116,15 +113,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.aggregate_min", "object", invoke_args
         )
 
     def aggregate_mean(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -137,15 +133,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.aggregate_mean", "object", invoke_args
         )
 
     def aggregate_count(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -158,15 +153,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.aggregate_count", "object", invoke_args
         )
 
     def aggregate_sum(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -179,15 +173,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.aggregate_sum", "object", invoke_args
         )
 
     def aggregate_stats(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -200,15 +193,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.aggregate_stats", "object", invoke_args
         )
 
     def aggregate_array(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -221,15 +213,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.aggregate_array", "object", invoke_args
         )
 
     def aggregate_product(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -242,15 +233,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.aggregate_product", "object", invoke_args
         )
 
     def aggregate_sample_sd(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -263,15 +253,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.aggregate_sample_sd", "object", invoke_args
         )
 
     def aggregate_sample_var(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -284,15 +273,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.aggregate_sample_var", "object", invoke_args
         )
 
     def aggregate_total_sd(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -305,15 +293,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.aggregate_total_sd", "object", invoke_args
         )
 
     def aggregate_total_var(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -326,15 +313,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.aggregate_total_var", "object", invoke_args
         )
 
     def aggregate_histogram(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -347,15 +333,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.aggregate_histogram", "object", invoke_args
         )
 
     def aggregate_count_distinct(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -368,15 +353,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.aggregate_count_distinct", "object", invoke_args
         )
 
     def aggregate_first(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -391,15 +375,14 @@
         return FunctionHelper.apply(
             "FeatureCollection.aggregate_first", "object", invoke_args
         )
 
     def reduceColumns(
         self, reducer: aie.Reducer, selectors: list, weightSelectors: list = None
     ) -> object:
-
         if reducer is not None and not isinstance(reducer, aie.Reducer):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"reducer 只支持aie.Reducer类型参数, 传入类型为{type(reducer)}",
             )
 
         if selectors is not None and not isinstance(selectors, list):
@@ -430,15 +413,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数selectors不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.reduceColumns", "object", invoke_args
         )
 
     def union(self, maxError: int = None) -> aie.FeatureCollection:
-
         if maxError is not None and not isinstance(maxError, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"maxError 只支持int类型参数, 传入类型为{type(maxError)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -448,15 +430,14 @@
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply(
             "FeatureCollection.union", "aie.FeatureCollection", invoke_args
         )
 
     def distinct(self, properties: list) -> aie.FeatureCollection:
-
         if properties is not None and not isinstance(properties, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"properties 只支持list类型参数, 传入类型为{type(properties)}",
             )
 
         invoke_args = {
@@ -472,24 +453,22 @@
         return FunctionHelper.apply(
             "FeatureCollection.distinct", "aie.FeatureCollection", invoke_args
         )
 
     def map(
         self, baseAlgorithm: types.FunctionType
     ) -> Union[aie.ImageCollection, aie.FeatureCollection]:
-
         node = super(FeatureCollection, self).map(baseAlgorithm)
         baseAlgorithm_return_type = type(node.invoke_args["baseAlgorithm"].body)
         if aie.Image == baseAlgorithm_return_type:
             return FunctionHelper.cast(node, "aie.ImageCollection")
         else:
             return FunctionHelper.cast(node, "aie.FeatureCollection")
 
     def merge(self, collection2: aie.FeatureCollection) -> aie.FeatureCollection:
-
         if collection2 is not None and not isinstance(
             collection2, aie.FeatureCollection
         ):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"collection2 只支持aie.FeatureCollection类型参数, 传入类型为{type(collection2)}",
             )
@@ -507,15 +486,14 @@
         return FunctionHelper.apply(
             "FeatureCollection.merge", "aie.FeatureCollection", invoke_args
         )
 
     def randomColumn(
         self, columnName: str = "random", seed: int = 0, distribution: str = "uniform"
     ) -> aie.FeatureCollection:
-
         if columnName is not None and not isinstance(columnName, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"columnName 只支持str类型参数, 传入类型为{type(columnName)}",
             )
 
         if seed is not None and not isinstance(seed, int):
@@ -542,15 +520,14 @@
             "FeatureCollection.randomColumn", "aie.FeatureCollection", invoke_args
         )
 
     @staticmethod
     def randomPoints(
         region: aie.Geometry, points: int = 1000, seed: int = 0, maxError: int = None
     ) -> aie.FeatureCollection:
-
         if region is not None and not isinstance(region, aie.Geometry):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"region 只支持aie.Geometry类型参数, 传入类型为{type(region)}",
             )
 
         if points is not None and not isinstance(points, int):
@@ -586,15 +563,14 @@
 
     def select(
         self,
         propertySelectors: list,
         newProperties: list = None,
         retainGeometry: bool = True,
     ) -> aie.FeatureCollection:
-
         if propertySelectors is not None and not isinstance(propertySelectors, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"propertySelectors 只支持list类型参数, 传入类型为{type(propertySelectors)}",
             )
 
         if newProperties is not None and not isinstance(newProperties, list):
@@ -622,51 +598,45 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数propertySelectors不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.select", "aie.FeatureCollection", invoke_args
         )
 
     def filter(self, filter: aie.Filter) -> aie.FeatureCollection:
-
         node = super(FeatureCollection, self).filter(filter)
         return FunctionHelper.cast(node, "aie.FeatureCollection")
 
     def filterBounds(
         self, geometry: Union[aie.Geometry, aie.Feature, aie.FeatureCollection]
     ) -> aie.FeatureCollection:
-
         node = super(FeatureCollection, self).filterBounds(geometry)
         return FunctionHelper.cast(node, "aie.FeatureCollection")
 
     def first(self) -> aie.Feature:
-
         node = super(FeatureCollection, self).first()
         return FunctionHelper.cast(node, "aie.Feature")
 
     def limit(
         self, max: [int, float], property: str = None, ascending: bool = None
     ) -> aie.FeatureCollection:
-
         node = super(FeatureCollection, self).limit(max, property=None, ascending=None)
         return FunctionHelper.cast(node, "aie.FeatureCollection")
 
     def geometry(self) -> aie.Geometry:
-
         invoke_args = {
             "collection": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply(
             "FeatureCollection.geometry", "aie.Geometry", invoke_args
         )
 
     def toList(self, count: int, offset: int = 0) -> object:
-
         if count is not None and not isinstance(count, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"count 只支持int类型参数, 传入类型为{type(count)}"
             )
 
         if offset is not None and not isinstance(offset, int):
             raise AIEError(
@@ -683,15 +653,14 @@
 
         if "count" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数count不能为空")
 
         return FunctionHelper.apply("FeatureCollection.toList", "object", invoke_args)
 
     def sort(self, property: str, ascending: bool = True) -> aie.FeatureCollection:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         if ascending is not None and not isinstance(ascending, bool):
             raise AIEError(
@@ -713,15 +682,14 @@
         return FunctionHelper.apply(
             "FeatureCollection.sort", "aie.FeatureCollection", invoke_args
         )
 
     def classify(
         self, classifier: aie.Classifier, outputName: str = "classification"
     ) -> aie.FeatureCollection:
-
         if classifier is not None and not isinstance(classifier, aie.Classifier):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"classifier 只支持aie.Classifier类型参数, 传入类型为{type(classifier)}",
             )
 
         if outputName is not None and not isinstance(outputName, str):
@@ -742,15 +710,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数classifier不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.classify", "aie.FeatureCollection", invoke_args
         )
 
     def errorMatrix(self, actual: str, predicted: str) -> aie.ConfusionMatrix:
-
         if actual is not None and not isinstance(actual, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"actual 只支持str类型参数, 传入类型为{type(actual)}"
             )
 
         if predicted is not None and not isinstance(predicted, str):
             raise AIEError(
@@ -772,15 +739,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数predicted不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.errorMatrix", "aie.ConfusionMatrix", invoke_args
         )
 
     def renamePropertyNames(self, var_args: dict) -> aie.FeatureCollection:
-
         if var_args is not None and not isinstance(var_args, dict):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"var_args 只支持dict类型参数, 传入类型为{type(var_args)}"
             )
 
         invoke_args = {
             "input": self,
```

### Comparing `aie-sdk-2.2.2/aie/aie_object/filter.py` & `aie-sdk-2.2.5/aie/aie_object/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from aie.function_helper import FunctionHelper
 from aie.error.aie_error import AIEError, AIEErrorCode
 
 
 class Filter(FunctionNode):
     @staticmethod
     def date(start: str, end: str = None) -> aie.Filter:
-
         if start is not None and not isinstance(start, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"start 只支持str类型参数, 传入类型为{type(start)}"
             )
 
         if end is not None and not isinstance(end, str):
             raise AIEError(AIEErrorCode.ARGS_ERROR, f"end 只支持str类型参数, 传入类型为{type(end)}")
@@ -39,15 +38,14 @@
 
         return FunctionHelper.apply("Filter.date", "aie.Filter", invoke_args)
 
     @staticmethod
     def bounds(
         geometry: Union[aie.Geometry, aie.Feature, aie.FeatureCollection]
     ) -> aie.Filter:
-
         if geometry is not None and not isinstance(
             geometry, (aie.Geometry, aie.Feature, aie.FeatureCollection)
         ):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"geometry 只支持(aie.Geometry,aie.Feature,aie.FeatureCollection)类型参数, 传入类型为{type(geometry)}",
             )
@@ -61,15 +59,14 @@
         if "geometry" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数geometry不能为空")
 
         return FunctionHelper.apply("Filter.bounds", "aie.Filter", invoke_args)
 
     @staticmethod
     def eq(name: str, value: object) -> aie.Filter:
-
         if name is not None and not isinstance(name, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"name 只支持str类型参数, 传入类型为{type(name)}"
             )
 
         if value is not None and not isinstance(value, object):
             raise AIEError(
@@ -89,15 +86,14 @@
         if "value" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数value不能为空")
 
         return FunctionHelper.apply("Filter.eq", "aie.Filter", invoke_args)
 
     @staticmethod
     def gt(name: str, value: object) -> aie.Filter:
-
         if name is not None and not isinstance(name, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"name 只支持str类型参数, 传入类型为{type(name)}"
             )
 
         if value is not None and not isinstance(value, object):
             raise AIEError(
@@ -117,15 +113,14 @@
         if "value" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数value不能为空")
 
         return FunctionHelper.apply("Filter.gt", "aie.Filter", invoke_args)
 
     @staticmethod
     def gte(name: str, value: object) -> aie.Filter:
-
         if name is not None and not isinstance(name, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"name 只支持str类型参数, 传入类型为{type(name)}"
             )
 
         if value is not None and not isinstance(value, object):
             raise AIEError(
@@ -145,15 +140,14 @@
         if "value" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数value不能为空")
 
         return FunctionHelper.apply("Filter.gte", "aie.Filter", invoke_args)
 
     @staticmethod
     def lt(name: str, value: object) -> aie.Filter:
-
         if name is not None and not isinstance(name, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"name 只支持str类型参数, 传入类型为{type(name)}"
             )
 
         if value is not None and not isinstance(value, object):
             raise AIEError(
@@ -173,15 +167,14 @@
         if "value" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数value不能为空")
 
         return FunctionHelper.apply("Filter.lt", "aie.Filter", invoke_args)
 
     @staticmethod
     def lte(name: str, value: object) -> aie.Filter:
-
         if name is not None and not isinstance(name, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"name 只支持str类型参数, 传入类型为{type(name)}"
             )
 
         if value is not None and not isinstance(value, object):
             raise AIEError(
@@ -201,15 +194,14 @@
         if "value" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数value不能为空")
 
         return FunctionHelper.apply("Filter.lte", "aie.Filter", invoke_args)
 
     @staticmethod
     def neq(name: str, value: object) -> aie.Filter:
-
         if name is not None and not isinstance(name, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"name 只支持str类型参数, 传入类型为{type(name)}"
             )
 
         if value is not None and not isinstance(value, object):
             raise AIEError(
@@ -229,15 +221,14 @@
         if "value" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数value不能为空")
 
         return FunctionHelper.apply("Filter.neq", "aie.Filter", invoke_args)
 
     @staticmethod
     def And(filters: list) -> aie.Filter:
-
         if filters is not None and not isinstance(filters, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"filters 只支持list类型参数, 传入类型为{type(filters)}"
             )
 
         invoke_args = {
             "filters": filters,
@@ -248,15 +239,14 @@
         if "filters" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数filters不能为空")
 
         return FunctionHelper.apply("Filter.and", "aie.Filter", invoke_args)
 
     @staticmethod
     def Or(filters: list) -> aie.Filter:
-
         if filters is not None and not isinstance(filters, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"filters 只支持list类型参数, 传入类型为{type(filters)}"
             )
 
         invoke_args = {
             "filters": filters,
@@ -267,26 +257,24 @@
         if "filters" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数filters不能为空")
 
         return FunctionHelper.apply("Filter.or", "aie.Filter", invoke_args)
 
     @staticmethod
     def Not() -> aie.Filter:
-
         invoke_args = {}
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Filter.not", "aie.Filter", invoke_args)
 
     @staticmethod
     def calendarRange(
         start: int, end: int = None, field: str = "day_of_year"
     ) -> aie.Filter:
-
         if start is not None and not isinstance(start, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"start 只支持int类型参数, 传入类型为{type(start)}"
             )
 
         if end is not None and not isinstance(end, int):
             raise AIEError(AIEErrorCode.ARGS_ERROR, f"end 只支持int类型参数, 传入类型为{type(end)}")
@@ -312,15 +300,14 @@
     @staticmethod
     def dateRangeContains(
         leftField: str = None,
         rightValue: object = None,
         rightField: str = None,
         leftValue: object = None,
     ) -> aie.Filter:
-
         if leftField is not None and not isinstance(leftField, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"leftField 只支持str类型参数, 传入类型为{type(leftField)}"
             )
 
         if rightValue is not None and not isinstance(rightValue, object):
             raise AIEError(
@@ -351,15 +338,14 @@
 
         return FunctionHelper.apply(
             "Filter.dateRangeContains", "aie.Filter", invoke_args
         )
 
     @staticmethod
     def dayOfYear(start: int, end: int) -> aie.Filter:
-
         if start is not None and not isinstance(start, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"start 只支持int类型参数, 传入类型为{type(start)}"
             )
 
         if end is not None and not isinstance(end, int):
             raise AIEError(AIEErrorCode.ARGS_ERROR, f"end 只支持int类型参数, 传入类型为{type(end)}")
@@ -382,15 +368,14 @@
     @staticmethod
     def equals(
         leftField: str = None,
         rightValue: object = None,
         rightField: str = None,
         leftValue: object = None,
     ) -> aie.Filter:
-
         if leftField is not None and not isinstance(leftField, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"leftField 只支持str类型参数, 传入类型为{type(leftField)}"
             )
 
         if rightValue is not None and not isinstance(rightValue, object):
             raise AIEError(
@@ -424,15 +409,14 @@
     @staticmethod
     def greaterThan(
         leftField: str = None,
         rightValue: object = None,
         rightField: str = None,
         leftValue: object = None,
     ) -> aie.Filter:
-
         if leftField is not None and not isinstance(leftField, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"leftField 只支持str类型参数, 传入类型为{type(leftField)}"
             )
 
         if rightValue is not None and not isinstance(rightValue, object):
             raise AIEError(
@@ -466,15 +450,14 @@
     @staticmethod
     def greaterThanOrEquals(
         leftField: str = None,
         rightValue: object = None,
         rightField: str = None,
         leftValue: object = None,
     ) -> aie.Filter:
-
         if leftField is not None and not isinstance(leftField, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"leftField 只支持str类型参数, 传入类型为{type(leftField)}"
             )
 
         if rightValue is not None and not isinstance(rightValue, object):
             raise AIEError(
@@ -510,15 +493,14 @@
     @staticmethod
     def lessThan(
         leftField: str = None,
         rightValue: object = None,
         rightField: str = None,
         leftValue: object = None,
     ) -> aie.Filter:
-
         if leftField is not None and not isinstance(leftField, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"leftField 只支持str类型参数, 传入类型为{type(leftField)}"
             )
 
         if rightValue is not None and not isinstance(rightValue, object):
             raise AIEError(
@@ -552,15 +534,14 @@
     @staticmethod
     def lessThanOrEquals(
         leftField: str = None,
         rightValue: object = None,
         rightField: str = None,
         leftValue: object = None,
     ) -> aie.Filter:
-
         if leftField is not None and not isinstance(leftField, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"leftField 只支持str类型参数, 传入类型为{type(leftField)}"
             )
 
         if rightValue is not None and not isinstance(rightValue, object):
             raise AIEError(
@@ -596,15 +577,14 @@
     @staticmethod
     def notEquals(
         leftField: str = None,
         rightValue: object = None,
         rightField: str = None,
         leftValue: object = None,
     ) -> aie.Filter:
-
         if leftField is not None and not isinstance(leftField, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"leftField 只支持str类型参数, 传入类型为{type(leftField)}"
             )
 
         if rightValue is not None and not isinstance(rightValue, object):
             raise AIEError(
@@ -633,15 +613,14 @@
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Filter.notEquals", "aie.Filter", invoke_args)
 
     @staticmethod
     def notNull(properties: list) -> aie.Filter:
-
         if properties is not None and not isinstance(properties, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"properties 只支持list类型参数, 传入类型为{type(properties)}",
             )
 
         invoke_args = {
```

### Comparing `aie-sdk-2.2.2/aie/aie_object/geometry.py` & `aie-sdk-2.2.5/aie/aie_object/geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,14 @@
             )
         return aie.client.Maps.getMapId(self, vis_params)
 
     @staticmethod
     def BBox(
         west: [int, float], south: [int, float], east: [int, float], north: [int, float]
     ) -> aie.Geometry:
-
         if west is not None and not isinstance(west, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"west 只支持(int,float)类型参数, 传入类型为{type(west)}"
             )
 
         if south is not None and not isinstance(south, (int, float)):
             raise AIEError(
@@ -110,15 +109,14 @@
 
         return FunctionHelper.apply(
             "GeometryConstructors.BBox", "aie.Geometry", invoke_args
         )
 
     @staticmethod
     def Point(coordinates: list) -> aie.Geometry:
-
         if coordinates is not None and not isinstance(coordinates, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"coordinates 只支持list类型参数, 传入类型为{type(coordinates)}",
             )
 
         invoke_args = {
@@ -132,15 +130,14 @@
 
         return FunctionHelper.apply(
             "GeometryConstructors.Point", "aie.Geometry", invoke_args
         )
 
     @staticmethod
     def Polygon(coordinates: list) -> aie.Geometry:
-
         if coordinates is not None and not isinstance(coordinates, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"coordinates 只支持list类型参数, 传入类型为{type(coordinates)}",
             )
 
         invoke_args = {
@@ -154,15 +151,14 @@
 
         return FunctionHelper.apply(
             "GeometryConstructors.Polygon", "aie.Geometry", invoke_args
         )
 
     @staticmethod
     def Rectangle(coordinates: list) -> aie.Geometry:
-
         if coordinates is not None and not isinstance(coordinates, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"coordinates 只支持list类型参数, 传入类型为{type(coordinates)}",
             )
 
         invoke_args = {
@@ -176,15 +172,14 @@
 
         return FunctionHelper.apply(
             "GeometryConstructors.Rectangle", "aie.Geometry", invoke_args
         )
 
     @staticmethod
     def LineString(coordinates: list) -> aie.Geometry:
-
         if coordinates is not None and not isinstance(coordinates, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"coordinates 只支持list类型参数, 传入类型为{type(coordinates)}",
             )
 
         invoke_args = {
@@ -198,15 +193,14 @@
 
         return FunctionHelper.apply(
             "GeometryConstructors.LineString", "aie.Geometry", invoke_args
         )
 
     @staticmethod
     def MultiPoint(coordinates: list) -> aie.Geometry:
-
         if coordinates is not None and not isinstance(coordinates, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"coordinates 只支持list类型参数, 传入类型为{type(coordinates)}",
             )
 
         invoke_args = {
@@ -220,15 +214,14 @@
 
         return FunctionHelper.apply(
             "GeometryConstructors.MultiPoint", "aie.Geometry", invoke_args
         )
 
     @staticmethod
     def MultiLineString(coordinates: list) -> aie.Geometry:
-
         if coordinates is not None and not isinstance(coordinates, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"coordinates 只支持list类型参数, 传入类型为{type(coordinates)}",
             )
 
         invoke_args = {
@@ -242,15 +235,14 @@
 
         return FunctionHelper.apply(
             "GeometryConstructors.MultiLineString", "aie.Geometry", invoke_args
         )
 
     @staticmethod
     def MultiPolygon(coordinates: list) -> aie.Geometry:
-
         if coordinates is not None and not isinstance(coordinates, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"coordinates 只支持list类型参数, 传入类型为{type(coordinates)}",
             )
 
         invoke_args = {
@@ -263,41 +255,38 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数coordinates不能为空")
 
         return FunctionHelper.apply(
             "GeometryConstructors.MultiPolygon", "aie.Geometry", invoke_args
         )
 
     def voronoiDiagram(self) -> aie.Geometry:
-
         invoke_args = {
             "geometry": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply(
             "Geometry.voronoiDiagram", "aie.Geometry", invoke_args
         )
 
     def delaunayTriangulation(self) -> aie.Geometry:
-
         invoke_args = {
             "geometry": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply(
             "Geometry.delaunayTriangulation", "aie.Geometry", invoke_args
         )
 
     def smooth(
         self, iterations: int, offset: [int, float], maxAngle: [int, float]
     ) -> aie.Geometry:
-
         if iterations is not None and not isinstance(iterations, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"iterations 只支持int类型参数, 传入类型为{type(iterations)}",
             )
 
         if offset is not None and not isinstance(offset, (int, float)):
@@ -329,95 +318,86 @@
 
         if "maxAngle" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数maxAngle不能为空")
 
         return FunctionHelper.apply("Geometry.smooth", "aie.Geometry", invoke_args)
 
     def area(self) -> object:
-
         invoke_args = {
             "geometry": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Geometry.area", "object", invoke_args)
 
     def perimeter(self) -> object:
-
         invoke_args = {
             "geometry": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Geometry.perimeter", "object", invoke_args)
 
     def length(self) -> object:
-
         invoke_args = {
             "geometry": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Geometry.length", "object", invoke_args)
 
     def coordinates(self) -> object:
-
         invoke_args = {
             "geometry": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Geometry.coordinates", "object", invoke_args)
 
     def type(self) -> object:
-
         invoke_args = {
             "geometry": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Geometry.type", "object", invoke_args)
 
     def bounds(self) -> aie.Geometry:
-
         invoke_args = {
             "geometry": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Geometry.bounds", "aie.Geometry", invoke_args)
 
     def centroid(self) -> aie.Geometry:
-
         invoke_args = {
             "geometry": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Geometry.centroid", "aie.Geometry", invoke_args)
 
     def convexHull(self) -> aie.Geometry:
-
         invoke_args = {
             "geometry": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Geometry.convexHull", "aie.Geometry", invoke_args)
 
     def cutLines(self, distance: list) -> aie.Geometry:
-
         if distance is not None and not isinstance(distance, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"distance 只支持list类型参数, 传入类型为{type(distance)}"
             )
 
         invoke_args = {
             "geometry": self,
@@ -428,15 +408,14 @@
 
         if "distance" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数distance不能为空")
 
         return FunctionHelper.apply("Geometry.cutLines", "aie.Geometry", invoke_args)
 
     def simplify(self, tolerance: [int, float]) -> aie.Geometry:
-
         if tolerance is not None and not isinstance(tolerance, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"tolerance 只支持(int,float)类型参数, 传入类型为{type(tolerance)}",
             )
 
         invoke_args = {
@@ -448,15 +427,14 @@
 
         if "tolerance" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数tolerance不能为空")
 
         return FunctionHelper.apply("Geometry.simplify", "aie.Geometry", invoke_args)
 
     def transform(self, proj: str) -> aie.Geometry:
-
         if proj is not None and not isinstance(proj, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"proj 只支持str类型参数, 传入类型为{type(proj)}"
             )
 
         invoke_args = {
             "geometry": self,
@@ -467,15 +445,14 @@
 
         if "proj" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数proj不能为空")
 
         return FunctionHelper.apply("Geometry.transform", "aie.Geometry", invoke_args)
 
     def distance(self, right: aie.Geometry) -> object:
-
         if right is not None and not isinstance(right, aie.Geometry):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"right 只支持aie.Geometry类型参数, 传入类型为{type(right)}",
             )
 
         invoke_args = {
@@ -487,15 +464,14 @@
 
         if "right" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply("Geometry.distance", "object", invoke_args)
 
     def withinDistance(self, right: aie.Geometry, distance: [int, float]) -> object:
-
         if right is not None and not isinstance(right, aie.Geometry):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"right 只支持aie.Geometry类型参数, 传入类型为{type(right)}",
             )
 
         if distance is not None and not isinstance(distance, (int, float)):
@@ -517,15 +493,14 @@
 
         if "distance" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数distance不能为空")
 
         return FunctionHelper.apply("Geometry.withinDistance", "object", invoke_args)
 
     def containedIn(self, right: aie.Geometry) -> object:
-
         if right is not None and not isinstance(right, aie.Geometry):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"right 只支持aie.Geometry类型参数, 传入类型为{type(right)}",
             )
 
         invoke_args = {
@@ -537,15 +512,14 @@
 
         if "right" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply("Geometry.containedIn", "object", invoke_args)
 
     def contains(self, right: aie.Geometry) -> object:
-
         if right is not None and not isinstance(right, aie.Geometry):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"right 只支持aie.Geometry类型参数, 传入类型为{type(right)}",
             )
 
         invoke_args = {
@@ -557,15 +531,14 @@
 
         if "right" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply("Geometry.contains", "object", invoke_args)
 
     def difference(self, right: aie.Geometry) -> aie.Geometry:
-
         if right is not None and not isinstance(right, aie.Geometry):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"right 只支持aie.Geometry类型参数, 传入类型为{type(right)}",
             )
 
         invoke_args = {
@@ -577,15 +550,14 @@
 
         if "right" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply("Geometry.difference", "aie.Geometry", invoke_args)
 
     def disjoint(self, right: aie.Geometry) -> object:
-
         if right is not None and not isinstance(right, aie.Geometry):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"right 只支持aie.Geometry类型参数, 传入类型为{type(right)}",
             )
 
         invoke_args = {
@@ -597,25 +569,23 @@
 
         if "right" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply("Geometry.disjoint", "object", invoke_args)
 
     def dissolve(self) -> aie.Geometry:
-
         invoke_args = {
             "geometry": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Geometry.dissolve", "aie.Geometry", invoke_args)
 
     def intersection(self, right: aie.Geometry) -> aie.Geometry:
-
         if right is not None and not isinstance(right, aie.Geometry):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"right 只支持aie.Geometry类型参数, 传入类型为{type(right)}",
             )
 
         invoke_args = {
@@ -629,15 +599,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply(
             "Geometry.intersection", "aie.Geometry", invoke_args
         )
 
     def intersects(self, right: aie.Geometry) -> object:
-
         if right is not None and not isinstance(right, aie.Geometry):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"right 只支持aie.Geometry类型参数, 传入类型为{type(right)}",
             )
 
         invoke_args = {
@@ -649,15 +618,14 @@
 
         if "right" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply("Geometry.intersects", "object", invoke_args)
 
     def symmetricDifference(self, right: aie.Geometry) -> aie.Geometry:
-
         if right is not None and not isinstance(right, aie.Geometry):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"right 只支持aie.Geometry类型参数, 传入类型为{type(right)}",
             )
 
         invoke_args = {
@@ -671,15 +639,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply(
             "Geometry.symmetricDifference", "aie.Geometry", invoke_args
         )
 
     def union(self, right: aie.Geometry) -> aie.Geometry:
-
         if right is not None and not isinstance(right, aie.Geometry):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"right 只支持aie.Geometry类型参数, 传入类型为{type(right)}",
             )
 
         invoke_args = {
@@ -691,15 +658,14 @@
 
         if "right" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply("Geometry.union", "aie.Geometry", invoke_args)
 
     def buffer(self, distance: [int, float]) -> aie.Geometry:
-
         if distance is not None and not isinstance(distance, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"distance 只支持(int,float)类型参数, 传入类型为{type(distance)}",
             )
 
         invoke_args = {
@@ -711,15 +677,14 @@
 
         if "distance" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数distance不能为空")
 
         return FunctionHelper.apply("Geometry.buffer", "aie.Geometry", invoke_args)
 
     def geometries(self) -> object:
-
         invoke_args = {
             "geometry": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Geometry.geometries", "object", invoke_args)
```

### Comparing `aie-sdk-2.2.2/aie/aie_object/image.py` & `aie-sdk-2.2.5/aie/aie_object/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,14 @@
         else:
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"args 只支持number|str|list类型参数, 传入类型为{type(args)}",
             )
 
     def select(self, bandSelectors: Union[str, list]) -> aie.Image:
-
         if bandSelectors is not None and not isinstance(bandSelectors, (str, list)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"bandSelectors 只支持(str,list)类型参数, 传入类型为{type(bandSelectors)}",
             )
 
         if isinstance(bandSelectors, str):
@@ -68,15 +67,14 @@
 
         if "bandSelectors" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数bandSelectors不能为空")
 
         return FunctionHelper.apply("Image.select", "aie.Image", invoke_args)
 
     def rename(self, names: list) -> aie.Image:
-
         if names is not None and not isinstance(names, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"names 只支持list类型参数, 传入类型为{type(names)}"
             )
 
         invoke_args = {
             "input": self,
@@ -87,15 +85,14 @@
 
         if "names" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数names不能为空")
 
         return FunctionHelper.apply("Image.rename", "aie.Image", invoke_args)
 
     def normalizedDifference(self, bandNames: list) -> aie.Image:
-
         if bandNames is not None and not isinstance(bandNames, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"bandNames 只支持list类型参数, 传入类型为{type(bandNames)}",
             )
 
         invoke_args = {
@@ -109,15 +106,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数bandNames不能为空")
 
         return FunctionHelper.apply(
             "Image.normalizedDifference", "aie.Image", invoke_args
         )
 
     def expression(self, expression: str, map: dict = None) -> aie.Image:
-
         if expression is not None and not isinstance(expression, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"expression 只支持str类型参数, 传入类型为{type(expression)}",
             )
 
         if map is not None and not isinstance(map, dict):
@@ -157,15 +153,14 @@
         bbox = aie.client.InteractiveSession.getBounds(self)
         if bbox is not None and isinstance(bbox, list):
             bounds = [bbox[0], bbox[1], bbox[2], bbox[3]]
             return bounds
         raise AIEError(AIEErrorCode.ARGS_ERROR, f"获取Bounds失败. bbox: {bbox}")
 
     def where(self, test: aie.Image, value: aie.Image) -> aie.Image:
-
         if test is not None and not isinstance(test, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"test 只支持aie.Image类型参数, 传入类型为{type(test)}"
             )
 
         if value is not None and not isinstance(value, aie.Image):
             raise AIEError(
@@ -185,35 +180,32 @@
 
         if "value" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数value不能为空")
 
         return FunctionHelper.apply("Image.where", "aie.Image", invoke_args)
 
     def abs(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.abs", "aie.Image", invoke_args)
 
     def acos(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.acos", "aie.Image", invoke_args)
 
     def add(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -224,45 +216,41 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.add", "aie.Image", invoke_args)
 
     def asin(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.asin", "aie.Image", invoke_args)
 
     def atan(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.atan", "aie.Image", invoke_args)
 
     def ceil(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.ceil", "aie.Image", invoke_args)
 
     def clamp(self, low: [int, float], high: [int, float]) -> aie.Image:
-
         if low is not None and not isinstance(low, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"low 只支持(int,float)类型参数, 传入类型为{type(low)}"
             )
 
         if high is not None and not isinstance(high, (int, float)):
             raise AIEError(
@@ -282,25 +270,23 @@
 
         if "high" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数high不能为空")
 
         return FunctionHelper.apply("Image.clamp", "aie.Image", invoke_args)
 
     def cos(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.cos", "aie.Image", invoke_args)
 
     def divide(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -311,55 +297,50 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.divide", "aie.Image", invoke_args)
 
     def exp(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.exp", "aie.Image", invoke_args)
 
     def floor(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.floor", "aie.Image", invoke_args)
 
     def log(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.log", "aie.Image", invoke_args)
 
     def log10(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.log10", "aie.Image", invoke_args)
 
     def max(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -370,15 +351,14 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.max", "aie.Image", invoke_args)
 
     def min(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -389,15 +369,14 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.min", "aie.Image", invoke_args)
 
     def mod(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -408,15 +387,14 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.mod", "aie.Image", invoke_args)
 
     def multiply(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -427,15 +405,14 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.multiply", "aie.Image", invoke_args)
 
     def pow(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -446,55 +423,50 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.pow", "aie.Image", invoke_args)
 
     def round(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.round", "aie.Image", invoke_args)
 
     def signum(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.signum", "aie.Image", invoke_args)
 
     def sin(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.sin", "aie.Image", invoke_args)
 
     def sqrt(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.sqrt", "aie.Image", invoke_args)
 
     def subtract(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -505,25 +477,23 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.subtract", "aie.Image", invoke_args)
 
     def tan(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.tan", "aie.Image", invoke_args)
 
     def eq(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -534,15 +504,14 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.eq", "aie.Image", invoke_args)
 
     def gt(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -553,15 +522,14 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.gt", "aie.Image", invoke_args)
 
     def gte(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -572,15 +540,14 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.gte", "aie.Image", invoke_args)
 
     def lt(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -591,15 +558,14 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.lt", "aie.Image", invoke_args)
 
     def lte(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -610,15 +576,14 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.lte", "aie.Image", invoke_args)
 
     def neq(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -629,15 +594,14 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.neq", "aie.Image", invoke_args)
 
     def And(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -648,25 +612,23 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.and", "aie.Image", invoke_args)
 
     def Not(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.not", "aie.Image", invoke_args)
 
     def Or(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -677,15 +639,14 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.or", "aie.Image", invoke_args)
 
     def bitwiseAnd(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -696,25 +657,23 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.bitwiseAnd", "aie.Image", invoke_args)
 
     def bitwiseNot(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.bitwiseNot", "aie.Image", invoke_args)
 
     def bitwiseOr(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -725,15 +684,14 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.bitwiseOr", "aie.Image", invoke_args)
 
     def bitwiseXor(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -744,15 +702,14 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.bitwiseXor", "aie.Image", invoke_args)
 
     def leftShift(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -763,15 +720,14 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.leftShift", "aie.Image", invoke_args)
 
     def rightShift(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -782,15 +738,14 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.rightShift", "aie.Image", invoke_args)
 
     def mask(self, mask: aie.Image = None) -> aie.Image:
-
         if mask is not None and not isinstance(mask, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"mask 只支持aie.Image类型参数, 传入类型为{type(mask)}"
             )
 
         invoke_args = {
             "input": self,
@@ -798,15 +753,14 @@
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.mask", "aie.Image", invoke_args)
 
     def unmask(self, value: aie.Image = None, sameFootprint: bool = True) -> aie.Image:
-
         if value is not None and not isinstance(value, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"value 只支持aie.Image类型参数, 传入类型为{type(value)}"
             )
 
         if sameFootprint is not None and not isinstance(sameFootprint, bool):
             raise AIEError(
@@ -821,15 +775,14 @@
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.unmask", "aie.Image", invoke_args)
 
     def updateMask(self, mask: aie.Image) -> aie.Image:
-
         if mask is not None and not isinstance(mask, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"mask 只支持aie.Image类型参数, 传入类型为{type(mask)}"
             )
 
         invoke_args = {
             "image": self,
@@ -846,15 +799,14 @@
     def focalMax(
         self,
         radius: [int, float] = 1.0,
         kernelType: str = "square",
         units: str = "pixels",
         iterations: int = 1,
     ) -> aie.Image:
-
         if radius is not None and not isinstance(radius, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"radius 只支持(int,float)类型参数, 传入类型为{type(radius)}",
             )
 
         if kernelType is not None and not isinstance(kernelType, str):
@@ -889,15 +841,14 @@
     def focalMean(
         self,
         radius: [int, float] = 1.0,
         kernelType: str = "square",
         units: str = "pixels",
         iterations: int = 1,
     ) -> aie.Image:
-
         if radius is not None and not isinstance(radius, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"radius 只支持(int,float)类型参数, 传入类型为{type(radius)}",
             )
 
         if kernelType is not None and not isinstance(kernelType, str):
@@ -932,15 +883,14 @@
     def focalMedian(
         self,
         radius: [int, float] = 1.0,
         kernelType: str = "square",
         units: str = "pixels",
         iterations: int = 1,
     ) -> aie.Image:
-
         if radius is not None and not isinstance(radius, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"radius 只支持(int,float)类型参数, 传入类型为{type(radius)}",
             )
 
         if kernelType is not None and not isinstance(kernelType, str):
@@ -975,15 +925,14 @@
     def focalMin(
         self,
         radius: [int, float] = 1.0,
         kernelType: str = "square",
         units: str = "pixels",
         iterations: int = 1,
     ) -> aie.Image:
-
         if radius is not None and not isinstance(radius, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"radius 只支持(int,float)类型参数, 传入类型为{type(radius)}",
             )
 
         if kernelType is not None and not isinstance(kernelType, str):
@@ -1018,15 +967,14 @@
     def focalMode(
         self,
         radius: [int, float] = 1.0,
         kernelType: str = "square",
         units: str = "pixels",
         iterations: int = 1,
     ) -> aie.Image:
-
         if radius is not None and not isinstance(radius, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"radius 只支持(int,float)类型参数, 传入类型为{type(radius)}",
             )
 
         if kernelType is not None and not isinstance(kernelType, str):
@@ -1061,15 +1009,14 @@
     def focalSum(
         self,
         radius: [int, float] = 1.0,
         kernelType: str = "square",
         units: str = "pixels",
         iterations: int = 1,
     ) -> aie.Image:
-
         if radius is not None and not isinstance(radius, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"radius 只支持(int,float)类型参数, 传入类型为{type(radius)}",
             )
 
         if kernelType is not None and not isinstance(kernelType, str):
@@ -1104,15 +1051,14 @@
     def focalStandardDeviation(
         self,
         radius: [int, float] = 1.0,
         kernelType: str = "square",
         units: str = "pixels",
         iterations: int = 1,
     ) -> aie.Image:
-
         if radius is not None and not isinstance(radius, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"radius 只支持(int,float)类型参数, 传入类型为{type(radius)}",
             )
 
         if kernelType is not None and not isinstance(kernelType, str):
@@ -1149,15 +1095,14 @@
     def focalConway(
         self,
         radius: [int, float] = 1.0,
         kernelType: str = "square",
         units: str = "pixels",
         iterations: int = 1,
     ) -> aie.Image:
-
         if radius is not None and not isinstance(radius, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"radius 只支持(int,float)类型参数, 传入类型为{type(radius)}",
             )
 
         if kernelType is not None and not isinstance(kernelType, str):
@@ -1186,15 +1131,14 @@
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.focalConway", "aie.Image", invoke_args)
 
     def reduce(self, reducer: aie.Reducer) -> aie.Image:
-
         if reducer is not None and not isinstance(reducer, aie.Reducer):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"reducer 只支持aie.Reducer类型参数, 传入类型为{type(reducer)}",
             )
 
         invoke_args = {
@@ -1211,15 +1155,14 @@
 
     def reduceRegion(
         self,
         reducer: aie.Reducer,
         geometry: aie.Geometry = None,
         scale: [int, float] = None,
     ) -> object:
-
         if reducer is not None and not isinstance(reducer, aie.Reducer):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"reducer 只支持aie.Reducer类型参数, 传入类型为{type(reducer)}",
             )
 
         if geometry is not None and not isinstance(geometry, aie.Geometry):
@@ -1249,15 +1192,14 @@
 
     def reduceRegions(
         self,
         collection: aie.FeatureCollection,
         reducer: aie.Reducer,
         scale: [int, float] = None,
     ) -> aie.FeatureCollection:
-
         if collection is not None and not isinstance(collection, aie.FeatureCollection):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"collection 只支持aie.FeatureCollection类型参数, 传入类型为{type(collection)}",
             )
 
         if reducer is not None and not isinstance(reducer, aie.Reducer):
@@ -1287,15 +1229,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数reducer不能为空")
 
         return FunctionHelper.apply(
             "Image.reduceRegions", "aie.FeatureCollection", invoke_args
         )
 
     def clip(self, geometry: Union[aie.Geometry, aie.Feature]) -> aie.Image:
-
         if geometry is not None and not isinstance(
             geometry, (aie.Geometry, aie.Feature)
         ):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"geometry 只支持(aie.Geometry,aie.Feature)类型参数, 传入类型为{type(geometry)}",
             )
@@ -1311,15 +1252,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数geometry不能为空")
 
         return FunctionHelper.apply("Image.clip", "aie.Image", invoke_args)
 
     def addBands(
         self, srcImg: aie.Image, names: list = None, overwrite: bool = False
     ) -> aie.Image:
-
         if srcImg is not None and not isinstance(srcImg, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"srcImg 只支持aie.Image类型参数, 传入类型为{type(srcImg)}"
             )
 
         if names is not None and not isinstance(names, list):
             raise AIEError(
@@ -1344,15 +1284,14 @@
         if "srcImg" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数srcImg不能为空")
 
         return FunctionHelper.apply("Image.addBands", "aie.Image", invoke_args)
 
     @staticmethod
     def constant(value: Union[int, float, list]) -> aie.Image:
-
         if value is not None and not isinstance(value, (int, float, list)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"value 只支持(int,float,list)类型参数, 传入类型为{type(value)}",
             )
 
         invoke_args = {
@@ -1363,45 +1302,41 @@
 
         if "value" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数value不能为空")
 
         return FunctionHelper.apply("Image.constant", "aie.Image", invoke_args)
 
     def bandNames(self) -> object:
-
         invoke_args = {
             "image": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.bandNames", "object", invoke_args)
 
     def bandTypes(self) -> object:
-
         invoke_args = {
             "image": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.bandTypes", "object", invoke_args)
 
     def date(self) -> object:
-
         invoke_args = {
             "image": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.date", "object", invoke_args)
 
     def get(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "input": self,
@@ -1413,15 +1348,14 @@
         if "property" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply("Image.get", "object", invoke_args)
 
     @staticmethod
     def rgb(r: aie.Image, g: aie.Image, b: aie.Image) -> aie.Image:
-
         if r is not None and not isinstance(r, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"r 只支持aie.Image类型参数, 传入类型为{type(r)}"
             )
 
         if g is not None and not isinstance(g, aie.Image):
             raise AIEError(
@@ -1449,35 +1383,32 @@
 
         if "b" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数b不能为空")
 
         return FunctionHelper.apply("Image.rgb", "aie.Image", invoke_args)
 
     def rgbToHsv(self) -> aie.Image:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.rgbToHsv", "aie.Image", invoke_args)
 
     def hsvToRgb(self) -> aie.Image:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.hsvToRgb", "aie.Image", invoke_args)
 
     def unitScale(self, low: [int, float], high: [int, float]) -> aie.Image:
-
         if low is not None and not isinstance(low, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"low 只支持(int,float)类型参数, 传入类型为{type(low)}"
             )
 
         if high is not None and not isinstance(high, (int, float)):
             raise AIEError(
@@ -1497,45 +1428,41 @@
 
         if "high" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数high不能为空")
 
         return FunctionHelper.apply("Image.unitScale", "aie.Image", invoke_args)
 
     def sinh(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.sinh", "aie.Image", invoke_args)
 
     def cosh(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.cosh", "aie.Image", invoke_args)
 
     def tanh(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.tanh", "aie.Image", invoke_args)
 
     def atan2(self, right: aie.Image) -> aie.Image:
-
         if right is not None and not isinstance(right, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"right 只支持aie.Image类型参数, 传入类型为{type(right)}"
             )
 
         invoke_args = {
             "left": self,
@@ -1546,15 +1473,14 @@
 
         if "right" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply("Image.atan2", "aie.Image", invoke_args)
 
     def fastAtan2(self, right: aie.Image) -> aie.Image:
-
         if right is not None and not isinstance(right, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"right 只支持aie.Image类型参数, 传入类型为{type(right)}"
             )
 
         invoke_args = {
             "left": self,
@@ -1565,15 +1491,14 @@
 
         if "right" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数right不能为空")
 
         return FunctionHelper.apply("Image.fastAtan2", "aie.Image", invoke_args)
 
     def convolve(self, kernel: aie.Kernel) -> aie.Image:
-
         if kernel is not None and not isinstance(kernel, aie.Kernel):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"kernel 只支持aie.Kernel类型参数, 传入类型为{type(kernel)}",
             )
 
         invoke_args = {
@@ -1585,95 +1510,86 @@
 
         if "kernel" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数kernel不能为空")
 
         return FunctionHelper.apply("Image.convolve", "aie.Image", invoke_args)
 
     def toByte(self) -> aie.Image:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.toByte", "aie.Image", invoke_args)
 
     def toInt16(self) -> aie.Image:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.toInt16", "aie.Image", invoke_args)
 
     def toUint16(self) -> aie.Image:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.toUint16", "aie.Image", invoke_args)
 
     def toInt32(self) -> aie.Image:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.toInt32", "aie.Image", invoke_args)
 
     def toUint32(self) -> aie.Image:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.toUint32", "aie.Image", invoke_args)
 
     def toFloat(self) -> aie.Image:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.toFloat", "aie.Image", invoke_args)
 
     def toDouble(self) -> aie.Image:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.toDouble", "aie.Image", invoke_args)
 
     def selfMask(self) -> aie.Image:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.selfMask", "aie.Image", invoke_args)
 
     def polynomial(self, coeffs: list) -> aie.Image:
-
         if coeffs is not None and not isinstance(coeffs, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"coeffs 只支持list类型参数, 传入类型为{type(coeffs)}"
             )
 
         invoke_args = {
             "input": self,
@@ -1684,25 +1600,23 @@
 
         if "coeffs" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数coeffs不能为空")
 
         return FunctionHelper.apply("Image.polynomial", "aie.Image", invoke_args)
 
     def gamma(self) -> aie.Image:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.gamma", "aie.Image", invoke_args)
 
     def digamma(self) -> aie.Image:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.digamma", "aie.Image", invoke_args)
@@ -1710,15 +1624,14 @@
     def remap(
         self,
         fromValue: list,
         toValue: list,
         defaultValue: [int, float] = None,
         bandName: str = None,
     ) -> aie.Image:
-
         if fromValue is not None and not isinstance(fromValue, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"fromValue 只支持list类型参数, 传入类型为{type(fromValue)}",
             )
 
         if toValue is not None and not isinstance(toValue, list):
@@ -1752,75 +1665,68 @@
 
         if "toValue" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数toValue不能为空")
 
         return FunctionHelper.apply("Image.remap", "aie.Image", invoke_args)
 
     def erf(self) -> aie.Image:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.erf", "aie.Image", invoke_args)
 
     def erfc(self) -> aie.Image:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.erfc", "aie.Image", invoke_args)
 
     def erfInv(self) -> aie.Image:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.erfInv", "aie.Image", invoke_args)
 
     def erfcInv(self) -> aie.Image:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.erfcInv", "aie.Image", invoke_args)
 
     def pixelArea(self) -> aie.Image:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.pixelArea", "aie.Image", invoke_args)
 
     def derivative(self) -> aie.Image:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.derivative", "aie.Image", invoke_args)
 
     def entropy(self, kernel: aie.Kernel) -> aie.Image:
-
         if kernel is not None and not isinstance(kernel, aie.Kernel):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"kernel 只支持aie.Kernel类型参数, 传入类型为{type(kernel)}",
             )
 
         invoke_args = {
@@ -1832,15 +1738,14 @@
 
         if "kernel" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数kernel不能为空")
 
         return FunctionHelper.apply("Image.entropy", "aie.Image", invoke_args)
 
     def distance(self, kernel: aie.Kernel, skipMasked: bool = True) -> aie.Image:
-
         if kernel is not None and not isinstance(kernel, aie.Kernel):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"kernel 只支持aie.Kernel类型参数, 传入类型为{type(kernel)}",
             )
 
         if skipMasked is not None and not isinstance(skipMasked, bool):
@@ -1861,15 +1766,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数kernel不能为空")
 
         return FunctionHelper.apply("Image.distance", "aie.Image", invoke_args)
 
     def spectralDilation(
         self, metric: str = "sam", kernel: aie.Kernel = None, useCentroid: bool = False
     ) -> aie.Image:
-
         if metric is not None and not isinstance(metric, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"metric 只支持str类型参数, 传入类型为{type(metric)}"
             )
 
         if kernel is not None and not isinstance(kernel, aie.Kernel):
             raise AIEError(
@@ -1893,15 +1797,14 @@
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.spectralDilation", "aie.Image", invoke_args)
 
     def spectralErosion(
         self, metric: str = "sam", kernel: aie.Kernel = None, useCentroid: bool = False
     ) -> aie.Image:
-
         if metric is not None and not isinstance(metric, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"metric 只支持str类型参数, 传入类型为{type(metric)}"
             )
 
         if kernel is not None and not isinstance(kernel, aie.Kernel):
             raise AIEError(
@@ -1925,15 +1828,14 @@
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.spectralErosion", "aie.Image", invoke_args)
 
     def spectralGradient(
         self, metric: str = "sam", kernel: aie.Kernel = None, useCentroid: bool = False
     ) -> aie.Image:
-
         if metric is not None and not isinstance(metric, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"metric 只支持str类型参数, 传入类型为{type(metric)}"
             )
 
         if kernel is not None and not isinstance(kernel, aie.Kernel):
             raise AIEError(
@@ -1955,15 +1857,14 @@
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.spectralGradient", "aie.Image", invoke_args)
 
     def spectralDistance(self, image2: aie.Image, metric: str = "sam") -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         if metric is not None and not isinstance(metric, str):
             raise AIEError(
@@ -1980,25 +1881,23 @@
 
         if "image2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.spectralDistance", "aie.Image", invoke_args)
 
     def lanczos(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.lanczos", "aie.Image", invoke_args)
 
     def pixelCoordinates(self, projection: str) -> aie.Image:
-
         if projection is not None and not isinstance(projection, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"projection 只支持str类型参数, 传入类型为{type(projection)}",
             )
 
         invoke_args = {
@@ -2010,25 +1909,23 @@
 
         if "projection" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数projection不能为空")
 
         return FunctionHelper.apply("Image.pixelCoordinates", "aie.Image", invoke_args)
 
     def pixelLonLat(self) -> aie.Image:
-
         invoke_args = {
             "value": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.pixelLonLat", "aie.Image", invoke_args)
 
     def unmix(self, endmembers: list) -> aie.Image:
-
         if endmembers is not None and not isinstance(endmembers, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"endmembers 只支持list类型参数, 传入类型为{type(endmembers)}",
             )
 
         invoke_args = {
@@ -2040,15 +1937,14 @@
 
         if "endmembers" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数endmembers不能为空")
 
         return FunctionHelper.apply("Image.unmix", "aie.Image", invoke_args)
 
     def clipToCollection(self, collection: aie.FeatureCollection) -> aie.Image:
-
         if collection is not None and not isinstance(collection, aie.FeatureCollection):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"collection 只支持aie.FeatureCollection类型参数, 传入类型为{type(collection)}",
             )
 
         invoke_args = {
@@ -2060,25 +1956,23 @@
 
         if "collection" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数collection不能为空")
 
         return FunctionHelper.apply("Image.clipToCollection", "aie.Image", invoke_args)
 
     def propertyNames(self) -> object:
-
         invoke_args = {
             "element": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.propertyNames", "object", invoke_args)
 
     def copyProperties(self, image2: aie.Image) -> aie.Image:
-
         if image2 is not None and not isinstance(image2, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"image2 只支持aie.Image类型参数, 传入类型为{type(image2)}"
             )
 
         invoke_args = {
             "image1": self,
@@ -2091,15 +1985,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数image2不能为空")
 
         return FunctionHelper.apply("Image.copyProperties", "aie.Image", invoke_args)
 
     def classify(
         self, classifier: aie.Classifier, outputName: str = "classification"
     ) -> aie.Image:
-
         if classifier is not None and not isinstance(classifier, aie.Classifier):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"classifier 只支持aie.Classifier类型参数, 传入类型为{type(classifier)}",
             )
 
         if outputName is not None and not isinstance(outputName, str):
@@ -2125,15 +2018,14 @@
         self,
         region: aie.Geometry,
         scale: [int, float],
         numPixels: int,
         seed: int = 0,
         geometries: bool = False,
     ) -> aie.FeatureCollection:
-
         if region is not None and not isinstance(region, aie.Geometry):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"region 只支持aie.Geometry类型参数, 传入类型为{type(region)}",
             )
 
         if scale is not None and not isinstance(scale, (int, float)):
@@ -2178,35 +2070,32 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数numPixels不能为空")
 
         return FunctionHelper.apply(
             "Image.sample", "aie.FeatureCollection", invoke_args
         )
 
     def mask(self) -> aie.Image:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.mask", "aie.Image", invoke_args)
 
     def id(self) -> object:
-
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.id", "object", invoke_args)
 
     def getNumber(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "input": self,
@@ -2217,15 +2106,14 @@
 
         if "property" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply("Image.getNumber", "object", invoke_args)
 
     def getString(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "input": self,
@@ -2236,15 +2124,14 @@
 
         if "property" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply("Image.getString", "object", invoke_args)
 
     def random(self, seed: int = 0, distribution: str = "uniform") -> aie.Image:
-
         if seed is not None and not isinstance(seed, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"seed 只支持int类型参数, 传入类型为{type(seed)}"
             )
 
         if distribution is not None and not isinstance(distribution, str):
             raise AIEError(
@@ -2261,15 +2148,14 @@
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Image.random", "aie.Image", invoke_args)
 
     def sampleRegion(
         self, region: aie.Geometry, scale: [int, float], geometries: bool = False
     ) -> aie.FeatureCollection:
-
         if region is not None and not isinstance(region, aie.Geometry):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"region 只支持aie.Geometry类型参数, 传入类型为{type(region)}",
             )
 
         if scale is not None and not isinstance(scale, (int, float)):
@@ -2305,15 +2191,14 @@
     def sampleRegions(
         self,
         collection: aie.FeatureCollection,
         scale: [int, float],
         properties: list = None,
         geometries: bool = False,
     ) -> aie.FeatureCollection:
-
         if collection is not None and not isinstance(collection, aie.FeatureCollection):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"collection 只支持aie.FeatureCollection类型参数, 传入类型为{type(collection)}",
             )
 
         if scale is not None and not isinstance(scale, (int, float)):
@@ -2356,15 +2241,14 @@
     def samplePoints(
         self,
         collection: aie.FeatureCollection,
         scale: [int, float],
         properties: list = None,
         geometries: bool = False,
     ) -> aie.FeatureCollection:
-
         if collection is not None and not isinstance(collection, aie.FeatureCollection):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"collection 只支持aie.FeatureCollection类型参数, 传入类型为{type(collection)}",
             )
 
         if scale is not None and not isinstance(scale, (int, float)):
@@ -2401,15 +2285,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数scale不能为空")
 
         return FunctionHelper.apply(
             "Image.samplePoints", "aie.FeatureCollection", invoke_args
         )
 
     def cast(self, bandTypes: dict) -> aie.Image:
-
         if bandTypes is not None and not isinstance(bandTypes, dict):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"bandTypes 只支持dict类型参数, 传入类型为{type(bandTypes)}",
             )
 
         invoke_args = {
@@ -2421,15 +2304,14 @@
 
         if "bandTypes" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数bandTypes不能为空")
 
         return FunctionHelper.apply("Image.cast", "aie.Image", invoke_args)
 
     def set(self, var_args: dict) -> aie.Image:
-
         if var_args is not None and not isinstance(var_args, dict):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"var_args 只支持dict类型参数, 传入类型为{type(var_args)}"
             )
 
         invoke_args = {
             "input": self,
```

### Comparing `aie-sdk-2.2.2/aie/aie_object/image_collection.py` & `aie-sdk-2.2.5/aie/aie_object/image_collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,23 +46,43 @@
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"vis_params 只支持dict类型参数, 传入类型为{type(vis_params)}",
             )
         return aie.client.Maps.getMapId(self, vis_params)
 
     def mosaic(self) -> aie.Image:
-
         invoke_args = {
             "collection": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("ImageCollection.mosaic", "aie.Image", invoke_args)
 
+    def qualityMosaic(self, qualityBand: str) -> aie.Image:
+        if qualityBand is not None and not isinstance(qualityBand, str):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR,
+                f"qualityBand 只支持str类型参数, 传入类型为{type(qualityBand)}",
+            )
+
+        invoke_args = {
+            "collection": self,
+            "qualityBand": qualityBand,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        if "qualityBand" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数qualityBand不能为空")
+
+        return FunctionHelper.apply(
+            "ImageCollection.qualityMosaic", "aie.Image", invoke_args
+        )
+
     def getCenter(self) -> tuple:
         bbox = aie.client.InteractiveSession.getBounds(self)
         if bbox is not None and isinstance(bbox, list):
             center = ((bbox[0] + bbox[2]) / 2, (bbox[1] + bbox[3]) / 2)
             return center
         raise AIEError(AIEErrorCode.ARGS_ERROR, f"获取Center失败. bbox: {bbox}")
 
@@ -70,15 +90,14 @@
         bbox = aie.client.InteractiveSession.getBounds(self)
         if bbox is not None and isinstance(bbox, list):
             bounds = [bbox[0], bbox[1], bbox[2], bbox[3]]
             return bounds
         raise AIEError(AIEErrorCode.ARGS_ERROR, f"获取Bounds失败. bbox: {bbox}")
 
     def toList(self, count: int, offset: int = 0) -> object:
-
         if count is not None and not isinstance(count, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"count 只支持int类型参数, 传入类型为{type(count)}"
             )
 
         if offset is not None and not isinstance(offset, int):
             raise AIEError(
@@ -95,27 +114,24 @@
 
         if "count" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数count不能为空")
 
         return FunctionHelper.apply("ImageCollection.toList", "object", invoke_args)
 
     def filter(self, filter: Union[str, aie.Filter]) -> aie.ImageCollection:
-
         node = super(ImageCollection, self).filter(filter)
         return FunctionHelper.cast(node, "aie.ImageCollection")
 
     def filterBounds(
         self, geometry: Union[aie.Geometry, aie.Feature, aie.FeatureCollection]
     ) -> aie.ImageCollection:
-
         node = super(ImageCollection, self).filterBounds(geometry)
         return FunctionHelper.cast(node, "aie.ImageCollection")
 
     def filterDate(self, start: str, end: str) -> aie.ImageCollection:
-
         if start is not None and not isinstance(start, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"start 只支持str类型参数, 传入类型为{type(start)}"
             )
 
         if end is not None and not isinstance(end, str):
             raise AIEError(AIEErrorCode.ARGS_ERROR, f"end 只支持str类型参数, 传入类型为{type(end)}")
@@ -135,27 +151,24 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数end不能为空")
 
         return FunctionHelper.apply(
             "Collection.filterDate", "aie.ImageCollection", invoke_args
         )
 
     def first(self) -> aie.Image:
-
         node = super(ImageCollection, self).first()
         return FunctionHelper.cast(node, "aie.Image")
 
     def limit(
         self, limit: int, property: str = None, ascending: bool = True
     ) -> aie.ImageCollection:
-
         node = super(ImageCollection, self).limit(limit, property=None, ascending=True)
         return FunctionHelper.cast(node, "aie.ImageCollection")
 
     def reduce(self, reducer: aie.Reducer) -> aie.Image:
-
         if reducer is not None and not isinstance(reducer, aie.Reducer):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"reducer 只支持aie.Reducer类型参数, 传入类型为{type(reducer)}",
             )
 
         invoke_args = {
@@ -167,129 +180,117 @@
 
         if "reducer" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数reducer不能为空")
 
         return FunctionHelper.apply("ImageCollection.reduce", "aie.Image", invoke_args)
 
     def And(self) -> aie.Image:
-
         invoke_args = {
             "collection": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("reduce.and", "aie.Image", invoke_args)
 
     def count(self) -> aie.Image:
-
         invoke_args = {
             "collection": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("reduce.count", "aie.Image", invoke_args)
 
     def max(self) -> aie.Image:
-
         invoke_args = {
             "collection": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("reduce.max", "aie.Image", invoke_args)
 
     def mean(self) -> aie.Image:
-
         invoke_args = {
             "collection": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("reduce.mean", "aie.Image", invoke_args)
 
     def median(self) -> aie.Image:
-
         invoke_args = {
             "collection": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("reduce.median", "aie.Image", invoke_args)
 
     def min(self) -> aie.Image:
-
         invoke_args = {
             "collection": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("reduce.min", "aie.Image", invoke_args)
 
     def mode(self) -> aie.Image:
-
         invoke_args = {
             "collection": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("reduce.mode", "aie.Image", invoke_args)
 
     def Or(self) -> aie.Image:
-
         invoke_args = {
             "collection": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("reduce.or", "aie.Image", invoke_args)
 
     def product(self) -> aie.Image:
-
         invoke_args = {
             "collection": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("reduce.product", "aie.Image", invoke_args)
 
     def sum(self) -> aie.Image:
-
         invoke_args = {
             "collection": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("reduce.sum", "aie.Image", invoke_args)
 
     def map(
         self, baseAlgorithm: types.FunctionType
     ) -> Union[aie.ImageCollection, aie.FeatureCollection]:
-
         node = super(ImageCollection, self).map(baseAlgorithm)
         baseAlgorithm_return_type = type(node.invoke_args["baseAlgorithm"].body)
         if aie.Feature == baseAlgorithm_return_type:
             return FunctionHelper.cast(node, "aie.FeatureCollection")
         else:
             return FunctionHelper.cast(node, "aie.ImageCollection")
 
     def select(self, selectors) -> aie.ImageCollection:
         return self.map(lambda image: image.select(selectors))
 
     def sort(self, property: str, ascending: bool = True) -> aie.ImageCollection:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         if ascending is not None and not isinstance(ascending, bool):
             raise AIEError(
@@ -309,26 +310,24 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "ImageCollection.sort", "aie.ImageCollection", invoke_args
         )
 
     def toBands(self) -> aie.Image:
-
         invoke_args = {
             "collection": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("ImageCollection.toBands", "aie.Image", invoke_args)
 
     @staticmethod
     def fromImages(images: list) -> aie.ImageCollection:
-
         if images is not None and not isinstance(images, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"images 只支持list类型参数, 传入类型为{type(images)}"
             )
 
         invoke_args = {
             "images": images,
@@ -340,15 +339,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数images不能为空")
 
         return FunctionHelper.apply(
             "ImageCollection.fromImages", "aie.ImageCollection", invoke_args
         )
 
     def merge(self, collection2: aie.ImageCollection) -> aie.ImageCollection:
-
         if collection2 is not None and not isinstance(collection2, aie.ImageCollection):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"collection2 只支持aie.ImageCollection类型参数, 传入类型为{type(collection2)}",
             )
 
         invoke_args = {
@@ -362,15 +360,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数collection2不能为空")
 
         return FunctionHelper.apply(
             "ImageCollection.merge", "aie.ImageCollection", invoke_args
         )
 
     def cast(self, bandTypes: dict) -> aie.ImageCollection:
-
         if bandTypes is not None and not isinstance(bandTypes, dict):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"bandTypes 只支持dict类型参数, 传入类型为{type(bandTypes)}",
             )
 
         invoke_args = {
@@ -384,15 +381,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数bandTypes不能为空")
 
         return FunctionHelper.apply(
             "ImageCollection.cast", "aie.ImageCollection", invoke_args
         )
 
     def aggregate_max(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -405,15 +401,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "ImageCollection.aggregate_max", "object", invoke_args
         )
 
     def aggregate_min(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -426,15 +421,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "ImageCollection.aggregate_min", "object", invoke_args
         )
 
     def aggregate_mean(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -447,15 +441,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "ImageCollection.aggregate_mean", "object", invoke_args
         )
 
     def aggregate_count(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -468,15 +461,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "ImageCollection.aggregate_count", "object", invoke_args
         )
 
     def aggregate_sum(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -489,15 +481,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "ImageCollection.aggregate_sum", "object", invoke_args
         )
 
     def aggregate_stats(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -510,15 +501,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "ImageCollection.aggregate_stats", "object", invoke_args
         )
 
     def aggregate_array(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -531,15 +521,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "ImageCollection.aggregate_array", "object", invoke_args
         )
 
     def aggregate_product(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -552,15 +541,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "ImageCollection.aggregate_product", "object", invoke_args
         )
 
     def aggregate_sample_sd(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -573,15 +561,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "ImageCollection.aggregate_sample_sd", "object", invoke_args
         )
 
     def aggregate_sample_var(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -594,15 +581,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "ImageCollection.aggregate_sample_var", "object", invoke_args
         )
 
     def aggregate_total_sd(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -615,15 +601,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "ImageCollection.aggregate_total_sd", "object", invoke_args
         )
 
     def aggregate_total_var(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -636,15 +621,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "ImageCollection.aggregate_total_var", "object", invoke_args
         )
 
     def aggregate_histogram(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -657,15 +641,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "ImageCollection.aggregate_histogram", "object", invoke_args
         )
 
     def aggregate_count_distinct(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
@@ -678,15 +661,14 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "ImageCollection.aggregate_count_distinct", "object", invoke_args
         )
 
     def aggregate_first(self, property: str) -> object:
-
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
             "collection": self,
```

### Comparing `aie-sdk-2.2.2/aie/aie_object/kernel.py` & `aie-sdk-2.2.5/aie/aie_object/kernel.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     @staticmethod
     def chebyshev(
         radius: [int, float],
         units: str = "pixels",
         normalize: bool = False,
         magnitude: [int, float] = 1.0,
     ) -> aie.Kernel:
-
         if radius is not None and not isinstance(radius, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"radius 只支持(int,float)类型参数, 传入类型为{type(radius)}",
             )
 
         if units is not None and not isinstance(units, str):
@@ -64,15 +63,14 @@
     @staticmethod
     def circle(
         radius: [int, float],
         units: str = "pixels",
         normalize: bool = False,
         magnitude: [int, float] = 1.0,
     ) -> aie.Kernel:
-
         if radius is not None and not isinstance(radius, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"radius 只支持(int,float)类型参数, 传入类型为{type(radius)}",
             )
 
         if units is not None and not isinstance(units, str):
@@ -104,15 +102,14 @@
         if "radius" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数radius不能为空")
 
         return FunctionHelper.apply("Kernel.circle", "aie.Kernel", invoke_args)
 
     @staticmethod
     def compass(normalize: bool = False, magnitude: [int, float] = 1.0) -> aie.Kernel:
-
         if normalize is not None and not isinstance(normalize, bool):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"normalize 只支持bool类型参数, 传入类型为{type(normalize)}",
             )
 
         if magnitude is not None and not isinstance(magnitude, (int, float)):
@@ -133,15 +130,14 @@
     @staticmethod
     def cross(
         radius: [int, float],
         units: str = "pixels",
         normalize: bool = False,
         magnitude: [int, float] = 1.0,
     ) -> aie.Kernel:
-
         if radius is not None and not isinstance(radius, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"radius 只支持(int,float)类型参数, 传入类型为{type(radius)}",
             )
 
         if units is not None and not isinstance(units, str):
@@ -178,15 +174,14 @@
     @staticmethod
     def diamond(
         radius: [int, float],
         units: str = "pixels",
         normalize: bool = False,
         magnitude: [int, float] = 1.0,
     ) -> aie.Kernel:
-
         if radius is not None and not isinstance(radius, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"radius 只支持(int,float)类型参数, 传入类型为{type(radius)}",
             )
 
         if units is not None and not isinstance(units, str):
@@ -223,15 +218,14 @@
     @staticmethod
     def euclidean(
         radius: [int, float],
         units: str = "pixels",
         normalize: bool = False,
         magnitude: [int, float] = 1.0,
     ) -> aie.Kernel:
-
         if radius is not None and not isinstance(radius, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"radius 只支持(int,float)类型参数, 传入类型为{type(radius)}",
             )
 
         if units is not None and not isinstance(units, str):
@@ -263,15 +257,14 @@
         if "radius" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数radius不能为空")
 
         return FunctionHelper.apply("Kernel.euclidean", "aie.Kernel", invoke_args)
 
     @staticmethod
     def fixed(weights: list, normalize: bool = False) -> aie.Kernel:
-
         if weights is not None and not isinstance(weights, list):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"weights 只支持list类型参数, 传入类型为{type(weights)}"
             )
 
         if normalize is not None and not isinstance(normalize, bool):
             raise AIEError(
@@ -295,15 +288,14 @@
     def gaussian(
         radius: [int, float],
         sigma: [int, float] = 1.0,
         units: str = "pixels",
         normalize: bool = False,
         magnitude: [int, float] = 1.0,
     ) -> aie.Kernel:
-
         if radius is not None and not isinstance(radius, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"radius 只支持(int,float)类型参数, 传入类型为{type(radius)}",
             )
 
         if sigma is not None and not isinstance(sigma, (int, float)):
@@ -341,15 +333,14 @@
         if "radius" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数radius不能为空")
 
         return FunctionHelper.apply("Kernel.gaussian", "aie.Kernel", invoke_args)
 
     @staticmethod
     def kirsch(normalize: bool = False, magnitude: [int, float] = 1.0) -> aie.Kernel:
-
         if normalize is not None and not isinstance(normalize, bool):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"normalize 只支持bool类型参数, 传入类型为{type(normalize)}",
             )
 
         if magnitude is not None and not isinstance(magnitude, (int, float)):
@@ -367,15 +358,14 @@
 
         return FunctionHelper.apply("Kernel.kirsch", "aie.Kernel", invoke_args)
 
     @staticmethod
     def laplacian4(
         normalize: bool = False, magnitude: [int, float] = 1.0
     ) -> aie.Kernel:
-
         if normalize is not None and not isinstance(normalize, bool):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"normalize 只支持bool类型参数, 传入类型为{type(normalize)}",
             )
 
         if magnitude is not None and not isinstance(magnitude, (int, float)):
@@ -393,15 +383,14 @@
 
         return FunctionHelper.apply("Kernel.laplacian4", "aie.Kernel", invoke_args)
 
     @staticmethod
     def laplacian8(
         normalize: bool = False, magnitude: [int, float] = 1.0
     ) -> aie.Kernel:
-
         if normalize is not None and not isinstance(normalize, bool):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"normalize 只支持bool类型参数, 传入类型为{type(normalize)}",
             )
 
         if magnitude is not None and not isinstance(magnitude, (int, float)):
@@ -422,15 +411,14 @@
     @staticmethod
     def manhattan(
         radius: [int, float],
         units: str = "pixels",
         normalize: bool = False,
         magnitude: [int, float] = 1.0,
     ) -> aie.Kernel:
-
         if radius is not None and not isinstance(radius, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"radius 只支持(int,float)类型参数, 传入类型为{type(radius)}",
             )
 
         if units is not None and not isinstance(units, str):
@@ -467,15 +455,14 @@
     @staticmethod
     def plus(
         radius: [int, float],
         units: str = "pixels",
         normalize: bool = False,
         magnitude: [int, float] = 1.0,
     ) -> aie.Kernel:
-
         if radius is not None and not isinstance(radius, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"radius 只支持(int,float)类型参数, 传入类型为{type(radius)}",
             )
 
         if units is not None and not isinstance(units, str):
@@ -507,15 +494,14 @@
         if "radius" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数radius不能为空")
 
         return FunctionHelper.apply("Kernel.plus", "aie.Kernel", invoke_args)
 
     @staticmethod
     def prewitt(normalize: bool = False, magnitude: [int, float] = 1.0) -> aie.Kernel:
-
         if normalize is not None and not isinstance(normalize, bool):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"normalize 只支持bool类型参数, 传入类型为{type(normalize)}",
             )
 
         if magnitude is not None and not isinstance(magnitude, (int, float)):
@@ -537,15 +523,14 @@
     def rectangle(
         xRadius: [int, float],
         yRadius: [int, float],
         units: str = "pixels",
         normalize: bool = False,
         magnitude: [int, float] = 1.0,
     ) -> aie.Kernel:
-
         if xRadius is not None and not isinstance(xRadius, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"xRadius 只支持(int,float)类型参数, 传入类型为{type(xRadius)}",
             )
 
         if yRadius is not None and not isinstance(yRadius, (int, float)):
@@ -587,15 +572,14 @@
         if "yRadius" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数yRadius不能为空")
 
         return FunctionHelper.apply("Kernel.rectangle", "aie.Kernel", invoke_args)
 
     @staticmethod
     def roberts(normalize: bool = False, magnitude: [int, float] = 1.0) -> aie.Kernel:
-
         if normalize is not None and not isinstance(normalize, bool):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"normalize 只支持bool类型参数, 传入类型为{type(normalize)}",
             )
 
         if magnitude is not None and not isinstance(magnitude, (int, float)):
@@ -611,15 +595,14 @@
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Kernel.roberts", "aie.Kernel", invoke_args)
 
     @staticmethod
     def sobel(normalize: bool = False, magnitude: [int, float] = 1.0) -> aie.Kernel:
-
         if normalize is not None and not isinstance(normalize, bool):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"normalize 只支持bool类型参数, 传入类型为{type(normalize)}",
             )
 
         if magnitude is not None and not isinstance(magnitude, (int, float)):
@@ -640,15 +623,14 @@
     @staticmethod
     def square(
         radius: [int, float],
         units: str = "pixels",
         normalize: bool = False,
         magnitude: [int, float] = 1.0,
     ) -> aie.Kernel:
-
         if radius is not None and not isinstance(radius, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"radius 只支持(int,float)类型参数, 传入类型为{type(radius)}",
             )
 
         if units is not None and not isinstance(units, str):
@@ -679,15 +661,14 @@
 
         if "radius" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数radius不能为空")
 
         return FunctionHelper.apply("Kernel.square", "aie.Kernel", invoke_args)
 
     def add(self, kernel2: aie.Kernel, normalize: bool = False) -> aie.Kernel:
-
         if kernel2 is not None and not isinstance(kernel2, aie.Kernel):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"kernel2 只支持aie.Kernel类型参数, 传入类型为{type(kernel2)}",
             )
 
         if normalize is not None and not isinstance(normalize, bool):
@@ -706,15 +687,14 @@
 
         if "kernel2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数kernel2不能为空")
 
         return FunctionHelper.apply("Kernel.add", "aie.Kernel", invoke_args)
 
     def subtract(self, kernel2: aie.Kernel, normalize: bool = False) -> aie.Kernel:
-
         if kernel2 is not None and not isinstance(kernel2, aie.Kernel):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"kernel2 只支持aie.Kernel类型参数, 传入类型为{type(kernel2)}",
             )
 
         if normalize is not None and not isinstance(normalize, bool):
@@ -733,15 +713,14 @@
 
         if "kernel2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数kernel2不能为空")
 
         return FunctionHelper.apply("Kernel.subtract", "aie.Kernel", invoke_args)
 
     def multiply(self, kernel2: aie.Kernel, normalize: bool = False) -> aie.Kernel:
-
         if kernel2 is not None and not isinstance(kernel2, aie.Kernel):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"kernel2 只支持aie.Kernel类型参数, 传入类型为{type(kernel2)}",
             )
 
         if normalize is not None and not isinstance(normalize, bool):
@@ -760,15 +739,14 @@
 
         if "kernel2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数kernel2不能为空")
 
         return FunctionHelper.apply("Kernel.multiply", "aie.Kernel", invoke_args)
 
     def divide(self, kernel2: aie.Kernel, normalize: bool = False) -> aie.Kernel:
-
         if kernel2 is not None and not isinstance(kernel2, aie.Kernel):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"kernel2 只支持aie.Kernel类型参数, 传入类型为{type(kernel2)}",
             )
 
         if normalize is not None and not isinstance(normalize, bool):
@@ -787,25 +765,23 @@
 
         if "kernel2" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数kernel2不能为空")
 
         return FunctionHelper.apply("Kernel.divide", "aie.Kernel", invoke_args)
 
     def inverse(self) -> aie.Kernel:
-
         invoke_args = {
             "kernel": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Kernel.inverse", "aie.Kernel", invoke_args)
 
     def rotate(self, rotations: int) -> aie.Kernel:
-
         if rotations is not None and not isinstance(rotations, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"rotations 只支持int类型参数, 传入类型为{type(rotations)}"
             )
 
         invoke_args = {
             "kernel": self,
```

### Comparing `aie-sdk-2.2.2/aie/aie_object/model.py` & `aie-sdk-2.2.5/aie/aie_object/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 class Model(FunctionNode):
     def __init__(self, modelName) -> aie.Model:
         self.modelName = modelName
         super(Model, self).__init__("Model.load", {"modelName": modelName})
 
     def predict(self, src: aie.Image, dst: aie.Image = None) -> aie.Image:
-
         if src is not None and not isinstance(src, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"src 只支持aie.Image类型参数, 传入类型为{type(src)}"
             )
 
         if dst is not None and not isinstance(dst, aie.Image):
             raise AIEError(
```

### Comparing `aie-sdk-2.2.2/aie/aie_object/reducer.py` & `aie-sdk-2.2.5/aie/aie_object/reducer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from aie.error.aie_error import AIEError, AIEErrorCode
 
 
 class Reducer(FunctionNode):
     def combine(
         self, reducer2: aie.Reducer, outputPrefix: str = "", sharedInputs: bool = False
     ) -> aie.Reducer:
-
         if reducer2 is not None and not isinstance(reducer2, aie.Reducer):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"reducer2 只支持aie.Reducer类型参数, 传入类型为{type(reducer2)}",
             )
 
         if outputPrefix is not None and not isinstance(outputPrefix, str):
@@ -52,15 +51,14 @@
 
         return FunctionHelper.apply("Reducer.combine", "aie.Reducer", invoke_args)
 
     @staticmethod
     def histogram(
         maxBuckets: int = None, minBucketWidth: [int, float] = None, maxRaw: int = None
     ) -> aie.Reducer:
-
         if maxBuckets is not None and not isinstance(maxBuckets, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"maxBuckets 只支持int类型参数, 传入类型为{type(maxBuckets)}",
             )
 
         if minBucketWidth is not None and not isinstance(minBucketWidth, (int, float)):
@@ -82,24 +80,22 @@
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Reducer.histogram", "aie.Reducer", invoke_args)
 
     @staticmethod
     def count() -> aie.Reducer:
-
         invoke_args = {}
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Reducer.count", "aie.Reducer", invoke_args)
 
     @staticmethod
     def max(numInputs: int = 1) -> aie.Reducer:
-
         if numInputs is not None and not isinstance(numInputs, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"numInputs 只支持int类型参数, 传入类型为{type(numInputs)}"
             )
 
         invoke_args = {
             "numInputs": numInputs,
@@ -107,26 +103,24 @@
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Reducer.max", "aie.Reducer", invoke_args)
 
     @staticmethod
     def mean() -> aie.Reducer:
-
         invoke_args = {}
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Reducer.mean", "aie.Reducer", invoke_args)
 
     @staticmethod
     def median(
         maxBuckets: int = None, minBucketWidth: [int, float] = None, maxRaw: int = None
     ) -> aie.Reducer:
-
         if maxBuckets is not None and not isinstance(maxBuckets, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"maxBuckets 只支持int类型参数, 传入类型为{type(maxBuckets)}",
             )
 
         if minBucketWidth is not None and not isinstance(minBucketWidth, (int, float)):
@@ -148,15 +142,14 @@
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Reducer.median", "aie.Reducer", invoke_args)
 
     @staticmethod
     def min(numInputs: int = 1) -> aie.Reducer:
-
         if numInputs is not None and not isinstance(numInputs, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"numInputs 只支持int类型参数, 传入类型为{type(numInputs)}"
             )
 
         invoke_args = {
             "numInputs": numInputs,
@@ -164,26 +157,24 @@
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Reducer.min", "aie.Reducer", invoke_args)
 
     @staticmethod
     def minMax() -> aie.Reducer:
-
         invoke_args = {}
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Reducer.minMax", "aie.Reducer", invoke_args)
 
     @staticmethod
     def mode(
         maxBuckets: int = None, minBucketWidth: [int, float] = None, maxRaw: int = None
     ) -> aie.Reducer:
-
         if maxBuckets is not None and not isinstance(maxBuckets, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"maxBuckets 只支持int类型参数, 传入类型为{type(maxBuckets)}",
             )
 
         if minBucketWidth is not None and not isinstance(minBucketWidth, (int, float)):
@@ -205,107 +196,96 @@
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Reducer.mode", "aie.Reducer", invoke_args)
 
     @staticmethod
     def product() -> aie.Reducer:
-
         invoke_args = {}
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Reducer.product", "aie.Reducer", invoke_args)
 
     @staticmethod
     def stdDev() -> aie.Reducer:
-
         invoke_args = {}
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Reducer.stdDev", "aie.Reducer", invoke_args)
 
     @staticmethod
     def sum() -> aie.Reducer:
-
         invoke_args = {}
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Reducer.sum", "aie.Reducer", invoke_args)
 
     @staticmethod
     def variance() -> aie.Reducer:
-
         invoke_args = {}
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Reducer.variance", "aie.Reducer", invoke_args)
 
     @staticmethod
     def allNonZero() -> aie.Reducer:
-
         invoke_args = {}
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Reducer.allNonZero", "aie.Reducer", invoke_args)
 
     @staticmethod
     def anyNonZero() -> aie.Reducer:
-
         invoke_args = {}
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Reducer.anyNonZero", "aie.Reducer", invoke_args)
 
     @staticmethod
     def bitwiseAnd() -> aie.Reducer:
-
         invoke_args = {}
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Reducer.bitwiseAnd", "aie.Reducer", invoke_args)
 
     @staticmethod
     def bitwiseOr() -> aie.Reducer:
-
         invoke_args = {}
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Reducer.bitwiseOr", "aie.Reducer", invoke_args)
 
     @staticmethod
     def sampleStdDev() -> aie.Reducer:
-
         invoke_args = {}
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Reducer.sampleStdDev", "aie.Reducer", invoke_args)
 
     @staticmethod
     def sampleVariance() -> aie.Reducer:
-
         invoke_args = {}
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply(
             "Reducer.sampleVariance", "aie.Reducer", invoke_args
         )
 
     @staticmethod
     def histogram(buckets: int) -> aie.Reducer:
-
         if buckets is not None and not isinstance(buckets, int):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"buckets 只支持int类型参数, 传入类型为{type(buckets)}"
             )
 
         invoke_args = {
             "buckets": buckets,
@@ -318,15 +298,14 @@
 
         return FunctionHelper.apply("Reducer.histogram", "aie.Reducer", invoke_args)
 
     @staticmethod
     def fixedHistogram(
         min: [int, float], max: [int, float], buckets: int
     ) -> aie.Reducer:
-
         if min is not None and not isinstance(min, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"min 只支持(int,float)类型参数, 传入类型为{type(min)}"
             )
 
         if max is not None and not isinstance(max, (int, float)):
             raise AIEError(
@@ -357,57 +336,52 @@
 
         return FunctionHelper.apply(
             "Reducer.fixedHistogram", "aie.Reducer", invoke_args
         )
 
     @staticmethod
     def linearFit() -> aie.Reducer:
-
         invoke_args = {}
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Reducer.linearFit", "aie.Reducer", invoke_args)
 
     @staticmethod
     def linearRegression() -> aie.Reducer:
-
         invoke_args = {}
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply(
             "Reducer.linearRegression", "aie.Reducer", invoke_args
         )
 
     @staticmethod
     def pearsonsCorrelation() -> aie.Reducer:
-
         invoke_args = {}
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply(
             "Reducer.pearsonsCorrelation", "aie.Reducer", invoke_args
         )
 
     @staticmethod
     def spearmansCorrelation() -> aie.Reducer:
-
         invoke_args = {}
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply(
             "Reducer.spearmansCorrelation", "aie.Reducer", invoke_args
         )
 
     @staticmethod
     def ridgeRegression(regParam: [int, float] = 0.1) -> aie.Reducer:
-
         if regParam is not None and not isinstance(regParam, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"regParam 只支持(int,float)类型参数, 传入类型为{type(regParam)}",
             )
 
         invoke_args = {
@@ -418,15 +392,14 @@
 
         return FunctionHelper.apply(
             "Reducer.ridgeRegression", "aie.Reducer", invoke_args
         )
 
     @staticmethod
     def lassoRegression(regParam: [int, float] = 0.1) -> aie.Reducer:
-
         if regParam is not None and not isinstance(regParam, (int, float)):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"regParam 只支持(int,float)类型参数, 传入类型为{type(regParam)}",
             )
 
         invoke_args = {
```

### Comparing `aie-sdk-2.2.2/aie/aie_object/terrain.py` & `aie-sdk-2.2.5/aie/aie_object/terrain.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from aie.function_helper import FunctionHelper
 from aie.error.aie_error import AIEError, AIEErrorCode
 
 
 class Terrain(FunctionNode):
     @staticmethod
     def aspect(input: aie.Image) -> aie.Image:
-
         if input is not None and not isinstance(input, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"input 只支持aie.Image类型参数, 传入类型为{type(input)}"
             )
 
         invoke_args = {
             "input": input,
@@ -33,15 +32,14 @@
         if "input" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数input不能为空")
 
         return FunctionHelper.apply("Terrain.aspect", "aie.Image", invoke_args)
 
     @staticmethod
     def slope(input: aie.Image) -> aie.Image:
-
         if input is not None and not isinstance(input, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"input 只支持aie.Image类型参数, 传入类型为{type(input)}"
             )
 
         invoke_args = {
             "input": input,
@@ -54,15 +52,14 @@
 
         return FunctionHelper.apply("Terrain.slope", "aie.Image", invoke_args)
 
     @staticmethod
     def hillshade(
         input: aie.Image, azimuth: [int, float] = 270, elevation: [int, float] = 45
     ) -> aie.Image:
-
         if input is not None and not isinstance(input, aie.Image):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"input 只支持aie.Image类型参数, 传入类型为{type(input)}"
             )
 
         if azimuth is not None and not isinstance(azimuth, (int, float)):
             raise AIEError(
```

### Comparing `aie-sdk-2.2.2/aie/auth.py` & `aie-sdk-2.2.5/aie/auth.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/client/client.py` & `aie-sdk-2.2.5/aie/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import json
+import os
+
 import requests
 from aie.error import AIEError, AIEErrorCode
 import aie.g_var as g_var
 import aie
 
 import urllib3
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 class BaseClient(object):
     @staticmethod
     def __append_extra_hdrs(hdrs):
         hdrs["x-aie-auth-token"] = aie.auth.Authenticate.getCurrentUserToken()
+
+        project_id = os.getenv(g_var.JupyterEnv.PROJECT_ID, "local")
+        hdrs['x-aie-client-name'] = f"aie-sdk@Project-{project_id}"
         return hdrs
 
     @staticmethod
     def post(url, hdrs, data, append_extra_hdrs=True):
         if append_extra_hdrs:
             hdrs = BaseClient.__append_extra_hdrs(hdrs)
```

### Comparing `aie-sdk-2.2.2/aie/client/constants.py` & `aie-sdk-2.2.5/aie/client/constants.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/client/dataset.py` & `aie-sdk-2.2.5/aie/client/dataset.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/client/endpoints.py` & `aie-sdk-2.2.5/aie/client/endpoints.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/client/interactive_session.py` & `aie-sdk-2.2.5/aie/client/interactive_session.py`

 * *Files 10% similar despite different names*

```diff
@@ -112,14 +112,20 @@
         }
 
         url = Endpoints.INTERACTIVE_SESSION + InteractiveSessionResource.CANCEL_ALL
         InteractiveSessionClient.post(url, data, True)
 
     @staticmethod
     def getInfo(obj):
+        if isinstance(obj, (aie.Image, aie.Feature)) \
+                and obj.func_name is None \
+                and obj.invoke_args is None \
+                and '_MAPPING_VAR' in obj.var_name:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "请勿在map函数中使用getInfo方法",
+                           "请尝试使用for循环逐个获取，https://engine-aiearth.aliyun.com/docs/page/api?d=9e276c")
         expr = aie.serialize.serializer.encode(obj)
         options = {
             "taskType": "getInfo"
         }
         task_id = newUUID()
         data = {
             "taskId": task_id,
@@ -142,14 +148,20 @@
                 extrainfo["taskId"] = data["taskId"]
             raise AIEError(payload["output"]["error_code"],
                            payload["output"]["error_message"], json.dumps(extrainfo))
         return payload["output"]["data"]["application/json"]
 
     @staticmethod
     def getBounds(obj):
+        if isinstance(obj, (aie.Image, aie.Feature)) \
+                and obj.func_name is None \
+                and obj.invoke_args is None \
+                and '_MAPPING_VAR' in obj.var_name:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "请勿在map函数中使用getBounds方法",
+                           "请尝试使用for循环逐个获取，https://engine-aiearth.aliyun.com/docs/page/api?d=9e276c")
         expr = aie.serialize.serializer.encode(obj)
         options = {
             "taskType": "getBounds"
         }
         task_id = newUUID()
         data = {
             "taskId": task_id,
```

### Comparing `aie-sdk-2.2.2/aie/client/maps.py` & `aie-sdk-2.2.5/aie/client/maps.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/client/mlproxy.py` & `aie-sdk-2.2.5/aie/client/mlproxy.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/client/mlproxy_back.py` & `aie-sdk-2.2.5/aie/client/mlproxy_back.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/client/task.py` & `aie-sdk-2.2.5/aie/client/task.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/error/aie_error.py` & `aie-sdk-2.2.5/aie/error/aie_error.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/export.py` & `aie-sdk-2.2.5/aie/export.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/function_helper.py` & `aie-sdk-2.2.5/aie/function_helper.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/g_var.py` & `aie-sdk-2.2.5/aie/g_var.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/gen_python_functions.py` & `aie-sdk-2.2.5/aie/gen_python_functions.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/map/aie_color.py` & `aie-sdk-2.2.5/aie/map/aie_color.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/map/aie_layer.py` & `aie-sdk-2.2.5/aie/map/aie_layer.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/map/aie_map.py` & `aie-sdk-2.2.5/aie/map/aie_map.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/map/color.csv` & `aie-sdk-2.2.5/aie/map/color.csv`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/serialize/gen_visitor.py` & `aie-sdk-2.2.5/aie/serialize/gen_visitor.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/serialize/optimizer.py` & `aie-sdk-2.2.5/aie/serialize/optimizer.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie/serialize/serializer_impl.py` & `aie-sdk-2.2.5/aie/serialize/serializer_impl.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/aie_sdk.egg-info/SOURCES.txt` & `aie-sdk-2.2.5/aie_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.2/setup.py` & `aie-sdk-2.2.5/setup.py`

 * *Files identical despite different names*

