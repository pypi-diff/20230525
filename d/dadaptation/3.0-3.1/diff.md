# Comparing `tmp/dadaptation-3.0.tar.gz` & `tmp/dadaptation-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dadaptation-3.0.tar", last modified: Mon May 22 15:06:30 2023, max compression
+gzip compressed data, was "dadaptation-3.1.tar", last modified: Thu May 25 14:32:34 2023, max compression
```

## Comparing `dadaptation-3.0.tar` & `dadaptation-3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-05-22 15:06:30.000000 dadaptation-3.0/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     1091 2023-01-09 18:27:36.000000 dadaptation-3.0/LICENSE
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3327 2023-05-22 15:06:30.000000 dadaptation-3.0/PKG-INFO
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     2829 2023-05-22 15:04:09.000000 dadaptation-3.0/README.md
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-05-22 15:06:30.000000 dadaptation-3.0/dadaptation/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      184 2023-05-22 15:03:35.000000 dadaptation-3.0/dadaptation/__init__.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9568 2023-05-22 15:03:35.000000 dadaptation-3.0/dadaptation/dadapt_adagrad.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     8764 2023-05-22 15:03:35.000000 dadaptation-3.0/dadaptation/dadapt_adam.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9511 2023-05-22 15:03:35.000000 dadaptation-3.0/dadaptation/dadapt_adan.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5309 2023-05-22 15:03:35.000000 dadaptation-3.0/dadaptation/dadapt_lion.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6974 2023-05-22 15:03:35.000000 dadaptation-3.0/dadaptation/dadapt_sgd.py
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-05-22 15:06:30.000000 dadaptation-3.0/dadaptation/experimental/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       94 2023-05-22 15:03:35.000000 dadaptation-3.0/dadaptation/experimental/__init__.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9113 2023-05-22 15:03:35.000000 dadaptation-3.0/dadaptation/experimental/dadapt_adam_preprint.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9737 2023-04-17 18:47:49.000000 dadaptation-3.0/dadaptation/experimental/dadapt_adan_ip.py
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-05-22 15:06:30.000000 dadaptation-3.0/dadaptation.egg-info/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3327 2023-05-22 15:06:29.000000 dadaptation-3.0/dadaptation.egg-info/PKG-INFO
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      471 2023-05-22 15:06:29.000000 dadaptation-3.0/dadaptation.egg-info/SOURCES.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)        1 2023-05-22 15:06:29.000000 dadaptation-3.0/dadaptation.egg-info/dependency_links.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       12 2023-05-22 15:06:29.000000 dadaptation-3.0/dadaptation.egg-info/top_level.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      304 2023-01-20 15:51:35.000000 dadaptation-3.0/pyproject.toml
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       38 2023-05-22 15:06:30.000000 dadaptation-3.0/setup.cfg
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      895 2023-05-22 15:03:35.000000 dadaptation-3.0/setup.py
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-05-25 14:32:34.805770 dadaptation-3.1/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     1091 2023-01-09 18:27:36.000000 dadaptation-3.1/LICENSE
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3492 2023-05-25 14:32:34.804382 dadaptation-3.1/PKG-INFO
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3031 2023-05-23 17:04:15.000000 dadaptation-3.1/README.md
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-05-25 14:32:34.769946 dadaptation-3.1/dadaptation/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      384 2023-05-23 17:05:19.000000 dadaptation-3.1/dadaptation/__init__.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9568 2023-05-22 15:03:35.000000 dadaptation-3.1/dadaptation/dadapt_adagrad.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     8767 2023-05-23 13:59:13.000000 dadaptation-3.1/dadaptation/dadapt_adam.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9614 2023-05-25 14:31:43.000000 dadaptation-3.1/dadaptation/dadapt_adan.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5596 2023-05-25 14:31:43.000000 dadaptation-3.1/dadaptation/dadapt_lion.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6973 2023-05-25 14:31:43.000000 dadaptation-3.1/dadaptation/dadapt_sgd.py
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-05-25 14:32:34.799203 dadaptation-3.1/dadaptation/experimental/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      294 2023-05-23 17:04:57.000000 dadaptation-3.1/dadaptation/experimental/__init__.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9113 2023-05-22 15:03:35.000000 dadaptation-3.1/dadaptation/experimental/dadapt_adam_preprint.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9737 2023-04-17 18:47:49.000000 dadaptation-3.1/dadaptation/experimental/dadapt_adan_ip.py
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-05-25 14:32:34.786750 dadaptation-3.1/dadaptation.egg-info/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3492 2023-05-25 14:32:34.000000 dadaptation-3.1/dadaptation.egg-info/PKG-INFO
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      471 2023-05-25 14:32:34.000000 dadaptation-3.1/dadaptation.egg-info/SOURCES.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)        1 2023-05-25 14:32:34.000000 dadaptation-3.1/dadaptation.egg-info/dependency_links.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       12 2023-05-25 14:32:34.000000 dadaptation-3.1/dadaptation.egg-info/top_level.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      304 2023-01-20 15:51:35.000000 dadaptation-3.1/pyproject.toml
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       38 2023-05-25 14:32:34.806766 dadaptation-3.1/setup.cfg
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      895 2023-05-25 14:31:43.000000 dadaptation-3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dadaptation-3.0/LICENSE` & `dadaptation-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dadaptation-3.0/PKG-INFO` & `dadaptation-3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: dadaptation
-Version: 3.0
+Version: 3.1
 Summary: Learning Rate Free Learning for Adam, SGD and AdaGrad
 Home-page: https://github.com/facebookresearch/dadaptation
 Author: Aaron Defazio
 Author-email: adefazio@meta.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # D-Adaptation
