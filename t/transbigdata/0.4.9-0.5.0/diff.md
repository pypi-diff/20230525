# Comparing `tmp/transbigdata-0.4.9.tar.gz` & `tmp/transbigdata-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transbigdata-0.4.9.tar", last modified: Fri Jul  1 13:10:09 2022, max compression
+gzip compressed data, was "transbigdata-0.5.0.tar", last modified: Thu May 25 14:49:01 2023, max compression
```

## Comparing `transbigdata-0.4.9.tar` & `transbigdata-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:10:09.160637 transbigdata-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-07-01 13:09:56.000000 transbigdata-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-07-01 13:09:56.000000 transbigdata-0.4.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    15013 2022-07-01 13:10:09.160637 transbigdata-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14136 2022-07-01 13:09:56.000000 transbigdata-0.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-01 13:10:09.160637 transbigdata-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-07-01 13:09:57.000000 transbigdata-0.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:10:09.160637 transbigdata-0.4.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:10:09.160637 transbigdata-0.4.9/src/transbigdata/
--rw-r--r--   0 runner    (1001) docker     (121)     6040 2022-07-01 13:09:57.000000 transbigdata-0.4.9/src/transbigdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4692 2022-07-01 13:09:57.000000 transbigdata-0.4.9/src/transbigdata/bikedata.py
--rw-r--r--   0 runner    (1001) docker     (121)    12125 2022-07-01 13:09:57.000000 transbigdata-0.4.9/src/transbigdata/busgps.py
--rw-r--r--   0 runner    (1001) docker     (121)    10881 2022-07-01 13:09:57.000000 transbigdata-0.4.9/src/transbigdata/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (121)    13016 2022-07-01 13:09:57.000000 transbigdata-0.4.9/src/transbigdata/crawler.py
--rw-r--r--   0 runner    (1001) docker     (121)    10560 2022-07-01 13:09:57.000000 transbigdata-0.4.9/src/transbigdata/gisprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)    49993 2022-07-01 13:09:57.000000 transbigdata-0.4.9/src/transbigdata/grids.py
--rw-r--r--   0 runner    (1001) docker     (121)     9356 2022-07-01 13:09:57.000000 transbigdata-0.4.9/src/transbigdata/metro.py
--rw-r--r--   0 runner    (1001) docker     (121)    10675 2022-07-01 13:09:57.000000 transbigdata-0.4.9/src/transbigdata/odprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)    20024 2022-07-01 13:09:57.000000 transbigdata-0.4.9/src/transbigdata/plotmap.py
--rw-r--r--   0 runner    (1001) docker     (121)    15340 2022-07-01 13:09:57.000000 transbigdata-0.4.9/src/transbigdata/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     4296 2022-07-01 13:09:57.000000 transbigdata-0.4.9/src/transbigdata/quality.py
--rw-r--r--   0 runner    (1001) docker     (121)     6289 2022-07-01 13:09:57.000000 transbigdata-0.4.9/src/transbigdata/taxigps.py
--rw-r--r--   0 runner    (1001) docker     (121)    15482 2022-07-01 13:09:57.000000 transbigdata-0.4.9/src/transbigdata/traj.py
--rw-r--r--   0 runner    (1001) docker     (121)    25522 2022-07-01 13:09:57.000000 transbigdata-0.4.9/src/transbigdata/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 13:10:09.160637 transbigdata-0.4.9/transbigdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15013 2022-07-01 13:10:08.000000 transbigdata-0.4.9/transbigdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-07-01 13:10:09.000000 transbigdata-0.4.9/transbigdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-01 13:10:08.000000 transbigdata-0.4.9/transbigdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-07-01 13:10:08.000000 transbigdata-0.4.9/transbigdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-01 13:10:09.000000 transbigdata-0.4.9/transbigdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:01.961894 transbigdata-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-25 14:48:50.000000 transbigdata-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 14:48:50.000000 transbigdata-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-25 14:49:01.961894 transbigdata-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13991 2023-05-25 14:48:50.000000 transbigdata-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:49:01.961894 transbigdata-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-25 14:48:51.000000 transbigdata-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:01.957894 transbigdata-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:01.961894 transbigdata-0.5.0/src/transbigdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/bikedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/busgps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13711 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/gisprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49157 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/grids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/mobilephonedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/odprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/plotmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/taxigps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31808 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/traj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25655 2023-05-25 14:48:51.000000 transbigdata-0.5.0/src/transbigdata/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:01.961894 transbigdata-0.5.0/transbigdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-25 14:49:01.000000 transbigdata-0.5.0/transbigdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-25 14:49:01.000000 transbigdata-0.5.0/transbigdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:49:01.000000 transbigdata-0.5.0/transbigdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-25 14:49:01.000000 transbigdata-0.5.0/transbigdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 14:49:01.000000 transbigdata-0.5.0/transbigdata.egg-info/top_level.txt
```

### Comparing `transbigdata-0.4.9/LICENSE` & `transbigdata-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `transbigdata-0.4.9/PKG-INFO` & `transbigdata-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transbigdata
-Version: 0.4.9
+Version: 0.5.0
 Summary: A Python package developed for transportation spatio-temporal big data processing and analysis.
 Home-page: https://github.com/ni1o1/transbigdata
 Author: Qing Yu
 Author-email: qingyu0815@foxmail.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/ni1o1/transbigdata/issues
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 
 English [中文版](README-zh_CN.md)
 
 # TransBigData
 
 <img src="https://github.com/ni1o1/transbigdata/raw/main/docs/source/_static/logo-wordmark-dark.png" style="width:550px">
 
-[![Documentation Status](https://readthedocs.org/projects/transbigdata/badge/?version=latest)](https://transbigdata.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://pepy.tech/badge/transbigdata)](https://pepy.tech/project/transbigdata) [![Downloads](https://pepy.tech/badge/transbigdata/week)](https://pepy.tech/project/transbigdata) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ni1o1/transbigdata/d7d6fa33ff16440ba1698b10dd3cf3f76ff00abd?urlpath=lab%2Ftree%2Fexample%2FExample%201-Taxi%20GPS%20data%20processing.ipynb) [![Tests](https://github.com/ni1o1/transbigdata/actions/workflows/tests.yml/badge.svg)](https://github.com/ni1o1/transbigdata/actions/workflows/tests.yml) [![codecov](https://codecov.io/gh/ni1o1/transbigdata/branch/main/graph/badge.svg?token=GLAVYYCD9L)](https://codecov.io/gh/ni1o1/transbigdata)
+[![Documentation Status](https://readthedocs.org/projects/transbigdata/badge/?version=latest)](https://transbigdata.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://pepy.tech/badge/transbigdata)](https://pepy.tech/project/transbigdata) [![Downloads](https://pepy.tech/badge/transbigdata/week)](https://pepy.tech/project/transbigdata) [![Tests](https://github.com/ni1o1/transbigdata/actions/workflows/tests.yml/badge.svg)](https://github.com/ni1o1/transbigdata/actions/workflows/tests.yml) [![codecov](https://codecov.io/gh/ni1o1/transbigdata/branch/main/graph/badge.svg?token=GLAVYYCD9L)](https://codecov.io/gh/ni1o1/transbigdata)
 
 ## Introduction
 
 `TransBigData` is a Python package developed for transportation spatio-temporal big data processing, analysis and visualization. `TransBigData` provides fast and concise methods for processing common transportation spatio-temporal big data such as Taxi GPS data, bicycle sharing data and bus GPS data. `TransBigData` provides a variety of processing methods for each stage of transportation spatio-temporal big data analysis. The code with `TransBigData` is clean, efficient, flexible, and easy to use, allowing complex data tasks to be achieved with concise code.
 
 For some specific types of data, `TransBigData` also provides targeted tools for specific needs, such as extraction of Origin and Destination(OD) of taxi trips from taxi GPS data and identification of arrival and departure information from bus GPS data. The latest stable release of the software can be installed via pip and full documentation
 can be found at https://transbigdata.readthedocs.io/en/latest/. Introduction PPT can be found [here](https://github.com/ni1o1/transbigdata/blob/main/introduction/IntroductionofTransBigData.pdf) and [here(in Chinese)](https://github.com/ni1o1/transbigdata/blob/main/introduction/gridbasedframework.pdf)
@@ -57,23 +57,23 @@
 * **Data Aggregating**: Provides methods to aggregate GPS data and OD data into geographic polygon.
 * **Data Visualization**: Built-in visualization capabilities leverage the visualization package keplergl to interactively visualize data on Jupyter notebook with simple code.
 * **Trajectory Processing**: Provides methods to process trajectory data, including generating trajectory linestring from GPS points, and trajectory densification, etc.
 * **Basemap Loading**: Provides methods to display Mapbox basemap on matplotlib figures
 
 ## Installation
 
-It is recommended to use `Python 3.7, 3.8, 3.9`
+`TransBigData` support Python >= 3.6
 
 ### Using pypi [![PyPI version](https://badge.fury.io/py/transbigdata.svg)](https://badge.fury.io/py/transbigdata)
 
 `TransBigData` can be installed by using `pip install`. Before installing `TransBigData`, make sure that you have installed the available [geopandas package](https://geopandas.org/en/stable/getting_started/install.html). If you already have geopandas installed, run the following code directly from the command prompt to install `TransBigData`:
 
     pip install transbigdata
 
-### Using conda-forge [![Conda Version](https://img.shields.io/conda/vn/conda-forge/transbigdata.svg)](https://anaconda.org/conda-forge/transbigdata) [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/transbigdata.svg)](https://anaconda.org/conda-forge/transbigdata) 
+### Using conda-forge [![Conda Version](https://img.shields.io/conda/vn/conda-forge/transbigdata.svg)](https://anaconda.org/conda-forge/transbigdata) [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/transbigdata.svg)](https://anaconda.org/conda-forge/transbigdata)
 
 You can also install `TransBigData` by `conda-forge`, this will automaticaly solve the dependency, it can be installed with:
 
     conda install -c conda-forge transbigdata
 
 ## Contributing to TransBigData [![GitHub contributors](https://img.shields.io/github/contributors/ni1o1/transbigdata.svg)](https://github.com/ni1o1/transbigdata/graphs/contributors) [![Join the chat at https://gitter.im/transbigdata/community](https://badges.gitter.im/transbigdata/community.svg)](https://gitter.im/transbigdata/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ni1o1/transbigdata)
 
@@ -81,23 +81,23 @@
 
 ## Examples
 
 ### Example of data visualization
 
 #### Visualize trajectories (with keplergl)
 
-![gif](https://github.com/ni1o1/transbigdata/raw/main/images/tbdexample1.gif)
+![gif](https://github.com/ni1o1/transbigdata/raw/main/image/README/tbdexample1.gif)
 
 #### Visualize data distribution (with keplergl)
 
-![gif](https://github.com/ni1o1/transbigdata/raw/main/images/tbdexample2.gif)
+![gif](https://github.com/ni1o1/transbigdata/raw/main/image/README/tbdexample2.gif)
 
 #### Visualize OD (with keplergl)
 
-![gif](https://github.com/ni1o1/transbigdata/raw/main/images/tbdexample3.gif)
+![gif](https://github.com/ni1o1/transbigdata/raw/main/image/README/tbdexample3.gif)
 
 ### Example of taxi GPS data processing
 
 The following example shows how to use the `TransBigData` to perform data gridding, data aggregating and data visualization for taxi GPS data.
 
 #### Read the data
 
@@ -276,15 +276,15 @@
 #Change the type into GeoDataFrame
 import geopandas as gpd
 grid_agg = gpd.GeoDataFrame(grid_agg)
 #Plot the grids
 grid_agg.plot(column = 'VehicleNum',cmap = 'autumn_r')
 ```
 
