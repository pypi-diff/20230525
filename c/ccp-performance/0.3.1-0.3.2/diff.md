# Comparing `tmp/ccp-performance-0.3.1.tar.gz` & `tmp/ccp-performance-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/ccp/ccp/dist/.tmp-3nffs68v/ccp-performance-0.3.1.tar", last modified: Mon May  8 16:12:37 2023, max compression
+gzip compressed data, was "/home/runner/work/ccp/ccp/dist/.tmp-gbz19118/ccp-performance-0.3.2.tar", last modified: Thu May 25 20:37:46 2023, max compression
```

## Comparing `ccp-performance-0.3.1.tar` & `ccp-performance-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/ccp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/ccp/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/ccp/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   288892 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/ccp/tests/data/UTGCA_1231_A_1s.csv
--rw-r--r--   0 runner    (1001) docker     (123)   502046 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/ccp/tests/data/lp-sec1-caso-a-eff.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/ccp/tests/data/lp-sec1-caso-a-head.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/ccp/tests/data/normal-eff.csv
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/ccp/tests/data/normal-head.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/ccp_performance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/ccp_performance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/ccp_performance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/ccp_performance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/ccp_performance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/ccp_performance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp/
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47176 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/compressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/config/fluids.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/config/new_units.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/config/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/config/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp/data_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/data_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/data_io/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/data_io/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/data_io/read_xl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/fo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39930 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/impeller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/plotly_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57872 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24461 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   288892 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/tests/data/UTGCA_1231_A_1s.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   502046 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/tests/data/lp-sec1-caso-a-eff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/tests/data/lp-sec1-caso-a-head.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/tests/data/normal-eff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/tests/data/normal-head.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp_performance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp_performance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp_performance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp_performance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp_performance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp_performance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/setup.py
```

### Comparing `ccp-performance-0.3.1/LICENSE` & `ccp-performance-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.1/PKG-INFO` & `ccp-performance-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccp-performance
-Version: 0.3.1
+Version: 0.3.2
 Summary: Centrifugal Compressor Performance calculation.
 Author: Raphael Timbó
 Author-email: raphaelts@petrobras.com.br
 License: Apache License 2.0
 Project-URL: Documentation, https://ccp-centrifugal-compressor-performance.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/petrobras/ccp/issues
 Project-URL: Source Code, https://github.com/petrobras/ccp
