# Comparing `tmp/ModularTorch-0.1.tar.gz` & `tmp/ModularTorch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ModularTorch-0.1.tar", last modified: Thu May 25 19:18:55 2023, max compression
+gzip compressed data, was "ModularTorch-0.1.1.tar", last modified: Thu May 25 19:34:16 2023, max compression
```

## Comparing `ModularTorch-0.1.tar` & `ModularTorch-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 19:18:55.002230 ModularTorch-0.1/
--rw-rw-rw-   0        0        0     1094 2023-05-11 17:12:36.000000 ModularTorch-0.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-25 19:18:54.997215 ModularTorch-0.1/ModularTorch.egg-info/
--rw-rw-rw-   0        0        0     1034 2023-05-25 19:18:54.000000 ModularTorch-0.1/ModularTorch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-05-25 19:18:54.000000 ModularTorch-0.1/ModularTorch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 19:18:54.000000 ModularTorch-0.1/ModularTorch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      626 2023-05-25 19:18:54.000000 ModularTorch-0.1/ModularTorch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-25 19:18:54.000000 ModularTorch-0.1/ModularTorch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1034 2023-05-25 19:18:55.002230 ModularTorch-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-05-25 18:36:23.000000 ModularTorch-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 19:18:54.999223 ModularTorch-0.1/modular_torch/
--rw-rw-rw-   0        0        0     3410 2023-05-10 17:43:35.000000 ModularTorch-0.1/modular_torch/DataSetup.py
--rw-rw-rw-   0        0        0      658 2023-05-25 18:36:23.000000 ModularTorch-0.1/modular_torch/Metrics.py
--rw-rw-rw-   0        0        0     2925 2023-05-25 18:36:23.000000 ModularTorch-0.1/modular_torch/ModelBuilder.py
--rw-rw-rw-   0        0        0    10761 2023-05-25 18:36:23.000000 ModularTorch-0.1/modular_torch/Trainers.py
--rw-rw-rw-   0        0        0     3305 2023-05-25 18:36:23.000000 ModularTorch-0.1/modular_torch/Utils.py
--rw-rw-rw-   0        0        0      261 2023-05-25 18:36:23.000000 ModularTorch-0.1/modular_torch/__init__.py
--rw-rw-rw-   0        0        0       86 2023-05-25 19:18:55.002766 ModularTorch-0.1/setup.cfg
--rw-rw-rw-   0        0        0     2900 2023-05-25 19:18:20.000000 ModularTorch-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 19:34:16.011979 ModularTorch-0.1.1/
+-rw-rw-rw-   0        0        0     1094 2023-05-11 17:12:36.000000 ModularTorch-0.1.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-25 19:34:16.007515 ModularTorch-0.1.1/ModularTorch.egg-info/
+-rw-rw-rw-   0        0        0     1036 2023-05-25 19:34:15.000000 ModularTorch-0.1.1/ModularTorch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-05-25 19:34:15.000000 ModularTorch-0.1.1/ModularTorch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 19:34:15.000000 ModularTorch-0.1.1/ModularTorch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-05-25 19:34:15.000000 ModularTorch-0.1.1/ModularTorch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-25 19:34:15.000000 ModularTorch-0.1.1/ModularTorch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1036 2023-05-25 19:34:16.011979 ModularTorch-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-05-25 18:36:23.000000 ModularTorch-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 19:34:16.009516 ModularTorch-0.1.1/modular_torch/
+-rw-rw-rw-   0        0        0     3410 2023-05-10 17:43:35.000000 ModularTorch-0.1.1/modular_torch/DataSetup.py
+-rw-rw-rw-   0        0        0      658 2023-05-25 18:36:23.000000 ModularTorch-0.1.1/modular_torch/Metrics.py
+-rw-rw-rw-   0        0        0     2925 2023-05-25 18:36:23.000000 ModularTorch-0.1.1/modular_torch/ModelBuilder.py
+-rw-rw-rw-   0        0        0    10761 2023-05-25 18:36:23.000000 ModularTorch-0.1.1/modular_torch/Trainers.py
+-rw-rw-rw-   0        0        0     3305 2023-05-25 18:36:23.000000 ModularTorch-0.1.1/modular_torch/Utils.py
+-rw-rw-rw-   0        0        0      261 2023-05-25 18:36:23.000000 ModularTorch-0.1.1/modular_torch/__init__.py
+-rw-rw-rw-   0        0        0       86 2023-05-25 19:34:16.012984 ModularTorch-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1523 2023-05-25 19:34:13.000000 ModularTorch-0.1.1/setup.py
```

### Comparing `ModularTorch-0.1/LICENSE` & `ModularTorch-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ModularTorch-0.1/ModularTorch.egg-info/PKG-INFO` & `ModularTorch-0.1.1/ModularTorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ModularTorch
-Version: 0.1
+Version: 0.1.1
 Summary: custom torch wrapper
 Home-page: https://github.com/sirreajohn/ModularTorch
 Download-URL: https://github.com/sirreajohn/ModularTorch/archive/refs/tags/v0.1a.tar.gz
 Author: Mahesh Patapalli
 Author-email: mahesh.patapali@gmail.com
 License: MIT
 Keywords: pytorch,python,deep learning
```

### Comparing `ModularTorch-0.1/PKG-INFO` & `ModularTorch-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ModularTorch
-Version: 0.1
+Version: 0.1.1
 Summary: custom torch wrapper
 Home-page: https://github.com/sirreajohn/ModularTorch
 Download-URL: https://github.com/sirreajohn/ModularTorch/archive/refs/tags/v0.1a.tar.gz
 Author: Mahesh Patapalli
 Author-email: mahesh.patapali@gmail.com
 License: MIT
 Keywords: pytorch,python,deep learning
```

### Comparing `ModularTorch-0.1/modular_torch/DataSetup.py` & `ModularTorch-0.1.1/modular_torch/DataSetup.py`

 * *Files identical despite different names*

### Comparing `ModularTorch-0.1/modular_torch/Metrics.py` & `ModularTorch-0.1.1/modular_torch/Metrics.py`

 * *Files identical despite different names*

### Comparing `ModularTorch-0.1/modular_torch/ModelBuilder.py` & `ModularTorch-0.1.1/modular_torch/ModelBuilder.py`

 * *Files identical despite different names*

### Comparing `ModularTorch-0.1/modular_torch/Trainers.py` & `ModularTorch-0.1.1/modular_torch/Trainers.py`

 * *Files identical despite different names*

### Comparing `ModularTorch-0.1/modular_torch/Utils.py` & `ModularTorch-0.1.1/modular_torch/Utils.py`

 * *Files identical despite different names*

