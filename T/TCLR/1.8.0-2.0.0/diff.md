# Comparing `tmp/TCLR-1.8.0.tar.gz` & `tmp/TCLR-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TCLR-1.8.0.tar", last modified: Tue May  9 03:03:46 2023, max compression
+gzip compressed data, was "TCLR-2.0.0.tar", last modified: Thu May 25 08:43:54 2023, max compression
```

## Comparing `TCLR-1.8.0.tar` & `TCLR-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-09 03:03:46.174685 TCLR-1.8.0/
--rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-09 03:03:46.174567 TCLR-1.8.0/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)     2570 2022-08-21 10:21:47.000000 TCLR-1.8.0/README.md
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-09 03:03:46.173807 TCLR-1.8.0/TCLR/
--rw-r-----   0 jacob      (501) staff       (20)    37461 2023-05-09 03:02:55.000000 TCLR-1.8.0/TCLR/TCLRalgorithm.py
--rw-r--r--   0 jacob      (501) staff       (20)      981 2023-05-08 04:07:49.000000 TCLR-1.8.0/TCLR/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-09 03:03:46.174405 TCLR-1.8.0/TCLR.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-09 03:03:46.000000 TCLR-1.8.0/TCLR.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      196 2023-05-09 03:03:46.000000 TCLR-1.8.0/TCLR.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-09 03:03:46.000000 TCLR-1.8.0/TCLR.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       30 2023-05-09 03:03:46.000000 TCLR-1.8.0/TCLR.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        5 2023-05-09 03:03:46.000000 TCLR-1.8.0/TCLR.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-09 03:03:46.174722 TCLR-1.8.0/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1440 2023-05-09 03:03:27.000000 TCLR-1.8.0/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-25 08:43:54.962953 TCLR-2.0.0/
+-rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-25 08:43:54.962828 TCLR-2.0.0/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)     2570 2022-08-21 10:21:47.000000 TCLR-2.0.0/README.md
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-25 08:43:54.962075 TCLR-2.0.0/TCLR/
+-rw-r-----   0 jacob      (501) staff       (20)    38792 2023-05-25 08:43:15.000000 TCLR-2.0.0/TCLR/TCLRalgorithm.py
+-rw-r--r--   0 jacob      (501) staff       (20)      988 2023-05-25 08:16:57.000000 TCLR-2.0.0/TCLR/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-25 08:43:54.962659 TCLR-2.0.0/TCLR.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-25 08:43:54.000000 TCLR-2.0.0/TCLR.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      196 2023-05-25 08:43:54.000000 TCLR-2.0.0/TCLR.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-25 08:43:54.000000 TCLR-2.0.0/TCLR.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       30 2023-05-25 08:43:54.000000 TCLR-2.0.0/TCLR.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        5 2023-05-25 08:43:54.000000 TCLR-2.0.0/TCLR.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-25 08:43:54.962991 TCLR-2.0.0/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1440 2023-05-25 08:43:27.000000 TCLR-2.0.0/setup.py
```

### Comparing `TCLR-1.8.0/PKG-INFO` & `TCLR-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TCLR
-Version: 1.8.0
+Version: 2.0.0
 Summary: Tree-Classifier for Linear Regression (TCLR) is a novel tree model to capture the functional relationships between features and a target based on correlation.
 Home-page: https://github.com/Bin-Cao/TCLRmodel
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `TCLR-1.8.0/README.md` & `TCLR-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `TCLR-1.8.0/TCLR/TCLRalgorithm.py` & `TCLR-2.0.0/TCLR/TCLRalgorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+"""
+    Tree Classifier for Linear Regression (TCLR) 
+    Author : Bin CAO (binjacobcao@gmail.com) 
+
+    TCLR is a new tree model proposed by Professor T-Y Zhang and Mr. Bin Cao et al. for capturing the functional relationships 
+    between features and target variables. The model partitions the feature space into a set of rectangles, with each partition
+    embodying a specific function. This approach is conceptually simple, yet powerful for distinguishing mechanisms. The entire
+    feature space is divided into disjointed unit intervals by hyperplanes parallel to the coordinate axes. Within each partition,
+    the target variable y is modeled as a linear function of a feature xj (j = 1,⋯,m), which is the linear function used in our studied problem.
+    
+    Patent No. : 2021SR1951267, China
+    Reference : Domain knowledge guided interpretive machine learning ——  Formula discovery for the oxidation behavior of Ferritic-Martensitic steels in supercritical water. Bin Cao et al., 2022, JMI, journal paper.
+    DOI : 10.20517/jmi.2022.04
+"""
+
 import math
 import re
 from tabnanny import check
 from textwrap import indent
 import time
 import copy
 import os
@@ -800,15 +815,15 @@
         weightRb = len(subDataSetB[:, -1]) / (len(subDataSetA[:, -1]) + len(subDataSetB[:, -1]))
         R = weightRa * newRa + weightRb * newRb
         return R
     else:
         print('Parameter error | weight')
 
 
-# code on 22023 May 9, Bin Cao
+# code on 2023 May 9, Bin Cao
 def generate_random_features(df: pd.DataFrame, 
                             feature_list: List[str],
                             num_combinations: int,
                              random_seed:int) -> pd.DataFrame:
     """
     randomly generates new feature combinations.
 
@@ -822,19 +837,25 @@
     # randomly generates combination features
     for i in range(num_combinations):
         # randomly chooses two features
         f1 = random.choice(feature_list)
         f2 = random.choice(feature_list)
         
         # choose a operator
-        op = random.choice(['+', '-', '*'])
+        op = random.choice(['+', '-', '*',])
+
+        self_op1 = random.choice(['*1', '*2', '*3','*4','**2','**3'])
+        self_op2 = random.choice(['*1', '*2', '*3','*4','**2','**3'])
         
+        new_f1 = f'{f1} {self_op1}'
+        new_f2 = f'{f2} {self_op2}'
+
         # new feature name
-        new_feature = f'({f1} {op} {f2})'
+        new_feature = f'({new_f1} {op} {new_f2})'
         
         new_features.append(new_feature)
         
         # cal new features
-        df[new_feature] = eval(f'df["{f1}"] {op} df["{f2}"]')
+        df[new_feature] = eval(f'(df["{f1}"] {self_op1}) {op} (df["{f2}"] {self_op2})')
     
     # reture DataFrame 
     return df
```

### Comparing `TCLR-1.8.0/TCLR.egg-info/PKG-INFO` & `TCLR-2.0.0/TCLR.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TCLR
-Version: 1.8.0
+Version: 2.0.0
 Summary: Tree-Classifier for Linear Regression (TCLR) is a novel tree model to capture the functional relationships between features and a target based on correlation.
 Home-page: https://github.com/Bin-Cao/TCLRmodel
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `TCLR-1.8.0/setup.py` & `TCLR-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='TCLR',  # 包名
-    version='1.8.0',  # 版本
+    version='2.0.0',  # 版本
     description="Tree-Classifier for Linear Regression (TCLR) is a novel tree model to capture the functional relationships between features and a target based on correlation.",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
```

