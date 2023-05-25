# Comparing `tmp/pyopenrivercam-0.4.3.tar.gz` & `tmp/pyopenrivercam-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopenrivercam-0.4.3.tar", last modified: Fri Apr  7 09:17:26 2023, max compression
+gzip compressed data, was "pyopenrivercam-0.5.0.tar", last modified: Thu May 25 18:22:10 2023, max compression
```

## Comparing `pyopenrivercam-0.4.3.tar` & `pyopenrivercam-0.5.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 09:17:26.074780 pyopenrivercam-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-07 09:17:07.000000 pyopenrivercam-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-04-07 09:17:26.074780 pyopenrivercam-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-04-07 09:17:07.000000 pyopenrivercam-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 09:17:26.066780 pyopenrivercam-0.4.3/pyopenrivercam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-04-07 09:17:26.000000 pyopenrivercam-0.4.3/pyopenrivercam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-07 09:17:26.000000 pyopenrivercam-0.4.3/pyopenrivercam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 09:17:26.000000 pyopenrivercam-0.4.3/pyopenrivercam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-07 09:17:26.000000 pyopenrivercam-0.4.3/pyopenrivercam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 09:17:25.000000 pyopenrivercam-0.4.3/pyopenrivercam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-07 09:17:26.000000 pyopenrivercam-0.4.3/pyopenrivercam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 09:17:26.000000 pyopenrivercam-0.4.3/pyopenrivercam.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 09:17:26.066780 pyopenrivercam-0.4.3/pyorc/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 09:17:26.070780 pyopenrivercam-0.4.3/pyorc/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33354 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/api/cameraconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    20800 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/api/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)    14887 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/api/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/api/orcbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    25778 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/api/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/api/transect.py
--rw-r--r--   0 runner    (1001) docker     (123)    35404 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/api/velocimetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19367 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/api/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 09:17:26.070780 pyopenrivercam-0.4.3/pyorc/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14708 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/cli/cli_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/cli/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/cli/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    39272 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/cv.py
--rw-r--r--   0 runner    (1001) docker     (123)    21279 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/piv_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 09:17:26.070780 pyopenrivercam-0.4.3/pyorc/service/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/service/camera_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/pyorc/service/velocimetry.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 09:17:26.074780 pyopenrivercam-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 09:17:26.074780 pyopenrivercam-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14443 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/tests/test_cameraconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/tests/test_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/tests/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/tests/test_transect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/tests/test_velocimetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-07 09:17:08.000000 pyopenrivercam-0.4.3/tests/test_video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:22:10.792118 pyopenrivercam-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-05-25 18:22:10.792118 pyopenrivercam-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:22:10.788118 pyopenrivercam-0.5.0/pyopenrivercam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-05-25 18:22:10.000000 pyopenrivercam-0.5.0/pyopenrivercam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-25 18:22:10.000000 pyopenrivercam-0.5.0/pyopenrivercam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 18:22:10.000000 pyopenrivercam-0.5.0/pyopenrivercam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 18:22:10.000000 pyopenrivercam-0.5.0/pyopenrivercam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 18:22:10.000000 pyopenrivercam-0.5.0/pyopenrivercam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-25 18:22:10.000000 pyopenrivercam-0.5.0/pyopenrivercam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 18:22:10.000000 pyopenrivercam-0.5.0/pyopenrivercam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:22:10.788118 pyopenrivercam-0.5.0/pyorc/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:22:10.792118 pyopenrivercam-0.5.0/pyorc/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40309 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/api/cameraconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20874 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/api/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14887 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/api/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/api/orcbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25778 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/api/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/api/transect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/api/velocimetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17689 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/api/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:22:10.792118 pyopenrivercam-0.5.0/pyorc/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20829 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/cli/cli_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/cli/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/cli/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29408 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21279 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/piv_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:22:10.792118 pyopenrivercam-0.5.0/pyorc/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/service/camera_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/service/velocimetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 18:22:10.792118 pyopenrivercam-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:22:10.792118 pyopenrivercam-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/tests/test_cameraconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/tests/test_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/tests/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/tests/test_transect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/tests/test_velocimetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/tests/test_video.py
```

### Comparing `pyopenrivercam-0.4.3/LICENSE` & `pyopenrivercam-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.4.3/PKG-INFO` & `pyopenrivercam-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopenrivercam
-Version: 0.4.3
+Version: 0.5.0
 Summary: pyopenrivercam (pyorc) is a front and backend to control river camera observation locations
 Home-page: https://github.com/localdevices/pyorc
 Author: Hessel Winsemius
 Author-email: winsemius@rainbowsensing.com
 License: AGPLv3
 Keywords: hydrology,hydrometry,river-flow,pyorc
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyopenrivercam-0.4.3/README.md` & `pyopenrivercam-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.4.3/pyopenrivercam.egg-info/PKG-INFO` & `pyopenrivercam-0.5.0/pyopenrivercam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopenrivercam
-Version: 0.4.3
+Version: 0.5.0
 Summary: pyopenrivercam (pyorc) is a front and backend to control river camera observation locations
 Home-page: https://github.com/localdevices/pyorc
 Author: Hessel Winsemius
 Author-email: winsemius@rainbowsensing.com
 License: AGPLv3
 Keywords: hydrology,hydrometry,river-flow,pyorc
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyopenrivercam-0.4.3/pyopenrivercam.egg-info/SOURCES.txt` & `pyopenrivercam-0.5.0/pyopenrivercam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.4.3/pyorc/api/cameraconfig.py` & `pyopenrivercam-0.5.0/pyorc/api/cameraconfig.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import copy
 import cv2
 import json
 import matplotlib.pyplot as plt
 import numpy as np
 import os
+import shapely.geometry
 from shapely import ops, wkt
 from shapely.geometry import Polygon, LineString, Point
 
 from matplotlib import patches
 from pyproj import CRS, Transformer
 from pyproj.exceptions import CRSError
 
+from typing import Any, Dict, List, Optional, Tuple, Union
+
 from .. import cv, helpers
 
 
 class CameraConfig:
     """
     Camera configuration containing information about the perspective of the camera with respect to real world
     coordinates
@@ -23,28 +26,29 @@
         return str(self.to_json())
 
     def __repr__(self):
         return self.to_json()
 
     def __init__(
             self,
-            height,
-            width,
-            crs=None,
-            window_size=10,
-            resolution=0.05,
-            bbox=None,
-            camera_matrix=None,
-            dist_coeffs=None,
-            lens_position=None,
-            corners=None,
-            gcps=None,
-            lens_pars=None,
-            calibration_video=None
-
+            height: int,
+            width: int,
+            crs: Optional[Any] = None,
+            window_size: int = 10,
+            resolution: float = 0.05,
+            bbox: Optional[shapely.geometry.Polygon] = None,
+            camera_matrix: Optional[List[List[float]]] = None,
+            dist_coeffs: Optional[List[List[float]]] = None,
+            lens_position: Optional[List[float]] = None,
+            corners: Optional[List[List[float]]] = None,
+            gcps: Optional[Dict[str, Union[List, float]]] = None,
+            lens_pars: Optional[Dict[str, float]] = None,
+            calibration_video: Optional[str] = None,
+            is_nadir: Optional[bool] = False,
+            stabilize: Optional[List[List]] = None
     ):
         """
 
         Parameters
         ----------
         height : int
             height of frame in pixels
@@ -60,67 +64,79 @@
         bbox : shapely.geometry.Polygon, optional
             bounding box in geographical coordinates
         lens_position : list of floats (3),
             x, y, z coordinate of lens position in CRS
         corners : list of lists of floats (2)
             [x, y] coordinates defining corners of area of interest in camera cols/rows, bbox will be computed from this
         gcps : dict
-            Can contain "src": list of 4 lists, with column, row locations in objective of control points,
-            "dst": list of 4 lists, with x, y locations (local or global coordinate reference system) of control points,
+            Can contain "src": list of lists, with column, row locations in objective of control points,
+            "dst": list of lists, with x, y or x, y, z locations (local or global coordinate reference system) of
+            control points,
             "h_ref": float, measured water level [m] in local reference system (e.g. from staff gauge or pressure gauge)
             during gcp survey,
             "z_0": float, water level [m] in global reference system (e.g. from used GPS system CRS). This must be in
             the same vertical reference as the measured bathymetry and other survey points,
             "crs": int, str or CRS object, CRS in which "dst" points are measured. If None, a local coordinate system is
             assumed (e.g. from spirit level).
-        lens_pars : dict, optional
+        lens_pars (deprecated) : dict, optional
             Lens parameters, containing: "k1": float, barrel lens distortion parameter (default: 0.),
             "c": float, optical center (default: 2.),
-            "f": float, focal length (default: 1.)
+            "focal_length": float, focal length (default: width of image frame)
         calibration_video : str, optional
             local path to video file containing a checkerboard pattern. Must be 9x6 if called directly, otherwise use
             ``.calibrate_camera`` explicitly and provide ``chessboard_size`` explicitly. When used, an automated camera
             calibration on the video file will be attempted.
         """
         assert(isinstance(height, int)), 'height must be provided as type "int"'
         assert(isinstance(width, int)), 'width must be provided as type "int"'
         assert (isinstance(window_size, int)), 'window_size must be of type "int"'
         self.height = height
         self.width = width
+        self.is_nadir = is_nadir
         if crs is not None:
             try:
                 crs = CRS.from_user_input(crs)
             except CRSError:
                 raise CRSError(f'crs "{crs}" is not a valid Coordinate Reference System')
-            assert (crs.is_geographic == 0), "Provided crs must be projected with units like [m]"
+            assert (crs.is_geographic == 0), "Prodstvided crs must be projected with units like [m]"
             self.crs = crs.to_wkt()
         if resolution is not None:
             self.resolution = resolution
         if lens_position is not None:
             self.set_lens_position(*lens_position)
+        else:
+            self.lens_position = None
         if gcps is not None:
             self.set_gcps(**gcps)
-        if lens_pars is not None:
-            self.set_lens_pars(**lens_pars)
+        if camera_matrix is None or dist_coeffs is None:
+            if self.is_nadir:
+                # with nadir, no perspective can be constructed, hence, camera matrix and dist coeffs will be set to default values
+                self.camera_matrix = cv._get_cam_mtx(self.height, self.width)
+                self.dist_coeffs = cv.DIST_COEFFS
+            # camera pars are incomplete and need to be derived
+            else:
+                self.set_intrinsic(
+                    camera_matrix=camera_matrix,
+                    lens_pars=lens_pars
+                )
         else:
-            self.set_lens_pars()
-        if calibration_video is not None:
-            self.set_lens_calibration(calibration_video, plot=False)
-        # camera matrix and dist coeffs can also be set hard, this overrules the lens_pars option
-        if camera_matrix is not None:
+            # camera matrix and dist coeffs can also be set hard, this overrules the lens_pars option
             self.camera_matrix = camera_matrix
-        if dist_coeffs is not None:
             self.dist_coeffs = dist_coeffs
+        if calibration_video is not None:
+            self.set_lens_calibration(calibration_video, plot=False)
         if bbox is not None:
             self.bbox = bbox
         if window_size is not None:
             self.window_size = window_size
         # override the transform and bbox with the set corners
         if corners is not None:
             self.set_bbox_from_corners(corners)
+        if stabilize is not None:
+            self.stabilize = stabilize
 
     @property
     def bbox(self):
         """
         Returns geographical bbox fitting around corners points of area of interest in camera perspective
 
         Returns
@@ -147,49 +163,118 @@
     def dist_coeffs(self):
         return self._dist_coeffs
 
     @dist_coeffs.setter
     def dist_coeffs(self, dist_coeffs):
         self._dist_coeffs = dist_coeffs.tolist() if isinstance(dist_coeffs, np.ndarray) else dist_coeffs
 
+
     @property
-    def gcp_reduced(self):
+    def gcps_dest(self):
+        """
+
+        Returns
+        -------
+        dst : np.ndarray
+            destination coordinates of ground control point. z-coordinates are parsed from z_0 if necessary
+        """
+        if hasattr(self, "gcps"):
+            if "dst" in self.gcps:
+                return np.array(self.gcps["dst"] if len(self.gcps["dst"][0]) == 3 else np.c_[self.gcps["dst"], np.ones(4)*self.gcps["z_0"]])
+        # if conditions are not yet met, then return None
+        return None
+
+    @property
+    def gcps_dest_bbox(self):
+        """
+
+        Returns
+        -------
+        dst : np.ndarray
+            Destination coordinates measured as column, row in the intended bounding box with the intended resolution
+        """
+        return np.array(cv.transform_to_bbox(self.gcps_dest, self.bbox, self.resolution))
+
+
+    @property
+    def gcps_bbox_reduced(self):
+        """
+
+        Returns
+        -------
+        dst : np.ndarray
+            Destination coordinates in col, row in the intended bounding box, reduced with their mean coordinate
+
+        """
+        return self.gcps_dest_bbox - self.gcps_dest_bbox.mean(axis=0)
+    @property
+    def gcps_reduced(self):
         """
         Get the location of gcp destination points, reduced with their mean for better local projection
 
         Returns
         -------
-        gcp_reduced : np.ndarray
+        dst : np.ndarray
             Reduced coordinate (x, y) or (x, y, z) of gcp destination points
         """
-        return np.array(self.gcps["dst"]) - self.gcp_mean
+        return np.array(self.gcps_dest - self.gcps_mean)
 
     @property
-    def gcp_mean(self):
+    def gcps_mean(self):
         """
         Get the mean location of gcp destination points
 
         Returns
         -------
-        gcp_mean : np.ndarray
+        dst_mean : np.ndarray
             mean coordinate (x, y) or (x, y, z) of gcp destination points
         """
