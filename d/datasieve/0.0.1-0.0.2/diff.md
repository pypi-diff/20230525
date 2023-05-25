# Comparing `tmp/datasieve-0.0.1.tar.gz` & `tmp/datasieve-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasieve-0.0.1.tar", max compression
+gzip compressed data, was "datasieve-0.0.2.tar", max compression
```

## Comparing `datasieve-0.0.1.tar` & `datasieve-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1059 2023-05-25 13:22:18.715702 datasieve-0.0.1/LICENSE
--rw-r--r--   0        0        0     6162 2023-05-25 13:01:32.371608 datasieve-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-25 12:33:12.836729 datasieve-0.0.1/datasieve/__init__.py
--rw-r--r--   0        0        0     6059 2023-05-25 12:33:45.700647 datasieve-0.0.1/datasieve/pipeline.py
--rw-r--r--   0        0        0      575 2023-05-25 12:50:22.661676 datasieve-0.0.1/datasieve/transforms/__init__.py
--rw-r--r--   0        0        0     5458 2023-05-25 12:45:29.750610 datasieve-0.0.1/datasieve/transforms/dbscan.py
--rw-r--r--   0        0        0     2874 2023-05-25 12:38:23.699896 datasieve-0.0.1/datasieve/transforms/dissimilarity_index.py
--rw-r--r--   0        0        0     1158 2023-05-25 12:48:33.926026 datasieve-0.0.1/datasieve/transforms/minmax_scaler.py
--rw-r--r--   0        0        0     1553 2023-05-25 12:39:53.967634 datasieve-0.0.1/datasieve/transforms/pca.py
--rw-r--r--   0        0        0     1502 2023-05-25 12:36:20.980240 datasieve-0.0.1/datasieve/transforms/svm_outlier_extractor.py
--rw-r--r--   0        0        0     1305 2023-05-25 12:50:35.305635 datasieve-0.0.1/datasieve/transforms/variance_threshold.py
--rw-r--r--   0        0        0     2999 2023-05-25 12:37:08.608108 datasieve-0.0.1/datasieve/utils.py
--rw-r--r--   0        0        0      523 2023-05-25 13:17:54.760555 datasieve-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     7057 1970-01-01 00:00:00.000000 datasieve-0.0.1/setup.py
--rw-r--r--   0        0        0     6800 1970-01-01 00:00:00.000000 datasieve-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-05-25 13:22:18.715702 datasieve-0.0.2/LICENSE
+-rw-r--r--   0        0        0     9987 2023-05-25 14:11:51.276521 datasieve-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-25 12:33:12.836729 datasieve-0.0.2/datasieve/__init__.py
+-rw-r--r--   0        0        0     6059 2023-05-25 12:33:45.700647 datasieve-0.0.2/datasieve/pipeline.py
+-rw-r--r--   0        0        0      575 2023-05-25 12:50:22.661676 datasieve-0.0.2/datasieve/transforms/__init__.py
+-rw-r--r--   0        0        0     5458 2023-05-25 12:45:29.750610 datasieve-0.0.2/datasieve/transforms/dbscan.py
+-rw-r--r--   0        0        0     2874 2023-05-25 12:38:23.699896 datasieve-0.0.2/datasieve/transforms/dissimilarity_index.py
+-rw-r--r--   0        0        0     1158 2023-05-25 12:48:33.926026 datasieve-0.0.2/datasieve/transforms/minmax_scaler.py
+-rw-r--r--   0        0        0     1553 2023-05-25 12:39:53.967634 datasieve-0.0.2/datasieve/transforms/pca.py
+-rw-r--r--   0        0        0     1502 2023-05-25 12:36:20.980240 datasieve-0.0.2/datasieve/transforms/svm_outlier_extractor.py
+-rw-r--r--   0        0        0     1305 2023-05-25 12:50:35.305635 datasieve-0.0.2/datasieve/transforms/variance_threshold.py
+-rw-r--r--   0        0        0     2999 2023-05-25 12:37:08.608108 datasieve-0.0.2/datasieve/utils.py
+-rw-r--r--   0        0        0      522 2023-05-25 14:20:54.206414 datasieve-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    10959 1970-01-01 00:00:00.000000 datasieve-0.0.2/setup.py
+-rw-r--r--   0        0        0    10675 1970-01-01 00:00:00.000000 datasieve-0.0.2/PKG-INFO
```

### Comparing `datasieve-0.0.1/LICENSE` & `datasieve-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.1/README.md` & `datasieve-0.0.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -99,14 +99,91 @@
 
 Finally, similar to SKLearn's pipeline, the `feature_pipeline` can be used to inverse_transform an array `X3` array that has the same dimensions as the returned `X` array from the pipeline:
 
 ```python
 Xinv, _ ,_ = feature_pipeline.inverse_transform(X)
 ```
 
