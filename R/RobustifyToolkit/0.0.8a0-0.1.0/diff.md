# Comparing `tmp/RobustifyToolkit-0.0.8a0.tar.gz` & `tmp/RobustifyToolkit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobustifyToolkit-0.0.8a0.tar", last modified: Thu May 25 16:48:02 2023, max compression
+gzip compressed data, was "RobustifyToolkit-0.1.0.tar", last modified: Thu May 25 20:27:30 2023, max compression
```

## Comparing `RobustifyToolkit-0.0.8a0.tar` & `RobustifyToolkit-0.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:48:02.798044 RobustifyToolkit-0.0.8a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-25 16:48:02.798044 RobustifyToolkit-0.0.8a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:48:02.794044 RobustifyToolkit-0.0.8a0/RobustifyToolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-25 16:48:02.000000 RobustifyToolkit-0.0.8a0/RobustifyToolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-25 16:48:02.000000 RobustifyToolkit-0.0.8a0/RobustifyToolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:48:02.000000 RobustifyToolkit-0.0.8a0/RobustifyToolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 16:48:02.000000 RobustifyToolkit-0.0.8a0/RobustifyToolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 16:48:02.000000 RobustifyToolkit-0.0.8a0/RobustifyToolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:48:02.794044 RobustifyToolkit-0.0.8a0/robustify/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:48:02.794044 RobustifyToolkit-0.0.8a0/robustify/noise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/noise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/noise/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/noise/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/noiseCorruptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:48:02.798044 RobustifyToolkit-0.0.8a0/robustify/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/_importances.py
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/_scorers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/robustify/utils/_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 16:48:02.798044 RobustifyToolkit-0.0.8a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:48:02.798044 RobustifyToolkit-0.0.8a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/tests/test_gaussianNoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/tests/test_poissonNoise.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/tests/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/tests/test_scikt-learn_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-05-25 16:47:53.000000 RobustifyToolkit-0.0.8a0/tests/test_tensorflow_keras_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:30.421832 RobustifyToolkit-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-05-25 20:27:30.421832 RobustifyToolkit-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:30.417832 RobustifyToolkit-0.1.0/RobustifyToolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-05-25 20:27:30.000000 RobustifyToolkit-0.1.0/RobustifyToolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-25 20:27:30.000000 RobustifyToolkit-0.1.0/RobustifyToolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:27:30.000000 RobustifyToolkit-0.1.0/RobustifyToolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 20:27:30.000000 RobustifyToolkit-0.1.0/RobustifyToolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 20:27:30.000000 RobustifyToolkit-0.1.0/RobustifyToolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:30.417832 RobustifyToolkit-0.1.0/robustify/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:30.417832 RobustifyToolkit-0.1.0/robustify/noise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/noise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/noise/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/noise/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/noise_corruptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:30.421832 RobustifyToolkit-0.1.0/robustify/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/_importances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/_scorers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/robustify/utils/_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 20:27:30.421832 RobustifyToolkit-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:30.421832 RobustifyToolkit-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/tests/test_gaussianNoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/tests/test_poissonNoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/tests/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/tests/test_scikt-learn_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-25 20:27:14.000000 RobustifyToolkit-0.1.0/tests/test_tensorflow_keras_compatibility.py
```

### Comparing `RobustifyToolkit-0.0.8a0/LICENSE` & `RobustifyToolkit-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.0.8a0/PKG-INFO` & `RobustifyToolkit-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobustifyToolkit
-Version: 0.0.8a0
+Version: 0.1.0
 Summary: Robustify:
 Author: Isabel Foster
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -65,15 +65,15 @@
 
 ## Examples
 ### Keras
 ### Pytorch
 ### Scikit-learn
 
 ## Documentation
-See the [Wiki][1] for documentation of the availabel methods. 
+See the [Wiki][1] for documentation of the available methods. 
 
 License is MIT.
 
 [1]: https://github.com/IsaFoster/robustify/wiki
 [2]: https://scikit-learn.org/stable/index.html
 [3]: https://scikit-learn.org/stable/modules/generated/sklearn.inspection.permutation_importance.html
 [4]: https://github.com/TeamHG-Memex/eli5
```

### Comparing `RobustifyToolkit-0.0.8a0/README.md` & `RobustifyToolkit-0.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 ## Examples
 ### Keras
 ### Pytorch
 ### Scikit-learn
 
 ## Documentation
-See the [Wiki][1] for documentation of the availabel methods. 
+See the [Wiki][1] for documentation of the available methods. 
 
 License is MIT.
 
 [1]: https://github.com/IsaFoster/robustify/wiki
 [2]: https://scikit-learn.org/stable/index.html
 [3]: https://scikit-learn.org/stable/modules/generated/sklearn.inspection.permutation_importance.html
 [4]: https://github.com/TeamHG-Memex/eli5
```

### Comparing `RobustifyToolkit-0.0.8a0/RobustifyToolkit.egg-info/PKG-INFO` & `RobustifyToolkit-0.1.0/RobustifyToolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobustifyToolkit
-Version: 0.0.8a0
+Version: 0.1.0
 Summary: Robustify:
 Author: Isabel Foster
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -65,15 +65,15 @@
 
 ## Examples
 ### Keras
 ### Pytorch
 ### Scikit-learn
 
 ## Documentation
-See the [Wiki][1] for documentation of the availabel methods. 
+See the [Wiki][1] for documentation of the available methods. 
 
 License is MIT.
 
 [1]: https://github.com/IsaFoster/robustify/wiki
 [2]: https://scikit-learn.org/stable/index.html
 [3]: https://scikit-learn.org/stable/modules/generated/sklearn.inspection.permutation_importance.html
 [4]: https://github.com/TeamHG-Memex/eli5
```

### Comparing `RobustifyToolkit-0.0.8a0/RobustifyToolkit.egg-info/SOURCES.txt` & `RobustifyToolkit-0.1.0/RobustifyToolkit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 setup.py
 RobustifyToolkit.egg-info/PKG-INFO
 RobustifyToolkit.egg-info/SOURCES.txt
 RobustifyToolkit.egg-info/dependency_links.txt
 RobustifyToolkit.egg-info/requires.txt
 RobustifyToolkit.egg-info/top_level.txt
 robustify/__init__.py
-robustify/noiseCorruptions.py
+robustify/noise_corruptions.py
 robustify/noise/__init__.py
 robustify/noise/continuous.py
 robustify/noise/discrete.py
 robustify/utils/__init__.py
 robustify/utils/_filter.py
 robustify/utils/_importances.py
 robustify/utils/_plot.py
```

### Comparing `RobustifyToolkit-0.0.8a0/robustify/noise/continuous.py` & `RobustifyToolkit-0.1.0/robustify/noise/continuous.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,36 @@
+
 import numpy as np
 import pandas as pd
 
