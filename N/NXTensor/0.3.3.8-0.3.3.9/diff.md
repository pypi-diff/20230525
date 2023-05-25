# Comparing `tmp/NXTensor-0.3.3.8.tar.gz` & `tmp/NXTensor-0.3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NXTensor-0.3.3.8.tar", last modified: Wed Apr 14 12:54:35 2021, max compression
+gzip compressed data, was "dist/NXTensor-0.3.3.9.tar", last modified: Wed Jun  2 12:51:16 2021, max compression
```

## Comparing `NXTensor-0.3.3.8.tar` & `NXTensor-0.3.3.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 sgardoll (40315) ipsl     (20000)        0 2021-04-14 12:54:35.373836 NXTensor-0.3.3.8/
-drwxr-xr-x   0 sgardoll (40315) ipsl     (20000)        0 2021-04-14 12:54:35.363836 NXTensor-0.3.3.8/NXTensor.egg-info/
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     2207 2021-04-14 12:54:35.000000 NXTensor-0.3.3.8/NXTensor.egg-info/PKG-INFO
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     1172 2021-04-14 12:54:35.000000 NXTensor-0.3.3.8/NXTensor.egg-info/SOURCES.txt
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)        1 2021-04-14 12:54:35.000000 NXTensor-0.3.3.8/NXTensor.egg-info/dependency_links.txt
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)      150 2021-04-14 12:54:35.000000 NXTensor-0.3.3.8/NXTensor.egg-info/requires.txt
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)        9 2021-04-14 12:54:35.000000 NXTensor-0.3.3.8/NXTensor.egg-info/top_level.txt
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     2207 2021-04-14 12:54:35.373836 NXTensor-0.3.3.8/PKG-INFO
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)      997 2021-04-14 12:47:59.000000 NXTensor-0.3.3.8/README.md
-drwxr-xr-x   0 sgardoll (40315) ipsl     (20000)        0 2021-04-14 12:54:35.365836 NXTensor-0.3.3.8/nxtensor/
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)      143 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/__init__.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)    10618 2021-04-14 12:47:59.000000 NXTensor-0.3.3.8/nxtensor/assembly.py
-drwxr-xr-x   0 sgardoll (40315) ipsl     (20000)        0 2021-04-14 12:54:35.367836 NXTensor-0.3.3.8/nxtensor/core/
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)      143 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/core/__init__.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)    10354 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/core/assembly.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)      926 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/core/types.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)    13000 2021-02-09 09:13:43.000000 NXTensor-0.3.3.8/nxtensor/core/xarray_channel_extraction.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     5877 2020-12-11 13:44:38.000000 NXTensor-0.3.3.8/nxtensor/core/xarray_extractions.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)      213 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/exceptions.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     7312 2021-04-14 12:47:59.000000 NXTensor-0.3.3.8/nxtensor/extraction.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     4603 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/extractor.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)    11299 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/square_extractor.py
-drwxr-xr-x   0 sgardoll (40315) ipsl     (20000)        0 2021-04-14 12:54:35.368836 NXTensor-0.3.3.8/nxtensor/tests/
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)      143 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/tests/__init__.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     5310 2021-04-14 07:49:39.000000 NXTensor-0.3.3.8/nxtensor/tests/create_era5_extraction.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     5583 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/tests/create_era5_variables.py
-drwxr-xr-x   0 sgardoll (40315) ipsl     (20000)        0 2021-04-14 12:54:35.372836 NXTensor-0.3.3.8/nxtensor/utils/
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)      143 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/utils/__init__.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     5167 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/utils/coordinate_utils.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)      597 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/utils/coordinates.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)      369 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/utils/csv_option_names.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     2694 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/utils/csv_utils.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)      178 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/utils/db_types.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     2951 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/utils/db_utils.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)      676 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/utils/file_utils.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)      533 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/utils/hdf5_utils.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     1164 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/utils/image_utils.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     7895 2021-01-11 10:15:08.000000 NXTensor-0.3.3.8/nxtensor/utils/interpolation_utils.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     4098 2021-02-09 09:13:43.000000 NXTensor-0.3.3.8/nxtensor/utils/naming_utils.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)      405 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/utils/tensor_dimensions.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)      559 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/utils/time_resolutions.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     3740 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/utils/time_utils.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     8028 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/utils/xarray_rpn_calulator.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     8466 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/variable.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     5603 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/variable_block_extraction.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     1719 2020-12-11 10:42:34.000000 NXTensor-0.3.3.8/nxtensor/yaml_serializable.py
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)       38 2021-04-14 12:54:35.373836 NXTensor-0.3.3.8/setup.cfg
--rw-r--r--   0 sgardoll (40315) ipsl     (20000)     1477 2021-04-14 12:47:59.000000 NXTensor-0.3.3.8/setup.py
+drwxr-xr-x   0 sgardoll (40315) ipsl     (20000)        0 2021-06-02 12:51:16.364570 NXTensor-0.3.3.9/
+drwxr-xr-x   0 sgardoll (40315) ipsl     (20000)        0 2021-06-02 12:51:16.342571 NXTensor-0.3.3.9/NXTensor.egg-info/
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     2207 2021-06-02 12:51:16.000000 NXTensor-0.3.3.9/NXTensor.egg-info/PKG-INFO
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     1172 2021-06-02 12:51:16.000000 NXTensor-0.3.3.9/NXTensor.egg-info/SOURCES.txt
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)        1 2021-06-02 12:51:16.000000 NXTensor-0.3.3.9/NXTensor.egg-info/dependency_links.txt
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)      150 2021-06-02 12:51:16.000000 NXTensor-0.3.3.9/NXTensor.egg-info/requires.txt
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)        9 2021-06-02 12:51:16.000000 NXTensor-0.3.3.9/NXTensor.egg-info/top_level.txt
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     2207 2021-06-02 12:51:16.363571 NXTensor-0.3.3.9/PKG-INFO
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)      997 2021-04-14 12:47:59.000000 NXTensor-0.3.3.9/README.md
+drwxr-xr-x   0 sgardoll (40315) ipsl     (20000)        0 2021-06-02 12:51:16.345571 NXTensor-0.3.3.9/nxtensor/
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)      143 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/__init__.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)    10618 2021-04-14 12:47:59.000000 NXTensor-0.3.3.9/nxtensor/assembly.py
+drwxr-xr-x   0 sgardoll (40315) ipsl     (20000)        0 2021-06-02 12:51:16.348571 NXTensor-0.3.3.9/nxtensor/core/
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)      143 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/core/__init__.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)    10354 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/core/assembly.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)      926 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/core/types.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)    13000 2021-02-09 09:13:43.000000 NXTensor-0.3.3.9/nxtensor/core/xarray_channel_extraction.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     5877 2020-12-11 13:44:38.000000 NXTensor-0.3.3.9/nxtensor/core/xarray_extractions.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)      213 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/exceptions.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     7452 2021-06-02 12:49:41.000000 NXTensor-0.3.3.9/nxtensor/extraction.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     4799 2021-06-02 12:49:41.000000 NXTensor-0.3.3.9/nxtensor/extractor.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)    11730 2021-06-02 12:49:41.000000 NXTensor-0.3.3.9/nxtensor/square_extractor.py
+drwxr-xr-x   0 sgardoll (40315) ipsl     (20000)        0 2021-06-02 12:51:16.350571 NXTensor-0.3.3.9/nxtensor/tests/
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)      143 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/tests/__init__.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     5366 2021-06-02 12:49:41.000000 NXTensor-0.3.3.9/nxtensor/tests/create_era5_extraction.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     5583 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/tests/create_era5_variables.py
+drwxr-xr-x   0 sgardoll (40315) ipsl     (20000)        0 2021-06-02 12:51:16.362571 NXTensor-0.3.3.9/nxtensor/utils/
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)      143 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/utils/__init__.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     5554 2021-06-02 12:49:41.000000 NXTensor-0.3.3.9/nxtensor/utils/coordinate_utils.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)      597 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/utils/coordinates.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)      369 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/utils/csv_option_names.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     2694 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/utils/csv_utils.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)      178 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/utils/db_types.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     2951 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/utils/db_utils.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)      676 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/utils/file_utils.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)      533 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/utils/hdf5_utils.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     1164 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/utils/image_utils.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     7895 2021-01-11 10:15:08.000000 NXTensor-0.3.3.9/nxtensor/utils/interpolation_utils.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     4098 2021-02-09 09:13:43.000000 NXTensor-0.3.3.9/nxtensor/utils/naming_utils.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)      405 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/utils/tensor_dimensions.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)      559 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/utils/time_resolutions.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     3740 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/utils/time_utils.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     8028 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/utils/xarray_rpn_calulator.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     8466 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/variable.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     5722 2021-06-02 12:49:41.000000 NXTensor-0.3.3.9/nxtensor/variable_block_extraction.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     1719 2020-12-11 10:42:34.000000 NXTensor-0.3.3.9/nxtensor/yaml_serializable.py
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)       38 2021-06-02 12:51:16.364570 NXTensor-0.3.3.9/setup.cfg
+-rw-r--r--   0 sgardoll (40315) ipsl     (20000)     1477 2021-06-02 12:49:41.000000 NXTensor-0.3.3.9/setup.py
```

### Comparing `NXTensor-0.3.3.8/NXTensor.egg-info/PKG-INFO` & `NXTensor-0.3.3.9/NXTensor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NXTensor
-Version: 0.3.3.8
+Version: 0.3.3.9
 Summary: NXTensor is a tensor making framework based on Xarray. It automates the extraction of multichannel images (tensors) from NetCDF time series of geolocated data.
 Home-page: UNKNOWN
 Author: Sébastien Gardoll
 Author-email: sebastien@gardoll.fr
 License: UNKNOWN
 Description: # NXTensor
