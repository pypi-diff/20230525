# Comparing `tmp/easytorch-3.7.7.tar.gz` & `tmp/easytorch-3.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytorch-3.7.7.tar", last modified: Wed May 10 18:11:51 2023, max compression
+gzip compressed data, was "easytorch-3.7.8.tar", last modified: Wed May 24 23:19:59 2023, max compression
```

## Comparing `easytorch-3.7.7.tar` & `easytorch-3.7.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:11:51.100686 easytorch-3.7.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-10 18:11:40.000000 easytorch-3.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-10 18:11:51.100686 easytorch-3.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-10 18:11:40.000000 easytorch-3.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:11:51.096686 easytorch-3.7.7/easytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:11:51.100686 easytorch-3.7.7/easytorch/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/config/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:11:51.100686 easytorch-3.7.7/easytorch/data/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12983 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/data/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/data/datautils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/data/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/easytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:11:51.100686 easytorch-3.7.7/easytorch/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/metrics/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:11:51.100686 easytorch-3.7.7/easytorch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/utils/ddp_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/utils/tensorutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:11:51.100686 easytorch-3.7.7/easytorch/vision/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/vision/imageutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/vision/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/vision/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:11:51.096686 easytorch-3.7.7/easytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-10 18:11:51.000000 easytorch-3.7.7/easytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-10 18:11:51.000000 easytorch-3.7.7/easytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:11:51.000000 easytorch-3.7.7/easytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 18:11:51.000000 easytorch-3.7.7/easytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 18:11:51.000000 easytorch-3.7.7/easytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 18:11:51.100686 easytorch-3.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-10 18:11:40.000000 easytorch-3.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:19:59.446579 easytorch-3.7.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-24 23:19:48.000000 easytorch-3.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-24 23:19:59.446579 easytorch-3.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-24 23:19:48.000000 easytorch-3.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:19:59.442579 easytorch-3.7.8/easytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:19:59.442579 easytorch-3.7.8/easytorch/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/config/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:19:59.446579 easytorch-3.7.8/easytorch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/data/datautils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/data/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/easytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:19:59.446579 easytorch-3.7.8/easytorch/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/metrics/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:19:59.446579 easytorch-3.7.8/easytorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/utils/ddp_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/utils/tensorutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:19:59.446579 easytorch-3.7.8/easytorch/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/vision/imageutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/vision/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/vision/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:19:59.442579 easytorch-3.7.8/easytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-24 23:19:59.000000 easytorch-3.7.8/easytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-24 23:19:59.000000 easytorch-3.7.8/easytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 23:19:59.000000 easytorch-3.7.8/easytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-24 23:19:59.000000 easytorch-3.7.8/easytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 23:19:59.000000 easytorch-3.7.8/easytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 23:19:59.446579 easytorch-3.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-24 23:19:48.000000 easytorch-3.7.8/setup.py
```

### Comparing `easytorch-3.7.7/LICENSE` & `easytorch-3.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.7/PKG-INFO` & `easytorch-3.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytorch
-Version: 3.7.7
+Version: 3.7.8
 Summary: Easy Neural Network Experiments with pytorch
 Home-page: https://github.com/sraashis/easytorch
 Author: Aashis Khana1
 Author-email: sraashis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `easytorch-3.7.7/README.md` & `easytorch-3.7.8/README.md`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.7/easytorch/config/__init__.py` & `easytorch-3.7.8/easytorch/config/__init__.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.7/easytorch/config/state.py` & `easytorch-3.7.8/easytorch/config/state.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.7/easytorch/data/data.py` & `easytorch-3.7.8/easytorch/data/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
             dataset.add(files=data_split[handle_key], diskcache=self.diskcache, verbose=self.conf['verbose'])
             return self.dataloader_args[handle_key].setdefault('dataset', dataset)
 
     def get_data_loader(self, handle_key='', distributed=False, use_unpadded_sampler=False, **kw):
         args = {**self.conf}
         args['distributed'] = distributed
         args['use_unpadded_sampler'] = use_unpadded_sampler
