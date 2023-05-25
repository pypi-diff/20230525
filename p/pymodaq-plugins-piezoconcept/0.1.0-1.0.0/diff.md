# Comparing `tmp/pymodaq_plugins_piezoconcept-0.1.0.tar.gz` & `tmp/pymodaq_plugins_piezoconcept-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_piezoconcept-0.1.0.tar", last modified: Wed Nov 10 20:54:24 2021, max compression
+gzip compressed data, was "pymodaq_plugins_piezoconcept-1.0.0.tar", last modified: Thu May 25 09:14:19 2023, max compression
```

## Comparing `pymodaq_plugins_piezoconcept-0.1.0.tar` & `pymodaq_plugins_piezoconcept-1.0.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:54:24.428687 pymodaq_plugins_piezoconcept-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-10 20:54:14.000000 pymodaq_plugins_piezoconcept-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-11-10 20:54:14.000000 pymodaq_plugins_piezoconcept-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2155 2021-11-10 20:54:24.428687 pymodaq_plugins_piezoconcept-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2021-11-10 20:54:14.000000 pymodaq_plugins_piezoconcept-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-10 20:54:24.428687 pymodaq_plugins_piezoconcept-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2021-11-10 20:54:14.000000 pymodaq_plugins_piezoconcept-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:54:24.420687 pymodaq_plugins_piezoconcept-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:54:24.424687 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-11-10 20:54:14.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 20:54:14.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:54:24.428687 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      483 2021-11-10 20:54:14.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/daq_move_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9260 2021-11-10 20:54:14.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/daq_move_plugins/daq_move_PiezoConcept.py
--rw-r--r--   0 runner    (1001) docker     (121)     9294 2021-11-10 20:54:14.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/daq_move_plugins/daq_move_PiezoConceptPI.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:54:24.428687 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        3 2021-11-10 20:54:14.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:54:24.428687 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (121)      487 2021-11-10 20:54:14.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/plugins_0D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:54:24.428687 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (121)      487 2021-11-10 20:54:14.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/plugins_1D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:54:24.428687 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (121)      488 2021-11-10 20:54:14.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/plugins_2D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:54:24.428687 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (121)      487 2021-11-10 20:54:14.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/plugins_ND/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:54:24.428687 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/hardware/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 20:54:14.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/hardware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:54:24.428687 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/hardware/piezoconcept/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 20:54:14.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/hardware/piezoconcept/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      800 2021-11-10 20:54:14.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/hardware/piezoconcept/piezo_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    11087 2021-11-10 20:54:14.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/hardware/piezoconcept/piezoconcept.py
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2021-11-10 20:54:14.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/hardware/piezoconcept/run_arbitrary.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:54:24.428687 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2155 2021-11-10 20:54:24.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2021-11-10 20:54:24.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-10 20:54:24.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2021-11-10 20:54:24.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-11-10 20:54:24.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-11-10 20:54:24.000000 pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:14:19.673179 pymodaq_plugins_piezoconcept-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-25 09:14:04.000000 pymodaq_plugins_piezoconcept-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 09:14:04.000000 pymodaq_plugins_piezoconcept-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-25 09:14:19.673179 pymodaq_plugins_piezoconcept-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-25 09:14:04.000000 pymodaq_plugins_piezoconcept-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:14:19.673179 pymodaq_plugins_piezoconcept-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-25 09:14:04.000000 pymodaq_plugins_piezoconcept-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:14:19.673179 pymodaq_plugins_piezoconcept-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:14:19.673179 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-25 09:14:04.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-25 09:14:04.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:14:19.673179 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-25 09:14:04.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/daq_move_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-05-25 09:14:04.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/daq_move_plugins/daq_move_PiezoConcept.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-25 09:14:04.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/daq_move_plugins/daq_move_PiezoConceptPI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:14:19.673179 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-25 09:14:04.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:14:19.673179 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-25 09:14:04.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/plugins_0D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:14:19.673179 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-25 09:14:04.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/plugins_1D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:14:19.673179 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-25 09:14:04.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/plugins_2D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:14:19.673179 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-25 09:14:04.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/daq_viewer_plugins/plugins_ND/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:14:19.673179 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:14:04.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/hardware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:14:19.673179 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/hardware/piezoconcept/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:14:04.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/hardware/piezoconcept/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-25 09:14:04.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/hardware/piezoconcept/piezo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-05-25 09:14:04.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/hardware/piezoconcept/piezoconcept.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-25 09:14:04.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/hardware/piezoconcept/run_arbitrary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:14:19.673179 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-25 09:14:19.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-25 09:14:19.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:14:19.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 09:14:19.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 09:14:19.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 09:14:19.000000 pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_piezoconcept-0.1.0/LICENSE` & `pymodaq_plugins_piezoconcept-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_piezoconcept-0.1.0/PKG-INFO` & `pymodaq_plugins_piezoconcept-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pymodaq_plugins_piezoconcept
-Version: 0.1.0
+Version: 1.0.0
 Summary: Set of PyMoDAQ plugins for Actuators from Piezoconcept (Tested on the Bio200 XY stage. Include a version of the controller firmware emulating functions from PhysikInstrumente)
