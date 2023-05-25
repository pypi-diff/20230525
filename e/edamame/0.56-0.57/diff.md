# Comparing `tmp/edamame-0.56.tar.gz` & `tmp/edamame-0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edamame-0.56.tar", last modified: Thu May 25 09:01:01 2023, max compression
+gzip compressed data, was "edamame-0.57.tar", last modified: Thu May 25 09:13:43 2023, max compression
```

## Comparing `edamame-0.56.tar` & `edamame-0.57.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-25 09:01:01.024598 edamame-0.56/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.56/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11946 2023-05-25 09:01:01.023897 edamame-0.56/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10192 2023-05-23 09:35:51.000000 edamame-0.56/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-25 09:01:01.014991 edamame-0.56/edamame/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-05-25 08:34:24.000000 edamame-0.56/edamame/__init__.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-25 09:01:01.019010 edamame-0.56/edamame/classifier/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      194 2023-05-04 19:56:56.000000 edamame-0.56/edamame/classifier/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22458 2023-05-25 08:55:07.000000 edamame-0.56/edamame/classifier/classification.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8677 2023-05-25 08:39:28.000000 edamame-0.56/edamame/classifier/diagnose.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-25 09:01:01.021350 edamame-0.56/edamame/eda/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      876 2023-05-06 16:04:28.000000 edamame-0.56/edamame/eda/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-05-23 21:20:45.000000 edamame-0.56/edamame/eda/eda.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4460 2023-05-22 20:40:47.000000 edamame-0.56/edamame/eda/tools.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-25 09:01:01.022944 edamame-0.56/edamame/regressor/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.56/edamame/regressor/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8347 2023-05-04 19:55:27.000000 edamame-0.56/edamame/regressor/diagnose.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22021 2023-05-23 08:36:34.000000 edamame-0.56/edamame/regressor/regression.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-25 09:01:01.017084 edamame-0.56/edamame.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11946 2023-05-25 09:01:01.000000 edamame-0.56/edamame.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      461 2023-05-25 09:01:01.000000 edamame-0.56/edamame.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-05-25 09:01:01.000000 edamame-0.56/edamame.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-05-25 09:01:01.000000 edamame-0.56/edamame.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-05-25 09:01:01.000000 edamame-0.56/edamame.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-05-25 08:34:21.000000 edamame-0.56/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-05-25 09:01:01.024863 edamame-0.56/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-25 09:13:43.322663 edamame-0.57/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.57/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11946 2023-05-25 09:13:43.322250 edamame-0.57/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10192 2023-05-23 09:35:51.000000 edamame-0.57/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-25 09:13:43.313746 edamame-0.57/edamame/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-05-25 09:07:16.000000 edamame-0.57/edamame/__init__.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-25 09:13:43.317664 edamame-0.57/edamame/classifier/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      194 2023-05-04 19:56:56.000000 edamame-0.57/edamame/classifier/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22458 2023-05-25 09:08:17.000000 edamame-0.57/edamame/classifier/classification.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8677 2023-05-25 08:39:28.000000 edamame-0.57/edamame/classifier/diagnose.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-25 09:13:43.319625 edamame-0.57/edamame/eda/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      876 2023-05-06 16:04:28.000000 edamame-0.57/edamame/eda/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-05-23 21:20:45.000000 edamame-0.57/edamame/eda/eda.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4460 2023-05-22 20:40:47.000000 edamame-0.57/edamame/eda/tools.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-25 09:13:43.321221 edamame-0.57/edamame/regressor/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.57/edamame/regressor/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8347 2023-05-04 19:55:27.000000 edamame-0.57/edamame/regressor/diagnose.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22021 2023-05-23 08:36:34.000000 edamame-0.57/edamame/regressor/regression.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-25 09:13:43.315852 edamame-0.57/edamame.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11946 2023-05-25 09:13:43.000000 edamame-0.57/edamame.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      461 2023-05-25 09:13:43.000000 edamame-0.57/edamame.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-05-25 09:13:43.000000 edamame-0.57/edamame.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-05-25 09:13:43.000000 edamame-0.57/edamame.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-05-25 09:13:43.000000 edamame-0.57/edamame.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-05-25 09:07:12.000000 edamame-0.57/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-05-25 09:13:43.322756 edamame-0.57/setup.cfg
```

### Comparing `edamame-0.56/LICENSE` & `edamame-0.57/LICENSE`

 * *Files identical despite different names*

### Comparing `edamame-0.56/PKG-INFO` & `edamame-0.57/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edamame
-Version: 0.56
+Version: 0.57
 Summary: Exploratory data analysis tools
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `edamame-0.56/README.md` & `edamame-0.57/README.md`

 * *Files identical despite different names*

### Comparing `edamame-0.56/edamame/classifier/classification.py` & `edamame-0.57/edamame/classifier/classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,15 +249,15 @@
         grid_svm_c = GridSearchCV(svm_c, tuned_parameters, cv=n_folds, refit=True, verbose=0, scoring='accuracy')
         grid_svm_c.fit(self.X_train, self.y_train.squeeze())
         # save the model in the instance attributes
         self.__svm_fit = grid_svm_c.best_estimator_
         return self.__svm_fit
 
 