```

### Comparing `NXTensor-0.3.3.8/NXTensor.egg-info/SOURCES.txt` & `NXTensor-0.3.3.9/NXTensor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/PKG-INFO` & `NXTensor-0.3.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NXTensor
-Version: 0.3.3.8
+Version: 0.3.3.9
 Summary: NXTensor is a tensor making framework based on Xarray. It automates the extraction of multichannel images (tensors) from NetCDF time series of geolocated data.
 Home-page: UNKNOWN
 Author: Sébastien Gardoll
 Author-email: sebastien@gardoll.fr
 License: UNKNOWN
 Description: # NXTensor
```

### Comparing `NXTensor-0.3.3.8/README.md` & `NXTensor-0.3.3.9/README.md`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/nxtensor/assembly.py` & `NXTensor-0.3.3.9/nxtensor/assembly.py`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/nxtensor/core/assembly.py` & `NXTensor-0.3.3.9/nxtensor/core/assembly.py`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/nxtensor/core/types.py` & `NXTensor-0.3.3.9/nxtensor/core/types.py`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/nxtensor/core/xarray_channel_extraction.py` & `NXTensor-0.3.3.9/nxtensor/core/xarray_channel_extraction.py`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/nxtensor/core/xarray_extractions.py` & `NXTensor-0.3.3.9/nxtensor/core/xarray_extractions.py`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/nxtensor/extraction.py` & `NXTensor-0.3.3.9/nxtensor/extraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,17 @@
 
         # At the end of the tensor assemble. Has it to be shuffled ?
         self.has_tensor_to_be_shuffled: bool = None
 
         # Are the channels of the tensor at the last dimensions of the tensor ?
         self.is_channels_last = None
 
