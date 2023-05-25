# Comparing `tmp/DataDoctor-1.0.6.tar.gz` & `tmp/DataDoctor-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DataDoctor-1.0.6.tar", last modified: Thu May 25 15:40:26 2023, max compression
+gzip compressed data, was "DataDoctor-1.0.7.tar", last modified: Thu May 25 15:44:08 2023, max compression
```

## Comparing `DataDoctor-1.0.6.tar` & `DataDoctor-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 15:40:26.686672 DataDoctor-1.0.6/
-drwxrwxrwx   0        0        0        0 2023-05-25 15:40:26.668487 DataDoctor-1.0.6/DataDoctor.egg-info/
--rw-rw-rw-   0        0        0     4315 2023-05-25 15:40:26.000000 DataDoctor-1.0.6/DataDoctor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-25 15:40:26.000000 DataDoctor-1.0.6/DataDoctor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 15:40:26.000000 DataDoctor-1.0.6/DataDoctor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-25 15:40:26.000000 DataDoctor-1.0.6/DataDoctor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-25 15:40:26.000000 DataDoctor-1.0.6/DataDoctor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-05-25 13:43:05.000000 DataDoctor-1.0.6/LICENSE.md
--rw-rw-rw-   0        0        0     4315 2023-05-25 15:40:26.686672 DataDoctor-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3435 2023-05-25 15:28:29.000000 DataDoctor-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 15:40:26.684119 DataDoctor-1.0.6/data_doctor/
--rw-rw-rw-   0        0        0       34 2023-05-25 15:39:28.000000 DataDoctor-1.0.6/data_doctor/__init__.py
--rw-rw-rw-   0        0        0     8399 2023-05-25 00:59:10.000000 DataDoctor-1.0.6/data_doctor/cleaner.py
--rw-rw-rw-   0        0        0     7391 2023-05-25 13:50:05.000000 DataDoctor-1.0.6/data_doctor/normalizer.py
--rw-rw-rw-   0        0        0      248 2023-05-25 13:51:08.000000 DataDoctor-1.0.6/data_doctor/utils.py
--rw-rw-rw-   0        0        0       42 2023-05-25 15:40:26.686672 DataDoctor-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1277 2023-05-25 15:40:13.000000 DataDoctor-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:44:08.586089 DataDoctor-1.0.7/
+drwxrwxrwx   0        0        0        0 2023-05-25 15:44:08.571701 DataDoctor-1.0.7/DataDoctor.egg-info/
+-rw-rw-rw-   0        0        0     4315 2023-05-25 15:44:08.000000 DataDoctor-1.0.7/DataDoctor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-25 15:44:08.000000 DataDoctor-1.0.7/DataDoctor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 15:44:08.000000 DataDoctor-1.0.7/DataDoctor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-25 15:44:08.000000 DataDoctor-1.0.7/DataDoctor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-25 15:44:08.000000 DataDoctor-1.0.7/DataDoctor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-05-25 13:43:05.000000 DataDoctor-1.0.7/LICENSE.md
+-rw-rw-rw-   0        0        0     4315 2023-05-25 15:44:08.583888 DataDoctor-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3435 2023-05-25 15:28:29.000000 DataDoctor-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 15:44:08.582707 DataDoctor-1.0.7/data_doctor/
+-rw-rw-rw-   0        0        0       34 2023-05-25 15:39:28.000000 DataDoctor-1.0.7/data_doctor/__init__.py
+-rw-rw-rw-   0        0        0     8399 2023-05-25 00:59:10.000000 DataDoctor-1.0.7/data_doctor/cleaner.py
+-rw-rw-rw-   0        0        0     7326 2023-05-25 15:43:46.000000 DataDoctor-1.0.7/data_doctor/normalizer.py
+-rw-rw-rw-   0        0        0      248 2023-05-25 13:51:08.000000 DataDoctor-1.0.7/data_doctor/utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-25 15:44:08.586089 DataDoctor-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1277 2023-05-25 15:44:03.000000 DataDoctor-1.0.7/setup.py
```

### Comparing `DataDoctor-1.0.6/DataDoctor.egg-info/PKG-INFO` & `DataDoctor-1.0.7/DataDoctor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataDoctor
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python package for data cleaning and preprocessing.
 Author: Aryan Bajaj
 Author-email: aryanbajaj104@email.com
 Keywords: data cleaning preprocessing machine learning pandas numpy scikit-learn fuzzywuzzy data normalization
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DataDoctor-1.0.6/LICENSE.md` & `DataDoctor-1.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `DataDoctor-1.0.6/PKG-INFO` & `DataDoctor-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataDoctor
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python package for data cleaning and preprocessing.
 Author: Aryan Bajaj
 Author-email: aryanbajaj104@email.com
 Keywords: data cleaning preprocessing machine learning pandas numpy scikit-learn fuzzywuzzy data normalization
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DataDoctor-1.0.6/README.md` & `DataDoctor-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `DataDoctor-1.0.6/data_doctor/cleaner.py` & `DataDoctor-1.0.7/data_doctor/cleaner.py`

 * *Files identical despite different names*

### Comparing `DataDoctor-1.0.6/data_doctor/normalizer.py` & `DataDoctor-1.0.7/data_doctor/normalizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from sklearn.impute import SimpleImputer, IterativeImputer
 from sklearn.preprocessing import StandardScaler
 from sklearn.ensemble import IsolationForest
 from fuzzywuzzy import fuzz
 import re
 import warnings
 import chardet
-from data_doctor.normalizer import DataDoctor as DataNormalizer
 from data_doctor.utils import detect_encoding
 
 warnings.filterwarnings("ignore")
 
 
 class DataDoctor:
     def __init__(self):
```

### Comparing `DataDoctor-1.0.6/setup.py` & `DataDoctor-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='DataDoctor',
-    version='1.0.6',
+    version='1.0.7',
     author='Aryan Bajaj',
     author_email='aryanbajaj104@email.com',
     description="A Python package for data cleaning and preprocessing.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