-def gaussian_Noise(clean_data, percentage, feature_name=None, random_state=None):
+def gaussian_noise(clean_data, percentage, feature_name=None, random_state=None):
     """
     Parameters:
     ----------
         clean_data: ndarray or dataframe of shape (n_samples, n_features)
-            Array of the feature values that will be permuted. If dataframe, feature_name is required to determine which feature the noise should be applied to. .
+            Array of the feature values that will be permuted. If dataframe,
+            feature_name is required to determine which feature the noise should
+            be applied to. .
         percentage: float
-            Percentage of change in noise over signal that should be added (on average) when permuting the feature.
+            Percentage of change in noise over signal that should be added (on
+            average) when permuting the feature.
         feature_name: str, deafult=None
-            If clean_data is a dataframe feature name is required to determine which feature will be permuted.
+            If clean_data is a dataframe feature name is required to determine
+            which feature will be permuted.
         random_state: int, RandomState instance or None, deafult=None
             Controls randomness in drawing from the distribution.
     Returns:  
     ----------    
         result: ndarray or dataframe of shape (n_samples, n_features)
-            Array or dataframe (depends on input format) with the noisy feature permuted.
+            Array or dataframe (depends on input format) with the noisy feature
+            permuted.
     """
     np.random.seed(random_state)
-    if (isinstance(clean_data, pd.DataFrame)):
+    if isinstance(clean_data, pd.DataFrame):
         data_col = clean_data[feature_name]
         noise = (data_col * percentage) * np.random.normal(0, 1, len(data_col))
         clean_data[feature_name] = data_col + noise
         return clean_data
-    if (isinstance(clean_data, (np.ndarray, np.generic, list))):
+    if isinstance(clean_data, (np.ndarray, np.generic, list)):
         noise = (clean_data * percentage) * np.random.normal(0, 1, len(clean_data))
         return clean_data + noise
```

### Comparing `RobustifyToolkit-0.0.8a0/robustify/noise/discrete.py` & `RobustifyToolkit-0.1.0/robustify/noise/discrete.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,71 @@
+
 import numpy as np
 import pandas as pd
 
 def binomial_noise(clean_data, level, feature_name=None, random_state=None):
     """
     Parameters:
     ----------
     clean_data: ndarray or dataframe of shape (n_samples, n_features)
-        Array of the feature values that will be permuted. If dataframe, feature_name is required to determine which feature the noise should be applied to. .
+        Array of the feature values that will be permuted. If dataframe,
+        feature_name is required to determine which feature the noise should be
+        applied to. .
     level: float
-        The probability of each value to be permuted. If 0, feature is returned without changes. If 1, every value is flipped.
+        The probability of each value to be permuted. If 0, feature is returned
+        without changes. If 1, every value is flipped.
     feature_name: str, deafult=None
-        If clean_data is a dataframe feature name is required to determine which feature will be permuted.
+        If clean_data is a dataframe feature name is required to determine which
+        feature will be permuted.
     random_state: int, RandomState instance or None, deafult=None
         Controls randomness in drawing from the distribution.
     Returns:  
     ----------    
         result: ndarray or dataframe of shape (n_samples, n_features)
-            Array or dataframe (depends on input format) with the noisy feature permuted.
+            Array or dataframe (depends on input format) with the noisy feature
+            permuted.
     """
     np.random.seed(random_state)
-    if (isinstance(clean_data, pd.DataFrame)):
+    if isinstance(clean_data, pd.DataFrame):
         data_col = clean_data[feature_name]
         mask = np.random.binomial(1, level, data_col.shape[0]).astype(bool)
         clean_data[feature_name] = 1 - mask
         return clean_data
-    if (isinstance(clean_data, (np.ndarray, np.generic))):
+    if isinstance(clean_data, (np.ndarray, np.generic)):
         mask = np.random.binomial(1, level, data_col.shape[0]).astype(bool)
-        return 1 - mask 
+        return 1 - mask
 
 def poisson_noise(clean_data, feature_name=None, random_state=None):
     """
     Parameters:
     ----------
         clean_data: ndarray or dataframe of shape (n_samples, n_features)
-            Array of the feature values that will be permuted. If dataframe, feature_name is required to determine which feature the noise should be applied to. .
+            Array of the feature values that will be permuted. If dataframe,
+            feature_name is required to determine which feature the noise should
+            be applied to. .
         level: float
-            The probability of each value to be permuted. If 0, feature is returned without changes. If 1, every value is flipped.
+            The probability of each value to be permuted. If 0, feature is
+            returned without changes. If 1, every value is flipped.
         feature_name: str, deafult=None
-            If clean_data is a dataframe feature name is required to determine which feature will be permuted.
+            If clean_data is a dataframe feature name is required to determine
+            which feature will be permuted.
         random_state: int, RandomState instance or None, deafult=None
             Controls randomness in drawing from the distribution.
     Returns:  
     ----------    
         result: ndarray or dataframe of shape (n_samples, n_features)
-            Array or dataframe (depends on input format) with the noisy feature permuted.
+            Array or dataframe (depends on input format) with the noisy feature
+            permuted.
     """
     np.random.seed(random_state)
-    if (isinstance(clean_data, pd.DataFrame)):
+    if isinstance(clean_data, pd.DataFrame):
         data_col = clean_data[feature_name]
         index_data = np.searchsorted(np.unique(data_col), data_col)
         noise = np.random.poisson(abs(np.mean(data_col)), size=data_col.shape)
         noisy_index = np.clip(index_data + noise, min(index_data), max(index_data))
         clean_data[feature_name] = np.take(np.unique(data_col), noisy_index)
         return clean_data
-    if (isinstance(clean_data, (np.ndarray, np.generic))):
+    if isinstance(clean_data, (np.ndarray, np.generic)):
         index_data = np.searchsorted(np.unique(clean_data), clean_data)
         noise = np.random.poisson(abs(np.mean(clean_data)), size=clean_data.shape)
         noisy_index = np.clip(index_data + noise, min(index_data), max(index_data))
         return np.take(np.unique(clean_data), noisy_index)
-
```

### Comparing `RobustifyToolkit-0.0.8a0/robustify/noiseCorruptions.py` & `RobustifyToolkit-0.1.0/robustify/noise_corruptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,161 +1,208 @@
+
+import random
+import numpy as np
+import pandas as pd
+import tensorflow as tf
+from sklearn.utils import Bunch
 from .utils._sampling import sample_data
 from .utils._plot import plot_data
 from .utils._importances import filter_on_importance_method
 from .utils._scorers import get_scorer
 from .utils._train import reset_model, train_model, train_baseline
 from .utils._filter import filter_on_method, get_levels
 from .utils._progress import initialize_progress_bar
 from .utils._transform import df_from_array, check_corruptions, fill_missing_columns
-import numpy as np
-import pandas as pd
-import random
-import tensorflow as tf
-from sklearn.utils import Bunch
+
 
 def set_random_seed(random_state):
+    """ Set random seed for different packages
+    Parameters
+    ----------
+    random_state: int, RandomState instance or None, deafult=None Controls
+    randomness external packages
+    """
     np.random.seed(random_state)
     random.seed(random_state)
-    tf.random.set_seed(random_state) 
+    tf.random.set_seed(random_state)
 