-Home-page: https://github.com/CEMES-CNRS/pymodaq_plugins_piezoconcept
+Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_piezoconcept
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: MIT License
@@ -26,16 +25,16 @@
    :target: https://pypi.org/project/pymodaq_plugins_piezoconcept/
    :alt: Latest Version
 
 .. image:: https://readthedocs.org/projects/pymodaq/badge/?version=latest
    :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
    :alt: Documentation Status
 
-.. image:: https://github.com/CEMES-CNRS/pymodaq_plugins_piezoconcept/workflows/Upload%20Python%20Package/badge.svg
-    :target: https://github.com/CEMES-CNRS/pymodaq_plugins_piezoconcept
+.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_piezoconcept/workflows/Upload%20Python%20Package/badge.svg
+    :target: https://github.com/PyMoDAQ/pymodaq_plugins_piezoconcept
 
 PyMoDAQ plugin for actuators from Piezoconcept (Tested on the Bio2.100 XY stage). Include a version of the
 controller firmware emulating functions from PhysikInstrumente
 
 
 Authors
 =======
@@ -47,9 +46,7 @@
 Below is the list of instruments included in this plugin
 
 Actuators
 +++++++++
 
 * **PiezoConcept** : piezoconcept stages (tested on BIO2.100) using the usual serial commands
 * **PiezoConceptPI**: Special firmware to emulate functions form the GCS2 library from Physik Instrumente
-
-
```

### Comparing `pymodaq_plugins_piezoconcept-0.1.0/README.rst` & `pymodaq_plugins_piezoconcept-1.0.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,16 @@
    :target: https://pypi.org/project/pymodaq_plugins_piezoconcept/
    :alt: Latest Version
 
 .. image:: https://readthedocs.org/projects/pymodaq/badge/?version=latest
    :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
    :alt: Documentation Status
 
-.. image:: https://github.com/CEMES-CNRS/pymodaq_plugins_piezoconcept/workflows/Upload%20Python%20Package/badge.svg
-    :target: https://github.com/CEMES-CNRS/pymodaq_plugins_piezoconcept
+.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_piezoconcept/workflows/Upload%20Python%20Package/badge.svg
+    :target: https://github.com/PyMoDAQ/pymodaq_plugins_piezoconcept
 
 PyMoDAQ plugin for actuators from Piezoconcept (Tested on the Bio2.100 XY stage). Include a version of the
 controller firmware emulating functions from PhysikInstrumente
 
 
 Authors
 =======