-        return np.array(self.gcps["dst"]).mean(axis=0)
+        return np.array(self.gcps_dest).mean(axis=0)
 
     @property
-    def gcp_dims(self):
+    def gcps_dims(self):
         """
 
         Returns
         -------
         dims : int
             amount of dimensions of gcps (can be 2 or 3)
 
         """
-        return len(self.gcps["dst"][0])
+        return len(self.gcps["dst"][0]) if hasattr(self, "gcps") else None
+
+    @property
+    def is_nadir(self):
+        """
+        Returns if the camera configuration belongs to nadir video
+
+        Returns
+        -------
+        is_nadir : bool
+            False if not nadir, True if nadir
+
+        """
+        return self._is_nadir
+
+    @is_nadir.setter
+    def is_nadir(
+            self,
+            nadir_prop: bool
+    ):
+        self._is_nadir = nadir_prop
+
+    @property
+    def pnp(self):
+        return cv.solvepnp(
+            self.gcps_reduced,
+            self.gcps["src"],
+            self.camera_matrix,
+            self.dist_coeffs
+        )
+
 
     @property
     def shape(self):
         """
         Returns rows and columns in projected frames from ``Frames.project``
 
         Returns
@@ -203,32 +288,51 @@
             self.bbox,
             resolution=self.resolution,
             round=1
         )
         return rows, cols
 
     @property
+    def stabilize(self):
+        """
+        Return stabilization polygon (anything outside is used for stabilization
+
+        Returns
+        -------
+        coords : list of lists
+            coordinates in original image frame comprising the polygon for use in stabilization
+        """
+        return self._stabilize
+
+    @stabilize.setter
+    def stabilize(
+            self,
+            coords: List[List[float]]
+    ):
+        self._stabilize = coords
+
+    @property
     def transform(self):
         """
         Returns Affine transform of projected frames from ``Frames.project``
 
         Returns
         -------
         transform : rasterio.transform.Affine object
 
         """
         return cv._get_transform(self.bbox, resolution=self.resolution)
 
     def set_lens_calibration(
         self,
-        fn,
-        chessboard_size=(9, 6),
-        max_imgs=30,
-        plot=True,
-        progress_bar=True,
+        fn: str,
+        chessboard_size: Optional[Tuple] = (9, 6),
+        max_imgs: Optional[int] = 30,
+        plot: Optional[bool] = True,
+        progress_bar: Optional[bool] = True,
         **kwargs
     ):
         """
         Calibrates and sets the properties ``camera_matrix`` and ``dist_coeffs`` using a video of a chessboard pattern.
         Follows methods described on https://docs.opencv.org/4.x/dc/dbb/tutorial_py_calibration.html
 
         Parameters
@@ -261,58 +365,66 @@
             plot,
             progress_bar,
             **kwargs
         )
         self.camera_matrix = camera_matrix
         self.dist_coeffs = dist_coeffs
 
-    def get_bbox(self, camera=False, h_a=None, redistort=False):
+    def get_bbox(
+            self,
+            camera: Optional[bool] = False,
+            h_a: Optional[float] = None,
+            redistort: Optional[bool] = False
+    ) -> Polygon:
         """
 
         Parameters
         ----------
         camera : bool, optional
             If set, the bounding box will be returned as row and column coordinates in the camera perspective.
             In this case ``h_a`` may be set to provide the right water level, to estimate the bounding box for.
         h_a : float, optional
             If set with ``camera=True``, then the bbox coordinates will be transformed to the camera perspective,
             using h_a as a present water level. In case a video with higher (lower) water levels is used, this
             will result in a different perspective plane than the control video.
         redistort : bool, optional
             If set in combination with ``camera``, the bbox will be redistorted in the camera objective using the
             distortion coefficients and camera matrix. Not used in orthorectification because this occurs by default
-            on already undistorted images.
+            on already undistorted images. Typically only used for plotting purposes on original frames.
 
         Returns
         -------
         A bounding box, that in the used CRS is perfectly rectangular, and aligned in the up/downstream direction.
         It can (and certainly will) be rotated with respect to a typical bbox with xlim, ylim coordinates.
         If user sets ``camera=True`` then the geographical bounding box will be converted into a camera perspective,
         using the homography belonging to the available ground control points and current water level.
 
         This can then be used to reconstruct the grid for velocimetry calculations.
         """
         bbox = self.bbox
         if camera:
             coords = np.array(bbox.exterior.coords)
-            # convert to perspective rowcol coordinates
-            M = self.get_M(reverse=True, h_a=h_a)
-            # reduce coords by control point mean
-            coords -= self.gcp_mean[0:2]
-            # TODO: re-distort if needed
-            corners = cv2.perspectiveTransform(np.float32([coords]), M)[0]
+            z_a = self.get_z_a(h_a)
             if redistort:
-                # for visualization on still distorted frames this can be done. DO NOT do this if used for
-                # orthorectification, as this typically occurs on undistorted images.
-                corners = cv.undistort_points(corners, self.camera_matrix, self.dist_coeffs, reverse=True)
-
+                # typically only done for plotting on original frame, expand number of points to be able to see distortion
+                coords_expand = np.zeros((0, 2))
+                for n in range(0, len(coords)-1):
+                    new_coords = np.linspace(coords[n], coords[n + 1], 100)
+                    coords_expand = np.r_[coords_expand, new_coords]
+                coords = coords_expand
+            coords = np.c_[coords, np.ones(len(coords))*z_a]
+            corners = self.project_points(coords)
             bbox = Polygon(corners)
         return bbox
 
-    def get_depth(self, z, h_a=None):
+    def get_depth(
+            self,
+            z: List[float],
+            h_a: Optional[float] = None
+    ) -> List[float]:
         """
         Retrieve depth for measured bathymetry points using the camera configuration and an actual water level,
         measured in local reference (e.g. staff gauge).
 
         Parameters
         ----------
         z : list of floats
@@ -327,42 +439,22 @@
 
         """
         if h_a is None:
             h_a = self.gcps["h_ref"]
         z_pressure = np.maximum(self.gcps["z_0"] - self.gcps["h_ref"] + h_a, z)
         return z_pressure - z
 
-    def get_dst_a(self, h_a=None):
-        """
-        h_a : float, optional
-            actual water level measured [m], if not set, assumption is that a single video
-            is processed and thus changes in water level are not relevant. (default: None)
-
-        Returns
-        -------
-        Actual locations of control points (in case these are only x, y) given the current set water level and
-        the camera location
-        """
-        # map where the destination points are with the actual water level h_a.
-        if h_a is None or h_a == self.gcps["h_ref"]:
-            # fill in the same value for h_ref and h_a
-            dst_a = self.gcps["dst"]
-        else:
-            h_ref = self.gcps["h_ref"]
-            lens_position = self.lens_position
-            dst_a = cv._get_gcps_a(
-                lens_position,
-                h_a,
-                self.gcps["dst"],
-                self.gcps["z_0"],
-                h_ref,
-            )
-        return dst_a
 
-    def get_dist_shore(self, x, y, z, h_a=None):
+    def get_dist_shore(
+            self,
+            x: List[float],
+            y: List[float],
+            z: List[float],
+            h_a: Optional[float] = None
+    ) -> List[float]:
         """
         Retrieve depth for measured bathymetry points using the camera configuration and an actual water level, measured
         in local reference (e.g. staff gauge).
 
         Parameters
         ----------
         x : list of floats
@@ -391,21 +483,51 @@
             # h_ref = self.gcps["h_ref"]
         z_dry = depth <= 0
         z_dry[[0, -1]] = True
         # compute distance to nearest dry points with Pythagoras
         dist_shore = np.array([(((x[z_dry] - _x) ** 2 + (y[z_dry] - _y) ** 2) ** 0.5).min() for _x, _y, in zip(x, y)])
         return dist_shore
 
-    def get_dist_wall(self, x, y, z, h_a=None):
+    def get_dist_wall(
+            self,
+            x: List[float],
+            y: List[float],
+            z: List[float],
+            h_a: Optional[float] = None
+    ) -> List[float]:
+        """
+        Retrieve distance to wall for measured bathymetry points using the camera configuration and an actual water
+        level, measured in local reference (e.g. staff gauge).
+
+        Parameters
+        ----------
+        x : list of floats
+            measured bathymetry point x-coordinates
+        y : list of floats
+            measured bathymetry point y-coordinates
+        z : list of floats
+            measured bathymetry point depths
+        h_a : float, optional
+            actual water level measured [m], if not set, assumption is that a single video
+            is processed and thus changes in water level are not relevant. (default: None)
+
+        Returns
+        -------
+        distance : list of floats
+
+        """
         depth = self.get_depth(z, h_a=h_a)
         dist_shore = self.get_dist_shore(x, y, z, h_a=h_a)
         dist_wall = (dist_shore**2 + depth**2)**0.5
         return dist_wall
 
-    def z_to_h(self, z):
+    def z_to_h(
+            self,
+            z: float
+    ) -> float:
         """Convert z coordinates of bathymetry to height coordinates in local reference (e.g. staff gauge)
 
         Parameters
         ----------
         z : float
             measured bathymetry point
 
@@ -413,15 +535,20 @@
         -------
         h : float
         """
         h_ref = 0 if self.gcps["h_ref"] is None else self.gcps["h_ref"]
         h = z + h_ref - self.gcps["z_0"]
         return h
 
-    def get_M(self, h_a=None, to_bbox_grid=False, reverse=False):
+    def get_M(
+            self,
+            h_a: Optional[float] = None,
+            to_bbox_grid: Optional[bool] = False,
+            reverse: Optional[bool] = False
+    ) -> np.ndarray:
         """Establish a transformation matrix for a certain actual water level `h_a`. This is done by mapping where the
         ground control points, measured at `h_ref` will end up with new water level `h_a`, given the lens position.
 
         Parameters
         ----------
         h_a : float, optional
             actual water level [m] (Default: None)
@@ -435,50 +562,36 @@
         -------
         M : np.ndarray
             2x3 transformation matrix
 
         """
         src = cv.undistort_points(self.gcps["src"], self.camera_matrix, self.dist_coeffs)
         if to_bbox_grid:
-            # lookup where the destination points are in row/column space
-            # dst_a is the destination point locations position with the actual water level
-            dst_a = cv.transform_to_bbox(
-                self.get_dst_a(h_a),
-                self.bbox,
-                self.resolution
-            )
-            dst_a = np.array(dst_a)
+            dst_a = self.gcps_bbox_reduced
         else:
-            # in case we are dealing with a 2D 4-point, then reproject points on water surface, else keep 3D points
-            dst_a = self.get_dst_a(h_a) if self.gcp_dims == 2 else self.gcps["dst"]
-            # reduce dst_a with its mean to get much more accurate projection result in case x and y order of
-            # magnitude is very large
-            dst_a -= self.gcp_mean
-        # src_a = self.get_src(**lens_pars)
-        if dst_a.shape[-1] == 3:
-            # compute the water level in the coordinate system reduced with the mean gcp coordinate
-            z_a = self.get_z_a(h_a)
-            z_a -= self.gcp_mean[-1]
-            # treating 3D homography
-            return cv.get_M_3D(
-                src=src,
-                dst=dst_a,
-                camera_matrix=self.camera_matrix,
-                dist_coeffs=self.dist_coeffs,
-                z=z_a,
-                reverse=reverse
-            )
-        else:
-            return cv.get_M_2D(
-                src=src,
-                dst=dst_a,
-                reverse=reverse
-            )
+            dst_a = self.gcps_reduced
+        # compute the water level in the coordinate system reduced with the mean gcp coordinate
+        z_a = self.get_z_a(h_a)
+        z_a -= self.gcps_mean[-1]
+        # treating 3D homography
+        print(dst_a)
+        # print(z_a)
+        return cv.get_M_3D(
+            src=src,
+            dst=dst_a,
+            camera_matrix=self.camera_matrix,
+            dist_coeffs=cv.DIST_COEFFS, # self.dist_coeffs,
+            z=z_a,
+            reverse=reverse
+        )
 
-    def get_z_a(self, h_a=None):
+    def get_z_a(
+            self,
+            h_a: Optional[float] = None
+    ) -> float:
         """
         h_a : float, optional
             actual water level measured [m], if not set, assumption is that a single video
             is processed and thus changes in water level are not relevant. (default: None)
 
         Returns
         -------
@@ -486,42 +599,75 @@
         the camera location
         """
         if h_a is None:
             return self.gcps["z_0"]
         else:
             return self.gcps["z_0"] + (h_a - self.gcps["h_ref"])
 
-    def set_bbox_from_corners(self, corners):
+    def set_bbox_from_corners(
+            self,
+            corners: List[List[float]]
+    ):
         """
         Establish bbox based on a set of camera perspective corner points Assign corner coordinates to camera
         configuration
 
         Parameters
         ----------
         corners : list of lists (4)