+        # Specify if the coordinates has to be rounded according to the variable resolutions.
+        self.has_to_round_coordinates = None
+
         # The tensor will be split into the given dataset ratios.
         self.tensor_dataset_ratios: Mapping[str, float] = None
 
         # TODO: save metadata options (csv).
 
     def save(self, file_path: str) -> None:
         variables = self.__variables
```

### Comparing `NXTensor-0.3.3.8/nxtensor/extractor.py` & `NXTensor-0.3.3.9/nxtensor/extractor.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,36 +34,39 @@
             return ExtractionVisitor.__EXTRACTOR_FACTORY[shape]
         except KeyError:
             msg = f"> [ERROR] unknown extraction shape '{shape}'"
             raise ConfigurationError(msg)
 
     def __init__(self, period: Period, extraction_metadata_blocks: List[Tuple[LabelId, MetaDataBlock]],
                  half_lat_frame: int,
-                 half_lon_frame: int, dask_scheduler: str = 'single-threaded',
+                 half_lon_frame: int, has_to_round_coordinates: bool, dask_scheduler: str = 'single-threaded',
                  shape: ExtractionShape = ExtractionShape.SQUARE):
         self.__period: Period = period
         self.__extraction_metadata_blocks: List[Tuple[LabelId, MetaDataBlock]] = extraction_metadata_blocks
         self.__half_lat_frame: int = half_lat_frame
         self.__half_lon_frame: int = half_lon_frame
