# Comparing `tmp/pyheartlib-0.0.2.tar.gz` & `tmp/pyheartlib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyheartlib-0.0.2.tar", max compression
+gzip compressed data, was "pyheartlib-0.0.6.tar", max compression
```

## Comparing `pyheartlib-0.0.2.tar` & `pyheartlib-0.0.6.tar`

### file list

```diff
@@ -1,38 +1,19 @@
--rw-r--r--   0        0        0       59 2023-05-22 17:25:45.393222 pyheartlib-0.0.2/LICENSE
--rw-r--r--   0        0        0     1707 2023-05-22 17:25:45.393222 pyheartlib-0.0.2/README.md
--rw-r--r--   0        0        0     1408 2023-05-22 17:27:19.694561 pyheartlib-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      112 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/__init__.py
--rw-r--r--   0        0        0       54 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/__init__.py
--rw-r--r--   0        0        0     3925 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/arr_conv1d.py
--rw-r--r--   0        0        0     9430 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/beat_Anomaly_mhb.pyy
--rw-r--r--   0        0        0     1618 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/beat_anomaly_FCN.py
--rw-r--r--   0        0        0     1953 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/beat_anomaly_conv1d.py
--rw-r--r--   0        0        0     2244 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/beat_anomaly_conv2d.py
--rw-r--r--   0        0        0     3902 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/beat_conv1D.py
--rw-r--r--   0        0        0     4910 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/beat_conv1d_rri.py
--rw-r--r--   0        0        0     2652 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/beat_conv1d_rri_paral.py
--rw-r--r--   0        0        0     2891 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/beat_conv2d_rri.py
--rw-r--r--   0        0        0     1549 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/beat_model.py
--rw-r--r--   0        0        0       54 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/old/__init__.py
--rw-r--r--   0        0        0     7495 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/old/modelM1.py
--rw-r--r--   0        0        0     8026 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/old/modelM1_ab1.py
--rw-r--r--   0        0        0     8034 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/old/modelM1_ab2.py
--rw-r--r--   0        0        0     8433 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/old/model_with_one_mhb-ORIGINAL.py
--rw-r--r--   0        0        0     8957 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/old/model_with_one_mhb.py
--rw-r--r--   0        0        0     2166 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/rpeak1.py
--rw-r--r--   0        0        0     2694 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/rpeak2.py
--rw-r--r--   0        0        0     3921 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/archs/rpeak3.py
--rw-r--r--   0        0        0    18725 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/beat_info.py
--rw-r--r--   0        0        0     1160 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/config.yaml
--rw-r--r--   0        0        0     5349 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/data.py
--rw-r--r--   0        0        0     9295 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/data_arrhythmia.py
--rw-r--r--   0        0        0    22880 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/data_beat.py
--rw-r--r--   0        0        0     9605 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/data_rpeak.py
--rw-r--r--   0        0        0       39 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/extra/__init__.py
--rw-r--r--   0        0        0     4176 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/extra/pqrst.py
--rw-r--r--   0        0        0     2827 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/extra/report.py
--rw-r--r--   0        0        0     5887 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/extra/utils.py
--rw-r--r--   0        0        0     5866 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/features.py
--rw-r--r--   0        0        0     2579 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/io.py
--rw-r--r--   0        0        0     8796 2023-05-22 17:25:45.405222 pyheartlib-0.0.2/src/pyheartlib/processing.py
--rw-r--r--   0        0        0     2351 1970-01-01 00:00:00.000000 pyheartlib-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-05-25 08:38:53.575999 pyheartlib-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2438 2023-05-25 08:38:53.575999 pyheartlib-0.0.6/README.md
+-rw-r--r--   0        0        0     1412 2023-05-25 08:40:33.947862 pyheartlib-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/__init__.py
+-rw-r--r--   0        0        0       54 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/archs/__init__.py
+-rw-r--r--   0        0        0    18725 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/beat_info.py
+-rw-r--r--   0        0        0     1160 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/config.yaml
+-rw-r--r--   0        0        0     5349 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/data.py
+-rw-r--r--   0        0        0     9295 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/data_arrhythmia.py
+-rw-r--r--   0        0        0    22880 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/data_beat.py
+-rw-r--r--   0        0        0     9605 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/data_rpeak.py
+-rw-r--r--   0        0        0       39 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/extra/__init__.py
+-rw-r--r--   0        0        0     4176 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/extra/pqrst.py
+-rw-r--r--   0        0        0     2827 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/extra/report.py
+-rw-r--r--   0        0        0     5887 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/extra/utils.py
+-rw-r--r--   0        0        0     5866 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/features.py
+-rw-r--r--   0        0        0     2579 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/io.py
+-rw-r--r--   0        0        0     8796 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/processing.py
+-rw-r--r--   0        0        0     3088 1970-01-01 00:00:00.000000 pyheartlib-0.0.6/PKG-INFO
```

### Comparing `pyheartlib-0.0.2/pyproject.toml` & `pyheartlib-0.0.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "pyheartlib"
-version = "0.0.2"
+version = "0.0.6"
 description = "A Python package for processing and modeling electrocardiogram signals"
 authors = ["Sadegh Mohammadi"]
 license = "Proprietary"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.10.4,<3.12"