-            [columns, row] coordinates in camera perspective
+            [columns, row] coordinates in original camera perspective without any undistortion applied
 
         """
         assert (np.array(corners).shape == (4,
                                             2)), f"a list of lists of 4 coordinates must be given, resulting in (4, " \
                                                  f"2) shape. Current shape is {corners.shape} "
 
-        # get homography, this is the only place besides self.get_M where cv.get_M is used.
-        M_gcp = self.get_M()
-        # TODO: make derivation dependent on 3D or 2D point availability
-        # if self.gcps["src"].shape == 3:
-        #     # TODO: homography from solvepnp
-        bbox = cv.get_aoi(M_gcp, corners, resolution=self.resolution)
-        # bbox is offset by self.gcp_mean. Regenerate bbox after adding offset
-        bbox_xy = np.array(bbox.exterior.coords)
-        bbox_xy += self.gcp_mean[0:2]
-        bbox = Polygon(bbox_xy)
+        # get homography
+        corners_xyz = self.unproject_points(corners, np.ones(4)*self.gcps["z_0"])
+        bbox = cv.get_aoi(
+            corners_xyz,
+            resolution=self.resolution
+        )
         self.bbox = bbox
 
-    def set_lens_pars(self, k1=0, c=2, f=4):
+
+    def set_intrinsic(
+            self,
+            camera_matrix: Optional[List[List]] = None,
+            dist_coeffs: Optional[List[List]] = None,
+            lens_pars: Optional[Dict[str, float]] = None
+    ):
+        # first set a default estimate from pose if 3D gcps are available
+        self.set_lens_pars()  # default parameters use width of frame
+        if hasattr(self, "gcps"):
+            if len(self.gcps["src"]) >= 4:
+            # if self.gcp_dims == 3:
+                self.camera_matrix, self.dist_coeffs, err = cv.optimize_intrinsic(
+                    self.gcps["src"],
+                    self.gcps_dest,
+                    # self.gcps["dst"],
+                    self.height,
+                    self.width,
+                    lens_position=self.lens_position
+                )
+            if lens_pars is not None:
+                # override with lens parameter set by user
+                self.set_lens_pars(**lens_pars)
+            if camera_matrix is not None and dist_coeffs is not None:
+                # override with
+                self.camera_matrix = camera_matrix
+                self.dist_coeffs = dist_coeffs
+
+
+    def set_lens_pars(
+            self,
+            k1: Optional[float] = 0.,
+            c: Optional[float] = 2.,
+            focal_length: Optional[float] = None
+    ):
         """Set the lens parameters of the given CameraConfig
 
         Parameters
         ----------
         k1 : float, optional
             lens curvature [-], zero (default) means no curvature
         c : float, optional
@@ -529,28 +675,36 @@
             centre.
         f : float, optional
             focal length [mm], typical values could be 2.8, or 4 (default).
 
 
         """
         assert (isinstance(k1, (int, float))), "k1 must be a float"
-        assert (isinstance(c, (int, float))), "k1 must be a float"
-        assert (isinstance(f, (int, float))), "k1 must be a float"
+        assert (isinstance(c, (int, float))), "c must be a float"
+        if focal_length is not None:
+            assert (isinstance(focal_length, (int, float, None))), "f must be a float"
         self.dist_coeffs = cv._get_dist_coefs(k1)
-        self.camera_matrix = cv._get_cam_mtx(self.height, self.width, c=c, f=f)
+        self.camera_matrix = cv._get_cam_mtx(self.height, self.width, c=c, focal_length=focal_length)
 
-    def set_gcps(self, src, dst, z_0, h_ref=None, crs=None):
+    def set_gcps(
+            self,
+            src: List[List],
+            dst: List[List],
+            z_0: float,
+            h_ref: Optional[float] = None,
+            crs: Optional[Any] = None
+    ):
         """
         Set ground control points for the given CameraConfig
 
         Parameters
         ----------
-        src : list of lists (4 or 6+)
+        src : list of lists (2, 4 or 6+)
             [x, y] pairs of columns and rows in the frames of the original video
-        dst : list of lists (4 or 6+)
+        dst : list of lists (2, 4 or 6+)
             [x, y] or [x, y, z] pairs of real world coordinates in the given coordinate reference system.
         z_0 : float
             Water level measured in global reference system such as a geoid or ellipsoid used
             by a GPS device. All other surveyed points (lens position and cross section) must have the same vertical
             reference.
         h_ref :  float, optional
             Water level, belonging to the 4 control points in `dst`. This is the water level
@@ -586,25 +740,32 @@
                     'CameraConfig does not contain a crs, so gcps also cannot contain a crs. Ensure that the provided '
                     'destination coordinates are in a locally defined coordinate reference system, e.g. established '
                     'with a spirit level.')
             dst = helpers.xyz_transform(dst, crs, CRS.from_wkt(self.crs))
         # if there is no h_ref, then no local gauge system, so set h_ref to zero
         # check if 2 points are available
         if len(src) == 2:
+            self.is_nadir = True
             src, dst = cv._get_gcps_2_4(src, dst, self.width, self.height)
         if h_ref is None:
             h_ref = 0.
         self.gcps = {
             "src": src,
             "dst": dst,
             "h_ref": h_ref,
             "z_0": z_0,
         }
 
-    def set_lens_position(self, x, y, z, crs=None):
+    def set_lens_position(
+            self,
+            x: float,
+            y: float,
+            z: float,
+            crs: Optional[Any] = None
+    ):
         """Set the geographical position of the lens of current CameraConfig.
 
         Parameters
         ----------
         x : float
             x-coordinate
         y : float
@@ -619,24 +780,88 @@
 
         if crs is not None:
             if self.crs is None:
                 raise ValueError("CameraConfig does not contain a crs, ")
             x, y = helpers.xyz_transform([[x, y]], crs, self.crs)[0]
         self.lens_position = [x, y, z]
 
+    def project_points(
+            self,
+            points: List[List]
+    ) -> np.ndarray:
+        """
+        Project real world x, y, z coordinates into col, row coordinates on image
+
+        Parameters
+        ----------
+        points : list of lists or array-like
+            list of points [x, y, z] in real world coordinates
+
+        Returns
+        -------
+        points_project : list or array-like
+            list of points (equal in length as points) with [col, row] coordinates
+        """
+        _, rvec, tvec = self.pnp
+        # normalize points wrt mean of gcps
+        points = np.float32(np.array(points) - self.gcps_mean)
+        points_proj, jacobian = cv2.projectPoints(
+            points,
+            rvec,
+            tvec,
+            np.array(self.camera_matrix),
+            np.array(self.dist_coeffs)
+        )
+        points_proj = np.array([list(point[0]) for point in points_proj])
+        return points_proj
+
+
+    def unproject_points(
+            self,
+            points: List[List],
+            zs: List[float]
+    ) -> np.ndarray:
+        """
+        Reverse projects points in [column, row] space to [x, y, z] real world
+        Parameters
+        ----------
+        points : List of lists or array-like
+            Points in [col, row] to unproject
+        zs : float or list of floats : z-coordinate on which to unproject points
+
+        Returns
+        -------
+        points_unproject : List of lists or array-like
+            unprojected points as list of [x, y, z] coordinates
+        """
+        _, rvec, tvec = self.pnp
+        # reduce zs by the mean of the gcps
+        _zs = np.atleast_1d(zs) - self.gcps_mean[-1]
+        dst = cv.unproject_points(
+            np.array(points),
+            _zs,
+            rvec=rvec,
+            tvec=tvec,
+            camera_matrix=self.camera_matrix,
+            dist_coeffs=self.dist_coeffs
+        )
+        dst = np.array(dst) + self.gcps_mean
+        return dst
+
+
     def plot(
             self,
-            figsize=(13, 8),
-            ax=None,
-            tiles=None,
-            buffer=0.0005,
-            zoom_level=19,
-            camera=False,
-            tiles_kwargs={}
-    ):
+            figsize: Optional[Tuple] = (13, 8),
+            ax: Optional[plt.Axes] = None,
+            tiles: Optional[Any] = None,
+            buffer: Optional[float] = 0.0005,
+            zoom_level: Optional[int] = 19,
+            camera: Optional[bool] = False,
+            tiles_kwargs: Optional[Dict] = {}
+    ) -> plt.Axes:
         """
         Plot the geographical situation of the CameraConfig. This is very useful to check if the CameraConfig seems
         to be in the right location. Requires cartopy to be installed.
 
         Parameters
         ----------
         figsize : tuple, optional
@@ -670,15 +895,17 @@
         # prepare points for plotting
         if camera:
             points = [Point(x, y) for x, y in self.gcps["src"]]
         else:
             points = [Point(p[0], p[1]) for p in self.gcps["dst"]]
 
         if not camera:
