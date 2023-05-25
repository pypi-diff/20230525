# Comparing `tmp/pymodaq_plugins_horiba-0.1.0.tar.gz` & `tmp/pymodaq_plugins_horiba-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_horiba-0.1.0.tar", last modified: Wed Nov 10 20:38:33 2021, max compression
+gzip compressed data, was "pymodaq_plugins_horiba-1.0.0.tar", last modified: Thu May 25 09:15:25 2023, max compression
```

## Comparing `pymodaq_plugins_horiba-0.1.0.tar` & `pymodaq_plugins_horiba-1.0.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:38:33.060022 pymodaq_plugins_horiba-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-10 20:38:18.000000 pymodaq_plugins_horiba-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-11-10 20:38:18.000000 pymodaq_plugins_horiba-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1899 2021-11-10 20:38:33.060022 pymodaq_plugins_horiba-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      948 2021-11-10 20:38:18.000000 pymodaq_plugins_horiba-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-10 20:38:33.060022 pymodaq_plugins_horiba-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2021-11-10 20:38:18.000000 pymodaq_plugins_horiba-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:38:33.056022 pymodaq_plugins_horiba-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:38:33.060022 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-11-10 20:38:18.000000 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 20:38:18.000000 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:38:33.060022 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      483 2021-11-10 20:38:18.000000 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/daq_move_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:38:33.060022 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        3 2021-11-10 20:38:18.000000 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:38:33.060022 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (121)      487 2021-11-10 20:38:18.000000 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_0D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:38:33.060022 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (121)      487 2021-11-10 20:38:18.000000 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_1D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11577 2021-11-10 20:38:18.000000 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Labspec6TCP.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:38:33.060022 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (121)      488 2021-11-10 20:38:18.000000 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_2D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:38:33.060022 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (121)      487 2021-11-10 20:38:18.000000 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_ND/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:38:33.060022 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/hardware/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 20:38:18.000000 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/hardware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:38:33.060022 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/hardware/horiba/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 20:38:18.000000 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/hardware/horiba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16786 2021-11-10 20:38:18.000000 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/hardware/horiba/labspec6.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:38:33.060022 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1899 2021-11-10 20:38:32.000000 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2021-11-10 20:38:32.000000 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-10 20:38:32.000000 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-11-10 20:38:32.000000 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-11-10 20:38:32.000000 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-11-10 20:38:32.000000 pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:15:25.107378 pymodaq_plugins_horiba-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-25 09:15:13.000000 pymodaq_plugins_horiba-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 09:15:13.000000 pymodaq_plugins_horiba-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-25 09:15:25.107378 pymodaq_plugins_horiba-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-25 09:15:13.000000 pymodaq_plugins_horiba-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:15:25.107378 pymodaq_plugins_horiba-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-25 09:15:13.000000 pymodaq_plugins_horiba-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:15:25.095378 pymodaq_plugins_horiba-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:15:25.099378 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-25 09:15:13.000000 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-25 09:15:13.000000 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:15:25.103378 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-25 09:15:13.000000 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/daq_move_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:15:25.103378 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-25 09:15:13.000000 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:15:25.103378 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-25 09:15:13.000000 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_0D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:15:25.103378 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-25 09:15:13.000000 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_1D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-05-25 09:15:13.000000 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Labspec6TCP.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:15:25.107378 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-25 09:15:13.000000 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_2D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:15:25.107378 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-25 09:15:13.000000 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_ND/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:15:25.107378 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:15:13.000000 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/hardware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:15:25.107378 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/hardware/horiba/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:15:13.000000 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/hardware/horiba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16786 2023-05-25 09:15:13.000000 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/hardware/horiba/labspec6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:15:25.103378 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-25 09:15:25.000000 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-25 09:15:25.000000 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:15:25.000000 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 09:15:25.000000 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-25 09:15:25.000000 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 09:15:25.000000 pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_horiba-0.1.0/LICENSE` & `pymodaq_plugins_horiba-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_horiba-0.1.0/PKG-INFO` & `pymodaq_plugins_horiba-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pymodaq_plugins_horiba
-Version: 0.1.0
+Version: 1.0.0
 Summary: Set of PyMoDAQ plugins for Horiba Instruments (Lapspec6TCP to communicate with labspec softaware using the AFM TCP/IP protocol)
-Home-page: https://github.com/CEMES-CNRS/pymodaq_plugins_horiba
+Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_horiba
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
    :target: https://pypi.org/project/pymodaq_plugins_horiba/
    :alt: Latest Version
 
 .. image:: https://readthedocs.org/projects/pymodaq/badge/?version=latest
    :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
    :alt: Documentation Status
 