@@ -18,15 +18,15 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 
 # <img src="https://ccp-centrifugal-compressor-performance.readthedocs.io/en/latest/_static/ccp.png" alt="drawing" width="40"/> Centrifugal Compressor Performance
 
 [![PyPI Version](https://img.shields.io/pypi/v/ccp-performance.svg)](https://pypi.org/project/ccp-performance/)
-[![License](https://img.shields.io/pypi/l/ccp-performance.svg)](https://github.com/raphaeltimbo/ccp/blob/master/LICENSE)
+[![License](https://img.shields.io/pypi/l/ccp-performance.svg)](https://github.com/raphaeltimbo/ccp/blob/main/LICENSE)
 [![code style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ccp is a python library for calculation of centrifugal compressor performance. It uses CoolProp/REFPROP for the gas properties calculations.
 
 ```python
 import ccp
 
@@ -79,9 +79,9 @@
 # Documentation 
 Access the documentation [here](https://ccp-centrifugal-compressor-performance.readthedocs.io/en/stable/).
 
 # Questions
 If you have any questions, you can use the [Discussions](https://github.com/petrobras/ccp/discussions) area in the repository.
 
 # Contributing to ccp
-ROSS is a community-driven project. If you want to contribute to the project, please
-check [CONTRIBUTING.md](https://github.com/petrobras/ccp/blob/master/CONTRIBUTING.md). 
+ccp is a community-driven project. If you want to contribute to the project, please
+check [CONTRIBUTING.md](https://github.com/petrobras/ccp/blob/main/CONTRIBUTING.md).
```

### Comparing `ccp-performance-0.3.1/README.md` & `ccp-performance-0.3.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # <img src="https://ccp-centrifugal-compressor-performance.readthedocs.io/en/latest/_static/ccp.png" alt="drawing" width="40"/> Centrifugal Compressor Performance
 
 [![PyPI Version](https://img.shields.io/pypi/v/ccp-performance.svg)](https://pypi.org/project/ccp-performance/)
-[![License](https://img.shields.io/pypi/l/ccp-performance.svg)](https://github.com/raphaeltimbo/ccp/blob/master/LICENSE)
+[![License](https://img.shields.io/pypi/l/ccp-performance.svg)](https://github.com/raphaeltimbo/ccp/blob/main/LICENSE)
 [![code style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ccp is a python library for calculation of centrifugal compressor performance. It uses CoolProp/REFPROP for the gas properties calculations.
 
 ```python
 import ccp
 
@@ -58,9 +58,9 @@
 # Documentation 
 Access the documentation [here](https://ccp-centrifugal-compressor-performance.readthedocs.io/en/stable/).
 
 # Questions
 If you have any questions, you can use the [Discussions](https://github.com/petrobras/ccp/discussions) area in the repository.
 
 # Contributing to ccp
-ROSS is a community-driven project. If you want to contribute to the project, please
-check [CONTRIBUTING.md](https://github.com/petrobras/ccp/blob/master/CONTRIBUTING.md). 
+ccp is a community-driven project. If you want to contribute to the project, please
+check [CONTRIBUTING.md](https://github.com/petrobras/ccp/blob/main/CONTRIBUTING.md).
```

### Comparing `ccp-performance-0.3.1/ccp/tests/data/UTGCA_1231_A_1s.csv` & `ccp-performance-0.3.2/ccp/tests/data/UTGCA_1231_A_1s.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.1/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h` & `ccp-performance-0.3.2/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.1/ccp/tests/data/lp-sec1-caso-a-eff.csv` & `ccp-performance-0.3.2/ccp/tests/data/lp-sec1-caso-a-eff.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.1/ccp/tests/data/lp-sec1-caso-a-head.csv` & `ccp-performance-0.3.2/ccp/tests/data/lp-sec1-caso-a-head.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.1/ccp/tests/data/normal-eff.csv` & `ccp-performance-0.3.2/ccp/tests/data/normal-eff.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.1/ccp/tests/data/normal-head.csv` & `ccp-performance-0.3.2/ccp/tests/data/normal-head.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.1/ccp_performance.egg-info/PKG-INFO` & `ccp-performance-0.3.2/ccp_performance.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccp-performance
-Version: 0.3.1
+Version: 0.3.2
 Summary: Centrifugal Compressor Performance calculation.
 Author: Raphael Timbó
 Author-email: raphaelts@petrobras.com.br
 License: Apache License 2.0
 Project-URL: Documentation, https://ccp-centrifugal-compressor-performance.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/petrobras/ccp/issues
 Project-URL: Source Code, https://github.com/petrobras/ccp
@@ -18,15 +18,15 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 
 # <img src="https://ccp-centrifugal-compressor-performance.readthedocs.io/en/latest/_static/ccp.png" alt="drawing" width="40"/> Centrifugal Compressor Performance
 
 [![PyPI Version](https://img.shields.io/pypi/v/ccp-performance.svg)](https://pypi.org/project/ccp-performance/)
-[![License](https://img.shields.io/pypi/l/ccp-performance.svg)](https://github.com/raphaeltimbo/ccp/blob/master/LICENSE)
+[![License](https://img.shields.io/pypi/l/ccp-performance.svg)](https://github.com/raphaeltimbo/ccp/blob/main/LICENSE)
 [![code style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ccp is a python library for calculation of centrifugal compressor performance. It uses CoolProp/REFPROP for the gas properties calculations.
 
 ```python
 import ccp
 
@@ -79,9 +79,9 @@
 # Documentation 
 Access the documentation [here](https://ccp-centrifugal-compressor-performance.readthedocs.io/en/stable/).
 
 # Questions
 If you have any questions, you can use the [Discussions](https://github.com/petrobras/ccp/discussions) area in the repository.
 
 # Contributing to ccp
-ROSS is a community-driven project. If you want to contribute to the project, please
-check [CONTRIBUTING.md](https://github.com/petrobras/ccp/blob/master/CONTRIBUTING.md). 
+ccp is a community-driven project. If you want to contribute to the project, please
+check [CONTRIBUTING.md](https://github.com/petrobras/ccp/blob/main/CONTRIBUTING.md).
```

### Comparing `ccp-performance-0.3.1/setup.py` & `ccp-performance-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             "linkify-it-py",
             "sphinx-book-theme",
             "sphinx-panels",
             "sphinx-copybutton",
             "sphinx-rtd-theme",
         ],
     },
-    py_modules=[],
+    packages=find_packages(),
     license="Apache License 2.0",
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

