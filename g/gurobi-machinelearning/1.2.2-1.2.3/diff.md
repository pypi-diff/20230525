# Comparing `tmp/gurobi-machinelearning-1.2.2.tar.gz` & `tmp/gurobi-machinelearning-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gurobi-machinelearning-1.2.2.tar", last modified: Mon May 15 15:26:17 2023, max compression
+gzip compressed data, was "gurobi-machinelearning-1.2.3.tar", last modified: Thu May 25 10:39:55 2023, max compression
```

## Comparing `gurobi-machinelearning-1.2.2.tar` & `gurobi-machinelearning-1.2.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:26:17.410841 gurobi-machinelearning-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-15 15:26:17.410841 gurobi-machinelearning-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-15 15:26:17.414841 gurobi-machinelearning-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:26:17.402841 gurobi-machinelearning-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:26:17.406841 gurobi-machinelearning-1.2.2/src/gurobi_machinelearning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-15 15:26:17.000000 gurobi-machinelearning-1.2.2/src/gurobi_machinelearning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-15 15:26:17.000000 gurobi-machinelearning-1.2.2/src/gurobi_machinelearning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:26:17.000000 gurobi-machinelearning-1.2.2/src/gurobi_machinelearning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-15 15:26:17.000000 gurobi-machinelearning-1.2.2/src/gurobi_machinelearning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 15:26:17.000000 gurobi-machinelearning-1.2.2/src/gurobi_machinelearning.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:26:17.406841 gurobi-machinelearning-1.2.2/src/gurobi_ml/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-15 15:26:08.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/add_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:26:17.406841 gurobi-machinelearning-1.2.2/src/gurobi_ml/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/keras/keras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:26:17.406841 gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/_var_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/base_predictor_constr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/get_convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:26:17.406841 gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/neuralnet/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/neuralnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/neuralnet/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/neuralnet/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/neuralnet/neural_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/submodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/register_user_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/registered_predictors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:26:17.410841 gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/base_regressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/column_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/decision_tree_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/gradient_boosting_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/mlpregressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/pls_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/predictors_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/random_forest_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/skgetter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:26:17.410841 gurobi-machinelearning-1.2.2/src/gurobi_ml/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-15 15:26:06.000000 gurobi-machinelearning-1.2.2/src/gurobi_ml/torch/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:39:55.109146 gurobi-machinelearning-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-25 10:39:55.109146 gurobi-machinelearning-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 10:39:55.109146 gurobi-machinelearning-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:39:55.101146 gurobi-machinelearning-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:39:55.101146 gurobi-machinelearning-1.2.3/src/gurobi_machinelearning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-25 10:39:55.000000 gurobi-machinelearning-1.2.3/src/gurobi_machinelearning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-25 10:39:55.000000 gurobi-machinelearning-1.2.3/src/gurobi_machinelearning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 10:39:55.000000 gurobi-machinelearning-1.2.3/src/gurobi_machinelearning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 10:39:55.000000 gurobi-machinelearning-1.2.3/src/gurobi_machinelearning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 10:39:55.000000 gurobi-machinelearning-1.2.3/src/gurobi_machinelearning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:39:55.101146 gurobi-machinelearning-1.2.3/src/gurobi_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-25 10:39:48.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/add_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:39:55.105146 gurobi-machinelearning-1.2.3/src/gurobi_ml/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/keras/keras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:39:55.105146 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/_var_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/base_predictor_constr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/get_convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:39:55.105146 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/neuralnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/neuralnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/neuralnet/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/neuralnet/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/neuralnet/neural_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/submodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/register_user_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/registered_predictors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:39:55.105146 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/base_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/column_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/decision_tree_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/gradient_boosting_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/mlpregressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/pls_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/predictors_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/random_forest_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/skgetter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:39:55.109146 gurobi-machinelearning-1.2.3/src/gurobi_ml/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/torch/sequential.py
```

### Comparing `gurobi-machinelearning-1.2.2/LICENSE` & `gurobi-machinelearning-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/PKG-INFO` & `gurobi-machinelearning-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gurobi-machinelearning
-Version: 1.2.2
+Version: 1.2.3
 Summary: package to insert ML models in Gurobi
 Author: Gurobi Optimization LLC
 Maintainer: Pierre Bonami
 Maintainer-email: bonami@gurobi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Gurobi/gurobi-machinelearning
 Project-URL: Documentation, https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com
