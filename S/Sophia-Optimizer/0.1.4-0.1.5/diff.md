# Comparing `tmp/Sophia-Optimizer-0.1.4.tar.gz` & `tmp/Sophia-Optimizer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sophia-Optimizer-0.1.4.tar", last modified: Wed May 24 23:06:05 2023, max compression
+gzip compressed data, was "Sophia-Optimizer-0.1.5.tar", last modified: Wed May 24 23:08:57 2023, max compression
```

## Comparing `Sophia-Optimizer-0.1.4.tar` & `Sophia-Optimizer-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:06:05.815930 Sophia-Optimizer-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 23:05:54.000000 Sophia-Optimizer-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-24 23:06:05.815930 Sophia-Optimizer-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13213 2023-05-24 23:05:54.000000 Sophia-Optimizer-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:06:05.815930 Sophia-Optimizer-0.1.4/Sophia/
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-24 23:05:54.000000 Sophia-Optimizer-0.1.4/Sophia/Sophia.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 23:05:54.000000 Sophia-Optimizer-0.1.4/Sophia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:06:05.815930 Sophia-Optimizer-0.1.4/Sophia_Optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-24 23:06:05.000000 Sophia-Optimizer-0.1.4/Sophia_Optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-24 23:06:05.000000 Sophia-Optimizer-0.1.4/Sophia_Optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 23:06:05.000000 Sophia-Optimizer-0.1.4/Sophia_Optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 23:06:05.000000 Sophia-Optimizer-0.1.4/Sophia_Optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 23:06:05.000000 Sophia-Optimizer-0.1.4/Sophia_Optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 23:06:05.815930 Sophia-Optimizer-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-24 23:05:54.000000 Sophia-Optimizer-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:57.816585 Sophia-Optimizer-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 23:08:44.000000 Sophia-Optimizer-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-24 23:08:57.816585 Sophia-Optimizer-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13213 2023-05-24 23:08:44.000000 Sophia-Optimizer-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:57.816585 Sophia-Optimizer-0.1.5/Sophia/
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-24 23:08:44.000000 Sophia-Optimizer-0.1.5/Sophia/Sophia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 23:08:44.000000 Sophia-Optimizer-0.1.5/Sophia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:57.816585 Sophia-Optimizer-0.1.5/Sophia_Optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-24 23:08:57.000000 Sophia-Optimizer-0.1.5/Sophia_Optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-24 23:08:57.000000 Sophia-Optimizer-0.1.5/Sophia_Optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 23:08:57.000000 Sophia-Optimizer-0.1.5/Sophia_Optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-24 23:08:57.000000 Sophia-Optimizer-0.1.5/Sophia_Optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 23:08:57.000000 Sophia-Optimizer-0.1.5/Sophia_Optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 23:08:57.816585 Sophia-Optimizer-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-24 23:08:44.000000 Sophia-Optimizer-0.1.5/setup.py
```

### Comparing `Sophia-Optimizer-0.1.4/LICENSE` & `Sophia-Optimizer-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Sophia-Optimizer-0.1.4/PKG-INFO` & `Sophia-Optimizer-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sophia-Optimizer
-Version: 0.1.4
+Version: 0.1.5
 Summary: Sophia Optimizer ULTRA FAST
 Home-page: https://github.com/kyegomez/Sophia
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: APACHE
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Sophia-Optimizer-0.1.4/README.md` & `Sophia-Optimizer-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `Sophia-Optimizer-0.1.4/Sophia/Sophia.py` & `Sophia-Optimizer-0.1.5/Sophia/Sophia.py`

 * *Files identical despite different names*

### Comparing `Sophia-Optimizer-0.1.4/Sophia_Optimizer.egg-info/PKG-INFO` & `Sophia-Optimizer-0.1.5/Sophia_Optimizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sophia-Optimizer
-Version: 0.1.4
+Version: 0.1.5
 Summary: Sophia Optimizer ULTRA FAST
 Home-page: https://github.com/kyegomez/Sophia
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: APACHE
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Sophia-Optimizer-0.1.4/setup.py` & `Sophia-Optimizer-0.1.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'Sophia-Optimizer',
   packages = find_packages(exclude=[]),
-  version = '0.1.4',
+  version = '0.1.5',
   license='APACHE',
   description = 'Sophia Optimizer ULTRA FAST',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/Sophia',
   keywords = [
     'artificial intelligence',
     'deep learning',
     'optimizers',
     "Prompt Engineering"
   ],
   install_requires=[
     'torch',
+    'datasets',
+    'transformers',
+
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

