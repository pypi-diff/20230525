# Comparing `tmp/iris-ued-5.3.4.tar.gz` & `tmp/iris-ued-5.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iris-ued-5.3.4.tar", last modified: Mon Aug 15 19:59:04 2022, max compression
+gzip compressed data, was "iris-ued-5.3.5.tar", last modified: Thu May 25 10:51:19 2023, max compression
```

## Comparing `iris-ued-5.3.4.tar` & `iris-ued-5.3.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-15 19:59:04.094701 iris-ued-5.3.4/
--rw-r--r--   0 runner     (501) staff       (20)     6126 2022-08-15 19:56:23.000000 iris-ued-5.3.4/CHANGELOG.rst
--rw-r--r--   0 runner     (501) staff       (20)    35148 2022-08-15 19:56:23.000000 iris-ued-5.3.4/LICENSE.txt
--rw-r--r--   0 runner     (501) staff       (20)      217 2022-08-15 19:56:23.000000 iris-ued-5.3.4/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     5144 2022-08-15 19:59:04.094885 iris-ued-5.3.4/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3550 2022-08-15 19:56:23.000000 iris-ued-5.3.4/README.md
--rw-r--r--   0 runner     (501) staff       (20)       59 2022-08-15 19:56:23.000000 iris-ued-5.3.4/dev-requirements.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-15 19:59:04.080264 iris-ued-5.3.4/iris/
--rw-r--r--   0 runner     (501) staff       (20)      456 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2349 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)    34493 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/dataset.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-15 19:59:04.088162 iris-ued-5.3.4/iris/gui/
--rw-r--r--   0 runner     (501) staff       (20)     2927 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/gui/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     7456 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/gui/angular_average_dialog.py
--rw-r--r--   0 runner     (501) staff       (20)     9562 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/gui/bragg_peak_dialog.py
--rw-r--r--   0 runner     (501) staff       (20)     8947 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/gui/calibrate_q_dialog.py
--rw-r--r--   0 runner     (501) staff       (20)    18938 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/gui/control_bar.py
--rw-r--r--   0 runner     (501) staff       (20)    30633 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/gui/controller.py
--rw-r--r--   0 runner     (501) staff       (20)     8583 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/gui/data_viewer.py
--rw-r--r--   0 runner     (501) staff       (20)    35747 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/gui/gui.py
--rw-r--r--   0 runner     (501) staff       (20)     3352 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/gui/metadata_edit_dialog.py
--rw-r--r--   0 runner     (501) staff       (20)     4170 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/gui/powder_viewer.py
--rw-r--r--   0 runner     (501) staff       (20)    21353 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/gui/processing_dialog.py
--rw-r--r--   0 runner     (501) staff       (20)     3143 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/gui/qbusyindicator.py
--rw-r--r--   0 runner     (501) staff       (20)     1912 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/gui/qlogger.py
--rw-r--r--   0 runner     (501) staff       (20)     7538 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/gui/symmetrize_dialog.py
--rw-r--r--   0 runner     (501) staff       (20)     7826 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/gui/time_series_widget.py
--rw-r--r--   0 runner     (501) staff       (20)     1940 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/gui/update.py
--rw-r--r--   0 runner     (501) staff       (20)     5526 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/meta.py
--rw-r--r--   0 runner     (501) staff       (20)     1421 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/plugins.py
--rw-r--r--   0 runner     (501) staff       (20)    17965 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/powder.py
--rw-r--r--   0 runner     (501) staff       (20)    12955 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/raw.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-15 19:59:04.091514 iris-ued-5.3.4/iris/tests/
--rw-r--r--   0 runner     (501) staff       (20)      867 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      243 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/tests/broken_plugin.py
--rw-r--r--   0 runner     (501) staff       (20)     1168 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/tests/plugin_fixture.py
--rw-r--r--   0 runner     (501) staff       (20)    12507 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/tests/test_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     1462 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/tests/test_plugins.py
--rw-r--r--   0 runner     (501) staff       (20)     4201 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/tests/test_powder.py
--rw-r--r--   0 runner     (501) staff       (20)     1780 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris/tests/test_raw.py
--rw-r--r--   0 runner     (501) staff       (20)   367261 2022-08-15 19:56:23.000000 iris-ued-5.3.4/iris_screen.png
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-15 19:59:04.094325 iris-ued-5.3.4/iris_ued.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     5144 2022-08-15 19:59:04.000000 iris-ued-5.3.4/iris_ued.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1023 2022-08-15 19:59:04.000000 iris-ued-5.3.4/iris_ued.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-08-15 19:59:04.000000 iris-ued-5.3.4/iris_ued.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       41 2022-08-15 19:59:04.000000 iris-ued-5.3.4/iris_ued.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)      171 2022-08-15 19:59:04.000000 iris-ued-5.3.4/iris_ued.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        5 2022-08-15 19:59:04.000000 iris-ued-5.3.4/iris_ued.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)      343 2022-08-15 19:56:23.000000 iris-ued-5.3.4/requirements.txt
--rw-r--r--   0 runner     (501) staff       (20)      161 2022-08-15 19:59:04.095582 iris-ued-5.3.4/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     3273 2022-08-15 19:56:23.000000 iris-ued-5.3.4/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-25 10:51:19.320162 iris-ued-5.3.5/
+-rw-r--r--   0 runner     (501) staff       (20)     6352 2023-05-25 10:48:56.000000 iris-ued-5.3.5/CHANGELOG.rst
+-rw-r--r--   0 runner     (501) staff       (20)    35148 2023-05-25 10:48:56.000000 iris-ued-5.3.5/LICENSE.txt
+-rw-r--r--   0 runner     (501) staff       (20)      217 2023-05-25 10:48:56.000000 iris-ued-5.3.5/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     5196 2023-05-25 10:51:19.320338 iris-ued-5.3.5/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3550 2023-05-25 10:48:56.000000 iris-ued-5.3.5/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-05-25 10:48:56.000000 iris-ued-5.3.5/dev-requirements.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-25 10:51:19.306393 iris-ued-5.3.5/iris/
+-rw-r--r--   0 runner     (501) staff       (20)      456 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2349 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)    34495 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/dataset.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-25 10:51:19.313899 iris-ued-5.3.5/iris/gui/
+-rw-r--r--   0 runner     (501) staff       (20)     2927 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/gui/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7456 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/gui/angular_average_dialog.py
+-rw-r--r--   0 runner     (501) staff       (20)     9684 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/gui/bragg_peak_dialog.py
+-rw-r--r--   0 runner     (501) staff       (20)     8947 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/gui/calibrate_q_dialog.py
+-rw-r--r--   0 runner     (501) staff       (20)    18938 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/gui/control_bar.py
+-rw-r--r--   0 runner     (501) staff       (20)    30686 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/gui/controller.py
+-rw-r--r--   0 runner     (501) staff       (20)     8525 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/gui/data_viewer.py
+-rw-r--r--   0 runner     (501) staff       (20)    35565 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/gui/gui.py
+-rw-r--r--   0 runner     (501) staff       (20)     3352 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/gui/metadata_edit_dialog.py
+-rw-r--r--   0 runner     (501) staff       (20)     4170 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/gui/powder_viewer.py
+-rw-r--r--   0 runner     (501) staff       (20)    21589 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/gui/processing_dialog.py
+-rw-r--r--   0 runner     (501) staff       (20)     3143 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/gui/qbusyindicator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1912 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/gui/qlogger.py
+-rw-r--r--   0 runner     (501) staff       (20)     7556 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/gui/symmetrize_dialog.py
+-rw-r--r--   0 runner     (501) staff       (20)     8005 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/gui/time_series_widget.py
+-rw-r--r--   0 runner     (501) staff       (20)     1940 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/gui/update.py
+-rw-r--r--   0 runner     (501) staff       (20)     5526 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/meta.py
+-rw-r--r--   0 runner     (501) staff       (20)     1421 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/plugins.py
+-rw-r--r--   0 runner     (501) staff       (20)    17965 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/powder.py
+-rw-r--r--   0 runner     (501) staff       (20)    12959 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/raw.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-25 10:51:19.317158 iris-ued-5.3.5/iris/tests/
+-rw-r--r--   0 runner     (501) staff       (20)      867 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/tests/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      243 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/tests/broken_plugin.py
+-rw-r--r--   0 runner     (501) staff       (20)     1168 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/tests/plugin_fixture.py
+-rw-r--r--   0 runner     (501) staff       (20)    12532 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/tests/test_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     1462 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/tests/test_plugins.py
+-rw-r--r--   0 runner     (501) staff       (20)     4201 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/tests/test_powder.py
+-rw-r--r--   0 runner     (501) staff       (20)     1780 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris/tests/test_raw.py
+-rw-r--r--   0 runner     (501) staff       (20)   367261 2023-05-25 10:48:56.000000 iris-ued-5.3.5/iris_screen.png
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-25 10:51:19.319820 iris-ued-5.3.5/iris_ued.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     5196 2023-05-25 10:51:19.000000 iris-ued-5.3.5/iris_ued.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1023 2023-05-25 10:51:19.000000 iris-ued-5.3.5/iris_ued.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-05-25 10:51:19.000000 iris-ued-5.3.5/iris_ued.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       41 2023-05-25 10:51:19.000000 iris-ued-5.3.5/iris_ued.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)      165 2023-05-25 10:51:19.000000 iris-ued-5.3.5/iris_ued.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        5 2023-05-25 10:51:19.000000 iris-ued-5.3.5/iris_ued.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)      201 2023-05-25 10:48:56.000000 iris-ued-5.3.5/requirements.txt
+-rw-r--r--   0 runner     (501) staff       (20)      161 2023-05-25 10:51:19.320989 iris-ued-5.3.5/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     3329 2023-05-25 10:48:56.000000 iris-ued-5.3.5/setup.py
```

### Comparing `iris-ued-5.3.4/CHANGELOG.rst` & `iris-ued-5.3.5/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,22 @@
+Release 5.3.5
+-------------
+
+* Fixed an issue where migrating older datasets to add a diffraction center automatically could fail (#26).
+
 Release 5.3.4
 -------------
 
 * Added new Bragg peak functionality of processed datasets, as well as arbitrary mask loading and generation for pre-processing.
 
+Release 5.3.3
+-------------
+
+* Fixed an issue when computing azimuthal averages (#18).
+
 Release 5.3.2
 -------------
 
 * Fixed some issues with new versions of Python and PyQt5 (#16) and other maintenance (#17).
 
 Release 5.3.1
 -------------
```

### Comparing `iris-ued-5.3.4/LICENSE.txt` & `iris-ued-5.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/PKG-INFO` & `iris-ued-5.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris-ued
-Version: 5.3.4
+Version: 5.3.5
 Summary: Ultrafast electron diffraction data exploration
 Home-page: http://iris-ued.readthedocs.io
 Author: Laurent P. René de Cotret
 Author-email: laurent.renedecotret@mail.mcgill.ca
 Maintainer: Laurent P. René de Cotret
 Maintainer-email: laurent.renedecotret@mail.mcgill.ca
 License: GPLv3
@@ -21,19 +21,20 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >= 3.7
+Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Iris - Ultrafast Electron Scattering Data Exploration
 
 [![Documentation Build Status](https://readthedocs.org/projects/iris-ued/badge/?version=master)](http://iris-ued.readthedocs.io/) [![PyPI Version](https://img.shields.io/pypi/v/iris-ued.svg)](https://pypi.python.org/pypi/iris-ued) [![Conda-forge Version](https://img.shields.io/conda/vn/conda-forge/iris-ued.svg)](https://anaconda.org/conda-forge/iris-ued) [![DOI badge](https://img.shields.io/badge/DOI-10.1186%2Fs40679--018--0060--y-blue)](https://doi.org/10.1186/s40679-018-0060-y)
 
@@ -69,15 +70,15 @@
     conda install iris-ued
 
 To install the latest development version from
 [Github](https://github.com/LaurentRDC/iris-ued):
 
     python -m pip install git+git://github.com/LaurentRDC/iris-ued.git
 
-Each version is tested against Python 3.7+. If you are using a different
+Each version is tested against Python 3.8+. If you are using a different
 version, tests can be run using the `pytest` package.
 
 ### Windows Installers
 
 For Windows, installers are available on the [Releases](https://github.com/LaurentRDC/iris-ued/releases) page. You will still need to install `iris` via `pip` or `conda` to use the scripting functionality.
 
 ## Usage
```

### Comparing `iris-ued-5.3.4/README.md` & `iris-ued-5.3.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     conda install iris-ued
 
 To install the latest development version from
 [Github](https://github.com/LaurentRDC/iris-ued):
 
     python -m pip install git+git://github.com/LaurentRDC/iris-ued.git
 
-Each version is tested against Python 3.7+. If you are using a different
+Each version is tested against Python 3.8+. If you are using a different
 version, tests can be run using the `pytest` package.
 
 ### Windows Installers
 
 For Windows, installers are available on the [Releases](https://github.com/LaurentRDC/iris-ued/releases) page. You will still need to install `iris` via `pip` or `conda` to use the scripting functionality.
 
 ## Usage
```

### Comparing `iris-ued-5.3.4/iris/__main__.py` & `iris-ued-5.3.5/iris/__main__.py`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/iris/dataset.py` & `iris-ued-5.3.5/iris/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Diffraction dataset types
 """
-from sys import platform
 from collections import OrderedDict
-from collections.abc import Callable
-from functools import lru_cache, partial, wraps
-from math import sqrt
+from functools import partial, wraps
 from warnings import warn
 
 import h5py
 import numpy as np
 from scipy.ndimage import gaussian_filter
 
 import npstreams as ns
@@ -745,15 +742,15 @@
 
         if relative:
             out -= self.diff_eq()
             out /= self.diff_eq()
 
             # Division might introduce infs and nans
             out[:] = np.nan_to_num(out, copy=False)
-            np.minimum(out, 2 ** 16 - 1, out=out)
+            np.minimum(out, 2**16 - 1, out=out)
 
         return out
 
     def time_series(self, rect, relative=False, out=None):
         """
         Integrated intensity over time inside bounds.
 
@@ -862,19 +859,22 @@
         PermissionError
             if the dataset has not been opened with write access.
         ValueError
             If all pixels that are deemed valid have zero intensity.
         """
         intensity = self.diffraction_group["intensity"]
         image = ns.average(intensity[:, :, i] for i in range(intensity.shape[2]))
+
+        # In cases where there's no intensity data, we want to assign a reasonable
+        # diffraction center rather than fail the autocenter routine.
+        # See #26.
         if np.allclose(image * self.valid_mask, 0):
-            raise ValueError(
-                "There is not enough data to determine a center; all valid pixels have zero intensity."
-            )
-        r, c = autocenter(im=image, mask=self.valid_mask)
+            r, c = image.shape[0]//2, image.shape[1]//2
+        else:
+            r, c = autocenter(im=image, mask=self.valid_mask)
 
         # Note that for backwards-compatibility, the center
         # coordinates need to be stored as (col, row)
         self.center = (c, r)
 
     @property
     def experimental_parameters_group(self):
```

### Comparing `iris-ued-5.3.4/iris/gui/__init__.py` & `iris-ued-5.3.5/iris/gui/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,17 +53,17 @@
         Path to either a raw dataset or a processed datasets.
         Raw dataset formats will be guessed.
     dset_type : {'raw', 'reduced', None}, optional
         Dataset type.
     """
 
     with gui_environment():
-        if hasattr(QtGui, 'QApplication'):
+        if hasattr(QtGui, "QApplication"):
             app = QtGui.QApplication(sys.argv)
-        elif hasattr(QtWidgets, 'QApplication'):
+        elif hasattr(QtWidgets, "QApplication"):
             app = QtWidgets.QApplication(sys.argv)
         else:
             warn("PyQT5 has no known location of `QApplication`. Exiting now.")
             sys.exit(2)
         app.setStyleSheet(load_stylesheet_pyqt5())
         app.setWindowIcon(QtGui.QIcon(join(IMAGE_FOLDER, "eye.png")))
         gui = Iris()
```

### Comparing `iris-ued-5.3.4/iris/gui/angular_average_dialog.py` & `iris-ued-5.3.5/iris/gui/angular_average_dialog.py`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/iris/gui/bragg_peak_dialog.py` & `iris-ued-5.3.5/iris/gui/bragg_peak_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,35 +10,40 @@
 import pyqtgraph as pg
 from PyQt5 import QtCore, QtWidgets
 from skued import bragg_peaks, autocenter
 from .controller import WorkThread
 from .qbusyindicator import QBusyIndicator
 from .processing_dialog import MaskCreator
 
+
 class RectROIWithCenter(pg.RectROI):
 
     # Calculating the center position assumes that PyQtGraph is configured
     # such that imageAxisOrder == 'row-major'
     def center(self):
         corner_x, corner_y = self.pos().x(), self.pos().y()
-        return (round(corner_x + self.size().x() / 2), round(corner_y + self.size().y() / 2))
+        return (
+            round(corner_x + self.size().x() / 2),
+            round(corner_y + self.size().y() / 2),
+        )
 
     def set_center(self, x, y):
         left = x - self.size().x() / 2
         bottom = y - self.size().y() / 2
         self.setPos(left, bottom)
+
+
 # -*- coding: utf-8 -*-
 
-description = (
-    """Auto-determine the Bragg peak positions and add manually those not found. Subsequent calculation will optimize and realign the Bragg peaks to local maxima. """
-)
+description = """Auto-determine the Bragg peak positions and add manually those not found. Subsequent calculation will optimize and realign the Bragg peaks to local maxima. """
 vertices_help = """This is the number of vertices you expect the projection of the Brilluoin
 zone to have. Since this tool is just a visualization aid, this ensures only robustly determined
 Brilluoin zones will be computed."""
 
+
 class BraggPeakDialog(QtWidgets.QDialog):
     """
     Modal dialog to determine Bragg peak locations and corresponding
     2D projections of Brilluoin zones
     """
 
     bragg_peak_signal = QtCore.pyqtSignal(dict)
@@ -70,27 +75,29 @@
         self.viewer = pg.ImageView(parent=self)
         self.viewer.setSizePolicy(
             QtWidgets.QSizePolicy.MinimumExpanding,
             QtWidgets.QSizePolicy.MinimumExpanding,
         )
         self.viewer.setImage(image)
         if pixel_width is None:
-            pixel_width = 1.4e-5 #default to Gatan pixel width
-        self.bbox_size = int(7e-4 / pixel_width) #7e-4 m^-1 is about what looks right to cover most bragg peaks
+            pixel_width = 1.4e-5  # default to Gatan pixel width
+        self.bbox_size = int(
+            7e-4 / pixel_width
+        )  # 7e-4 m^-1 is about what looks right to cover most bragg peaks
         self.center_finder = RectROIWithCenter(
-            pos=np.array(image.shape) / 2 - 100, size=[self.bbox_size, self.bbox_size]#, pen=pg.mkPen("r")
+            pos=np.array(image.shape) / 2 - 100,
+            size=[self.bbox_size, self.bbox_size],  # , pen=pg.mkPen("r")
         )
         # self.autocenter = autocenter(self._image, self._mask)
         # self.center_finder.set_center(self.autocenter[1], self.autocenter[0])
         if center is not None and center != (0, 0):
             self.center_finder.set_center(*center)
 
         self.viewer.getView().addItem(self.center_finder)
 
-
         self.accept_btn = QtWidgets.QPushButton("Calculate", self)
         self.accept_btn.clicked.connect(self.accept)
 
         self.cancel_btn = QtWidgets.QPushButton("Cancel", self)
         self.cancel_btn.clicked.connect(self.reject)
         self.cancel_btn.setDefault(True)
 
@@ -111,15 +118,15 @@
         self.add_circ_mask_btn.clicked.connect(self.add_bragg_peak)
         self.add_circ_mask_btn.setEnabled(False)
 
         self.vertices_widget = QtWidgets.QSpinBox(parent=self)
         self.vertices_widget.setRange(1, 12)
         self.vertices_widget.setValue(6)
         self.vertices_widget.setToolTip(vertices_help)
-    
+
         self.vertices_layout = QtWidgets.QFormLayout()
         self.vertices_layout.addRow("Number of vertices:", self.vertices_widget)
 
         btns = QtWidgets.QHBoxLayout()
         btns.addWidget(self.accept_btn)
         btns.addWidget(self.cancel_btn)
 
@@ -149,42 +156,39 @@
         self.setLayout(self.layout)
 
         self.initiate_autopeaks()
 
     @QtCore.pyqtSlot()
     def add_bragg_peak(self):
         new_roi = pg.RectROI(
-            pos=self._resolution/2,
-            size=(self.bbox_size,self.bbox_size),
-            resizable=False
+            pos=self._resolution / 2,
+            size=(self.bbox_size, self.bbox_size),
+            resizable=False,
         )
         self.viewer.addItem(new_roi)
         self.__bragg_peak_items.append(new_roi)
 
-
     @QtCore.pyqtSlot()
     def accept(self):
         # Calculating the center position assumes that PyQtGraph is configured
         # such that imageAxisOrder == 'row-major'
-        
+
         for item in self.__bragg_peak_items:
             self.__bragg_peaks.append([item.pos().x(), item.pos().y()])
-        params = {
-            "peaks" : self.__bragg_peaks,
-            "sym" : int(self.vertices_widget.value())
-        }
+        params = {"peaks": self.__bragg_peaks, "sym": int(self.vertices_widget.value())}
         self.bragg_peak_signal.emit(params)
         super().accept()
 
     @QtCore.pyqtSlot()
     def initiate_autopeaks(self):
         """Automatically determine the bragg peaks
         and move the center-finder accordingly"""
         self._worker = AutobraggpeakThread(
-            function=bragg_peaks, kwargs=dict(im=self._image, mask=self._mask, min_dist=self.bbox_size)
+            function=bragg_peaks,
+            kwargs=dict(im=self._image, mask=self._mask, min_dist=self.bbox_size),
         )
 
         self._worker.results_signal.connect(self.set_peaks)
         self._worker.in_progress_signal.connect(self.busy_indicator.toggle_animation)
         self._worker.in_progress_signal.connect(self.autopeak_btn.setDisabled)
         self._worker.start()
 
@@ -195,28 +199,32 @@
         self.__bragg_peak_items.clear()
 
         # self.__bragg_peak_items.append(self.center_finder)
         for idx, peak in enumerate(rc):
             r, c = peak
             self.__bragg_peak_items.append(
                 pg.RectROI(
-                    pos=(c-self.bbox_size//2, r-self.bbox_size//2), size=(self.bbox_size,self.bbox_size), movable=True, resizable=False, removable=True
+                    pos=(c - self.bbox_size // 2, r - self.bbox_size // 2),
+                    size=(self.bbox_size, self.bbox_size),
+                    movable=True,
+                    resizable=False,
+                    removable=True,
                 )
             )
         for item in self.__bragg_peak_items:
             self.viewer.addItem(item)
-        
+
         self.add_circ_mask_btn.setEnabled(True)
         self._worker.exit()
 
+
 class AutobraggpeakThread(WorkThread):
     results_signal = QtCore.pyqtSignal(object)
 
 
-
 def parse_range(range_str):
     """
     Parse an integer range into a list of numbers.
 
     Parameters
     ----------
     range_str : str
```

### Comparing `iris-ued-5.3.4/iris/gui/calibrate_q_dialog.py` & `iris-ued-5.3.5/iris/gui/calibrate_q_dialog.py`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/iris/gui/control_bar.py` & `iris-ued-5.3.5/iris/gui/control_bar.py`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/iris/gui/controller.py` & `iris-ued-5.3.5/iris/gui/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             self.error_message_signal.emit(exc)
             warnings.warn(exc, UserWarning)
 
     return aware_func
 
 
 class ErrorAware(type(QtCore.QObject)):
-    """ Metaclass for error-aware Qt applications. """
+    """Metaclass for error-aware Qt applications."""
 
     def __new__(meta, classname, bases, class_dict):
         new_class_dict = dict()
         for attr_name, attr in class_dict.items():
             if isinstance(attr, FunctionType):
                 attr = error_aware(attr)
             new_class_dict[attr_name] = attr
@@ -90,30 +90,27 @@
     status_message_signal = QtCore.pyqtSignal(str)
 
     raw_data_signal = QtCore.pyqtSignal(object)
     averaged_data_signal = QtCore.pyqtSignal(object, bool)
     powder_data_signal = QtCore.pyqtSignal(object, object)
     bragg_peaks_signal = QtCore.pyqtSignal(dict)
 
-
     time_series_signal = QtCore.pyqtSignal(object, object)
     powder_time_series_signal = QtCore.pyqtSignal(object, object)
 
     relative_powder_enable_signal = QtCore.pyqtSignal(bool)
     relative_averaged_enable_signal = QtCore.pyqtSignal(bool)
     powder_bgr_enable_signal = QtCore.pyqtSignal(bool)
     bragg_peak_enable_signal = QtCore.pyqtSignal(bool)
-    bz_enable_signal   = QtCore.pyqtSignal(bool)
+    bz_enable_signal = QtCore.pyqtSignal(bool)
 
     processing_progress_signal = QtCore.pyqtSignal(int)
     powder_promotion_progress = QtCore.pyqtSignal(int)
     angular_average_progress = QtCore.pyqtSignal(int)
 
-
-
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.worker = None
         self.raw_dataset = None
         self.dataset = None
 
         # Internal state for powder background removal. If True, display_powder_data
@@ -173,15 +170,14 @@
         self._parent = value
 
     # @QtCore.pyqtSlot()
     @parent.deleter
     def parent(self):
         del self._parent
 
-
     @QtCore.pyqtSlot(str)
     @QtCore.pyqtSlot(str, object)
     def log(self, message, level=logging.INFO):
         """
         Interface to the iris logger.
 
         ALL logging should go through the controller.
@@ -254,36 +250,35 @@
             )
 
         self.averaged_data_signal.emit(self._averaged_data_container, autocontrast)
         self.status_message_signal.emit(f"Displaying data at {timedelay:.3f}ps.")
 
     @QtCore.pyqtSlot()
     def display_powder_data(self):
-        """ Emit a powder data signal with/out background """
+        """Emit a powder data signal with/out background"""
         # Preallocation isn't so important for powder data because the whole block
         # is loaded
         self.powder_data_signal.emit(
             self.dataset.scattering_vector,
             self.dataset.powder_data(
                 timedelay=None, relative=self._relative_powder, bgr=self._bgr_powder
             ),
         )
 
     @QtCore.pyqtSlot()
     def display_bragg_peaks(self):
         params = {
-            "enable_peaks" : self._enable_bragg,
-            "peaks" : self.bragg_peaks,
-            "enable_bz" : self._enable_bz,
-            "bz" : self.bzs,
-            "n_vertices" : self.bz_vertices
+            "enable_peaks": self._enable_bragg,
+            "peaks": self.bragg_peaks,
+            "enable_bz": self._enable_bz,
+            "bz": self.bzs,
+            "n_vertices": self.bz_vertices,
         }
         self.bragg_peaks_signal.emit(params)
 
-    
     @QtCore.pyqtSlot(bool)
     def powder_background_subtracted(self, enable):
         """
         Toggle background subtraction for polycrystalline data.
 
         Parameters
         ----------
@@ -378,85 +373,88 @@
         params : dict
             Parameters are passed to `skued.powder_calq`.
         """
         self.dataset.powder_calq(**params)
         self.display_powder_data()
         self.status_message_signal.emit("Scattering vector range calibrated.")
 
-
     @QtCore.pyqtSlot(dict)
     @indicate_in_progress
     def optimize_bragg_peaks(self, params):
         """
-        Update Bragg peaks to actual local maxima, as well as identify BZ 
+        Update Bragg peaks to actual local maxima, as well as identify BZ
         using Voronoi diagramming
 
         Parameters
         ----------
         peaks : list
             Items returned from Bragg peak dialog
         """
         self.initially_run_bragg_signal.emit(True)
-        peaks = params['peaks']
-        symmetry = params['sym']
+        peaks = params["peaks"]
+        symmetry = params["sym"]
 
         from scipy.spatial import Voronoi
+
         current_view = self.dataset.diff_eq()
-        peaks = np.vstack((self.dataset.center[::-1],peaks))
+        peaks = np.vstack((self.dataset.center[::-1], peaks))
         new_peaks = np.array(peaks)
         for idx, peak in enumerate(peaks):
             # if idx == 0:
             #     c, r = peaks[idx]
             # else:
             r, c = peaks[idx]
             peak = np.asarray(peak).astype(int)
-            disk = DiskSelection(
-                shape=current_view.shape, center=peak[::-1], radius=25
-            )
+            disk = DiskSelection(shape=current_view.shape, center=peak[::-1], radius=25)
             r1, r2, c1, c2 = disk.bounding_box
             region = current_view[r1:r2, c1:c2]
             try:
                 true_peak_idx_local = np.where(region == region.max())
-                true_peak_idx_global = np.where(current_view == region[true_peak_idx_local])
+                true_peak_idx_global = np.where(
+                    current_view == region[true_peak_idx_local]
+                )
                 new_r, new_c = true_peak_idx_global[0][0], true_peak_idx_global[1][0]
             except:
-                if idx != 0:    print(f"Could not optimize peak {idx}")
+                if idx != 0:
+                    print(f"Could not optimize peak {idx}")
                 # self.log(f"Could not optimize peak {idx}", level=logging.DEBUG)
                 new_r, new_c = r, c
 
             new_peaks[idx] = np.array((new_r, new_c)).astype(int)
         self.bragg_peaks = new_peaks
 
-        #load BZs
-        self.__vor = Voronoi(new_peaks[:,[1,0]])
+        # load BZs
+        self.__vor = Voronoi(new_peaks[:, [1, 0]])
         self.__voronoi_regions = []
 
         for i, point_region in enumerate(self.__vor.point_region):
             region = self.__vor.regions[point_region]
             vr = VoronoiRegion(point_region)
             for r in region:
                 vr.add_vertex(r, self.__vor.vertices)
             vr.point_inside = (i, self.__vor.points[i])
             vr.set_center(self.__vor.points[i])
             self.__voronoi_regions.append(vr)
 
         for r in self.__voronoi_regions:
             if not r.is_inf:
-                verts = np.array(r.vertices).reshape(-1,2)
-                COND1 = np.all(np.sqrt(np.sum(verts**2, axis=1)) < int(0.95*current_view.shape[0]))
+                verts = np.array(r.vertices).reshape(-1, 2)
+                COND1 = np.all(
+                    np.sqrt(np.sum(verts**2, axis=1))
+                    < int(0.95 * current_view.shape[0])
+                )
                 COND2 = verts.shape[0] == symmetry
                 if COND1 and COND2:
                     r.add_visible_vertex(verts)
-            r.visible_vertices = np.array(r.visible_vertices).reshape(-1,2)
+            r.visible_vertices = np.array(r.visible_vertices).reshape(-1, 2)
             if r.visible_vertices.size != 0:
                 r.is_visible = True
         self.bzs = self.__voronoi_regions
         self.bz_vertices = symmetry
         # self.display_bragg_peaks(new_peaks)
-        
 
     @QtCore.pyqtSlot(dict)
     def update_metadata(self, metadata):
         """
         Update metadata attributes in DiffractionDataset
 
         Parameters
@@ -562,15 +560,15 @@
             }
         )
         self.display_raw_data(timedelay_index=0, scan=min(self.raw_dataset.scans))
         self.status_message_signal.emit(path + " loaded.")
 
     @QtCore.pyqtSlot()
     def close_raw_dataset(self):
-        """ Close raw dataset. """
+        """Close raw dataset."""
         self.raw_dataset = None
         self.raw_dataset_loaded_signal.emit(False)
         self.raw_data_signal.emit(None)
 
         self.status_message_signal.emit("Raw dataset closed.")
 
     @QtCore.pyqtSlot(str)
@@ -606,15 +604,15 @@
         # therefore, we open the file and do nothing
         # TODO: stop writing datasets in PowderDiffractionDataset.__init__
         #       since the GUI will only open datasets in read-mode by default
         if cls is PowderDiffractionDataset:
             with cls(path, mode="r+"):
                 pass
 
-        self.dataset = cls(path, mode="r")
+        self.dataset = cls(path, mode="r+")
         self.dataset_metadata.emit(self.dataset.metadata)
 
         # Initialize containers
         # This *must* be done before data is displayed
         self._averaged_data_container = np.empty(
             shape=self.dataset.resolution,
             dtype=self.dataset.diffraction_group["intensity"].dtype,
@@ -634,15 +632,15 @@
             # hence, switch views to the relevant widgets
             self.processed_dataset_loaded_signal.emit(True)
 
         self.status_message_signal.emit(path + " loaded.")
 
     @QtCore.pyqtSlot()
     def close_dataset(self):
-        """ Close current DiffractionDataset. """
+        """Close current DiffractionDataset."""
         with suppress(AttributeError):  # in case self.dataset is None
             self.dataset.close()
         self.dataset = None
         self.processed_dataset_loaded_signal.emit(False)
         self.powder_dataset_loaded_signal.emit(False)
 
         self.averaged_data_signal.emit(None, True)
@@ -796,15 +794,15 @@
 def calculate_azimuthal_averages(**kwargs):
     """Create a PowderDiffractionDataset from a DiffractionDataset. If azimuthal averages
     were already calculated, recalculate them."""
     filename = kwargs.pop("filename")
 
     # Determine if azimuthal averages have already been computed
     recomputed = False
-    with PowderDiffractionDataset(filename, 'r+') as d:
+    with PowderDiffractionDataset(filename, "r+") as d:
         if PowderDiffractionDataset._powder_group_name in d:
             # We simply need to recompute the azimuthal averages
             recomputed = True
             d.compute_angular_averages(**kwargs)
 
     if recomputed:
         return filename
@@ -845,15 +843,15 @@
     """
     with PowderDiffractionDataset(fname, mode="r+") as dset:
         dset.compute_baseline(**kwargs)
     return fname
 
 
 def process(**kwargs):
-    """ Process a RawDataset into a DiffractionDataset """
+    """Process a RawDataset into a DiffractionDataset"""
     with DiffractionDataset.from_raw(**kwargs) as dset:
         fname = dset.filename
     return fname
 
 
 class VoronoiRegion:
     """
@@ -862,34 +860,35 @@
 
     Parameters
     ----------
 
     region_id: type(int)
         Defines the ID number of this particular Voronoi region
 
-    
+
     """
+
     def __init__(self, region_id):
         self.id = region_id
         self.vertices = []
         self.is_inf = False
         self.point_inside = None
         self.visible_vertices = []
         self.is_visible = False
 
     def __str__(self):
-        text = f'region id={self.id}'
+        text = f"region id={self.id}"
         if self.point_inside:
             point_idx, point = self.point_inside
-            text = f'{text}[point:{point}(point_id:{point_idx})]'
-        text += ', vertices: '
+            text = f"{text}[point:{point}(point_id:{point_idx})]"
+        text += ", vertices: "
         if self.is_inf:
-            text += '(inf)'
+            text += "(inf)"
         for v in self.vertices:
-            text += f'{v}'
+            text += f"{v}"
         return text
 
     def __repr__(self):
         return str(self)
 
     def add_vertex(self, vertex, vertices):
         if vertex == -1:
```

### Comparing `iris-ued-5.3.4/iris/gui/data_viewer.py` & `iris-ued-5.3.5/iris/gui/data_viewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,51 +79,51 @@
         y1 = round(max(0, rect.topLeft().x()))
         y2 = round(max(0, rect.x() + rect.width()))
 
         self.timeseries_rect_signal.emit((x1, x2, y1, y2))
 
     @QtCore.pyqtSlot(object)
     def update_cursor_info(self, event):
-        """ Provide information about the cursor (position, value, etc) """
+        """Provide information about the cursor (position, value, etc)"""
         mouse_point = self.image_viewer.getView().mapSceneToView(event[0])
         i, j = int(mouse_point.x()), int(mouse_point.y())
         try:
             val = self.image_viewer.getImageItem().image[j, i]
         except IndexError:
             val = 0
         self.cursor_info_widget.setText(
             f"Position: ({i},{j}) | Pixel value: {val:.2f} cnts"
         )
 
     @QtCore.pyqtSlot(bool)
     def toggle_peak_dynamics(self, toggle):
-        """ Toggle interactive peak dynamics region-of-interest"""
+        """Toggle interactive peak dynamics region-of-interest"""
         if toggle:
             self.timeseries_rect_region.show()
         else:
             self.timeseries_rect_region.hide()
             self.roi_topleft_text.setText("")
             self.roi_bottomright_text.setText("")
 
         self.time_series_widget.setVisible(toggle)
 
     @QtCore.pyqtSlot(bool)
     def toggle_roi_bounds_text(self, enable):
-        """ Toggle showing array indices around the peak dynamics region-of-interest """
+        """Toggle showing array indices around the peak dynamics region-of-interest"""
         if enable:
             self.timeseries_rect_signal.connect(self._update_roi_bounds_text)
             self.update_timeseries_rect()
         else:
             self.roi_topleft_text.setText("")
             self.roi_bottomright_text.setText("")
             self.timeseries_rect_signal.disconnect(self._update_roi_bounds_text)
 
     @QtCore.pyqtSlot(tuple)
     def _update_roi_bounds_text(self, rect):
-        """ Update the ROI bounds text based on the bounds in ``rect`` """
+        """Update the ROI bounds text based on the bounds in ``rect``"""
         x1, x2, y1, y2 = rect
         self.roi_topleft_text.setPos(y1, x1)
         self.roi_topleft_text.setText(f"({y1},{x1})")
 
         self.roi_bottomright_text.setPos(y2, x2)
         self.roi_bottomright_text.setText(f"({y2},{x2})")
 
@@ -164,45 +164,45 @@
         Parameters
         ----------
         peaks : list of 2-tuple
             List of tuples [row, col] where Bragg peaks are located.
         """
         enabled_peaks = params["enable_peaks"]
         peaks = params["peaks"]
-        enabled_bzs = params['enable_bz']
-        voronoi_regions = params['bz']
-        n_vertices = params['n_vertices']
-        self.bbox_size = int(0.025*self.image_viewer.getImageItem().image.shape[0])
+        enabled_bzs = params["enable_bz"]
+        voronoi_regions = params["bz"]
+        n_vertices = params["n_vertices"]
+        self.bbox_size = int(0.025 * self.image_viewer.getImageItem().image.shape[0])
         for item in self.__bragg_peak_items:
             self.image_viewer.removeItem(item)
         self.__bragg_peak_items.clear()
         if enabled_peaks:
             for idx, peak in enumerate(peaks):
                 r, c = peak
                 generator = generate_connections(4)
                 nodes = list()
                 for _ in range(4):
                     nodes.append(next(generator))
-                nodes = np.array(nodes).reshape(-1,2)
+                nodes = np.array(nodes).reshape(-1, 2)
                 self.__bragg_peak_items.append(
                     # pg.RectROI(
                     #     pos=(c-25, r-25), size=(50,50), movable=False, resizable=False, removable=False
                     # )
                     pg.GraphItem(
-                        pos = np.array(
+                        pos=np.array(
                             [
-                                [c-self.bbox_size//2, r-self.bbox_size//2],
-                                [c-self.bbox_size//2, r+self.bbox_size//2],
-                                [c+self.bbox_size//2, r+self.bbox_size//2],
-                                [c+self.bbox_size//2,r-self.bbox_size//2]
+                                [c - self.bbox_size // 2, r - self.bbox_size // 2],
+                                [c - self.bbox_size // 2, r + self.bbox_size // 2],
+                                [c + self.bbox_size // 2, r + self.bbox_size // 2],
+                                [c + self.bbox_size // 2, r - self.bbox_size // 2],
                             ]
                         ),
-                        adj = nodes,
+                        adj=nodes,
                         pen=pg.mkPen("r"),
-                        size=0
+                        size=0,
                     )
                 )
             for item in self.__bragg_peak_items:
                 self.image_viewer.addItem(item)
 
         for item in self.__bz_items:
             self.image_viewer.removeItem(item)
@@ -211,26 +211,23 @@
             for r in voronoi_regions:
                 if r.is_visible:
                     generator = generate_connections(n_vertices)
                     N = np.array(r.vertices).reshape(-1, 2).shape[0]
                     nodes = list()
                     for _ in range(N):
                         nodes.append(next(generator))
-                    nodes = np.array(nodes).reshape(-1,2)
+                    nodes = np.array(nodes).reshape(-1, 2)
                     self.__bz_items.append(
-                        pg.GraphItem(
-                            pos = np.array(r.vertices).reshape(-1, 2),
-                            adj = nodes
-                        )
+                        pg.GraphItem(pos=np.array(r.vertices).reshape(-1, 2), adj=nodes)
                     )
             for item in self.__bz_items:
                 self.image_viewer.addItem(item)
 
+
 def generate_connections(sym):
     """
     Generator of the connections between points to graph closed polygons in pyqtgraph
     """
     num = 0
     while True:
-        yield (num, (num+1)%(sym))
+        yield (num, (num + 1) % (sym))
         num += 1
-
```

### Comparing `iris-ued-5.3.4/iris/gui/gui.py` & `iris-ued-5.3.5/iris/gui/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         self.controller.angular_average_progress.connect(self.progress_bar.setValue)
 
         # Status bar ----------------------------------------------------------
         # Operation in progress widget
         # Including custom 'busy' indicator
         status_bar = QtWidgets.QStatusBar(parent=self)
         self.controller.status_message_signal.connect(
-            lambda msg: status_bar.showMessage(msg, 20e3)
+            lambda msg: status_bar.showMessage(msg, 20_000)
         )
         self.setStatusBar(status_bar)
 
         # Progress bar added to status bar ------------------------------------
         status_bar.addPermanentWidget(self.progress_bar)
 
         # Busy indicator ------------------------------------------------------
@@ -311,15 +311,14 @@
         self.calculate_bragg_peaks_action.triggered.connect(
             self.launch_calculate_bragg_peaks_dialog
         )
         self.controller.processed_dataset_loaded_signal.connect(
             self.calculate_bragg_peaks_action.setEnabled
         )
 
-
         self.update_metadata_action = QtWidgets.QAction(
             QtGui.QIcon(join(IMAGE_FOLDER, "save.png")),
             "& Update dataset metadata",
             self,
         )
         self.update_metadata_action.triggered.connect(self.launch_metadata_edit_dialog)
         self.controller.processed_dataset_loaded_signal.connect(
@@ -388,45 +387,34 @@
         self.show_diff_relative_action.toggled.connect(
             self.controller.enable_averaged_relative
         )
         self.controller.processed_dataset_loaded_signal.connect(
             self.show_diff_relative_action.setEnabled
         )
 
-        self.show_bragg_peaks_action = QtWidgets.QAction(
-            "& Show Bragg peaks", self
-        )
+        self.show_bragg_peaks_action = QtWidgets.QAction("& Show Bragg peaks", self)
         self.show_bragg_peaks_action.setCheckable(True)
         self.controller.bragg_peak_enable_signal.connect(
             self.show_bragg_peaks_action.setChecked
         )
-        self.show_bragg_peaks_action.toggled.connect(
-            self.controller.enable_bragg
-        )
+        self.show_bragg_peaks_action.toggled.connect(self.controller.enable_bragg)
         self.controller.initially_run_bragg_signal.connect(
             self.show_bragg_peaks_action.setEnabled
         )
         self.show_bragg_peaks_action.setEnabled(False)
 
-        self.show_BZ_action = QtWidgets.QAction(
-            "& Show Brilluoin zones", self
-        )
+        self.show_BZ_action = QtWidgets.QAction("& Show Brilluoin zones", self)
         self.show_BZ_action.setCheckable(True)
-        self.controller.bz_enable_signal.connect(
-            self.show_BZ_action.setChecked
-        )
-        self.show_BZ_action.toggled.connect(
-            self.controller.enable_bz
-        )
+        self.controller.bz_enable_signal.connect(self.show_BZ_action.setChecked)
+        self.show_BZ_action.toggled.connect(self.controller.enable_bz)
         self.controller.initially_run_bragg_signal.connect(
             self.show_BZ_action.setEnabled
         )
         self.show_BZ_action.setEnabled(False)
 
-
         self.show_powder_relative_action = QtWidgets.QAction(
             "& Toggle relative dynamics", self
         )
         self.show_powder_relative_action.setCheckable(True)
         self.controller.relative_powder_enable_signal.connect(
             self.show_powder_relative_action.setChecked
         )
@@ -477,17 +465,15 @@
         )
         self.diffraction_dataset_display_options_menu.addAction(
             self.show_diff_relative_action
         )
         self.diffraction_dataset_display_options_menu.addAction(
             self.show_bragg_peaks_action
         )
-        self.diffraction_dataset_display_options_menu.addAction(
-            self.show_BZ_action
-        )
+        self.diffraction_dataset_display_options_menu.addAction(self.show_BZ_action)
 
         self.powder_dataset_display_options_menu.addAction(
             self.show_powder_relative_action
         )
         self.powder_dataset_display_options_menu.addAction(
             self.toggle_powder_background_action
         )
@@ -652,21 +638,17 @@
             self.controller.dataset.diff_data(self.controller.dataset.time_points[0]),
             mask=self.controller.dataset.valid_mask,
             pixel_width=self.controller.dataset.pixel_width,
             center=self.controller.dataset.center,
             parent=self,
         )
         bragg_dialog.resize(0.75 * self.size())
-        bragg_dialog.bragg_peak_signal.connect(
-            self.controller.optimize_bragg_peaks
-        )
+        bragg_dialog.bragg_peak_signal.connect(self.controller.optimize_bragg_peaks)
         bragg_dialog.exec_()
-        bragg_dialog.bragg_peak_signal.disconnect(
-            self.controller.optimize_bragg_peaks
-        )
+        bragg_dialog.bragg_peak_signal.disconnect(self.controller.optimize_bragg_peaks)
 
     @QtCore.pyqtSlot()
     def launch_symmetrize_dialog(self):
         symmetrize_dialog = SymmetrizeDialog(
             parent=self,
             image=self.controller.dataset.diff_data(
                 timedelay=self.controller.dataset.time_points[0]
@@ -733,15 +715,15 @@
         dialog.resize(0.75 * self.size())
         dialog.calibration_parameters.connect(self.controller.powder_calq)
         dialog.exec_()
         dialog.calibration_parameters.disconnect(self.controller.powder_calq)
 
     @QtCore.pyqtSlot(bool)
     def update_available(self, available):
-        """ Handle UI in case an update is available or not. """
+        """Handle UI in case an update is available or not."""
         if available:
             self.update_action.setEnabled(True)
             self.update_action.setText("An update is available!")
         else:
             self.update_action.setEnabled(False)
             self.update_action.setText("No updates available.")
 
@@ -753,15 +735,15 @@
         if not path:
             return
         self.raw_dataset_path_signal.emit(path, cls)
 
     @QtCore.pyqtSlot()
     def load_dataset(self):
         path = self.file_dialog.getOpenFileName(
-            parent=self, caption="Load dataset", filter="*.hdf5"
+            parent=self, caption="Load dataset", filter="HDF5-files (*.h5 *.hdf5)"
         )[0]
         if not path:
             return
         self.dataset_path_signal.emit(path)
 
     @QtCore.pyqtSlot()
     def load_single_picture(self):
@@ -792,15 +774,15 @@
         qr = self.frameGeometry()
         cp = QtWidgets.QDesktopWidget().availableGeometry().center()
         qr.moveCenter(cp)
         self.move(qr.topLeft())
 
     @QtCore.pyqtSlot()
     def install_plugin(self):
-        """ Load plug-in. """
+        """Load plug-in."""
         explanation = INSTALL_PLUGIN_HELP.format(dir=PLUGIN_DIR)
 
         QtWidgets.QMessageBox.information(self, "Loading a plug-in", explanation)
 
         path = self.file_dialog.getOpenFileName(
             parent=self, caption="Load plug-in file", filter="Python source (*.py)"
         )[0]
@@ -808,15 +790,15 @@
             return
 
         install_plugin(path)
         self.create_load_raw_menu()
 
     @QtCore.pyqtSlot()
     def show_about(self):
-        """ Show the About information """
+        """Show the About information"""
 
         return QtWidgets.QMessageBox.about(self, "About Iris", make_about_string())
 
 
 def make_about_string():
     import h5py
     import sys
```

### Comparing `iris-ued-5.3.4/iris/gui/metadata_edit_dialog.py` & `iris-ued-5.3.5/iris/gui/metadata_edit_dialog.py`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/iris/gui/powder_viewer.py` & `iris-ued-5.3.5/iris/gui/powder_viewer.py`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/iris/gui/processing_dialog.py` & `iris-ued-5.3.5/iris/gui/processing_dialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,20 +35,24 @@
 
 exclude_scans_help = """ Specify scans to exclude comma separated,
 e.g. 3,4, 5, 10, 32. """.replace(
     "\n", ""
 )
 
 ngon_help = """ Create polgyon with arbitrary number of vertices and vertex locations. Click in the middle
-of line segments to generate a new vertex handle (which can be deleted).""".replace("\n", "")
+of line segments to generate a new vertex handle (which can be deleted).""".replace(
+    "\n", ""
+)
 
 description = """Set the processing parameters for the dataset, including mask generation. Arbitrary masks can
  be uploaded by dragging and dropping the file into the image viewport. These masks must be Numpy arrays with invalid 
 pixels indicated by True.
-""".replace("\n","")
+""".replace(
+    "\n", ""
+)
 
 DTYPE_NAMES = {
     "Auto": None,
     "64-bit floats": np.float64,
     "32-bit floats": np.float32,
     "16-bit floats": np.float16,
     "64-bit integers": np.int64,
@@ -63,15 +67,15 @@
     def __init__(self, image, **kwargs):
         super().__init__(**kwargs)
 
         self.resolution = np.array(image.shape)
         self.loaded_mask = np.zeros_like(image, dtype=bool)
         self.rect_masks = list()  # list of pg.ROI objects
         self.circ_masks = list()
-        self.arb_masks  = list()
+        self.arb_masks = list()
 
         self.viewer = pg.ImageView(parent=self)
         self.viewer.setImage(image)
         self.viewer.setSizePolicy(
             QtWidgets.QSizePolicy.MinimumExpanding,
             QtWidgets.QSizePolicy.MinimumExpanding,
         )
@@ -102,29 +106,30 @@
         self.viewer.addItem(new_roi)
         self.circ_masks.append(new_roi)
 
     @QtCore.pyqtSlot()
     def add_arb_mask(self, pos=None, append=True):
         if pos is None:
             positions = [
-                    (0.6*self.resolution[0], 0.6*self.resolution[1]),
-                    (0.6*self.resolution[0], 0.4*self.resolution[1]),
-                    (0.4*self.resolution[0], 0.4*self.resolution[1]),
-                    (0.4*self.resolution[0], 0.6*self.resolution[1])
-                ]
+                (0.6 * self.resolution[0], 0.6 * self.resolution[1]),
+                (0.6 * self.resolution[0], 0.4 * self.resolution[1]),
+                (0.4 * self.resolution[0], 0.4 * self.resolution[1]),
+                (0.4 * self.resolution[0], 0.6 * self.resolution[1]),
+            ]
         else:
             positions = pos
         new_roi = pg.PolyLineROI(
-            positions = positions,
-            closed=True, pen=pg.mkPen("r", width=4)
+            positions=positions, closed=True, pen=pg.mkPen("r", width=4)
         )
-        
+
         self.viewer.addItem(new_roi)
-        if append: self.arb_masks.append(new_roi)
-        else: return new_roi
+        if append:
+            self.arb_masks.append(new_roi)
+        else:
+            return new_roi
 
     @QtCore.pyqtSlot()
     def show_preview_mask(self):
         image = np.array(self.viewer.image)
         mask = self.composite_mask()
         image[mask] = False
 
@@ -148,15 +153,31 @@
 
     def composite_mask(self):
         """Returns composite mask where invalid pixels are marked as True"""
         # Initially, all pixels are valid
         mask = np.zeros_like(self.loaded_mask, dtype=bool)
         if len(self.circ_masks + self.rect_masks + self.arb_masks) == 0:
             return self.loaded_mask
-
+        if self.arb_masks:
+            for arb_mask in self.arb_masks:
+                locs = np.array([(p[1].x(), p[1].y()) for p in arb_mask.getLocalHandlePositions()])
+                all_identical = True
+                for idp, point in enumerate(locs):
+                    new_pt = np.clip(point, a_min = 0, a_max = self.resolution)
+                    if not np.array_equal(point, new_pt):
+                        all_identical = False
+                        locs[idp,:] = new_pt
+                if not all_identical:
+                    trimmed_arb_mask = self.add_arb_mask(pos = locs, append = False)
+                    self.viewer.removeItem(trimmed_arb_mask)
+                else:
+                    trimmed_arb_mask = arb_mask
+                width, height = int(trimmed_arb_mask.parentBounds().width()), int(trimmed_arb_mask.parentBounds().height())
+                left, top = int(trimmed_arb_mask.parentBounds().left()), int(trimmed_arb_mask.parentBounds().top())
+                mask[top:top+height, left:left+width ] = trimmed_arb_mask.renderShapeMask(width,height).astype(bool).T
         # No need to compute xx, yy, and rr if there are no
         # circular masks, hence the check for empty list
         if self.circ_masks:
             xx, yy = np.meshgrid(
                 np.arange(0, mask.shape[0]), np.arange(0, mask.shape[1])
             )
             rr = np.empty_like(xx)
@@ -172,62 +193,56 @@
         if self.rect_masks:
             for rect_mask in self.rect_masks:
                 (x_slice, y_slice), _ = rect_mask.getArraySlice(
                     data=mask, img=self.viewer.getImageItem()
                 )
                 mask[x_slice, y_slice] = True
         
-        if self.arb_masks:
-            for arb_mask in self.arb_masks:
-                locs = np.array([(p[1].x(), p[1].y()) for p in arb_mask.getLocalHandlePositions()])
-                all_identical = True
-                for idp, point in enumerate(locs):
-                    new_pt = np.clip(point, a_min = 0, a_max = self.resolution)
-                    if not np.array_equal(point, new_pt):
-                        all_identical = False
-                        locs[idp,:] = new_pt
-                if not all_identical:
-                    trimmed_arb_mask = self.add_arb_mask(pos = locs, append = False)
-                    self.viewer.removeItem(trimmed_arb_mask)
-                else:
-                    trimmed_arb_mask = arb_mask
-                width, height = int(trimmed_arb_mask.parentBounds().width()), int(trimmed_arb_mask.parentBounds().height())
-                left, top = int(trimmed_arb_mask.parentBounds().left()), int(trimmed_arb_mask.parentBounds().top())
-                mask[top:top+height, left:left+width ] = trimmed_arb_mask.renderShapeMask(width,height).astype(bool).T
         return np.logical_or(self.loaded_mask, mask)
-            
+
     def toggleinversionLoadedMask(self):
         try:
             self.loaded_mask = ~self.loaded_mask
             self.parent().parent.controller.logger.info("Inverted loaded mask.")
         except:
             self.parent().parent.controller.logger.error("Error inverting loaded mask.")
 
     def dragEnterEvent(self, e):
         if e.mimeData().hasUrls():
             fname = e.mimeData().urls()[0].path()
-            if 'npy' in fname:
+            if "npy" in fname:
                 e.accept()
             else:
-                self.parent().parent.controller.logger.error(f'Mask given by {fname} does not have type numpy.ndarray.')
+                self.parent().parent.controller.logger.error(
+                    f"Mask given by {fname} does not have type numpy.ndarray."
+                )
                 e.ignore()
         else:
-            self.parent().parent.controller.logger.error(f'Item dropped is not a file URL.')
+            self.parent().parent.controller.logger.error(
+                f"Item dropped is not a file URL."
+            )
             e.ignore()
 
     def dropEvent(self, e):
         fname = e.mimeData().urls()[0].path()
         try:
             self.loaded_mask = np.logical_or(self.loaded_mask, np.load(fname))
             if self.loaded_mask.shape == tuple(self.resolution):
-                self.parent().parent.controller.logger.info(f'Successfully loaded {fname} as processing mask.')
+                self.parent().parent.controller.logger.info(
+                    f"Successfully loaded {fname} as processing mask."
+                )
             else:
-                self.parent().parent.controller.logger.error(f'Mask dimensions in {fname} do not agree with dataset dimensions. Did not load mask.')
+                self.parent().parent.controller.logger.error(
+                    f"Mask dimensions in {fname} do not agree with dataset dimensions. Did not load mask."
+                )
         except:
-            self.parent().parent.controller.logger.error(f'Error loading {fname} as the processing mask. ')
+            self.parent().parent.controller.logger.error(
+                f"Error loading {fname} as the processing mask. "
+            )
+
 
 class ProcessingDialog(QtWidgets.QDialog):
     """
     Modal dialog used to select dataset processing options.
     """
 
     processing_parameters_signal = QtCore.pyqtSignal(dict)
@@ -236,15 +251,15 @@
     def __init__(self, raw, **kwargs):
         """
         Parameters
         ----------
         raw : AbstractRawDataset instance
         """
         super().__init__(**kwargs)
-        self.parent = kwargs['parent']
+        self.parent = kwargs["parent"]
         self.setModal(True)
         self.setWindowTitle("Diffraction Dataset Processing")
 
         self.error_message_signal.connect(self.show_error_message)
 
         image = raw.raw_data(timedelay=raw.time_points[0], scan=raw.scans[0], bgr=True)
         self.mask_widget = MaskCreator(image, parent=self)
@@ -329,19 +344,23 @@
         self.add_arb_mask_btn = QtWidgets.QPushButton("Add n-gon mask", self)
         self.add_arb_mask_btn.setSizePolicy(
             QtWidgets.QSizePolicy.Maximum, QtWidgets.QSizePolicy.Maximum
         )
         self.add_arb_mask_btn.clicked.connect(self.mask_widget.add_arb_mask)
         self.add_arb_mask_btn.setToolTip(ngon_help)
 
-        self.toggle_inversion_loaded_mask_btn = QtWidgets.QPushButton("Invert loaded mask", self)
+        self.toggle_inversion_loaded_mask_btn = QtWidgets.QPushButton(
+            "Invert loaded mask", self
+        )
         self.toggle_inversion_loaded_mask_btn.setSizePolicy(
             QtWidgets.QSizePolicy.Maximum, QtWidgets.QSizePolicy.Maximum
         )
-        self.toggle_inversion_loaded_mask_btn.clicked.connect(self.mask_widget.toggleinversionLoadedMask)
+        self.toggle_inversion_loaded_mask_btn.clicked.connect(
+            self.mask_widget.toggleinversionLoadedMask
+        )
 
         self.preview_mask_btn = QtWidgets.QPushButton("Preview mask", self)
         self.preview_mask_btn.setSizePolicy(
             QtWidgets.QSizePolicy.Maximum, QtWidgets.QSizePolicy.Maximum
         )
         self.preview_mask_btn.clicked.connect(self.mask_widget.show_preview_mask)
```

### Comparing `iris-ued-5.3.4/iris/gui/qbusyindicator.py` & `iris-ued-5.3.5/iris/gui/qbusyindicator.py`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/iris/gui/qlogger.py` & `iris-ued-5.3.5/iris/gui/qlogger.py`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/iris/gui/symmetrize_dialog.py` & `iris-ued-5.3.5/iris/gui/symmetrize_dialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     def show_error_message(self, msg):
         self.error_dialog = QtGui.QErrorMessage(parent=self)
         self.error_dialog.showMessage(msg)
 
     @QtCore.pyqtSlot()
     def accept(self):
         self.file_dialog = QtWidgets.QFileDialog(parent=self)
-        filename = self.file_dialog.getSaveFileName(filter="*.hdf5")[0]
+        filename = self.file_dialog.getSaveFileName(filter="HDF5-files (*.h5 *.hdf5)")[0]
         if filename == "":
             return
 
         center = self.center_finder.center()
 
         params = {
             "center": center,
```

### Comparing `iris-ued-5.3.4/iris/gui/time_series_widget.py` & `iris-ued-5.3.5/iris/gui/time_series_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         # Internal state on whether or not to 'connect the dots'
         self._time_series_connect = False
         self._symbol_size = 5
 
         # Internal memory on last time-series info
         self._last_times = None
         self._last_intensities_abs = None
+        self._last_norm_mask = None
         self._refresh_signal.connect(self.plot)
 
         self.connect_widget = QtWidgets.QCheckBox("Connect time-series", self)
         self.connect_widget.toggled.connect(self.enable_connect)
 
         self.symbol_size_widget = QtWidgets.QSpinBox(parent=self)
         self.symbol_size_widget.setRange(1, 25)
@@ -117,23 +118,26 @@
         time_points : `~numpy.ndarray`, shape (N,)
             Time-delays [ps]
         intensity : `~numpy.ndarray`, shape (N,)
             Diffracted intensity in absolute units.
         """
         self._last_times = np.asarray(time_points)
         self._last_intensities_abs = np.asarray(intensity)
+        self._last_norm_mask = self._last_times < 0
+        if self._last_norm_mask.sum() == 0:
+            self._last_norm_mask[0] = True
 
         # Normalize to intensity before time-zero
         # Note that the change in units is taken care of in the toggle_absolute_intensity method
         absolute = self.absolute_intensity_widget.isChecked()
         intensity = (
             self._last_intensities_abs
             if absolute
             else self._last_intensities_abs
-            / np.mean(self._last_intensities_abs[self._last_times < 0])
+            / np.mean(self._last_intensities_abs[self._last_norm_mask])
         )
 
         # Only compute the colors if number of time-points changes or first time
         pens, brushes = pens_and_brushes(len(time_points))
 
         connect_kwargs = {"pen": None} if not self._time_series_connect else dict()
         self.plot_widget.plot(
```

### Comparing `iris-ued-5.3.4/iris/gui/update.py` & `iris-ued-5.3.5/iris/gui/update.py`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/iris/meta.py` & `iris-ued-5.3.5/iris/meta.py`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/iris/plugins.py` & `iris-ued-5.3.5/iris/plugins.py`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/iris/powder.py` & `iris-ued-5.3.5/iris/powder.py`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/iris/raw.py` & `iris-ued-5.3.5/iris/raw.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ===================
 """
 from abc import abstractmethod
 from collections import OrderedDict
 from contextlib import AbstractContextManager
 from functools import wraps, partial
 from pathlib import Path
-import multiprocessing as mp
+from multiprocessing import Pool
 
 import numpy as np
 
 from npstreams import average, itercopy, peek
 from skued import ialign
 
 from .meta import ExperimentalParameter, MetaRawDataset
```

### Comparing `iris-ued-5.3.4/iris/tests/__init__.py` & `iris-ued-5.3.5/iris/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/iris/tests/plugin_fixture.py` & `iris-ued-5.3.5/iris/tests/plugin_fixture.py`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/iris/tests/test_dataset.py` & `iris-ued-5.3.5/iris/tests/test_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import sys
 import os
 from contextlib import suppress
 from itertools import repeat
+from pathlib import Path
 from tempfile import gettempdir
 
 import numpy as np
+import pytest
+from flaky import flaky
 from numpy.random import random
+from skued import (ArbitrarySelection, DiskSelection, RectSelection, RingSelection, nfold)
 
-from crystals import Crystal
 from iris import DiffractionDataset
 from iris.dataset import SWMR_AVAILABLE
-from skued import nfold, RectSelection, DiskSelection, RingSelection, ArbitrarySelection
-from pathlib import Path
+
 from . import TestRawDataset
-import pytest
 
 np.random.seed(23)
 
 
 def double(im):
     return im * 2
 
@@ -165,14 +165,15 @@
     assert np.allclose(2 * before, after)
 
     with pytest.raises(TypeError):
         dataset.diff_apply(None)
 
 
 @pytest.mark.skipif(not SWMR_AVAILABLE, reason="Parallel execution is not available")
+@flaky(max_runs=5)
 def test_diff_apply_parallel(dataset):
     """Test that the diff_apply method works as expected in parallel mode"""
     before = np.array(dataset.diffraction_group["intensity"])
     dataset.diff_apply(double, processes=2)
     after = np.array(dataset.diffraction_group["intensity"])
     assert np.allclose(2 * before, after)
 
@@ -213,14 +214,15 @@
     dataset.symmetrize(mod=3, center=(63, 65))
     after = np.array(dataset.diffraction_group["intensity"])
 
     assert np.allclose(symmetrized, after)
 
 
 @pytest.mark.skipif(not SWMR_AVAILABLE, reason="Parallel execution is not available")
+@flaky(max_runs=5)
 def test_symmetrization_parallel(dataset):
     """Test correctness of symmetrization operation in parallel mode"""
     before = np.array(dataset.diffraction_group["intensity"])
     symmetrized = np.array(before, copy=True)
     for index, _ in enumerate(dataset.time_points):
         symmetrized[:, :, index] = nfold(
             before[:, :, index], mod=3, center=(63, 65), mask=dataset.valid_mask
```

### Comparing `iris-ued-5.3.4/iris/tests/test_plugins.py` & `iris-ued-5.3.5/iris/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/iris/tests/test_powder.py` & `iris-ued-5.3.5/iris/tests/test_powder.py`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/iris/tests/test_raw.py` & `iris-ued-5.3.5/iris/tests/test_raw.py`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/iris_screen.png` & `iris-ued-5.3.5/iris_screen.png`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/iris_ued.egg-info/PKG-INFO` & `iris-ued-5.3.5/iris_ued.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris-ued
-Version: 5.3.4
+Version: 5.3.5
 Summary: Ultrafast electron diffraction data exploration
 Home-page: http://iris-ued.readthedocs.io
 Author: Laurent P. René de Cotret
 Author-email: laurent.renedecotret@mail.mcgill.ca
 Maintainer: Laurent P. René de Cotret
 Maintainer-email: laurent.renedecotret@mail.mcgill.ca
 License: GPLv3
@@ -21,19 +21,20 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >= 3.7
+Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Iris - Ultrafast Electron Scattering Data Exploration
 
 [![Documentation Build Status](https://readthedocs.org/projects/iris-ued/badge/?version=master)](http://iris-ued.readthedocs.io/) [![PyPI Version](https://img.shields.io/pypi/v/iris-ued.svg)](https://pypi.python.org/pypi/iris-ued) [![Conda-forge Version](https://img.shields.io/conda/vn/conda-forge/iris-ued.svg)](https://anaconda.org/conda-forge/iris-ued) [![DOI badge](https://img.shields.io/badge/DOI-10.1186%2Fs40679--018--0060--y-blue)](https://doi.org/10.1186/s40679-018-0060-y)
 
@@ -69,15 +70,15 @@
     conda install iris-ued
 
 To install the latest development version from
 [Github](https://github.com/LaurentRDC/iris-ued):
 
     python -m pip install git+git://github.com/LaurentRDC/iris-ued.git
 
-Each version is tested against Python 3.7+. If you are using a different
+Each version is tested against Python 3.8+. If you are using a different
 version, tests can be run using the `pytest` package.
 
 ### Windows Installers
 
 For Windows, installers are available on the [Releases](https://github.com/LaurentRDC/iris-ued/releases) page. You will still need to install `iris` via `pip` or `conda` to use the scripting functionality.
 
 ## Usage
```

### Comparing `iris-ued-5.3.4/iris_ued.egg-info/SOURCES.txt` & `iris-ued-5.3.5/iris_ued.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iris-ued-5.3.4/setup.py` & `iris-ued-5.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,25 +63,26 @@
         include_package_data=True,
         project_urls={
             "Documentation": "http://iris-ued.readthedocs.io/en/master/",
             "Source": "https://github.com/LaurentRDC/iris-ued",
             "Tracker": "https://github.com/LaurentRDC/iris-ued/issues",
             "Home": "http://www.physics.mcgill.ca/siwicklab/software.html",
         },
-        python_requires=">= 3.7",
+        python_requires=">= 3.8",
         classifiers=[
             "Development Status :: 5 - Production/Stable",
             "Intended Audience :: Science/Research",
             "Topic :: Scientific/Engineering",
             "Topic :: Scientific/Engineering :: Physics",
             "Topic :: Scientific/Engineering :: Chemistry",
             "Topic :: Scientific/Engineering :: Visualization",
             "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
             "Natural Language :: English",
             "Operating System :: OS Independent",
             "Programming Language :: Python",
-            "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "Programming Language :: Python :: 3.11",
             "Programming Language :: Python :: Implementation :: CPython",
         ],
     )
```