-    def model_metrics(self, model_name: Literal["all", "logistic", "guassian_nb", "knn", "tree", "random_forest", "xgboost", "svm"] = 'all', cm: bool = False) -> None:
+    def model_metrics(self, model_name: Literal["all", "logistic", "gaussian_nb", "knn", "tree", "random_forest", "xgboost", "svm"] = 'all', cm: bool = False) -> None:
         """
         Display classification metrics (confusion matrix and classification report) for specified or all trained models.
 
         Args:
             model_name (Literal["all", "logistic", "guassian_nb", "knn", "tree", "random_forest", "xgboost", "svm"]): The name of the model to display the metrics for. Defaults to 'all'.
             cm (bool): Whether to display the confusion matrix. Defaults to False.
 
@@ -266,15 +266,15 @@
 
         Example:
             >>> from edamame.classifier import TrainClassifier
             >>> classifier = TrainClassifier(X_train=X_train, y_train=y_train, X_test=X_test, y_test=y_test)
             >>> xgboost = classifier.xgboost(n_estimators=(10, 100, 5), n_folds=2) 
             >>> classifier.model_metrics(model_name="xgboost")
         """
-        model_dct = {'logistic': 0, 'guassian_nb': 1, 'knn': 2, 'tree': 3, 'random_forest': 4, 'xgboost': 5, 'svm': 6}
+        model_dct = {'logistic': 0, 'gaussian_nb': 1, 'knn': 2, 'tree': 3, 'random_forest': 4, 'xgboost': 5, 'svm': 6}
         model_list = [self.__logistic_fit, self.__gaussian_nb_fit, self.__knn_fit, self.__tree_fit, self.__random_forest_fit, self.__xgb_fit, self.__svm_fit]
         if model_name == 'all':
             for key in model_dct:
                 if model_list[model_dct[key]].__class__.__name__ == 'dict':
                         display(f'unable to show {key} model metrics')
                 else:
                     title = f'### {key} model metrics:'
@@ -386,15 +386,15 @@
         plt.figure(figsize=(10,8))
         box.T.boxplot()
         plt.show()
 
         return [self.__logistic_fit, self.__gaussian_nb_fit, self.__knn_fit, self.__tree_fit, self.__random_forest_fit, self.__xgb_fit, self.__svm_fit]
 
 
-    def save_model(self, model_name: Literal["all", "logistic", "guassian_nb", "knn", "tree", "random_forest", "xgboost", "svm"] = 'all') -> None:
+    def save_model(self, model_name: Literal["all", "logistic", "gaussian_nb", "knn", "tree", "random_forest", "xgboost", "svm"] = 'all') -> None:
         """
         Saves the specified machine learning model or all models in the instance to a pickle file.
 
         Args:
             model_name (Literal["all", "linear", "lasso", "ridge", "tree", "random_forest", "xgboost", "svm"]): 
                 The name of the model to save. Defaults to 'all'.
             
@@ -403,15 +403,15 @@
 
         Example:
             >>> from edamame.classifier import TrainClassifier
             >>> classifier = TrainClassifier(X_train=X_train, y_train=y_train, X_test=X_test, y_test=y_test)
             >>> model_list = classifier.auto_ml()
             >>> classifier.save_model(model_name="all")
         """
-        model_dct = {'logistic': 0, 'guassian_nb': 1, 'knn': 2, 'tree': 3, 'random_forest': 4, 'xgboost': 5, 'svm': 6}
+        model_dct = {'logistic': 0, 'gaussian_nb': 1, 'knn': 2, 'tree': 3, 'random_forest': 4, 'xgboost': 5, 'svm': 6}
         model_list = [self.__logistic_fit, self.__gaussian_nb_fit, self.__knn_fit, self.__tree_fit, self.__random_forest_fit, self.__xgb_fit, self.__svm_fit]
         if model_name == 'all':
             for key in model_dct:
                 if model_list[model_dct[key]].__class__.__name__ == 'dict':
                         display(f'unable to save {key} model')
                 else:
                     filename = f'{key}.pkl'
```

### Comparing `edamame-0.56/edamame/classifier/diagnose.py` & `edamame-0.57/edamame/classifier/diagnose.py`

 * *Files identical despite different names*

### Comparing `edamame-0.56/edamame/eda/__init__.py` & `edamame-0.57/edamame/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `edamame-0.56/edamame/eda/eda.py` & `edamame-0.57/edamame/eda/eda.py`

 * *Files identical despite different names*

### Comparing `edamame-0.56/edamame/eda/tools.py` & `edamame-0.57/edamame/eda/tools.py`

 * *Files identical despite different names*

### Comparing `edamame-0.56/edamame/regressor/diagnose.py` & `edamame-0.57/edamame/regressor/diagnose.py`

 * *Files identical despite different names*

### Comparing `edamame-0.56/edamame/regressor/regression.py` & `edamame-0.57/edamame/regressor/regression.py`

 * *Files identical despite different names*

### Comparing `edamame-0.56/edamame.egg-info/PKG-INFO` & `edamame-0.57/edamame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edamame
-Version: 0.56
+Version: 0.57
 Summary: Exploratory data analysis tools
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `edamame-0.56/pyproject.toml` & `edamame-0.57/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "edamame"
-version = "0.56"
+version = "0.57"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Exploratory data analysis tools"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