+        self.__has_to_round_coordinates = has_to_round_coordinates
         self.__dask_scheduler: str = dask_scheduler
         self.__shape: ExtractionShape = shape
         self.result: List[Tuple[LabelId, xr.DataArray, MetaDataBlock]] = list()
 
     def __core_extraction(self, var: Variable, datasets: Mapping[VariableId, xr.Dataset]) -> None:
 
         for label_id, extraction_metadata_block in self.__extraction_metadata_blocks:
             extracted_regions: List[xr.DataArray] = list()
             # The order of extraction_data_list must be deterministic so as all the channel
             # match their extracted region line by line.
             for extraction_data in extraction_metadata_block:
-                extractor = ExtractionVisitor.__create_extractor(self.__shape)(datasets=datasets,
-                                                                               extraction_data=extraction_data,
-                                                                               half_lat_frame=self.__half_lat_frame,
-                                                                               half_lon_frame=self.__half_lon_frame,
-                                                                               dask_scheduler=self.__dask_scheduler)
+                extractor = ExtractionVisitor.__create_extractor(self.__shape)(
+                                                           datasets=datasets,
+                                                           extraction_data=extraction_data,
+                                                           half_lat_frame=self.__half_lat_frame,
+                                                           half_lon_frame=self.__half_lon_frame,
+                                                           has_to_round_coordinates=self.__has_to_round_coordinates,
+                                                           dask_scheduler=self.__dask_scheduler)
                 var.accept(extractor)
                 extracted_regions.append(extractor.get_result())
 
             # dims are lost when instantiating a DataArray based on other DataArray objects.
             dims = (var.str_id, TensorDimension.X, TensorDimension.Y)
             # Stack the extracted regions in a xarray data array => data extraction_metadata_blocks.
             data = xr.DataArray(extracted_regions, dims=dims)
```

### Comparing `NXTensor-0.3.3.8/nxtensor/square_extractor.py` & `NXTensor-0.3.3.9/nxtensor/square_extractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,34 +20,37 @@
 from nxtensor.core.types import VariableId
 
 
 class RegionExtractionVisitor(VariableVisitor):
     @abstractmethod
     def __init__(self, datasets: Mapping[VariableId, xr.Dataset],
                  extraction_data: Mapping[Union[Coordinate, TimeResolution], Union[int, float]],
-                 half_lat_frame: int, half_lon_frame: int, dask_scheduler: str = 'single-threaded'):
+                 half_lat_frame: int, half_lon_frame: int, has_to_round_coordinates: bool,
+                 dask_scheduler: str = 'single-threaded'):
         # Buffer of extracted regions: optimization for computed variables.
         # Computed variables may contain computed variables, recursively !
         self._extracted_regions: Dict[VariableId, xr.DataArray] = dict()
         self._datasets: Mapping[VariableId, xr.Dataset] = datasets
         self._extraction_data: Mapping[Union[Coordinate, TimeResolution], Union[int, float]] = extraction_data
         self._half_lat_frame: int = half_lat_frame
         self._half_lon_frame: int = half_lon_frame
