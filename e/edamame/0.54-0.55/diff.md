# Comparing `tmp/edamame-0.54.tar.gz` & `tmp/edamame-0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edamame-0.54.tar", last modified: Wed May 24 21:35:58 2023, max compression
+gzip compressed data, was "edamame-0.55.tar", last modified: Wed May 24 21:52:55 2023, max compression
```

## Comparing `edamame-0.54.tar` & `edamame-0.55.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-24 21:35:58.775701 edamame-0.54/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.54/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11946 2023-05-24 21:35:58.775166 edamame-0.54/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10192 2023-05-23 09:35:51.000000 edamame-0.54/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-24 21:35:58.767033 edamame-0.54/edamame/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-05-24 21:28:49.000000 edamame-0.54/edamame/__init__.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-24 21:35:58.770671 edamame-0.54/edamame/classifier/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      194 2023-05-04 19:56:56.000000 edamame-0.54/edamame/classifier/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22454 2023-05-24 21:28:18.000000 edamame-0.54/edamame/classifier/classification.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8611 2023-05-22 22:01:19.000000 edamame-0.54/edamame/classifier/diagnose.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-24 21:35:58.772617 edamame-0.54/edamame/eda/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      876 2023-05-06 16:04:28.000000 edamame-0.54/edamame/eda/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-05-23 21:20:45.000000 edamame-0.54/edamame/eda/eda.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4460 2023-05-22 20:40:47.000000 edamame-0.54/edamame/eda/tools.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-24 21:35:58.774423 edamame-0.54/edamame/regressor/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.54/edamame/regressor/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8347 2023-05-04 19:55:27.000000 edamame-0.54/edamame/regressor/diagnose.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22021 2023-05-23 08:36:34.000000 edamame-0.54/edamame/regressor/regression.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-24 21:35:58.768586 edamame-0.54/edamame.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11946 2023-05-24 21:35:58.000000 edamame-0.54/edamame.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      461 2023-05-24 21:35:58.000000 edamame-0.54/edamame.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-05-24 21:35:58.000000 edamame-0.54/edamame.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-05-24 21:35:58.000000 edamame-0.54/edamame.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-05-24 21:35:58.000000 edamame-0.54/edamame.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-05-24 21:28:37.000000 edamame-0.54/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-05-24 21:35:58.775839 edamame-0.54/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-24 21:52:55.607667 edamame-0.55/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.55/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11946 2023-05-24 21:52:55.607139 edamame-0.55/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10192 2023-05-23 09:35:51.000000 edamame-0.55/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-24 21:52:55.596121 edamame-0.55/edamame/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-05-24 21:50:35.000000 edamame-0.55/edamame/__init__.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-24 21:52:55.600678 edamame-0.55/edamame/classifier/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      194 2023-05-04 19:56:56.000000 edamame-0.55/edamame/classifier/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22426 2023-05-24 21:50:09.000000 edamame-0.55/edamame/classifier/classification.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8611 2023-05-22 22:01:19.000000 edamame-0.55/edamame/classifier/diagnose.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-24 21:52:55.603668 edamame-0.55/edamame/eda/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      876 2023-05-06 16:04:28.000000 edamame-0.55/edamame/eda/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-05-23 21:20:45.000000 edamame-0.55/edamame/eda/eda.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4460 2023-05-22 20:40:47.000000 edamame-0.55/edamame/eda/tools.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-24 21:52:55.605852 edamame-0.55/edamame/regressor/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.55/edamame/regressor/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8347 2023-05-04 19:55:27.000000 edamame-0.55/edamame/regressor/diagnose.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22021 2023-05-23 08:36:34.000000 edamame-0.55/edamame/regressor/regression.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-24 21:52:55.598262 edamame-0.55/edamame.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11946 2023-05-24 21:52:55.000000 edamame-0.55/edamame.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      461 2023-05-24 21:52:55.000000 edamame-0.55/edamame.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-05-24 21:52:55.000000 edamame-0.55/edamame.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-05-24 21:52:55.000000 edamame-0.55/edamame.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-05-24 21:52:55.000000 edamame-0.55/edamame.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-05-24 21:50:19.000000 edamame-0.55/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-05-24 21:52:55.607807 edamame-0.55/setup.cfg
```

### Comparing `edamame-0.54/LICENSE` & `edamame-0.55/LICENSE`

 * *Files identical despite different names*

### Comparing `edamame-0.54/PKG-INFO` & `edamame-0.55/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edamame
-Version: 0.54
+Version: 0.55
 Summary: Exploratory data analysis tools
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `edamame-0.54/README.md` & `edamame-0.55/README.md`

 * *Files identical despite different names*

