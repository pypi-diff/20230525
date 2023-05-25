# Comparing `tmp/solo_epd_loader-0.2.1.tar.gz` & `tmp/solo_epd_loader-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solo_epd_loader-0.2.1.tar", last modified: Thu Apr 20 13:34:16 2023, max compression
+gzip compressed data, was "solo_epd_loader-0.2.2.tar", last modified: Thu May 25 07:45:48 2023, max compression
```

## Comparing `solo_epd_loader-0.2.1.tar` & `solo_epd_loader-0.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 13:34:16.025219 solo_epd_loader-0.2.1/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.1/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.1/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16777 2023-04-20 13:34:16.025219 solo_epd_loader-0.2.1/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15829 2023-04-20 13:32:52.000000 solo_epd_loader-0.2.1/README.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.2.1/code_of_conduct.md
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 13:34:16.021219 solo_epd_loader-0.2.1/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.1/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.1/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.2.1/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.1/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 13:34:16.021219 solo_epd_loader-0.2.1/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.2.1/examples/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.2.1/examples/ws2021_fig_2d.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.2.1/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.2.1/gh2021_fig_2a.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 13:34:16.021219 solo_epd_loader-0.2.1/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.1/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.1/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.1/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2302 2023-04-20 13:34:16.025219 solo_epd_loader-0.2.1/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.1/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 13:34:16.025219 solo_epd_loader-0.2.1/solo_epd_loader/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    37798 2022-11-16 14:15:40.000000 solo_epd_loader-0.2.1/solo_epd_loader/__init__ (STEP UPDATE).py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    44704 2023-04-20 12:40:04.000000 solo_epd_loader-0.2.1/solo_epd_loader/__init__.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 13:34:16.025219 solo_epd_loader-0.2.1/solo_epd_loader/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.1/solo_epd_loader/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-04-20 13:34:15.000000 solo_epd_loader-0.2.1/solo_epd_loader/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 13:34:16.025219 solo_epd_loader-0.2.1/solo_epd_loader.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16777 2023-04-20 13:34:15.000000 solo_epd_loader-0.2.1/solo_epd_loader.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      653 2023-04-20 13:34:16.000000 solo_epd_loader-0.2.1/solo_epd_loader.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-04-20 13:34:15.000000 solo_epd_loader-0.2.1/solo_epd_loader.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.2.1/solo_epd_loader.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      188 2023-04-20 13:34:15.000000 solo_epd_loader-0.2.1/solo_epd_loader.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-04-20 13:34:15.000000 solo_epd_loader-0.2.1/solo_epd_loader.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.2.1/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-25 07:45:48.558088 solo_epd_loader-0.2.2/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.2/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.2/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    17529 2023-05-25 07:45:48.558088 solo_epd_loader-0.2.2/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16581 2023-05-23 14:42:04.000000 solo_epd_loader-0.2.2/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.2.2/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-25 07:45:48.554088 solo_epd_loader-0.2.2/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.2/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.2/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.2.2/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.2/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-25 07:45:48.554088 solo_epd_loader-0.2.2/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.2.2/examples/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.2.2/examples/ws2021_fig_2d.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.2.2/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.2.2/gh2021_fig_2a.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-25 07:45:48.554088 solo_epd_loader-0.2.2/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.2/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.2/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.2/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2302 2023-05-25 07:45:48.562088 solo_epd_loader-0.2.2/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.2/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-25 07:45:48.558088 solo_epd_loader-0.2.2/solo_epd_loader/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    37798 2022-11-16 14:15:40.000000 solo_epd_loader-0.2.2/solo_epd_loader/__init__ (STEP UPDATE).py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    44832 2023-05-25 07:34:00.000000 solo_epd_loader-0.2.2/solo_epd_loader/__init__.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-25 07:45:48.558088 solo_epd_loader-0.2.2/solo_epd_loader/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.2/solo_epd_loader/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-05-25 07:45:48.000000 solo_epd_loader-0.2.2/solo_epd_loader/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-25 07:45:48.558088 solo_epd_loader-0.2.2/solo_epd_loader.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    17529 2023-05-25 07:45:48.000000 solo_epd_loader-0.2.2/solo_epd_loader.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      653 2023-05-25 07:45:48.000000 solo_epd_loader-0.2.2/solo_epd_loader.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-05-25 07:45:48.000000 solo_epd_loader-0.2.2/solo_epd_loader.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.2.2/solo_epd_loader.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      188 2023-05-25 07:45:48.000000 solo_epd_loader-0.2.2/solo_epd_loader.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-05-25 07:45:48.000000 solo_epd_loader-0.2.2/solo_epd_loader.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.2.2/tox.ini
```

### Comparing `solo_epd_loader-0.2.1/LICENSE.rst` & `solo_epd_loader-0.2.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.1/PKG-INFO` & `solo_epd_loader-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo_epd_loader
-Version: 0.2.1
+Version: 0.2.2
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -79,29 +79,31 @@
 returns Pandas dataframe(s) of the EPD measurements and a dictionary
 containing information on the energy channels.
 
 .. code:: python
 
    from solo_epd_loader import epd_load
 