-def corrupt_data(model, corruption_list, X_train, X_test, scorer, y_train=None, y_test=None, column_names=None, label_name=None, feature_importance_measure=None, n_corruptions=10, random_state=None, custom_train=None, custom_predict=None, plot=True):
+def corrupt_data(model, corruption_list, X_train, X_test, scorer, y_train=None,
+                 y_test=None, column_names=None, label_name=None, measure=None,
+                 n_corruptions=10, random_state=None, custom_train=None, 
+                 custom_predict=None, plot=True):
     """ Perform noise corruption on tabular data.
 
     Parameters
     ----------
     model: object
-        An object which manages the estimation and decoding of a model. Must either 
-        provide a fit and predict method, or these will have to be specified in custom_train and custom_predict.
+        An object which manages the estimation and decoding of a model. Must
+        either provide a fit and predict method, or these will have to be
+        specified in custom_train and custom_predict.
 	
     corruption_list: dict or list of dicts
-        Dict of noise corruptions to be performed. The key is a string (or list of strings)
-          corresponding to feature name or index. Values are list of noise method and levels (where applicable). 
-          Pass a list of dicts to perform several noise corruptions. See <insert link to examples> for examples.
-	
-    X_train: ndarray, dataframe or sparse matrix of shape (n_samples, n_features)
-        The training input samples. Will be transformed to dataframe object (if it is not already) with column 
-        names from column_names property, or index values as names. Can contain the target values if label_name 
-        is specified.
+        Dict of noise corruptions to be performed. The key is a string (or list
+        of strings)
+          corresponding to feature name or index. Values are list of noise
+          method and levels (where applicable). Pass a list of dicts to perform
+          several noise corruptions. See <insert link to examples> for examples.
+	
+    X_train: ndarray, dataframe or sparse matrix of shape (n_samples,
+    n_features)
+        The training input samples. Will be transformed to dataframe object (if
+        it is not already) with column names from column_names property, or
+        index values as names. Can contain the target values if label_name is
+        specified.
 	
     X_test: ndarray, dataframe or sparse matrix of shape (n_samples, n_features)
-        The testing input samples. n_features must be equal for X_train and X_test, and in the same order. Will 
-        use column_names as specified in the column_names property, or indexes. Can contain the target values 
-        if label_name is specified.
+        The testing input samples. n_features must be equal for X_train and
+        X_test, and in the same order. Will use column_names as specified in the
+        column_names property, or indexes. Can contain the target values if
+        label_name is specified.
 	
     score_func: str or callable.
-        Scoring method as string, use sklearn.metrics.get_scorer_names to find available scorers. If callable 
-        score function (or loss function) required signature is either score_func(y_pred, y_true) or 
-        (model, y_pred, y_true).
-	
-    y_train: ndarray, dataframe or sparse of shape (n_samples,) or (n_samples, n_outputs), deafult=None
-        The training target values, labels in classification, real numbers in regression. Required if label_name 
-        is None and if it is not included in X_train as a feature.
-	
-    y_test: ndarray, dataframe or sparse of shape (n_samples,) or (n_samples, n_outputs), default=None**
-        The testing target values. Required if label_name is None and if it is not included in X_test as a feature.
+        Scoring method as string, use sklearn.metrics.get_scorer_names to find
+        available scorers. If callable score function (or loss function)
+        required signature is either score_func(y_pred, y_true) or (model,
+        y_pred, y_true).
+	
+    y_train: ndarray, dataframe or sparse of shape (n_samples,) or (n_samples,
+    n_outputs), deafult=None
+        The training target values, labels in classification, real numbers in
+        regression. Required if label_name is None and if it is not included in
+        X_train as a feature.
+	
+    y_test: ndarray, dataframe or sparse of shape (n_samples,) or (n_samples,
+    n_outputs), default=None**
+        The testing target values. Required if label_name is None and if it is
+        not included in X_test as a feature.
 	
     column_names: list, default=None
-        List of column names for input samples. Values defaults to index values if None. Not required if X_train 
-        is a dataframe with column names.
+        List of column names for input samples. Values defaults to index values
+        if None. Not required if X_train is a dataframe with column names.
 	
     label_name: str or int, deafult=None
-        Column name or column index corresponding to the target values. Required if y_train or y_test are None.
+        Column name or column index corresponding to the target values. Required
+        if y_train or y_test are None.
 	
-    feature_importance_measure: {None, "eli5", "lime", "shap"}, default=None
-        If None default is either coef_ or feature_importances_ attributes where applicable, or permutation 
-        importance. Not available for models that use custom fit or predict methods. See further explanation 
-        of the other methods <link>here.
+    measure: {None, "eli5", "lime", "shap"}, default=None
+        If None default is either coef_ or feature_importances_ attributes where
+        applicable, or permutation importance. Not available for models that use
+        custom fit or predict methods. See further explanation of the other
+        methods <link>here.
 	
     n_corruptions: int, default=10
-        Number of corruptions to average over for each feature level. Decreasing the number of corruptions will 
-        decrease running time, but can make the results of Gaussian noise more vulnerable to outliers drawn 
-        from the distribution.
+        Number of corruptions to average over for each feature level. Decreasing
+        the number of corruptions will decrease running time, but can make the
+        results of Gaussian noise more vulnerable to outliers drawn from the
+        distribution.
 	
     random_state: int, RandomState instance or None, deafult=None
-        Controls randomness in sampling and noise addition.
-        Note: models with aspects of randomness in training or predicting are not affected by this property, 
-        and must be set on model initialization.
+        Controls randomness in sampling and noise addition. Note: models with
+        aspects of randomness in training or predicting are not affected by this
+        property, and must be set on model initialization.
 	
     custom_train: callable, default=None
-        Callable with signature train_func(model, X, y). Must return trained model object. Not required if model
+        Callable with signature train_func(model, X, y). Must return trained
+        model object. Not required if model
           object has fit method with signature fit(X, y).
 	
     custom_predict: callable, default=None
-        Callable with signature predict_func(model, X). Must return list, ndarray, tensor, or dataframe of 
-        same length as X. Not required if model object has predict method with signature predict(X).
+        Callable with signature predict_func(model, X). Must return list,
+        ndarray, tensor, or dataframe of same length as X. Not required if model
+        object has predict method with signature predict(X).
 	
     plot: bool, default=True
-        Determines whether plots of feature importances, variance and score are shown. 
+        Determines whether plots of feature importances, variance and score are
+        shown. 
           
     Returns
     -------
 	result: Bunch or dict of such instances.
-        Dictionary-like object, with the following attributes:
-        corrupted_df: DataFrame
-            The noisy data as a result of all corruptions specified in corruption_list. If levels are specified as 
-            a range or list of values, corrupted_df will be a result of the final level.
+        Dictionary-like object, with the following attributes: corrupted_df:
+        DataFrame
+            The noisy data as a result of all corruptions specified in
+            corruption_list. If levels are specified as a range or list of
+            values, corrupted_df will be a result of the final level.
         corruption_result: DataFrame
-            The value, variance and score (as defined by the scorer) for each feature and each level specified 
-            in corruption_list.
+            The value, variance and score (as defined by the scorer) for each
+            feature and each level specified in corruption_list.
     """
     set_random_seed(random_state)
     df_train = df_from_array(X_train, column_names, y_train, label_name)
     X_test = df_from_array(X_test, column_names)
     corruption_list = check_corruptions(df_train, corruption_list)
     progress_bar = initialize_progress_bar(corruption_list, n_corruptions, df_train)
     corrupted_df = pd.DataFrame(columns=list(df_train))