-        args.update(self.dataloader_args.get(handle_key, {}))
         args.update(**kw)
 
         if args.get('dataset') is None:
             return None
 
         loader_args = {
             'dataset': None,
@@ -94,14 +93,15 @@
             'drop_last': False,
             'timeout': 0,
             'worker_init_fn': _multi.seed_worker if args.get('seed_all') else None
         }
 
         for k in loader_args.keys():
             loader_args[k] = args.get(k, loader_args.get(k))
+        loader_args.update(**self.dataloader_args.get(handle_key, {}))
 
         if loader_args['sampler'] is not None:
             """Sampler and shuffle are mutually exclusive"""
             loader_args['shuffle'] = False
 
         if args['distributed']:
             sampler_args = {
```

### Comparing `easytorch-3.7.7/easytorch/data/datautils.py` & `easytorch-3.7.8/easytorch/data/datautils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.7/easytorch/data/multiproc.py` & `easytorch-3.7.8/easytorch/data/multiproc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import multiprocessing as _mp
 import traceback as _tb
 from functools import partial as _partial
 from typing import Callable
 
 import numpy as _np
+import random as _random
 import torch as _torch
 from torch.utils.data._utils.collate import default_collate as _default_collate
 
 LOG_FREQ = 100
 
 
 def _job(total, func, i, f):
@@ -46,14 +47,15 @@
         loader_args['batch_size'] = loader_args['batch_size'] // conf['num_gpus']
     return loader_args['batch_size']
 
 
 def seed_worker(worker_id):
     seed = (int(_torch.initial_seed()) + worker_id) % (2 ** 32 - 1)
     _np.random.seed(seed)
+    _random.seed(seed)
 
 
 def _et_data_job(file, mode, conf, dataset_cls, diskcache):
     dataset = dataset_cls(mode=mode, **conf)
     try:
         dataset.add(files=[file], diskcache=diskcache, verbose=False)
     except Exception as e:
```

### Comparing `easytorch-3.7.7/easytorch/easytorch.py` & `easytorch-3.7.8/easytorch/easytorch.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.7/easytorch/metrics/loss.py` & `easytorch-3.7.8/easytorch/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.7/easytorch/metrics/metrics.py` & `easytorch-3.7.8/easytorch/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.7/easytorch/runner.py` & `easytorch-3.7.8/easytorch/runner.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.7/easytorch/utils/__init__.py` & `easytorch-3.7.8/easytorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.7/easytorch/utils/ddp_check.py` & `easytorch-3.7.8/easytorch/utils/ddp_check.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.7/easytorch/utils/tensorutils.py` & `easytorch-3.7.8/easytorch/utils/tensorutils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.7/easytorch/vision/imageutils.py` & `easytorch-3.7.8/easytorch/vision/imageutils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.7/easytorch/vision/plotter.py` & `easytorch-3.7.8/easytorch/vision/plotter.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.7/easytorch/vision/transforms.py` & `easytorch-3.7.8/easytorch/vision/transforms.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.7/easytorch.egg-info/PKG-INFO` & `easytorch-3.7.8/easytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytorch
-Version: 3.7.7
+Version: 3.7.8
 Summary: Easy Neural Network Experiments with pytorch
 Home-page: https://github.com/sraashis/easytorch
 Author: Aashis Khana1
 Author-email: sraashis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `easytorch-3.7.7/easytorch.egg-info/SOURCES.txt` & `easytorch-3.7.8/easytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.7/setup.py` & `easytorch-3.7.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     import cv2
 except:
     _requires.append('opencv-contrib-python-headless')
 
 # This call to setup() does all the work
 setup(
     name="easytorch",
-    version="3.7.7",
+    version="3.7.8",
     description="Easy Neural Network Experiments with pytorch",
     long_description=_README,
     long_description_content_type="text/markdown",
     url="https://github.com/sraashis/easytorch",
     author="Aashis Khana1",
     author_email="sraashis@gmail.com",
     license="MIT",
```

