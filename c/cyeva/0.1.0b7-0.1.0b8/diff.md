# Comparing `tmp/cyeva-0.1.0b7.tar.gz` & `tmp/cyeva-0.1.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyeva-0.1.0b7.tar", last modified: Thu Mar  2 07:07:08 2023, max compression
+gzip compressed data, was "cyeva-0.1.0b8.tar", last modified: Wed May 24 06:43:44 2023, max compression
```

## Comparing `cyeva-0.1.0b7.tar` & `cyeva-0.1.0b8.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:07:08.601654 cyeva-0.1.0b7/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-03-02 07:07:08.601654 cyeva-0.1.0b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:07:08.597654 cyeva-0.1.0b7/cyeva/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/cyeva/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:07:08.597654 cyeva-0.1.0b7/cyeva/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/cyeva/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:07:08.597654 cyeva-0.1.0b7/cyeva/config/directions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/cyeva/config/directions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/cyeva/config/directions/wind.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:07:08.597654 cyeva-0.1.0b7/cyeva/config/levels/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/cyeva/config/levels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:07:08.597654 cyeva-0.1.0b7/cyeva/config/levels/precip/
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/cyeva/config/levels/precip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:07:08.597654 cyeva-0.1.0b7/cyeva/config/levels/wind/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/cyeva/config/levels/wind/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:07:08.601654 cyeva-0.1.0b7/cyeva/core/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/cyeva/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/cyeva/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/cyeva/core/binarize.py
--rw-r--r--   0 runner    (1001) docker     (123)    24657 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/cyeva/core/precip.py
--rw-r--r--   0 runner    (1001) docker     (123)    20871 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/cyeva/core/statistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/cyeva/core/temp.py
--rw-r--r--   0 runner    (1001) docker     (123)    30912 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/cyeva/core/wind.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/cyeva/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:07:08.601654 cyeva-0.1.0b7/cyeva/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/cyeva/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/cyeva/utils/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:07:08.597654 cyeva-0.1.0b7/cyeva.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-03-02 07:07:08.000000 cyeva-0.1.0b7/cyeva.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-02 07:07:08.000000 cyeva-0.1.0b7/cyeva.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 07:07:08.000000 cyeva-0.1.0b7/cyeva.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-02 07:07:08.000000 cyeva-0.1.0b7/cyeva.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-02 07:07:08.000000 cyeva-0.1.0b7/cyeva.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:07:08.601654 cyeva-0.1.0b7/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/requirements/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 07:07:08.601654 cyeva-0.1.0b7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:07:08.601654 cyeva-0.1.0b7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/tests/test_binarize.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    24403 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/tests/test_precip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/tests/test_temp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-03-02 07:06:57.000000 cyeva-0.1.0b7/tests/test_wind.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.804003 cyeva-0.1.0b8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-05-24 06:43:44.804003 cyeva-0.1.0b8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.800003 cyeva-0.1.0b8/cyeva/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.800003 cyeva-0.1.0b8/cyeva/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.800003 cyeva-0.1.0b8/cyeva/config/directions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/config/directions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/config/directions/wind.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.800003 cyeva-0.1.0b8/cyeva/config/levels/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/config/levels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.800003 cyeva-0.1.0b8/cyeva/config/levels/precip/
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/config/levels/precip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.800003 cyeva-0.1.0b8/cyeva/config/levels/wind/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/config/levels/wind/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.800003 cyeva-0.1.0b8/cyeva/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/core/binarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24657 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/core/precip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22926 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/core/statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/core/temp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30926 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/core/wind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.804003 cyeva-0.1.0b8/cyeva/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/cyeva/utils/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.800003 cyeva-0.1.0b8/cyeva.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-05-24 06:43:44.000000 cyeva-0.1.0b8/cyeva.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-24 06:43:44.000000 cyeva-0.1.0b8/cyeva.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 06:43:44.000000 cyeva-0.1.0b8/cyeva.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-24 06:43:44.000000 cyeva-0.1.0b8/cyeva.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 06:43:44.000000 cyeva-0.1.0b8/cyeva.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.804003 cyeva-0.1.0b8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/requirements/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 06:43:44.804003 cyeva-0.1.0b8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:43:44.804003 cyeva-0.1.0b8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/tests/test_binarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24403 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/tests/test_precip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/tests/test_statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/tests/test_temp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-05-24 06:43:28.000000 cyeva-0.1.0b8/tests/test_wind.py
```

### Comparing `cyeva-0.1.0b7/PKG-INFO` & `cyeva-0.1.0b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyeva
-Version: 0.1.0b7
+Version: 0.1.0b8
 Summary: A package to evaluate weather forecast correction
 Home-page: https://github.com/caiyunapp/cyeva
 Author: caiyunapp
 Author-email: oss@caiyunapp.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -30,15 +30,15 @@
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/cyeva/badges/platforms.svg)](https://anaconda.org/conda-forge/cyeva)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/cyeva/badges/latest_release_date.svg)](https://anaconda.org/conda-forge/cyeva)
 [![Pypi](https://badge.fury.io/py/cyeva.svg)](https://badge.fury.io/py/cyeva)
 [![Documentation Status](https://readthedocs.org/projects/cyeva/badge/?version=latest)](https://cyeva.readthedocs.io/zh_CN/latest/?badge=latest)
 [![Download statistic](https://pepy.tech/badge/cyeva)](https://pepy.tech/project/cyeva)
 [![codecov](https://codecov.io/gh/caiyunapp/cyeva/branch/main/graph/badge.svg?token=344FXDKAYD)](https://codecov.io/gh/caiyunapp/cyeva)
 [![style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Anaconda-Server Badge](https://anaconda.org/conda-forge/cyeva/badges/license.svg)](https://anaconda.org/conda-forge/cyeva)
+
 
 cyeva 是一个由彩云科技天气团队开发的用于对气象要素确定性预报准确率进行快速评测的 Python 开源工具库。
 
 cyeva 将致力于让气象要素确定性预报准确率的自动化评估变得简单直接，将集成常用的确定性预报准确率评估指标，且内部算法广泛使用了 numpy 的向量运算实现，对于大数据量的计算也具有较高的计算效率。
 
 ## 安装
```

### Comparing `cyeva-0.1.0b7/README.md` & `cyeva-0.1.0b8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/cyeva/badges/platforms.svg)](https://anaconda.org/conda-forge/cyeva)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/cyeva/badges/latest_release_date.svg)](https://anaconda.org/conda-forge/cyeva)
 [![Pypi](https://badge.fury.io/py/cyeva.svg)](https://badge.fury.io/py/cyeva)
 [![Documentation Status](https://readthedocs.org/projects/cyeva/badge/?version=latest)](https://cyeva.readthedocs.io/zh_CN/latest/?badge=latest)
 [![Download statistic](https://pepy.tech/badge/cyeva)](https://pepy.tech/project/cyeva)
 [![codecov](https://codecov.io/gh/caiyunapp/cyeva/branch/main/graph/badge.svg?token=344FXDKAYD)](https://codecov.io/gh/caiyunapp/cyeva)
 [![style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Anaconda-Server Badge](https://anaconda.org/conda-forge/cyeva/badges/license.svg)](https://anaconda.org/conda-forge/cyeva)
+
 
 cyeva 是一个由彩云科技天气团队开发的用于对气象要素确定性预报准确率进行快速评测的 Python 开源工具库。
 
 cyeva 将致力于让气象要素确定性预报准确率的自动化评估变得简单直接，将集成常用的确定性预报准确率评估指标，且内部算法广泛使用了 numpy 的向量运算实现，对于大数据量的计算也具有较高的计算效率。
 
 ## 安装
```

### Comparing `cyeva-0.1.0b7/cyeva/config/directions/wind.py` & `cyeva-0.1.0b8/cyeva/config/directions/wind.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b7/cyeva/config/levels/precip/__init__.py` & `cyeva-0.1.0b8/cyeva/config/levels/precip/__init__.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b7/cyeva/config/levels/wind/__init__.py` & `cyeva-0.1.0b8/cyeva/config/levels/wind/__init__.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b7/cyeva/core/base.py` & `cyeva-0.1.0b8/cyeva/core/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from ..utils import result_round_digit, source_round_digit
 from .binarize import threshold_binarize
 from .statistic import (
     calc_diff_accuracy_ratio,
     calc_rmse,
     calc_mae,
+    calc_mbe,
     calc_rss,
     calc_chi_square,
     calc_linregress,
     calc_bias_score,
     calc_binary_accuracy_ratio,
 )
 
@@ -69,14 +70,31 @@
         if forecast is None:
             forecast = self.forecast
 
         return calc_mae(observation, forecast)
 
     @result_round_digit(4)
     @source_round_digit()
+    def calc_mbe(
+        self,
+        observation: Union[np.ndarray, list] = None,
+        forecast: Union[np.ndarray, list] = None,
+        *args,
+        **kwargs
+    ) -> float:
+        """Mean Bias Error"""
+        if observation is None:
+            observation = self.observation
+        if forecast is None:
+            forecast = self.forecast
+
+        return calc_mbe(observation, forecast)
+
+    @result_round_digit(4)
+    @source_round_digit()
     def calc_chi_square(
         self,
         observation: Union[np.ndarray, list] = None,
         forecast: Union[np.ndarray, list] = None,
         *args,
         **kwargs
     ) -> float:
```

### Comparing `cyeva-0.1.0b7/cyeva/core/binarize.py` & `cyeva-0.1.0b8/cyeva/core/binarize.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b7/cyeva/core/precip.py` & `cyeva-0.1.0b8/cyeva/core/precip.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b7/cyeva/core/statistic.py` & `cyeva-0.1.0b8/cyeva/core/statistic.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,14 +323,35 @@
     return np.sum(np.abs(observation - forecast)) / len(observation)
 
 
 @assert_length
 @fix_zero_division
 @convert_to_ndarray
 @drop_nan
+def calc_mbe(
+    observation: Union[list, np.ndarray], forecast: Union[list, np.ndarray]
+) -> float:
+    """Calculate MAE(mean absolute error).
+
+    Args:
+        observation (Union[list, np.ndarray]): Binarized observation data array
+                                               that consist of numbers.
+        forecast (Union[list, np.ndarray]): Binarized forecast data array that
+                                            consist of numbers.
+
+    Returns:
+        float: The MAE of forecast to observation.
+    """
+    return np.sum(forecast - observation) / len(observation)
+
+
+@assert_length
+@fix_zero_division
+@convert_to_ndarray
+@drop_nan
 def calc_rss(
     observation: Union[list, np.ndarray], forecast: Union[list, np.ndarray]
 ) -> float:
     """Calculate the residual sum of square between forecast and observation.
 
     Args:
         observation (Union[list, np.ndarray]): Binarized observation data array
@@ -421,14 +442,49 @@
     )
 
     return calc_binary_accuracy_ratio(obs_bins, fct_bins)
 
 
 @assert_length
 @drop_nan
+def calc_threshold_hit_ratio(
+    observation: Union[list, np.ndarray],
+    forecast: Union[list, np.ndarray],
+    threshold: Number,
+    compare: str = ">=",
+) -> float:
+    """Calculate hit ratio of forecast filtered by threshold.
+
+    Args:
+        observation (Union[list, np.ndarray]): Binarized observation data array
+                                               that consist of numbers.
+        forecast (Union[list, np.ndarray]): Binarized forecast data array that
+                                            consist of numbers.
+        threshold (Number): The threshold to filter obervation and forecast.
+                            This parameter should be used with `compare` parameter,
+                            The `compare` parameter will control the logical operator.
+        compare (str, optional): The logical operator applying `threshold` parameter.
+                                * '>' greater
+                                * '<' less
+                                * '>=' greater or equal
+                                * '<=' less or equal
+                                Defaults to '>='.
+
+    Returns:
+        float: The missing ratio of forecast filtered by threshold.
+    """
+    obs_bins, fct_bins = threshold_binarize(
+        observation, forecast, threshold=threshold, compare=compare
+    )
+
+    return calc_hit_ratio(obs_bins, fct_bins)
+
+
+@assert_length
+@drop_nan
 def calc_threshold_miss_ratio(
     observation: Union[list, np.ndarray],
     forecast: Union[list, np.ndarray],
     threshold: Number,
     compare: str = ">=",
 ) -> float:
     """Calculate missing ratio of forecast filtered by threshold.
```

### Comparing `cyeva-0.1.0b7/cyeva/core/temp.py` & `cyeva-0.1.0b8/cyeva/core/temp.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b7/cyeva/core/wind.py` & `cyeva-0.1.0b8/cyeva/core/wind.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,15 +335,15 @@
     if return_index:
         return index
     else:
         return filtered_obs, filtered_fct
 
 
 class WindComparison(Comparison):
-    # FIXME: 需要加最小扇形逻辑
+    # FIXME: 需要加最小扇形逻辑，Issue：#33
     def __init__(
         self,
         obs_spd: Union[np.ndarray, list] = None,
         fct_spd: Union[np.ndarray, list] = None,
         obs_dir: Union[np.ndarray, list] = None,
         fct_dir: Union[np.ndarray, list] = None,
         unit_spd: str = "m/s",
```

### Comparing `cyeva-0.1.0b7/cyeva/utils/decorators.py` & `cyeva-0.1.0b8/cyeva/utils/decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,14 +62,19 @@
 
 
 def drop_nan(func):
     """Drop nan"""
 
     @wraps(func)
     def wrapper(observation, forecast, *args, **kwargs):
+        if not isinstance(observation, np.ndarray):
+            observation = np.array(observation)
+        if not isinstance(forecast, np.ndarray):
+            forecast = np.array(forecast)
+
         where_obs_nan = observation != observation
         where_fct_nan = forecast != forecast
 
         either_nan = where_obs_nan | where_fct_nan
 
         valid_obs = observation[~either_nan]
         valid_fct = forecast[~either_nan]
```

### Comparing `cyeva-0.1.0b7/cyeva.egg-info/PKG-INFO` & `cyeva-0.1.0b8/cyeva.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyeva
-Version: 0.1.0b7
+Version: 0.1.0b8
 Summary: A package to evaluate weather forecast correction
 Home-page: https://github.com/caiyunapp/cyeva
 Author: caiyunapp
 Author-email: oss@caiyunapp.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -30,15 +30,15 @@
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/cyeva/badges/platforms.svg)](https://anaconda.org/conda-forge/cyeva)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/cyeva/badges/latest_release_date.svg)](https://anaconda.org/conda-forge/cyeva)
 [![Pypi](https://badge.fury.io/py/cyeva.svg)](https://badge.fury.io/py/cyeva)
 [![Documentation Status](https://readthedocs.org/projects/cyeva/badge/?version=latest)](https://cyeva.readthedocs.io/zh_CN/latest/?badge=latest)
 [![Download statistic](https://pepy.tech/badge/cyeva)](https://pepy.tech/project/cyeva)
 [![codecov](https://codecov.io/gh/caiyunapp/cyeva/branch/main/graph/badge.svg?token=344FXDKAYD)](https://codecov.io/gh/caiyunapp/cyeva)
 [![style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Anaconda-Server Badge](https://anaconda.org/conda-forge/cyeva/badges/license.svg)](https://anaconda.org/conda-forge/cyeva)
+
 
 cyeva 是一个由彩云科技天气团队开发的用于对气象要素确定性预报准确率进行快速评测的 Python 开源工具库。
 
 cyeva 将致力于让气象要素确定性预报准确率的自动化评估变得简单直接，将集成常用的确定性预报准确率评估指标，且内部算法广泛使用了 numpy 的向量运算实现，对于大数据量的计算也具有较高的计算效率。
 
 ## 安装
```

### Comparing `cyeva-0.1.0b7/cyeva.egg-info/SOURCES.txt` & `cyeva-0.1.0b8/cyeva.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -27,9 +27,10 @@
 requirements/requirements-dev.txt
 requirements/requirements-doc.txt
 requirements/requirements.txt
 tests/test_base.py
 tests/test_binarize.py
 tests/test_errors.py
 tests/test_precip.py
+tests/test_statistic.py
 tests/test_temp.py
 tests/test_wind.py
```

### Comparing `cyeva-0.1.0b7/setup.py` & `cyeva-0.1.0b8/setup.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b7/tests/test_base.py` & `cyeva-0.1.0b8/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b7/tests/test_binarize.py` & `cyeva-0.1.0b8/tests/test_binarize.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b7/tests/test_errors.py` & `cyeva-0.1.0b8/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b7/tests/test_precip.py` & `cyeva-0.1.0b8/tests/test_precip.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b7/tests/test_temp.py` & `cyeva-0.1.0b8/tests/test_temp.py`

 * *Files identical despite different names*

### Comparing `cyeva-0.1.0b7/tests/test_wind.py` & `cyeva-0.1.0b8/tests/test_wind.py`

 * *Files identical despite different names*