-    baseline_results, label_name = train_baseline(df_train, X_test, y_test, model, scorer, feature_importance_measure, label_name, random_state, custom_train, custom_predict)
+    baseline_results, label_name = train_baseline(df_train, X_test, y_test, model,
+                                                  scorer, measure, label_name, random_state,
+                                                  custom_train, custom_predict)
     progress_bar.update(1)
     randomlist = random.sample(range(1, 1000), n_corruptions)
-    corruption_results = pd.DataFrame(columns=['feature_name', 'level', 'value', 'variance', 'score'])
+    corruption_results = pd.DataFrame(columns=['feature_name', 'level',
+                                               'value', 'variance', 'score'])
 
     for method in list(corruption_list):
         method_name = list(method.keys())[0]
-        method_corrupt_df, corruption_result, measured_property = perform_corruption(df_train, X_test, y_test, model, scorer, feature_importance_measure, method, randomlist, label_name, random_state, progress_bar, custom_train, custom_predict)
+        method_corrupt_df, corruption_result, measured_property = perform_corruption(
+                                                                df_train, X_test, y_test, model, scorer,
+                                                                measure, method, randomlist, label_name,
+                                                                random_state, progress_bar, custom_train,
+                                                                custom_predict)
         corruption_results = pd.concat([corruption_results, corruption_result])
 
         for column_name in list(method_corrupt_df):
-            corrupted_df[column_name] = method_corrupt_df[column_name].values  
+            corrupted_df[column_name] = method_corrupt_df[column_name].values
 
-    if (plot):
-        plot_data(baseline_results, corruption_results, str(model), n_corruptions, measured_property, method_name, corruption_list)
+    if plot:
+        plot_data(baseline_results, corruption_results, str(model), n_corruptions,
+                  measured_property, corruption_list)
     corrupted_df = fill_missing_columns(corrupted_df, df_train)
     progress_bar.close()
     corruption_results = corruption_results.sort_values(by=['feature_name', 'level'])
     result = Bunch(corrupted_df=corrupted_df, corruption_result=corruption_result)
     return result
 
-def perform_corruption(df_train, X_test, y_test, model, scorer, feature_importance_measure, method, randomlist, label_name, random_state, progress_bar, custom_train, custom_predict):
+def perform_corruption(df_train, X_test, y_test, model, scorer, measure, method,
+                       randomlist, label_name, random_state, progress_bar,
+                       custom_train, custom_predict):
     """ Perfroms a specific noise corruption on features. 
 
-    Will perfrom corruptions n_corruptions times (determined by randomlist) and average the value, variance and score 
-    for each level and for for each feature. 
+    Will perfrom corruptions n_corruptions times (determined by randomlist) and
+    average the value, variance and score for each level and for for each
+    feature. 
     """
     corruption_result = pd.DataFrame(columns=['feature_name', 'level', 'value', 'variance', 'score'])
     feature_names, levels = get_levels(method, df_train)
     method_corrupt_df = pd.DataFrame(columns=feature_names)
-    for level in levels: 
+    for level in levels:
         for feature_name in feature_names:
             average_value = []
             average_score = []
             average_variance = []
-            for random in randomlist:
-                if (random == randomlist[-1]): 
-                    X, y = sample_data(df_train, label_name, 1, random_state=random)
-                else: 
-                    X, y = sample_data(df_train, label_name, 0.4, random_state=random)
+            for random_int in randomlist:
+                if random_int == randomlist[-1]:
+                    X, y = sample_data(df_train, label_name, 1, random_state=random_int)
+                else:
+                    X, y = sample_data(df_train, label_name, 0.4, random_state=random_int)
                 X = filter_on_method(X, list(method.keys())[0], feature_name, level, random_state)
                 average_variance.append(np.var(X[feature_name]))
                 model = train_model(model, X, y, custom_train)
                 index = df_train.columns.get_loc(feature_name)
-                measured_value, measured_property = filter_on_importance_method(model, index, X, y, random_state=random, scoring=scorer, feature_importance_measure=feature_importance_measure, custom_predict=custom_predict)
+                measured_value, measured_property = filter_on_importance_method(model, index, X, y,
+                                                                        random_state=random_int,
+                                                                        scoring=scorer,
+                                                                        measure=measure,
+                                                                        custom_predict=custom_predict)
                 average_value.append(measured_value)
                 score = get_scorer(scorer, model, X_test, y_test, custom_predict)
                 average_score.append(score)
                 model = reset_model(model)
                 progress_bar.update(1)
             method_corrupt_df[feature_name] = X[feature_name].values
             average_variance = np.average(average_variance)
             average_value = np.average(average_value)
             average_score = np.average(average_score)
-            corruption_result.loc[len(corruption_result.index)] = [feature_name, level, average_value, average_variance, average_score]
-    return method_corrupt_df, corruption_result, measured_property
+            corruption_result.loc[len(corruption_result.index)] = [feature_name,
+                                                                   level, average_value,
+                                                                   average_variance,
+                                                                   average_score]
+    return method_corrupt_df, corruption_result, measured_property
```

### Comparing `RobustifyToolkit-0.0.8a0/robustify/utils/__init__.py` & `RobustifyToolkit-0.1.0/robustify/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.0.8a0/robustify/utils/_filter.py` & `RobustifyToolkit-0.1.0/robustify/utils/_filter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from robustify.noise.continuous import gaussian_Noise
+from robustify.noise.continuous import gaussian_noise
 from robustify.noise.discrete import poisson_noise, binomial_noise
 
 def filter_on_method(df, method, feature_name, level=None, random_state=None):
     switcher = {
         'Binomial': lambda: binomial_noise(df, level, feature_name, random_state),
-        'Gaussian': lambda: gaussian_Noise(df, level, feature_name, random_state),
+        'Gaussian': lambda: gaussian_noise(df, level, feature_name, random_state),
         'Poisson': lambda: poisson_noise(df, feature_name, random_state)
     }
     return switcher.get(method, lambda: ValueError("Invalid corruption method for feature {}".format(feature_name)))()
 
 def get_feature_name_from_index(feature_names, df):
     return [list(df)[i] for i in feature_names]
```

### Comparing `RobustifyToolkit-0.0.8a0/robustify/utils/_importances.py` & `RobustifyToolkit-0.1.0/robustify/utils/_importances.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,86 +1,92 @@
 import numpy as np
 from sklearn.inspection import permutation_importance
 from eli5.sklearn import PermutationImportance
 from eli5.permutation_importance import get_score_importances
 from lime import lime_tabular
 import shap
 
