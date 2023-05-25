# Comparing `tmp/neuralint-0.0.2.tar.gz` & `tmp/neuralint-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\neuralint-0.0.2.tar", last modified: Wed May 24 20:45:10 2023, max compression
+gzip compressed data, was "dist\neuralint-0.0.3.tar", last modified: Wed May 24 21:35:23 2023, max compression
```

## Comparing `neuralint-0.0.2.tar` & `neuralint-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 20:45:10.602153 neuralint-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-05-24 20:45:10.586135 neuralint-0.0.2/Neuralint/
--rw-rw-rw-   0        0        0        0 2023-04-04 14:08:16.000000 neuralint-0.0.2/Neuralint/__init__.py
--rw-rw-rw-   0        0        0     3934 2023-05-24 16:22:31.000000 neuralint-0.0.2/Neuralint/endToEnd.py
--rw-rw-rw-   0        0        0     9648 2023-05-19 18:51:52.000000 neuralint-0.0.2/Neuralint/grooveParser.py
--rw-rw-rw-   0        0        0     4840 2023-05-19 18:51:52.000000 neuralint-0.0.2/Neuralint/mix_bugs_1.py
--rw-rw-rw-   0        0        0    63375 2023-05-19 18:51:52.000000 neuralint-0.0.2/Neuralint/nodes_Keras.py
--rw-rw-rw-   0        0        0    60891 2023-05-19 18:51:52.000000 neuralint-0.0.2/Neuralint/nodes_TF.py
--rw-rw-rw-   0        0        0    11164 2023-05-19 18:51:52.000000 neuralint-0.0.2/Neuralint/parser_Keras.py
--rw-rw-rw-   0        0        0     9675 2023-05-19 18:51:52.000000 neuralint-0.0.2/Neuralint/parser_TF.py
--rw-rw-rw-   0        0        0      582 2023-05-24 20:45:10.602153 neuralint-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-24 20:45:10.602153 neuralint-0.0.2/neuralint.egg-info/
--rw-rw-rw-   0        0        0      582 2023-05-24 20:45:10.000000 neuralint-0.0.2/neuralint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-05-24 20:45:10.000000 neuralint-0.0.2/neuralint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 20:45:10.000000 neuralint-0.0.2/neuralint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-24 20:45:10.000000 neuralint-0.0.2/neuralint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-24 20:45:10.000000 neuralint-0.0.2/neuralint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 20:45:10.602153 neuralint-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      844 2023-05-24 20:43:30.000000 neuralint-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 21:35:23.694762 neuralint-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-05-24 21:35:23.679125 neuralint-0.0.3/Neuralint/
+-rw-rw-rw-   0        0        0       25 2023-05-24 21:34:18.000000 neuralint-0.0.3/Neuralint/__init__.py
+-rw-rw-rw-   0        0        0     3934 2023-05-24 16:22:31.000000 neuralint-0.0.3/Neuralint/endToEnd.py
+-rw-rw-rw-   0        0        0     9648 2023-05-19 18:51:52.000000 neuralint-0.0.3/Neuralint/grooveParser.py
+-rw-rw-rw-   0        0        0     4840 2023-05-19 18:51:52.000000 neuralint-0.0.3/Neuralint/mix_bugs_1.py
+-rw-rw-rw-   0        0        0    63375 2023-05-19 18:51:52.000000 neuralint-0.0.3/Neuralint/nodes_Keras.py
+-rw-rw-rw-   0        0        0    60891 2023-05-19 18:51:52.000000 neuralint-0.0.3/Neuralint/nodes_TF.py
+-rw-rw-rw-   0        0        0    11164 2023-05-19 18:51:52.000000 neuralint-0.0.3/Neuralint/parser_Keras.py
+-rw-rw-rw-   0        0        0     9675 2023-05-19 18:51:52.000000 neuralint-0.0.3/Neuralint/parser_TF.py
+-rw-rw-rw-   0        0        0      582 2023-05-24 21:35:23.694762 neuralint-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-24 21:35:23.694762 neuralint-0.0.3/neuralint.egg-info/
+-rw-rw-rw-   0        0        0      582 2023-05-24 21:35:23.000000 neuralint-0.0.3/neuralint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-05-24 21:35:23.000000 neuralint-0.0.3/neuralint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 21:35:23.000000 neuralint-0.0.3/neuralint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-24 21:35:23.000000 neuralint-0.0.3/neuralint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-24 21:35:23.000000 neuralint-0.0.3/neuralint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 21:35:23.694762 neuralint-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      844 2023-05-24 21:35:17.000000 neuralint-0.0.3/setup.py
```

### Comparing `neuralint-0.0.2/Neuralint/endToEnd.py` & `neuralint-0.0.3/Neuralint/endToEnd.py`

 * *Files identical despite different names*

### Comparing `neuralint-0.0.2/Neuralint/grooveParser.py` & `neuralint-0.0.3/Neuralint/grooveParser.py`

 * *Files identical despite different names*

### Comparing `neuralint-0.0.2/Neuralint/mix_bugs_1.py` & `neuralint-0.0.3/Neuralint/mix_bugs_1.py`

 * *Files identical despite different names*

### Comparing `neuralint-0.0.2/Neuralint/nodes_Keras.py` & `neuralint-0.0.3/Neuralint/nodes_Keras.py`

 * *Files identical despite different names*

### Comparing `neuralint-0.0.2/Neuralint/nodes_TF.py` & `neuralint-0.0.3/Neuralint/nodes_TF.py`

 * *Files identical despite different names*

### Comparing `neuralint-0.0.2/Neuralint/parser_Keras.py` & `neuralint-0.0.3/Neuralint/parser_Keras.py`

 * *Files identical despite different names*

### Comparing `neuralint-0.0.2/Neuralint/parser_TF.py` & `neuralint-0.0.3/Neuralint/parser_TF.py`

 * *Files identical despite different names*

### Comparing `neuralint-0.0.2/PKG-INFO` & `neuralint-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralint
-Version: 0.0.2
+Version: 0.0.3
 Summary: Neuralint package
 Home-page: UNKNOWN
 Author: Poly
 Author-email: <ghassendaoud99@gmail.com>
 License: UNKNOWN
 Description: Neuralint package.
 Keywords: python,cnn,test
```

### Comparing `neuralint-0.0.2/neuralint.egg-info/PKG-INFO` & `neuralint-0.0.3/neuralint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralint
-Version: 0.0.2
+Version: 0.0.3
 Summary: Neuralint package
 Home-page: UNKNOWN
 Author: Poly
 Author-email: <ghassendaoud99@gmail.com>
 License: UNKNOWN
 Description: Neuralint package.
 Keywords: python,cnn,test
```

### Comparing `neuralint-0.0.2/setup.py` & `neuralint-0.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Neuralint package'
 LONG_DESCRIPTION = 'Neuralint package.'
 
 # Setting up
 setup(
     name="neuralint",
     version=VERSION,
```