-.. image:: https://github.com/CEMES-CNRS/pymodaq_plugins_horiba/workflows/Upload%20Python%20Package/badge.svg
-    :target: https://github.com/CEMES-CNRS/pymodaq_plugins_horiba
+.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_horiba/workflows/Upload%20Python%20Package/badge.svg
+    :target: https://github.com/PyMoDAQ/pymodaq_plugins_horiba
 
 PyMoDAQ plugin for Horiba Instruments (Lapspec6TCP to communicate with labspec
 software using the AFM TCP/IP protocol
 
 
 Authors
 =======
@@ -47,9 +46,7 @@
 Below is the list of instruments included in this plugin
 
 
 Viewer1D
 ++++++++
 
 * **Labspec6TCP**: Control of Labspec6 settings and acquisition using TCP/IP communication
-
-
```

### Comparing `pymodaq_plugins_horiba-0.1.0/README.rst` & `pymodaq_plugins_horiba-1.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
    :target: https://pypi.org/project/pymodaq_plugins_horiba/
    :alt: Latest Version
 
 .. image:: https://readthedocs.org/projects/pymodaq/badge/?version=latest
    :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
    :alt: Documentation Status
 
-.. image:: https://github.com/CEMES-CNRS/pymodaq_plugins_horiba/workflows/Upload%20Python%20Package/badge.svg
-    :target: https://github.com/CEMES-CNRS/pymodaq_plugins_horiba
+.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_horiba/workflows/Upload%20Python%20Package/badge.svg
+    :target: https://github.com/PyMoDAQ/pymodaq_plugins_horiba
 
 PyMoDAQ plugin for Horiba Instruments (Lapspec6TCP to communicate with labspec
 software using the AFM TCP/IP protocol
 
 
 Authors
 =======
```

### Comparing `pymodaq_plugins_horiba-0.1.0/setup.py` & `pymodaq_plugins_horiba-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Labspec6TCP.py` & `pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Labspec6TCP.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,31 +6,19 @@
 
 Issue: The protocol in version 0.6.2 doesn't update the exposure time in Labspec GUI but still take it into account.
 Issue: Binning: issue with the server, it says it doesnt recognise the binning command but set its value nevertheless
 This plugin use a wrapper in hardware/horiba/labspec6.py => Labspec6Client that deals with TCP/IP commands and retrieves
 data
 
 """
-
-
-
-from qtpy.QtCore import QThread
-from qtpy import QtWidgets
-from pymodaq.daq_viewer.utility_classes import DAQ_Viewer_base
-import numpy as np
-from easydict import EasyDict as edict
-from collections import OrderedDict
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo, gauss1D, linspace_step, DataFromPlugins, Axis
-from pymodaq.daq_viewer.utility_classes import comon_parameters
-from pyqtgraph.parametertree import Parameter, ParameterTree
-import pyqtgraph.parametertree.parameterTypes as pTypes
-import pymodaq.daq_utils.parameter.pymodaq_ptypes as pymodaq_ptypes
-from ...hardware.horiba.labspec6 import Labspec6Client
-
-
+from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, main
+from pymodaq.utils.daq_utils import ThreadCommand
+from pymodaq.utils.data import DataFromPlugins, Axis
+from pymodaq.control_modules.viewer_utility_classes import comon_parameters
+from pymodaq_plugins_horiba.hardware.horiba.labspec6 import Labspec6Client
 
 
 class DAQ_1DViewer_Labspec6TCP(DAQ_Viewer_base):
     """
     1D viewer plugin Enabling communication with Labspec6 software controlling horiba spectrometers.
     Labspec must be opened and its AFM server turned on, see Labspec6 configuration
     """
@@ -48,30 +36,29 @@
                 {'title': 'Exp. Time (s)', 'name': 'exposure', 'type': 'float', 'value': 1.0, 'min': 0.001},
                 {'title': 'Accumulation', 'name': 'accumulations', 'type': 'int', 'value': 1, 'min': 1},
                 {'title': 'Binning', 'name': 'binning', 'type': 'int', 'value': 1, 'min': 1},
                 {'title': 'Npts Map', 'name': 'npts_map', 'type': 'int', 'value': 2, 'min': 1, 'visible': False}, #only there to enable fast scan without having to send a list of points at each grab
                 ]
              },
             {'title': 'Instrument setup', 'name': 'inst_setup', 'type': 'group', 'children': [
-                {'title': 'Grating', 'name': 'grating', 'type': 'list', 'values': []},
-                {'title': 'Laser', 'name': 'laser', 'type': 'list', 'values': []},
+                {'title': 'Grating', 'name': 'grating', 'type': 'list', 'limits': []},
+                {'title': 'Laser', 'name': 'laser', 'type': 'list', 'limits': []},
                 {'title': 'Hole', 'name': 'hole', 'type': 'int', 'value': 70, 'min': 1},
                 {'title': 'Slit', 'name': 'slit', 'type': 'int', 'value': 100, 'min': 1},
                 ],
             },
     ]
 
     param_mapping = {'spectro_wl': 'Spectro', 'exposure': 'Exposure', 'accumulation': 'Accumulations',
                      'binning': 'Binning', 'grating': 'Grating', 'laser': 'Laser', 'hole': 'Hole', 'slit': 'Slit'}
 
     hardware_averaging = False
 
-    def __init__(self, parent=None, params_state=None): #init_params is a list of tuple where each tuple contains info on a 1D channel (Ntps,amplitude, width, position and noise)
-        self.controller = None
-        super().__init__(parent, params_state)
+    def ini_attributes(self):
+        self.controller: Labspec6Client = None
         self.x_axis = dict(label='photon wavelength', unit='nm')
         self.sock = None
         self.controller_ready = False
 
     def commit_settings(self, param):
         """
             Setting the mock data
@@ -156,49 +143,36 @@
         """
             Initialisation procedure of the detector updating the status dictionnary.
 
             See Also
             --------
             set_Mock_data, daq_utils.ThreadCommand
         """
-        self.status.update(edict(initialized=False,info="",x_axis=None,y_axis=None,controller=None))
-        try:
+        self.ini_detector_init(old_controller=controller,
+                               new_controller=Labspec6Client())
 
-            if self.settings.child(('controller_status')).value()=="Slave":
-                if controller is None: 
-                    raise Exception('no controller has been defined externally while this detector is a slave one')
-                else:
-                    self.controller = controller
-            else:
-                self.controller = Labspec6Client()
-                ret, data, extra = self.controller.connect(self.settings.child('connection', 'ip_address').value(),
-                                                           self.settings.child('connection', 'port').value())
-                if ret != 'OK':
-                    raise IOError('Wrong return from Server')
-                self.settings.child('connection',  'controllerid').setValue(data)
-
-            self.controller.timeout_mult = self.settings.child('connection', 'timeout').value()
-            self.init_params()
-
-            # initialize viewers with the future type of data
-            self.x_axis = self.controller.get_x_axis()
-
-            self.data_grabed_signal_temp.emit([DataFromPlugins(name='LabSpec6', data=[self.x_axis*0], dim='Data1D',
-                x_axis=Axis(data=self.x_axis, units='nm', label='Wavelength'), labels=['Spectrum']),])
-
-            self.status.initialized = True
-            self.status.controller = self.controller
-            self.status.x_axis = self.x_axis
-            return self.status
-
-        except Exception as e:
-            self.emit_status(ThreadCommand('Update_Status', [getLineInfo() + str(e), 'log']))
-            self.status.info = getLineInfo() + str(e)
-            self.status.initialized = False
-            return self.status
+        if self.settings.child('controller_status').value() == "Master":
+            ret, data, extra = self.controller.connect(self.settings.child('connection', 'ip_address').value(),
+                                                       self.settings.child('connection', 'port').value())
+            if ret != 'OK':
+                raise IOError('Wrong return from Server')
+            self.settings.child('connection',  'controllerid').setValue(data)
+
+        self.controller.timeout_mult = self.settings.child('connection', 'timeout').value()
+        self.init_params()
+
+        # initialize viewers with the future type of data
+        self.x_axis = self.controller.get_x_axis()
+
+        self.data_grabed_signal_temp.emit([DataFromPlugins(name='LabSpec6', data=[self.x_axis*0], dim='Data1D',
+            x_axis=Axis(data=self.x_axis, units='nm', label='Wavelength'), labels=['Spectrum']),])
+
+        info = "Whatever info you want to log"
+        initialized = True
+        return info, initialized
 
     def close(self):
         """
             Not implemented.
         """
         self.controller.close()
 
@@ -263,7 +237,11 @@
 
     def stop(self):
         """
             not implemented.
         """
         
         return ""
+
+
+if __name__ == '__main__':
+    main(__file__, init=True)
```

### Comparing `pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba/hardware/horiba/labspec6.py` & `pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba/hardware/horiba/labspec6.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba.egg-info/PKG-INFO` & `pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pymodaq-plugins-horiba
-Version: 0.1.0
+Version: 1.0.0
 Summary: Set of PyMoDAQ plugins for Horiba Instruments (Lapspec6TCP to communicate with labspec softaware using the AFM TCP/IP protocol)
-Home-page: https://github.com/CEMES-CNRS/pymodaq_plugins_horiba
+Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_horiba
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
    :target: https://pypi.org/project/pymodaq_plugins_horiba/
    :alt: Latest Version
 
 .. image:: https://readthedocs.org/projects/pymodaq/badge/?version=latest
    :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
    :alt: Documentation Status
 
-.. image:: https://github.com/CEMES-CNRS/pymodaq_plugins_horiba/workflows/Upload%20Python%20Package/badge.svg
-    :target: https://github.com/CEMES-CNRS/pymodaq_plugins_horiba
+.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_horiba/workflows/Upload%20Python%20Package/badge.svg
+    :target: https://github.com/PyMoDAQ/pymodaq_plugins_horiba
 
 PyMoDAQ plugin for Horiba Instruments (Lapspec6TCP to communicate with labspec
 software using the AFM TCP/IP protocol
 
 
 Authors
 =======
@@ -47,9 +46,7 @@
 Below is the list of instruments included in this plugin
 
 
 Viewer1D
 ++++++++
 
 * **Labspec6TCP**: Control of Labspec6 settings and acquisition using TCP/IP communication
-
-
```

### Comparing `pymodaq_plugins_horiba-0.1.0/src/pymodaq_plugins_horiba.egg-info/SOURCES.txt` & `pymodaq_plugins_horiba-1.0.0/src/pymodaq_plugins_horiba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

