# Comparing `tmp/rgbloom-1.4.tar.gz` & `tmp/rgbloom-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgbloom-1.4.tar", last modified: Mon May 22 11:44:14 2023, max compression
+gzip compressed data, was "/Users/cardiel/s/rgbloom/dist/.tmp-33py9cu4/rgbloom-1.5.tar", last modified: Wed May 24 13:48:45 2023, max compression
```

## Comparing `rgbloom-1.4.tar` & `rgbloom-1.5.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-22 11:44:14.626926 rgbloom-1.4/
--rw-r--r--   0 cardiel    (501) staff       (20)    35149 2022-11-06 08:36:25.000000 rgbloom-1.4/LICENSE
--rw-r--r--   0 cardiel    (501) staff       (20)    12806 2023-05-22 11:44:14.626987 rgbloom-1.4/PKG-INFO
--rw-r--r--   0 cardiel    (501) staff       (20)    12016 2023-05-22 11:40:39.000000 rgbloom-1.4/README.md
--rw-r--r--   0 cardiel    (501) staff       (20)      100 2022-11-06 08:38:35.000000 rgbloom-1.4/pyproject.toml
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-22 11:44:14.624347 rgbloom-1.4/rgbloom/
--rw-r--r--   0 cardiel    (501) staff       (20)       51 2022-11-06 08:39:16.000000 rgbloom-1.4/rgbloom/__init__.py
--rw-r--r--   0 cardiel    (501) staff       (20)     6508 2023-05-22 11:40:39.000000 rgbloom-1.4/rgbloom/__main__.py
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-22 11:44:14.626364 rgbloom-1.4/rgbloom/core/
--rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-06 08:39:16.000000 rgbloom-1.4/rgbloom/core/__init__.py
--rw-r--r--   0 cardiel    (501) staff       (20)     2487 2022-11-06 08:39:16.000000 rgbloom-1.4/rgbloom/core/step1.py
--rw-r--r--   0 cardiel    (501) staff       (20)     1844 2022-11-06 08:39:16.000000 rgbloom-1.4/rgbloom/core/step2.py
--rw-r--r--   0 cardiel    (501) staff       (20)     3128 2023-03-21 17:40:50.000000 rgbloom-1.4/rgbloom/core/step3.py
--rw-r--r--   0 cardiel    (501) staff       (20)     2560 2022-11-06 08:39:16.000000 rgbloom-1.4/rgbloom/core/step4.py
--rw-r--r--   0 cardiel    (501) staff       (20)     3007 2023-03-21 17:42:15.000000 rgbloom-1.4/rgbloom/core/step5.py
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-22 11:44:14.626811 rgbloom-1.4/rgbloom/gui/
--rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-06 08:39:16.000000 rgbloom-1.4/rgbloom/gui/__init__.py
--rw-r--r--   0 cardiel    (501) staff       (20)    10034 2023-05-22 11:40:39.000000 rgbloom-1.4/rgbloom/gui/step6.py
--rw-r--r--   0 cardiel    (501) staff       (20)      497 2022-11-06 08:39:16.000000 rgbloom-1.4/rgbloom/gui/style.py
--rw-r--r--   0 cardiel    (501) staff       (20)       16 2023-05-22 11:40:39.000000 rgbloom-1.4/rgbloom/version.py
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-22 11:44:14.625016 rgbloom-1.4/rgbloom.egg-info/
--rw-r--r--   0 cardiel    (501) staff       (20)    12806 2023-05-22 11:44:14.000000 rgbloom-1.4/rgbloom.egg-info/PKG-INFO
--rw-r--r--   0 cardiel    (501) staff       (20)      499 2023-05-22 11:44:14.000000 rgbloom-1.4/rgbloom.egg-info/SOURCES.txt
--rw-r--r--   0 cardiel    (501) staff       (20)        1 2023-05-22 11:44:14.000000 rgbloom-1.4/rgbloom.egg-info/dependency_links.txt
--rw-r--r--   0 cardiel    (501) staff       (20)       50 2023-05-22 11:44:14.000000 rgbloom-1.4/rgbloom.egg-info/entry_points.txt
--rw-r--r--   0 cardiel    (501) staff       (20)       80 2023-05-22 11:44:14.000000 rgbloom-1.4/rgbloom.egg-info/requires.txt
--rw-r--r--   0 cardiel    (501) staff       (20)        8 2023-05-22 11:44:14.000000 rgbloom-1.4/rgbloom.egg-info/top_level.txt
--rw-r--r--   0 cardiel    (501) staff       (20)     1040 2023-05-22 11:44:14.627308 rgbloom-1.4/setup.cfg
--rw-r--r--   0 cardiel    (501) staff       (20)       68 2022-11-06 08:39:44.000000 rgbloom-1.4/setup.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-24 13:48:45.619313 rgbloom-1.5/
+-rw-r--r--   0 cardiel    (501) staff       (20)    35149 2022-11-06 08:36:25.000000 rgbloom-1.5/LICENSE
+-rw-r--r--   0 cardiel    (501) staff       (20)    13243 2023-05-24 13:48:45.619433 rgbloom-1.5/PKG-INFO
+-rw-r--r--   0 cardiel    (501) staff       (20)    12453 2023-05-24 13:46:56.000000 rgbloom-1.5/README.md
+-rw-r--r--   0 cardiel    (501) staff       (20)      100 2022-11-06 08:38:35.000000 rgbloom-1.5/pyproject.toml
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-24 13:48:45.582715 rgbloom-1.5/rgbloom/
+-rw-r--r--   0 cardiel    (501) staff       (20)       51 2022-11-06 08:39:16.000000 rgbloom-1.5/rgbloom/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     6597 2023-05-24 13:46:56.000000 rgbloom-1.5/rgbloom/__main__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)      439 2023-05-24 13:46:56.000000 rgbloom-1.5/rgbloom/choices_mag_plot.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-24 13:48:45.617696 rgbloom-1.5/rgbloom/core/
+-rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-06 08:39:16.000000 rgbloom-1.5/rgbloom/core/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     2487 2022-11-06 08:39:16.000000 rgbloom-1.5/rgbloom/core/step1.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1844 2022-11-06 08:39:16.000000 rgbloom-1.5/rgbloom/core/step2.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     3128 2023-03-21 17:40:50.000000 rgbloom-1.5/rgbloom/core/step3.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     2560 2022-11-06 08:39:16.000000 rgbloom-1.5/rgbloom/core/step4.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     3007 2023-03-21 17:42:15.000000 rgbloom-1.5/rgbloom/core/step5.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-24 13:48:45.618798 rgbloom-1.5/rgbloom/gui/
+-rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-06 08:39:16.000000 rgbloom-1.5/rgbloom/gui/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)    11742 2023-05-24 13:46:56.000000 rgbloom-1.5/rgbloom/gui/step6.py
+-rw-r--r--   0 cardiel    (501) staff       (20)      497 2022-11-06 08:39:16.000000 rgbloom-1.5/rgbloom/gui/style.py
+-rw-r--r--   0 cardiel    (501) staff       (20)       16 2023-05-24 13:46:56.000000 rgbloom-1.5/rgbloom/version.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-24 13:48:45.584888 rgbloom-1.5/rgbloom.egg-info/
+-rw-r--r--   0 cardiel    (501) staff       (20)    13243 2023-05-24 13:48:45.000000 rgbloom-1.5/rgbloom.egg-info/PKG-INFO
+-rw-r--r--   0 cardiel    (501) staff       (20)      527 2023-05-24 13:48:45.000000 rgbloom-1.5/rgbloom.egg-info/SOURCES.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)        1 2023-05-24 13:48:45.000000 rgbloom-1.5/rgbloom.egg-info/dependency_links.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)       50 2023-05-24 13:48:45.000000 rgbloom-1.5/rgbloom.egg-info/entry_points.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)       80 2023-05-24 13:48:45.000000 rgbloom-1.5/rgbloom.egg-info/requires.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)        8 2023-05-24 13:48:45.000000 rgbloom-1.5/rgbloom.egg-info/top_level.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)     1040 2023-05-24 13:48:45.620096 rgbloom-1.5/setup.cfg
+-rw-r--r--   0 cardiel    (501) staff       (20)       68 2022-11-06 08:39:44.000000 rgbloom-1.5/setup.py
```

### Comparing `rgbloom-1.4/LICENSE` & `rgbloom-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rgbloom-1.4/PKG-INFO` & `rgbloom-1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: rgbloom
-Version: 1.4
-Summary: RGB from Gaia EDR3
-Home-page: https://github.com/guaix-ucm/rgbloom
-Author: Nicolás Cardiel
-Author-email: cardiel@ucm.es
-License: GPLv3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Astronomy
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # rgbloom
 
 This Python script retrieves RGB magnitudes computed from low resolution
 spectra published in *Gaia* DR3, following the work described in 
 [Carrasco et al. (2023)](#3).
 These magnitudes are given in the standard system defined by
 [Cardiel et al. (2021a)](#1).
@@ -57,40 +35,40 @@
 ## Installing the code
 
 In order to keep your current Python installation clean, it is highly 
 recommended to first build Python 3 *virtual environment*.
 
 ### Creating and activating the Python virtual environment
 
-```bash
+```shell
 $ python3 -m venv venv_rgb
 $ . venv_rgb/bin/activate
 (venv_rgb) $
 ```
 
 ### Installing the package
 
 We recommend installing the latest stable version, which is available via
-the PyPI respository:
+the [PyPI respository](https://pypi.org/project/rgbloom/):
 
-```bash
+```shell
 (venv_rgb) $ pip install rgbloom
 ```
 
 The latest development version is available through GitHub:
 
-```bash
+```shell
 (venv_rgb) $ pip install git+https://github.com/guaix-ucm/rgbloom.git@main#egg=rgbloom
 ```
 
 ## Executing the program
 
 Just execute it from the command line:
 
-```bash
+```shell
 (venv_rgb) $ rgbloom 56.66 24.10 1.0 12
 ```
 
 The last instruction executes the program providing the 
 four positional arguments: right ascension, declination, search radius and 
 limiting *Gaia* G magnitude. *Note that the coordinates and search radius 
 must be given in decimal degrees*.
@@ -103,15 +81,15 @@
 recover disk space).
 
 The execution of this example should led to the following output in the
 terminal (except for the absolute path where the auxiliary downloaded files 
 are stored):
 
 ```
-        Welcome to rgbloom version 1.4
+        Welcome to rgbloom version 1.5
         ==============================
 
 Downloading data from 'http://nartex.fis.ucm.es/~ncl/rgbphot/gaiaDR3/reference_healpix8.csv' to file '/Users/cardiel/Library/Caches/pooch/635cd722cf61b23bd8eee20635e4d580-reference_healpix8.csv'.
 <STEP1> Starting cone search in Gaia DR3... (please wait)
   INFO: Query finished. [astroquery.utils.tap.core]
         --> 310 objects found
         --> 23 objects classified as VARIABLE
@@ -216,27 +194,32 @@
   grey diamond on objects outside the *Gaia* -0.5 < G_BP - G_RP < 2.0 colour
   interval.
 
 Note that the three output archives (1 PDF and 2 CSV files) share the same root
 name `rgbloom`. This can be easily modified using the optional argument
 `--basename <newbasename>` in the command line.
 
+Since version 1.5, it is also possible to display a particular magnitude
+(instead of the objetc number in the CSV files) using `--display_mag
+<magname>`, where `<magname>` can be any of the following: `RGB_B`, `RGB_R`,
+`RGB_R`, `Gaia_G`, `Gaia_BP`, `Gaia_RP`, `Gaia_BP-RP`.
+
+
 ### Additional help
 
 Some auxiliary optional arguments are also available. See description 
 invoking the script help:
 
-```bash
+```shell
 $ rgbloom --help
-usage: rgbloom [-h] [--basename BASENAME] [--brightlimit BRIGHTLIMIT] [--symbsize SYMBSIZE] [--max_symbsize MAX_SYMBSIZE]
-               [--min_symbsize MIN_SYMBSIZE] [--mag_power MAG_POWER] [--display_g_mag] [--num_fontsize NUM_FONTSIZE]
-               [--nonumbers] [--noplot] [--nocolor] [--verbose]
+usage: rgbloom [-h] [--basename BASENAME] [--brightlimit BRIGHTLIMIT] [--symbsize SYMBSIZE] [--max_symbsize MAX_SYMBSIZE] [--min_symbsize MIN_SYMBSIZE] [--mag_power MAG_POWER] [--display_mag {None,RGB_B,RGB_G,RGB_R,Gaia_G,Gaia_BP,Gaia_RP,Gaia_BP_RP}]
+               [--num_fontsize NUM_FONTSIZE] [--nonumbers] [--noplot] [--nocolor] [--verbose]
                ra_center dec_center search_radius g_limit
 
-RGB predictions from Gaia DR3 spectrophotometry (version 1.4)
+RGB predictions from Gaia DR3 spectrophotometry (version 1.5)
 
 positional arguments:
   ra_center             right Ascension (decimal degrees)
   dec_center            declination (decimal degrees)
   search_radius         search radius (decimal degrees)
   g_limit               limiting Gaia G magnitude
 
@@ -248,15 +231,16 @@
   --symbsize SYMBSIZE   global multiplying factor for symbol size (default=1.0)
   --max_symbsize MAX_SYMBSIZE
                         maximum symbol size in chart (default=1000)
   --min_symbsize MIN_SYMBSIZE
                         minimum symbol size in chart (default=10)
   --mag_power MAG_POWER
                         power to scale symbol sizes in chart (default=3)
-  --display_g_mag       display Gaia G magnitude instead of object number
+  --display_mag {None,RGB_B,RGB_G,RGB_R,Gaia_G,Gaia_BP,Gaia_RP,Gaia_BP_RP}
+                        display selected magnitude instead of object number
   --num_fontsize NUM_FONTSIZE
                         font size for numbers in chart (default=5)
   --nonumbers           do not display object identification number in PDF chart
   --noplot              skip PDF chart generation
   --nocolor             do not use colors in PDF chart
   --verbose             increase program verbosity
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rgbloom-1.4/README.md` & `rgbloom-1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: rgbloom
+Version: 1.5
+Summary: RGB from Gaia EDR3
+Home-page: https://github.com/guaix-ucm/rgbloom
+Author: Nicolás Cardiel
+Author-email: cardiel@ucm.es
+License: GPLv3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Astronomy
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # rgbloom
 
 This Python script retrieves RGB magnitudes computed from low resolution
 spectra published in *Gaia* DR3, following the work described in 
 [Carrasco et al. (2023)](#3).
 These magnitudes are given in the standard system defined by
 [Cardiel et al. (2021a)](#1).
@@ -35,40 +57,40 @@
 ## Installing the code
 
 In order to keep your current Python installation clean, it is highly 
 recommended to first build Python 3 *virtual environment*.
 
 ### Creating and activating the Python virtual environment
 
-```bash
+```shell
 $ python3 -m venv venv_rgb
 $ . venv_rgb/bin/activate
 (venv_rgb) $
 ```
 
 ### Installing the package
 
 We recommend installing the latest stable version, which is available via
-the PyPI respository:
+the [PyPI respository](https://pypi.org/project/rgbloom/):
 
-```bash
+```shell
 (venv_rgb) $ pip install rgbloom
 ```
 
 The latest development version is available through GitHub:
 
-```bash
+```shell
 (venv_rgb) $ pip install git+https://github.com/guaix-ucm/rgbloom.git@main#egg=rgbloom
 ```
 
 ## Executing the program
 
 Just execute it from the command line:
 
-```bash
+```shell
 (venv_rgb) $ rgbloom 56.66 24.10 1.0 12
 ```
 
 The last instruction executes the program providing the 
 four positional arguments: right ascension, declination, search radius and 
 limiting *Gaia* G magnitude. *Note that the coordinates and search radius 
 must be given in decimal degrees*.
@@ -81,15 +103,15 @@
 recover disk space).
 
 The execution of this example should led to the following output in the
 terminal (except for the absolute path where the auxiliary downloaded files 
 are stored):
 
 ```
-        Welcome to rgbloom version 1.4
+        Welcome to rgbloom version 1.5
         ==============================
 
 Downloading data from 'http://nartex.fis.ucm.es/~ncl/rgbphot/gaiaDR3/reference_healpix8.csv' to file '/Users/cardiel/Library/Caches/pooch/635cd722cf61b23bd8eee20635e4d580-reference_healpix8.csv'.
 <STEP1> Starting cone search in Gaia DR3... (please wait)
   INFO: Query finished. [astroquery.utils.tap.core]
         --> 310 objects found
         --> 23 objects classified as VARIABLE
@@ -194,27 +216,32 @@
   grey diamond on objects outside the *Gaia* -0.5 < G_BP - G_RP < 2.0 colour
   interval.
 
 Note that the three output archives (1 PDF and 2 CSV files) share the same root
 name `rgbloom`. This can be easily modified using the optional argument
 `--basename <newbasename>` in the command line.
 
+Since version 1.5, it is also possible to display a particular magnitude
+(instead of the objetc number in the CSV files) using `--display_mag
+<magname>`, where `<magname>` can be any of the following: `RGB_B`, `RGB_R`,
+`RGB_R`, `Gaia_G`, `Gaia_BP`, `Gaia_RP`, `Gaia_BP-RP`.
+
+
 ### Additional help
 
 Some auxiliary optional arguments are also available. See description 
 invoking the script help:
 
-```bash
+```shell
 $ rgbloom --help
-usage: rgbloom [-h] [--basename BASENAME] [--brightlimit BRIGHTLIMIT] [--symbsize SYMBSIZE] [--max_symbsize MAX_SYMBSIZE]
-               [--min_symbsize MIN_SYMBSIZE] [--mag_power MAG_POWER] [--display_g_mag] [--num_fontsize NUM_FONTSIZE]
-               [--nonumbers] [--noplot] [--nocolor] [--verbose]
+usage: rgbloom [-h] [--basename BASENAME] [--brightlimit BRIGHTLIMIT] [--symbsize SYMBSIZE] [--max_symbsize MAX_SYMBSIZE] [--min_symbsize MIN_SYMBSIZE] [--mag_power MAG_POWER] [--display_mag {None,RGB_B,RGB_G,RGB_R,Gaia_G,Gaia_BP,Gaia_RP,Gaia_BP_RP}]
+               [--num_fontsize NUM_FONTSIZE] [--nonumbers] [--noplot] [--nocolor] [--verbose]
                ra_center dec_center search_radius g_limit
 
-RGB predictions from Gaia DR3 spectrophotometry (version 1.4)
+RGB predictions from Gaia DR3 spectrophotometry (version 1.5)
 
 positional arguments:
   ra_center             right Ascension (decimal degrees)
   dec_center            declination (decimal degrees)
   search_radius         search radius (decimal degrees)
   g_limit               limiting Gaia G magnitude
 
@@ -226,15 +253,16 @@
   --symbsize SYMBSIZE   global multiplying factor for symbol size (default=1.0)
   --max_symbsize MAX_SYMBSIZE
                         maximum symbol size in chart (default=1000)
   --min_symbsize MIN_SYMBSIZE
                         minimum symbol size in chart (default=10)
   --mag_power MAG_POWER
                         power to scale symbol sizes in chart (default=3)
-  --display_g_mag       display Gaia G magnitude instead of object number
+  --display_mag {None,RGB_B,RGB_G,RGB_R,Gaia_G,Gaia_BP,Gaia_RP,Gaia_BP_RP}
+                        display selected magnitude instead of object number
   --num_fontsize NUM_FONTSIZE
                         font size for numbers in chart (default=5)
   --nonumbers           do not display object identification number in PDF chart
   --noplot              skip PDF chart generation
   --nocolor             do not use colors in PDF chart
   --verbose             increase program verbosity
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rgbloom-1.4/rgbloom/__main__.py` & `rgbloom-1.5/rgbloom/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 """
 
 import argparse
 import pandas as pd
 import pooch
 import sys
 
+from .choices_mag_plot import CHOICES_MAG_PLOT
 from .core.step1 import step1
 from .core.step2 import step2
 from .core.step3 import step3
 from .core.step4 import step4
 from .core.step5 import step5
 from .gui.step6 import step6
 from .version import version
@@ -151,15 +152,15 @@
             args.dec_center,
             args.search_radius,
             args.brightlimit,
             args.symbsize,
             args.max_symbsize,
             args.min_symbsize,
             args.mag_power,
-            args.display_g_mag,
+            args.display_mag,
             args.num_fontsize,
             args.nonumbers,
             args.nocolor,
             args.basename,
             version,
             args.verbose
         )
@@ -181,16 +182,16 @@
                         type=float, default=1.0)
     parser.add_argument("--max_symbsize", help="maximum symbol size in chart (default=1000)",
                         type=float, default=1000)
     parser.add_argument("--min_symbsize", help="minimum symbol size in chart (default=10)",
                         type=float, default=10)
     parser.add_argument("--mag_power", help="power to scale symbol sizes in chart (default=3)",
                         type=float, default=3)
-    parser.add_argument("--display_g_mag", help="display Gaia G magnitude instead of object number",
-                        action="store_true")
+    parser.add_argument("--display_mag", help="display selected magnitude instead of object number",
+                        type=str, default="None", choices=list(CHOICES_MAG_PLOT.keys()))
     parser.add_argument("--num_fontsize", help="font size for numbers in chart (default=5)",
                         type=int, default=5)
     parser.add_argument("--nonumbers", help="do not display object identification number in PDF chart",
                         action="store_true")
     parser.add_argument("--noplot", help="skip PDF chart generation", action="store_true")
     parser.add_argument("--nocolor", help="do not use colors in PDF chart", action="store_true")
     parser.add_argument("--verbose", help="increase program verbosity", action="store_true")
```

### Comparing `rgbloom-1.4/rgbloom/core/step1.py` & `rgbloom-1.5/rgbloom/core/step1.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.4/rgbloom/core/step2.py` & `rgbloom-1.5/rgbloom/core/step2.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.4/rgbloom/core/step3.py` & `rgbloom-1.5/rgbloom/core/step3.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.4/rgbloom/core/step4.py` & `rgbloom-1.5/rgbloom/core/step4.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.4/rgbloom/core/step5.py` & `rgbloom-1.5/rgbloom/core/step5.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.4/rgbloom/gui/step6.py` & `rgbloom-1.5/rgbloom/gui/step6.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 from astropy.wcs import WCS
 from astropy.coordinates import SkyCoord
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import matplotlib.style
 import numpy as np
 
+from ..choices_mag_plot import CHOICES_MAG_PLOT
 from .style import mpl_style
 OUTTYPES_COLOR = {'200m': 'red', 'no200m': 'black', 'var': 'blue'}
 
 matplotlib.use('pdf')
 
 
 def step6(r_dr3_200m, r_dr3_no200m, ra_center, dec_center, search_radius, brightlimit,
           symbsize, max_symbsize, min_symbsize, mag_power,
-          display_g_mag, num_fontsize, nonumbers, nocolor,
+          display_mag, num_fontsize, nonumbers, nocolor,
           basename, version, verbose):
     """Perform EDR3 query
 
     Parameters
     ----------
     r_dr3_200m : astropy Table
         Objects in both the DR3 query and the 200M sample.
@@ -54,16 +55,16 @@
         Maximum symbol size in chart.
     min_symbsize : float
         Minimum symbol size in chart.
     mag_power: float
         Power to scale symbol sizes in chart. The relative magnitude
         difference (rescaled between 0 and 1) is raised to this power
         to set the symbol size.
-    display_g_mag : bool
-        If True display Gaia G mag instead of object number.
+    display_mag : bool
+        If True display selected magnitude instead of object number.
     num_fontsize : int
         Font size for numbers in chart.
     nonumbers : bool
         If True, do not display star numbers in PDF chart.
     nocolor : bool
         If True, do not use colors in PDF chart.
     basename : str
@@ -147,16 +148,20 @@
                 ax.scatter(x_pix[i], y_pix[i], marker='.',
                            edgecolors='black', linewidth=0.2, s=symbol_size[i], zorder=i+1,
                            cmap=cmap, c=r_table[i]['bp_rp'], vmin=cmap_vmin, vmax=cmap_vmax)
 
         # display numbers if requested
         if not nonumbers:
             for irow in range(len(r_table)):
-                if display_g_mag:
-                    text = f'{r_table[irow]["phot_g_mean_mag"]:.2f}'
+                if CHOICES_MAG_PLOT[display_mag] is not None:
+                    dumvalue = r_table[irow][CHOICES_MAG_PLOT[display_mag]]
+                    if isinstance(dumvalue, np.ma.core.MaskedConstant):
+                        text = 'NA'  # Not Available
+                    else:
+                        text = f'{dumvalue:.2f}'
                 else:
                     text = r_table[irow]['number']
                 if r_table[irow]['qlflag'] == 1:
                     bbox = dict(facecolor='none', edgecolor='gray', boxstyle='round, pad=0.2', lw=1, alpha=0.3)
                 else:
                     bbox = None
                 if isinstance(r_table[irow]['qlflag'], np.int64):
@@ -186,25 +191,45 @@
         mask_variable = r_dr3_no200m['phot_variable_flag'] == 'VARIABLE'
         if np.any(mask_variable):
             iok_bool = np.argwhere(mask_variable)
             ax.scatter(x_pix[iok_bool], y_pix[iok_bool], s=240, marker='s',
                        facecolors='none', edgecolors=OUTTYPES_COLOR['var'], linewidth=0.5, zorder=0)
 
     # legend
-    ax.scatter(0.03, 0.96, s=240, marker='s', facecolors='white',
+    ax.scatter(0.03, 0.97, s=240, marker='s', facecolors='white',
                edgecolors=OUTTYPES_COLOR['var'], linewidth=0.5,
                transform=ax.transAxes)
-    ax.text(0.06, 0.96, 'variable in Gaia DR3', fontsize=12, backgroundcolor='white',
+    ax.text(0.06, 0.97, 'variable in Gaia DR3', fontsize=12, backgroundcolor='white',
             horizontalalignment='left', verticalalignment='center', transform=ax.transAxes)
 
-    ax.scatter(0.03, 0.92, s=240, marker='D', facecolors='white', edgecolors='grey', linewidth=0.5,
+    ax.scatter(0.03, 0.93, s=240, marker='D', facecolors='white', edgecolors='grey', linewidth=0.5,
                transform=ax.transAxes)
-    ax.text(0.06, 0.92, 'outside colour range', fontsize=12, backgroundcolor='white',
+    ax.text(0.06, 0.93, 'outside colour range', fontsize=12, backgroundcolor='white',
             horizontalalignment='left', verticalalignment='center', transform=ax.transAxes)
 
+    if CHOICES_MAG_PLOT[display_mag] is None:
+        ax.text(0.03, 0.89, 'n', color='red', fontsize=12,
+                horizontalalignment='center', verticalalignment='center', transform=ax.transAxes)
+        ax.text(0.06, 0.89, '# in *_200m.csv', color='gray', fontsize=12,
+                horizontalalignment='left', verticalalignment='center', transform=ax.transAxes)
+        ax.text(0.03, 0.85, 'n', color='black', fontsize=12,
+                horizontalalignment='center', verticalalignment='center', transform=ax.transAxes)
+        ax.text(0.06, 0.85, '# in *_no200m.csv', color='gray', fontsize=12,
+                horizontalalignment='left', verticalalignment='center', transform=ax.transAxes)
+    else:
+        ax.text(0.03, 0.89, 'mag', color='red', fontsize=12,
+                horizontalalignment='center', verticalalignment='center', transform=ax.transAxes)
+        ax.text(0.06, 0.89, f'{display_mag} in *_200m.csv', color='gray', fontsize=12,
+                horizontalalignment='left', verticalalignment='center', transform=ax.transAxes)
+        ax.text(0.03, 0.85, 'mag', color='black', fontsize=12,
+                horizontalalignment='center', verticalalignment='center', transform=ax.transAxes)
+        ax.text(0.06, 0.85, f'{display_mag} in *_no200m.csv', color='gray', fontsize=12,
+                horizontalalignment='left', verticalalignment='center', transform=ax.transAxes)
+
+    # plot labels
     ax.set_xlabel('ra')
     ax.set_ylabel('dec')
 
     ax.set_aspect('equal')
 
     if not nocolor:
         cbaxes = fig.add_axes([0.683, 0.81, 0.15, 0.02])
```

### Comparing `rgbloom-1.4/rgbloom.egg-info/PKG-INFO` & `rgbloom-1.5/rgbloom.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgbloom
-Version: 1.4
+Version: 1.5
 Summary: RGB from Gaia EDR3
 Home-page: https://github.com/guaix-ucm/rgbloom
 Author: Nicolás Cardiel
 Author-email: cardiel@ucm.es
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -57,40 +57,40 @@
 ## Installing the code
 
 In order to keep your current Python installation clean, it is highly 
 recommended to first build Python 3 *virtual environment*.
 
 ### Creating and activating the Python virtual environment
 
-```bash
+```shell
 $ python3 -m venv venv_rgb
 $ . venv_rgb/bin/activate
 (venv_rgb) $
 ```
 
 ### Installing the package
 
 We recommend installing the latest stable version, which is available via
-the PyPI respository:
+the [PyPI respository](https://pypi.org/project/rgbloom/):
 
-```bash
+```shell
 (venv_rgb) $ pip install rgbloom
 ```
 
 The latest development version is available through GitHub:
 
-```bash
+```shell
 (venv_rgb) $ pip install git+https://github.com/guaix-ucm/rgbloom.git@main#egg=rgbloom
 ```
 
 ## Executing the program
 
 Just execute it from the command line:
 
-```bash
+```shell
 (venv_rgb) $ rgbloom 56.66 24.10 1.0 12
 ```
 
 The last instruction executes the program providing the 
 four positional arguments: right ascension, declination, search radius and 
 limiting *Gaia* G magnitude. *Note that the coordinates and search radius 
 must be given in decimal degrees*.
@@ -103,15 +103,15 @@
 recover disk space).
 
 The execution of this example should led to the following output in the
 terminal (except for the absolute path where the auxiliary downloaded files 
 are stored):
 
 ```
-        Welcome to rgbloom version 1.4
+        Welcome to rgbloom version 1.5
         ==============================
 
 Downloading data from 'http://nartex.fis.ucm.es/~ncl/rgbphot/gaiaDR3/reference_healpix8.csv' to file '/Users/cardiel/Library/Caches/pooch/635cd722cf61b23bd8eee20635e4d580-reference_healpix8.csv'.
 <STEP1> Starting cone search in Gaia DR3... (please wait)
   INFO: Query finished. [astroquery.utils.tap.core]
         --> 310 objects found
         --> 23 objects classified as VARIABLE
@@ -216,27 +216,32 @@
   grey diamond on objects outside the *Gaia* -0.5 < G_BP - G_RP < 2.0 colour
   interval.
 
 Note that the three output archives (1 PDF and 2 CSV files) share the same root
 name `rgbloom`. This can be easily modified using the optional argument
 `--basename <newbasename>` in the command line.
 
+Since version 1.5, it is also possible to display a particular magnitude
+(instead of the objetc number in the CSV files) using `--display_mag
+<magname>`, where `<magname>` can be any of the following: `RGB_B`, `RGB_R`,
+`RGB_R`, `Gaia_G`, `Gaia_BP`, `Gaia_RP`, `Gaia_BP-RP`.
+
+
 ### Additional help
 
 Some auxiliary optional arguments are also available. See description 
 invoking the script help:
 
-```bash
+```shell
 $ rgbloom --help
-usage: rgbloom [-h] [--basename BASENAME] [--brightlimit BRIGHTLIMIT] [--symbsize SYMBSIZE] [--max_symbsize MAX_SYMBSIZE]
-               [--min_symbsize MIN_SYMBSIZE] [--mag_power MAG_POWER] [--display_g_mag] [--num_fontsize NUM_FONTSIZE]
-               [--nonumbers] [--noplot] [--nocolor] [--verbose]
+usage: rgbloom [-h] [--basename BASENAME] [--brightlimit BRIGHTLIMIT] [--symbsize SYMBSIZE] [--max_symbsize MAX_SYMBSIZE] [--min_symbsize MIN_SYMBSIZE] [--mag_power MAG_POWER] [--display_mag {None,RGB_B,RGB_G,RGB_R,Gaia_G,Gaia_BP,Gaia_RP,Gaia_BP_RP}]
+               [--num_fontsize NUM_FONTSIZE] [--nonumbers] [--noplot] [--nocolor] [--verbose]
                ra_center dec_center search_radius g_limit
 
-RGB predictions from Gaia DR3 spectrophotometry (version 1.4)
+RGB predictions from Gaia DR3 spectrophotometry (version 1.5)
 
 positional arguments:
   ra_center             right Ascension (decimal degrees)
   dec_center            declination (decimal degrees)
   search_radius         search radius (decimal degrees)
   g_limit               limiting Gaia G magnitude
 
@@ -248,15 +253,16 @@
   --symbsize SYMBSIZE   global multiplying factor for symbol size (default=1.0)
   --max_symbsize MAX_SYMBSIZE
                         maximum symbol size in chart (default=1000)
   --min_symbsize MIN_SYMBSIZE
                         minimum symbol size in chart (default=10)
   --mag_power MAG_POWER
                         power to scale symbol sizes in chart (default=3)
-  --display_g_mag       display Gaia G magnitude instead of object number
+  --display_mag {None,RGB_B,RGB_G,RGB_R,Gaia_G,Gaia_BP,Gaia_RP,Gaia_BP_RP}
+                        display selected magnitude instead of object number
   --num_fontsize NUM_FONTSIZE
                         font size for numbers in chart (default=5)
   --nonumbers           do not display object identification number in PDF chart
   --noplot              skip PDF chart generation
   --nocolor             do not use colors in PDF chart
   --verbose             increase program verbosity
 ```
```

### Comparing `rgbloom-1.4/setup.cfg` & `rgbloom-1.5/setup.cfg`

 * *Files identical despite different names*