+        self._has_to_round_coordinates: bool = has_to_round_coordinates
         self._dask_scheduler: str = dask_scheduler
         self._recursive_call_count: int = 0
         # noinspection PyTypeChecker
         self._result: xr.DataArray = None
 
 
 class SquareRegionExtractionVisitor(RegionExtractionVisitor):
 
     def __init__(self, datasets: Mapping[VariableId, xr.Dataset],
                  extraction_data: Mapping[Union[Coordinate, TimeResolution], Union[int, float]], half_lat_frame: int,
-                 half_lon_frame: int, dask_scheduler: str = 'single-threaded'):
-        super().__init__(datasets, extraction_data, half_lat_frame, half_lon_frame, dask_scheduler)
+                 half_lon_frame: int, has_to_round_coordinates: bool, dask_scheduler: str = 'single-threaded'):
+        super().__init__(datasets, extraction_data, half_lat_frame, half_lon_frame, has_to_round_coordinates,
+                         dask_scheduler)
 
     def __bootstrap(self, var: SingleLevelVariable) -> str:
         # month2d, day2d and hour2d are computed when calling convert_block_to_dict function from module
         # xarray_channel_extraction.
         formatted_date = var.date_template.format(**self._extraction_data)
         return formatted_date
 
@@ -62,15 +65,16 @@
                                                         half_lat_frame=self._half_lat_frame,
                                                         lon=self._extraction_data[Coordinate.LON],
                                                         lon_resolution=var.lon_resolution,
                                                         half_lon_frame=self._half_lon_frame,
                                                         time_netcdf_attr_name=var.time_netcdf_attr_name,
                                                         lat_netcdf_attr_name=var.lat_netcdf_attr_name,
                                                         lon_netcdf_attr_name=var.lon_netcdf_attr_name,
-                                                        has_to_round=True, lat_nb_decimal=var.lat_nb_decimal,
+                                                        has_to_round=self._has_to_round_coordinates,
+                                                        lat_nb_decimal=var.lat_nb_decimal,
                                                         lon_nb_decimal=var.lon_nb_decimal,
                                                         dask_scheduler=self._dask_scheduler)
             self._extracted_regions[var.str_id] = self._result
 
     def visit_multi_level_variable(self, var: MultiLevelVariable) -> None:
         if var.str_id not in self._extracted_regions:
             formatted_date = self.__bootstrap(var)
@@ -83,15 +87,16 @@
                                                         lon=self._extraction_data[Coordinate.LON],
                                                         lon_resolution=var.lon_resolution,
                                                         half_lon_frame=self._half_lon_frame, variable_level=var.level,
                                                         level_netcdf_attr_name=var.level_netcdf_attr_name,
                                                         time_netcdf_attr_name=var.time_netcdf_attr_name,
                                                         lat_netcdf_attr_name=var.lat_netcdf_attr_name,
                                                         lon_netcdf_attr_name=var.lon_netcdf_attr_name,
-                                                        has_to_round=True, lat_nb_decimal=var.lat_nb_decimal,
+                                                        has_to_round=self._has_to_round_coordinates,
+                                                        lat_nb_decimal=var.lat_nb_decimal,
                                                         lon_nb_decimal=var.lon_nb_decimal,
                                                         dask_scheduler=self._dask_scheduler)
             self._extracted_regions[var.str_id] = self._result
 
     def visit_computed_variable(self, var: ComputedVariable) -> None:
         if var.str_id not in self._extracted_regions:
             self._recursive_call_count = self._recursive_call_count + 1