```

### Comparing `pymodaq_plugins_piezoconcept-0.1.0/setup.py` & `pymodaq_plugins_piezoconcept-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/daq_move_plugins/daq_move_PiezoConcept.py` & `pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/daq_move_plugins/daq_move_PiezoConcept.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from qtpy.QtCore import QThread
-from pymodaq.daq_move.utility_classes import DAQ_Move_base
-from pymodaq.daq_move.utility_classes import comon_parameters
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.control_modules.move_utility_classes import DAQ_Move_base, comon_parameters_fun, main
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
 from easydict import EasyDict as edict
-from ..hardware.piezoconcept.piezoconcept import PiezoConcept, Position, Time
+from pymodaq_plugins_piezoconcept.hardware.piezoconcept.piezoconcept import PiezoConcept, Position, Time
+
 
 class DAQ_Move_PiezoConcept(DAQ_Move_base):
     """
     Plugin to drive piezoconcpet XY (Z) stages. There is a string nonlinear offset between the set position and the read
     position. It seems to bnot be problem in the sens where a given displacement is maintained. But because the read
     position is not "accurate", I've decided to ignore it and just trust the set position. So the return will be always
     strictly equal to the set position. However, if there is more that 10% difference raise a warning
@@ -17,37 +17,29 @@
 
     #find available COM ports
     import serial.tools.list_ports
     ports = [str(port)[0:4] for port in list(serial.tools.list_ports.comports())]
     port = 'COM6' if 'COM6' in ports else ports[0] if len(ports) > 0 else ''
     #if ports==[]:
     #    ports.append('')
-
+    _epsilon = 1
 
     is_multiaxes = True
     stage_names = ['X', 'Y', 'Z']
     min_bound = -95  #*µm
     max_bound = 95  #µm
     offset = 100  #µm
 
     params= [{'title': 'Time interval (ms):', 'name': 'time_interval', 'type': 'int', 'value': 200},
              {'title': 'Controller Info:', 'name': 'controller_id', 'type': 'text', 'value': '', 'readonly': True},
-             {'title': 'COM Port:', 'name': 'com_port', 'type': 'list', 'values': ports, 'value': port},
-              {'title': 'MultiAxes:', 'name': 'multiaxes', 'type': 'group','visible':is_multiaxes, 'children':[
-                        {'title': 'is Multiaxes:', 'name': 'ismultiaxes', 'type': 'bool', 'value': is_multiaxes, 'default': False},
-                        {'title': 'Status:', 'name': 'multi_status', 'type': 'list', 'value': 'Master', 'values': ['Master', 'Slave']},
-                        {'title': 'Axis:', 'name': 'axis', 'type': 'list',  'values':stage_names},
-                        
-                        ]}]+comon_parameters
-
-    def __init__(self,parent=None,params_state=None):
-        super().__init__(parent, params_state)
+             {'title': 'COM Port:', 'name': 'com_port', 'type': 'list', 'limits': ports, 'value': port},
+             ] + comon_parameters_fun(is_multiaxes, stage_names, epsilon=_epsilon)
 
-        self.controller=None
-        self.settings.child(('epsilon')).setValue(1)
+    def ini_attributes(self):
+        self.controller: PiezoConcept = None
 
     def ini_stage(self, controller=None):
         """
             Initialize the controller and stages (axes) with given parameters.
 
             =============== =========================================== ===========================================================================================
             **Parameters**   **Type**                                     **Description**
