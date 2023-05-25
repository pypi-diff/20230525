# Comparing `tmp/pymodaq_plugins_physik_instrumente-0.2.0.tar.gz` & `tmp/pymodaq_plugins_physik_instrumente-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_physik_instrumente-0.2.0.tar", last modified: Wed Feb  8 14:38:38 2023, max compression
+gzip compressed data, was "pymodaq_plugins_physik_instrumente-1.0.0.tar", last modified: Thu May 25 09:18:37 2023, max compression
```

## Comparing `pymodaq_plugins_physik_instrumente-0.2.0.tar` & `pymodaq_plugins_physik_instrumente-1.0.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:38:38.664165 pymodaq_plugins_physik_instrumente-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-02-08 14:38:38.664165 pymodaq_plugins_physik_instrumente-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 14:38:38.664165 pymodaq_plugins_physik_instrumente-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:38:38.660165 pymodaq_plugins_physik_instrumente-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:38:38.660165 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:38:38.660165 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI.py
--rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI_MMC.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:38:38.660165 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:38:38.660165 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_0D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:38:38.660165 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_1D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:38:38.660165 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_2D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:38:38.660165 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_ND/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:38:38.660165 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:38:38.660165 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC.H
--rw-r--r--   0 runner    (1001) docker     (123)    68608 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC.dll
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.H
--rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.c
--rw-r--r--   0 runner    (1001) docker     (123)    22270 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.lib
--rw-r--r--   0 runner    (1001) docker     (123)    68608 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC_418.dll
--rw-r--r--   0 runner    (1001) docker     (123)   649494 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MercuryNativeCommands_MS176E101.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   300347 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/Mercury_DLL-LV_MS177E500.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/mmc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 14:38:27.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:38:38.660165 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-02-08 14:38:38.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-02-08 14:38:38.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 14:38:38.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-08 14:38:38.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-08 14:38:38.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-08 14:38:38.000000 pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:18:37.818065 pymodaq_plugins_physik_instrumente-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-25 09:18:37.818065 pymodaq_plugins_physik_instrumente-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:18:37.818065 pymodaq_plugins_physik_instrumente-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:18:37.814065 pymodaq_plugins_physik_instrumente-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:18:37.814065 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:18:37.818065 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI_MMC.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:18:37.818065 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:18:37.818065 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_0D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:18:37.818065 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_1D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:18:37.818065 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_2D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:18:37.818065 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_ND/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:18:37.818065 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:18:37.818065 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC.H
+-rw-r--r--   0 runner    (1001) docker     (123)    68608 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC.dll
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.H
+-rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.c
+-rw-r--r--   0 runner    (1001) docker     (123)    22270 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.lib
+-rw-r--r--   0 runner    (1001) docker     (123)    68608 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC_418.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   649494 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MercuryNativeCommands_MS176E101.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   300347 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/Mercury_DLL-LV_MS177E500.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/mmc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:18:25.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:18:37.814065 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-25 09:18:37.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-25 09:18:37.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:18:37.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-25 09:18:37.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 09:18:37.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 09:18:37.000000 pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_physik_instrumente-0.2.0/LICENSE` & `pymodaq_plugins_physik_instrumente-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-0.2.0/PKG-INFO` & `pymodaq_plugins_physik_instrumente-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq_plugins_physik_instrumente
-Version: 0.2.0
+Version: 1.0.0
 Summary: Set of PyMoDAQ plugins for Actuators from Physik Instumente (All the ones compatible with the GCS2 commands as well as the old 32bits MMC controller...)
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_physik_instrumente
 Author: Sebastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_physik_instrumente-0.2.0/README.rst` & `pymodaq_plugins_physik_instrumente-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-0.2.0/setup.py` & `pymodaq_plugins_physik_instrumente-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI.py` & `pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Tuple
 
 import numpy as np
 from easydict import EasyDict as edict
 from pipython import GCSDevice
 import serial.tools.list_ports as list_ports
 