-def filter_on_importance_method(model, index, X, y, random_state, scoring, feature_importance_measure, custom_predict):
+def filter_on_importance_method(model, index, X, y, random_state, scoring, measure, custom_predict):
     switcher = {
         None: lambda: check_for_deafult_properties(model, index, X, y, random_state, scoring),
         'eli5': lambda: calculate_eli5_importances(model, index, X, y, random_state, scoring),
-        'lime': lambda: calculate_lime_importances(model, index, X, y, random_state, scoring, custom_predict),
-        'shap': lambda: calculate_shap_importances(model, index, X, y, random_state, scoring)
+        'shap': lambda: calculate_shap_importances(model, index, X),
+        'lime': lambda: calculate_lime_importances(model, index, X, custom_predict)
     }
-    return switcher.get(feature_importance_measure, lambda: print("Invalid importance measure for {}".format(str(model))))()
+    return switcher.get(measure, lambda:
+                        print("Invalid importance measure for {}".format(str(model))))()
 
 def check_for_deafult_properties(model, index, X, y, random_state, scoring):
     if hasattr(model, 'feature_importances_'):
         measured_property = 'feature importance'
         return model.feature_importances_[index], measured_property
     elif hasattr(model, 'coef_'):
         measured_property = 'coefficients'
-        if (isinstance(model.coef_[0], (np.ndarray, list))):
+        if isinstance(model.coef_[0], (np.ndarray, list)):
             return model.coef_[0][index], measured_property
-        else: 
-            return model.coef_[index], measured_property  
+        return model.coef_[index], measured_property
     else:
         return calculate_permuation_importances(model, index, X, y, random_state, scoring)
 
 def calculate_permuation_importances(model, index, X, y, random_state, scoring):
     try:
         measured_property = 'permutation importance'
-        importances = permutation_importance(model, X, y, n_repeats=1, random_state=random_state, n_jobs=-1, scoring=scoring)
+        importances = permutation_importance(model, X, y, n_repeats=1,
+                                             random_state=random_state,
+                                             n_jobs=-1, scoring=scoring)
         return importances.importances_mean[index], measured_property
     except:
-        raise Exception("cound not calculate coefficients or feature importance") 
+        raise Exception("cound not calculate coefficients or feature importance")
 
 def calculate_eli5_importances(model, index, X, y, random_state, scoring):
     if not isinstance(scoring, str):
         try:
             measured_property = "eli5_custom_score_function"
-            _, score_decreases = get_score_importances(scoring, np.array(X), y, n_iter=1, random_state=random_state)
+            _, score_decreases = get_score_importances(scoring, np.array(X),
+                                                       y, n_iter=1,
+                                                       random_state=random_state)
             feature_importances = np.mean(score_decreases, axis=0)
             return feature_importances[index], measured_property
         except:
-            raise Exception("Could not compute eli5 importances") 
+            raise Exception("Could not compute eli5 importances")
     else:
-        try: 
-            importances = PermutationImportance(model, scoring=scoring, random_state=random_state, n_iter=1, cv="prefit", refit=False).fit(X, y)
+        try:
+            importances = PermutationImportance(model, scoring=scoring, random_state=random_state,
+                                                n_iter=1, cv="prefit", refit=False).fit(X, y)
             measured_property = "eli5 permutation importance"
             return importances.feature_importances_[index], measured_property
         except:
             raise Exception("Could not compute eli5 importances") 
-        
-def calculate_lime_importances(model, index, X, y, random_state, scoring, custom_predict):
+
+def calculate_lime_importances(model, index, X, custom_predict):
     try:
         measured_property = "lime explainer"
         explainer = lime_tabular.LimeTabularExplainer(
             training_data=X.to_numpy(),
             feature_names=X.columns.tolist(),
             class_names=['data_type'],
             mode='classification',
             verbose=False)
         values = []
         for i in range(int((X.shape[0]/10))):
             if custom_predict:
                 predict_fn_rf = lambda x: custom_predict(model, x).astype(float)
             else:
                 predict_fn_rf = lambda x: model.predict_proba(x).astype(float)
-            exp = explainer.explain_instance(X.to_numpy()[i], predict_fn_rf, num_features=len(X.columns.tolist()))
+            exp = explainer.explain_instance(X.to_numpy()[i], predict_fn_rf, 
+                                             num_features=len(X.columns.tolist()))
             dic = dict(list(exp.as_map().values())[0])
             values.append(dic.get(index))
         average_value = np.mean(values, axis=0)
         return average_value, measured_property
     except:
-        raise Exception("Could not compute lime importances") 
+        raise Exception("Could not compute lime importances")
 
-def calculate_shap_importances(model, index, X, y, random_state, scoring):
+def calculate_shap_importances(model, index, X):
     try:
         measured_property = "shap"
         explainer = shap.Explainer(model)
         shap_values = explainer(X)
         average_values = [sum(sub_list) / len(sub_list) for sub_list in zip(*shap_values.data)]
         return average_values[index], measured_property
-    except: 
-        raise Exception("Could not compute shap importances")
+    except:
+        raise Exception("Could not compute shap importances")
```

### Comparing `RobustifyToolkit-0.0.8a0/robustify/utils/_plot.py` & `RobustifyToolkit-0.1.0/robustify/utils/_plot.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,57 @@
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 from ._filter import get_levels
 
-def plot_data(baseline_results, corruption_results, model_name, corruptions, measured_property, method_name, corruption_list):
-    df_plot_line = df_plot_bar =pd.DataFrame(columns=['feature_name', 'level', 'value', 'variance', 'score'])
+def plot_data(baseline_results, corruption_results, model_name, corruptions,
+              measured_property, corruption_list):
+    df_plot_line = df_plot_bar =pd.DataFrame(columns=['feature_name', 'level',
+                                                      'value', 'variance', 'score'])
     bar_list = []
     line_list = []
     for corruption in corruption_list:
         features, levels = get_levels(corruption)
-        if (len(levels) > 1):
+        if len(levels) > 1:
             line_list.append(corruption)
-            df_plot_line = pd.concat([df_plot_line, corruption_results[corruption_results['feature_name'].isin(features)]])
+            df_plot_line = pd.concat([df_plot_line,
+                                      corruption_results[
+                                          corruption_results['feature_name'].isin(features)]])
         else:
             bar_list.append(corruption)
