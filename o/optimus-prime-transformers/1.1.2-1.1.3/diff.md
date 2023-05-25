# Comparing `tmp/optimus-prime-transformers-1.1.2.tar.gz` & `tmp/optimus-prime-transformers-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimus-prime-transformers-1.1.2.tar", last modified: Tue May 16 02:21:47 2023, max compression
+gzip compressed data, was "optimus-prime-transformers-1.1.3.tar", last modified: Thu May 25 03:49:10 2023, max compression
```

## Comparing `optimus-prime-transformers-1.1.2.tar` & `optimus-prime-transformers-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:21:47.280943 optimus-prime-transformers-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 02:21:35.000000 optimus-prime-transformers-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-16 02:21:47.280943 optimus-prime-transformers-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    63442 2023-05-16 02:21:35.000000 optimus-prime-transformers-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:21:47.280943 optimus-prime-transformers-1.1.2/optimus_prime/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-16 02:21:36.000000 optimus-prime-transformers-1.1.2/optimus_prime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-16 02:21:36.000000 optimus-prime-transformers-1.1.2/optimus_prime/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-16 02:21:36.000000 optimus-prime-transformers-1.1.2/optimus_prime/autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-16 02:21:36.000000 optimus-prime-transformers-1.1.2/optimus_prime/continuous_autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-16 02:21:36.000000 optimus-prime-transformers-1.1.2/optimus_prime/nonautoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    54721 2023-05-16 02:21:36.000000 optimus-prime-transformers-1.1.2/optimus_prime/x_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-16 02:21:36.000000 optimus-prime-transformers-1.1.2/optimus_prime/xl_autoregressive_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:21:47.280943 optimus-prime-transformers-1.1.2/optimus_prime_transformers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-16 02:21:47.000000 optimus-prime-transformers-1.1.2/optimus_prime_transformers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-16 02:21:47.000000 optimus-prime-transformers-1.1.2/optimus_prime_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 02:21:47.000000 optimus-prime-transformers-1.1.2/optimus_prime_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-16 02:21:47.000000 optimus-prime-transformers-1.1.2/optimus_prime_transformers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 02:21:47.000000 optimus-prime-transformers-1.1.2/optimus_prime_transformers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 02:21:47.280943 optimus-prime-transformers-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-16 02:21:36.000000 optimus-prime-transformers-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:49:10.071202 optimus-prime-transformers-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-25 03:49:10.067202 optimus-prime-transformers-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    63442 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:49:10.067202 optimus-prime-transformers-1.1.3/optimus_prime/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/optimus_prime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/optimus_prime/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/optimus_prime/autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/optimus_prime/continuous_autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/optimus_prime/nonautoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54721 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/optimus_prime/x_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/optimus_prime/xl_autoregressive_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:49:10.067202 optimus-prime-transformers-1.1.3/optimus_prime_transformers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-25 03:49:10.000000 optimus-prime-transformers-1.1.3/optimus_prime_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-25 03:49:10.000000 optimus-prime-transformers-1.1.3/optimus_prime_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 03:49:10.000000 optimus-prime-transformers-1.1.3/optimus_prime_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 03:49:10.000000 optimus-prime-transformers-1.1.3/optimus_prime_transformers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 03:49:10.000000 optimus-prime-transformers-1.1.3/optimus_prime_transformers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 03:49:10.071202 optimus-prime-transformers-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/setup.py
```

### Comparing `optimus-prime-transformers-1.1.2/LICENSE` & `optimus-prime-transformers-1.1.3/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 Phil Wang
+Copyright (c) 2020 Kye Gomez
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `optimus-prime-transformers-1.1.2/PKG-INFO` & `optimus-prime-transformers-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimus-prime-transformers
-Version: 1.1.2
+Version: 1.1.3
 Summary: optimus-prime - Pytorch
 Home-page: https://github.com/kyegomez/Optimus-Prime
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `optimus-prime-transformers-1.1.2/README.md` & `optimus-prime-transformers-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.2/optimus_prime/__init__.py` & `optimus-prime-transformers-1.1.3/optimus_prime/__init__.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.2/optimus_prime/attend.py` & `optimus-prime-transformers-1.1.3/optimus_prime/attend.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.2/optimus_prime/autoregressive_wrapper.py` & `optimus-prime-transformers-1.1.3/optimus_prime/autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.2/optimus_prime/continuous_autoregressive_wrapper.py` & `optimus-prime-transformers-1.1.3/optimus_prime/continuous_autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.2/optimus_prime/nonautoregressive_wrapper.py` & `optimus-prime-transformers-1.1.3/optimus_prime/nonautoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.2/optimus_prime/x_transformers.py` & `optimus-prime-transformers-1.1.3/optimus_prime/x_transformers.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.2/optimus_prime/xl_autoregressive_wrapper.py` & `optimus-prime-transformers-1.1.3/optimus_prime/xl_autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.2/optimus_prime_transformers.egg-info/PKG-INFO` & `optimus-prime-transformers-1.1.3/optimus_prime_transformers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimus-prime-transformers
-Version: 1.1.2
+Version: 1.1.3
 Summary: optimus-prime - Pytorch
 Home-page: https://github.com/kyegomez/Optimus-Prime
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `optimus-prime-transformers-1.1.2/optimus_prime_transformers.egg-info/SOURCES.txt` & `optimus-prime-transformers-1.1.3/optimus_prime_transformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.2/setup.py` & `optimus-prime-transformers-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'optimus-prime-transformers',
   packages = find_packages(exclude=['examples']),
-  version = '1.1.2',
+  version = '1.1.3',
   license='MIT',
   description = 'optimus-prime - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   url = 'https://github.com/kyegomez/Optimus-Prime',
   long_description_content_type = 'text/markdown',
   keywords = [
```