-from pymodaq.control_modules.move_utility_classes import DAQ_Move_base, main
-from pymodaq.daq_move.utility_classes import comon_parameters_fun
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo
-from pymodaq.daq_utils.parameter.utils import iter_children
+from pymodaq.control_modules.move_utility_classes import DAQ_Move_base, main, comon_parameters_fun
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.utils.parameter.utils import iter_children
 
 
 class DAQ_Move_PI(DAQ_Move_base):
     """
     Plugin using the pipython package wrapper. It is compatible with :
     DLLDEVICES = {
     'PI_GCS2_DLL': ['C-413', 'C-663.11', 'C-863.11', 'C-867', 'C-877', 'C-884', 'C-885', 'C-887',
```

### Comparing `pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI_MMC.py` & `pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI_MMC.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 C-663 Mercury™-Step Motor Controller
 C-170 Redstone PILine® Controller
 
 """
 
 import sys, os
 from qtpy.QtCore import QThread
-from pymodaq.control_modules.move_utility_classes import DAQ_Move_base
-from pymodaq.daq_move.utility_classes import comon_parameters
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.control_modules.move_utility_classes import DAQ_Move_base, comon_parameters_fun, main
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
 from easydict import EasyDict as edict
 
-from ..hardware.PI.mmc_wrapper import MMC_Wrapper
+from pymodaq_plugins_physik_instrumente.hardware.PI.mmc_wrapper import MMC_Wrapper
 
 #is64bit = sys.maxsize > 2**32
 if (sys.maxsize > 2**32):
     raise Exception("It must a python 32 bit version")
 
 ports = MMC_Wrapper.ports
 
+
 class DAQ_Move_PI_MMC(DAQ_Move_base):
     """
         Wrapper object to access the Physik Instrumente fonctionnalities, similar wrapper for all controllers.
 
         =============== =======================
         **Attributes**   **Type**
         *GCS_path*       string
@@ -48,20 +48,15 @@
     stage_names=[]
 
     params= [{'title': 'COM Ports:', 'name': 'com_port', 'type': 'list', 'limits': com_ports},
            {'title': 'Controller_address:', 'name': 'controller_address', 'type': 'list', 'limits': controller_addresses},
            {'title': 'Stages:', 'name': 'stage', 'type': 'list', 'limits': list(MMC_Wrapper.stages.keys())},
            {'title': 'Closed loop?:', 'name': 'closed_loop', 'type': 'bool', 'value': True},
            {'title': 'Controller ID:', 'name': 'controller_id', 'type': 'str', 'value': '', 'readonly': True},
-           {'title': 'MultiAxes:', 'name': 'multiaxes', 'type': 'group','visible':is_multiaxes, 'children':[
-                    {'title': 'is Multiaxes:', 'name': 'ismultiaxes', 'type': 'bool', 'value': is_multiaxes, 'default': False},
-                    {'title': 'Status:', 'name': 'multi_status', 'type': 'list', 'value': 'Master', 'limits': ['Master','Slave']},
-                    {'title': 'Axis:', 'name': 'axis', 'type': 'list',  'limits':stage_names},
-
-                    ]}]+comon_parameters
+           ] + comon_parameters_fun(is_multiaxes, stage_names, epsilon=_epsilon)
 
 
 
 
 
     def __init__(self,parent=None,params_state=None):
 
@@ -235,7 +230,9 @@
             QThread.msleep(100)
             pos = pos_tmp
         self.controller.MMC_sendCommand('DH')  #to define it as home
         QThread.msleep(500)
         self.check_position()
 
 
+if __name__ == '__main__':
+    main(__file__, init=True)
```

### Comparing `pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC.H` & `pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC.H`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC.dll` & `pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC.dll`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.H` & `pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.H`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.c` & `pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.c`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.lib` & `pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.lib`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC_418.dll` & `pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC_418.dll`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MercuryNativeCommands_MS176E101.pdf` & `pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MercuryNativeCommands_MS176E101.pdf`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/Mercury_DLL-LV_MS177E500.pdf` & `pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/Mercury_DLL-LV_MS177E500.pdf`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/mmc_wrapper.py` & `pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/mmc_wrapper.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente.egg-info/PKG-INFO` & `pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq-plugins-physik-instrumente
-Version: 0.2.0
+Version: 1.0.0
 Summary: Set of PyMoDAQ plugins for Actuators from Physik Instumente (All the ones compatible with the GCS2 commands as well as the old 32bits MMC controller...)
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_physik_instrumente
 Author: Sebastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_physik_instrumente-0.2.0/src/pymodaq_plugins_physik_instrumente.egg-info/SOURCES.txt` & `pymodaq_plugins_physik_instrumente-1.0.0/src/pymodaq_plugins_physik_instrumente.egg-info/SOURCES.txt`

 * *Files identical despite different names*