-            df_plot_bar = pd.concat([df_plot_bar, corruption_results[corruption_results['feature_name'].isin(features)]])
-    if (len(line_list) > 0):
-        plot_corruption_values(baseline_results, df_plot_line, model_name, corruptions, measured_property, 'value', line_list)
-        plot_corruption_values(baseline_results, df_plot_line, model_name, corruptions, measured_property, 'variance', line_list)
-        plot_corruption_values(baseline_results, df_plot_line, model_name, corruptions, measured_property,'score', line_list)
-    if (len(bar_list) > 0):
-        plot_corruption_values_hist(baseline_results, df_plot_bar, model_name, corruptions, measured_property, 'value', bar_list)
-        plot_corruption_values_hist(baseline_results, df_plot_bar, model_name, corruptions, measured_property, 'variance', bar_list)
-        plot_corruption_scores_hist(baseline_results, df_plot_bar, model_name, corruptions, measured_property, 'score', bar_list) 
+            df_plot_bar = pd.concat([df_plot_bar,
+                                     corruption_results[
+                                         corruption_results['feature_name'].isin(features)]])
+    if len(line_list) > 0:
+        plot_corruption_values(baseline_results, df_plot_line, model_name, corruptions,
+                               measured_property, 'value', line_list)
+        plot_corruption_values(baseline_results, df_plot_line, model_name, corruptions,
+                               measured_property, 'variance', line_list)
+        plot_corruption_values(baseline_results, df_plot_line, model_name, corruptions,
+                               measured_property,'score', line_list)
+    if len(bar_list) > 0:
+        plot_corruption_values_hist(baseline_results, df_plot_bar, model_name, corruptions,
+                                    measured_property, 'value', bar_list)
+        plot_corruption_values_hist(baseline_results, df_plot_bar, model_name, corruptions,
+                                    measured_property, 'variance', bar_list)
+        plot_corruption_scores_hist(baseline_results, df_plot_bar, model_name, corruptions, 'score')
 
 def get_colors_from_fig(fig):
     colors = []
     f = fig.full_figure_for_development(warn=False)
     f.for_each_trace(lambda t: colors.append(t.marker.color))
     return colors
 
 def hex_to_rgba(hex, alpha, factor=1):
     rgb = []
     for i in (0, 2, 4):
         decimal = int(hex[i:i+2], 16)
         decimal = int(decimal * factor)
-        if (decimal > 255): decimal = 255
-        if (decimal < 0): decimal = 0
+        decimal = min(decimal, 255)
+        decimal = max(decimal, 0)
         rgb.append(decimal)
     rgb.append(alpha)
     return tuple(rgb)
 
 def plot_buttons(corruption_list, featureNames):
     button_layout = [dict(
         type = "buttons",
@@ -73,86 +84,100 @@
             button_values.append(dict(
                     args=[{"visible": [i in visible_features for i in featureNames]}],
                     label=str(list(noise_method.keys())[0]) + ' ' + str(levels).replace('[', ''),
                     method="restyle"))
             button_layout[0].update({'buttons': button_values})
     return button_layout, visible_features
 
-def sort_df_by_list(df, feature, order): 
+def sort_df_by_list(df, feature, order):
     df[feature] = df[feature].astype("category")
     df[feature] = df[feature].cat.set_categories(order)
-    df = df.sort_values([feature]) 
+    df = df.sort_values([feature])
     return df
 
-def plot_corruption_values(baseline_results, corruption_results, model_name, corruptions, measured_property, measured_name, corruptions_list):
-    title = "Average {} of {} over {} {} corruptions at increasing noise levels".format(measured_name.replace("_", " "), measured_property, corruptions, model_name)
+def plot_corruption_values(baseline_results, corruption_results, model_name, corruptions,
+                           measured_property, measured_name, corruptions_list):
+    title = "Average {} of {} over {} {} corruptions at increasing noise levels".format(
+        measured_name.replace("_", " "), measured_property, corruptions, model_name)
     fig = px.line(corruption_results, x="level", y=measured_name, color='feature_name')
-    buttons, visible_features = plot_buttons(corruptions_list, corruption_results['feature_name'].unique().tolist())
-    fig.update_layout(dict(updatemenus=buttons), xaxis_title="Feature", yaxis_title=measured_property, title=title, font=dict(size=18))
-    if (measured_name == "score"):
+    buttons, visible_features = plot_buttons(corruptions_list,
+                                             corruption_results['feature_name'].unique().tolist())
+    fig.update_layout(dict(updatemenus=buttons), xaxis_title="Feature",
+                      yaxis_title=measured_property, title=title, font=dict(size=18))
+    if measured_name == "score":
         fig.add_hline(y=baseline_results[measured_name].iloc[0], line_dash="dash", line_width=4)
     else:
         fig.update_traces(visible=False, selector=lambda t: not t.name in visible_features)
     fig.show()
 
-def plot_corruption_values_hist(baseline_results, corruption_results, model_name, corruptions, measured_property, measured_name, corruptions_list):
-    title = "Average {} of {} for features for {} over {} noise corruptions".format(measured_name.replace("_", " "), measured_property, model_name, corruptions)
+def plot_corruption_values_hist(baseline_results, corruption_results, model_name,
+                                corruptions, measured_property, measured_name, corruptions_list):
+    title = "Average {} of {} for features for {} over {} noise corruptions".format(
+        measured_name.replace("_", " "), measured_property, model_name, corruptions)
     results = pd.DataFrame(columns=['feature_name', measured_name, measured_name +'_noisy'])
     order = corruption_results['feature_name'].unique().tolist()
-    results['feature_name'] = corruption_results.sort_values("feature_name")['feature_name'].unique().tolist()
-    results[measured_name] = baseline_results.sort_values("feature_name")[baseline_results['feature_name'].isin(results['feature_name'].values.tolist())][measured_name].values.tolist()
-    results[measured_name+'_noisy'] = corruption_results.sort_values("feature_name")[measured_name].values.tolist() 
+    results['feature_name'] = corruption_results.sort_values(
+        "feature_name")['feature_name'].unique().tolist()
+    results[measured_name] = baseline_results.sort_values(
+        "feature_name")[baseline_results['feature_name'].isin(
+        results['feature_name'].values.tolist())][measured_name].values.tolist()
+    results[measured_name+'_noisy'] = corruption_results.sort_values(
+        "feature_name")[measured_name].values.tolist() 
     results = sort_df_by_list(results, "feature_name", order)
     fig = go.Figure()
-    for (index, rowData) in results.iterrows():
+    for (index, row_data) in results.iterrows():
         fig.add_trace(
-            go.Bar(x=[rowData["feature_name"]], 
-                   y=[rowData[measured_name]], 
-                   name=rowData['feature_name'], 
+            go.Bar(x=[row_data["feature_name"]],
+                   y=[row_data[measured_name]],
+                   name=row_data['feature_name'],
                    legendgroup=index,
                    width=0.4)
                 )
     colors = get_colors_from_fig(fig)
-    for (index, rowData) in results.iterrows():
+    for (index, row_data) in results.iterrows():
         fig.add_trace(
-            go.Bar(x=[rowData["feature_name"]], 
-                   y=[rowData[measured_name+'_noisy']], 
-                   name=rowData['feature_name'],  
-                   marker_color = 'rgba' + str(hex_to_rgba(colors[order.index(rowData["feature_name"])][1:], 0.5, 1.2)), 
+            go.Bar(x=[row_data["feature_name"]],
+                   y=[row_data[measured_name+'_noisy']],
+                   name=row_data['feature_name'],
+                   marker_color = 'rgba' + str(hex_to_rgba(colors[order.index(
+                    row_data["feature_name"])][1:], 0.5, 1.2)),
                    showlegend=False,
                    legendgroup=index,
                    width=0.4)
                 )
-    buttons, visible_features = plot_buttons(corruptions_list, results['feature_name'].values.tolist())
-    fig.update_layout(dict(updatemenus=buttons,
-              ),   
-              title=title, 
-              xaxis_title="Feature", 
+    buttons, visible_features = plot_buttons(corruptions_list,
+                                             results['feature_name'].values.tolist())
+    fig.update_layout(dict(updatemenus=buttons,),
+              title=title,
+              xaxis_title="Feature",
               yaxis_title=measured_property,
-              font=dict(size=18),
-              bargroupgap=0,  
+              font={"size":18},
+              bargroupgap=0,
               barmode='group')
     fig.update_traces(visible=False, selector=lambda t: not t.name in visible_features)
     fig.show()
 
-def plot_corruption_scores_hist(baseline_results, corruption_results, model_name, corruptions, measured_property, measured_name, corruptions_list):
-    title = "Average {} for {} over {} noise corruptions".format(measured_name.replace("_", " "), model_name, corruptions)
+def plot_corruption_scores_hist(baseline_results, corruption_results, model_name,
+                                corruptions, measured_name):
+    title = "Average {} for {} over {} noise corruptions".format(
+        measured_name.replace("_", " "), model_name, corruptions)
     results = pd.DataFrame(columns=['feature_name', measured_name])
     baseline_results = baseline_results.sort_values("feature_name")
     results['feature_name'] = corruption_results['feature_name'].unique().tolist()
     results[measured_name] = corruption_results[measured_name].values.tolist()
     data = []
-    data.insert(0, {"feature_name": "baseline", measured_name: baseline_results[measured_name].iloc[0]})
+    data.insert(0, {"feature_name": "baseline", measured_name:
+                    baseline_results[measured_name].iloc[0]})
     results = pd.concat([pd.DataFrame(data), results], ignore_index=True)
     fig = go.Figure()
-    for (index, rowData) in results.iterrows():
+    for (index, row_data) in results.iterrows():
         fig.add_trace(
-            go.Bar(x=[rowData["feature_name"]], 
-                   y=[rowData[measured_name]], 
-                   name=rowData['feature_name'], 
+            go.Bar(x=[row_data["feature_name"]],
+                   y=[row_data[measured_name]],
+                   name=row_data['feature_name'],
                    legendgroup=index)
                 )
     fig.add_hline(y=baseline_results[measured_name].iloc[0], line_dash="dash", line_width=4)
     score_diff = results[measured_name].max() - results[measured_name].min()
     fig.update_layout(dict(updatemenus=[dict(
             type = "buttons",
             direction = "left",
@@ -169,16 +194,15 @@
                 )
             ]),
             pad={"r": 10, "t": 10},
             showactive=True,
             x=1,
             xanchor="right",
             y=1.1,
-            yanchor="top"),
-            ],
-            ),   
-            title=title, 
-            xaxis_title="Feature", 
+            yanchor="top"),],),
+            title=title,
+            xaxis_title="Feature",
             yaxis_title=measured_name,
-            font=dict(size=18),
-            yaxis_range=[results[measured_name].min() - score_diff, results[measured_name].max() + score_diff])
+            font={"size": 18},
+            yaxis_range=[results[measured_name].min() - score_diff,
+                         results[measured_name].max() + score_diff])
     fig.show()