+## Data removal
+
+The command `feature_pipeline.fit_transform(X, y, sample_weight)` fits each pipeline step to `X`, and transforms `X` according to each step's `transform()` method. In some cases, this will not affect `y` or `sample_weight`. For example, `FlowdaptMinMaxScaler` simply scales `X` and saves the normalization information.  Meanwhile, in the `SVMOutlierExtractor`, `.fit()` will fit an SVM to `X` and `.transform()` will remove any detected outliers from `X`. Typical `Scikit-Learn` pipelines do not remove those data points from `y` and `sample_weight`. Luckily, the `FlowdaptPipeline` takes care of the "associated removal" of the same outlier data points from `y` and `sample_weight`. 
+
+## Feature modification
+
+Another feature is demonstrated in the `FlowdaptPCA`, which fits a PCA transform to `X` and then transforms `X` to principal components. This dimensionality reduction means that the features are no longer the same, instead they are now `PC1`, `PC2` ... `PCX`. `FlowdaptPipeline` handles the feature renaming at that step (which is not a feature available in the `Scikit-Learn` pipeline). Similar to `FlowdaptPCA`, the `FlowdaptVarianceThreshold` subclasses the `Scikit-Learn` `VarianceThreshold` which is geared toward removing features that have a low variance. `FlowdaptVarianceThreshold` ensures that the removed features are properly handled when `X` passes through this part of the pipeline.
+
+## Adding a custom step
+
+Each step of the `Pipeline` *must* contain the following methods:
+
+```python
+class MyTransformer:
+    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        X, y, sample_weight = self.fit(X, y, sample_weight)
+        X, y, sample_weight = self.transform(X, y, sample_weight)
+        return X, y, sample_weight, feature_list
+
+    def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        return X, y, sample_weight, feature_list
+
+    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        return X, y, sample_weight, feature_list
+
+    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        return X, y, sample_weight, feature_list
+```
+
+This is because these four methods are called automatically by the `Pipeline` object. In most cases, the goal is to add functionality for an existing transformer from the `Scikit-Learn` library. Here is an example of subclassing the `MinMaxScaler` to work with the `FlowdaptPipeline`:
+
+```python
+class DataSieveMinMaxScaler(MinMaxScaler):
+    """
+    A subclass of the SKLearn MinMaxScaler that ensures fit, transform, fit_transform and
+    inverse_transform all take the full set of params X, y, sample_weight (even if they
+    are unused) to follow the FlowdaptPipeline API.
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        super().fit(X)
+        X = super().transform(X)
+        return X, y, sample_weight, feature_list
+
+    def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        super().fit(X)
+        return X, y, sample_weight, feature_list
+
+    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        X = super().transform(X)
+        return X, y, sample_weight, feature_list
+
+    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        return super().inverse_transform(X), y, sample_weight, feature_list
+```
+
+
+
+# Installation
+
+The easiest way to install `datasieve` is with:
+
+```
+pip install datasieve
+```
+
+but you can also clone this repository and install it with:
+
+```
+git clone https://github.com/emergentmethods/datasieve.git
+cd datasieve
+poetry install
+```
+
 
 # License
 
 Copyright (c) 2023 DataSieve
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
```

### Comparing `datasieve-0.0.1/datasieve/pipeline.py` & `datasieve-0.0.2/datasieve/pipeline.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.1/datasieve/transforms/__init__.py` & `datasieve-0.0.2/datasieve/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.1/datasieve/transforms/dbscan.py` & `datasieve-0.0.2/datasieve/transforms/dbscan.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.1/datasieve/transforms/dissimilarity_index.py` & `datasieve-0.0.2/datasieve/transforms/dissimilarity_index.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.1/datasieve/transforms/minmax_scaler.py` & `datasieve-0.0.2/datasieve/transforms/minmax_scaler.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.1/datasieve/transforms/pca.py` & `datasieve-0.0.2/datasieve/transforms/pca.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.1/datasieve/transforms/svm_outlier_extractor.py` & `datasieve-0.0.2/datasieve/transforms/svm_outlier_extractor.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.1/datasieve/transforms/variance_threshold.py` & `datasieve-0.0.2/datasieve/transforms/variance_threshold.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.1/datasieve/utils.py` & `datasieve-0.0.2/datasieve/utils.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.1/pyproject.toml` & `datasieve-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "datasieve"
-version = "0.0.1"
+version = "0.0.2"
 description = "This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)"
 authors = ['Robert Caulk']
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<4.0"
 scikit-learn = "^1.2.0"
 pandas = "^1.3.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.1"
 autopep8 = "1.6.0"