-   df_1, df_2, energies = \
-       epd_load(sensor, level, startdate, enddate=None, viewing=None, path=None, autodownload=False)
+   df_1, df_2, energies = epd_load(sensor, startdate, enddate=None, level='l2', viewing=None, path=None, 
+                                   autodownload=False, only_averages=False, contamination_threshold=2)
 
 Input
 ~~~~~
 
 -  ``sensor``: ``'ept'``, ``'het'``, or ``'step'`` (string)
--  ``level``: ``'ll'`` or ``'l2'`` (string)
 -  ``startdate``, ``enddate``: Datetime object (e.g., ``dt.date(2021,12,31)`` or ``dt.datetime(2021,4,15)``) or integer of the form yyyymmdd with empty positions filled with zeros, e.g. ``20210415`` (if no ``enddate`` is provided, ``enddate = startdate`` will be used)
+-  ``level``: ``'l2'`` or ``'ll'`` (string); defines level of data product: level 2 (``'l2'``) or low-latency (``'ll'``). By default ``'l2'``.
 -  ``viewing``: ``'sun'``, ``'asun'``, ``'north'``, ``'south'`` (string) or ``None``; not
    needed for ``sensor = 'step'``
 -  ``path``: directory in which Solar Orbiter data is/should be
    organized; e.g. ``'/home/userxyz/solo/data/'`` (string). See `Data folder structure`_ for more details.
--  ``autodownload``: if ``True`` will try to download missing data files
+-  ``autodownload``: if ``True``, will try to download missing data files
    from SOAR (bolean)