-![png](https://github.com/ni1o1/transbigdata/raw/main/images/output_5_1.png)
+![png](https://github.com/ni1o1/transbigdata/raw/main/image/README/output_5_1.png)
 
 #### Triangle and Hexagon grids & rotation angle
 
 `TransBigData` also support the triangle and hexagon grids. It also supports given rotation angle for the grids. We can alter the gridding parameter:
 
 ```python
 #set to the hexagon grids
@@ -341,15 +341,15 @@
 
 #### Griding framework offered by TransBigData
 
 Here is an overview of the gridding framework offered by `TransBigData`.
 
 ![1648715064154.png](https://github.com/ni1o1/transbigdata/raw/main/image/README/1648715064154.png)
 
-See [This Example](https://github.com/ni1o1/transbigdata/blob/main/example/TBD_Core_Functions.ipynb) for further details.
+See [This Example](https://github.com/ni1o1/transbigdata/blob/main/docs/source/gallery/Example%202-Grid-base%20processing%20framework%20of%20TransBigData.ipynb) for further details.
 
 ## Citation information [![DOI](https://zenodo.org/badge/419559811.svg)](https://zenodo.org/badge/latestdoi/419559811) [![status](https://joss.theoj.org/papers/d1055fe3105dfa2dcff4cb6c7688a79b/status.svg)](https://joss.theoj.org/papers/d1055fe3105dfa2dcff4cb6c7688a79b)
 
 Please cite [this](https://doi.org/10.21105/joss.04021) when using `TransBigData` in your research. Citation information can be found at [CITATION.cff](https://github.com/ni1o1/transbigdata/blob/main/CITATION.cff).
 
 ## Introducing Video (In Chinese) [![bilibili](https://img.shields.io/badge/bilibili-%E5%90%8C%E6%B5%8E%E5%B0%8F%E6%97%AD%E5%AD%A6%E9%95%BF-green.svg)](https://space.bilibili.com/3051484)
```

### Comparing `transbigdata-0.4.9/README.md` & `transbigdata-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 English [中文版](README-zh_CN.md)
 
 # TransBigData
 
 <img src="https://github.com/ni1o1/transbigdata/raw/main/docs/source/_static/logo-wordmark-dark.png" style="width:550px">
 
-[![Documentation Status](https://readthedocs.org/projects/transbigdata/badge/?version=latest)](https://transbigdata.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://pepy.tech/badge/transbigdata)](https://pepy.tech/project/transbigdata) [![Downloads](https://pepy.tech/badge/transbigdata/week)](https://pepy.tech/project/transbigdata) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ni1o1/transbigdata/d7d6fa33ff16440ba1698b10dd3cf3f76ff00abd?urlpath=lab%2Ftree%2Fexample%2FExample%201-Taxi%20GPS%20data%20processing.ipynb) [![Tests](https://github.com/ni1o1/transbigdata/actions/workflows/tests.yml/badge.svg)](https://github.com/ni1o1/transbigdata/actions/workflows/tests.yml) [![codecov](https://codecov.io/gh/ni1o1/transbigdata/branch/main/graph/badge.svg?token=GLAVYYCD9L)](https://codecov.io/gh/ni1o1/transbigdata)
+[![Documentation Status](https://readthedocs.org/projects/transbigdata/badge/?version=latest)](https://transbigdata.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://pepy.tech/badge/transbigdata)](https://pepy.tech/project/transbigdata) [![Downloads](https://pepy.tech/badge/transbigdata/week)](https://pepy.tech/project/transbigdata) [![Tests](https://github.com/ni1o1/transbigdata/actions/workflows/tests.yml/badge.svg)](https://github.com/ni1o1/transbigdata/actions/workflows/tests.yml) [![codecov](https://codecov.io/gh/ni1o1/transbigdata/branch/main/graph/badge.svg?token=GLAVYYCD9L)](https://codecov.io/gh/ni1o1/transbigdata)
 
 ## Introduction
 
 `TransBigData` is a Python package developed for transportation spatio-temporal big data processing, analysis and visualization. `TransBigData` provides fast and concise methods for processing common transportation spatio-temporal big data such as Taxi GPS data, bicycle sharing data and bus GPS data. `TransBigData` provides a variety of processing methods for each stage of transportation spatio-temporal big data analysis. The code with `TransBigData` is clean, efficient, flexible, and easy to use, allowing complex data tasks to be achieved with concise code.
 
 For some specific types of data, `TransBigData` also provides targeted tools for specific needs, such as extraction of Origin and Destination(OD) of taxi trips from taxi GPS data and identification of arrival and departure information from bus GPS data. The latest stable release of the software can be installed via pip and full documentation
 can be found at https://transbigdata.readthedocs.io/en/latest/. Introduction PPT can be found [here](https://github.com/ni1o1/transbigdata/blob/main/introduction/IntroductionofTransBigData.pdf) and [here(in Chinese)](https://github.com/ni1o1/transbigdata/blob/main/introduction/gridbasedframework.pdf)
@@ -35,23 +35,23 @@
 * **Data Aggregating**: Provides methods to aggregate GPS data and OD data into geographic polygon.
 * **Data Visualization**: Built-in visualization capabilities leverage the visualization package keplergl to interactively visualize data on Jupyter notebook with simple code.
 * **Trajectory Processing**: Provides methods to process trajectory data, including generating trajectory linestring from GPS points, and trajectory densification, etc.
 * **Basemap Loading**: Provides methods to display Mapbox basemap on matplotlib figures
 
 ## Installation
 
-It is recommended to use `Python 3.7, 3.8, 3.9`
+`TransBigData` support Python >= 3.6
 
 ### Using pypi [![PyPI version](https://badge.fury.io/py/transbigdata.svg)](https://badge.fury.io/py/transbigdata)
 
 `TransBigData` can be installed by using `pip install`. Before installing `TransBigData`, make sure that you have installed the available [geopandas package](https://geopandas.org/en/stable/getting_started/install.html). If you already have geopandas installed, run the following code directly from the command prompt to install `TransBigData`:
 
     pip install transbigdata
 
-### Using conda-forge [![Conda Version](https://img.shields.io/conda/vn/conda-forge/transbigdata.svg)](https://anaconda.org/conda-forge/transbigdata) [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/transbigdata.svg)](https://anaconda.org/conda-forge/transbigdata) 
+### Using conda-forge [![Conda Version](https://img.shields.io/conda/vn/conda-forge/transbigdata.svg)](https://anaconda.org/conda-forge/transbigdata) [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/transbigdata.svg)](https://anaconda.org/conda-forge/transbigdata)
 
 You can also install `TransBigData` by `conda-forge`, this will automaticaly solve the dependency, it can be installed with:
 
     conda install -c conda-forge transbigdata
 
 ## Contributing to TransBigData [![GitHub contributors](https://img.shields.io/github/contributors/ni1o1/transbigdata.svg)](https://github.com/ni1o1/transbigdata/graphs/contributors) [![Join the chat at https://gitter.im/transbigdata/community](https://badges.gitter.im/transbigdata/community.svg)](https://gitter.im/transbigdata/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ni1o1/transbigdata)
 
@@ -59,23 +59,23 @@
 
 ## Examples
 
 ### Example of data visualization
 
 #### Visualize trajectories (with keplergl)
 
-![gif](https://github.com/ni1o1/transbigdata/raw/main/images/tbdexample1.gif)
+![gif](https://github.com/ni1o1/transbigdata/raw/main/image/README/tbdexample1.gif)
 
 #### Visualize data distribution (with keplergl)
 
-![gif](https://github.com/ni1o1/transbigdata/raw/main/images/tbdexample2.gif)
+![gif](https://github.com/ni1o1/transbigdata/raw/main/image/README/tbdexample2.gif)
 
 #### Visualize OD (with keplergl)
 
-![gif](https://github.com/ni1o1/transbigdata/raw/main/images/tbdexample3.gif)
+![gif](https://github.com/ni1o1/transbigdata/raw/main/image/README/tbdexample3.gif)
 
 ### Example of taxi GPS data processing
 
 The following example shows how to use the `TransBigData` to perform data gridding, data aggregating and data visualization for taxi GPS data.
 
 #### Read the data
 
@@ -254,15 +254,15 @@
 #Change the type into GeoDataFrame
 import geopandas as gpd
 grid_agg = gpd.GeoDataFrame(grid_agg)
 #Plot the grids
 grid_agg.plot(column = 'VehicleNum',cmap = 'autumn_r')
 ```
 
-![png](https://github.com/ni1o1/transbigdata/raw/main/images/output_5_1.png)
+![png](https://github.com/ni1o1/transbigdata/raw/main/image/README/output_5_1.png)
 
 #### Triangle and Hexagon grids & rotation angle
 
 `TransBigData` also support the triangle and hexagon grids. It also supports given rotation angle for the grids. We can alter the gridding parameter:
 
 ```python
 #set to the hexagon grids
@@ -319,15 +319,15 @@
 
 #### Griding framework offered by TransBigData
 
 Here is an overview of the gridding framework offered by `TransBigData`.
 
 ![1648715064154.png](https://github.com/ni1o1/transbigdata/raw/main/image/README/1648715064154.png)
 
-See [This Example](https://github.com/ni1o1/transbigdata/blob/main/example/TBD_Core_Functions.ipynb) for further details.
+See [This Example](https://github.com/ni1o1/transbigdata/blob/main/docs/source/gallery/Example%202-Grid-base%20processing%20framework%20of%20TransBigData.ipynb) for further details.
 
 ## Citation information [![DOI](https://zenodo.org/badge/419559811.svg)](https://zenodo.org/badge/latestdoi/419559811) [![status](https://joss.theoj.org/papers/d1055fe3105dfa2dcff4cb6c7688a79b/status.svg)](https://joss.theoj.org/papers/d1055fe3105dfa2dcff4cb6c7688a79b)
 
 Please cite [this](https://doi.org/10.21105/joss.04021) when using `TransBigData` in your research. Citation information can be found at [CITATION.cff](https://github.com/ni1o1/transbigdata/blob/main/CITATION.cff).
 
 ## Introducing Video (In Chinese) [![bilibili](https://img.shields.io/badge/bilibili-%E5%90%8C%E6%B5%8E%E5%B0%8F%E6%97%AD%E5%AD%A6%E9%95%BF-green.svg)](https://space.bilibili.com/3051484)
```

### Comparing `transbigdata-0.4.9/setup.py` & `transbigdata-0.5.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="transbigdata",
-    version="0.4.9",
+    version="0.5.0",
     author="Qing Yu",
     author_email="qingyu0815@foxmail.com",
     description="A Python package developed for transportation spatio-temporal big data processing and analysis.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="BSD",
     url="https://github.com/ni1o1/transbigdata",
     project_urls={
         "Bug Tracker": "https://github.com/ni1o1/transbigdata/issues",
     },
     install_requires=[
-        "numpy", "pandas", "shapely", "geopandas", "scipy", "matplotlib"
+        "numpy", "pandas", "shapely", "geopandas>=0.10.2", "scipy", "matplotlib",'pykalman','osmnx'
     ],
     classifiers=[
         "Operating System :: OS Independent",
         "Topic :: Text Processing :: Indexing",
         "Topic :: Utilities",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: BSD License",
```

### Comparing `transbigdata-0.4.9/src/transbigdata/__init__.py` & `transbigdata-0.5.0/src/transbigdata/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 `TransBigData`: A Python package develop for transportation spatio-temporal big
 data processing, analysis and visualization.
 
 BSD 3-Clause License
 
-Copyright (c) 2021, Qing Yu
+Copyright (c) 2023, Qing Yu
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
@@ -29,16 +29,16 @@
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 
-__version__ = '0.4.9'
-__author__ = 'Qing Yu <qingyu0815@foxmail.com>'
+__version__ = '0.5.0'
+__author__ = 'Qing Yu <yuq@sustech.edu.cn>'
 
 # module level doc-string
 __doc__ = """
 TransBigData - A Python package develop for transportation spatio-temporal big
 data processing, analysis and visualization.
 =====================================================================
 
@@ -78,119 +78,123 @@
   - Trajectory Processing: Provides methods to process trajectory data,
   including generating trajectory linestring from GPS points, and trajectory
   densification, etc.
   - Basemap Loading: Provides methods to display Mapbox basemap on matplotlib
   figures
 """
 
-from .plotmap import (
+from transbigdata.plotmap import (
     plot_map,
     plotscale,
     set_mapboxtoken,
-    set_imgsavepath
+    set_imgsavepath,
+    read_imgsavepath,
+    read_mapboxtoken
 )
-from .coordinates import (
+from transbigdata.coordinates import (
     gcj02tobd09,
     bd09togcj02,
     wgs84togcj02,
     gcj02towgs84,
     wgs84tobd09,
     bd09towgs84,
     bd09mctobd09,
     getdistance,
     transform_shape
 )
-from .grids import (
-    # new
+from transbigdata.grids import (
     area_to_grid,
     area_to_params,
     GPS_to_grid,
     grid_to_centre,
     grid_to_polygon,
     grid_to_area,
     grid_to_params,
     grid_params_optimize,
-    # old
-    rect_grids,
-    grid_params,
-    grids_centre,
-    gridid_sjoin_shape,
-    regenerate_params,
     geohash_encode,
     geohash_decode,
-    geohash_togrid,
-    GPS_to_grids,
-    GPS_to_grids_rect,
-    GPS_to_grids_tri,
-    GPS_to_grids_hexa,
-    gridid_to_polygon,
-    gridid_to_polygon_rect,
-    gridid_to_polygon_tri,
-    gridid_to_polygon_hexa
+    geohash_togrid
 )
-from .gisprocess import (
+from transbigdata.gisprocess import (
     ckdnearest,
     ckdnearest_point,
     ckdnearest_line,
     splitline_with_length,
     merge_polygon,
-    polyon_exterior,
-    ellipse_params,
-    ellipse_plot
+    polyon_exterior
 )
-from .odprocess import (
+from transbigdata.odprocess import (
     odagg_grid,
     odagg_shape,
     tolinewitharrow
 )
-from .preprocess import (
-    clean_same,
-    clean_drift,
+from transbigdata.preprocess import (
     clean_outofbounds,
     clean_outofshape,
-    clean_traj,
     dataagg,
     id_reindex_disgap,
     id_reindex
 )
-from .bikedata import (
+from transbigdata.bikedata import (
     bikedata_to_od
 )
-from .taxigps import (
+from transbigdata.taxigps import (
     clean_taxi_status,
     taxigps_to_od,
     taxigps_traj_point
 )
-from .traj import (
-    plot_activity,
-    traj_stay_move,
+from transbigdata.mobilephonedata import (
+    mobile_stay_duration,
+    mobile_identify_home,
+    mobile_identify_work,    
+    )
+from transbigdata.traj import (
+    traj_mapmatch,
+    traj_clean_drift,
+    traj_clean_redundant,
+    traj_slice,
+    traj_smooth,
+    traj_segment,
     traj_densify,
     traj_sparsify,
+    traj_stay_move,
     points_to_traj,
+)
+
+from transbigdata.utils import (
     dumpjson
 )
-from .quality import (
+
+from transbigdata.quality import (
     sample_duration,
     data_summary
 )
-from .busgps import (
+from transbigdata.busgps import (
     busgps_arriveinfo,
     busgps_onewaytime
 )
-from .crawler import (
+from transbigdata.crawler import (
     getadmin,
     getbusdata,
     get_isochrone_amap,
     get_isochrone_mapbox,
 )
-from .metro import (
+from transbigdata.metro import (
     split_subwayline,
     metro_network,
     get_path_traveltime,
     get_shortest_path,
     get_k_shortest_paths
 )
-from .visualization import (
+from transbigdata.visualization import (
     visualization_trip,
     visualization_od,
     visualization_data
 )
+
+from transbigdata.activity import (
+    entropy,
+    entropy_rate,
+    ellipse_params,
+    ellipse_plot,
+    plot_activity
+)
```

### Comparing `transbigdata-0.4.9/src/transbigdata/bikedata.py` & `transbigdata-0.5.0/src/transbigdata/bikedata.py`

 * *Files identical despite different names*

### Comparing `transbigdata-0.4.9/src/transbigdata/busgps.py` & `transbigdata-0.5.0/src/transbigdata/busgps.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,20 @@
 
 import geopandas as gpd
 import pandas as pd
 import numpy as np
 from shapely.geometry import LineString
 import shapely
 from .preprocess import (
-    clean_same,
     clean_outofshape,
     id_reindex
 )
+from .traj import(
+    traj_clean_redundant
+)
 
 
 def busgps_arriveinfo(data, line, stop, col=[
         'VehicleId', 'GPSDateTime', 'lon', 'lat', 'stopname'],
         stopbuffer=200, mintime=300, project_epsg=2416,
         timegap=1800, method='project', projectoutput=False):
     '''
@@ -94,15 +96,15 @@
     print('Cleaning data', end='')
     line.set_crs(crs='epsg:4326', allow_override=True, inplace=True)
     line = line.to_crs(epsg=project_epsg)
     line_buffer = line.copy()
     line_buffer['geometry'] = line_buffer.buffer(200)
     line_buffer = line_buffer.to_crs(epsg=4326)
     print('.', end='')
-    data = clean_same(data, col=[VehicleId, GPSDateTime, lon, lat])
+    data = traj_clean_redundant(data, col=[VehicleId, GPSDateTime, lon, lat])
     print('.', end='')
     data = clean_outofshape(data, line_buffer, col=[lon, lat], accuracy=500)
     print('.')
     data = id_reindex(data, VehicleId, timegap=timegap,
                       timecol=GPSDateTime, suffix='')
 
     print('Position matching', end='')
@@ -179,15 +181,15 @@
                     continue
                 else:
                     if type(
                         line_intersection
                     ) == shapely.geometry.linestring.LineString:
                         arrive = [line_intersection]
                     else:
-                        arrive = list(line_intersection)
+                        arrive = list(line_intersection.geoms)
                 arrive = pd.DataFrame(arrive)
                 arrive['arrivetime'] = arrive[0].apply(
                     lambda r: r.coords[0][0])
                 arrive['leavetime'] = arrive[0].apply(
                     lambda r: r.coords[-1][0])
                 # Filtering arrival information through time threshold
                 a = arrive[['arrivetime']].copy()
@@ -215,15 +217,15 @@
     arrive_info['arrivetime'] = starttime + \
         arrive_info['arrivetime'].apply(
             lambda r: pd.Timedelta(int(r), unit='s'))
     arrive_info['leavetime'] = starttime + \
         arrive_info['leavetime'].apply(
             lambda r: pd.Timedelta(int(r), unit='s'))
     if projectoutput:
-        return arrive_info, data
+        return arrive_info, data # pragma: no cover
     else:
         return arrive_info
 
 
 def busgps_onewaytime(arrive_info, start, end,
                       col=['VehicleId', 'stopname',
                            'arrivetime', 'leavetime']):
```

### Comparing `transbigdata-0.4.9/src/transbigdata/coordinates.py` & `transbigdata-0.5.0/src/transbigdata/coordinates.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,18 @@
         [3.09191371068437e-9, 0.000008983055096812155, 0.00006995724062,
          23.10934304144901, -0.00023663490511, -0.6321817810242,
          -0.00663494467273, 0.03430082397953, -0.00466043876332, 2555164.4],
         [2.890871144776878e-9, 0.000008983055095805407, -3.068298e-8,
          7.47137025468032, -0.00000353937994, -0.02145144861037,
          -0.00001234426596, 0.00010322952773, -0.00000323890364, 826088.5]
     ]
-    y1 = y.iloc[0]
+    try:
+        y1 = y.iloc[0]
+    except Exception:
+        y1 = y
     for cD in range(len(MCBAND)):
         if y1 >= MCBAND[cD]:
             cE = MC2LL[cD]
             break
     cD = cE
     T = cD[0] + cD[1] * np.abs(x)
     cB = np.abs(y) / cD[9]
```

### Comparing `transbigdata-0.4.9/src/transbigdata/crawler.py` & `transbigdata-0.5.0/src/transbigdata/crawler.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,29 +30,30 @@
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 '''
 
 import pandas as pd
 import numpy as np
 import geopandas as gpd
 from shapely.geometry import Polygon, LineString
+import requests
 import urllib.request
-from urllib import parse
+import urllib.parse
 import urllib
 import json
 import re
 from .plotmap import read_mapboxtoken
 from .coordinates import (
     gcj02towgs84,
     bd09towgs84,
     bd09mctobd09,
     wgs84togcj02
 )
 
 
-def getadmin(keyword, ak, jscode='', subdistricts=False):
+def getadmin(keyword, ak, jscode='', subdistricts=False, timeout=20):
     '''
     Input the keyword and the Amap ak. The output is the GIS file of
     the administrative boundary (Only in China)
 
     Parameters
     -------
     keywords : str
@@ -61,26 +62,28 @@
     ak : str
         Amap accesstoken
     jscode : jscode
         Amap safty code
     subdistricts : bool
         Whether to output the information of the administrative district
         boundary
+    timeout : number
+        Timeout of data fetching
 
     Returns
     -------
     admin : GeoDataFrame
         Administrative district(WGS84)
     districts : DataFrame
         The information of subdistricts. This can be used to further get
         the boundary of lower level districts
     '''
 
     # API url
-    url = 'https://restapi.amap.com/v3/config/district?'
+    url = 'https://restapi.amap.com/v3/config/district'
     # Condition
     dict1 = {
         'subdistrict': '3',
         'showbiz': 'false',
         'extensions': 'all',
         'key': ak,
         'jscode': jscode,
@@ -88,23 +91,24 @@
         'output': 'json',
         'level': 'district',
         'keywords': keyword,
         'platform': 'JS',
         'logversion': '2.0',
         'sdkversion': '1.4.10'
     }
-    url_data = parse.urlencode(dict1)
-    url = url+url_data
-    request = urllib.request.Request(url)
-    response = urllib.request.urlopen(request)
-    webpage = response.read()
-    result = json.loads(webpage.decode('utf8', 'ignore'))
+    # 发送请求
+    response = requests.get(url,params = dict1,timeout=timeout)
+    result = json.loads(response.text)
+    if result['info'] == 'INVALID_USER_SCODE':
+        raise ValueError('缺少jscode，请将高德开放平台Key中的安全密钥以jscode参数的形式传入该方法')   # pragma: no cover
     # Organize Data
     datas = []
     k = 0
+    if result['count']=='0':
+        raise ValueError('无法搜素到该行政区划')   # pragma: no cover
     polyline = result['districts'][k]['polyline']
     polyline1 = polyline.split('|')
     res = []
     for polyline2 in polyline1:
         polyline2 = polyline2.split(';')
         p = []
         for i in polyline2:
@@ -118,91 +122,93 @@
     data1 = pd.DataFrame()
     data1['geometry'] = res
     data1 = gpd.GeoDataFrame(data1)
     poly = data1.unary_union
     data['geometry'] = [poly]
     try:
         data['citycode'] = result['districts'][k]['citycode']
-    except Exception:
-        pass
+    except Exception:   # pragma: no cover
+        pass   # pragma: no cover
     try:
         data['adcode'] = result['districts'][k]['adcode']
-    except Exception:
-        pass
+    except Exception:   # pragma: no cover
+        pass   # pragma: no cover
     try:
         data['name'] = result['districts'][k]['name']
-    except Exception:
-        pass
+    except Exception:   # pragma: no cover
+        pass   # pragma: no cover
     try:
         data['level'] = result['districts'][k]['level']
-    except Exception:
-        pass
+    except Exception:   # pragma: no cover
+        pass   # pragma: no cover
     try:
         data['center'] = result['districts'][k]['center']
-    except Exception:
-        pass
+    except Exception:   # pragma: no cover
+        pass   # pragma: no cover
     datas.append(data)
     datas = pd.concat(datas)
     admin = gpd.GeoDataFrame(datas)
     if subdistricts:
         districts = result['districts'][k]['districts']
         districts = pd.DataFrame(districts)
         return admin, districts
-    else:
-        return admin
+    else:   # pragma: no cover
+        return admin   # pragma: no cover
 
 
-def getbusdata(city, keywords, accurate=True):
+def getbusdata(city, keywords, accurate=True, timeout=20):
     '''
     Obtain the geographic information of the bus station and bus line from
     the map service (Only in China)
 
     Parameters
     -------
     city : str
         city name
     keywords : list
         Keyword, the line name
     accurate : bool
         Accurate matching
+    timeout : number
+        Timeout of data fetching
 
     Returns
     -------
     data : GeoDataFrame
         The generated bus line(WGS84)
     stop : GeoDataFrame
         The generated bus station(WGS84)
     '''
     def getlineuid(keyword, c, acc=True):
         url = 'http://map.baidu.com/?qt=s&wd=' + \
             urllib.parse.quote(keyword)+'&c='+c+'&from=webmap'
-        response1 = urllib.request.urlopen(url)
-        searchinfo = json.loads(response1.read().decode('utf8'))
+        response = requests.get(url)
+        searchinfo = json.loads(response.text)
         try:
             res = pd.DataFrame(searchinfo['content'])
             if acc:
                 res = list(res[(res['geo_type'] == 1) &
                            (res['acc_flag'] == 1)]['uid'])
                 return res
             else:
-                res = list(res[res['geo_type'] == 1]['uid'])
-                return res
-        except Exception:
-            return []
+                res = list(res[res['geo_type'] == 1]['uid'])   # pragma: no cover
+                return res   # pragma: no cover
+        except Exception:   # pragma: no cover
+            return []   # pragma: no cover
 
     def getcitycode(c):
         url = 'http://map.baidu.com/?qt=s&wd='+urllib.parse.quote(c)
-        response1 = urllib.request.urlopen(url, timeout=60)
-        searchinfo = json.loads(response1.read().decode('utf8'))
+        response1 = requests.get(url, timeout=timeout)
+        searchinfo = json.loads(response1.text)
         return str(searchinfo['content']['code'])
 
     def getlinegeo(uid, c):
         url = 'http://map.baidu.com/?qt=bsl&uid='+uid+'&c='+c+"&auth=1"
-        response = urllib.request.urlopen(url, timeout=60)
-        searchinfo = json.loads(response.read().decode('utf8'))
+        response1 = requests.get(url, timeout=timeout)
+        searchinfo = json.loads(response1.text)
         linename = searchinfo['content'][0]['name']
         stations = searchinfo['content'][0]['stations']
         geo = searchinfo['content'][0]['geo'].split('|')[2][:-1].split(',')
         stationgeo = []
         stationnames = []
         for station in stations:
             stationname = station['name']
@@ -235,15 +241,15 @@
     linenames = []
     lines = []
     c = getcitycode(city)
     print('success')
     stop = []
     uids = []
     if type(keywords) != list:
-        keywords = [str(keywords)]
+        keywords = [str(keywords)]   # pragma: no cover
     for keyword in keywords:
         print(keyword)
         for uid in getlineuid(keyword, c, accurate):
             if uid not in uids:
                 try:
                     linename, coo, stationnames, stationgeo = getlinegeo(
                         uid, c)
@@ -259,19 +265,19 @@
                     stops['lon'] = stops['geo'].apply(
                         lambda row: row.split(',')[0])
                     stops['lat'] = stops['geo'].apply(
                         lambda row: row.split(',')[1])
                     stop.append(stops)
                     print(linename+' success')
                     uids.append(uid)
-                except Exception:
-                    pass
+                except Exception:  # pragma: no cover
+                    pass  # pragma: no cover
     if len(stop) == 0:
-        print('No such busline')
-        return gpd.GeoDataFrame(), gpd.GeoDataFrame()
+        print('No such busline')   # pragma: no cover
+        return gpd.GeoDataFrame(), gpd.GeoDataFrame()   # pragma: no cover
     data = gpd.GeoDataFrame()
     data['linename'] = linenames
     data['geometry'] = lines
     data['city'] = city
     stop = pd.concat(stop)
     stop['lon'], stop['lat'] = bd09towgs84(stop['lon'], stop['lat'])
     stop['geometry'] = gpd.points_from_xy(stop['lon'], stop['lat'])
@@ -282,15 +288,15 @@
     stop['id'] = range(len(stop))
     stop['id'] = stop.groupby('linename')['id'].rank()
     data = data.drop_duplicates(subset=['linename'])
     stop = stop.drop_duplicates(subset=['linename', 'stationnames'])
     return data, stop
 
 
-def get_isochrone_amap(lon, lat, reachtime, ak, jscode='', mode=2):
+def get_isochrone_amap(lon, lat, reachtime, ak, jscode='', mode=2, timeout=20):
     '''
     Obtain the isochrone from Amap reachcricle
 
     Parameters
     -------
     lon : float
         Longitude of the start point(WGS84)
@@ -300,42 +306,41 @@
         Reachtime of the isochrone
     ak : str
         Amap access token
     jscode : jscode
         Amap safty code
     mode : int or str
         Travel mode, should be 0(bus), 1(subway), 2(bus+subway)
+    timeout : number
+        Timeout of data fetching
 
     Returns
     -------
     isochrone : GeoDataFrame
         The isochrone GeoDataFrame(WGS84)
     '''
     strategy = str(mode)
     if strategy not in ['0', '1', '2']:
-        raise ValueError(
-            'Travel mode, should be 0(bus), 1(subway), 2(bus+subway)')
+        raise ValueError(   # pragma: no cover
+            'Travel mode, should be 0(bus), 1(subway), 2(bus+subway)')   # pragma: no cover
     lon, lat = wgs84togcj02(lon, lat)
-    url = 'http://restapi.amap.com/v3/direction/reachcircle?'
+    url = 'http://restapi.amap.com/v3/direction/reachcircle'
     dict1 = {
         'key': ak,
         'jscode': jscode,
         'location': str(round(float(lon), 6))+','+str(round(float(lat), 6)),
         'time': reachtime,
         'output': 'json',
         's': 'rsv3',
         'extensions': 'all',
         'strategy': str(strategy)
     }
-    url_data = parse.urlencode(dict1)
-    url = url+url_data
-    request = urllib.request.Request(url)
-    response = urllib.request.urlopen(request, timeout=10)
-    webpage = response.read()
-    result = json.loads(webpage.decode('utf8', 'ignore'))
+    response = requests.get(url,params = dict1,timeout=timeout)
+    result = json.loads(response.text)
+    
     P_all = []
     for each in result['polylines']:
         data = each['outer']
         ll = re.split('[,;]', data)
         ll = np.reshape(ll, (int(len(ll)/2), 2))
         l2 = []
         for i in ll:
@@ -348,15 +353,15 @@
     g['lon'] = lon
     g['lat'] = lat
     g['reachtime'] = reachtime
     return g
 
 
 def get_isochrone_mapbox(lon, lat, reachtime, access_token='auto',
-                         mode='driving'):
+                         mode='driving', timeout=20):
     '''
     Obtain the isochrone from mapbox isochrone
 
     Parameters
     -------
     lon : float
         Longitude of the start point(WGS84)
@@ -364,30 +369,30 @@
         Latitude of the start point(WGS84)
     reachtime : number
         Reachtime of the isochrone
     access_token : str
         Mapbox access token, if `auto` it will use the preset access token
     mode : bool
         Travel mode, should be `driving`, `walking` or `cycling`
+    timeout : number
+        Timeout of data fetching
 
     Returns
     -------
     isochrone : GeoDataFrame
         The isochrone GeoDataFrame(WGS84)
     '''
     if access_token == 'auto':
-        access_token = read_mapboxtoken()
+        access_token = read_mapboxtoken()   # pragma: no cover
     if mode not in ['driving', 'walking', 'cycling']:
-        raise ValueError(
-            'Travel mode should be `driving`, `walking` or `cycling`')
+        raise ValueError(   # pragma: no cover
+            'Travel mode should be `driving`, `walking` or `cycling`')   # pragma: no cover
     url = 'https://api.mapbox.com/isochrone/v1/mapbox/'+mode+'/' +\
         str(lon)+','+str(lat)+'?contours_minutes='+str(reachtime) +\
         '&polygons=true&access_token='+access_token
-    request = urllib.request.Request(url)
-    response = urllib.request.urlopen(request, timeout=1)
-    webpage = response.read()
-    result = webpage.decode('utf8', 'ignore')
-    isochrone = gpd.GeoDataFrame.from_features(json.loads(result))
+    response = requests.get(url,timeout = timeout)
+    result = json.loads(response.text)
+    isochrone = gpd.GeoDataFrame.from_features(result)
     isochrone['lon'] = lon
     isochrone['lat'] = lat
     isochrone['reachtime'] = reachtime
     return isochrone[['lon', 'lat', 'reachtime', 'geometry']]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `transbigdata-0.4.9/src/transbigdata/gisprocess.py` & `transbigdata-0.5.0/src/transbigdata/gisprocess.py`

 * *Files 18% similar despite different names*

```diff
@@ -61,31 +61,31 @@
 
     Returns
     -------
     gdf : DataFrame
         The output DataFrame
     '''
     if len(dfA_origin) == 0:
-        raise Exception('The input DataFrame dfA is empty')
+        raise Exception('The input DataFrame dfA is empty')   # pragma: no cover
     if len(dfB_origin) == 0:
-        raise Exception('The input DataFrame dfB is empty')
+        raise Exception('The input DataFrame dfB is empty')   # pragma: no cover
     gdA = dfA_origin.copy()
     gdB = dfB_origin.copy()
     from scipy.spatial import cKDTree
     btree = cKDTree(gdB[Bname].values)
     dist, idx = btree.query(gdA[Aname].values, k=1)
     gdA['index'] = idx
     gdB['index'] = range(len(gdB))
     gdf = pd.merge(gdA, gdB, on='index')
     if (Aname[0] == Bname[0]) & (Aname[1] == Bname[1]):
-        gdf['dist'] = getdistance(
-            gdf[Aname[0]+'_x'],
-            gdf[Aname[1]+'_y'],
-            gdf[Bname[0]+'_x'],
-            gdf[Bname[1]+'_y'])
+        gdf['dist'] = getdistance(   # pragma: no cover
+            gdf[Aname[0]+'_x'],   # pragma: no cover
+            gdf[Aname[1]+'_y'],   # pragma: no cover
+            gdf[Bname[0]+'_x'],   # pragma: no cover
+            gdf[Bname[1]+'_y'])   # pragma: no cover
     else:
         gdf['dist'] = getdistance(
             gdf[Aname[0]],
             gdf[Aname[1]],
             gdf[Bname[0]],
             gdf[Bname[1]])
     return gdf
@@ -106,17 +106,17 @@
 
     Returns
     -------
     gdf : DataFrame
         The output DataFrame
     '''
     if len(gdA) == 0:
-        raise Exception('The input GeoDataFrame gdfA is empty')
+        raise Exception('The input GeoDataFrame gdfA is empty')   # pragma: no cover
     if len(gdB) == 0:
-        raise Exception('The input GeoDataFrame gdfB is empty')
+        raise Exception('The input GeoDataFrame gdfB is empty')   # pragma: no cover
     nA = np.array(list(gdA.geometry.apply(lambda x: (x.x, x.y))))
     nB = np.array(list(gdB.geometry.apply(lambda x: (x.x, x.y))))
     btree = cKDTree(nB)
     dist, idx = btree.query(nA, k=1)
     gdA['dist'] = dist
     gdA['index'] = idx
     gdB['index'] = range(len(gdB))
@@ -139,17 +139,17 @@
 
     Returns
     -------
     gdf : DataFrame
         Searching the nearset linestring in gdfB for the point in gdfA
     '''
     if len(gdfA) == 0:
-        raise Exception('The input GeoDataFrame gdfA is empty')
+        raise Exception('The input GeoDataFrame gdfA is empty')   # pragma: no cover
     if len(gdfB) == 0:
-        raise Exception('The input GeoDataFrame gdfB is empty')
+        raise Exception('The input GeoDataFrame gdfB is empty')   # pragma: no cover
     A = np.concatenate(
         [np.array(geom.coords) for geom in gdfA.geometry.to_list()])
     B = [np.array(geom.coords) for geom in gdfB.geometry.to_list()]
     B_ix = tuple(itertools.chain.from_iterable(
         [itertools.repeat(i, x) for i, x in enumerate(list(map(len, B)))]))
     B = np.concatenate(B)
     ckd_tree = cKDTree(B)
@@ -183,15 +183,15 @@
         routelength = route.length
         from shapely.geometry import LineString
         lss = []
         for k in range(int(routelength/maxlength)+1):
             if k == int(routelength/maxlength):
                 lm = routelength
             else:
-                lm = (k+1)*maxlength
+                lm = (k+1)*maxlength   # pragma: no cover
             a = np.linspace(k*maxlength, lm, 10)
             ls = []
             for line in a:
                 ls.append(route.interpolate(line))
             lss.append(LineString(ls))
         lss = gpd.GeoDataFrame(lss, columns=['geometry'])
         return lss
@@ -256,92 +256,22 @@
     '''
     data1 = data.copy()
 
     def polyexterior(p):
         from shapely.geometry import Polygon, MultiPolygon
         if type(p) == MultiPolygon:
             geometries = []
-            for i in p:
+            for i in p.geoms:
                 poly = Polygon(i.exterior)
                 if minarea > 0:
                     if poly.area > minarea:
                         geometries.append(poly)
                 else:
-                    geometries.append(poly)
+                    geometries.append(poly) # pragma: no cover
             return MultiPolygon(geometries)
         if type(p) == Polygon:
             return Polygon(p.exterior)
     data1['geometry'] = data1['geometry'].apply(polyexterior)
     data1 = data1[-data1['geometry'].is_empty]
     return data1
 
 
-def ellipse_params(data, col=['lon', 'lat'], confidence=95, epsg=None):
-    '''
-    confidence ellipse parameter estimation for point data
-
-    Parameters
-    -------
-    data : DataFrame
-        point data
-    confidence : number
-        confidence level: 99，95 or 90
-    epsg : number
-        If given, the original coordinates are transformed from WGS84 to
-        the given EPSG coordinate system for confidence ellipse parameter
-        estimation
-    col: List
-        Column names, [lon，lat]
-
-    Returns
-    -------
-    params: List
-        Centroid ellipse parameters[pos,width,height,theta,area,oblateness]
-        Respectively [Center point coordinates, minor axis, major axis,
-        angle, area, oblateness]
-    '''
-    lon, lat = col
-    if confidence == 99:
-        nstd = 9.210**0.5
-    if confidence == 95:
-        nstd = 5.991**0.5
-    if confidence == 90:
-        nstd = 4.605**0.5
-    points = data.copy()
-    points = gpd.GeoDataFrame(points)
-    points['geometry'] = gpd.points_from_xy(points[lon], points[lat])
-    if epsg:
-        points.crs = {'init': 'epsg:4326'}
-        points = points.to_crs(epsg=epsg)
-    point_np = np.array([points.geometry.x, points.geometry.y]).T
-    pos = point_np.mean(axis=0)
-    cov = np.cov(point_np, rowvar=False)
-    vals, vecs = np.linalg.eigh(cov)
-    theta = np.degrees(np.arctan2(*vecs[:, 0][::-1]))
-    width, height = 2 * nstd * np.sqrt(vals)
-    area = width/2*height/2*math.pi
-    oblateness = (height-width)/height
-
-    ellip_params = [pos, width, height, theta, area, oblateness]
-    return ellip_params
-
-
-def ellipse_plot(ellip_params, ax, **kwargs):
-    '''
-    Enter the parameters of the confidence ellipse and plot the confidence
-    ellipse
-
-    输入
-    -------
-    ellip_params : List
-        Centroid ellipse parameters[pos,width,height,theta,area,oblateness]
-        Respectively[Center point coordinates, minor axis, major axis, angle
-        , area, oblateness]
-
-    ax : matplotlib.axes._subplots.AxesSubplot
-        Where to plot
-    '''
-    [pos, width, height, theta, area, alpha] = ellip_params
-    from matplotlib.patches import Ellipse
-    ellip = Ellipse(xy=pos, width=width, height=height,
-                    angle=theta, linestyle='-', **kwargs)
-    ax.add_artist(ellip)
```

### Comparing `transbigdata-0.4.9/src/transbigdata/grids.py` & `transbigdata-0.5.0/src/transbigdata/grids.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,23 +76,23 @@
     if (type(location) == list) | (type(location) == tuple):
         shape = ''
         bounds = location
     elif type(location) == gpd.geodataframe.GeoDataFrame:
         shape = location
         bounds = shape.unary_union.bounds
     else:
-        raise Exception(
+        raise Exception(  # pragma: no cover
             'Location should be either bounds(List) or shape(GeoDataFrame)')
     lon1, lat1, lon2, lat2 = bounds
     if (lon1 > lon2) | (lat1 > lat2) | (abs(lat1) > 90) | (abs(lon1) > 180) | (
             abs(lat2) > 90) | (abs(lon2) > 180):
-        raise Exception(
-            'Bounds error. The input bounds should be in the order of \
-                [lon1,lat1,lon2,lat2]. (lon1,lat1) is the lower left \
-                    corner and (lon2,lat2) is the upper right corner.'
+        raise Exception(  # pragma: no cover
+            'Bounds error. The input bounds should be in the order '
+            'of [lon1,lat1,lon2,lat2]. (lon1,lat1) is the lower left '
+            'corner and (lon2,lat2) is the upper right corner.'
         )
     latStart = min(lat1, lat2)
     lonStart = min(lon1, lon2)
     deltaLon = accuracy * 360 / \
         (2 * math.pi * 6371004 * math.cos((lat1 + lat2) * math.pi / 360))
     deltaLat = accuracy * 360 / (2 * math.pi * 6371004)
     if params == 'auto':
@@ -187,18 +187,18 @@
         bounds = location
     elif type(location) == gpd.geodataframe.GeoDataFrame:
         shape = location
         bounds = shape.unary_union.bounds
     lon1, lat1, lon2, lat2 = bounds
     if (lon1 > lon2) | (lat1 > lat2) | (abs(lat1) > 90) | (abs(lon1) > 180) | (
             abs(lat2) > 90) | (abs(lon2) > 180):
-        raise Exception(
-            'Bounds error. The input bounds should be in the order \
-                of [lon1,lat1,lon2,lat2]. (lon1,lat1) is the lower left \
-                    corner and (lon2,lat2) is the upper right corner.'
+        raise Exception(   # pragma: no cover
+            'Bounds error. The input bounds should be in the order '
+            'of [lon1,lat1,lon2,lat2]. (lon1,lat1) is the lower left '
+            'corner and (lon2,lat2) is the upper right corner.'
         )
     latStart = min(lat1, lat2)
     lonStart = min(lon1, lon2)
     deltaLon = accuracy * 360 / \
         (2 * math.pi * 6371004 * math.cos((lat1 + lat2) * math.pi / 360))
     deltaLat = accuracy * 360 / (2 * math.pi * 6371004)
     params = [lonStart, latStart, deltaLon, deltaLat]
@@ -327,15 +327,15 @@
         y3 = pd.Series(y3)
         y4 = pd.Series(y4)
 
         def intersection(x1, y1, x2, y2, x3, y3, x4, y4):
             if np.allclose((x2[0]-x1[0]), 0):
                 return x1, (x1-x3)*(y3-y4)/(x3-x4)+y3
             elif np.allclose((x3[0]-x4[0]), 0):
-                return x3, (x3-x1)*(y1-y2)/(x1-x2)+y1
+                return x3, (x3-x1)*(y1-y2)/(x1-x2)+y1   # pragma: no cover
             x = (x1*(y2-y1)/(x2-x1)-x3/(x4-x3)*(y4-y3)+y3-y1) / \
                 ((y2-y1)/(x2-x1)-(y4-y3)/(x4-x3))
             y = (x-x1)*(y2-y1)/(x2-x1)+y1
             return x, y
         hblon, hblat = intersection(x1, y1, x2, y2, x3, y3, x4, y4)
         return hblon.values, hblat.values
 
@@ -469,16 +469,16 @@
                          col=['uid', 'lon', 'lat'],
                          optmethod='centerdist',
                          printlog=False,
                          sample=0,
                          pop=15,
                          max_iter=50,
                          w=0.1,
-                        c1=0.5,
-                        c2=0.5):
+                         c1=0.5,
+                         c2=0.5):
     '''
     Optimize the grid params
 
     Parameters
     -------
     data : DataFrame
         Trajectory data
@@ -510,16 +510,16 @@
 
     params = convertparams(params)
     method = params['method']
 
     [uid, lon, lat] = col
     try:
         from sko.PSO import PSO
-    except ImportError:
-        raise ImportError(
+    except ImportError:  # pragma: no cover
+        raise ImportError(  # pragma: no cover
             "Please install scikit-opt, run following code "
             "in cmd: pip install scikit-opt")
 
     def grids_index_gini(gpsdata, params, col=['longitude', 'latitude']):
         [lon, lat] = col
         data = gpsdata.copy()
         if params['method'] == 'rect':
@@ -622,26 +622,27 @@
                 'method': params['method'],
                 'theta': x[2] / theta_lambda,
             },
                 col=[uid, lon, lat])
 
         f = f_gridscount
     else:
-        raise Exception('Method should be one of: centerdist,gini,gridscount')
+        raise Exception(
+            'Method should be one of: centerdist,gini,gridscount')  # pragma: no cover
 
     pso = PSO(func=f,
-            n_dim=3,
-            pop=pop, 
-            max_iter=max_iter,
-            lb=[0, 0, 0],
-            ub=[params['deltalon'] * times, params['deltalat']
-                * times, 90 * theta_lambda],
-            w=w, 
-            c1=c1, 
-            c2=c2)
+              n_dim=3,
+              pop=pop,
+              max_iter=max_iter,
+              lb=[0, 0, 0],
+              ub=[params['deltalon'] * times, params['deltalat']
+                  * times, 90 * theta_lambda],
+              w=w,
+              c1=c1,
+              c2=c2)
     result = pso.run()
 
     x = result[0]
     params_optimized = {
         'slon': params['slon'] + x[0] / times,
         'slat': params['slat'] + x[1] / times,
         'deltalon': params['deltalon'],
@@ -745,15 +746,15 @@
     loncol = pd.Series(loncol)
     latcol = pd.Series(latcol)
     costheta = np.cos(theta * np.pi / 180)
     sintheta = np.sin(theta * np.pi / 180)
     R = np.array([[costheta * deltaLon, -sintheta * deltaLat],
                   [sintheta * deltaLon, costheta * deltaLat]])
     if from_origin:
-        hblonhblat = np.dot(np.array([loncol.values, latcol.values]).T,
+        hblonhblat = np.dot(np.array([loncol.values, latcol.values]).T,   # pragma: no cover
                             R) + np.array([lonStart, latStart]) - (
                                 R[0, :] / 2 + R[1, :] / 2)
     else:
         hblonhblat = np.dot(np.array([loncol.values, latcol.values]).T,
                             R) + np.array([lonStart, latStart])
     hblon = hblonhblat[:, 0]
     hblat = hblonhblat[:, 1]
@@ -1065,15 +1066,15 @@
     y5 = pd.Series(y5)
     y6 = pd.Series(y6)
 
     def intersection(x1, y1, x2, y2, x3, y3, x4, y4):
         if np.allclose((x2[0]-x1[0]), 0):
             return x1, (x1-x3)*(y3-y4)/(x3-x4)+y3
         elif np.allclose((x3[0]-x4[0]), 0):
-            return x3, (x3-x1)*(y1-y2)/(x1-x2)+y1
+            return x3, (x3-x1)*(y1-y2)/(x1-x2)+y1   # pragma: no cover
         x = (x1*(y2-y1)/(x2-x1)-x3/(x4-x3)*(y4-y3)+y3-y1) / \
             ((y2-y1)/(x2-x1)-(y4-y3)/(x4-x3))
         y = (x-x1)*(y2-y1)/(x2-x1)+y1
         return x, y
 
     testpoint = pd.DataFrame()
     testpoint['p1_x'], testpoint['p1_y'] = intersection(
@@ -1185,74 +1186,34 @@
         if len(params) == 4:
             lonStart, latStart, deltaLon, deltaLat = params
             theta = 0
             method = 'rect'
         elif len(params) == 5:
             lonStart, latStart, deltaLon, deltaLat, theta = params
             method = 'rect'
-        elif len(params) == 6:
-            lonStart, latStart, deltaLon, deltaLat, theta, method = params
+        elif len(params) == 6:  # pragma: no cover
+            lonStart, latStart, deltaLon, deltaLat, theta, method = params  # pragma: no cover
         dicparams = dict()
         dicparams['slon'] = lonStart
         dicparams['slat'] = latStart
         dicparams['deltalon'] = deltaLon
         dicparams['deltalat'] = deltaLat
         dicparams['theta'] = theta
         dicparams['method'] = method
     else:
         dicparams = params
         if 'theta' not in dicparams:
-            dicparams['theta'] = 0
+            dicparams['theta'] = 0  # pragma: no cover
         if 'method' not in dicparams:
-            dicparams['method'] = 'rect'
+            dicparams['method'] = 'rect'  # pragma: no cover
     if dicparams['method'] not in ['rect', 'tri', 'hexa']:
-        raise ValueError('Method should be `rect`,`tri` or `hexa`')
+        raise ValueError(
+            'Method should be `rect`,`tri` or `hexa`')  # pragma: no cover
     return dicparams
 
-
-'''
-Old namespace
-'''
-
-
-def regenerate_params(*args, **kwargs):
-    warnings.warn("This method is renamed as transbigdata.grid_to_params")
-    return grid_to_params(*args, **kwargs)
-
-
-def grid_params(*args, **kwargs):
-    warnings.warn("This method is renamed as transbigdata.area_to_params")
-    return area_to_params(*args, **kwargs)
-
-
-def GPS_to_grids(*args, **kwargs):
-    warnings.warn("This method is renamed as transbigdata.GPS_to_grid")
-    return GPS_to_grid(*args, **kwargs)
-
-
-def rect_grids(*args, **kwargs):
-    warnings.warn("This method is renamed as transbigdata.area_to_grid")
-    return area_to_grid(*args, **kwargs)
-
-
-def gridid_sjoin_shape(*args, **kwargs):
-    warnings.warn("This method is renamed as transbigdata.grid_to_area")
-    return grid_to_area(*args, **kwargs)
-
-
-def grids_centre(loncol, latcol, params):
-    warnings.warn("This method is renamed as transbigdata.grid_to_centre")
-    return grid_to_centre([loncol, latcol], params)
-
-
-def gridid_to_polygon(loncol, latcol, params):
-    warnings.warn("This method is renamed as transbigdata.grid_to_polygon")
-    return grid_to_polygon([loncol, latcol], params)
-
-
 '''
 Geohash
 '''
 
 __base32 = '0123456789bcdefghjkmnpqrstuvwxyz'
 __decodemap = {}
 for i in range(len(__base32)):
```

### Comparing `transbigdata-0.4.9/src/transbigdata/metro.py` & `transbigdata-0.5.0/src/transbigdata/metro.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,17 +53,17 @@
         Generated section line shape
     '''
     def getline(r2, line_geometry):
         ls = []
         if r2['o_project'] <= r2['d_project']:
             tmp1 = np.linspace(r2['o_project'], r2['d_project'], 10)
         if r2['o_project'] > r2['d_project']:
-            tmp1 = np.linspace(
+            tmp1 = np.linspace( # pragma: no cover
                 r2['o_project']-line_geometry.length, r2['d_project'], 10)
-            tmp1[tmp1 < 0] = tmp1[tmp1 < 0]+line_geometry.length
+            tmp1[tmp1 < 0] = tmp1[tmp1 < 0]+line_geometry.length # pragma: no cover
         for j in tmp1:
             ls.append(line_geometry.interpolate(j))
         return LineString(ls)
     lss = []
     for k in range(len(line)):
         r = line.iloc[k]
         line_geometry = r['geometry']
@@ -126,15 +126,15 @@
         Network edge for transfering.
     node : List
         Network nodes.
     '''
     # Obtain edge1: Network edge for line section.
     linestop = stop.copy()
     if ('speed' not in line.columns) | ('stoptime' not in line.columns):
-        raise ValueError(
+        raise ValueError( # pragma: no cover
             'Lines should have `line` column to store line name,'
             '`speed` column to store metro speed and'
             '`stoptime` column to store stop time at each station'
         )
     for i in linestop.columns:
         linestop[i+'1'] = linestop[i].shift(-1)
     linestop = linestop[linestop['linename'] == linestop['linename1']].copy()
@@ -171,24 +171,24 @@
     tmp = tmp[['stationnames', 'line', 'station']].drop_duplicates()
     tmp = pd.merge(tmp, tmp, on='stationnames')
 
     edge2 = tmp[tmp['line_x'] != tmp['line_y']][['station_x', 'station_y']]
     # All transfer time are set as the same, export `edge2` for further degign
     edge2['duration'] = transfertime
     edge2.columns = edge1.columns
-    edge = edge1.append(edge2)
+    edge = pd.concat([edge1,edge2])
     node = list(edge['ostation'].drop_duplicates())
     if nxgraph:
         import networkx as nx
         G = nx.Graph()
         G.add_nodes_from(node)
         G.add_weighted_edges_from(edge.values)
         return G
     else:
-        return edge1, edge2, node
+        return edge1, edge2, node # pragma: no cover
 
 
 def get_shortest_path(G, stop, ostation, dstation):
     '''
     Obtain the travel path of shortest path from the metro nextwork
 
     Parameters
@@ -212,15 +212,14 @@
     import networkx as nx
     o = stop[stop['stationnames'] == ostation]['line'].iloc[0]+ostation
     d = stop[stop['stationnames'] == dstation]['line'].iloc[0]+dstation
     return nx.shortest_path(G, source=o, target=d, weight='weight')
 
 
 def get_k_shortest_paths(G, stop, ostation, dstation, k):
-    from itertools import islice
     '''
     Obtain the k th shortest paths from the metro nextwork
 
     Parameters
     -------
 
     G : networkx.classes.graph.Graph
@@ -236,14 +235,15 @@
 
 
     Returns
     -------
     paths : list
         travel path: list of travel paths
     '''
+    from itertools import islice
     import networkx as nx
     o = stop[stop['stationnames'] == ostation]['line'].iloc[0]+ostation
     d = stop[stop['stationnames'] == dstation]['line'].iloc[0]+dstation
     return list(
         islice(nx.shortest_simple_paths(G, o, d, weight='weight'), k)
     )
```

### Comparing `transbigdata-0.4.9/src/transbigdata/odprocess.py` & `transbigdata-0.5.0/src/transbigdata/odprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,18 +61,18 @@
 
     Returns
     -------
     oddata1 : GeoDataFrame
         GeoDataFrame of OD after aggregation
     '''
     if len(col) == 4:
-        [slon, slat, elon, elat] = col
+        [slon, slat, elon, elat] = col  # pragma: no cover
         count = 'count'
     if len(col) == 5:
-        [slon, slat, elon, elat, count] = col
+        [slon, slat, elon, elat, count] = col  # pragma: no cover
     oddata['SLONCOL'], oddata['SLATCOL'] = GPS_to_grid(
         oddata[slon], oddata[slat], params)
     oddata['ELONCOL'], oddata['ELATCOL'] = GPS_to_grid(
         oddata[elon], oddata[elat], params)
     if len(col) == 4:
         oddata[count] = 1
     oddata_agg = oddata.groupby(['SLONCOL', 'SLATCOL', 'ELONCOL', 'ELATCOL'])[
@@ -132,15 +132,15 @@
     oddata1 : GeoDataFrame
         GeoDataFrame of OD after aggregation
     '''
     if len(col) == 4:
         [slon, slat, elon, elat] = col
         count = 'count'
     if len(col) == 5:
-        [slon, slat, elon, elat, count] = col
+        [slon, slat, elon, elat, count] = col  # pragma: no cover
     shape_1 = shape.copy()
     shape['x'] = shape.centroid.x
     shape['y'] = shape.centroid.y
     shape = shape[['x', 'y', 'geometry']]
     if params:
         oddata['SLONCOL'], oddata['SLATCOL'] = GPS_to_grid(
             oddata[slon], oddata[slat], params)
@@ -194,16 +194,16 @@
         if len(col) == 4:
             oddata[count] = 1
         oddata_agg = oddata.groupby([
             'sindex', 'sx', 'sy', 'eindex', 'ex', 'ey'])[
             count].sum().reset_index()
     from shapely.geometry import LineString
     if arrow:
-        oddata_agg['geometry'] = oddata_agg.apply(lambda r: tolinewitharrow(
-            r['sx'], r['sy'], r['ex'], r['ey'], **kwargs), axis=1)
+        oddata_agg['geometry'] = oddata_agg.apply(lambda r: tolinewitharrow(  # pragma: no cover
+            r['sx'], r['sy'], r['ex'], r['ey'], **kwargs), axis=1)  # pragma: no cover
     else:
         oddata_agg['geometry'] = oddata_agg.apply(lambda r: LineString(
             [[r['sx'], r['sy']], [r['ex'], r['ey']]]), axis=1)
     oddata_agg = gpd.GeoDataFrame(oddata_agg)
     oddata_agg = oddata_agg[['sindex', 'eindex', count, 'geometry']]
     oddata_agg = pd.merge(oddata_agg, shape_1.reset_index().rename(
         columns={'index': 'sindex'}).drop('geometry', axis=1), on='sindex')
```

### Comparing `transbigdata-0.4.9/src/transbigdata/plotmap.py` & `transbigdata-0.5.0/src/transbigdata/plotmap.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,103 +28,94 @@
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 '''
 
 import numpy as np
 import math
-import urllib
 import io
 from PIL import Image
 import os
-import sys
 import warnings
-
-
-def searchfile(filename):
-    '''
-    Search for mapboxtoken file
-    '''
-    fileroot = ''
-    for i in sys.path:
-        try:
-            if filename in os.listdir(i):
-                fileroot = i
-        except Exception:
-            pass
-    if fileroot == '':
-        fileroot = sys.path[-1]
-    return fileroot+'/'+filename
+from configparser import ConfigParser
 
 
 def set_mapboxtoken(mapboxtoken):
-    '''
-    Set mapboxtoken
-
-    Parameters
-    -------
-    mapboxtoken : str
-        mapboxtoken
-    '''
-    filepath = searchfile('mapboxtoken.txt')
-    f = open(filepath, mode='w')
-    f.write(mapboxtoken)
-    f.close()
-    print('Success')
+    config_path = os.path.join(os.path.dirname(
+        os.path.abspath(__file__)), 'config.ini')
+    config = ConfigParser()
+    config.read(config_path)
+    if not config.has_section('MAPBOX'):
+        config.add_section('MAPBOX')   # pragma: no cover
+
+    config.set('MAPBOX', 'mapboxtoken', mapboxtoken)
+    with open(config_path, 'w') as configfile:
+        config.write(configfile)
+        print('Set mapboxtoken success')
 
 
 def read_mapboxtoken():
     '''
     Read mapboxtoken
     '''
-    filepath = searchfile('mapboxtoken.txt')
     try:
-        f = open(filepath, mode='r')
-        mapboxtoken = f.readline()
-        f.close()
-    except Exception:
-        warnings.warn("Mapboxtoken not found, "
+        config_path = os.path.join(os.path.dirname(
+            os.path.abspath(__file__)), 'config.ini')
+        config = ConfigParser()
+        config.read(config_path)
+        mapboxtoken = config['MAPBOX']['mapboxtoken']
+    except Exception:  # pragma: no cover
+        warnings.warn("Mapboxtoken not found, "   # pragma: no cover
                       "The basemap is set as OpenStreetMap"
                       "please use tbd.set_mapboxtoken() to set the access token, see: "
                       "https://transbigdata.readthedocs.io/en/latest/plot_map.html"
                       )
-        mapboxtoken = ''
+        mapboxtoken = ''  # pragma: no cover
     return mapboxtoken
 
 
 def set_imgsavepath(imgsavepath):
     '''
     Set savepath for maps
 
     Parameters
     -------
     imgsavepath : str
         savepath
     '''
-    filepath = searchfile('imgsavepath.txt')
-    f = open(filepath, mode='w')
-    f.write(imgsavepath)
-    f.close()
-    print('Success')
+    if not os.path.exists(imgsavepath):
+        raise ValueError('Path do not exist')  # pragma: no cover
+    config_path = os.path.join(os.path.dirname(
+        os.path.abspath(__file__)), 'config.ini')
+    config = ConfigParser()
+    config.read(config_path)
+    if not config.has_section('MAPBOX'):
+        config.add_section('MAPBOX')   # pragma: no cover
+
+    config.set('MAPBOX', 'imgsavepath', imgsavepath)
+    with open(config_path, 'w') as configfile:
+        config.write(configfile)
+        print('Set imgsavepath success')
 
 
 def read_imgsavepath():
     '''
     Read map savepath
     '''
-    filepath = searchfile('imgsavepath.txt')
     try:
-        f = open(filepath, mode='r')
-        imgsavepath = f.readline()
-        f.close()
-    except:
+        config_path = os.path.join(os.path.dirname(
+            os.path.abspath(__file__)), 'config.ini')
+        config = ConfigParser()
+        config.read(config_path)
+        imgsavepath = config['MAPBOX']['imgsavepath']
+    except Exception:  # pragma: no cover
         warnings.warn('Map base map storage path not found, \
         please use tbd.set_imgsavepath() to set it first, \
-        see: https://transbigdata.readthedocs.io/en/latest/plot_map.html')
-        imgsavepath=''
+        see: https://transbigdata.readthedocs.io/en/latest/plot_map.html')  # pragma: no cover
+        imgsavepath = ''  # pragma: no cover
     return imgsavepath
 
 
 def deg2num(lat_deg, lon_deg, zoom):
     '''
     Calculate xy tiles from coordinates
 
@@ -168,140 +159,160 @@
 def getImageCluster(lon_deg, lat_deg, delta_long, delta_lat, zoom,
                     printlog, imgsavepath, style=4, access_token=''):
     '''
     Get map image
     '''
     smurl = ''
     if (style == 1) | (style == 'streets'):
-        styleid = 'ckwinzgw581od14mpyfhka6nk'
+        styleid = 'ckwinzgw581od14mpyfhka6nk'  # pragma: no cover
         smurl = r'https://api.mapbox.com/styles/v1/ni1o1/'+styleid + \
-            r'/tiles/256/{0}/{1}/{2}?&access_token='+access_token
+            r'/tiles/256/{0}/{1}/{2}?&access_token=' + \
+                access_token  # pragma: no cover
     if (style == 2) | (style == 'outdoors'):
-        styleid = 'ckwinx7aj4y4a15p7ftfwq9dn'
+        styleid = 'ckwinx7aj4y4a15p7ftfwq9dn'  # pragma: no cover
         smurl = r'https://api.mapbox.com/styles/v1/ni1o1/'+styleid + \
-            r'/tiles/256/{0}/{1}/{2}?&access_token='+access_token
+            r'/tiles/256/{0}/{1}/{2}?&access_token=' + \
+                access_token  # pragma: no cover
     if (style == 3) | (style == 'satellite'):
-        styleid = 'cjv36cj9u4h1q1ftemjed4f2y'
+        styleid = 'cjv36cj9u4h1q1ftemjed4f2y'  # pragma: no cover
         smurl = r'https://api.mapbox.com/styles/v1/ni1o1/'+styleid + \
-            r'/tiles/256/{0}/{1}/{2}?&access_token='+access_token
+            r'/tiles/256/{0}/{1}/{2}?&access_token=' + \
+                access_token  # pragma: no cover
     if (style == 4) | (style == 'light'):
-        styleid = 'ckwfx658z4dpb14ocnz6tky9d'
+        styleid = 'ckwfx658z4dpb14ocnz6tky9d'  # pragma: no cover
         smurl = r'https://api.mapbox.com/styles/v1/ni1o1/'+styleid + \
-            r'/tiles/256/{0}/{1}/{2}?&access_token='+access_token
+            r'/tiles/256/{0}/{1}/{2}?&access_token=' + \
+                access_token  # pragma: no cover
     if (style == 5) | (style == 'dark'):
-        styleid = 'cjetnd20i1vbi2qqxbh0by7p8'
+        styleid = 'cjetnd20i1vbi2qqxbh0by7p8'  # pragma: no cover
         smurl = r'https://api.mapbox.com/styles/v1/ni1o1/'+styleid + \
-            r'/tiles/256/{0}/{1}/{2}?&access_token='+access_token
+            r'/tiles/256/{0}/{1}/{2}?&access_token=' + \
+                access_token  # pragma: no cover
     if (style == 6) | (style == 'light-ch'):
-        styleid = 'ckj9bhq7s9mvj19mq3e3fye35'
+        styleid = 'ckj9bhq7s9mvj19mq3e3fye35'  # pragma: no cover
         smurl = r'https://api.mapbox.com/styles/v1/ni1o1/'+styleid + \
-            r'/tiles/256/{0}/{1}/{2}?&access_token='+access_token
+            r'/tiles/256/{0}/{1}/{2}?&access_token=' + \
+                access_token  # pragma: no cover
     if (style == 7) | (style == 'ice creem'):
-        styleid = 'cjv36iiz9243t1fo8mweb4z6r'
+        styleid = 'cjv36iiz9243t1fo8mweb4z6r'  # pragma: no cover
         smurl = r'https://api.mapbox.com/styles/v1/ni1o1/'+styleid + \
-            r'/tiles/256/{0}/{1}/{2}?&access_token='+access_token
+            r'/tiles/256/{0}/{1}/{2}?&access_token=' + \
+                access_token  # pragma: no cover
     if (style == 8) | (style == 'night'):
-        styleid = 'ck2o3fyvy0dch1cp6j2pkz2dv'
+        styleid = 'ck2o3fyvy0dch1cp6j2pkz2dv'  # pragma: no cover
         smurl = r'https://api.mapbox.com/styles/v1/ni1o1/'+styleid + \
-            r'/tiles/256/{0}/{1}/{2}?&access_token='+access_token
+            r'/tiles/256/{0}/{1}/{2}?&access_token=' + \
+                access_token  # pragma: no cover
     if (style == 9) | (style == 'terrain'):
-        styleid = 'cjv36gyklf43q1fnuwibiuetl'
+        styleid = 'cjv36gyklf43q1fnuwibiuetl'  # pragma: no cover
         smurl = r'https://api.mapbox.com/styles/v1/ni1o1/'+styleid + \
-            r'/tiles/256/{0}/{1}/{2}?&access_token='+access_token
+            r'/tiles/256/{0}/{1}/{2}?&access_token=' + \
+                access_token  # pragma: no cover
     if (style == 10) | (style == 'basic blue'):
-        styleid = 'ckwio2ze12fgk15p2alr5a4xj'
+        styleid = 'ckwio2ze12fgk15p2alr5a4xj'  # pragma: no cover
         smurl = r'https://api.mapbox.com/styles/v1/ni1o1/'+styleid + \
-            r'/tiles/256/{0}/{1}/{2}?&access_token='+access_token
-    if (style == 11) :
-        styleid = 'cl39hgul1000514llp3yj7yh3'
+            r'/tiles/256/{0}/{1}/{2}?&access_token=' + \
+                access_token  # pragma: no cover
+    if (style == 11):
+        styleid = 'cl39hgul1000514llp3yj7yh3'  # pragma: no cover
+        smurl = r'https://api.mapbox.com/styles/v1/ni1o1/'+styleid + \
+            r'/tiles/256/{0}/{1}/{2}?&access_token=' + \
+                access_token  # pragma: no cover
+    if (style == 12):
+        styleid = 'cl38pljx0006r14qp7ioy7gcc'  # pragma: no cover
         smurl = r'https://api.mapbox.com/styles/v1/ni1o1/'+styleid + \
-            r'/tiles/256/{0}/{1}/{2}?&access_token='+access_token
-    if (style == 12) :
-        styleid = 'cl38pljx0006r14qp7ioy7gcc'
-        smurl = r'https://api.mapbox.com/styles/v1/ni1o1/'+styleid + \
-            r'/tiles/256/{0}/{1}/{2}?&access_token='+access_token
+            r'/tiles/256/{0}/{1}/{2}?&access_token=' + \
+                access_token  # pragma: no cover
     if (style == 0) | (style == 'OSM'):
-        styleid = 'osm'
-        smurl = r'https://tile.openstreetmap.org/{0}/{1}/{2}.png'
+        styleid = 'osm'  # pragma: no cover
+        smurl = r'https://tile.openstreetmap.org/{0}/{1}/{2}.png'  # pragma: no cover
     if (str(style)[:16] == 'mapbox://styles/'):
-        styleid = style.split('/')[-1]
+        styleid = style.split('/')[-1]  # pragma: no cover
         smurl = r'https://api.mapbox.com/styles/v1/'+style[16:] + \
-            r'/tiles/256/{0}/{1}/{2}?&access_token='+access_token
+            r'/tiles/256/{0}/{1}/{2}?&access_token=' + \
+                access_token  # pragma: no cover
     if smurl == '':
-        raise ValueError('Style error')
+        raise ValueError('Style error')  # pragma: no cover
 
     xmin, ymax = deg2num(lat_deg, lon_deg, zoom)
     xmax, ymin = deg2num(lat_deg + delta_lat, lon_deg + delta_long, zoom)
 
     def get_img(smurl, zoom, xtile, ytile, imgsize, imgsavepath):
         import os
 
         filename = str(style)+str(styleid)+'-'+str(zoom)+'-' + \
             str(xtile)+'-'+str(ytile)+'-'+str(imgsize)+'.png'
 
         def savefig(filename, tile):
             try:
                 if 'tileimg' in os.listdir(imgsavepath):
-                    if filename in os.listdir(imgsavepath+'tileimg'):
-                        pass
+                    if filename in os.listdir(imgsavepath+'tileimg'):  # pragma: no cover
+                        pass  # pragma: no cover
                     else:
-                        tile.save(imgsavepath+'tileimg/'+filename)
-                        if printlog:
-                            print('figsaved:'+imgsavepath+'tileimg/'+filename)
+
+                        tile.save(os.path.join(imgsavepath+'tileimg',
+                                  filename))  # pragma: no cover
+                        if printlog:  # pragma: no cover
+                            print('figsaved:'+os.path.join(imgsavepath+'tileimg',
+                                  filename))  # pragma: no cover
                 else:
                     os.mkdir(imgsavepath+'tileimg')
-            except Exception:
-                pass
+            except Exception as e:
+                print(e)
 
         def loadfig(filename):
             try:
                 if 'tileimg' in os.listdir(imgsavepath):
-                    if filename in os.listdir(imgsavepath+'tileimg'):
-                        tile = Image.open(imgsavepath+'tileimg\\'+filename)
-                        return tile
+                    if filename in os.listdir(imgsavepath+'tileimg'):  # pragma: no cover
+                        tile = Image.open(
+                            os.path.join(os.path.join(imgsavepath, 'tileimg'), filename))  # pragma: no cover
+                        return tile  # pragma: no cover
                     else:
-                        return None
+                        return None  # pragma: no cover
                 else:
                     os.mkdir(imgsavepath+'tileimg')
-                    return None
-            except Exception:
-                return None
+                    return None  # pragma: no cover
+            except Exception as e:
+                if printlog:  # pragma: no cover
+                    print(e) # pragma: no cover
+                return None # pragma: no cover
 
         tile = loadfig(filename)
         if tile is None:
             try:
                 t = 0
                 while t < 10:
                     try:
                         imgurl = smurl.format(zoom, xtile, ytile)
                         header = {}
                         header['Accept'] = 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8'
                         header['Accept-Language'] = 'zh-CN,zh;q=0.8'
                         header['Upgrade-Insecure-Requests'] = '1'
                         header['User-Agent'] = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/51.0.2704.84 Safari/537.36'
-                        request = urllib.request.Request(imgurl)
-                        for k, v in header.items():
-                            request.add_header(k, v)
-                        imgstr = urllib.request.urlopen(
-                            request, timeout=6).read()
+
+                        import requests
+                        response1 = requests.get(
+                            imgurl, headers=header, timeout=6)
+                        imgstr = response1.content
                         tile = Image.open(io.BytesIO(imgstr))
                         savefig(filename, tile)
                         Cluster.paste(tile, box=(
                             (xtile-xmin)*imgsize,  (ytile-ymin)*imgsize))
                         t = 10
-                    except Exception:
-                        if printlog:
-                            print('Get map tile failed, retry ', t)
-                        t += 1
-            except Exception:
-                print("Couldn't download image")
-                tile = None
-        else:
+                    except Exception:  # pragma: no cover
+                        if printlog:  # pragma: no cover
+                            print('Get map tile failed, retry ',
+                                  t)  # pragma: no cover
+                        t += 1  # pragma: no cover
+            except Exception:  # pragma: no cover
+                print("Couldn't download image")  # pragma: no cover
+                tile = None  # pragma: no cover
+        else:  # pragma: no cover
             Cluster.paste(tile, box=(
-                (xtile-xmin)*imgsize,  (ytile-ymin)*imgsize))
+                (xtile-xmin)*imgsize,  (ytile-ymin)*imgsize))  # pragma: no cover
 
     imgsize = 256
     import threading
     threads = []
     Cluster = Image.new(
         'RGB', ((xmax-xmin+1)*imgsize-1, (ymax-ymin+1)*imgsize-1))
     for xtile in range(xmin, xmax+1):
@@ -337,30 +348,32 @@
     printlog : bool
         Show log
     style : number
         The style of map basemap can be 1-10, as follows
     '''
     access_token = read_mapboxtoken()
     if access_token == '':
-        style = 0
+        style = 0  # pragma: no cover
     imgsavepath = read_imgsavepath()
     if imgsavepath != '':
         try:
             import os
             os.listdir(imgsavepath)
-        except Exception:
-            warnings.warn('imgsavepath do not exist, your tile map will not save')
+        except Exception:  # pragma: no cover
+            warnings.warn(  # pragma: no cover
+                'imgsavepath do not exist, your tile map will not save')
     else:
-        warnings.warn('imgsavepath do not exist, your tile map will not save')
+        warnings.warn(
+            'imgsavepath do not exist, your tile map will not save')  # pragma: no cover
     lon1 = bounds[0]
     lat1 = bounds[1]
     lon2 = bounds[2]
     lat2 = bounds[3]
     if zoom == 'auto':
-        zoom = 11-np.log(lon2-lon1)/np.log(2)
+        zoom = 11-np.log(lon2-lon1)/np.log(2)  # pragma: no cover
     zoom = min(18, int(zoom+0.5))
     a = getImageCluster(lon1, lat1, lon2-lon1,  lat2-lat1, zoom, style=style,
                         printlog=printlog, imgsavepath=imgsavepath,
                         access_token=access_token)
     x1, y1 = deg2num(lat1, lon1, zoom)
     x2, y2 = deg2num(lat2, lon2, zoom)
     x1, y1 = num2deg(x1, y1+1, zoom)
@@ -396,15 +409,15 @@
     '''
     import math
     lon1 = bounds[0]
     lat1 = bounds[1]
     lon2 = bounds[2]
     lat2 = bounds[3]
     if accuracy == 'auto':
-        accuracy = (int((lon2-lon1)/0.0003/1000+0.5)*1000)
+        accuracy = (int((lon2-lon1)/0.0003/1000+0.5)*1000)  # pragma: no cover
     a, c = rect
     b = 1-a
     d = 1-c
     alon, alat = (b*lon1+a*lon2)/(a+b), (d*lat1+c*lat2)/(c+d)
     deltaLon = accuracy * 360 / \
         (2 * math.pi * 6371004 * math.cos((lat1 + lat2) * math.pi / 360))
     # add scale
@@ -469,18 +482,18 @@
             ax.text(alon+8.5*deltaLon, alat+deltaLon*0.5, unit,
                     color=textcolor, fontsize=textsize,
                     ha='left', va='top')
     if style == 2:
         scale = gpd.GeoDataFrame({
             'color': [(0, 0, 0), (1, 1, 1)],
             'geometry':
-            [Polygon([(alon+deltaLon, alat),
+            [Polygon([(alon, alat),
                       (alon+4*deltaLon, alat),
                       (alon+4*deltaLon, alat+deltaLon*0.4),
-                      (alon+deltaLon, alat+deltaLon*0.4)]),
+                      (alon, alat+deltaLon*0.4)]),
                 Polygon([(alon+4*deltaLon, alat),
                          (alon+8*deltaLon, alat),
                          (alon+8 * deltaLon, alat+deltaLon*0.4),
                          (alon+4*deltaLon, alat+deltaLon*0.4)])
              ]})
         scale.plot(ax=ax, edgecolor=textcolor,
                    facecolor=scale['color'], lw=0.6, **kwargs)
```

### Comparing `transbigdata-0.4.9/src/transbigdata/preprocess.py` & `transbigdata-0.5.0/src/transbigdata/preprocess.py`

 * *Files 24% similar despite different names*

```diff
@@ -28,131 +28,24 @@
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 '''
 
 import geopandas as gpd
 import pandas as pd
+import numpy as np
 from .grids import (
     GPS_to_grid,
     area_to_params,
     grid_to_centre,
     grid_to_polygon
 )
 from .coordinates import getdistance
 
 
-def clean_same(data, col=['VehicleNum', 'Time', 'Lng', 'Lat']):
-    '''
-    Delete the data with the same information as the data before and
-    after to reduce the amount of data. For example, if several consecutive
-    data of an individual have the same information except for the time,
-    only the first and last two data can be kept
-
-    Parameters
-    -------
-    data : DataFrame
-        Data
-    col : List
-        The column name, in the order of [‘Vehicleid, Time’]. It will sort
-        by time, and then determine the information of other columns besides
-        the time
-
-    Returns
-    -------
-    data1 : DataFrame
-        Cleaned data
-    '''
-    [VehicleNum, Time, Lng, Lat] = col[:4]
-    extra = col[4:]
-    data1 = data.copy()
-    data1 = data1.drop_duplicates(subset=[VehicleNum, Time])
-    data1 = data1.sort_values(by=[VehicleNum, Time])
-    data1['issame'] = 0
-    for i in [VehicleNum, Lng, Lat]+extra:
-        data1['issame'] += (data1[i].shift() == data1[i]
-                            ) & (data1[i].shift(-1) == data1[i])
-    data1 = data1[-(data1['issame'] == len([VehicleNum, Lng, Lat]+extra))]
-    data1 = data1.drop('issame', axis=1)
-    return data1
-
-
-def clean_drift(data, col=['VehicleNum', 'Time', 'Lng', 'Lat'],
-                speedlimit=80, dislimit=1000):
-    '''
-    Delete the drift data. The select principle is that: if the speed of a
-    trajectory point is larger than the speed limit with before and after
-    points, while the speed between the before and after data is less than
-    the speedlimit. The time column in the input data is calculated more
-    efficiently if it is in datetime format.
-
-    Parameters
-    -------
-    data : DataFrame
-        Data
-    col : List
-        Column names, in the order of [‘VehicleNum’, ‘Time’, ‘Lng’, ‘Lat’]
-    speedlimit : number
-        Speed limitation
-
-    Returns
-    -------
-    data1 : DataFrame
-        Cleaned data
-    '''
-    [VehicleNum, Time, Lng, Lat] = col
-    data1 = data.copy()
-    data1 = data1.drop_duplicates(subset=[VehicleNum, Time])
-    data1[Time+'_dt'] = pd.to_datetime(data1[Time])
-    data1 = data1.sort_values(by=[VehicleNum, Time])
-    for i in [VehicleNum, Lng, Lat, Time+'_dt']:
-        data1[i+'_pre'] = data1[i].shift()
-        data1[i+'_next'] = data1[i].shift(-1)
-    data1['dis_pre'] = getdistance(
-        data1[Lng],
-        data1[Lat],
-        data1[Lng+'_pre'],
-        data1[Lat+'_pre'])
-    data1['dis_next'] = getdistance(
-        data1[Lng],
-        data1[Lat],
-        data1[Lng+'_next'],
-        data1[Lat+'_next'])
-    data1['dis_prenext'] = getdistance(
-        data1[Lng+'_pre'],
-        data1[Lat+'_pre'],
-        data1[Lng+'_next'],
-        data1[Lat+'_next'])
-    data1['timegap_pre'] = data1[Time+'_dt'] - data1[Time+'_dt_pre']
-    data1['timegap_next'] = data1[Time+'_dt_next'] - data1[Time+'_dt']
-    data1['timegap_prenext'] = data1[Time+'_dt_next'] - data1[Time+'_dt_pre']
-    data1['speed_pre'] = data1['dis_pre'] / \
-        data1['timegap_pre'].dt.total_seconds()*3.6
-    data1['speed_next'] = data1['dis_next'] / \
-        data1['timegap_next'].dt.total_seconds()*3.6
-    data1['speed_prenext'] = data1['dis_prenext'] / \
-        data1['timegap_prenext'].dt.total_seconds()*3.6
-    if speedlimit:
-        data1 = data1[
-            -((data1[VehicleNum+'_pre'] == data1[VehicleNum]) &
-              (data1[VehicleNum+'_next'] == data1[VehicleNum]) &
-                (data1['speed_pre'] > speedlimit) &
-              (data1['speed_next'] > speedlimit) &
-              (data1['speed_prenext'] < speedlimit))]
-    if dislimit:
-        data1 = data1[
-            -((data1[VehicleNum+'_pre'] == data1[VehicleNum]) &
-              (data1[VehicleNum+'_next'] == data1[VehicleNum]) &
-              (data1['dis_pre'] > dislimit) &
-              (data1['dis_next'] > dislimit) &
-              (data1['dis_prenext'] < dislimit))]
-    data1 = data1[data.columns]
-    return data1
-
-
 def clean_outofbounds(data, bounds, col=['Lng', 'Lat']):
     '''
     The input is the latitude and longitude coordinates of the lower
     left and upper right of the study area and exclude data that are
     outside the study area
 
     Parameters
@@ -169,15 +62,15 @@
     -------
     data1 : DataFrame
         Data within the scope of the study
     '''
     lon1, lat1, lon2, lat2 = bounds
     if (lon1 > lon2) | (lat1 > lat2) | (abs(lat1) > 90) | (
             abs(lon1) > 180) | (abs(lat2) > 90) | (abs(lon2) > 180):
-        raise Exception(
+        raise Exception(  # pragma: no cover
             'Bounds error. The input bounds should be in the order \
 of [lon1,lat1,lon2,lat2]. (lon1,lat1) is the lower left corner and \
 (lon2,lat2) is the upper right corner.')
     Lng, Lat = col
     data1 = data.copy()
     data1 = data1[(data1[Lng] > bounds[0]) & (data1[Lng] < bounds[2]) & (
         data1[Lat] > bounds[1]) & (data1[Lat] < bounds[3])]
@@ -219,72 +112,14 @@
         [data1_gdf['LONCOL'], data1_gdf['LATCOL']], params)
     data1_gdf = gpd.GeoDataFrame(data1_gdf)
     data1_gdf = data1_gdf[data1_gdf.intersects(shape_unary)]
     data1 = pd.merge(data1, data1_gdf[['LONCOL', 'LATCOL']]).drop(
         ['LONCOL', 'LATCOL'], axis=1)
     return data1
 
-
-def clean_traj(data, col=['uid', 'str_time', 'lon', 'lat'], tripgap=1800,
-               disgap=50000, speedlimit=80):
-    '''
-    A combo for trajectory data cleaning, including defining the the time
-    length threshold considered as a new trip, and the distance threshold
-    considered as a new trip
-
-    Parameters
-    -------
-    data : DataFrame
-        Trajectory data
-    col : List
-        Column names, in the order of [‘VehicleNum’, ‘Time’, ‘Lng’, ‘Lat’]
-    tripgap : number
-        The time length threshold considered as a new trip
-    disgap : number
-        The distance threshold considered as a new trip
-    speedlimit : number
-        Speed limit
-
-    Returns
-    -------
-    data1 : DataFrame
-        Cleaned data
-    '''
-    uid, timecol, lon, lat = col
-    data[timecol] = pd.to_datetime(data[timecol])
-    data = data.sort_values(by=[uid, timecol])
-    cols = []
-    for i in data.columns:
-        if i not in [uid, timecol, lon, lat]:
-            cols.append(i)
-    data = clean_same(data, col=[uid, timecol, lon, lat]+cols)
-    data = clean_drift(data, col=[uid, timecol, lon, lat],
-                       speedlimit=speedlimit)
-    data = id_reindex(data, uid, timecol=timecol, timegap=tripgap)
-    data = data.rename(columns={uid+'_new': 'tripid'})
-    data = id_reindex_disgap(
-        data, col=['tripid', lon, lat], disgap=disgap, suffix='')
-    data1 = data.copy()
-    data1['lon1'] = data1[lon].shift(-1)
-    data1['lat1'] = data1[lat].shift(-1)
-    data1['tripid1'] = data1['tripid'].shift(-1)
-    data1 = data1[data1['tripid'] == data1['tripid1']]
-    data1['dis'] = getdistance(
-        data1[lon], data1[lat], data1['lon1'], data1['lat1'])
-    a = data1.groupby(['tripid'])['dis'].sum()
-    a = a[-(a < 50)].reset_index()['tripid']
-    data = pd.merge(data, a)
-    data = data.drop('tripid', axis=1)
-    data = id_reindex(data, uid, timecol=timecol, timegap=tripgap)
-    data = data.rename(columns={uid+'_new': 'tripid'})
-    data = id_reindex_disgap(
-        data, col=['tripid', lon, lat], disgap=disgap, suffix='')
-    return data
-
-
 def dataagg(data, shape, col=['Lng', 'Lat', 'count'], accuracy=500):
     '''
     Aggregate data to traffic zone
 
     Parameters
     -------
     data : DataFrame
@@ -304,16 +139,16 @@
     -------
     aggresult : GeoDataFrame
         Traffic zone. The count column is the output result
     data1 : DataFrame
         The zone-matched data
     '''
     if len(col) == 2:
-        Lng, Lat = col
-        aggcol = None
+        Lng, Lat = col  # pragma: no cover
+        aggcol = None  # pragma: no cover
     else:
         Lng, Lat, aggcol = col
     shape['index'] = range(len(shape))
     shape_unary = shape.unary_union
     bounds = shape_unary.bounds
     params = area_to_params(bounds, accuracy)
     data1 = data.copy()
@@ -325,18 +160,18 @@
     data1_gdf = gpd.GeoDataFrame(data1_gdf)
     data1_gdf = gpd.sjoin(data1_gdf, shape, how='left')
     data1 = pd.merge(data1, data1_gdf).drop(['LONCOL', 'LATCOL'], axis=1)
     if aggcol:
         aggresult = pd.merge(shape, data1.groupby('index')[
                              aggcol].sum().reset_index()).drop('index', axis=1)
     else:
-        data1['_'] = 1
-        aggresult = pd.merge(shape, data1.groupby('index')['_'].sum().rename(
+        data1['_'] = 1  # pragma: no cover
+        aggresult = pd.merge(shape, data1.groupby('index')['_'].sum().rename(  # pragma: no cover
             'count').reset_index()).drop('index', axis=1)
-        data1 = data1.drop('_', axis=1)
+        data1 = data1.drop('_', axis=1)  # pragma: no cover
     data1 = data1.drop('index', axis=1)
     return aggresult, data1
 
 
 def id_reindex_disgap(data, col=['uid', 'lon', 'lat'], disgap=1000,
                       suffix='_new'):
     '''
```

### Comparing `transbigdata-0.4.9/src/transbigdata/quality.py` & `transbigdata-0.5.0/src/transbigdata/quality.py`

 * *Files 9% similar despite different names*

```diff
@@ -104,7 +104,23 @@
         print('-----------------')
         print('Mean: ', round(sd['duration'].mean(), roundnum), 's')
         print('Upper quartile: ', round(
             sd['duration'].quantile(0.75), roundnum), 's')
         print('Median: ', round(sd['duration'].quantile(0.5), roundnum), 's')
         print('Lower quartile: ', round(
             sd['duration'].quantile(0.25), roundnum), 's')
+        # Plot the distribution of sampling interval
+        import seaborn as sns
+        import matplotlib.pyplot as plt
+        import matplotlib
+        matplotlib.rcParams['font.sans-serif'] = 'Arial'
+        fig = plt.figure(1,(8,3),dpi=300)
+        ax = plt.subplot(111)
+        plt.subplots_adjust(left=0.19,right=0.98,top=0.9,bottom=0.19)
+        sns.kdeplot(sd[sd['duration']<sd['duration'].quantile(0.95)],ax=ax,legend=False)
+        from matplotlib import ticker
+        formatter = ticker.ScalarFormatter(useMathText=True)
+        formatter.set_scientific(True)
+        formatter.set_powerlimits((0,0))
+        plt.xlabel('Sampling interval (s)')
+        plt.xlim(0, sd['duration'].quantile(0.95))
+        plt.show()
```

### Comparing `transbigdata-0.4.9/src/transbigdata/taxigps.py` & `transbigdata-0.5.0/src/transbigdata/taxigps.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     Returns
     -------
     data1 : DataFrame
         Cleaned data
     '''
     data1 = data.copy()
     [VehicleNum, Time, OpenStatus] = col
+    #Sort the VehicleNum and Time columns
+    data1 = data1.sort_values(by=[VehicleNum,Time])
     if timelimit:
         data1[Time] = pd.to_datetime(data1[Time])
         data1 = data1[
             -((data1[OpenStatus].shift(-1) == data1[OpenStatus].shift()) &
               (data1[OpenStatus] != data1[OpenStatus].shift()) &
               (data1[VehicleNum].shift(-1) == data1[VehicleNum].shift()) &
               (data1[VehicleNum] == data1[VehicleNum].shift()) &
```

### Comparing `transbigdata-0.4.9/src/transbigdata/visualization.py` & `transbigdata-0.5.0/src/transbigdata/visualization.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,16 +66,16 @@
     Returns
     -------
     vmap : keplergl.keplergl.KeplerGl
         Visualizations provided by keplergl
     '''
     try:
         from keplergl import KeplerGl
-    except ImportError:
-        raise ImportError(
+    except ImportError: # pragma: no cover
+        raise ImportError( # pragma: no cover
             "Please install keplergl, run "
             "the following code in cmd: pip install keplergl")
     print('Processing trajectory data...')
     [Lng, Lat, ID, timecol] = col
         #clean data
     trajdata = trajdata[-((trajdata[Lng].isnull())|(trajdata[Lat].isnull()))]
     trajdata = trajdata[(trajdata[Lng]>=-180)&(trajdata[Lng]<=180)&(trajdata[Lat]>=-90)&(trajdata[Lat]<=90)]
@@ -166,16 +166,16 @@
     Returns
     -------
     vmap : keplergl.keplergl.KeplerGl
         Visualizations provided by keplergl
     '''
     try:
         from keplergl import KeplerGl
-    except ImportError:
-        raise ImportError(
+    except ImportError: # pragma: no cover
+        raise ImportError( # pragma: no cover
             "Please install keplergl, run "
             "the following code in cmd: pip install keplergl")
     import numpy as np
     if len(col) == 4:
         slon, slat, elon, elat = col
         lon1 = oddata[slon].astype(float).quantile(0.01)
         lon2 = oddata[slon].astype(float).quantile(0.99)
@@ -399,16 +399,16 @@
     Returns
     -------
     vmap : keplergl.keplergl.KeplerGl
         Visualizations provided by keplergl
     '''
     try:
         from keplergl import KeplerGl
-    except ImportError:
-        raise ImportError(
+    except ImportError: # pragma: no cover
+        raise ImportError( # pragma: no cover
             "Please install keplergl, run "
             "the following code in cmd: pip install keplergl")
 
     if len(col) == 2:
         lon, lat = col[0], col[1]
         count = 'count'
 
@@ -461,15 +461,15 @@
             [data['LONCOL'], data['LATCOL']], params)
         data[lon], data[lat] = grid_to_centre(
             [data['LONCOL'], data['LATCOL']], params)
 
         data = gpd.GeoDataFrame(data)
 
     if maptype == 'heatmap':
-        vmap = KeplerGl(config={
+        vmap = KeplerGl(config={ # pragma: no cover
             'version': 'v1',
             'config': {
                 'visState': {
                     'filters': [],
                     'layers': [
                         {'id': 'vpefba0o',
                          'type': 'heatmap',
```

### Comparing `transbigdata-0.4.9/transbigdata.egg-info/PKG-INFO` & `transbigdata-0.5.0/transbigdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transbigdata
-Version: 0.4.9
+Version: 0.5.0
 Summary: A Python package developed for transportation spatio-temporal big data processing and analysis.
 Home-page: https://github.com/ni1o1/transbigdata
 Author: Qing Yu
 Author-email: qingyu0815@foxmail.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/ni1o1/transbigdata/issues
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 
 English [中文版](README-zh_CN.md)
 
 # TransBigData
 
 <img src="https://github.com/ni1o1/transbigdata/raw/main/docs/source/_static/logo-wordmark-dark.png" style="width:550px">
 
-[![Documentation Status](https://readthedocs.org/projects/transbigdata/badge/?version=latest)](https://transbigdata.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://pepy.tech/badge/transbigdata)](https://pepy.tech/project/transbigdata) [![Downloads](https://pepy.tech/badge/transbigdata/week)](https://pepy.tech/project/transbigdata) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ni1o1/transbigdata/d7d6fa33ff16440ba1698b10dd3cf3f76ff00abd?urlpath=lab%2Ftree%2Fexample%2FExample%201-Taxi%20GPS%20data%20processing.ipynb) [![Tests](https://github.com/ni1o1/transbigdata/actions/workflows/tests.yml/badge.svg)](https://github.com/ni1o1/transbigdata/actions/workflows/tests.yml) [![codecov](https://codecov.io/gh/ni1o1/transbigdata/branch/main/graph/badge.svg?token=GLAVYYCD9L)](https://codecov.io/gh/ni1o1/transbigdata)
+[![Documentation Status](https://readthedocs.org/projects/transbigdata/badge/?version=latest)](https://transbigdata.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://pepy.tech/badge/transbigdata)](https://pepy.tech/project/transbigdata) [![Downloads](https://pepy.tech/badge/transbigdata/week)](https://pepy.tech/project/transbigdata) [![Tests](https://github.com/ni1o1/transbigdata/actions/workflows/tests.yml/badge.svg)](https://github.com/ni1o1/transbigdata/actions/workflows/tests.yml) [![codecov](https://codecov.io/gh/ni1o1/transbigdata/branch/main/graph/badge.svg?token=GLAVYYCD9L)](https://codecov.io/gh/ni1o1/transbigdata)
 
 ## Introduction
 
 `TransBigData` is a Python package developed for transportation spatio-temporal big data processing, analysis and visualization. `TransBigData` provides fast and concise methods for processing common transportation spatio-temporal big data such as Taxi GPS data, bicycle sharing data and bus GPS data. `TransBigData` provides a variety of processing methods for each stage of transportation spatio-temporal big data analysis. The code with `TransBigData` is clean, efficient, flexible, and easy to use, allowing complex data tasks to be achieved with concise code.
 
 For some specific types of data, `TransBigData` also provides targeted tools for specific needs, such as extraction of Origin and Destination(OD) of taxi trips from taxi GPS data and identification of arrival and departure information from bus GPS data. The latest stable release of the software can be installed via pip and full documentation
 can be found at https://transbigdata.readthedocs.io/en/latest/. Introduction PPT can be found [here](https://github.com/ni1o1/transbigdata/blob/main/introduction/IntroductionofTransBigData.pdf) and [here(in Chinese)](https://github.com/ni1o1/transbigdata/blob/main/introduction/gridbasedframework.pdf)
@@ -57,23 +57,23 @@
 * **Data Aggregating**: Provides methods to aggregate GPS data and OD data into geographic polygon.
 * **Data Visualization**: Built-in visualization capabilities leverage the visualization package keplergl to interactively visualize data on Jupyter notebook with simple code.
 * **Trajectory Processing**: Provides methods to process trajectory data, including generating trajectory linestring from GPS points, and trajectory densification, etc.
 * **Basemap Loading**: Provides methods to display Mapbox basemap on matplotlib figures
 
 ## Installation
 
-It is recommended to use `Python 3.7, 3.8, 3.9`
+`TransBigData` support Python >= 3.6
 
 ### Using pypi [![PyPI version](https://badge.fury.io/py/transbigdata.svg)](https://badge.fury.io/py/transbigdata)
 
 `TransBigData` can be installed by using `pip install`. Before installing `TransBigData`, make sure that you have installed the available [geopandas package](https://geopandas.org/en/stable/getting_started/install.html). If you already have geopandas installed, run the following code directly from the command prompt to install `TransBigData`:
 
     pip install transbigdata
 
-### Using conda-forge [![Conda Version](https://img.shields.io/conda/vn/conda-forge/transbigdata.svg)](https://anaconda.org/conda-forge/transbigdata) [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/transbigdata.svg)](https://anaconda.org/conda-forge/transbigdata) 
+### Using conda-forge [![Conda Version](https://img.shields.io/conda/vn/conda-forge/transbigdata.svg)](https://anaconda.org/conda-forge/transbigdata) [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/transbigdata.svg)](https://anaconda.org/conda-forge/transbigdata)
 
 You can also install `TransBigData` by `conda-forge`, this will automaticaly solve the dependency, it can be installed with:
 
     conda install -c conda-forge transbigdata
 
 ## Contributing to TransBigData [![GitHub contributors](https://img.shields.io/github/contributors/ni1o1/transbigdata.svg)](https://github.com/ni1o1/transbigdata/graphs/contributors) [![Join the chat at https://gitter.im/transbigdata/community](https://badges.gitter.im/transbigdata/community.svg)](https://gitter.im/transbigdata/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ni1o1/transbigdata)
 
@@ -81,23 +81,23 @@
 
 ## Examples
 
 ### Example of data visualization
 
 #### Visualize trajectories (with keplergl)
 
-![gif](https://github.com/ni1o1/transbigdata/raw/main/images/tbdexample1.gif)
+![gif](https://github.com/ni1o1/transbigdata/raw/main/image/README/tbdexample1.gif)
 
 #### Visualize data distribution (with keplergl)
 
-![gif](https://github.com/ni1o1/transbigdata/raw/main/images/tbdexample2.gif)
+![gif](https://github.com/ni1o1/transbigdata/raw/main/image/README/tbdexample2.gif)
 
 #### Visualize OD (with keplergl)
 
-![gif](https://github.com/ni1o1/transbigdata/raw/main/images/tbdexample3.gif)
+![gif](https://github.com/ni1o1/transbigdata/raw/main/image/README/tbdexample3.gif)
 
 ### Example of taxi GPS data processing
 
 The following example shows how to use the `TransBigData` to perform data gridding, data aggregating and data visualization for taxi GPS data.
 
 #### Read the data
 
@@ -276,15 +276,15 @@
 #Change the type into GeoDataFrame
 import geopandas as gpd
 grid_agg = gpd.GeoDataFrame(grid_agg)
 #Plot the grids
 grid_agg.plot(column = 'VehicleNum',cmap = 'autumn_r')
 ```
 
-![png](https://github.com/ni1o1/transbigdata/raw/main/images/output_5_1.png)
+![png](https://github.com/ni1o1/transbigdata/raw/main/image/README/output_5_1.png)
 
 #### Triangle and Hexagon grids & rotation angle
 
 `TransBigData` also support the triangle and hexagon grids. It also supports given rotation angle for the grids. We can alter the gridding parameter:
 
 ```python
 #set to the hexagon grids
@@ -341,15 +341,15 @@
 
 #### Griding framework offered by TransBigData
 
 Here is an overview of the gridding framework offered by `TransBigData`.
 
 ![1648715064154.png](https://github.com/ni1o1/transbigdata/raw/main/image/README/1648715064154.png)
 
-See [This Example](https://github.com/ni1o1/transbigdata/blob/main/example/TBD_Core_Functions.ipynb) for further details.
+See [This Example](https://github.com/ni1o1/transbigdata/blob/main/docs/source/gallery/Example%202-Grid-base%20processing%20framework%20of%20TransBigData.ipynb) for further details.
 
 ## Citation information [![DOI](https://zenodo.org/badge/419559811.svg)](https://zenodo.org/badge/latestdoi/419559811) [![status](https://joss.theoj.org/papers/d1055fe3105dfa2dcff4cb6c7688a79b/status.svg)](https://joss.theoj.org/papers/d1055fe3105dfa2dcff4cb6c7688a79b)
 
 Please cite [this](https://doi.org/10.21105/joss.04021) when using `TransBigData` in your research. Citation information can be found at [CITATION.cff](https://github.com/ni1o1/transbigdata/blob/main/CITATION.cff).
 
 ## Introducing Video (In Chinese) [![bilibili](https://img.shields.io/badge/bilibili-%E5%90%8C%E6%B5%8E%E5%B0%8F%E6%97%AD%E5%AD%A6%E9%95%BF-green.svg)](https://space.bilibili.com/3051484)
```

### Comparing `transbigdata-0.4.9/transbigdata.egg-info/SOURCES.txt` & `transbigdata-0.5.0/transbigdata.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 src/transbigdata/__init__.py
+src/transbigdata/activity.py
 src/transbigdata/bikedata.py
 src/transbigdata/busgps.py
 src/transbigdata/coordinates.py
 src/transbigdata/crawler.py
 src/transbigdata/gisprocess.py
 src/transbigdata/grids.py
 src/transbigdata/metro.py
+src/transbigdata/mobilephonedata.py
 src/transbigdata/odprocess.py
 src/transbigdata/plotmap.py
 src/transbigdata/preprocess.py
 src/transbigdata/quality.py
 src/transbigdata/taxigps.py
 src/transbigdata/traj.py
+src/transbigdata/utils.py
 src/transbigdata/visualization.py
 transbigdata.egg-info/PKG-INFO
 transbigdata.egg-info/SOURCES.txt
 transbigdata.egg-info/dependency_links.txt
 transbigdata.egg-info/requires.txt
 transbigdata.egg-info/top_level.txt
```

