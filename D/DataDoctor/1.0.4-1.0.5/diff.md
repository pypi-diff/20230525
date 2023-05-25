# Comparing `tmp/DataDoctor-1.0.4.tar.gz` & `tmp/DataDoctor-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DataDoctor-1.0.4.tar", last modified: Thu May 25 15:27:34 2023, max compression
+gzip compressed data, was "DataDoctor-1.0.5.tar", last modified: Thu May 25 15:29:27 2023, max compression
```

## Comparing `DataDoctor-1.0.4.tar` & `DataDoctor-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 15:27:34.544182 DataDoctor-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-05-25 15:27:34.536963 DataDoctor-1.0.4/DataDoctor.egg-info/
--rw-rw-rw-   0        0        0     4309 2023-05-25 15:27:34.000000 DataDoctor-1.0.4/DataDoctor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-25 15:27:34.000000 DataDoctor-1.0.4/DataDoctor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 15:27:34.000000 DataDoctor-1.0.4/DataDoctor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-25 15:27:34.000000 DataDoctor-1.0.4/DataDoctor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-25 15:27:34.000000 DataDoctor-1.0.4/DataDoctor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-05-25 13:43:05.000000 DataDoctor-1.0.4/LICENSE.md
--rw-rw-rw-   0        0        0     4309 2023-05-25 15:27:34.541667 DataDoctor-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3429 2023-05-25 15:20:12.000000 DataDoctor-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 15:27:34.540659 DataDoctor-1.0.4/data_doctor/
--rw-rw-rw-   0        0        0        0 2023-05-25 13:44:09.000000 DataDoctor-1.0.4/data_doctor/__init__.py
--rw-rw-rw-   0        0        0     8399 2023-05-25 00:59:10.000000 DataDoctor-1.0.4/data_doctor/cleaner.py
--rw-rw-rw-   0        0        0     7391 2023-05-25 13:50:05.000000 DataDoctor-1.0.4/data_doctor/normalizer.py
--rw-rw-rw-   0        0        0      248 2023-05-25 13:51:08.000000 DataDoctor-1.0.4/data_doctor/utils.py
--rw-rw-rw-   0        0        0       42 2023-05-25 15:27:34.545031 DataDoctor-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1277 2023-05-25 15:25:59.000000 DataDoctor-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:29:27.827395 DataDoctor-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-05-25 15:29:27.822032 DataDoctor-1.0.5/DataDoctor.egg-info/
+-rw-rw-rw-   0        0        0     4315 2023-05-25 15:29:27.000000 DataDoctor-1.0.5/DataDoctor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-25 15:29:27.000000 DataDoctor-1.0.5/DataDoctor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 15:29:27.000000 DataDoctor-1.0.5/DataDoctor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-25 15:29:27.000000 DataDoctor-1.0.5/DataDoctor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-25 15:29:27.000000 DataDoctor-1.0.5/DataDoctor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-05-25 13:43:05.000000 DataDoctor-1.0.5/LICENSE.md
+-rw-rw-rw-   0        0        0     4315 2023-05-25 15:29:27.824214 DataDoctor-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3435 2023-05-25 15:28:29.000000 DataDoctor-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 15:29:27.824214 DataDoctor-1.0.5/data_doctor/
+-rw-rw-rw-   0        0        0        0 2023-05-25 13:44:09.000000 DataDoctor-1.0.5/data_doctor/__init__.py
+-rw-rw-rw-   0        0        0     8399 2023-05-25 00:59:10.000000 DataDoctor-1.0.5/data_doctor/cleaner.py
+-rw-rw-rw-   0        0        0     7391 2023-05-25 13:50:05.000000 DataDoctor-1.0.5/data_doctor/normalizer.py
+-rw-rw-rw-   0        0        0      248 2023-05-25 13:51:08.000000 DataDoctor-1.0.5/data_doctor/utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-25 15:29:27.827395 DataDoctor-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1277 2023-05-25 15:29:21.000000 DataDoctor-1.0.5/setup.py
```

### Comparing `DataDoctor-1.0.4/DataDoctor.egg-info/PKG-INFO` & `DataDoctor-1.0.5/DataDoctor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataDoctor
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python package for data cleaning and preprocessing.
 Author: Aryan Bajaj
 Author-email: aryanbajaj104@email.com
 Keywords: data cleaning preprocessing machine learning pandas numpy scikit-learn fuzzywuzzy data normalization
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# DataDoctor
+# DataDoctor[Beta]
 
 DataDoctor is a Python package for data cleaning and preprocessing. It provides various methods to treat common issues in data such as missing values, duplicate records, inconsistent data formats, outliers, inconsistent naming conventions, data entry errors, and more. The package uses popular libraries such as pandas, numpy, scikit-learn, fuzzywuzzy, and chardet.
 
 [![Python Version](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue)](https://www.python.org/downloads/)
 
 ## Built With
```

### Comparing `DataDoctor-1.0.4/LICENSE.md` & `DataDoctor-1.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `DataDoctor-1.0.4/PKG-INFO` & `DataDoctor-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataDoctor
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python package for data cleaning and preprocessing.
 Author: Aryan Bajaj
 Author-email: aryanbajaj104@email.com
 Keywords: data cleaning preprocessing machine learning pandas numpy scikit-learn fuzzywuzzy data normalization
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# DataDoctor
+# DataDoctor[Beta]
 
 DataDoctor is a Python package for data cleaning and preprocessing. It provides various methods to treat common issues in data such as missing values, duplicate records, inconsistent data formats, outliers, inconsistent naming conventions, data entry errors, and more. The package uses popular libraries such as pandas, numpy, scikit-learn, fuzzywuzzy, and chardet.
 
 [![Python Version](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue)](https://www.python.org/downloads/)
 
 ## Built With
```

### Comparing `DataDoctor-1.0.4/README.md` & `DataDoctor-1.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# DataDoctor
+# DataDoctor[Beta]
 
 DataDoctor is a Python package for data cleaning and preprocessing. It provides various methods to treat common issues in data such as missing values, duplicate records, inconsistent data formats, outliers, inconsistent naming conventions, data entry errors, and more. The package uses popular libraries such as pandas, numpy, scikit-learn, fuzzywuzzy, and chardet.
 
 [![Python Version](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue)](https://www.python.org/downloads/)
 
 ## Built With
```

### Comparing `DataDoctor-1.0.4/data_doctor/cleaner.py` & `DataDoctor-1.0.5/data_doctor/cleaner.py`

 * *Files identical despite different names*

### Comparing `DataDoctor-1.0.4/data_doctor/normalizer.py` & `DataDoctor-1.0.5/data_doctor/normalizer.py`

 * *Files identical despite different names*

### Comparing `DataDoctor-1.0.4/setup.py` & `DataDoctor-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='DataDoctor',
-    version='1.0.4',
+    version='1.0.5',
     author='Aryan Bajaj',
     author_email='aryanbajaj104@email.com',
     description="A Python package for data cleaning and preprocessing.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

