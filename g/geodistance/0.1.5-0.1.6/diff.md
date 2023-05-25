# Comparing `tmp/geodistance-0.1.5.tar.gz` & `tmp/geodistance-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\geodistance-0.1.5.tar", last modified: Thu May 25 11:33:35 2023, max compression
+gzip compressed data, was "dist\geodistance-0.1.6.tar", last modified: Thu May 25 11:37:02 2023, max compression
```

## Comparing `geodistance-0.1.5.tar` & `geodistance-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 11:33:35.403884 geodistance-0.1.5/
--rw-rw-rw-   0        0        0     1241 2023-05-25 11:33:35.395900 geodistance-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-05-24 00:06:35.000000 geodistance-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 11:33:35.283883 geodistance-0.1.5/geodistance/
--rw-rw-rw-   0        0        0      679 2023-05-25 11:29:51.000000 geodistance-0.1.5/geodistance/Geodistance.py
--rw-rw-rw-   0        0        0       47 2023-05-25 11:29:54.000000 geodistance-0.1.5/geodistance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 11:33:35.387887 geodistance-0.1.5/geodistance.egg-info/
--rw-rw-rw-   0        0        0     1241 2023-05-25 11:33:35.000000 geodistance-0.1.5/geodistance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-25 11:33:35.000000 geodistance-0.1.5/geodistance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 11:33:35.000000 geodistance-0.1.5/geodistance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-25 11:33:35.000000 geodistance-0.1.5/geodistance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 11:33:35.403884 geodistance-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1634 2023-05-25 11:33:21.000000 geodistance-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 11:37:02.308267 geodistance-0.1.6/
+-rw-rw-rw-   0        0        0     1058 2023-05-25 11:37:02.180266 geodistance-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-05-24 00:06:35.000000 geodistance-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 11:37:01.908973 geodistance-0.1.6/geodistance/
+-rw-rw-rw-   0        0        0      679 2023-05-25 11:29:51.000000 geodistance-0.1.6/geodistance/Geodistance.py
+-rw-rw-rw-   0        0        0       47 2023-05-25 11:29:54.000000 geodistance-0.1.6/geodistance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 11:37:02.172263 geodistance-0.1.6/geodistance.egg-info/
+-rw-rw-rw-   0        0        0     1058 2023-05-25 11:37:01.000000 geodistance-0.1.6/geodistance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-05-25 11:37:01.000000 geodistance-0.1.6/geodistance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 11:37:01.000000 geodistance-0.1.6/geodistance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-25 11:37:01.000000 geodistance-0.1.6/geodistance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 11:37:02.414456 geodistance-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1491 2023-05-25 11:36:48.000000 geodistance-0.1.6/setup.py
```

### Comparing `geodistance-0.1.5/PKG-INFO` & `geodistance-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 Metadata-Version: 2.1
 Name: geodistance
-Version: 0.1.5
+Version: 0.1.6
 Summary: Distance calculation library
 Home-page: https://geodistance.readthedocs.io/
 Author: Adebayo Adeoye
 Author-email: adeoyeadebayo18@gmail.com
 License: MIT
-Description: A library that is used to calculate the distance between 2 coordinates                                       **Installation** 
-         `pip install geodistance`                                                                **Get Started** 
-         Calculating distance between 2 coordinates 
-         `from geodistance import Geodistance` 
-         `length = Geodistance().distance(42.546245, 1.601554, 23.424076, 53.847818)` 
-                                                  `print(length)`
+Description: A library that is used to calculate the distance between 2 coordinates \ **Installation** \ `pip install geodistance` \ **Get Started** \ Calculating distance between 2 coordinates \ `from geodistance import Geodistance` \ `length = Geodistance().distance(42.546245, 1.601554, 23.424076, 53.847818)` \ `print(length)`
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `geodistance-0.1.5/geodistance/Geodistance.py` & `geodistance-0.1.6/geodistance/Geodistance.py`

 * *Files identical despite different names*

### Comparing `geodistance-0.1.5/geodistance.egg-info/PKG-INFO` & `geodistance-0.1.6/geodistance.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 Metadata-Version: 2.1
 Name: geodistance
-Version: 0.1.5
+Version: 0.1.6
 Summary: Distance calculation library
 Home-page: https://geodistance.readthedocs.io/
 Author: Adebayo Adeoye
 Author-email: adeoyeadebayo18@gmail.com
 License: MIT
-Description: A library that is used to calculate the distance between 2 coordinates                                       **Installation** 
-         `pip install geodistance`                                                                **Get Started** 
-         Calculating distance between 2 coordinates 
-         `from geodistance import Geodistance` 
-         `length = Geodistance().distance(42.546245, 1.601554, 23.424076, 53.847818)` 
-                                                  `print(length)`
+Description: A library that is used to calculate the distance between 2 coordinates \ **Installation** \ `pip install geodistance` \ **Get Started** \ Calculating distance between 2 coordinates \ `from geodistance import Geodistance` \ `length = Geodistance().distance(42.546245, 1.601554, 23.424076, 53.847818)` \ `print(length)`
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `geodistance-0.1.5/setup.py` & `geodistance-0.1.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 # The directory containing this file
 HERE = path.abspath(path.dirname(__file__))
 
 
 # This call to setup() does all the work
 setup(
     name="geodistance",
-    version="0.1.5",
+    version="0.1.6",
     description="Distance calculation library",
-    long_description="A library that is used to calculate the distance between 2 coordinates                                       **Installation** \n `pip install geodistance`                                                                **Get Started** \n Calculating distance between 2 coordinates \n `from geodistance import Geodistance` \n `length = Geodistance().distance(42.546245, 1.601554, 23.424076, 53.847818)` \n                                          `print(length)`",
+    long_description="A library that is used to calculate the distance between 2 coordinates \ **Installation** \ `pip install geodistance` \ **Get Started** \ Calculating distance between 2 coordinates \ `from geodistance import Geodistance` \ `length = Geodistance().distance(42.546245, 1.601554, 23.424076, 53.847818)` \ `print(length)`",
     long_description_content_type="text/markdown",
     url="https://geodistance.readthedocs.io/",
     author="Adebayo Adeoye",
     author_email="adeoyeadebayo18@gmail.com",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
```

