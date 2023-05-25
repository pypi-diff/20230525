# Comparing `tmp/metoffice-weather-datahub-1.2.0.tar.gz` & `tmp/metoffice-weather-datahub-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metoffice-weather-datahub-1.2.0.tar", last modified: Tue Mar 21 10:54:54 2023, max compression
+gzip compressed data, was "metoffice-weather-datahub-1.2.1.tar", last modified: Thu May 25 11:08:01 2023, max compression
```

## Comparing `metoffice-weather-datahub-1.2.0.tar` & `metoffice-weather-datahub-1.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:54:54.249278 metoffice-weather-datahub-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-21 10:54:39.000000 metoffice-weather-datahub-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-21 10:54:39.000000 metoffice-weather-datahub-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-03-21 10:54:54.249278 metoffice-weather-datahub-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-03-21 10:54:39.000000 metoffice-weather-datahub-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:54:54.245278 metoffice-weather-datahub-1.2.0/metoffice_weather_datahub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-03-21 10:54:54.000000 metoffice-weather-datahub-1.2.0/metoffice_weather_datahub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-21 10:54:54.000000 metoffice-weather-datahub-1.2.0/metoffice_weather_datahub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 10:54:54.000000 metoffice-weather-datahub-1.2.0/metoffice_weather_datahub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-21 10:54:54.000000 metoffice-weather-datahub-1.2.0/metoffice_weather_datahub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-21 10:54:54.000000 metoffice-weather-datahub-1.2.0/metoffice_weather_datahub.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:54:54.245278 metoffice-weather-datahub-1.2.0/metofficedatahub/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-21 10:54:39.000000 metoffice-weather-datahub-1.2.0/metofficedatahub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-03-21 10:54:39.000000 metoffice-weather-datahub-1.2.0/metofficedatahub/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-03-21 10:54:39.000000 metoffice-weather-datahub-1.2.0/metofficedatahub/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-21 10:54:39.000000 metoffice-weather-datahub-1.2.0/metofficedatahub/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-03-21 10:54:39.000000 metoffice-weather-datahub-1.2.0/metofficedatahub/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-03-21 10:54:39.000000 metoffice-weather-datahub-1.2.0/metofficedatahub/multiple_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-03-21 10:54:39.000000 metoffice-weather-datahub-1.2.0/metofficedatahub/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-21 10:54:39.000000 metoffice-weather-datahub-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 10:54:54.249278 metoffice-weather-datahub-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-21 10:54:40.000000 metoffice-weather-datahub-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:54:54.249278 metoffice-weather-datahub-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-21 10:54:39.000000 metoffice-weather-datahub-1.2.0/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-03-21 10:54:39.000000 metoffice-weather-datahub-1.2.0/tests/test_multiple_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-21 10:54:39.000000 metoffice-weather-datahub-1.2.0/tests/test_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-21 10:54:39.000000 metoffice-weather-datahub-1.2.0/tests/test_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-21 10:54:39.000000 metoffice-weather-datahub-1.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:08:01.214213 metoffice-weather-datahub-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-25 11:07:49.000000 metoffice-weather-datahub-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 11:07:49.000000 metoffice-weather-datahub-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-25 11:08:01.214213 metoffice-weather-datahub-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-25 11:07:49.000000 metoffice-weather-datahub-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:08:01.214213 metoffice-weather-datahub-1.2.1/metoffice_weather_datahub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-25 11:08:01.000000 metoffice-weather-datahub-1.2.1/metoffice_weather_datahub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-25 11:08:01.000000 metoffice-weather-datahub-1.2.1/metoffice_weather_datahub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:08:01.000000 metoffice-weather-datahub-1.2.1/metoffice_weather_datahub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-25 11:08:01.000000 metoffice-weather-datahub-1.2.1/metoffice_weather_datahub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 11:08:01.000000 metoffice-weather-datahub-1.2.1/metoffice_weather_datahub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:08:01.214213 metoffice-weather-datahub-1.2.1/metofficedatahub/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-25 11:07:49.000000 metoffice-weather-datahub-1.2.1/metofficedatahub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-25 11:07:49.000000 metoffice-weather-datahub-1.2.1/metofficedatahub/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-05-25 11:07:49.000000 metoffice-weather-datahub-1.2.1/metofficedatahub/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-25 11:07:49.000000 metoffice-weather-datahub-1.2.1/metofficedatahub/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-25 11:07:49.000000 metoffice-weather-datahub-1.2.1/metofficedatahub/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-05-25 11:07:49.000000 metoffice-weather-datahub-1.2.1/metofficedatahub/multiple_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-25 11:07:49.000000 metoffice-weather-datahub-1.2.1/metofficedatahub/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-25 11:07:49.000000 metoffice-weather-datahub-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:08:01.214213 metoffice-weather-datahub-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-25 11:07:49.000000 metoffice-weather-datahub-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:08:01.214213 metoffice-weather-datahub-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-25 11:07:50.000000 metoffice-weather-datahub-1.2.1/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-25 11:07:50.000000 metoffice-weather-datahub-1.2.1/tests/test_multiple_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-25 11:07:50.000000 metoffice-weather-datahub-1.2.1/tests/test_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-25 11:07:50.000000 metoffice-weather-datahub-1.2.1/tests/test_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-25 11:07:50.000000 metoffice-weather-datahub-1.2.1/tests/test_utils.py
```

### Comparing `metoffice-weather-datahub-1.2.0/LICENSE` & `metoffice-weather-datahub-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.0/PKG-INFO` & `metoffice-weather-datahub-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metoffice-weather-datahub
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python wrapper for the UK Met Office Weather DataHub API
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `metoffice-weather-datahub-1.2.0/README.md` & `metoffice-weather-datahub-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.0/metoffice_weather_datahub.egg-info/PKG-INFO` & `metoffice-weather-datahub-1.2.1/metoffice_weather_datahub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metoffice-weather-datahub
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python wrapper for the UK Met Office Weather DataHub API
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `metoffice-weather-datahub-1.2.0/metoffice_weather_datahub.egg-info/SOURCES.txt` & `metoffice-weather-datahub-1.2.1/metoffice_weather_datahub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.0/metofficedatahub/app.py` & `metoffice-weather-datahub-1.2.1/metofficedatahub/app.py`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.0/metofficedatahub/base.py` & `metoffice-weather-datahub-1.2.1/metofficedatahub/base.py`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.0/metofficedatahub/models.py` & `metoffice-weather-datahub-1.2.1/metofficedatahub/models.py`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.0/metofficedatahub/multiple_files.py` & `metoffice-weather-datahub-1.2.1/metofficedatahub/multiple_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from typing import List
 
 import cfgrib
 import fsspec
 import pandas as pd
 import psutil
 import xarray as xr
+from ocf_blosc2 import Blosc2
 from pathy import Pathy
 
 from metofficedatahub.base import BaseMetOfficeDataHub
 from metofficedatahub.utils import add_x_y, post_process_dataset
 
 logger = logging.getLogger(__name__)
 
@@ -279,16 +280,24 @@
 
     chunked = _chunk(dataset, ideal_chunk_size_mb=ideal_chunk_size_mb)
     _log_and_save(chunked, f"{save_dir}/latest.zarr")
 
 
 def save_to_s3(dataset: xr.Dataset, path: str):
     """Save to s3"""
+
     if path.endswith(".zarr"):
-        dataset.to_zarr(store=path, mode="w", consolidated=True)
+        dataset.to_zarr(
+            store=path,
+            mode="w",
+            consolidated=True,
+            encoding={
+                "UKV": {"compressor": Blosc2("zstd", clevel=5)},
+            },
+        )
     elif path.endswith(".netcdf"):
         # xarray doesn't support writing .netcdf files directly to S3 like for .zarr files.
         # Also note the "simplecache::" and see https://github.com/pydata/xarray/issues/4122
         with fsspec.open("simplecache::" + path, mode="wb") as f:
             dataset.to_netcdf(f, engine="h5netcdf")
     else:
         assert False, "unexpected extension"
```