```

### Comparing `gurobi-machinelearning-1.2.2/README.md` & `gurobi-machinelearning-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/pyproject.toml` & `gurobi-machinelearning-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gurobi-machinelearning"
-version = "1.2.2"
+version = "1.2.3"
 description = "package to insert ML models in Gurobi"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text="Apache-2.0"}
 keywords = ["mathematical optimization", "gurobi", "scikit-learn", "pytorch", "tensorflow", "ml"]
 authors = [
   {name = "Gurobi Optimization LLC"}
```

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_machinelearning.egg-info/PKG-INFO` & `gurobi-machinelearning-1.2.3/src/gurobi_machinelearning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gurobi-machinelearning
-Version: 1.2.2
+Version: 1.2.3
 Summary: package to insert ML models in Gurobi
 Author: Gurobi Optimization LLC
 Maintainer: Pierre Bonami
 Maintainer-email: bonami@gurobi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Gurobi/gurobi-machinelearning
 Project-URL: Documentation, https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com
```

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_machinelearning.egg-info/SOURCES.txt` & `gurobi-machinelearning-1.2.3/src/gurobi_machinelearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/__init__.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/_version.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from importlib import metadata
 
 try:
     __version__ = metadata.version("gurobi_machinelearning")
 except metadata.PackageNotFoundError:
     __version__ = "dev"
 
-GIT_HASH = "b0b48ccd3327b1517f39adf5b57999e9a36a68b4"
+GIT_HASH = "dec8b6055b1d6cd38bcfb24a0c7d9510b6e4cca1"
 
 
 def get_versions():
     """Get package version."""
     # Downloaded package with inserted git hash.
     if "Format" not in GIT_HASH:
         git_hash = f"-{GIT_HASH}"
```

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/add_predictor.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/add_predictor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/exceptions.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/keras/__init__.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/keras/keras.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/keras/keras.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/__init__.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/_var_utils.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/_var_utils.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/base_predictor_constr.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/base_predictor_constr.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/get_convertor.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/get_convertor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/neuralnet/__init__.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/neuralnet/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/neuralnet/activations.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/neuralnet/activations.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/neuralnet/layers.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/neuralnet/layers.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/neuralnet/neural_net.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/neuralnet/neural_net.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/modeling/submodel.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/submodel.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/register_user_predictor.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/register_user_predictor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/registered_predictors.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/registered_predictors.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/__init__.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/base_regressions.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/base_regressions.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/column_transformer.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/column_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,19 +68,23 @@
             if trans == "passthrough":
                 if isinstance(cols, str) or isinstance(cols[0], str):
                     transformed.append(_input.loc[:, cols])
                 else:
                     if hasattr(_input, "iloc"):
                         transformed.append(_input.iloc[:, cols])
                     else:
-                        data = _input[:, cols]
+                        data = _input
+                        if data.ndim == 1:
+                            # If we have a one-dimensional numpy array reshape it.
+                            # By definition pandas dataframe should be 2-dimensional
+                            data = data.reshape(1, -1)
                         if isinstance(data, gp.MVar):
-                            transformed.append(_input[:, cols].tolist())
+                            transformed.append(data[:, cols].tolist())
                         else:
-                            transformed.append(_input[:, cols])
+                            transformed.append(data[:, cols])
             elif trans == "drop":
                 pass
             else:
                 if isinstance(cols, str) or isinstance(cols[0], str):
                     data = _input.loc[:, cols]
                     any_var = any(
                         map(lambda i: isinstance(i, gp.Var), data.to_numpy().ravel())
@@ -90,15 +94,20 @@
                         data = _input.iloc[:, cols]
                         any_var = any(
                             map(
                                 lambda i: isinstance(i, gp.Var), data.to_numpy().ravel()
                             )
                         )
                     else:
-                        data = _input[:, cols]
+                        data = _input
+                        if data.ndim == 1:
+                            # If we have a one-dimensional numpy array reshape it.
+                            # By definition pandas dataframe should be 2-dimensional
+                            data = data.reshape(1, -1)
+                        data = data[:, cols]
                         any_var = True
                 if any_var:
                     try:
                         trans_constr = transformers[name](self._gp_model, trans, data)
                     except KeyError:
                         raise NoModel(name, "No implementation found")
                     transformed.append(trans_constr.output.tolist())
```

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/decision_tree_regressor.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/gradient_boosting_regressor.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/gradient_boosting_regressor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/linear_regression.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/linear_regression.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/logistic_regression.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/mlpregressor.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/mlpregressor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/pipeline.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/pls_regression.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/pls_regression.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/predictors_list.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/predictors_list.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/preprocessing.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/random_forest_regressor.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/random_forest_regressor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/sklearn/skgetter.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/skgetter.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/torch/__init__.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.2/src/gurobi_ml/torch/sequential.py` & `gurobi-machinelearning-1.2.3/src/gurobi_ml/torch/sequential.py`

 * *Files identical despite different names*

