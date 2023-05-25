# Comparing `tmp/jjuke-0.0.0.4.tar.gz` & `tmp/jjuke-0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jjuke-0.0.0.4.tar", last modified: Wed May 24 09:08:15 2023, max compression
+gzip compressed data, was "dist/jjuke-0.0.0.5.tar", last modified: Thu May 25 18:12:22 2023, max compression
```

## Comparing `jjuke-0.0.0.4.tar` & `jjuke-0.0.0.5.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:08:15.000000 jjuke-0.0.0.4/
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-24 09:08:15.000000 jjuke-0.0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      162 2023-05-11 12:21:10.000000 jjuke-0.0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:08:15.000000 jjuke-0.0.0.4/jjuke/
--rw-r--r--   0 root         (0) root         (0)      121 2023-05-24 09:07:35.000000 jjuke-0.0.0.4/jjuke/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2857 2023-05-11 12:09:23.000000 jjuke-0.0.0.4/jjuke/logger.py
--rw-r--r--   0 root         (0) root         (0)     1666 2023-05-24 07:55:24.000000 jjuke-0.0.0.4/jjuke/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:08:15.000000 jjuke-0.0.0.4/jjuke/metrics/
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-11 12:09:23.000000 jjuke-0.0.0.4/jjuke/metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2967 2023-05-11 12:09:23.000000 jjuke-0.0.0.4/jjuke/metrics/pointcloud.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:08:15.000000 jjuke-0.0.0.4/jjuke/module/
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-11 12:09:23.000000 jjuke-0.0.0.4/jjuke/module/__init__.py
--rw-r--r--   0 root         (0) root         (0)      534 2023-05-11 12:09:23.000000 jjuke-0.0.0.4/jjuke/module/func.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-05-11 12:09:23.000000 jjuke-0.0.0.4/jjuke/module/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:08:15.000000 jjuke-0.0.0.4/jjuke/module/loss/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-11 12:09:23.000000 jjuke-0.0.0.4/jjuke/module/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-05-24 07:55:26.000000 jjuke-0.0.0.4/jjuke/module/loss/focal.py
--rw-r--r--   0 root         (0) root         (0)      362 2023-05-11 12:09:23.000000 jjuke-0.0.0.4/jjuke/module/loss/utils.py
--rw-r--r--   0 root         (0) root         (0)     4318 2023-05-24 07:55:25.000000 jjuke-0.0.0.4/jjuke/options.py
--rw-r--r--   0 root         (0) root         (0)    15015 2023-05-11 12:09:23.000000 jjuke-0.0.0.4/jjuke/sched.py
--rw-r--r--   0 root         (0) root         (0)    25202 2023-05-24 07:55:25.000000 jjuke-0.0.0.4/jjuke/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:08:15.000000 jjuke-0.0.0.4/jjuke/utils/
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-11 12:09:23.000000 jjuke-0.0.0.4/jjuke/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2493 2023-05-11 12:09:23.000000 jjuke-0.0.0.4/jjuke/utils/data.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-05-11 12:09:23.000000 jjuke-0.0.0.4/jjuke/utils/dist.py
--rw-r--r--   0 root         (0) root         (0)      457 2023-05-11 12:09:23.000000 jjuke-0.0.0.4/jjuke/utils/ema.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-05-11 12:09:23.000000 jjuke-0.0.0.4/jjuke/utils/indexing.py
--rw-r--r--   0 root         (0) root         (0)     9553 2023-05-11 12:09:23.000000 jjuke-0.0.0.4/jjuke/utils/interp1d.py
--rw-r--r--   0 root         (0) root         (0)      259 2023-05-11 12:09:23.000000 jjuke-0.0.0.4/jjuke/utils/io.py
--rw-r--r--   0 root         (0) root         (0)     7370 2023-05-11 12:09:23.000000 jjuke-0.0.0.4/jjuke/utils/optim.py
--rw-r--r--   0 root         (0) root         (0)     5673 2023-05-11 12:09:23.000000 jjuke-0.0.0.4/jjuke/utils/utils.py
--rw-r--r--   0 root         (0) root         (0)     9062 2023-05-11 12:09:23.000000 jjuke-0.0.0.4/jjuke/utils/vis3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:08:15.000000 jjuke-0.0.0.4/jjuke.egg-info/
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-24 09:08:15.000000 jjuke-0.0.0.4/jjuke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      736 2023-05-24 09:08:15.000000 jjuke-0.0.0.4/jjuke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 09:08:15.000000 jjuke-0.0.0.4/jjuke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-24 09:08:15.000000 jjuke-0.0.0.4/jjuke.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 09:08:15.000000 jjuke-0.0.0.4/jjuke.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-24 09:08:15.000000 jjuke-0.0.0.4/jjuke.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-24 09:08:15.000000 jjuke-0.0.0.4/jjuke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 09:08:15.000000 jjuke-0.0.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      622 2023-05-24 09:07:38.000000 jjuke-0.0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:12:22.000000 jjuke-0.0.0.5/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-25 18:12:22.000000 jjuke-0.0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      162 2023-05-11 12:21:10.000000 jjuke-0.0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:12:22.000000 jjuke-0.0.0.5/jjuke/
+-rw-r--r--   0 root         (0) root         (0)      121 2023-05-25 18:11:23.000000 jjuke-0.0.0.5/jjuke/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2023-05-11 12:09:23.000000 jjuke-0.0.0.5/jjuke/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-05-24 07:55:24.000000 jjuke-0.0.0.5/jjuke/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:12:22.000000 jjuke-0.0.0.5/jjuke/metrics/
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-25 18:10:12.000000 jjuke-0.0.0.5/jjuke/metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11621 2023-05-25 18:09:59.000000 jjuke-0.0.0.5/jjuke/metrics/evaluation_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-05-24 13:00:20.000000 jjuke-0.0.0.5/jjuke/metrics/pointcloud.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:12:22.000000 jjuke-0.0.0.5/jjuke/module/
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-11 12:09:23.000000 jjuke-0.0.0.5/jjuke/module/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      534 2023-05-11 12:09:23.000000 jjuke-0.0.0.5/jjuke/module/func.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-05-11 12:09:23.000000 jjuke-0.0.0.5/jjuke/module/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:12:22.000000 jjuke-0.0.0.5/jjuke/module/loss/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-11 12:09:23.000000 jjuke-0.0.0.5/jjuke/module/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2023-05-24 07:55:26.000000 jjuke-0.0.0.5/jjuke/module/loss/focal.py
+-rw-r--r--   0 root         (0) root         (0)      362 2023-05-11 12:09:23.000000 jjuke-0.0.0.5/jjuke/module/loss/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4318 2023-05-24 07:55:25.000000 jjuke-0.0.0.5/jjuke/options.py
+-rw-r--r--   0 root         (0) root         (0)    15015 2023-05-11 12:09:23.000000 jjuke-0.0.0.5/jjuke/sched.py
+-rw-r--r--   0 root         (0) root         (0)    25202 2023-05-24 07:55:25.000000 jjuke-0.0.0.5/jjuke/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:12:22.000000 jjuke-0.0.0.5/jjuke/utils/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-11 12:09:23.000000 jjuke-0.0.0.5/jjuke/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-05-11 12:09:23.000000 jjuke-0.0.0.5/jjuke/utils/data.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-11 12:09:23.000000 jjuke-0.0.0.5/jjuke/utils/dist.py
+-rw-r--r--   0 root         (0) root         (0)      457 2023-05-11 12:09:23.000000 jjuke-0.0.0.5/jjuke/utils/ema.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-05-11 12:09:23.000000 jjuke-0.0.0.5/jjuke/utils/indexing.py
+-rw-r--r--   0 root         (0) root         (0)     9553 2023-05-11 12:09:23.000000 jjuke-0.0.0.5/jjuke/utils/interp1d.py
+-rw-r--r--   0 root         (0) root         (0)      259 2023-05-11 12:09:23.000000 jjuke-0.0.0.5/jjuke/utils/io.py
+-rw-r--r--   0 root         (0) root         (0)     7370 2023-05-11 12:09:23.000000 jjuke-0.0.0.5/jjuke/utils/optim.py
+-rw-r--r--   0 root         (0) root         (0)     5673 2023-05-11 12:09:23.000000 jjuke-0.0.0.5/jjuke/utils/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9062 2023-05-11 12:09:23.000000 jjuke-0.0.0.5/jjuke/utils/vis3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:12:22.000000 jjuke-0.0.0.5/jjuke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-25 18:12:22.000000 jjuke-0.0.0.5/jjuke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      772 2023-05-25 18:12:22.000000 jjuke-0.0.0.5/jjuke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 18:12:22.000000 jjuke-0.0.0.5/jjuke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-25 18:12:22.000000 jjuke-0.0.0.5/jjuke.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 09:08:15.000000 jjuke-0.0.0.5/jjuke.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-25 18:12:22.000000 jjuke-0.0.0.5/jjuke.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-25 18:12:22.000000 jjuke-0.0.0.5/jjuke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 18:12:22.000000 jjuke-0.0.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      622 2023-05-25 18:11:11.000000 jjuke-0.0.0.5/setup.py
```

### Comparing `jjuke-0.0.0.4/jjuke/logger.py` & `jjuke-0.0.0.5/jjuke/logger.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.4/jjuke/main.py` & `jjuke-0.0.0.5/jjuke/main.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.4/jjuke/metrics/pointcloud.py` & `jjuke-0.0.0.5/jjuke/metrics/pointcloud.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import torch as th
+import torch
 from pytorch3d.ops import knn_points
 from torch import Tensor
 
 
 class PointDist:
     def __init__(self, a, b) -> None:
         """
@@ -55,16 +55,16 @@
         d2 = self._reduce_result(self._dist2, reduction=reduction)
         return d1 + d2
 
     def chamfer_lp(self, p: float, reduction="mean"):
         if not self._knn_done:
             self._calc_knn()
 
-        d1 = th.norm(self.a - self._knn1[:, :, 0], p=p, dim=-1)
-        d2 = th.norm(self.b - self._knn2[:, :, 0], p=p, dim=-1)
+        d1 = torch.norm(self.a - self._knn1[:, :, 0], p=p, dim=-1)
+        d2 = torch.norm(self.b - self._knn2[:, :, 0], p=p, dim=-1)
         d1 = self._reduce_result(d1, reduction=reduction)
         d2 = self._reduce_result(d2, reduction=reduction)
         return d1 + d2
 
     def recall(self, threshold=1e-3):
         if not self._knn_done:
             self._calc_knn()
```

### Comparing `jjuke-0.0.0.4/jjuke/module/func.py` & `jjuke-0.0.0.5/jjuke/module/func.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.4/jjuke/module/init.py` & `jjuke-0.0.0.5/jjuke/module/init.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.4/jjuke/module/loss/focal.py` & `jjuke-0.0.0.5/jjuke/module/loss/focal.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.4/jjuke/options.py` & `jjuke-0.0.0.5/jjuke/options.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.4/jjuke/sched.py` & `jjuke-0.0.0.5/jjuke/sched.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.4/jjuke/trainer.py` & `jjuke-0.0.0.5/jjuke/trainer.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.4/jjuke/utils/data.py` & `jjuke-0.0.0.5/jjuke/utils/data.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.4/jjuke/utils/dist.py` & `jjuke-0.0.0.5/jjuke/utils/dist.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.4/jjuke/utils/indexing.py` & `jjuke-0.0.0.5/jjuke/utils/indexing.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.4/jjuke/utils/interp1d.py` & `jjuke-0.0.0.5/jjuke/utils/interp1d.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.4/jjuke/utils/optim.py` & `jjuke-0.0.0.5/jjuke/utils/optim.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.4/jjuke/utils/utils.py` & `jjuke-0.0.0.5/jjuke/utils/utils.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.4/jjuke/utils/vis3d.py` & `jjuke-0.0.0.5/jjuke/utils/vis3d.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.4/jjuke.egg-info/SOURCES.txt` & `jjuke-0.0.0.5/jjuke.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 jjuke.egg-info/SOURCES.txt
 jjuke.egg-info/dependency_links.txt
 jjuke.egg-info/entry_points.txt
 jjuke.egg-info/not-zip-safe
 jjuke.egg-info/requires.txt
 jjuke.egg-info/top_level.txt
 jjuke/metrics/__init__.py
+jjuke/metrics/evaluation_metrics.py
 jjuke/metrics/pointcloud.py
 jjuke/module/__init__.py
 jjuke/module/func.py
 jjuke/module/init.py
 jjuke/module/loss/__init__.py
 jjuke/module/loss/focal.py
 jjuke/module/loss/utils.py
```

### Comparing `jjuke-0.0.0.4/setup.py` & `jjuke-0.0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="jjuke",
-    version="0.0.0.4",
+    version="0.0.0.5",
     description="utilities for AI models with Pytorch by JJukE",
     author="JJukE",
     author_email="psj9156@gmail.com",
     url="https://github.com/JJukE/JJuk_E.git",
     packages=find_packages(),
     zip_safe=False,
     install_requires=[
```