-            if hasattr(self, "lens_position") and not camera:
+            if self.lens_position is not None and not camera:
+            #
+            # if hasattr(self, "lens_position") and not camera:
                 points.append(Point(self.lens_position[0], self.lens_position[1]))
             # transform points in case a crs is provided
             if hasattr(self, "crs"):
                 # make a transformer to lat lon
                 transformer = Transformer.from_crs(
                     CRS.from_user_input(self.crs),
                     CRS.from_epsg(4326),
@@ -736,15 +963,23 @@
             ax.set_aspect("equal")
             if xlim is not None:
                 ax.set_xlim(xlim)
                 ax.set_ylim(ylim)
         ax.legend()
         return ax
 
-    def plot_bbox(self, ax=None, camera=False, transformer=None, h_a=None, **kwargs):
+    def plot_bbox(
+            self,
+            ax: Optional[plt.Axes] = None,
+            camera: Optional[bool] = False,
+            transformer: Optional[Any] = None,
+            h_a: Optional[float] = None,
+            redistort: Optional[bool] = True,
+            **kwargs
+    ):
         """
         Plot bounding box for orthorectification in a geographical projection (``camera=False``) or the camera
         Field Of View (``camera=True``).
 
         Parameters
         ----------
         ax : plt.axes, optional
@@ -759,29 +994,30 @@
             will result in a different perspective plane than the control video.
 
         Returns
         -------
         p : matplotlib.patch mappable
         """
         # collect information to plot
-        bbox = self.get_bbox(camera=camera, h_a=h_a)
+        bbox = self.get_bbox(camera=camera, h_a=h_a, redistort=redistort)
         if camera is False and transformer is not None:
             # geographical projection is needed
             bbox = ops.transform(transformer, bbox)
 
         bbox_x, bbox_y = bbox.exterior.xy
         bbox_coords = list(zip(bbox_x, bbox_y))
         patch = patches.Polygon(
             bbox_coords,
             **kwargs
         )
         p = ax.add_patch(patch)
         return p
 
-    def to_dict(self):
+
+    def to_dict(self) -> Dict:
         """Return the CameraConfig object as dictionary
 
         Returns
         -------
         camera_config_dict : dict
             serialized CameraConfig
 
@@ -791,34 +1027,37 @@
         # replace underscore keys for keys without underscore
         for k in list(d.keys()):
             if k[0] == "_":
                 d[k[1:]] = d.pop(k)
 
         return d
 
-    def to_dict_str(self):
+    def to_dict_str(self) -> Dict:
         d = self.to_dict()
         # convert anything that is not string in string
         dict_str = {k: v if not(isinstance(v, Polygon)) else v.__str__() for k, v in d.items()}
         return dict_str
 
-    def to_file(self, fn):
+    def to_file(
+            self,
+            fn: str
+    ):
         """Write the CameraConfig object to json structure
         
         Parameters
         ----------
         fn : str
             Path to file to write camera config to
 
         """
 
         with open(fn, "w") as f:
             f.write(self.to_json())
 
-    def to_json(self):
+    def to_json(self) -> str:
         """Convert CameraConfig object to string
         
         Returns
         -------
         json_str : str
             json string with CameraConfig components
         """
@@ -834,15 +1073,17 @@
     "width": 1920,
     "crs": ....
     ...
 }
 """
 
 
-def get_camera_config(s):
+def get_camera_config(
+        s: str
+) -> CameraConfig:
     """Read camera config from string
 
     Parameters
     ----------
     s : str
         json string containing camera config
 
@@ -857,15 +1098,17 @@
     # ensure the bbox is a Polygon object
     if "bbox" in d:
         if isinstance(d["bbox"], str):
             d["bbox"] = wkt.loads(d["bbox"])
     return CameraConfig(**d)
 
 
-def load_camera_config(fn):
+def load_camera_config(
+        fn: str
+) -> CameraConfig:
     """Load a CameraConfig from a geojson file.
 
     Parameters
     ----------
     fn : str
         path to file with camera config in json format.
```

### Comparing `pyopenrivercam-0.4.3/pyorc/api/frames.py` & `pyopenrivercam-0.5.0/pyorc/api/frames.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,16 +58,17 @@
         # set an overlap if not provided in kwargs
         if not("overlap" in kwargs):
             kwargs["overlap"] = int(round(camera_config.window_size) / 2)
         # first get rid of coordinates that need to be recalculated
         coords_drop = list(set(self._obj.coords) - set(self._obj.dims))
         obj = self._obj.drop_vars(coords_drop)
         # get frames and shifted frames in time
-        frames1 = obj.shift(time=1)[1:]
-        frames2 = obj[1:]
+        frames1 = obj.shift(time=1)[1:].chunk({"time": 10})
+        frames2 = obj[1:].chunk({"time": 10})
+
         # get the cols and rows coordinates of the expected results
         cols, rows = piv_process.get_piv_size(
             image_size=frames1[0].shape,
             search_area_size=kwargs["search_area_size"],
             overlap=kwargs["overlap"]
         )
         # retrieve the x and y-axis belonging to the results
@@ -170,20 +171,22 @@
         """
         camera_config = copy.deepcopy(self.camera_config)
         if resolution is not None:
             camera_config.resolution = resolution
         # convert bounding box coords into row/column space
         shape = camera_config.shape
         # get camera perspective bbox corners
-        src = camera_config.get_bbox(camera=True, h_a=self.h_a).exterior.coords[0:4]
+        src = camera_config.get_bbox(
+            camera=True,
+            h_a=self.h_a
+        ).exterior.coords[0:4]
         dst_xy = camera_config.get_bbox().exterior.coords[0:4]
         # get geographic coordinates bbox corners
         dst = cv.transform_to_bbox(dst_xy, camera_config.bbox, camera_config.resolution)
         M = cv.get_M_2D(src, dst)
-
         # prepare all coordinates
         y = np.flipud(np.linspace(
             camera_config.resolution / 2,
             camera_config.resolution * (shape[0] - 0.5),
             shape[0])
         )
         x = np.linspace(
```

### Comparing `pyopenrivercam-0.4.3/pyorc/api/mask.py` & `pyopenrivercam-0.5.0/pyorc/api/mask.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.4.3/pyorc/api/orcbase.py` & `pyopenrivercam-0.5.0/pyorc/api/orcbase.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.4.3/pyorc/api/plot.py` & `pyopenrivercam-0.5.0/pyorc/api/plot.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.4.3/pyorc/api/transect.py` & `pyopenrivercam-0.5.0/pyorc/api/transect.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,19 +159,20 @@
         """Depth integrated velocity for quantiles of time series using a correction v_corr between surface velocity and
         depth-average velocity.
 
         Parameters
         ----------
         v_corr : float, optional
             correction factor (default: 0.9)
-        fill_method : method to fill missing values. "zeros" fills NaNS with zeros, "interpolate" interpolates values
+        fill_method : str, optional
+            method to fill missing values. "zeros" fills NaNS with zeros, "interpolate" interpolates values
             from nearest neighbour, "log_interp" interpolates values linearly with velocities scaled by the log of
-             depth over a roughness length, "log_fit" fits a 4-parameter logarithmic profile with depth and with
-             changing velocities towards banks on known velocities, and fills missing with the fitted relationship
-             (experimental) (Default value = "zeros").
+            depth over a roughness length, "log_fit" fits a 4-parameter logarithmic profile with depth and with
+            changing velocities towards banks on known velocities, and fills missing with the fitted relationship
+            (experimental) (Default value = "zeros").
 
         Returns
         -------
         ds : xr.Dataset
             Transect for selected quantiles in time, with "q_nofill" containing the integrated values, and "q" the
             integrated values, filled with chosen fill method.
```

### Comparing `pyopenrivercam-0.4.3/pyorc/api/video.py` & `pyopenrivercam-0.5.0/pyorc/api/video.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import os
 import warnings
 import xarray as xr
 
+from typing import List, Optional, Union
+
 from .. import cv, const
 from .cameraconfig import load_camera_config, get_camera_config, CameraConfig
 
 
-class Video:  #(cv2.VideoCapture)
+class Video:  # (cv2.VideoCapture)
     def __repr__(self):
         template = """
 Filename: {:s}
 FPS: {:f}
 start frame: {:d}
 end frame: {:d}
 Camera configuration: {:s}
@@ -30,22 +32,21 @@
             self.start_frame,
             self.end_frame,
             self.camera_config.__repr__() if hasattr(self, "camera_config") else "none"
         )
 
     def __init__(
             self,
-            fn,
-            camera_config=None,
-            h_a=None,
-            start_frame=None,
-            end_frame=None,
-            freq=1,
-            stabilize=None,
-            mask_exterior=None,
+            fn: str,
+            camera_config: Optional[Union[str, CameraConfig]] = None,
+            h_a: Optional[float] = None,
+            start_frame: Optional[int] = None,
+            end_frame: Optional[int] = None,
+            freq: Optional[int] = 1,
+            stabilize: Optional[List[List]] = None,
     ):
         """
         Video class, inheriting parts from cv2.VideoCapture. Contains a camera configuration to it, and a start and end
         frame to read from the video. Several methods read frames into memory or into a xr.DataArray with attributes.
         These can then be processed with other pyorc API functionalities.
 
         Parameters
@@ -59,52 +60,48 @@
         h_a : float, optional
             actual height [m], measured in local vertical reference during the video (e.g. a staff gauge in view of
             the camera)
         start_frame : int, optional
             first frame to use in analysis (default: 0)
         end_frame : int, optional
             last frame to use in analysis (if not set, last frame available in video will be used)
-        stabilize : optional
-            If set to a recipe name, the video will be stabilized by attempting to find rigid points and track these with
-            Lukas Kanade optical flow. Currently supported is "fixed" for FOV that is meant to be in one place.
-        mask_exterior : list of lists,
+        stabilize : list of lists, optional
             set of coordinates, that together encapsulate the polygon that defines the mask, separating land from water.
-            The mask is used to select region (on land) for rigid point search for stabilization.
+            The mask is used to select region (on land) for rigid point search for stabilization. If not set, then no
+            stabilization will be performed
         """
-        assert(isinstance(start_frame, (int, type(None)))), 'start_frame must be of type "int"'
-        assert(isinstance(end_frame, (int, type(None)))), 'end_frame must be of type "int"'
-        assert(stabilize in ["fixed", None]), f'stabilize is only implemented for method "fixed", "{stabilize}" given'
-        self.feats_pos = None
+        assert (isinstance(start_frame, (int, type(None)))), 'start_frame must be of type "int"'
+        assert (isinstance(end_frame, (int, type(None)))), 'end_frame must be of type "int"'
+        # assert (isinstance(stabilize, (list, type(None)))), f'stabilize must contain a list of points, but is {stabilize}'
         self.feats_stats = None
         self.feats_errs = None
         self.ms = None
         self.mask = None
         self.stabilize = stabilize
         if camera_config is not None:
             self.camera_config = camera_config
-        # if camera_config is not None:
+            # if camera_config is not None:
             # check if h_a is supplied, if so, then also z_0 and h_ref must be available
             if h_a is not None:
-                assert(isinstance(self.camera_config.gcps["z_0"], float)),\
+                assert (isinstance(self.camera_config.gcps["z_0"], float)), \
                     "h_a was supplied, but camera config's gcps do not contain z_0, this is needed for dynamic " \
                     "reprojection. You can supplying z_0 and h_ref in the camera_config's gcps upon making a camera " \
                     "configuration. "
-                assert (isinstance(self.camera_config.gcps["h_ref"], float)),\
+                assert (isinstance(self.camera_config.gcps["h_ref"], float)), \
                     "h_a was supplied, but camera config's gcps do not contain h_ref, this is needed for dynamic " \
                     "reprojection. You must supply z_0 and h_ref in the camera_config's gcps upon making a camera " \
                     "configuration. "
         cap = cv2.VideoCapture(fn)
         cap.set(cv2.CAP_PROP_ORIENTATION_AUTO, 180.0)
         self.height = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
         self.width = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
-        self.mask_exterior = mask_exterior
         # explicitly open file for reading
-        if mask_exterior is not None:
-            # set a mask based on the roi points
-            self.set_mask_from_exterior(mask_exterior)
+        if self.stabilize is not None:
+            # set a gridded mask based on the roi points
+            self.set_mask_from_exterior(self.stabilize)
         # set end and start frame
         self.frame_count = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
         if start_frame is not None:
             if (start_frame > self.frame_count and self.frame_count > 0):
                 raise ValueError("Start frame is larger than total amount of frames")
         else:
             start_frame = 0
@@ -141,33 +138,14 @@
         # make camera config part of the vidoe object
         self.fn = fn
         self._stills = {}  # here all stills are stored lazily
         # nothing to be done at this stage, release file for now.
         cap.release()
         del cap
 
-
-    @property
-    def mask_exterior(self):
-        """
-
-        Returns
-        -------
-        np.ndarray
-            Mask of region of interest
-        """
-        return self._mask_exterior
-
-    @mask_exterior.setter
-    def mask_exterior(self, mask_exterior):
-        if mask_exterior is None:
-            self._mask_exterior = None
-        else:
-            self._mask_exterior = mask_exterior
-
     @property
     def mask(self):
         """
 
         Returns
         -------
         np.ndarray
@@ -207,15 +185,16 @@
             elif isinstance(camera_config_input, CameraConfig):
                 # set CameraConfig as is
                 self._camera_config = camera_config_input
             elif isinstance(camera_config_input, dict):
                 # Create CameraConfig from dict
                 self._camera_config = CameraConfig(**camera_config_input)
         except:
-            raise IOError("Could not recognise input as a CameraConfig file, string, dictionary or CameraConfig object.")
+            raise IOError(
+                "Could not recognise input as a CameraConfig file, string, dictionary or CameraConfig object.")
 
     @property
     def end_frame(self):
         """
 
         :return: int, last frame considered in analysis
         """
@@ -242,184 +221,212 @@
 
     @freq.setter
     def freq(self, freq=1):
         self._freq = freq
 
     @property
     def stabilize(self):
-        """
-
-        :return: int, last frame considered in analysis
-        """
-        return self._stabilize
+        if self._stabilize is not None:
+            return self._stabilize
+        elif hasattr(self, "camera_config"):
+            if hasattr(self.camera_config, "stabilize"):
+                return self.camera_config.stabilize
 
     @stabilize.setter
-    def stabilize(self, stabilize=None):
-        # sometimes last frames are not read by OpenCV, hence we skip the last frame always
-        self._stabilize = stabilize
-
+    def stabilize(
+            self,
+            coords: Optional[List[List]] = None
+    ):
+        self._stabilize = coords
 
     @property
     def h_a(self):
         """
 
         :return: Actual water level [m] during video
         """
         return self._h_a
 
     @h_a.setter
-    def h_a(self, h_a):
+    def h_a(
+            self,
+            h_a: float
+    ):
         if h_a is not None:
-            assert(isinstance(h_a, float)), f"The actual water level must be a float, you supplied a {type(h_a)}"
+            assert (isinstance(h_a, float)), f"The actual water level must be a float, you supplied a {type(h_a)}"
             if h_a < 0:
-                warnings.warn("Water level is negative. This can be correct, but may be unlikely, especially if you use a staff gauge.")
+                warnings.warn(
+                    "Water level is negative. This can be correct, but may be unlikely, especially if you use a staff gauge.")
         self._h_a = h_a
 
     @property
     def start_frame(self):
         """
 
         :return: int, first frame considered in analysis
         """
         return self._start_frame
 
     @start_frame.setter
-    def start_frame(self, start_frame=None):
+    def start_frame(
+            self,
+            start_frame: Optional[int] = None
+    ):
         if start_frame is None:
             self._start_frame = 0
         else:
             self._start_frame = start_frame
 
     @property
     def fps(self):
         """
 
         :return: float, frames per second
         """
         return self._fps
 
     @fps.setter
-    def fps(self, fps):
+    def fps(
+            self,
+            fps: float
+    ):
         if (np.isinf(fps)) or (fps <= 0):
             raise ValueError(f"FPS in video is {fps} which is not a valid value. Repair the video file before use")
         self._fps = fps
 
     @property
     def corners(self):
         """
 
         :return: list of 4 lists (int) with [column, row] locations of area of interest in video objective
         """
         return self._corners
 
     @corners.setter
-    def corners(self, corners):
+    def corners(
+            self,
+            corners: List[List]
+    ):
         self._corners = corners
 
-
     @property
     def rotation(self):
         return self._rotation
 
     @rotation.setter
-    def rotation(self, rotation_code):
+    def rotation(
+            self,
+            rotation_code: int
+    ):
         """
         Solves a likely bug in OpenCV (4.6.0) that straight up videos rotate in the wrong direction. Tested for both
         90 degree and 270 degrees rotation videos on several smartphone (iPhone and Android)
         """
         if rotation_code in [90, 270]:
             self._rotation = cv2.ROTATE_180
         else:
             self._rotation = None
 
-
-
-    def get_frame(self, n, method="grayscale", lens_corr=False):
+    def get_frame(
+            self,
+            n: int,
+            method: Optional[str] = "grayscale",
+            lens_corr: Optional[bool] = False
+    ) -> np.ndarray:
         """
         Retrieve one frame. Frame will be corrected for lens distortion if lens parameters are given.
 
-        :param n: int, frame number to retrieve
-        :param method: str, can be "rgb", "grayscale", or "hsv", default: "grayscale"
-        :param lens_corr: bool, optional, if set to True, lens parameters will be used to undistort image
-        :return: np.ndarray containing frame
-        """
-        assert(n >= 0), "frame number cannot be negative"
-        assert(n - self.start_frame <= self.end_frame - self.start_frame), "frame number is larger than the different between the start and end frame"
-        assert(method in ["grayscale", "rgb", "hsv"]), f'method must be "grayscale", "rgb" or "hsv", method is "{method}"'
+        Parameters:
+        -----------
+        n : int
+            frame number to retrieve
+        method : str
+            can be "rgb", "grayscale", or "hsv", default: "grayscale"
+        lens_corr: bool, optional
+            if set to True, lens parameters will be used to undistort image
+
+        Returns
+        -------
+        frame : np.ndarray
+            2d array (grayscale) or 3d (rgb/hsv) with frame
+        """
+        assert (n >= 0), "frame number cannot be negative"
+        assert (
+                n - self.start_frame <= self.end_frame - self.start_frame), "frame number is larger than the different between the start and end frame"
+        assert (method in ["grayscale", "rgb",
+                           "hsv"]), f'method must be "grayscale", "rgb" or "hsv", method is "{method}"'
         cap = cv2.VideoCapture(self.fn)
         cap.set(cv2.CAP_PROP_POS_FRAMES, n + self.start_frame)
         try:
             ret, img = cap.read()
             if self.rotation is not None:
                 img = cv2.rotate(img, self.rotation)
         except:
             raise IOError(f"Cannot read")
         if ret:
             if self.ms is not None:
-                # correct for stabilization
-                h = img.shape[0]
-                w = img.shape[1]
-                img = cv2.warpAffine(img, self.ms[n], (w, h))
-
-            # if lens_corr:
-            #     if self.camera_config.lens_pars is not None:
+                img = cv.transform(img, self.ms[n])
             # apply lens distortion correction
             if hasattr(self, "camera_config"):
                 img = cv.undistort_img(img, self.camera_config.camera_matrix, self.camera_config.dist_coeffs)
             if method == "grayscale":
                 # apply gray scaling, contrast- and gamma correction
                 # img = _corr_color(img, alpha=None, beta=None, gamma=0.4)
-                img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY) #  mean(axis=2)
+                img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)  # mean(axis=2)
             elif method == "rgb":
                 # turn bgr to rgb for plotting purposes
                 img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
             elif method == "hsv":
                 img = cv2.cvtColor(img, cv2.COLOR_BGR2HSV)
         self.frame_count = n + 1
         cap.set(cv2.CAP_PROP_POS_FRAMES, 0)
         cap.release()
         return img
 
-    def get_frames(self, **kwargs):
+    def get_frames(
+            self,
+            **kwargs
+    ) -> xr.DataArray:
         """
         Get a xr.DataArray, containing a dask array of frames, from `start_frame` until `end_frame`, expected to be read
         lazily. The xr.DataArray will contain all coordinate variables and attributes, needed for further processing
         steps.
 
-        :param kwargs: dict, keyword arguments to pass to `get_frame`. Currently only `grayscale` is supported.
-        :return: xr.DataArray, containing all requested frames
+        Parameters
+        ----------
+        **kwargs: dict, optional
+            keyword arguments to pass to `get_frame`. Currently only `grayscale` is supported.
+
+        Returns
+        -------
+        frames : xr.DataArray
+            containing all requested frames
         """
-        assert(hasattr(self, "_camera_config")), "No camera configuration is set, add it to the video using the .camera_config method"
+        assert (hasattr(self,
+                        "_camera_config")), "No camera configuration is set, add it to the video using the .camera_config method"
         # camera_config may be altered for the frames object, so copy below
         camera_config = copy.deepcopy(self.camera_config)
         get_frame = dask.delayed(self.get_frame, pure=True)  # Lazy version of get_frame
         # get all listed frames
         frames = [get_frame(n=n, **kwargs) for n, f_number in enumerate(self.frame_number)]
         sample = frames[0].compute()
         data_array = [da.from_delayed(
             frame,
             dtype=sample.dtype,
             shape=sample.shape
         ) for frame in frames]
-        # if "lens_corr" in kwargs:
-        #     if kwargs["lens_corr"]:
-                # also correct the control point src
+        # undistort source control points
         if hasattr(camera_config, "gcps"):
             camera_config.gcps["src"] = cv.undistort_points(
                 camera_config.gcps["src"],
                 camera_config.camera_matrix,
                 camera_config.dist_coeffs,
             )
-                # camera_config.corners = cv.undistort_points(
-                #     camera_config.corners,
-                #     sample.shape[0],
-                #     sample.shape[1],
-                #     **self.camera_config.lens_pars
-                # )
-        time = np.array(self.time) * 0.001 # measure in seconds to comply with CF conventions # np.arange(len(data_array))*1/self.fps
+        time = np.array(
+            self.time) * 0.001  # measure in seconds to comply with CF conventions # np.arange(len(data_array))*1/self.fps
         # y needs to be flipped up down to match the order of rows followed by coordinate systems (bottom to top)
         y = np.flipud(np.arange(data_array[0].shape[0]))
         x = np.arange(data_array[0].shape[1])
         # perspective column and row coordinate grids
         xp, yp = np.meshgrid(x, y)
         coords = {
             "time": time,
@@ -445,75 +452,46 @@
         if len(sample.shape) == 3:
             del coords["rgb"]
         # add coordinate grids (i.e. without time)
         frames = frames.frames._add_xy_coords([xp, yp], coords, const.PERSPECTIVE_ATTRS)
         frames.name = "frames"
         return frames
 
+    def set_mask_from_exterior(
+            self,
+            exterior
+    ):
+        """
+        Prepare a mask grid with 255 outside of the stabilization polygon and 0 inside
+
+        Parameters
+        ----------
+        exterior : list of lists
+            coordinates defining the polygon for masking
+
+        Returns
+        -------
+        self.mask : np.ndarray
+            mask for stabilization region
 
-    def set_mask_from_exterior(self, exterior):
+        """
         mask_coords = np.array([exterior], dtype=np.int32)
         mask = np.zeros((self.height, self.width), np.uint8)
         mask = cv2.fillPoly(mask, [mask_coords], 255)
-        mask[mask==0] = 1
-        mask[mask==255] = 0
-        mask[mask==1] = 255
+        mask[mask == 0] = 1
+        mask[mask == 255] = 0
+        mask[mask == 1] = 255
         self.mask = mask
 
-
-    def _get_pos_feats(self, cap, split=2, recipe=const.CLASSIFY_STANDING_CAM):
-        # go through the entire set of frames to gather transformation matrices per frame (except for the first one)
-        # get the displacements of trackable features
-        positions, stats, errs = cv._get_displacements(
-            cap,
-            start_frame=self.start_frame,
-            end_frame=self.end_frame,
-            split=split,
-            mask=self.mask
-        )
-        # filter features that belong to actual camera movement
-        for recipe in recipe:
-            classes = cv._classify_displacements(positions, **recipe)
-            # select positions which are classified as water
-            positions = positions[:, classes, :]
-            stats = stats[:, classes]
-        self.feats_pos = positions
-        self.feats_stats = stats
-        self.feats_errs = errs
-
-
-    def get_ms(self, cap, split=2):
+    def get_ms(
+            self,
+            cap: cv2.VideoCapture,
+            split: Optional[int] = 2
+    ):
         self.ms = cv._get_ms_gftt(
             cap,
             start_frame=self.start_frame,
             end_frame=self.end_frame,
             split=split,
             mask=self.mask,
         )
-    # def _get_ms(self):
-    #     # retrieve the transformation matrices for stabilization
-    #     self.ms = cv._ms_from_displacements(self.feats_pos, self.feats_stats)
-
-
-    def plot_rigid_pts(self, ax=None, **kwargs):
-        """
-        Plots found rigid points (column, row) for stabilization and their path throughout the frames in time on an
-        axes object.
 
-
-        Parameters
-        ----------
-        ax : plt.axes object, optional
-            If None (default), use the current axes.
-        **kwargs : additional keyword arguments to `matplotlib.pyplot.scatter` wrapped Matplotlib function.
-
-
-        Returns
-        -------
-
-        """
-        assert self.feats_pos is not None, "No stabilization applied hence no rigid points available to plot"
-        if ax is None:
-            ax = plt.axes()
-        for t_p in np.swapaxes(self.feats_pos, 0, 1):
-            p = ax.scatter(t_p[:, 0], t_p[:, 1], c=np.linspace(0, 1, len(t_p)), **kwargs)
-        return p
```

### Comparing `pyopenrivercam-0.4.3/pyorc/cli/cli_elements.py` & `pyopenrivercam-0.5.0/pyorc/cli/cli_elements.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,48 +7,53 @@
 import numpy as np
 from matplotlib import patheffects
 from matplotlib.backend_bases import MouseButton
 from matplotlib.widgets import Button
 from matplotlib.patches import Polygon
 from mpl_toolkits.axes_grid1 import Divider, Size
 from pyorc import helpers
+from pyorc.cli import cli_utils
 
 path_effects = [
     patheffects.Stroke(linewidth=2, foreground="w"),
     patheffects.Normal(),
 ]
 
 corner_labels = [
     "upstream-left",
     "downstream-left",
     "downstream-right",
     "upstream-right"
 ]
 class BaseSelect:
-    def __init__(self, img, dst, crs=None, buffer=0.0002, zoom_level=19, logger=logging):
+    def __init__(self, img, dst=None, crs=None, buffer=0.0002, zoom_level=19, logger=logging):
         self.logger = logger
+        self.height, self.width = img.shape[0:2]
+        self.crs = crs
         fig = plt.figure(figsize=(16, 9), frameon=False, facecolor="black")
         fig.subplots_adjust(left=0, bottom=0, right=1, top=1, wspace=None, hspace=None)
-        # fig = plt.figure(figsize=(12, 7))
-        xmin = np.array(dst)[:, 0].min()
-        xmax = np.array(dst)[:, 0].max()
-        ymin = np.array(dst)[:, 1].min()
-        ymax = np.array(dst)[:, 1].max()
-        extent = [xmin - buffer, xmax + buffer, ymin-buffer, ymax + buffer]
+        ax_geo = None
         # extent = [4.5, 4.51, 51.2, 51.21]
-        if crs is not None:
-            tiler = getattr(cimgt, "GoogleTiles")(style="satellite")
-            ax_geo = fig.add_axes([0., 0., 1, 1], projection=tiler.crs)
-            ax_geo.set_extent(extent, crs=ccrs.PlateCarree())
-            ax_geo.add_image(tiler, zoom_level, zorder=1)
-        else:
-            ax_geo = fig.add_axes([0., 0., 1, 1])
-            ax_geo.set_aspect("equal")
-        plt.tick_params(left=False, right=False, labelleft=False, labelbottom=False, bottom=False)
-        ax_geo.set_visible(False)
+        if dst is not None:
+            # fig = plt.figure(figsize=(12, 7))
+            xmin = np.array(dst)[:, 0].min()
+            xmax = np.array(dst)[:, 0].max()
+            ymin = np.array(dst)[:, 1].min()
+            ymax = np.array(dst)[:, 1].max()
+            extent = [xmin - buffer, xmax + buffer, ymin - buffer, ymax + buffer]
+            if crs is not None:
+                tiler = getattr(cimgt, "GoogleTiles")(style="satellite")
+                ax_geo = fig.add_axes([0., 0., 1, 1], projection=tiler.crs)
+                ax_geo.set_extent(extent, crs=ccrs.PlateCarree())
+                ax_geo.add_image(tiler, zoom_level, zorder=1)
+            else:
+                ax_geo = fig.add_axes([0., 0., 1, 1])
+                ax_geo.set_aspect("equal")
+            plt.tick_params(left=False, right=False, labelleft=False, labelbottom=False, bottom=False)
+            ax_geo.set_visible(False)
         ax = fig.add_axes([0.2, 0.1, 0.7, 0.8])
         ax.set_facecolor("k")
         ax.set_position([0, 0, 1, 1])
         plt.tick_params(left=False, right=False, labelleft=False, labelbottom=False, bottom=False)
 
         # fig, ax = plt.subplots()
         ax.imshow(img)
@@ -65,28 +70,29 @@
             textcoords="offset points",
             zorder=4,
             path_effects=[
                 patheffects.Stroke(linewidth=3, foreground="w"),
                 patheffects.Normal(),
             ],
         )
-        if crs is not None:
-            kwargs["transform"] = ccrs.PlateCarree()
-            transform = ccrs.PlateCarree()._as_mpl_transform(ax_geo)
-            kwargs_text["xycoords"] = transform
-        self.p_geo = ax_geo.plot(
-            *list(zip(*dst))[0:2], "o",
-            **kwargs
-        )
-        for n, _pt in enumerate(dst):
-            pt = ax_geo.annotate(
-                n + 1,
-                xy = _pt[0:2],
-                **kwargs_text
+        if dst is not None:
+            if crs is not None:
+                kwargs["transform"] = ccrs.PlateCarree()
+                transform = ccrs.PlateCarree()._as_mpl_transform(ax_geo)
+                kwargs_text["xycoords"] = transform
+            self.p_geo = ax_geo.plot(
+                *list(zip(*dst))[0:2], "o",
+                **kwargs
             )
+            for n, _pt in enumerate(dst):
+                pt = ax_geo.annotate(
+                    n + 1,
+                    xy = _pt[0:2],
+                    **kwargs_text
+                )
         self.fig = fig
         self.ax_geo = ax_geo
         self.ax = ax  # add axes
         self.pts_t = []
         self.add_buttons()
         self.press = False
         self.move = False
@@ -100,28 +106,35 @@
 
     def add_buttons(self):
         h = [Size.Fixed(0.5), Size.Fixed(0.6)]
         v = [Size.Fixed(0.95), Size.Fixed(0.3)]
         v2 = [Size.Fixed(1.45), Size.Fixed(0.3)]
         v3 = [Size.Fixed(1.95), Size.Fixed(0.3)]
 
-        divider1 = Divider(self.fig, (0, 0, 1, 1), h, v, aspect=False)
+        divider3 = Divider(self.fig, (0, 0, 1, 1), h, v, aspect=False)
         divider2 = Divider(self.fig, (0, 0, 1, 1), h, v2, aspect=False)
-        divider3 = Divider(self.fig, (0, 0, 1, 1), h, v3, aspect=False)
-        self.ax_button1 = self.fig.add_axes(divider1.get_position(),
-                                  axes_locator=divider1.new_locator(nx=1, ny=1))
-        self.ax_button2 = self.fig.add_axes(divider2.get_position(),
-                                  axes_locator=divider2.new_locator(nx=1, ny=1))
-        self.ax_button3 = self.fig.add_axes(divider3.get_position(),
-                                  axes_locator=divider3.new_locator(nx=1, ny=1))
-        self.button1 = Button(self.ax_button1, 'Camera')
-        self.button2 = Button(self.ax_button2, 'Map')
+        divider1 = Divider(self.fig, (0, 0, 1, 1), h, v3, aspect=False)
+        if self.ax_geo is not None:
+            self.ax_button1 = self.fig.add_axes(
+                divider1.get_position(),
+                axes_locator=divider1.new_locator(nx=1, ny=1)
+            )
+            self.button1 = Button(self.ax_button1, 'Camera')
+            self.button1.on_clicked(self.switch_to_ax)
+            self.ax_button2 = self.fig.add_axes(
+                divider2.get_position(),
+                axes_locator=divider2.new_locator(nx=1, ny=1)
+            )
+            self.button2 = Button(self.ax_button2, 'Map')
+            self.button2.on_clicked(self.switch_to_ax_geo)
+        self.ax_button3 = self.fig.add_axes(
+            divider3.get_position(),
+            axes_locator=divider3.new_locator(nx=1, ny=1)
+        )
         self.button3 = Button(self.ax_button3, 'Done')
-        self.button1.on_clicked(self.switch_to_ax)
-        self.button2.on_clicked(self.switch_to_ax_geo)
         self.button3.on_clicked(self.close_window)
         self.button3.set_active(False)
         self.button3.label.set_color("gray")
 
     def close_window(self, event):
         # close window
         plt.close(self.fig)
@@ -228,15 +241,23 @@
         if hasattr(camera_config, "crs"):
             crs = camera_config.crs
         else:
             crs = None
         super(AoiSelect, self).__init__(img, dst, crs=crs, logger=logger)
         # make empty plot
         self.camera_config = camera_config
-        self.p_gcps, = self.ax.plot(*list(zip(*src)), "o", color="w", markeredgecolor="k", markersize=10, zorder=3)
+        self.p_gcps, = self.ax.plot(
+            *list(zip(*src)),
+            "o",
+            color="w",
+            markeredgecolor="k",
+            markersize=10,
+            zorder=3,
+            label="GCPs"
+        )
         self.pts_t_gcps = [
             self.ax.annotate(
                 n + 1,
                 xytext=(6, 6),
                 xy=xy,
                 textcoords="offset points",
                 zorder=4,
@@ -303,72 +324,210 @@
                     patheffects.Stroke(linewidth=3, foreground="w"),
                     patheffects.Normal(),
                 ],
             )
             self.pts_t.append(pt)
             # check if all points are complete
             if len(self.src) == self.required_clicks:
-                self.camera_config.set_bbox_from_corners(self.src)
-                bbox_cam = list(zip(*self.camera_config.get_bbox(camera=True).exterior.xy))
-                bbox_geo = list(zip(*self.camera_config.get_bbox().exterior.xy))
-                if hasattr(self.camera_config, "crs"):
-                    bbox_geo = helpers.xyz_transform(
-                        bbox_geo,
-                        crs_from=self.camera_config.crs,
-                        crs_to=4326
-                    )
-                self.p_bbox.set_xy(bbox_cam)
-                self.p_bbox_geo.set_xy(bbox_geo)
-                self.ax.figure.canvas.draw()
-
+                try:
+                    self.camera_config.set_bbox_from_corners(self.src)
+                    bbox_cam = list(zip(*self.camera_config.get_bbox(camera=True, redistort=True).exterior.xy))
+                    bbox_geo = list(zip(*self.camera_config.get_bbox().exterior.xy))
+                    if hasattr(self.camera_config, "crs"):
+                        bbox_geo = helpers.xyz_transform(
+                            bbox_geo,
+                            crs_from=self.camera_config.crs,
+                            crs_to=4326
+                        )
+                    self.p_bbox.set_xy(bbox_cam)
+                    self.p_bbox_geo.set_xy(bbox_geo)
+                    self.ax.figure.canvas.draw()
+                except:
+                    self.title.set_text("Could not resolve bounding box with the set coordinates.\nThe coordinates are likely measured with too low accuracy.\nMeasure with cm accuracy.")
     def on_click(self, event):
         super(AoiSelect, self).on_click(event)
         if not(len(self.src) == self.required_clicks):
             # remove plot if present
             self.p_bbox.set_xy(np.zeros((0, 2)))
             self.p_bbox_geo.set_xy(np.zeros((0, 2)))
             self.ax.figure.canvas.draw()
 
 
 class GcpSelect(BaseSelect):
     """
     Selector tool to provide source GCP coordinates to pyOpenRiverCam
     """
 
-    def __init__(self, img, dst, crs=None, logger=logging):
+    def __init__(self, img, dst, crs=None, lens_position=None, logger=logging):
         super(GcpSelect, self).__init__(img, dst, crs=crs, logger=logger)
         # make empty plot
-        self.p, = self.ax.plot([], [], "o", color="w", markeredgecolor="k", markersize=10, zorder=3)
+        self.p, = self.ax.plot([], [], "o", color="w", markeredgecolor="k", markersize=10, zorder=3, label="Clicked control points")
         kwargs = dict(
-            color="r",
+            color="c",
             markeredgecolor="w",
             zorder=4,
             markersize=10,
             label="Selected control points"
         )
         if crs is not None:
             kwargs["transform"] = ccrs.PlateCarree()
         self.p_geo_selected, = self.ax_geo.plot(
             [], [], "o",
             **kwargs
         )
+        if len(dst) >= 4:
+            # plot an empty set of crosses for the fitted gcp row columns after optimization of perspective
+            self.p_fit, = self.ax.plot(
+                [], [], "+",
+                markersize=10,
+                color="r",
+                zorder=4,
+                label="Fitted control_points"
+           )
+        else:
+            self.p_fit = None
+
         xloc = self.ax.get_xlim()[0] + 50
         yloc = self.ax.get_ylim()[-1] + 50
         self.title = self.ax.text(
             xloc,
             yloc,
             "Select location of control points in the right order (check locations on map view)",
             size=12,
             path_effects=path_effects
         )
         self.ax_geo.legend()
-        # TODO: if no crs provided, then provide a normal axes with equal lengths on x and y axis
+        self.ax.legend()
+        self.lens_position = lens_position
+        # add dst coords in the intended CRS
+        if crs is not None:
+            self.dst_crs = helpers.xyz_transform(self.dst, 4326, crs)
+        else:
+            self.dst_crs = self.dst
         self.required_clicks = len(self.dst)
+        self.camera_matrix = None
+        self.dist_coeffs = None
+
+    def on_left_click(self, event):
+        super(GcpSelect, self).on_left_click(event)
+        # figure out if the fitted control points must be computed and plotted
+        if self.p_fit is not None:
+            if len(self.src) == self.required_clicks:
+                self.title.set_text("Fitting pose and camera parameters...")
+                self.ax.figure.canvas.draw()
+                src_fit, dst_fit, camera_matrix, dist_coeffs, err = cli_utils.get_gcps_optimized_fit(
+                    self.src,
+                    self.dst_crs,
+                    self.height,
+                    self.width,
+                    c=2.,
+                    lens_position=self.lens_position
+                )
+                self.p_fit.set_data(*list(zip(*src_fit)))
+                self.camera_matrix = camera_matrix
+                self.dist_coeffs = dist_coeffs
+                new_text = 'Pose and camera parameters fitted (see "+"), average x, y distance error: {:1.3f} m.'.format(err)
+                if err > 0.1:
+                    new_text += '\nWarning: error is larger than 0.1 meter. Are you sure that the coordinates are measured accurately?'
+                self.title.set_text(new_text)
+                self.ax.figure.canvas.draw()
+            else:
+                self.p_fit.set_data([], [])
+
+    def on_right_click(self, event):
+        super(GcpSelect, self).on_right_click(event)
+        if self.p_fit is not None:
+            if len(self.src) < self.required_clicks:
+                self.p_fit.set_data([], [])
 
     def on_click(self, event):
         super(GcpSelect, self).on_click(event)
         # update selected dst points
         dst_sel = self.dst[:len(self.src)]
         if len(dst_sel) > 0:
             self.p_geo_selected.set_data(*list(zip(*dst_sel))[0:2])
         else:
             self.p_geo_selected.set_data([], [])
+
+
+class StabilizeSelect(BaseSelect):
+    def __init__(self, img, logger=logging):
+        super(StabilizeSelect, self).__init__(img, logger=logger)
+        # make empty plot
+        pol = Polygon(np.zeros((0, 2)), edgecolor="w", alpha=0.5, linewidth=2)
+        self.p = self.ax.add_patch(pol)
+        kwargs = dict(
+            color="c",
+            markeredgecolor="w",
+            zorder=4,
+            markersize=10,
+            label="Selected control points"
+        )
+        xloc = self.ax.get_xlim()[0] + 50
+        yloc = self.ax.get_ylim()[-1] + 50
+        self.title = self.ax.text(
+            xloc,
+            yloc,
+            "Select a polygon of at least 4 points that encompasses at least the water surface. Areas outside will be "
+            "treated as stable areas for stabilization.",
+            size=12,
+            path_effects=path_effects
+        )
+        self.ax.legend()
+        # add dst coords in the intended CRS
+        self.required_clicks = 4  # minimum 4 points needed for a satisfactory ROI
+
+
+    def on_click(self, event):
+        # only if ax is visible and click was within the window
+        if self.ax.get_visible() and event.inaxes == self.ax:
+            if event.button is MouseButton.RIGHT:
+                self.on_right_click(event)
+            elif event.button is MouseButton.LEFT:
+                self.on_left_click(event)
+                # check if enough points are collected to enable the Done button
+            if len(self.src) >= self.required_clicks:
+                self.button3.set_active(True)
+                self.button3.label.set_color("k")
+            else:
+                self.button3.set_active(False)
+                self.button3.label.set_color("grey")
+
+        self.ax.figure.canvas.draw()
+
+
+    def on_right_click(self, event):
+        if len(self.pts_t) > 0:
+            self.pts_t[-1].remove()
+            del self.pts_t[-1]
+        if len(self.src) > 0:
+            del self.src[-1]
+            if len(self.src) > 0:
+                self.p.set_xy(self.src)
+            else:
+                self.p.set_xy(np.zeros((0, 2)))
+        self.ax.figure.canvas.draw()
+
+    def on_left_click(self, event):
+        if event.xdata is not None:
+            self.logger.debug(f"Storing coordinate x: {event.xdata} y: {event.ydata} to src")
+            self.src.append([int(np.round(event.xdata)), int(np.round(event.ydata))])
+            # self.p.set_data(*list(zip(*self.src)))
+            self.p.set_xy(self.src)
+            pt = self.ax.annotate(
+                len(self.src),
+                xytext=(6, 6),
+                xy=(event.xdata, event.ydata),
+                textcoords="offset points",
+                zorder=4,
+                path_effects=[
+                    patheffects.Stroke(linewidth=3, foreground="w"),
+                    patheffects.Normal(),
+                ],
+            )
+            self.pts_t.append(pt)
+            self.ax.figure.canvas.draw()
+
+    def on_close(self, event):
+        # overrule the amount of required clicks
+        self.required_clicks = len(self.src)
+        super(StabilizeSelect, self).on_close(event)
```

### Comparing `pyopenrivercam-0.4.3/pyorc/cli/cli_utils.py` & `pyopenrivercam-0.5.0/pyorc/cli/cli_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,119 @@
 import click
+import cv2
 import geopandas as gpd
 import hashlib
 import json
 import logging
 import matplotlib.pyplot as plt
+import numpy as np
 import os
 import pyorc
 import yaml
 
-from pyorc import Video, helpers, CameraConfig
-from pyorc.cli.cli_elements import GcpSelect, AoiSelect
+from pyorc import Video, helpers, CameraConfig, cv
+from pyorc.cli.cli_elements import GcpSelect, AoiSelect, StabilizeSelect
 from shapely.geometry import Point
 
 
-def get_corners_interactive(fn, gcps, crs=None, crs_gcps=None, frame_sample=0., logger=logging):
+def get_corners_interactive(
+        fn,
+        gcps,
+        crs=None,
+        crs_gcps=None,
+        frame_sample=0.,
+        camera_matrix=None,
+        dist_coeffs=None,
+        logger=logging,
+):
     vid = Video(fn, start_frame=frame_sample, end_frame=frame_sample + 1)
     # get first frame
     frame = vid.get_frame(0, method="rgb")
     src = gcps["src"]
     if crs_gcps is not None:
         dst = helpers.xyz_transform(gcps["dst"], crs_from=crs_gcps, crs_to=4326)
     else:
         dst = gcps["dst"]
     # setup preliminary cam config
-    cam_config = CameraConfig(height=frame.shape[0], width=frame.shape[1], gcps=gcps, crs=crs)
+    cam_config = CameraConfig(
+        height=frame.shape[0],
+        width=frame.shape[1],
+        gcps=gcps,
+        crs=crs,
+        camera_matrix=camera_matrix,
+        dist_coeffs=dist_coeffs
+    )
     selector = AoiSelect(frame, src, dst, cam_config, logger=logger)
     # uncomment below to test the interaction, not suitable for automated unit test
     plt.show(block=True)
     return selector.src
 
     # setup a cam_config without
 
-def get_gcps_interactive(fn, dst, crs=None, crs_gcps=None, frame_sample=0., logger=logging):
+
+def get_gcps_interactive(fn, dst, crs=None, crs_gcps=None, frame_sample=0, lens_position=None, logger=logging):
     vid = Video(fn, start_frame=frame_sample, end_frame=frame_sample + 1)
     # get first frame
     frame = vid.get_frame(0, method="rgb")
     if crs_gcps is not None:
         dst = helpers.xyz_transform(dst, crs_from=crs_gcps, crs_to=4326)
-    selector = GcpSelect(frame, dst, crs=crs, logger=logger)
-    # uncomment below to test the interaction, not suitable for automated unit test
+    selector = GcpSelect(frame, dst, crs=crs, lens_position=lens_position, logger=logger)
+    plt.show(block=True)
+    return selector.src, selector.camera_matrix, selector.dist_coeffs
+
+
+def get_stabilize_pol(
+        fn,
+        frame_sample=0,
+        logger=logging
+):
+    vid = Video(fn, start_frame=frame_sample, end_frame=frame_sample + 1)
+    frame = vid.get_frame(0, method="rgb")
+    selector = StabilizeSelect(frame, logger=logger)
     plt.show(block=True)
     return selector.src
 
 
+
 def get_file_hash(fn):
     hash256 = hashlib.sha256()
     with open(fn, "rb") as f:
         # Read and update hash string value in blocks of 4K
         for byte_block in iter(lambda: f.read(4096), b""):
             # print(byte_block)
             hash256.update(byte_block)
     return hash256
 
+def get_gcps_optimized_fit(src, dst, height, width, c=2., lens_position=None):
+    # optimize cam matrix and dist coeffs with provided control points
+    if np.array(dst).shape == (4, 2):
+        _dst = np.c_[np.array(dst), np.zeros(4)]
+    else:
+        _dst = np.array(dst)
+    camera_matrix, dist_coeffs, err = cv.optimize_intrinsic(
+        src,
+        _dst,
+        height,
+        width,
+        c=c,
+        lens_position=lens_position,
+        # dist_coeffs=cv.DIST_COEFFS
+    )
+    # once optimized, solve the perspective, and estimate the GCP locations with the perspective rot/trans
+    coord_mean = np.array(_dst).mean(axis=0)
+    _src = np.float32(src)
+    _dst = np.float32(_dst) - coord_mean
+    success, rvec, tvec = cv2.solvePnP(_dst, _src, camera_matrix, np.array(dist_coeffs))
+
+    # estimate source point location
+    src_est, jacobian = cv2.projectPoints(_dst, rvec, tvec, camera_matrix, np.array(dist_coeffs))
+    src_est = np.array([list(point[0]) for point in src_est])
+    dst_est = cv.unproject_points(_src, _dst[:, -1], rvec, tvec, camera_matrix, dist_coeffs)
+    dst_est = np.array(dst_est)[:, 0:len(coord_mean)] + coord_mean
+    return src_est, dst_est, camera_matrix, dist_coeffs, err
 
 def parse_json(ctx, param, value):
     if value is None:
         return None
     if os.path.isfile(value):
         with open(value, "r") as f:
             kwargs = json.load(f)
```

### Comparing `pyopenrivercam-0.4.3/pyorc/cli/log.py` & `pyopenrivercam-0.5.0/pyorc/cli/log.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.4.3/pyorc/cli/main.py` & `pyopenrivercam-0.5.0/pyorc/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,22 @@
 )
 @click.option(
     "--corners",
     type=str,
     callback=cli_utils.parse_corners,
     help="Video ojective corner points as list of 4 [column, row] points"
 )
+@click.option(
+    "--stabilize",
+    "-s",
+    is_flag=True,
+    default=False,
+    help="Stabilize the videos using this camera configuration (you can provide a stable area in an interactive view)."
+
+)
 @verbose_opt
 @click.pass_context
 @typechecked
 def camera_config(
         ctx,
         output: str,
         videofile: str,
@@ -167,17 +175,18 @@
         h_ref: Optional[float],
         crs_gcps: Optional[Union[str, int]],
         resolution: Optional[float],
         window_size: Optional[int],
         lens_position: Optional[List[float]],
         shapefile: Optional[str],
         corners: Optional[List[List]],
+        stabilize: Optional[bool],
         verbose: int
 ):
-    log_level = max(10, 30 - 10 * verbose)
+    log_level = max(10, 20 - 10 * verbose)
     logger = log.setuplog("cameraconfig", os.path.abspath("pyorc.log"), append=False, log_level=log_level)
     logger.info(f"Preparing your cameraconfig file in {output}")
     logger.info(f"Found video file  {videofile}")
 
     if src is not None:
         logger.info("Source points found and validated")
     if dst is not None:
@@ -200,20 +209,21 @@
     if dst is not None:
         logger.info("Destination points found and validated")
     else:
         raise click.UsageError("No destination control points for found, either provide a list of points with --dst or provide a shapefile with --shapefile")
     if not src:
         logger.warning("No source control points provided. No problem, you can interactively click them in your objective")
         if click.confirm('Do you want to continue and provide source points interactively?', default=True):
-            src = cli_utils.get_gcps_interactive(
+            src, camera_matrix, dist_coeffs = cli_utils.get_gcps_interactive(
                 videofile,
                 dst,
                 crs=crs,
                 crs_gcps=crs_gcps,
                 frame_sample=frame_sample,
+                lens_position=lens_position,
                 logger=logger
             )
             if len(src) != len(dst):
                 raise click.UsageError(f"You have not provided enough source points {len(src)}/{len(dst)} available")
     if crs is None and crs_gcps is not None:
         raise click.UsageError(f"--crs is None while --crs_gcps is {crs_gcps}, please supply --crs.")
     gcps = {
@@ -228,31 +238,44 @@
         if click.confirm('Do you want to continue and provide corners interactively?', default=True):
             corners = cli_utils.get_corners_interactive(
                 videofile,
                 gcps,
                 crs=crs,
                 crs_gcps=crs_gcps,
                 frame_sample=frame_sample,
+                camera_matrix=camera_matrix,
+                dist_coeffs=dist_coeffs,
                 logger=logger
             )
+    if stabilize:
+        stabilize = cli_utils.get_stabilize_pol(
+            videofile,
+            frame_sample=frame_sample,
+            logger=logger
+        )
+    else:
+        stabilize=None
     pyorc.service.camera_config(
         video_file=videofile,
         cam_config_file=output,
         gcps=gcps,
         crs=crs,
         frame_sample=frame_sample,
         resolution=resolution,
         window_size=window_size,
         lens_position=lens_position,
-        corners=corners
+        corners=corners,
+        camera_matrix=camera_matrix,
+        dist_coeffs=dist_coeffs,
+        stabilize=stabilize
     )
     logger.info(f"Camera configuration created and stored in {output}")
 
 
-## VELOCIMETRY
+# VELOCIMETRY
 @cli.command(short_help="Estimate velocimetry")
 @click.argument(
     'OUTPUT',
     type=click.Path(resolve_path=True, dir_okay=True, file_okay=False),
     callback=cli_utils.validate_dir,
     required=True,
 )
@@ -277,37 +300,45 @@
     "-p",
     "--prefix",
     type=str,
     default="",
     help="Prefix for produced output files"
 )
 @click.option(
+    "-h",
+    "--h_a",
+    type=float,
+    required=False,
+    help="Water level in local vertical datum (e.g. staff or pressure gauge) belonging to video."
+)
+@click.option(
     "-u",
     "--update",
     is_flag=True,
     default=False,
     help="Only update requested output files with changed inputs or if not present on file system",
 )
 
 @verbose_opt
 @click.pass_context
-def velocimetry(ctx, output, videofile, recipe, cameraconfig, prefix, update, verbose):
-    log_level = max(10, 30 - 10 * verbose)
+def velocimetry(ctx, output, videofile, recipe, cameraconfig, prefix, h_a, update, verbose):
+    log_level = max(10, 20 - 10 * verbose)
     logger = log.setuplog("velocimetry", os.path.abspath("pyorc.log"), append=False, log_level=log_level)
     logger.info(f"Preparing your velocimetry result in {output}")
+    if h_a is not None:
+        recipe["video"]["h_a"] = h_a
     processor = pyorc.service.VelocityFlowProcessor(
         recipe,
         videofile,
         cameraconfig,
         prefix,
         output,
         update=update,
         logger=logger
     )
     # process video following the settings
     processor.process()
-    # read yaml
     pass
 
 if __name__ == "__main__":
 #if getattr(sys, 'frozen', False):
     cli(sys.argv[1:])
```

### Comparing `pyopenrivercam-0.4.3/pyorc/const.py` & `pyopenrivercam-0.5.0/pyorc/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # attributes for PIV variables
 
 v_x = "v_x"
 v_y = "v_y"
 s2n = "s2n"
 corr = "corr"
 
+DIST_COEFFS = [[0.], [0.], [0.], [0.]]
+
 PIV_ATTRS = {
     v_x: {
         "standard_name": "sea_water_x_velocity",
         "long_name": "Flow element center velocity vector, x-component",
         "units": "m s-1",
         "coordinates": "lon lat",
     },
```

### Comparing `pyopenrivercam-0.4.3/pyorc/helpers.py` & `pyopenrivercam-0.5.0/pyorc/helpers.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.4.3/pyorc/piv_process.py` & `pyopenrivercam-0.5.0/pyorc/piv_process.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.4.3/pyorc/service/camera_config.py` & `pyopenrivercam-0.5.0/pyorc/service/camera_config.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.4.3/pyorc/service/velocimetry.py` & `pyopenrivercam-0.5.0/pyorc/service/velocimetry.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.4.3/setup.py` & `pyopenrivercam-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="pyopenrivercam",
     description="pyopenrivercam (pyorc) is a front and backend to control river camera observation locations",
-    version="0.4.3",
+    version="0.5.0",
     long_description=readme + "\n\n",
     long_description_content_type="text/markdown",
     url="https://github.com/localdevices/pyorc",
     author="Hessel Winsemius",
     author_email="winsemius@rainbowsensing.com",
     packages=find_packages(),
     package_dir={"pyorc": "pyorc"},
```

### Comparing `pyopenrivercam-0.4.3/tests/conftest.py` & `pyopenrivercam-0.5.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,18 @@
     return fn
 
 
 @pytest.fixture
 def cam_config_fn():
     return os.path.join(EXAMPLE_DATA_DIR, "ngwerere", "ngwerere.json")
 
+@pytest.fixture
+def cam_config_6gcps_fn():
+    return os.path.join(EXAMPLE_DATA_DIR, "geul", "dk_cam_config.json")
+
 
 @pytest.fixture
 def recipe_yml():
     return os.path.join(EXAMPLE_DATA_DIR, "ngwerere", "ngwerere_test.yml")
 
 
 @pytest.fixture
@@ -99,39 +103,52 @@
 @pytest.fixture
 def lens_position():
     return [642732.6705, 8304289.010, 1188.5]
 
 
 @pytest.fixture
 def bbox():
-    return wkt.loads("POLYGON ((642730.3058131004 8304292.867164782, 642731.2767039008 8304302.468199677, 642739.4450455057 8304301.642187919, 642738.4741547054 8304292.041153024, 642730.3058131004 8304292.867164782))")
+    return wkt.loads("POLYGON ((642730.233168765 8304293.351276383, 642731.5013330225 8304302.039208209, 642739.2789120832 8304300.903926767, 642738.0107478257 8304292.215994941, 642730.233168765 8304293.351276383))")
+
+@pytest.fixture
+def bbox_6gcps():
+    return wkt.loads("POLYGON ((192103.06271249574 313152.336519752, 192096.59215064772 313165.9688317118, 192104.64144816675 313169.78942190844, 192111.11201001477 313156.1571099486, 192103.06271249574 313152.336519752))")
 
 
 @pytest.fixture
 def corners():
     return [
         [292, 817],
         [50, 166],
         [1200, 236],
         [1600, 834]
     ]
 
+@pytest.fixture
+def corners_6gcps():
+    return [
+        [390, 440],
+        [1060, 160],
+        [1800, 270],
+        [1500, 880]
+    ]
+
 
 @pytest.fixture
 def lens_pars():
     return {
         "k1": 0,
         "c": 2.0,
-        "f": 1.0
+        "focal_length": 1550.
     }
 
 
 @pytest.fixture
 def camera_matrix():
-    return np.array([[1920., 0., 960.], [0., 1920., 540.], [0., 0., 1.]])
+    return np.array([[1550., 0., 960.], [0., 1550., 540.], [0., 0., 1.]])
 
 
 @pytest.fixture
 def cam_config(gcps, lens_position, lens_pars, corners):
     return pyorc.CameraConfig(
         height=1080,
         width=1920,
@@ -140,28 +157,31 @@
         lens_pars=lens_pars,
         corners=corners,
         window_size=25,
         resolution=0.01,
         crs=32735
         )
 
+@pytest.fixture
+def cam_config_6gcps(cam_config_6gcps_fn):
+    # load in memory
+    return pyorc.load_camera_config(cam_config_6gcps_fn)
 
 @pytest.fixture
 def cam_config_without_aoi(lens_position, gcps):
     return pyorc.CameraConfig(
         height=1080,
         width=1920,
         lens_position=lens_position,
         gcps=gcps,
         window_size=25,
         resolution=0.01,
         crs=32735
         )
 
-
 @pytest.fixture
 def cam_config_calib():
     return pyorc.CameraConfig(
         height=720,
         width=1280,
     )
 
@@ -186,14 +206,15 @@
             'gcps': {
                 'src': [[1421, 1001], [1251, 460], [421, 432], [470, 607]],
                 'dst': [[642735.8076, 8304292.119], [642737.5823, 8304295.593], [642732.7864, 8304298.425], [642732.6705, 8304296.858]],
                 'h_ref': 0.0,
                 'z_0': 1182.2
             },
             'window_size': 25,
+            'is_nadir': False
 
     }
 
 
 @pytest.fixture
 def cam_config_str():
     # return '{\n    "crs": "PROJCRS[\\"WGS 84 / UTM zone 35S\\",BASEGEOGCRS[\\"WGS 84\\",ENSEMBLE[\\"World Geodetic System 1984 ensemble\\",MEMBER[\\"World Geodetic System 1984 (Transit)\\"],MEMBER[\\"World Geodetic System 1984 (G730)\\"],MEMBER[\\"World Geodetic System 1984 (G873)\\"],MEMBER[\\"World Geodetic System 1984 (G1150)\\"],MEMBER[\\"World Geodetic System 1984 (G1674)\\"],MEMBER[\\"World Geodetic System 1984 (G1762)\\"],MEMBER[\\"World Geodetic System 1984 (G2139)\\"],ELLIPSOID[\\"WGS 84\\",6378137,298.257223563,LENGTHUNIT[\\"metre\\",1]],ENSEMBLEACCURACY[2.0]],PRIMEM[\\"Greenwich\\",0,ANGLEUNIT[\\"degree\\",0.0174532925199433]],ID[\\"EPSG\\",4326]],CONVERSION[\\"UTM zone 35S\\",METHOD[\\"Transverse Mercator\\",ID[\\"EPSG\\",9807]],PARAMETER[\\"Latitude of natural origin\\",0,ANGLEUNIT[\\"degree\\",0.0174532925199433],ID[\\"EPSG\\",8801]],PARAMETER[\\"Longitude of natural origin\\",27,ANGLEUNIT[\\"degree\\",0.0174532925199433],ID[\\"EPSG\\",8802]],PARAMETER[\\"Scale factor at natural origin\\",0.9996,SCALEUNIT[\\"unity\\",1],ID[\\"EPSG\\",8805]],PARAMETER[\\"False easting\\",500000,LENGTHUNIT[\\"metre\\",1],ID[\\"EPSG\\",8806]],PARAMETER[\\"False northing\\",10000000,LENGTHUNIT[\\"metre\\",1],ID[\\"EPSG\\",8807]]],CS[Cartesian,2],AXIS[\\"(E)\\",east,ORDER[1],LENGTHUNIT[\\"metre\\",1]],AXIS[\\"(N)\\",north,ORDER[2],LENGTHUNIT[\\"metre\\",1]],USAGE[SCOPE[\\"Engineering survey, topographic mapping.\\"],AREA[\\"Between 24\\u00b0E and 30\\u00b0E, southern hemisphere between 80\\u00b0S and equator, onshore and offshore. Botswana. Burundi. Democratic Republic of the Congo (Zaire). Rwanda. South Africa. Tanzania. Uganda. Zambia. Zimbabwe.\\"],BBOX[-80,24,0,30]],ID[\\"EPSG\\",32735]]",\n    "resolution": 0.01,\n    "lens_position": [\n        642732.6705,\n        8304289.01,\n        1188.5\n    ],\n    "gcps": {\n        "src": [\n            [\n                1421,\n                1001\n            ],\n            [\n                1251,\n                460\n            ],\n            [\n                421,\n                432\n            ],\n            [\n                470,\n                607\n            ]\n        ],\n        "dst": [\n            [\n                642735.8076,\n                8304292.119\n            ],\n            [\n                642737.5823,\n                8304295.593\n            ],\n            [\n                642732.7864,\n                8304298.425\n            ],\n            [\n                642732.6705,\n                8304296.858\n            ]\n        ],\n        "h_ref": 0.0,\n        "z_0": 1182.2\n    },\n    "lens_pars": {\n        "k1": 0,\n        "c": 2.0,\n        "f": 1.0\n    },\n    "window_size": 25,\n    "corners": [\n        [\n            292,\n            817\n        ],\n        [\n            50,\n            166\n        ],\n        [\n            1200,\n            236\n        ],\n        [\n            1600,\n            834\n        ]\n    ]\n}'
@@ -202,24 +223,41 @@
 
 @pytest.fixture
 def vid_file():
     return os.path.join(EXAMPLE_DATA_DIR, "ngwerere", "ngwerere_20191103.mp4")
 
 
 @pytest.fixture
+def vid_file_6gcps():
+    return os.path.join(EXAMPLE_DATA_DIR, "geul", "dk_control.mp4")
+
+
+@pytest.fixture
 def vid(vid_file):
     vid = pyorc.Video(
         vid_file,
         start_frame=0,
         end_frame=2,
     )
     yield vid
 
 
 @pytest.fixture
+def vid_6gcps_cam_config(vid_file_6gcps, cam_config_6gcps):
+    vid = pyorc.Video(
+        vid_file_6gcps,
+        start_frame=0,
+        end_frame=2,
+        camera_config=cam_config_6gcps,
+        h_a=92.36
+    )
+    yield vid
+
+
+@pytest.fixture
 def vid_cam_config(cam_config):
     vid = pyorc.Video(
         os.path.join(EXAMPLE_DATA_DIR, "ngwerere", "ngwerere_20191103.mp4"),
         start_frame=0,
         end_frame=2,
         camera_config=cam_config,
         h_a=0.
@@ -244,15 +282,20 @@
 def vid_cam_config_stabilize(cam_config):
     vid = pyorc.Video(
         os.path.join(EXAMPLE_DATA_DIR, "ngwerere", "ngwerere_20191103.mp4"),
         start_frame=0,
         end_frame=20,
         camera_config=cam_config,
         h_a=0.,
-        stabilize="fixed"
+        stabilize=[
+            [400, 1080],
+            [170, 0],
+            [1000, 0],
+            [1750, 1080]
+        ]  # coordinates for which outside area is meant for stabilization
     )
     yield vid
 
 
 @pytest.fixture
 def frame_rgb(vid_cam_config):
     return vid_cam_config.get_frame(0, method="rgb")
```

### Comparing `pyopenrivercam-0.4.3/tests/test_cli.py` & `pyopenrivercam-0.5.0/tests/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os.path
 
 from click.testing import CliRunner
 from pyorc.cli.main import cli
-from pyorc.cli.cli_elements import GcpSelect, AoiSelect
+from pyorc.cli.cli_elements import GcpSelect, AoiSelect, StabilizeSelect
 from pyorc.cli import cli_utils
 from pyorc.helpers import xyz_transform
 import json
 
 def test_cli_cam_config(cli_obj):
     result = cli_obj.invoke(
         cli, [
@@ -59,20 +59,22 @@
             'velocimetry',
             '-V',
             vid_file,
             '-c',
             cam_config_fn,
             '-r',
             cli_recipe_fn,
-            '-vvv',
+            '-v',
             cli_output_dir,
             '-u'
         ],
         echo=True
     )
+    import time
+    time.sleep(1)
     assert result.exit_code == 0
 
 
 def test_service_video(velocity_flow_processor):
     # ensure we are in the right folder
     print(f"current file is: {os.path.dirname(__file__)}")
     os.chdir(os.path.dirname(__file__))
@@ -87,15 +89,15 @@
     # crs = None
     if crs is not None:
         dst = xyz_transform(gcps_dst, crs_from=crs, crs_to=4326)
     else:
         dst = gcps_dst
     selector = GcpSelect(frame_rgb, dst, crs=crs)
     # uncomment below to test the interaction, not suitable for automated unit test
-    # plt.show(block=True)
+    plt.show(block=True)
 
 
 
 def test_aoi_interact(frame_rgb, cam_config_without_aoi):
     import matplotlib.pyplot as plt
     # convert dst to
     # del cam_config_without_aoi.crs
@@ -104,13 +106,19 @@
         dst = xyz_transform(cam_config_without_aoi.gcps["dst"], crs_from=cam_config_without_aoi.crs, crs_to=4326)
     else:
         dst = cam_config_without_aoi.gcps["dst"]
     selector = AoiSelect(frame_rgb, src, dst, cam_config_without_aoi)
     # uncomment below to test the interaction, not suitable for automated unit test
     # plt.show(block=True)
 
+def test_stabilize_interact(frame_rgb):
+    import matplotlib.pyplot as plt
+    selector = StabilizeSelect(frame_rgb)
+    # uncomment below to test the interaction, not suitable for automated unit test
+    # plt.show(block=True)
+
 # cli utils
 def test_read_shape(gcps_fn):
     coords, wkt = cli_utils.read_shape(gcps_fn)
     assert(isinstance(wkt, str))
     assert(isinstance(coords, list))
```

### Comparing `pyopenrivercam-0.4.3/tests/test_frames.py` & `pyopenrivercam-0.5.0/tests/test_frames.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import pytest
 import numpy as np
 import matplotlib.pyplot as plt
 
 @pytest.mark.parametrize(
     "frames, resolution, dims, shape",
     [
-        (pytest.lazy_fixture("frames_grayscale"), 0.1, 3, (83, 97)),
-        (pytest.lazy_fixture("frames_grayscale"), 0.01, 3, (821, 965)),
-        (pytest.lazy_fixture("frames_grayscale"), 0.005, 3, (1642, 1930)),
-        (pytest.lazy_fixture("frames_rgb"), 0.1, 4, (83, 97, 3)),
+        (pytest.lazy_fixture("frames_grayscale"), 0.1, 3, (79, 88)),
+        (pytest.lazy_fixture("frames_grayscale"), 0.01, 3, (786, 878)),
+        (pytest.lazy_fixture("frames_grayscale"), 0.005, 3, (1572, 1756)),
+        (pytest.lazy_fixture("frames_rgb"), 0.1, 4, (79, 88, 3)),
     ]
 )
 def test_project(frames, resolution, dims, shape):
 # def test_project(frames_grayscale, resolution=0.01, dims=3, shape=(840, 1100)):
     frames_proj = frames.frames.project(resolution=resolution)
     # check amount of time steps is equal
     assert(len(frames_proj.time) == len(frames.time))
@@ -40,15 +40,15 @@
     assert(frames_norm[0, 0, 0].values.dtype == "uint8"), f'dtype of result is {frames_norm[0, 0, 0].values.dtype}, expected "uint8"'
 
 
 def test_edge_detect(frames_proj):
     frames_edge = frames_proj.frames.edge_detect()
     assert(frames_edge.shape == frames_proj.shape)
     assert(frames_edge[0, 0, 0].values.dtype == "float32"), f'dtype of result is {frames_edge[0, 0, 0].values.dtype}, expected "float32"'
-    assert(np.allclose(frames_edge.values.flatten()[-4:], [6.328125, 2.34375, 0.0625, 0.40625]))
+    assert(np.allclose(frames_edge.values.flatten()[-4:], [-1.3828125, -4.3359375,  1.71875  ,  7.234375 ]))
 
 
 
 def test_reduce_rolling(frames_grayscale, samples=1):
     frames_reduced = frames_grayscale.frames.reduce_rolling(samples=samples)
     assert(frames_reduced.shape == frames_grayscale.shape)
 
@@ -78,17 +78,17 @@
     frames_proj[idx].frames.plot(mode="geographical")
     plt.close("all")
 
 
 @pytest.mark.parametrize(
     "window_size, result",
     [
-        (5, [0.04290744, np.nan, np.nan, 0.07388695]),
-        (10, [0.25739092, 0.22005227, 0.30368298, 0.33715272]),
-        (15, [0.27460322, 0.3151794, 0.26885322, 0.25401443])
+        # (5, [np.nan, np.nan, np.nan, 0.06877007]),
+        (10, [0.13262428, 0.1469308 , 0.24223496, 0.14565821]),
+        # (15, [0.21774408, 0.21398547, 0.25068682, 0.26456946])
     ]
 )
 def test_get_piv(frames_proj, window_size, result):
     piv = frames_proj.frames.get_piv(window_size=window_size)
     piv_mean = piv.mean(dim="time", keep_attrs=True)
     # check if results are stable
     assert(np.allclose(piv_mean["v_x"].values.flatten()[-4:], result, equal_nan=True))
```

### Comparing `pyopenrivercam-0.4.3/tests/test_mask.py` & `pyopenrivercam-0.5.0/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.4.3/tests/test_transect.py` & `pyopenrivercam-0.5.0/tests/test_transect.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import matplotlib.pyplot as plt
 
 def test_get_river_flow(piv_transect):
     # fill method is already tested in get_q, so choose default only
     piv_transect.transect.get_q()
     piv_transect.transect.get_river_flow()
     # because we only have PIV for one time step, all quantiles will have the same values
-    assert(np.allclose(piv_transect.river_flow.values, [0.07360698, 0.0772654 , 0.08183843, 0.08641146, 0.09006988]))
+    # we allow for 0.001 m3/s deviation for differences in versions of libs
+    assert(np.allclose(piv_transect.river_flow.values, [0.09619845, 0.10308669, 0.11169699, 0.12030729, 0.12719553], atol=0.001))
 
 
 @pytest.mark.parametrize(
     "fill_method",
     [
         "zeros",
         "log_interp",
@@ -38,9 +39,7 @@
         "quiver",
         # "scatter",
     ]
 )
 def test_plot(piv_transect, mode, method):
     piv_transect.transect.get_q()
     piv_transect.isel(quantile=2).transect.plot(method=method, mode=mode, add_text=True)
-    plt.show()
-    # plt.close("all")
```

### Comparing `pyopenrivercam-0.4.3/tests/test_video.py` & `pyopenrivercam-0.5.0/tests/test_video.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     assert(vid.fps == 30.)
 
 
 @pytest.mark.parametrize(
     "video, method, result",
     [
         (pytest.lazy_fixture("vid_cam_config"), "grayscale", [85, 71, 65, 80]),
-        (pytest.lazy_fixture("vid_cam_config_stabilize"), "grayscale", [8, 87, 76, 72]),
+        (pytest.lazy_fixture("vid_cam_config_stabilize"), "grayscale", [5, 88, 78, 73]),
         (pytest.lazy_fixture("vid_cam_config"), "rgb", [84, 91, 57, 70]),
         (pytest.lazy_fixture("vid_cam_config"), "hsv", [36, 95, 91, 36])
     ]
 )
 def test_get_frame(video, method, result):
     frame = video.get_frame(1, method=method)
     assert(np.allclose(frame.flatten()[0:4], result))
```

