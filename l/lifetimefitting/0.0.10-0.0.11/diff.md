# Comparing `tmp/lifetimefitting-0.0.10.tar.gz` & `tmp/lifetimefitting-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifetimefitting-0.0.10.tar", last modified: Thu May 25 20:25:46 2023, max compression
+gzip compressed data, was "lifetimefitting-0.0.11.tar", last modified: Thu May 25 21:01:01 2023, max compression
```

## Comparing `lifetimefitting-0.0.10.tar` & `lifetimefitting-0.0.11.tar`

### file list

```diff
@@ -1,22 +1,19 @@
-drwxr-xr-x   0 adrea      (502) staff       (20)        0 2023-05-25 20:25:46.448993 lifetimefitting-0.0.10/
--rw-r--r--   0 adrea      (502) staff       (20)       53 2023-05-25 18:16:23.000000 lifetimefitting-0.0.10/.gitignore
--rw-r--r--   0 adrea      (502) staff       (20)     1062 2023-05-25 19:43:07.000000 lifetimefitting-0.0.10/LICENSE.md
--rw-r--r--   0 adrea      (502) staff       (20)     2150 2023-05-25 20:25:46.448821 lifetimefitting-0.0.10/PKG-INFO
--rw-r--r--   0 adrea      (502) staff       (20)     1674 2023-05-25 20:23:16.000000 lifetimefitting-0.0.10/README.md
-drwxr-xr-x   0 adrea      (502) staff       (20)        0 2023-05-25 20:25:46.443219 lifetimefitting-0.0.10/app/
-drwxr-xr-x   0 adrea      (502) staff       (20)        0 2023-05-25 20:25:46.447337 lifetimefitting-0.0.10/app/lifetimefitting/
--rw-r--r--   0 adrea      (502) staff       (20)        0 2023-05-25 20:03:04.000000 lifetimefitting-0.0.10/app/lifetimefitting/__init__.py
--rw-r--r--   0 adrea      (502) staff       (20)    10040 2023-05-25 20:08:09.000000 lifetimefitting-0.0.10/app/lifetimefitting/__main__.py
--rw-r--r--   0 adrea      (502) staff       (20)     2013 2023-05-25 18:41:40.000000 lifetimefitting-0.0.10/app/lifetimefitting/funcs.py
--rw-r--r--   0 adrea      (502) staff       (20)    12256 2023-05-25 19:04:12.000000 lifetimefitting-0.0.10/app/lifetimefitting/gui.py
--rw-r--r--   0 adrea      (502) staff       (20)     7705 2023-05-25 14:22:16.000000 lifetimefitting-0.0.10/app/lifetimefitting/phd.py
-drwxr-xr-x   0 adrea      (502) staff       (20)        0 2023-05-25 20:25:46.448528 lifetimefitting-0.0.10/app/lifetimefitting.egg-info/
--rw-r--r--   0 adrea      (502) staff       (20)     2150 2023-05-25 20:25:46.000000 lifetimefitting-0.0.10/app/lifetimefitting.egg-info/PKG-INFO
--rw-r--r--   0 adrea      (502) staff       (20)      431 2023-05-25 20:25:46.000000 lifetimefitting-0.0.10/app/lifetimefitting.egg-info/SOURCES.txt
--rw-r--r--   0 adrea      (502) staff       (20)        1 2023-05-25 20:25:46.000000 lifetimefitting-0.0.10/app/lifetimefitting.egg-info/dependency_links.txt
--rw-r--r--   0 adrea      (502) staff       (20)       49 2023-05-25 20:25:46.000000 lifetimefitting-0.0.10/app/lifetimefitting.egg-info/requires.txt
--rw-r--r--   0 adrea      (502) staff       (20)       16 2023-05-25 20:25:46.000000 lifetimefitting-0.0.10/app/lifetimefitting.egg-info/top_level.txt
--rw-r--r--   0 adrea      (502) staff       (20)    11590 2023-05-25 18:05:49.000000 lifetimefitting-0.0.10/lifetimeGui.ui
--rw-r--r--   0 adrea      (502) staff       (20)   873440 2023-05-25 18:17:30.000000 lifetimefitting-0.0.10/screenshot.png
--rw-r--r--   0 adrea      (502) staff       (20)       38 2023-05-25 20:25:46.449039 lifetimefitting-0.0.10/setup.cfg
--rw-r--r--   0 adrea      (502) staff       (20)      867 2023-05-25 20:25:40.000000 lifetimefitting-0.0.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:01:01.291925 lifetimefitting-0.0.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-25 21:00:47.000000 lifetimefitting-0.0.11/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-25 21:01:01.291925 lifetimefitting-0.0.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-25 21:00:47.000000 lifetimefitting-0.0.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:01:01.291925 lifetimefitting-0.0.11/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:01:01.291925 lifetimefitting-0.0.11/app/lifetimefitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:00:47.000000 lifetimefitting-0.0.11/app/lifetimefitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-05-25 21:00:47.000000 lifetimefitting-0.0.11/app/lifetimefitting/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-25 21:00:47.000000 lifetimefitting-0.0.11/app/lifetimefitting/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12256 2023-05-25 21:00:47.000000 lifetimefitting-0.0.11/app/lifetimefitting/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-25 21:00:47.000000 lifetimefitting-0.0.11/app/lifetimefitting/phd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:01:01.291925 lifetimefitting-0.0.11/app/lifetimefitting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-25 21:01:01.000000 lifetimefitting-0.0.11/app/lifetimefitting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-25 21:01:01.000000 lifetimefitting-0.0.11/app/lifetimefitting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:01:01.000000 lifetimefitting-0.0.11/app/lifetimefitting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-25 21:01:01.000000 lifetimefitting-0.0.11/app/lifetimefitting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 21:01:01.000000 lifetimefitting-0.0.11/app/lifetimefitting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:01:01.291925 lifetimefitting-0.0.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-25 21:00:47.000000 lifetimefitting-0.0.11/setup.py
```

### Comparing `lifetimefitting-0.0.10/LICENSE.md` & `lifetimefitting-0.0.11/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.10/PKG-INFO` & `lifetimefitting-0.0.11/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.10
+Version: 0.0.11
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,25 @@
 # LifetimeFittingTool
 This is a quick tool I wrote to take some of my TCSPC fluorescence lifetime fitting tools from [spectraImport.ipynb](https://github.com/adreasnow/excided-state-notebooks/blob/main/spectraImport.ipynb) and make them usable for other people. It can read PicoHarp .phd files thanks to [adreasnow/picoharp-phd](https://github.com/adreasnow/picoharp-phd) and also reads the plain `.txt` output it can save.
 
 ![screenshot](screenshot.png)
 
 The app itself is a basic least squares regression tool but allows you to fit in linear or logarithmic space, supports up to 4 decays, and can export images as well as .csv files of the fitted histograms
 
-## Requirements
+## Installing
+
+### PyPi
+
+The easiest way to get it is to install it directly from pypy, so as too pull all the dependencies:
+
+```python
+pip install lifetimefitting
+```
+
+### Manually
 
 * Python (I'm not sure how old you could go, but I know it runs on >3.9)
 * Matplotlib
 * Numpy
 * PyQt5
 * Scipy
 
@@ -36,14 +46,30 @@
 
 or conda
 
 ```bash
 conda install matplotlib numpy scipy pyqt5
 ```
 
+Then you can clone the module down and install it manually
+
+```bash
+git clone https://github.com/adreasnow/LifetimeFittingTool.git
+cd LifetimeFittingTool
+python setup.py install
+```
+
+## Usage
+
+To run the app, all you need to do is execute the module in python and a QT window should appear :)
+
+```bash
+python -m lifetimefitting
+```
+
 
 
 ## The Maths
 
 Uses the form of the function:
 
 $$
@@ -58,15 +84,15 @@
 For the corrected fitting procedure, the convolved function is calculated as:
 
 $$
 fl=fl(t)_{IRF}\otimes fl(t)
 $$
 
 $$
-fl_{fitted}=\sum_{i=1}^{\text{\# exponents}} C_i\cdot fl(t)_i
+fl_{fitted}=\sum_{i=1}^{\text{exponents}} C_i\cdot fl(t)_i
 $$
 
 Where:
 * $fl(t)_{IRF} =$ Fitted instrument response function
 * $fl(t)_i =$ Fitted function for each decay
 * $C_i =$ Linear coefficient for each decay
```

### Comparing `lifetimefitting-0.0.10/README.md` & `lifetimefitting-0.0.11/app/lifetimefitting.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,40 @@
+Metadata-Version: 2.1
+Name: lifetimefitting
+Version: 0.0.11
+Summary: PicoHarp TCSPC lifetime fitting tool
+Home-page: https://github.com/adreasnow/LifetimeFittingTool
+Author: Adrea Snow
+Author-email: adrea.snow@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.md
+
 # LifetimeFittingTool
 This is a quick tool I wrote to take some of my TCSPC fluorescence lifetime fitting tools from [spectraImport.ipynb](https://github.com/adreasnow/excided-state-notebooks/blob/main/spectraImport.ipynb) and make them usable for other people. It can read PicoHarp .phd files thanks to [adreasnow/picoharp-phd](https://github.com/adreasnow/picoharp-phd) and also reads the plain `.txt` output it can save.
 
 ![screenshot](screenshot.png)
 
 The app itself is a basic least squares regression tool but allows you to fit in linear or logarithmic space, supports up to 4 decays, and can export images as well as .csv files of the fitted histograms
 
-## Requirements
+## Installing
+
+### PyPi
+
+The easiest way to get it is to install it directly from pypy, so as too pull all the dependencies:
+
+```python
+pip install lifetimefitting
+```
+
+### Manually
 
 * Python (I'm not sure how old you could go, but I know it runs on >3.9)
 * Matplotlib
 * Numpy
 * PyQt5
 * Scipy
 
@@ -21,14 +46,30 @@
 
 or conda
 
 ```bash
 conda install matplotlib numpy scipy pyqt5
 ```
 
+Then you can clone the module down and install it manually
+
+```bash
+git clone https://github.com/adreasnow/LifetimeFittingTool.git
+cd LifetimeFittingTool
+python setup.py install
+```
+
+## Usage
+
+To run the app, all you need to do is execute the module in python and a QT window should appear :)
+
+```bash
+python -m lifetimefitting
+```
+
 
 
 ## The Maths
 
 Uses the form of the function:
 
 $$
@@ -43,21 +84,21 @@
 For the corrected fitting procedure, the convolved function is calculated as:
 
 $$
 fl=fl(t)_{IRF}\otimes fl(t)
 $$
 
 $$
-fl_{fitted}=\sum_{i=1}^{\text{\# exponents}} C_i\cdot fl(t)_i
+fl_{fitted}=\sum_{i=1}^{\text{exponents}} C_i\cdot fl(t)_i
 $$
 
 Where:
 * $fl(t)_{IRF} =$ Fitted instrument response function
 * $fl(t)_i =$ Fitted function for each decay
 * $C_i =$ Linear coefficient for each decay
 
 $\chi^2$ is calculated as per [fluortools](http://www.fluortools.com/software/decayfit/documentation/fit)
 
 $$
 \chi^2 = \sum_{j=1}^{n} (c_j-\hat{c_j})^2/\hat{c_j}\\
 \chi^2_{red}=\frac{\chi^2}{n}
-$$
+$$
```

### Comparing `lifetimefitting-0.0.10/app/lifetimefitting/__main__.py` & `lifetimefitting-0.0.11/app/lifetimefitting/__main__.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.10/app/lifetimefitting/funcs.py` & `lifetimefitting-0.0.11/app/lifetimefitting/funcs.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.10/app/lifetimefitting/gui.py` & `lifetimefitting-0.0.11/app/lifetimefitting/gui.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.10/app/lifetimefitting/phd.py` & `lifetimefitting-0.0.11/app/lifetimefitting/phd.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.10/setup.py` & `lifetimefitting-0.0.11/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = "lifetimefitting",
-    version = "0.0.10",
+    version = "0.0.11",
     author = "Adrea Snow",
     author_email = "adrea.snow@gmail.com",
     description = "PicoHarp TCSPC lifetime fitting tool",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adreasnow/LifetimeFittingTool",
     classifiers = [
```