### Comparing `edamame-0.54/edamame/classifier/classification.py` & `edamame-0.55/edamame/classifier/classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,15 @@
                 if model_list[model_dct[key]].__class__.__name__ == 'dict':
                         display(f'unable to show {key} model metrics')
                 else:
                     title = f'### {key} model metrics:'
                     display(Markdown(title))
                     y_pred_train = model_list[model_dct[key]].predict(self.X_train)
                     y_pred_test = model_list[model_dct[key]].predict(self.X_test)
-                    if confusion_matrix:
+                    if cm:
                         plt.figure(figsize=(10,4))
                         plt.subplot(121)
                         sns.heatmap(confusion_matrix(self.y_train, y_pred_train), annot=True, fmt="2.0f")
                         plt.title(f'{key} train')
                         plt.subplot(122)
                         sns.heatmap(confusion_matrix(self.y_test, y_pred_test), annot=True, fmt="2.0f")
                         plt.title(f'{key} test')
@@ -301,15 +301,15 @@
             if model_list[model_dct[model_name]].__class__.__name__ == 'dict':
                 display(f'unable to show {model_name} model metrics')
             else:
                 title = f'### {model_name} model metrics:'
                 display(Markdown(title))
                 y_pred_train = model_list[model_dct[model_name]].predict(self.X_train)
                 y_pred_test = model_list[model_dct[model_name]].predict(self.X_test)
-                if confusion_matrix: 
+                if cm: 
                     plt.figure(figsize=(10,4))
                     plt.subplot(121)
                     sns.heatmap(confusion_matrix(self.y_train, y_pred_train), annot=True, fmt="2.0f")
                     plt.title(f'{model_name} train')
                     plt.subplot(122)
                     sns.heatmap(confusion_matrix(self.y_test, y_pred_test), annot=True, fmt="2.0f")
                     plt.title(f'{model_name} test')
```

### Comparing `edamame-0.54/edamame/classifier/diagnose.py` & `edamame-0.55/edamame/classifier/diagnose.py`

 * *Files identical despite different names*

### Comparing `edamame-0.54/edamame/eda/__init__.py` & `edamame-0.55/edamame/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `edamame-0.54/edamame/eda/eda.py` & `edamame-0.55/edamame/eda/eda.py`

 * *Files identical despite different names*

### Comparing `edamame-0.54/edamame/eda/tools.py` & `edamame-0.55/edamame/eda/tools.py`

 * *Files identical despite different names*

### Comparing `edamame-0.54/edamame/regressor/diagnose.py` & `edamame-0.55/edamame/regressor/diagnose.py`

 * *Files identical despite different names*

### Comparing `edamame-0.54/edamame/regressor/regression.py` & `edamame-0.55/edamame/regressor/regression.py`

 * *Files identical despite different names*

### Comparing `edamame-0.54/edamame.egg-info/PKG-INFO` & `edamame-0.55/edamame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edamame
-Version: 0.54
+Version: 0.55
 Summary: Exploratory data analysis tools
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `edamame-0.54/pyproject.toml` & `edamame-0.55/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "edamame"
-version = "0.54"
+version = "0.55"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Exploratory data analysis tools"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