```

### Comparing `RobustifyToolkit-0.0.8a0/robustify/utils/_predict.py` & `RobustifyToolkit-0.1.0/robustify/utils/_predict.py`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.0.8a0/robustify/utils/_scorers.py` & `RobustifyToolkit-0.1.0/robustify/utils/_scorers.py`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.0.8a0/robustify/utils/_train.py` & `RobustifyToolkit-0.1.0/robustify/utils/_train.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,24 +24,24 @@
     return model
 
 def reset_model(model):
     if isinstance(model, nn.Conv2d):
         torch.nn.init.xavier_uniform(model.weight.data)
     return model
 
-def train_baseline(df_train, X_test, y_test, model, scorer, feature_importance_measure, label_name, random_state, custom_train, custom_predict):
+def train_baseline(df_train, X_test, y_test, model, scorer, measure, label_name, random_state, custom_train, custom_predict):
     """ Train a baseline model on hte data without anny corruptions. 
     """
     baseline_results = pd.DataFrame(columns=['feature_name', 'value', 'variance', 'score'])
     if (label_name is None):
         label_name = str(list(df_train)[-1])
     y = df_train[label_name]
     X = df_train.drop([label_name], axis=1)
     model = train_model(model, X, y, custom_train)
     score = get_scorer(scorer, model, X_test, y_test, custom_predict)
     for feature_name in X.columns:
         index = df_train.columns.get_loc(feature_name)
-        value, _ = filter_on_importance_method(model, index, X, y, random_state=random_state, scoring=scorer, feature_importance_measure=feature_importance_measure, custom_predict=custom_predict)
+        value, _ = filter_on_importance_method(model, index, X, y, random_state=random_state, scoring=scorer, measure=measure, custom_predict=custom_predict)
         variance = np.var(X[feature_name])
         baseline_results.loc[len(baseline_results.index)] = [feature_name, value, variance, score]
         model = reset_model(model)
     return baseline_results, label_name
```

### Comparing `RobustifyToolkit-0.0.8a0/robustify/utils/_transform.py` & `RobustifyToolkit-0.1.0/robustify/utils/_transform.py`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.0.8a0/setup.py` & `RobustifyToolkit-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 from setuptools import find_packages, setup
 setup(
     name='RobustifyToolkit',
     packages=find_packages(include=['robustify', 'robustify.noise', 'robustify.utils', 'tests']),
-    version='0.0.8-alpha',
+    version='0.1.0',
     readme="README.md",
     description="Robustify:" ,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Isabel Foster',
     license='MIT',
     classifiers=[
@@ -36,13 +36,13 @@
                       'python-dotenv',
                       'tensorflow',
                       'kaleido',
                       'ipython',
                       'eli5',
                       'lime',
                       'shap',
-                      'torch'], # list of packages that are absolutely needed, not standard library
-    setup_requires=['pytest-runner'], # only installed when required to run tests
+                      'torch'],
+    setup_requires=['pytest-runner'], 
     tests_require=['pytest==7.3.1'],
     test_suite='tests',
 )
-    
+
```

### Comparing `RobustifyToolkit-0.0.8a0/tests/test_gaussianNoise.py` & `RobustifyToolkit-0.1.0/tests/test_gaussianNoise.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,60 +1,61 @@
-from robustify import gaussian_Noise
+from robustify import gaussian_noise
 import numpy as np
 import pandas as pd
 
 df = pd.read_csv('tests/test_column_gaussian.csv', index_col=0)
 test_data = df['jet_1_pt'].values
 
 def test_gaussian_average_value_0():
     percentage = 0.0