-numpy = "^1.24.1"
-pandas = "^1.5.3"
-tqdm = "^4.64.1"
-wfdb = "^4.1.0"
-tensorflow = "^2.11.0"
-scikit-learn = "^1.2.2"
+python = ">=3.10,<3.12"
+numpy = ">=1.22.0"
+wfdb = ">=4.0.0"
+pandas = ">=1.4.0"
+tqdm = ">=4.63.0"
+scikit-learn = ">=1.1.0"
+tensorflow = ">=2.8.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.1"
-pytest-cov = "^4.0.0"
-black = "^23.1.0"
-myst-nb = "^0.17.1"
-sphinx-autoapi = "^2.0.1"
-sphinx-rtd-theme = "^1.1.1"
-third-party-license-file-generator = "^2022.3.1"
+pytest = "^7.3.1"
+pytest-cov = "^4.1.0"
+black = "^23.3.0"
+myst-nb = "^0.17.2"
+sphinx-autoapi = "^2.1.0"
+sphinx-rtd-theme = "^1.2.1"
+third-party-license-file-generator = "^2023.2.22"
 flake8 = "^6.0.0"
 python-semantic-release = "^7.33.5"
 
 [tool.semantic_release]
 version_variable = "pyproject.toml:version" # version location
 branch = "main"                             # branch to make releases of
 changelog_file = "CHANGELOG.md"             # changelog file