@@ -189,26 +194,27 @@
 
 def __test_extraction(str_id, variable_parent_dir_path,
                       extraction_data: Mapping[Union[Coordinate, TimeResolution], Union[int, float]],
                       half_lat_frame, half_lon_frame, has_to_plot=True):
     import os.path as path
     from matplotlib import pyplot as plt
     import nxtensor.utils.file_utils as fu
+    has_to_round = True
     var = Variable.load(path.join(variable_parent_dir_path,
                         f"{str_id}{nxtensor.utils.naming_utils.NAME_SEPARATOR}{Variable.FILE_NAME_POSTFIX}"))
 
     # noinspection PyTypeChecker
     visitor = VariableNetcdfFilePathVisitor(extraction_data)
     var.accept(visitor)
     netcdf_file_path_dict = visitor.get_result()
     datasets = {var_id: xtract.open_netcdf(netcdf_file_path) for var_id, netcdf_file_path in
                 netcdf_file_path_dict.items()}
     extractor = SquareRegionExtractionVisitor(datasets=datasets, extraction_data=extraction_data,
                                               half_lat_frame=half_lat_frame, half_lon_frame=half_lon_frame,
-                                              dask_scheduler='single-threaded')
+                                              has_to_round_coordinates=has_to_round, dask_scheduler='single-threaded')
     var.accept(extractor)
     extracted_region = extractor.get_result()
     [dataset.close() for dataset in datasets.values()]
 
     if has_to_plot:
         plt.figure()
         plt.imshow(extracted_region, cmap='gist_rainbow_r', interpolation="none")
```

### Comparing `NXTensor-0.3.3.8/nxtensor/tests/create_era5_extraction.py` & `NXTensor-0.3.3.9/nxtensor/tests/create_era5_extraction.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
         extract_config.blocks_dir_path = path.join(output_parent_dir, 'blocks')
         extract_config.channels_dir_path = path.join(output_parent_dir, 'channels')
         extract_config.tensors_dir_path = path.join(output_parent_dir, 'tensors')
         extract_config.tmp_dir_path = path.join(output_parent_dir, 'tmp')
         extract_config.nb_process = nb_process
         extract_config.has_tensor_to_be_shuffled = True
         extract_config.is_channels_last = True
+        extract_config.has_to_round_coordinates = False
         extract_config.tensor_dataset_ratios = {'test': 0.2, 'validation': 0.2, 'training': 0.6}
         extract_config.max_walltime = '01:59:59'
         extract_config.extraction_mem_foot_print = '10gb'
         extract_config.assembly_mem_foot_print = '30gb'
         extract_config.qsub_log_dir_path = path.join(output_parent_dir, 'job_logs')
 
         file_path = path.join(config_parent_dir, ExtractionConfig.generate_filename(dataset_id))
```

### Comparing `NXTensor-0.3.3.8/nxtensor/tests/create_era5_variables.py` & `NXTensor-0.3.3.9/nxtensor/tests/create_era5_variables.py`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/nxtensor/utils/coordinate_utils.py` & `NXTensor-0.3.3.9/nxtensor/utils/coordinate_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,23 @@
 __CONVERT_MAPPING = dict()
 
 
 def round_nearest(value, resolution, num_decimal):
     return round(round(value / resolution) * resolution, num_decimal)
 
 
+def round_coordinates(dataframe: pd.DataFrame, column_name: str, resolution: float, nb_decimal_to_round: int):
+    # Update the format of the coordinate.
+    def __round_coordinates(value):
+        rounded_value = round_nearest(value, resolution, nb_decimal_to_round)
+        return rounded_value
+
+    dataframe[column_name] = np.vectorize(__round_coordinates)(dataframe[column_name])
+
+
 def reformat_coordinates(dataframe: pd.DataFrame, column_name: str, from_format: CoordinateFormat,
                          to_format: CoordinateFormat, resolution: float, nb_decimal_to_round: int):
     coordinate_mapping = __get_convert_mapping(from_format, to_format, resolution)
 
     # Update the format of the coordinate.
     def __convert_coordinates(value):
         rounded_value = round_nearest(value, resolution, nb_decimal_to_round)
```

