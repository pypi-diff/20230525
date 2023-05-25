# Comparing `tmp/ModularTorch-0.1.2.tar.gz` & `tmp/ModularTorch-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ModularTorch-0.1.2.tar", last modified: Thu May 25 19:42:48 2023, max compression
+gzip compressed data, was "ModularTorch-0.1.3.tar", last modified: Thu May 25 19:48:08 2023, max compression
```

## Comparing `ModularTorch-0.1.2.tar` & `ModularTorch-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 19:42:48.435454 ModularTorch-0.1.2/
--rw-rw-rw-   0        0        0     1094 2023-05-11 17:12:36.000000 ModularTorch-0.1.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-25 19:42:48.429911 ModularTorch-0.1.2/ModularTorch.egg-info/
--rw-rw-rw-   0        0        0     1036 2023-05-25 19:42:48.000000 ModularTorch-0.1.2/ModularTorch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-05-25 19:42:48.000000 ModularTorch-0.1.2/ModularTorch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 19:42:48.000000 ModularTorch-0.1.2/ModularTorch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-05-25 19:42:48.000000 ModularTorch-0.1.2/ModularTorch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-25 19:42:48.000000 ModularTorch-0.1.2/ModularTorch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1036 2023-05-25 19:42:48.435454 ModularTorch-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-05-25 18:36:23.000000 ModularTorch-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 19:42:48.432438 ModularTorch-0.1.2/modular_torch/
--rw-rw-rw-   0        0        0     3410 2023-05-10 17:43:35.000000 ModularTorch-0.1.2/modular_torch/DataSetup.py
--rw-rw-rw-   0        0        0      658 2023-05-25 18:36:23.000000 ModularTorch-0.1.2/modular_torch/Metrics.py
--rw-rw-rw-   0        0        0     2925 2023-05-25 18:36:23.000000 ModularTorch-0.1.2/modular_torch/ModelBuilder.py
--rw-rw-rw-   0        0        0    10761 2023-05-25 18:36:23.000000 ModularTorch-0.1.2/modular_torch/Trainers.py
--rw-rw-rw-   0        0        0     3305 2023-05-25 18:36:23.000000 ModularTorch-0.1.2/modular_torch/Utils.py
--rw-rw-rw-   0        0        0      261 2023-05-25 18:36:23.000000 ModularTorch-0.1.2/modular_torch/__init__.py
--rw-rw-rw-   0        0        0       86 2023-05-25 19:42:48.435454 ModularTorch-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1485 2023-05-25 19:42:31.000000 ModularTorch-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 19:48:08.654119 ModularTorch-0.1.3/
+-rw-rw-rw-   0        0        0     1094 2023-05-11 17:12:36.000000 ModularTorch-0.1.3/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-25 19:48:08.649865 ModularTorch-0.1.3/ModularTorch.egg-info/
+-rw-rw-rw-   0        0        0     1036 2023-05-25 19:48:08.000000 ModularTorch-0.1.3/ModularTorch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-05-25 19:48:08.000000 ModularTorch-0.1.3/ModularTorch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 19:48:08.000000 ModularTorch-0.1.3/ModularTorch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-05-25 19:48:08.000000 ModularTorch-0.1.3/ModularTorch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-25 19:48:08.000000 ModularTorch-0.1.3/ModularTorch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1036 2023-05-25 19:48:08.654119 ModularTorch-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-05-25 18:36:23.000000 ModularTorch-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 19:48:08.651835 ModularTorch-0.1.3/modular_torch/
+-rw-rw-rw-   0        0        0     3410 2023-05-10 17:43:35.000000 ModularTorch-0.1.3/modular_torch/DataSetup.py
+-rw-rw-rw-   0        0        0      658 2023-05-25 18:36:23.000000 ModularTorch-0.1.3/modular_torch/Metrics.py
+-rw-rw-rw-   0        0        0     2925 2023-05-25 18:36:23.000000 ModularTorch-0.1.3/modular_torch/ModelBuilder.py
+-rw-rw-rw-   0        0        0    10761 2023-05-25 18:36:23.000000 ModularTorch-0.1.3/modular_torch/Trainers.py
+-rw-rw-rw-   0        0        0     3305 2023-05-25 18:36:23.000000 ModularTorch-0.1.3/modular_torch/Utils.py
+-rw-rw-rw-   0        0        0      261 2023-05-25 18:36:23.000000 ModularTorch-0.1.3/modular_torch/__init__.py
+-rw-rw-rw-   0        0        0       86 2023-05-25 19:48:08.655134 ModularTorch-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1486 2023-05-25 19:48:05.000000 ModularTorch-0.1.3/setup.py
```

### Comparing `ModularTorch-0.1.2/LICENSE` & `ModularTorch-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ModularTorch-0.1.2/ModularTorch.egg-info/PKG-INFO` & `ModularTorch-0.1.3/ModularTorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ModularTorch
-Version: 0.1.2
+Version: 0.1.3
 Summary: custom torch wrapper
 Home-page: https://github.com/sirreajohn/ModularTorch
 Download-URL: https://github.com/sirreajohn/ModularTorch/archive/refs/tags/v0.1a.tar.gz
 Author: Mahesh Patapalli
 Author-email: mahesh.patapali@gmail.com
 License: MIT
 Keywords: pytorch,python,deep learning