@@ -65,100 +57,59 @@
                   * *initialized*: boolean indicating if initialization has been done corretly
 
             See Also
             --------
             daq_utils.ThreadCommand
         """
 
-        # initialize the stage and its controller status
-        # controller is an object that may be passed to other instances of DAQ_Move_Mock in case
-        # of one controller controlling multiaxes
-        try:
-            self.status.update(edict(info="",controller=None,initialized=False))
-
-
-            #check whether this stage is controlled by a multiaxe controller (to be defined for each plugin)
-
-            # if mutliaxes then init the controller here if Master state otherwise use external controller
-            if self.settings.child('multiaxes', 'ismultiaxes').value() and self.settings.child('multiaxes','multi_status').value()=="Slave":
-                if controller is None: 
-                    raise Exception('no controller has been defined externally while this stage is a slave one')
-                else:
-                    self.controller = controller
-            else: #Master stage
-                try:
-                    self.close()
-                except:
-                    pass
-                self.controller = PiezoConcept()
-                self.controller.init_communication(self.settings.child(('com_port')).value())
-
-            controller_id = self.controller.get_controller_infos()
-            self.settings.child(('controller_id')).setValue(controller_id)
-
-            self.settings.child('bounds', 'is_bounds').setValue(True)
-            self.settings.child('bounds', 'min_bound').setValue(self.min_bound)
-            self.settings.child('bounds', 'max_bound').setValue(self.max_bound)
-            self.settings.child('scaling', 'use_scaling').setValue(True)
-            self.settings.child('scaling', 'offset').setValue(self.offset)
-
-            self.move_Abs(0)
-
-
-            self.settings.child(('epsilon')).setValue(2)
-            self.status.info = controller_id
-            self.status.controller = self.controller
-            self.status.initialized = True
-            return self.status
-
-        except Exception as e:
-            self.emit_status(ThreadCommand('Update_Status', [getLineInfo()+ str(e), 'log']))
-            self.status.info = getLineInfo()+ str(e)
-            self.status.initialized = False
-            return self.status
+        self.ini_stage_init(old_controller=controller,
+                            new_controller=PiezoConcept())
+        if self.settings['multiaxes', 'multi_status'] == "Master":
+            self.controller.init_communication(self.settings['com_port'])
+
+        controller_id = self.controller.get_controller_infos()
+        self.settings.child('controller_id').setValue(controller_id)
+
+        self.settings.child('bounds', 'is_bounds').setValue(True)
+        self.settings.child('bounds', 'min_bound').setValue(self.min_bound)
+        self.settings.child('bounds', 'max_bound').setValue(self.max_bound)
+        self.settings.child('scaling', 'use_scaling').setValue(True)
+        self.settings.child('scaling', 'offset').setValue(self.offset)
+        self.move_abs(0)
+
+        info = controller_id
+        initialized = True
+        return info, initialized
 
     def close(self):
         """
             close the current instance of Piezo instrument.
         """
         try:
-            self.move_Abs(0)
+            self.move_abs(0)
             QThread.msleep(1000)
         except:
             pass
 
-
         self.controller.close_communication()
         self.controller = None
 
 
-    def check_position(self):
+    def get_actuator_value(self):
         """
-            Check the current position from the hardware.
-
-            Returns
-            -------
-            float
-                The position of the hardware.
-
-            See Also
-            --------
-            DAQ_Move_base.get_position_with_scaling, daq_utils.ThreadCommand
         """
         position = self.controller.get_position(self.settings.child('multiaxes', 'axis').value())  #in mm
         pos = position.pos/1000  # in um
         pos = self.get_position_with_scaling(pos)
         self.current_position = self.target_position  #should be pos but not precise enough conpared to set position
         self.emit_status(ThreadCommand('check_position', [self.target_position]))
         #print(pos)
         return self.target_position
 
-
-
-    def move_Abs(self,position):
+    def move_abs(self, position):
         """
 
         Parameters
         ----------
         position: (float) target position of the given axis in um (or scaled units)
 
         Returns
@@ -170,18 +121,16 @@
 
         #get positions in controller units
         position = self.set_position_with_scaling(position)
         pos = Position(self.settings.child('multiaxes', 'axis').value(), int(position*1000), unit='n')
         out = self.controller.move_axis('ABS', pos)
         #self.move_is_done = True
         QThread.msleep(50) #to make sure the closed loop converged
-        self.poll_moving()
-
 