```

### Comparing `pyheartlib-0.0.2/src/pyheartlib/beat_info.py` & `pyheartlib-0.0.6/src/pyheartlib/beat_info.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.2/src/pyheartlib/config.yaml` & `pyheartlib-0.0.6/src/pyheartlib/config.yaml`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.2/src/pyheartlib/data.py` & `pyheartlib-0.0.6/src/pyheartlib/data.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.2/src/pyheartlib/data_arrhythmia.py` & `pyheartlib-0.0.6/src/pyheartlib/data_arrhythmia.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.2/src/pyheartlib/data_beat.py` & `pyheartlib-0.0.6/src/pyheartlib/data_beat.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.2/src/pyheartlib/data_rpeak.py` & `pyheartlib-0.0.6/src/pyheartlib/data_rpeak.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.2/src/pyheartlib/extra/pqrst.py` & `pyheartlib-0.0.6/src/pyheartlib/extra/pqrst.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.2/src/pyheartlib/extra/report.py` & `pyheartlib-0.0.6/src/pyheartlib/extra/report.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.2/src/pyheartlib/extra/utils.py` & `pyheartlib-0.0.6/src/pyheartlib/extra/utils.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.2/src/pyheartlib/features.py` & `pyheartlib-0.0.6/src/pyheartlib/features.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.2/src/pyheartlib/io.py` & `pyheartlib-0.0.6/src/pyheartlib/io.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.2/src/pyheartlib/processing.py` & `pyheartlib-0.0.6/src/pyheartlib/processing.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.2/PKG-INFO` & `pyheartlib-0.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,63 @@
 Metadata-Version: 2.1
 Name: pyheartlib
-Version: 0.0.2
+Version: 0.0.6
 Summary: A Python package for processing and modeling electrocardiogram signals
 License: Proprietary
 Author: Sadegh Mohammadi
-Requires-Python: >=3.10.4,<3.12
+Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (>=1.24.1,<2.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
-Requires-Dist: tensorflow (>=2.11.0,<3.0.0)
-Requires-Dist: tqdm (>=4.64.1,<5.0.0)
-Requires-Dist: wfdb (>=4.1.0,<5.0.0)
+Requires-Dist: numpy (>=1.22.0)
+Requires-Dist: pandas (>=1.4.0)
+Requires-Dist: scikit-learn (>=1.1.0)
+Requires-Dist: tensorflow (>=2.8.0)
+Requires-Dist: tqdm (>=4.63.0)
+Requires-Dist: wfdb (>=4.0.0)
 Description-Content-Type: text/markdown
 
 # pyheartlib
 
+[![Documentation Status](https://readthedocs.org/projects/pyheartlib/badge/?version=latest)](https://pyheartlib.readthedocs.io/en/latest/?badge=latest)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyheartlib)
+[![codecov](https://codecov.io/gh/sadeghmdi/pyheartlib/branch/main/graph/badge.svg?token=6IB18KL3E9)](https://codecov.io/gh/sadeghmdi/pyheartlib)
+![PyPI](https://img.shields.io/pypi/v/pyheartlib?color=blue)
+
+
 pyheartlib is a Python package for processing and modeling electrocardiogram signals. This package facilitates processing signals for the task such as heartbeat detection, heartbeat classification, and arrhythmia classification. By using it, researchers can focus on these tasks without the burden of designing data processing modules. The package supports both raw signals and computed features for model building. Therefore traditional machine learning models and more advanced deep learning models can be used. The first release of this software supports Keras and Tensorflow libraries, and MIT-BIH Arrhythmia Database format. The package has optional preprocessing methods to remove noise and baseline wander from the raw signals.
 
 # Installation
 
 The package can be installed with pip:
 
 ```bash
 $ pip install pyheartlib
 ```
 
-# Requirements
-
-pyheartlib has been tested on Ubuntu, Python 3.11 and the depends on the packages.
+# Dependencies
 
-* numpy>=1.21.1
-* pandas>=1.3.1
+* python = ">=3.10,<3.12"
+* numpy = ">=1.22.0"
+* wfdb = ">=4.0.0"
+* pandas = ">=1.4.0"
+* tqdm = ">=4.63.0"
+* scikit-learn = ">=1.1.0"
+* tensorflow = ">=2.8.0"
 
 # Documentation
 
 Check out the [documentation](https://pyheartlib.readthedocs.io) for more information.
 
 # Examples
 
 Following examples demostrate dataset creation:
 
-* [Inter-patient dataset](examples/make_dataset_inter.py) <br>
-* [Intra-patient dataset](examples/make_dataset_intra.py) <br>
-* [Rpeak dataset](examples/make_dataset_rpeak.py) <br>
-* [Arrhythmia dataset](examples/make_dataset_arrhythmia.py) <br>
+* [Inter-patient dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/make_dataset_inter.py) <br>
+* [Intra-patient dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/make_dataset_intra.py) <br>
+* [Rpeak dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/make_dataset_rpeak.py) <br>
+* [Arrhythmia dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/make_dataset_arrhythmia.py) <br>
 
-As an example, a deep learning model was designed using Keras library for the heartbeat detection task. Because this task is less complex compared to the heartbeat and arrhythmia classification tasks, it can be trained with high accuracy using the available public datasets.
+As an example, a deep learning model was designed using Keras library for the heartbeat detection task. Because this task is less complex compared to the heartbeat and arrhythmia classification tasks, it can be trained with high accuracy using the available public datasets. 
 
-* [Beat detection model](model/README.md)
+* [Beat detection model](https://github.com/sadeghmdi/pyheartlib/blob/main/model/README.md)
```