+[![Downloads](https://static.pepy.tech/badge/dadaptation)](https://pepy.tech/project/dadaptation) [![Downloads](https://static.pepy.tech/badge/dadaptation/month)](https://pepy.tech/project/dadaptation)
 
 Learning rate free learning for SGD, AdaGrad and Adam! 
 
 *by Aaron Defazio and Konstantin Mishchenko [(Arxiv)](https://arxiv.org/abs/2301.07733)*
 
 ``` pip install dadaptation ```
 
@@ -60,9 +59,7 @@
 ![vision](figures/dadapt_gpt.png)
 ![vision](figures/dadapt_fastmri.png)
 ![vision](figures/dadapt_detectron.png)
 ![vision](figures/dadapt_dlrm.png)
 
 # License
 See the [License file](/LICENSE).
-
-
```

### Comparing `dadaptation-3.0/README.md` & `dadaptation-3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # D-Adaptation
+[![Downloads](https://static.pepy.tech/badge/dadaptation)](https://pepy.tech/project/dadaptation) [![Downloads](https://static.pepy.tech/badge/dadaptation/month)](https://pepy.tech/project/dadaptation)
 
 Learning rate free learning for SGD, AdaGrad and Adam! 
 
 *by Aaron Defazio and Konstantin Mishchenko [(Arxiv)](https://arxiv.org/abs/2301.07733)*
 
 ``` pip install dadaptation ```
```

### Comparing `dadaptation-3.0/dadaptation/dadapt_adagrad.py` & `dadaptation-3.1/dadaptation/dadapt_adagrad.py`

 * *Files identical despite different names*

### Comparing `dadaptation-3.0/dadaptation/dadapt_adam.py` & `dadaptation-3.1/dadaptation/dadapt_adam.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         params (iterable): 
             Iterable of parameters to optimize or dicts defining parameter groups.
         lr (float): 
             Learning rate adjustment parameter. Increases or decreases the D-adapted learning rate.
         betas (Tuple[float, float], optional): coefficients used for computing
             running averages of gradient and its square (default: (0.9, 0.999))
         eps (float): 
-            Term added to the denominator outside of the root operation to improve numerical stability. (default: 0).
+            Term added to the denominator outside of the root operation to improve numerical stability. (default: 1e-8).
         weight_decay (float): 
             Weight decay, i.e. a L2 penalty (default: 0).
         log_every (int): 
             Log using print every k steps, default 0 (no logging).
         decouple (boolean): 
             Use AdamW style decoupled weight decay
         use_bias_correction (boolean):
```

### Comparing `dadaptation-3.0/dadaptation/dadapt_adan.py` & `dadaptation-3.1/dadaptation/dadapt_adan.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,22 @@
         return x.real
     else:
         return x
 
 
 class DAdaptAdan(torch.optim.Optimizer):
     r"""
-    Implements Adan with D-Adaptation automatic step-sizes. Leave LR set to 1 unless you encounter instability.
+    Implements Adan with D-Adaptation automatic step-sizes. 
+    Has not been as heavily tested as DAdaptAdam and should be considered experimental.
+    
+    Leave LR set to 1 unless you encounter instability.
     Adan was proposed in
     Adan: Adaptive Nesterov Momentum Algorithm for Faster Optimizing Deep Models[J]. arXiv preprint arXiv:2208.06677, 2022.
     https://arxiv.org/abs/2208.06677
+    
     Arguments:
         params (iterable): 
             Iterable of parameters to optimize or dicts defining parameter groups.
         lr (float): 
             Learning rate adjustment parameter. Increases or decreases the D-adapted learning rate.
         betas (Tuple[float, float, flot], optional): coefficients used for computing
             running averages of gradient and its norm. (default: (0.98, 0.92, 0.99))
```

### Comparing `dadaptation-3.0/dadaptation/dadapt_lion.py` & `dadaptation-3.1/dadaptation/dadapt_lion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,28 @@
+# Copyright (c) Meta Platforms, Inc. and affiliates.
+# All rights reserved.
+# 
+# This source code is licensed under the license found in the
+# LICENSE file in the root directory of this source tree.
+
 from typing import Tuple, Optional, Callable
 
 import torch
 from torch.optim.optimizer import Optimizer
 import torch.distributed as dist
 import logging
 import pdb
 
 class DAdaptLion(Optimizer):
     r"""
-    Implements Adam with D-Adaptation automatic step-sizes. Leave LR set to 1 unless you encounter instability.
+    Implements Lion with D-Adaptation automatic step-sizes. 
+    Has not been as heavily tested as DAdaptAdam and should be considered experimental.
+    
+    
+    Leave LR set to 1 unless you encounter instability.
     Arguments:
         params (iterable): 
             Iterable of parameters to optimize or dicts defining parameter groups.
         lr (float): 
             Learning rate adjustment parameter. Increases or decreases the D-adapted learning rate.
         betas (Tuple[float, float], optional): coefficients used for computing
             running averages of gradient and its square (default: (0.9, 0.999))
@@ -88,15 +98,14 @@
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 state = self.state[p]
 
                 if 'exp_avg' not in state:
-                    print("Initializing")
                     state['exp_avg'] = torch.zeros_like(p).detach()
                     state['s'] = torch.zeros_like(p).detach()
 
                 exp_avg = state['exp_avg']
                 s = state['s']
 
                 #AdamW style weight decay
@@ -111,15 +120,16 @@
                 numerator_acum += dlr * torch.dot(update.flatten(), s.flatten()).item()
                 
                 s.mul_(sqrt_beta2).add_(update, alpha=(1-sqrt_beta2)*dlr)
                 
                 sk_l1 += s.abs().sum().item()
 
         numerator_weighted = sqrt_beta2*numerator_weighted + (1-sqrt_beta2)*numerator_acum
-
+        d_hat = d
+        
         # if we have not done any progres, return
         # if we have any gradients available, will have sk_l1 > 0 (unless \|g\|=0)
         if sk_l1 == 0:
             return loss
         
         if lr > 0.0:
             if fsdp_in_use:
```

### Comparing `dadaptation-3.0/dadaptation/dadapt_sgd.py` & `dadaptation-3.1/dadaptation/dadapt_sgd.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import pdb
 import math
 import logging
 import torch.distributed as dist
 
 class DAdaptSGD(torch.optim.Optimizer):
     r"""
-    Implements Adam with D-Adaptation automatic step-sizes. Leave LR set to 1 unless you encounter instability.
+    Implements SGD with D-Adaptation automatic step-sizes. Leave LR set to 1 unless you encounter instability.
 
     Arguments:
         params (iterable): 
             Iterable of parameters to optimize or dicts defining parameter groups.
         lr (float): 
             Learning rate adjustment parameter. Increases or decreases the D-adapted learning rate.
         momentum (float):
```

### Comparing `dadaptation-3.0/dadaptation/experimental/dadapt_adam_preprint.py` & `dadaptation-3.1/dadaptation/experimental/dadapt_adam_preprint.py`

 * *Files identical despite different names*

### Comparing `dadaptation-3.0/dadaptation/experimental/dadapt_adan_ip.py` & `dadaptation-3.1/dadaptation/experimental/dadapt_adan_ip.py`

 * *Files identical despite different names*

### Comparing `dadaptation-3.0/dadaptation.egg-info/PKG-INFO` & `dadaptation-3.1/dadaptation.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: dadaptation
-Version: 3.0
+Version: 3.1
 Summary: Learning Rate Free Learning for Adam, SGD and AdaGrad
 Home-page: https://github.com/facebookresearch/dadaptation
 Author: Aaron Defazio
 Author-email: adefazio@meta.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # D-Adaptation
+[![Downloads](https://static.pepy.tech/badge/dadaptation)](https://pepy.tech/project/dadaptation) [![Downloads](https://static.pepy.tech/badge/dadaptation/month)](https://pepy.tech/project/dadaptation)
 
 Learning rate free learning for SGD, AdaGrad and Adam! 
 
 *by Aaron Defazio and Konstantin Mishchenko [(Arxiv)](https://arxiv.org/abs/2301.07733)*
 
 ``` pip install dadaptation ```
 
@@ -60,9 +59,7 @@
 ![vision](figures/dadapt_gpt.png)
 ![vision](figures/dadapt_fastmri.png)
 ![vision](figures/dadapt_detectron.png)
 ![vision](figures/dadapt_dlrm.png)
 
 # License
 See the [License file](/LICENSE).
-
-
```

### Comparing `dadaptation-3.0/setup.py` & `dadaptation-3.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dadaptation",
-    version="3.0",
+    version="3.1",
     author="Aaron Defazio",
     author_email="adefazio@meta.com",
     description="Learning Rate Free Learning for Adam, SGD and AdaGrad",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/facebookresearch/dadaptation",
     packages=setuptools.find_packages(),
```