-    def move_Rel(self,position):
+    def move_rel(self,position):
         """
             Make the hardware relative move of the Piezo instrument from the given position after thread command signal was received in DAQ_Move_main.
 
             =============== ========= =======================
             **Parameters**  **Type**   **Description**
 
             *position*       float     The absolute position
@@ -196,28 +145,32 @@
         self.target_position = position+self.current_position
 
         position = self.set_position_relative_with_scaling(position)
 
         pos = Position(self.settings.child('multiaxes', 'axis').value(), position*1000, unit='n')  # always use microns for simplicity
         out = self.controller.move_axis('REL', pos)
         QThread.msleep(50)  # to make sure the closed loop converged
-        self.poll_moving()
 
-    def move_Home(self):
+
+    def move_home(self):
         """
             Move to the absolute vlue 100 corresponding the default point of the Piezo instrument.
 
             See Also
             --------
-            DAQ_Move_base.move_Abs
+            DAQ_Move_base.move_abs
         """
-        self.move_Abs(100) #put the axis on the middle position so 100µm
+        self.move_abs(100) #put the axis on the middle position so 100µm
 
     def stop_motion(self):
-      """
+        """
         Call the specific move_done function (depending on the hardware).
 
         See Also
         --------
         move_done
-      """
-      self.move_done()
+        """
+        self.move_done()
+
+
+if __name__ == '__main__':
+    main(__file__, init=False)
```

### Comparing `pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/hardware/piezoconcept/piezo_test.py` & `pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/hardware/piezoconcept/piezo_test.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/hardware/piezoconcept/piezoconcept.py` & `pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/hardware/piezoconcept/piezoconcept.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept/hardware/piezoconcept/run_arbitrary.py` & `pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept/hardware/piezoconcept/run_arbitrary.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept.egg-info/PKG-INFO` & `pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pymodaq-plugins-piezoconcept
-Version: 0.1.0
+Version: 1.0.0
 Summary: Set of PyMoDAQ plugins for Actuators from Piezoconcept (Tested on the Bio200 XY stage. Include a version of the controller firmware emulating functions from PhysikInstrumente)
-Home-page: https://github.com/CEMES-CNRS/pymodaq_plugins_piezoconcept
+Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_piezoconcept
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: MIT License
@@ -26,16 +25,16 @@
    :target: https://pypi.org/project/pymodaq_plugins_piezoconcept/
    :alt: Latest Version
 
 .. image:: https://readthedocs.org/projects/pymodaq/badge/?version=latest
    :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
    :alt: Documentation Status
 
-.. image:: https://github.com/CEMES-CNRS/pymodaq_plugins_piezoconcept/workflows/Upload%20Python%20Package/badge.svg
-    :target: https://github.com/CEMES-CNRS/pymodaq_plugins_piezoconcept
+.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_piezoconcept/workflows/Upload%20Python%20Package/badge.svg
+    :target: https://github.com/PyMoDAQ/pymodaq_plugins_piezoconcept
 
 PyMoDAQ plugin for actuators from Piezoconcept (Tested on the Bio2.100 XY stage). Include a version of the
 controller firmware emulating functions from PhysikInstrumente
 
 
 Authors
 =======
@@ -47,9 +46,7 @@
 Below is the list of instruments included in this plugin
 
 Actuators
 +++++++++
 
 * **PiezoConcept** : piezoconcept stages (tested on BIO2.100) using the usual serial commands
 * **PiezoConceptPI**: Special firmware to emulate functions form the GCS2 library from Physik Instrumente
-
-
```

### Comparing `pymodaq_plugins_piezoconcept-0.1.0/src/pymodaq_plugins_piezoconcept.egg-info/SOURCES.txt` & `pymodaq_plugins_piezoconcept-1.0.0/src/pymodaq_plugins_piezoconcept.egg-info/SOURCES.txt`

 * *Files identical despite different names*