```

### Comparing `datasieve-0.0.1/PKG-INFO` & `datasieve-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: datasieve
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)
 License: MIT
 Author: Robert Caulk
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=1.3.3,<2.0.0)
 Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # DataSieve
 
 DataSieve is very similar to the SKlearn Pipeline in that it:
@@ -115,14 +116,91 @@
 
 Finally, similar to SKLearn's pipeline, the `feature_pipeline` can be used to inverse_transform an array `X3` array that has the same dimensions as the returned `X` array from the pipeline:
 
 ```python
 Xinv, _ ,_ = feature_pipeline.inverse_transform(X)
 ```
 
+## Data removal
+
+The command `feature_pipeline.fit_transform(X, y, sample_weight)` fits each pipeline step to `X`, and transforms `X` according to each step's `transform()` method. In some cases, this will not affect `y` or `sample_weight`. For example, `FlowdaptMinMaxScaler` simply scales `X` and saves the normalization information.  Meanwhile, in the `SVMOutlierExtractor`, `.fit()` will fit an SVM to `X` and `.transform()` will remove any detected outliers from `X`. Typical `Scikit-Learn` pipelines do not remove those data points from `y` and `sample_weight`. Luckily, the `FlowdaptPipeline` takes care of the "associated removal" of the same outlier data points from `y` and `sample_weight`. 
+
+## Feature modification
+
+Another feature is demonstrated in the `FlowdaptPCA`, which fits a PCA transform to `X` and then transforms `X` to principal components. This dimensionality reduction means that the features are no longer the same, instead they are now `PC1`, `PC2` ... `PCX`. `FlowdaptPipeline` handles the feature renaming at that step (which is not a feature available in the `Scikit-Learn` pipeline). Similar to `FlowdaptPCA`, the `FlowdaptVarianceThreshold` subclasses the `Scikit-Learn` `VarianceThreshold` which is geared toward removing features that have a low variance. `FlowdaptVarianceThreshold` ensures that the removed features are properly handled when `X` passes through this part of the pipeline.
+
+## Adding a custom step
+
+Each step of the `Pipeline` *must* contain the following methods:
+
+```python
+class MyTransformer:
+    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        X, y, sample_weight = self.fit(X, y, sample_weight)
+        X, y, sample_weight = self.transform(X, y, sample_weight)
+        return X, y, sample_weight, feature_list
+
+    def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        return X, y, sample_weight, feature_list
+
+    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        return X, y, sample_weight, feature_list
+
+    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        return X, y, sample_weight, feature_list
+```
+
+This is because these four methods are called automatically by the `Pipeline` object. In most cases, the goal is to add functionality for an existing transformer from the `Scikit-Learn` library. Here is an example of subclassing the `MinMaxScaler` to work with the `FlowdaptPipeline`:
+
+```python
+class DataSieveMinMaxScaler(MinMaxScaler):
+    """
+    A subclass of the SKLearn MinMaxScaler that ensures fit, transform, fit_transform and
+    inverse_transform all take the full set of params X, y, sample_weight (even if they
+    are unused) to follow the FlowdaptPipeline API.
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        super().fit(X)
+        X = super().transform(X)
+        return X, y, sample_weight, feature_list
+
+    def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        super().fit(X)
+        return X, y, sample_weight, feature_list
+
+    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        X = super().transform(X)
+        return X, y, sample_weight, feature_list
+
+    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        return super().inverse_transform(X), y, sample_weight, feature_list
+```
+
+
+
+# Installation
+
+The easiest way to install `datasieve` is with:
+
+```
+pip install datasieve
+```
+
+but you can also clone this repository and install it with:
+
+```
+git clone https://github.com/emergentmethods/datasieve.git
+cd datasieve
+poetry install
+```
+
 
 # License
 
 Copyright (c) 2023 DataSieve
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
```