+- ``only_averages``: If ``True``, will for STEP only return the averaged fluxes, and not the data of each of the 15 Pixels. This will reduce the memory consumption. By default ``False``.
+- ``contamination_threshold``: If integer, mask electron data that probably is contaminated (i.e., set it to ``nan``) using an integer contamination threshold following the equation ``Integral_Flux - Magnet_Flux > contamination_threshold * Integral_Uncertainty``. If ``False``, don't alter the data at all. Only implemented for new STEP data (after Oct 2021) so far. By default ``2``.
 
 Return
 ~~~~~~
 
 -  For ``sensor`` = ``'ept'`` or ``'het'``:
 
    1. Pandas dataframe with proton fluxes and errors (for EPT also alpha
```

### Comparing `solo_epd_loader-0.2.1/README.rst` & `solo_epd_loader-0.2.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -54,29 +54,31 @@
 returns Pandas dataframe(s) of the EPD measurements and a dictionary
 containing information on the energy channels.
 
 .. code:: python
 
    from solo_epd_loader import epd_load
 
-   df_1, df_2, energies = \
-       epd_load(sensor, level, startdate, enddate=None, viewing=None, path=None, autodownload=False)
+   df_1, df_2, energies = epd_load(sensor, startdate, enddate=None, level='l2', viewing=None, path=None, 
+                                   autodownload=False, only_averages=False, contamination_threshold=2)
 
 Input
 ~~~~~
 
 -  ``sensor``: ``'ept'``, ``'het'``, or ``'step'`` (string)
--  ``level``: ``'ll'`` or ``'l2'`` (string)
 -  ``startdate``, ``enddate``: Datetime object (e.g., ``dt.date(2021,12,31)`` or ``dt.datetime(2021,4,15)``) or integer of the form yyyymmdd with empty positions filled with zeros, e.g. ``20210415`` (if no ``enddate`` is provided, ``enddate = startdate`` will be used)
+-  ``level``: ``'l2'`` or ``'ll'`` (string); defines level of data product: level 2 (``'l2'``) or low-latency (``'ll'``). By default ``'l2'``.
 -  ``viewing``: ``'sun'``, ``'asun'``, ``'north'``, ``'south'`` (string) or ``None``; not
    needed for ``sensor = 'step'``
 -  ``path``: directory in which Solar Orbiter data is/should be
    organized; e.g. ``'/home/userxyz/solo/data/'`` (string). See `Data folder structure`_ for more details.
--  ``autodownload``: if ``True`` will try to download missing data files
+-  ``autodownload``: if ``True``, will try to download missing data files
    from SOAR (bolean)
+- ``only_averages``: If ``True``, will for STEP only return the averaged fluxes, and not the data of each of the 15 Pixels. This will reduce the memory consumption. By default ``False``.
+- ``contamination_threshold``: If integer, mask electron data that probably is contaminated (i.e., set it to ``nan``) using an integer contamination threshold following the equation ``Integral_Flux - Magnet_Flux > contamination_threshold * Integral_Uncertainty``. If ``False``, don't alter the data at all. Only implemented for new STEP data (after Oct 2021) so far. By default ``2``.
 
 Return
 ~~~~~~
 
 -  For ``sensor`` = ``'ept'`` or ``'het'``:
 
    1. Pandas dataframe with proton fluxes and errors (for EPT also alpha
```

### Comparing `solo_epd_loader-0.2.1/code_of_conduct.md` & `solo_epd_loader-0.2.2/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.1/docs/Makefile` & `solo_epd_loader-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.1/docs/conf.py` & `solo_epd_loader-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.1/docs/make.bat` & `solo_epd_loader-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.1/examples/gh2021_fig_2.png` & `solo_epd_loader-0.2.2/examples/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.1/examples/ws2021_fig_2d.png` & `solo_epd_loader-0.2.2/examples/ws2021_fig_2d.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.1/gh2021_fig_2.png` & `solo_epd_loader-0.2.2/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.1/gh2021_fig_2a.png` & `solo_epd_loader-0.2.2/gh2021_fig_2a.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.1/licenses/LICENSE.rst` & `solo_epd_loader-0.2.2/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.1/licenses/TEMPLATE_LICENSE.rst` & `solo_epd_loader-0.2.2/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.1/setup.cfg` & `solo_epd_loader-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.1/setup.py` & `solo_epd_loader-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.1/solo_epd_loader/__init__ (STEP UPDATE).py` & `solo_epd_loader-0.2.2/solo_epd_loader/__init__ (STEP UPDATE).py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.1/solo_epd_loader/__init__.py` & `solo_epd_loader-0.2.2/solo_epd_loader/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,23 +8,27 @@
     pass  # package is not installed
 
 import datetime as dt
 import glob
 import itertools
 import os
 import re
+import sunpy
 import urllib.request
 import warnings
 from pathlib import Path
 
 import cdflib
 import numpy as np
 import pandas as pd
 from astropy.io.votable import parse_single_table
-from sunpy.io.cdf import read_cdf
+if int(sunpy.__version__[0]) == 4:
+    from sunpy.io.cdf import read_cdf
+elif int(sunpy.__version__[0]) >= 5:
+    from sunpy.io._cdf import read_cdf
 from sunpy.timeseries import TimeSeries
 
 # omit Pandas' PerformanceWarning
 warnings.simplefilter(action='ignore', category=pd.errors.PerformanceWarning)
 
 
 """
```

### Comparing `solo_epd_loader-0.2.1/solo_epd_loader.egg-info/PKG-INFO` & `solo_epd_loader-0.2.2/solo_epd_loader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo-epd-loader
-Version: 0.2.1
+Version: 0.2.2
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -79,29 +79,31 @@
 returns Pandas dataframe(s) of the EPD measurements and a dictionary
 containing information on the energy channels.
 
 .. code:: python
 
    from solo_epd_loader import epd_load
 
-   df_1, df_2, energies = \
-       epd_load(sensor, level, startdate, enddate=None, viewing=None, path=None, autodownload=False)
+   df_1, df_2, energies = epd_load(sensor, startdate, enddate=None, level='l2', viewing=None, path=None, 
+                                   autodownload=False, only_averages=False, contamination_threshold=2)
 
 Input
 ~~~~~
 
 -  ``sensor``: ``'ept'``, ``'het'``, or ``'step'`` (string)
--  ``level``: ``'ll'`` or ``'l2'`` (string)
 -  ``startdate``, ``enddate``: Datetime object (e.g., ``dt.date(2021,12,31)`` or ``dt.datetime(2021,4,15)``) or integer of the form yyyymmdd with empty positions filled with zeros, e.g. ``20210415`` (if no ``enddate`` is provided, ``enddate = startdate`` will be used)
+-  ``level``: ``'l2'`` or ``'ll'`` (string); defines level of data product: level 2 (``'l2'``) or low-latency (``'ll'``). By default ``'l2'``.
 -  ``viewing``: ``'sun'``, ``'asun'``, ``'north'``, ``'south'`` (string) or ``None``; not
    needed for ``sensor = 'step'``
 -  ``path``: directory in which Solar Orbiter data is/should be
    organized; e.g. ``'/home/userxyz/solo/data/'`` (string). See `Data folder structure`_ for more details.
--  ``autodownload``: if ``True`` will try to download missing data files
+-  ``autodownload``: if ``True``, will try to download missing data files
    from SOAR (bolean)
+- ``only_averages``: If ``True``, will for STEP only return the averaged fluxes, and not the data of each of the 15 Pixels. This will reduce the memory consumption. By default ``False``.
+- ``contamination_threshold``: If integer, mask electron data that probably is contaminated (i.e., set it to ``nan``) using an integer contamination threshold following the equation ``Integral_Flux - Magnet_Flux > contamination_threshold * Integral_Uncertainty``. If ``False``, don't alter the data at all. Only implemented for new STEP data (after Oct 2021) so far. By default ``2``.
 
 Return
 ~~~~~~
 
 -  For ``sensor`` = ``'ept'`` or ``'het'``:
 
    1. Pandas dataframe with proton fluxes and errors (for EPT also alpha
```

### Comparing `solo_epd_loader-0.2.1/solo_epd_loader.egg-info/SOURCES.txt` & `solo_epd_loader-0.2.2/solo_epd_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.1/tox.ini` & `solo_epd_loader-0.2.2/tox.ini`

 * *Files identical despite different names*

