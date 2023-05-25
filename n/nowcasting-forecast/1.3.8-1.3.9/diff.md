# Comparing `tmp/nowcasting_forecast-1.3.8.tar.gz` & `tmp/nowcasting_forecast-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcasting_forecast-1.3.8.tar", last modified: Thu May  4 17:10:35 2023, max compression
+gzip compressed data, was "nowcasting_forecast-1.3.9.tar", last modified: Thu May  4 17:43:10 2023, max compression
```

## Comparing `nowcasting_forecast-1.3.8.tar` & `nowcasting_forecast-1.3.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:35.520061 nowcasting_forecast-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-04 17:10:35.520061 nowcasting_forecast-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:35.516060 nowcasting_forecast-1.3.8/nowcasting_forecast/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/dataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:35.520061 nowcasting_forecast-1.3.8/nowcasting_forecast/models/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/models/nwp_solar_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/models/sun.py
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:35.520061 nowcasting_forecast-1.3.8/nowcasting_forecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-04 17:10:35.000000 nowcasting_forecast-1.3.8/nowcasting_forecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-04 17:10:35.000000 nowcasting_forecast-1.3.8/nowcasting_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:10:35.000000 nowcasting_forecast-1.3.8/nowcasting_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-04 17:10:35.000000 nowcasting_forecast-1.3.8/nowcasting_forecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-04 17:10:35.000000 nowcasting_forecast-1.3.8/nowcasting_forecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 17:10:35.520061 nowcasting_forecast-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:35.520061 nowcasting_forecast-1.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/tests/test_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:43:10.381361 nowcasting_forecast-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-04 17:42:59.000000 nowcasting_forecast-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-04 17:42:59.000000 nowcasting_forecast-1.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-04 17:43:10.381361 nowcasting_forecast-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-04 17:42:59.000000 nowcasting_forecast-1.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:43:10.377361 nowcasting_forecast-1.3.9/nowcasting_forecast/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 17:42:59.000000 nowcasting_forecast-1.3.9/nowcasting_forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-04 17:42:59.000000 nowcasting_forecast-1.3.9/nowcasting_forecast/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-04 17:42:59.000000 nowcasting_forecast-1.3.9/nowcasting_forecast/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-04 17:42:59.000000 nowcasting_forecast-1.3.9/nowcasting_forecast/dataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:43:10.381361 nowcasting_forecast-1.3.9/nowcasting_forecast/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 17:42:59.000000 nowcasting_forecast-1.3.9/nowcasting_forecast/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-05-04 17:42:59.000000 nowcasting_forecast-1.3.9/nowcasting_forecast/models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-04 17:42:59.000000 nowcasting_forecast-1.3.9/nowcasting_forecast/models/nwp_solar_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-04 17:42:59.000000 nowcasting_forecast-1.3.9/nowcasting_forecast/models/sun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-05-04 17:42:59.000000 nowcasting_forecast-1.3.9/nowcasting_forecast/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-04 17:42:59.000000 nowcasting_forecast-1.3.9/nowcasting_forecast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:43:10.381361 nowcasting_forecast-1.3.9/nowcasting_forecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-04 17:43:10.000000 nowcasting_forecast-1.3.9/nowcasting_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-04 17:43:10.000000 nowcasting_forecast-1.3.9/nowcasting_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:43:10.000000 nowcasting_forecast-1.3.9/nowcasting_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-04 17:43:10.000000 nowcasting_forecast-1.3.9/nowcasting_forecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-04 17:43:10.000000 nowcasting_forecast-1.3.9/nowcasting_forecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-04 17:42:59.000000 nowcasting_forecast-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 17:43:10.381361 nowcasting_forecast-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-04 17:42:59.000000 nowcasting_forecast-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:43:10.381361 nowcasting_forecast-1.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-04 17:42:59.000000 nowcasting_forecast-1.3.9/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-04 17:42:59.000000 nowcasting_forecast-1.3.9/tests/test_batch.py
```

### Comparing `nowcasting_forecast-1.3.8/LICENSE` & `nowcasting_forecast-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.8/PKG-INFO` & `nowcasting_forecast-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting_forecast
-Version: 1.3.8
+Version: 1.3.9
 Summary: Live forecast for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_forecast
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: artificial intelligence,forecast
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_forecast-1.3.8/README.md` & `nowcasting_forecast-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.8/nowcasting_forecast/app.py` & `nowcasting_forecast-1.3.9/nowcasting_forecast/app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.8/nowcasting_forecast/batch.py` & `nowcasting_forecast-1.3.9/nowcasting_forecast/batch.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.8/nowcasting_forecast/dataloader.py` & `nowcasting_forecast-1.3.9/nowcasting_forecast/dataloader.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.8/nowcasting_forecast/models/hub.py` & `nowcasting_forecast-1.3.9/nowcasting_forecast/models/hub.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.8/nowcasting_forecast/models/nwp_solar_simple.py` & `nowcasting_forecast-1.3.9/nowcasting_forecast/models/nwp_solar_simple.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.8/nowcasting_forecast/models/sun.py` & `nowcasting_forecast-1.3.9/nowcasting_forecast/models/sun.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.8/nowcasting_forecast/models/utils.py` & `nowcasting_forecast-1.3.9/nowcasting_forecast/models/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.8/nowcasting_forecast/utils.py` & `nowcasting_forecast-1.3.9/nowcasting_forecast/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.8/nowcasting_forecast.egg-info/PKG-INFO` & `nowcasting_forecast-1.3.9/nowcasting_forecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting-forecast
-Version: 1.3.8
+Version: 1.3.9
 Summary: Live forecast for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_forecast
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: artificial intelligence,forecast
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_forecast-1.3.8/nowcasting_forecast.egg-info/SOURCES.txt` & `nowcasting_forecast-1.3.9/nowcasting_forecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.8/setup.py` & `nowcasting_forecast-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.8/tests/test_app.py` & `nowcasting_forecast-1.3.9/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.8/tests/test_batch.py` & `nowcasting_forecast-1.3.9/tests/test_batch.py`

 * *Files identical despite different names*