### Comparing `NXTensor-0.3.3.8/nxtensor/utils/coordinates.py` & `NXTensor-0.3.3.9/nxtensor/utils/coordinates.py`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/nxtensor/utils/csv_utils.py` & `NXTensor-0.3.3.9/nxtensor/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/nxtensor/utils/db_utils.py` & `NXTensor-0.3.3.9/nxtensor/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/nxtensor/utils/file_utils.py` & `NXTensor-0.3.3.9/nxtensor/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/nxtensor/utils/hdf5_utils.py` & `NXTensor-0.3.3.9/nxtensor/utils/hdf5_utils.py`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/nxtensor/utils/image_utils.py` & `NXTensor-0.3.3.9/nxtensor/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/nxtensor/utils/interpolation_utils.py` & `NXTensor-0.3.3.9/nxtensor/utils/interpolation_utils.py`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/nxtensor/utils/naming_utils.py` & `NXTensor-0.3.3.9/nxtensor/utils/naming_utils.py`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/nxtensor/utils/time_resolutions.py` & `NXTensor-0.3.3.9/nxtensor/utils/time_resolutions.py`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/nxtensor/utils/time_utils.py` & `NXTensor-0.3.3.9/nxtensor/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/nxtensor/utils/xarray_rpn_calulator.py` & `NXTensor-0.3.3.9/nxtensor/utils/xarray_rpn_calulator.py`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/nxtensor/variable.py` & `NXTensor-0.3.3.9/nxtensor/variable.py`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/nxtensor/variable_block_extraction.py` & `NXTensor-0.3.3.9/nxtensor/variable_block_extraction.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,20 +69,22 @@
 
     def process_blocks(self, period: Period, extraction_metadata_blocks: List[Tuple[LabelId, MetaDataBlock]]) \
             -> Tuple[str, List[Tuple[LabelId, xr.DataArray, MetaDataBlock]]]:
         # Must be a integer !!! TODO: check for that when designing an extraction.
         half_lat_frame = int((self.__extraction_conf.y_size * self.__variable.lat_resolution)/2)
         half_lon_frame = int((self.__extraction_conf.y_size * self.__variable.lon_resolution)/2)
 
-        extractor: ExtractionVisitor = ExtractionVisitor(period=period,
-                                                         extraction_metadata_blocks=extraction_metadata_blocks,
-                                                         half_lat_frame=half_lat_frame,
-                                                         half_lon_frame=half_lon_frame,
-                                                         dask_scheduler=self.__extraction_conf.dask_scheduler,
-                                                         shape=self.__extraction_conf.extraction_shape)
+        extractor: ExtractionVisitor = ExtractionVisitor(
+                                               period=period,
+                                               extraction_metadata_blocks=extraction_metadata_blocks,
+                                               half_lat_frame=half_lat_frame,
+                                               half_lon_frame=half_lon_frame,
+                                               has_to_round_coordinates=self.__extraction_conf.has_to_round_coordinates,
+                                               dask_scheduler=self.__extraction_conf.dask_scheduler,
+                                               shape=self.__extraction_conf.extraction_shape)
         self.__variable.accept(extractor)
         result: Tuple[str, List[Tuple[LabelId, xr.DataArray, MetaDataBlock]]] = \
             (self.__extraction_conf.blocks_dir_path, extractor.get_result())
 
         return result
```

### Comparing `NXTensor-0.3.3.8/nxtensor/yaml_serializable.py` & `NXTensor-0.3.3.9/nxtensor/yaml_serializable.py`

 * *Files identical despite different names*

### Comparing `NXTensor-0.3.3.8/setup.py` & `NXTensor-0.3.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="NXTensor",
-    version="0.3.3.8",
+    version="0.3.3.9",
     author="Sébastien Gardoll",
     author_email="sebastien@gardoll.fr",
     description="NXTensor is a tensor making framework based on Xarray. It automates the extraction " +
                 "of multichannel images (tensors) from NetCDF time series of geolocated data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
```

