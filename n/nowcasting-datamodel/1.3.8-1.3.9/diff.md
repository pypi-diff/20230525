# Comparing `tmp/nowcasting_datamodel-1.3.8.tar.gz` & `tmp/nowcasting_datamodel-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcasting_datamodel-1.3.8.tar", last modified: Thu May  4 11:40:08 2023, max compression
+gzip compressed data, was "nowcasting_datamodel-1.3.9.tar", last modified: Thu May  4 11:42:00 2023, max compression
```

## Comparing `nowcasting_datamodel-1.3.8.tar` & `nowcasting_datamodel-1.3.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:40:08.479687 nowcasting_datamodel-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-04 11:40:08.479687 nowcasting_datamodel-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/diagram_pv.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:40:08.471686 nowcasting_datamodel-1.3.8/nowcasting_datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/fake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:40:08.475686 nowcasting_datamodel-1.3.8/nowcasting_datamodel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/migrations/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:40:08.475686 nowcasting_datamodel-1.3.8/nowcasting_datamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/models/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/models/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/models/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/models/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/national.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:40:08.475686 nowcasting_datamodel-1.3.8/nowcasting_datamodel/read/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/read/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:40:08.475686 nowcasting_datamodel-1.3.8/nowcasting_datamodel/read/blend/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/read/blend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/read/blend/blend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/read/blend/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/read/blend/weights.py
--rw-r--r--   0 runner    (1001) docker     (123)    22872 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/read/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/read/read_gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/read/read_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/read/read_pv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:40:08.475686 nowcasting_datamodel-1.3.8/nowcasting_datamodel/save/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/save/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/save/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/save/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/save/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:40:08.475686 nowcasting_datamodel-1.3.8/nowcasting_datamodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-04 11:40:08.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-04 11:40:08.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:40:08.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-04 11:40:08.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 11:40:08.000000 nowcasting_datamodel-1.3.8/nowcasting_datamodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:40:08.479687 nowcasting_datamodel-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:40:08.479687 nowcasting_datamodel-1.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/tests/test_databaseconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/tests/test_fake_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/tests/test_national.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-04 11:39:55.000000 nowcasting_datamodel-1.3.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:42:00.215097 nowcasting_datamodel-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-04 11:42:00.215097 nowcasting_datamodel-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/diagram_pv.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:42:00.207097 nowcasting_datamodel-1.3.9/nowcasting_datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/fake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:42:00.211097 nowcasting_datamodel-1.3.9/nowcasting_datamodel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/migrations/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:42:00.211097 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/national.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:42:00.211097 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:42:00.211097 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/blend/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/blend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/blend/blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/blend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/blend/weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22872 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/read_gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/read_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/read_pv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:42:00.215097 nowcasting_datamodel-1.3.9/nowcasting_datamodel/save/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/save/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/save/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/save/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9578 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/save/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:42:00.211097 nowcasting_datamodel-1.3.9/nowcasting_datamodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-04 11:42:00.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-04 11:42:00.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:42:00.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-04 11:42:00.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 11:42:00.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:42:00.215097 nowcasting_datamodel-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:42:00.215097 nowcasting_datamodel-1.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/tests/test_databaseconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/tests/test_fake_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/tests/test_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/tests/test_utils.py
```

### Comparing `nowcasting_datamodel-1.3.8/PKG-INFO` & `nowcasting_datamodel-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting_datamodel
-Version: 1.3.8
+Version: 1.3.9
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.3.8/README.md` & `nowcasting_datamodel-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/diagram.png` & `nowcasting_datamodel-1.3.9/diagram.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/diagram_pv.png` & `nowcasting_datamodel-1.3.9/diagram_pv.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/connection.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/connection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/fake.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/migrations/app.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/migrations/app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/models/__init__.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/models/convert.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/convert.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/models/forecast.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/forecast.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/models/gsp.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/models/metric.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/models/models.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/models.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/models/pv.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/models/utils.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/national.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/read/blend/blend.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/blend/blend.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/read/blend/utils.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/blend/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/read/blend/weights.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/blend/weights.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/read/read.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/read.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/read/read_gsp.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/read_gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/read/read_metric.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/read_metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/read/read_pv.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/read_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/save/adjust.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/save/adjust.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/save/save.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/save/save.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/save/update.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/save/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     update_dict = {c.name: c for c in stmt.excluded if not c.primary_key}
 
     if not update_dict:
         raise ValueError("insert_or_update resulted in an empty update_dict")
 
     stmt = stmt.on_conflict_do_update(index_elements=primary_keys, set_=update_dict)
     session.execute(stmt, rows)
+    session.commit()
 
 
 def update_forecast_latest(
     forecast: ForecastSQL,
     session: Session,
     forecast_historic: Optional[ForecastSQL] = None,
     model_name: Optional[str] = None,
```

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel/utils.py` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel.egg-info/PKG-INFO` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting-datamodel
-Version: 1.3.8
+Version: 1.3.9
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.3.8/nowcasting_datamodel.egg-info/SOURCES.txt` & `nowcasting_datamodel-1.3.9/nowcasting_datamodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/setup.py` & `nowcasting_datamodel-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/tests/test_databaseconnection.py` & `nowcasting_datamodel-1.3.9/tests/test_databaseconnection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/tests/test_fake.py` & `nowcasting_datamodel-1.3.9/tests/test_fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/tests/test_fake_pv.py` & `nowcasting_datamodel-1.3.9/tests/test_fake_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/tests/test_national.py` & `nowcasting_datamodel-1.3.9/tests/test_national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.8/tests/test_utils.py` & `nowcasting_datamodel-1.3.9/tests/test_utils.py`

 * *Files identical despite different names*

