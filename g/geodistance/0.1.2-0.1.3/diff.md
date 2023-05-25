# Comparing `tmp/geodistance-0.1.2.tar.gz` & `tmp/geodistance-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\geodistance-0.1.2.tar", last modified: Thu May 25 11:24:57 2023, max compression
+gzip compressed data, was "dist\geodistance-0.1.3.tar", last modified: Thu May 25 11:27:32 2023, max compression
```

## Comparing `geodistance-0.1.2.tar` & `geodistance-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 11:24:57.535951 geodistance-0.1.2/
--rw-rw-rw-   0        0        0     1044 2023-05-25 11:24:57.519952 geodistance-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-05-24 00:06:35.000000 geodistance-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 11:24:57.479949 geodistance-0.1.2/geodistance/
--rw-rw-rw-   0        0        0      679 2023-05-23 23:34:54.000000 geodistance-0.1.2/geodistance/Geodistance.py
--rw-rw-rw-   0        0        0       47 2023-05-23 22:48:00.000000 geodistance-0.1.2/geodistance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 11:24:57.519952 geodistance-0.1.2/geodistance.egg-info/
--rw-rw-rw-   0        0        0     1044 2023-05-25 11:24:57.000000 geodistance-0.1.2/geodistance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-25 11:24:57.000000 geodistance-0.1.2/geodistance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 11:24:57.000000 geodistance-0.1.2/geodistance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-25 11:24:57.000000 geodistance-0.1.2/geodistance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 11:24:57.535951 geodistance-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1477 2023-05-25 11:24:41.000000 geodistance-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 11:27:32.572204 geodistance-0.1.3/
+-rw-rw-rw-   0        0        0     1065 2023-05-25 11:27:32.564207 geodistance-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-05-24 00:06:35.000000 geodistance-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 11:27:32.484211 geodistance-0.1.3/geodistance/
+-rw-rw-rw-   0        0        0      679 2023-05-23 23:34:54.000000 geodistance-0.1.3/geodistance/Geodistance.py
+-rw-rw-rw-   0        0        0       47 2023-05-23 22:48:00.000000 geodistance-0.1.3/geodistance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 11:27:32.564207 geodistance-0.1.3/geodistance.egg-info/
+-rw-rw-rw-   0        0        0     1065 2023-05-25 11:27:32.000000 geodistance-0.1.3/geodistance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-05-25 11:27:32.000000 geodistance-0.1.3/geodistance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 11:27:32.000000 geodistance-0.1.3/geodistance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-25 11:27:32.000000 geodistance-0.1.3/geodistance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 11:27:32.572204 geodistance-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1498 2023-05-25 11:27:19.000000 geodistance-0.1.3/setup.py
```

### Comparing `geodistance-0.1.2/PKG-INFO` & `geodistance-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: geodistance
-Version: 0.1.2
+Version: 0.1.3
 Summary: Distance calculation library
 Home-page: https://geodistance.readthedocs.io/
 Author: Adebayo Adeoye
 Author-email: adeoyeadebayo18@gmail.com
 License: MIT
-Description: A library that is used to calculate the distance between 2 coordinates **Installation** `pip install geodistance` **Get Started** Calculating distance between 2 coordinates `from geodistance import Geodistance` `length = Geodistance().distance(42.546245, 1.601554, 23.424076, 53.847818)` `print(length)`
+Description: A library that is used to calculate the distance between 2 coordinates /n **Installation** /n `pip install geodistance` /n **Get Started** /n Calculating distance between 2 coordinates /n `from geodistance import Geodistance` /n `length = Geodistance().distance(42.546245, 1.601554, 23.424076, 53.847818)` /n `print(length)`
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `geodistance-0.1.2/geodistance/Geodistance.py` & `geodistance-0.1.3/geodistance/Geodistance.py`

 * *Files identical despite different names*

### Comparing `geodistance-0.1.2/geodistance.egg-info/PKG-INFO` & `geodistance-0.1.3/geodistance.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: geodistance
-Version: 0.1.2
+Version: 0.1.3
 Summary: Distance calculation library
 Home-page: https://geodistance.readthedocs.io/
 Author: Adebayo Adeoye
 Author-email: adeoyeadebayo18@gmail.com
 License: MIT
-Description: A library that is used to calculate the distance between 2 coordinates **Installation** `pip install geodistance` **Get Started** Calculating distance between 2 coordinates `from geodistance import Geodistance` `length = Geodistance().distance(42.546245, 1.601554, 23.424076, 53.847818)` `print(length)`
+Description: A library that is used to calculate the distance between 2 coordinates /n **Installation** /n `pip install geodistance` /n **Get Started** /n Calculating distance between 2 coordinates /n `from geodistance import Geodistance` /n `length = Geodistance().distance(42.546245, 1.601554, 23.424076, 53.847818)` /n `print(length)`
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `geodistance-0.1.2/setup.py` & `geodistance-0.1.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 # The directory containing this file
 HERE = path.abspath(path.dirname(__file__))
 
 
 # This call to setup() does all the work
 setup(
     name="geodistance",
-    version="0.1.2",
+    version="0.1.3",
     description="Distance calculation library",
-    long_description="A library that is used to calculate the distance between 2 coordinates **Installation** `pip install geodistance` **Get Started** Calculating distance between 2 coordinates `from geodistance import Geodistance` `length = Geodistance().distance(42.546245, 1.601554, 23.424076, 53.847818)` `print(length)`",
+    long_description="A library that is used to calculate the distance between 2 coordinates /n **Installation** /n `pip install geodistance` /n **Get Started** /n Calculating distance between 2 coordinates /n `from geodistance import Geodistance` /n `length = Geodistance().distance(42.546245, 1.601554, 23.424076, 53.847818)` /n `print(length)`",
     long_description_content_type="text/markdown",
     url="https://geodistance.readthedocs.io/",
     author="Adebayo Adeoye",
     author_email="adeoyeadebayo18@gmail.com",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
```