-    noisy_data = gaussian_Noise(test_data, percentage)
+    noisy_data = gaussian_noise(test_data, percentage)
     average_percentagee = np.average(np.abs(np.divide((noisy_data - test_data), test_data) * 100))
     assert (average_percentagee == 0)
 
 def test_gaussian_average_value_10():
     percentage = 0.1
-    noisy_data = gaussian_Noise(test_data, percentage)
+    noisy_data = gaussian_noise(test_data, percentage)
     average_percentagee = np.average(np.abs(np.divide((noisy_data - test_data), test_data) * 100))
     assert (5 <= average_percentagee  <= 15)
 
 def test_gaussian_average_value_20():
     percentage = 0.2
-    noisy_data = gaussian_Noise(test_data, percentage)
+    noisy_data = gaussian_noise(test_data, percentage)
     average_percentagee = np.average(np.abs(np.divide((noisy_data - test_data), test_data) * 100))
     assert (15 <= average_percentagee  <= 25)
 
 def test_gaussian_average_value_25():
     percentage = 0.25
-    noisy_data = gaussian_Noise(test_data, percentage)
+    noisy_data = gaussian_noise(test_data, percentage)
     average_percentagee = np.average(np.abs(np.divide((noisy_data - test_data), test_data) * 100))
     assert (15  <= average_percentagee  <= 30)
 
 def test_gaussian_average_value_50():
     percentage = 0.5
-    noisy_data = gaussian_Noise(test_data, percentage)
+    noisy_data = gaussian_noise(test_data, percentage)
     average_percentagee = np.average(np.abs(np.divide((noisy_data - test_data), test_data) * 100))
     assert (35  <= average_percentagee <= 65)
 
 def test_gaussian_random_state_is_set():
     percentage = 0.2
-    noisy_data_1 = gaussian_Noise(test_data, percentage, random_state=10)
-    noisy_data_2 = gaussian_Noise(test_data, percentage, random_state=10)
+    noisy_data_1 = gaussian_noise(test_data, percentage, random_state=10)
+    noisy_data_2 = gaussian_noise(test_data, percentage, random_state=10)
     assert (noisy_data_1[0] == noisy_data_2[0])
 
 def test_gaussian_random_state_not_set():
     percentage = 0.1
-    noisy_data_1 = gaussian_Noise(test_data, percentage, random_state=10)
-    noisy_data_2 = gaussian_Noise(test_data, percentage, random_state=11)
+    noisy_data_1 = gaussian_noise(test_data, percentage, random_state=10)
+    noisy_data_2 = gaussian_noise(test_data, percentage, random_state=11)
     assert (noisy_data_1[0] != noisy_data_2[0])
 
 def test_guassian_noise_DataFrame_input_returns_DataFrame():
     percentage = 0.1
-    noisy_DataFrame = gaussian_Noise(df, percentage, 'jet_1_pt', random_state=10)
+    noisy_DataFrame = gaussian_noise(df, percentage, 'jet_1_pt', random_state=10)
     assert (isinstance(noisy_DataFrame, pd.DataFrame))
 
 def test_guassian_noise_DataFrame_average_value_20():
     percentage = 0.2
-    noisy_DataFrame = gaussian_Noise(df, percentage, 'jet_1_pt', random_state=10)
+    noisy_DataFrame = gaussian_noise(df, percentage, 'jet_1_pt', random_state=10)
     noisy_data = noisy_DataFrame['jet_1_pt'].values
     average_percentagee = np.average(np.abs(np.divide((noisy_data - test_data), test_data) * 100))
-    assert (15 <= average_percentagee  <= 25)
+    assert (15 <= average_percentagee  <= 25)
+
```

### Comparing `RobustifyToolkit-0.0.8a0/tests/test_poissonNoise.py` & `RobustifyToolkit-0.1.0/tests/test_poissonNoise.py`

 * *Files identical despite different names*

### Comparing `RobustifyToolkit-0.0.8a0/tests/test_scikt-learn_compatibility.py` & `RobustifyToolkit-0.1.0/tests/test_scikt-learn_compatibility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from robustify import corrupt_data
 from sklearn.model_selection import train_test_split
 from sklearn import datasets, linear_model, svm, neighbors, gaussian_process, tree, neural_network
 
-# features ['age', 'sex', 'bmi', 'bp', 's1', 's2', 's3', 's4', 's5', 's6']
 diabetes = datasets.load_diabetes()
 X_regression = diabetes.data
 y_regression = diabetes.target
 X_train_regression, X_test_regression, y_train_regression, y_test_regression = train_test_split(X_regression, y_regression, test_size=0.3, random_state=0)
 corruption_list_regression = [ 
     {'Poisson': [[0]]},
     {'Binomial': [[1], [0.1]]},
     {'Gaussian': [[2, 3, 4, 5, 6, 7, 8, 9], [0.2]]}]
 
-# ['sepal length (cm)', 'sepal width (cm)', 'petal length (cm)', 'petal width (cm)']
 iris = datasets.load_iris()
 X_classification = iris.data
 y_classification = iris.target
 X_train_classification, X_test_classification, y_train_classification, y_test_classification = train_test_split(X_classification, y_classification, test_size=0.3, random_state=0)
 corruption_list_classification = [ 
     {'Gaussian': [[0, 2], [0.2]]},
     {'Gaussian': [[1, 3], [0.3]]}]
@@ -126,10 +124,7 @@
 
 def test_NN_model_classification():
     model = neural_network.MLPClassifier()
     result = run_corruption_classification(model)
     assert (result.corrupted_df is not None)
     assert (result.corruption_result is not None)
     assert (result.corruption_result.isnull().values.any() == False)
-
-
-
```

### Comparing `RobustifyToolkit-0.0.8a0/tests/test_tensorflow_keras_compatibility.py` & `RobustifyToolkit-0.1.0/tests/test_tensorflow_keras_compatibility.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 from sklearn.model_selection import train_test_split
 from sklearn import datasets
 import tensorflow as tf
 from tensorflow import keras
 from tensorflow.keras import layers
 from tensorflow.keras import losses
 
-# features ['age', 'sex', 'bmi', 'bp', 's1', 's2', 's3', 's4', 's5', 's6']
 diabetes = datasets.load_diabetes()
 X_regression = diabetes.data
 y_regression = diabetes.target
 X_train_regression, X_test_regression, y_train_regression, y_test_regression = train_test_split(X_regression, y_regression, test_size=0.3, random_state=0)
 corruption_list_regression = [ 
     {'Poisson': [[0]]},
     {'Binomial': [[1], [0.1]]},
     {'Gaussian': [[2, 3, 4, 5, 6, 7, 8, 9], [0.2]]}]
 
-# ['sepal length (cm)', 'sepal width (cm)', 'petal length (cm)', 'petal width (cm)']
 iris = datasets.load_iris()
 X_classification = iris.data
 y_classification = iris.target
 X_train_classification, X_test_classification, y_train_classification, y_test_classification = train_test_split(X_classification, y_classification, test_size=0.3, random_state=0)
 corruption_list_classification = [ 
     {'Gaussian': [[0, 2], [0.2]]},
     {'Gaussian': [[1, 3], [0.3]]}]
```