### Comparing `metoffice-weather-datahub-1.2.0/metofficedatahub/utils.py` & `metoffice-weather-datahub-1.2.1/metofficedatahub/utils.py`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.0/setup.py` & `metoffice-weather-datahub-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 install_requires = (this_directory / "requirements.txt").read_text().splitlines()
 
 setup(
     name="metoffice-weather-datahub",
-    version="1.2.0",
+    version="1.2.1",
     license="MIT",
     description="Python wrapper for the UK Met Office Weather DataHub API",
     author="Peter Dudfield",
     author_email="info@openclimatefix.org",
     company="Open Climate Fix Ltd",
     install_requires=install_requires,
     long_description=long_description,
```

### Comparing `metoffice-weather-datahub-1.2.0/tests/test_app.py` & `metoffice-weather-datahub-1.2.1/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.0/tests/test_multiple_files.py` & `metoffice-weather-datahub-1.2.1/tests/test_multiple_files.py`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.0/tests/test_orders.py` & `metoffice-weather-datahub-1.2.1/tests/test_orders.py`

 * *Files identical despite different names*

### Comparing `metoffice-weather-datahub-1.2.0/tests/test_utils.py` & `metoffice-weather-datahub-1.2.1/tests/test_utils.py`

 * *Files identical despite different names*