```

### Comparing `ModularTorch-0.1.2/PKG-INFO` & `ModularTorch-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ModularTorch
-Version: 0.1.2
+Version: 0.1.3
 Summary: custom torch wrapper
 Home-page: https://github.com/sirreajohn/ModularTorch
 Download-URL: https://github.com/sirreajohn/ModularTorch/archive/refs/tags/v0.1a.tar.gz
 Author: Mahesh Patapalli
 Author-email: mahesh.patapali@gmail.com
 License: MIT
 Keywords: pytorch,python,deep learning
```

### Comparing `ModularTorch-0.1.2/modular_torch/DataSetup.py` & `ModularTorch-0.1.3/modular_torch/DataSetup.py`

 * *Files identical despite different names*

### Comparing `ModularTorch-0.1.2/modular_torch/Metrics.py` & `ModularTorch-0.1.3/modular_torch/Metrics.py`

 * *Files identical despite different names*

### Comparing `ModularTorch-0.1.2/modular_torch/ModelBuilder.py` & `ModularTorch-0.1.3/modular_torch/ModelBuilder.py`

 * *Files identical despite different names*

### Comparing `ModularTorch-0.1.2/modular_torch/Trainers.py` & `ModularTorch-0.1.3/modular_torch/Trainers.py`

 * *Files identical despite different names*

### Comparing `ModularTorch-0.1.2/modular_torch/Utils.py` & `ModularTorch-0.1.3/modular_torch/Utils.py`

 * *Files identical despite different names*

### Comparing `ModularTorch-0.1.2/setup.py` & `ModularTorch-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from distutils.core import setup
 setup(
   name = 'ModularTorch',         
   packages = ['modular_torch'],   
-  version = '0.1.2',      
+  version = '0.1.3',      
   license='MIT',
   description = 'custom torch wrapper',   
   author = 'Mahesh Patapalli',                   
   author_email = 'mahesh.patapali@gmail.com',      
   url = 'https://github.com/sirreajohn/ModularTorch',  
   download_url = 'https://github.com/sirreajohn/ModularTorch/archive/refs/tags/v0.1a.tar.gz',
   keywords = ['pytorch', 'python', 'deep learning'], 
   install_requires=[            
         "zipfile36",
         "requests",
         "pathlib",
         "torch",
-        "torchvision"
+        "torchvision",
         "numpy",
         "pandas"
         "tqdm",
         "tensorboard",
         "torch-tb-profiler",
         "plotly",
         "torchinfo"
```

