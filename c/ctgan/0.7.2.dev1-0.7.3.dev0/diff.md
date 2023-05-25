# Comparing `tmp/ctgan-0.7.2.dev1.tar.gz` & `tmp/ctgan-0.7.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctgan-0.7.2.dev1.tar", last modified: Tue May  9 15:15:15 2023, max compression
+gzip compressed data, was "ctgan-0.7.3.dev0.tar", last modified: Thu May 25 00:07:21 2023, max compression
```

## Comparing `ctgan-0.7.2.dev1.tar` & `ctgan-0.7.3.dev0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-09 15:15:15.366927 ctgan-0.7.2.dev1/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       58 2023-01-20 22:22:05.000000 ctgan-0.7.2.dev1/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8300 2022-08-17 21:26:32.000000 ctgan-0.7.2.dev1/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9261 2023-05-09 15:14:33.000000 ctgan-0.7.2.dev1/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4816 2023-01-20 22:22:05.000000 ctgan-0.7.2.dev1/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      265 2022-08-17 21:26:32.000000 ctgan-0.7.2.dev1/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    17473 2023-05-09 15:15:15.367044 ctgan-0.7.2.dev1/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7298 2023-01-20 22:22:05.000000 ctgan-0.7.2.dev1/README.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-09 15:15:15.363144 ctgan-0.7.2.dev1/ctgan/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      319 2023-05-04 17:51:30.000000 ctgan-0.7.2.dev1/ctgan/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4415 2022-10-07 17:29:33.000000 ctgan-0.7.2.dev1/ctgan/__main__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2457 2022-08-17 21:26:32.000000 ctgan-0.7.2.dev1/ctgan/data.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6203 2022-08-17 21:26:32.000000 ctgan-0.7.2.dev1/ctgan/data_sampler.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10417 2023-01-20 22:22:05.000000 ctgan-0.7.2.dev1/ctgan/data_transformer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2023-05-05 17:46:40.000000 ctgan-0.7.2.dev1/ctgan/demo.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-09 15:15:15.365057 ctgan-0.7.2.dev1/ctgan/synthesizers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      258 2022-10-07 17:29:33.000000 ctgan-0.7.2.dev1/ctgan/synthesizers/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5287 2023-02-25 01:28:14.000000 ctgan-0.7.2.dev1/ctgan/synthesizers/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    19056 2023-05-09 00:02:24.000000 ctgan-0.7.2.dev1/ctgan/synthesizers/ctgan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6953 2022-10-07 17:29:33.000000 ctgan-0.7.2.dev1/ctgan/synthesizers/tvae.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-09 15:15:15.364322 ctgan-0.7.2.dev1/ctgan.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    17473 2023-05-09 15:15:15.000000 ctgan-0.7.2.dev1/ctgan.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      922 2023-05-09 15:15:15.000000 ctgan-0.7.2.dev1/ctgan.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-05-09 15:15:15.000000 ctgan-0.7.2.dev1/ctgan.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       46 2023-05-09 15:15:15.000000 ctgan-0.7.2.dev1/ctgan.egg-info/entry_points.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-05-09 15:15:15.000000 ctgan-0.7.2.dev1/ctgan.egg-info/not-zip-safe
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1104 2023-05-09 15:15:15.000000 ctgan-0.7.2.dev1/ctgan.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        6 2023-05-09 15:15:15.000000 ctgan-0.7.2.dev1/ctgan.egg-info/top_level.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1302 2023-05-09 15:15:15.367550 ctgan-0.7.2.dev1/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3426 2023-05-09 15:14:33.000000 ctgan-0.7.2.dev1/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-09 15:15:15.359683 ctgan-0.7.2.dev1/tests/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-09 15:15:15.365381 ctgan-0.7.2.dev1/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       38 2023-05-09 15:14:33.000000 ctgan-0.7.2.dev1/tests/integration/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-09 15:15:15.365885 ctgan-0.7.2.dev1/tests/integration/synthesizer/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       58 2023-05-09 15:14:33.000000 ctgan-0.7.2.dev1/tests/integration/synthesizer/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9212 2023-05-05 17:46:40.000000 ctgan-0.7.2.dev1/tests/integration/synthesizer/test_ctgan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4316 2023-05-04 17:51:33.000000 ctgan-0.7.2.dev1/tests/integration/synthesizer/test_tvae.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1296 2022-08-17 21:26:32.000000 ctgan-0.7.2.dev1/tests/integration/test_data_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-09 15:15:15.366176 ctgan-0.7.2.dev1/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       27 2023-05-09 00:17:46.000000 ctgan-0.7.2.dev1/tests/unit/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-09 15:15:15.366794 ctgan-0.7.2.dev1/tests/unit/synthesizer/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       28 2022-10-07 17:29:33.000000 ctgan-0.7.2.dev1/tests/unit/synthesizer/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3593 2022-08-17 21:26:32.000000 ctgan-0.7.2.dev1/tests/unit/synthesizer/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11121 2022-10-07 17:29:33.000000 ctgan-0.7.2.dev1/tests/unit/synthesizer/test_ctgan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3367 2022-10-07 17:29:33.000000 ctgan-0.7.2.dev1/tests/unit/synthesizer/test_tvae.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    20075 2022-08-17 21:26:32.000000 ctgan-0.7.2.dev1/tests/unit/test_data_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 00:07:21.015591 ctgan-0.7.3.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       58 2023-01-20 22:22:05.000000 ctgan-0.7.3.dev0/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8300 2022-08-17 21:26:32.000000 ctgan-0.7.3.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9261 2023-05-10 22:06:03.000000 ctgan-0.7.3.dev0/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4816 2023-01-20 22:22:05.000000 ctgan-0.7.3.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      265 2022-08-17 21:26:32.000000 ctgan-0.7.3.dev0/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    17473 2023-05-25 00:07:21.015692 ctgan-0.7.3.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7298 2023-01-20 22:22:05.000000 ctgan-0.7.3.dev0/README.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 00:07:21.010539 ctgan-0.7.3.dev0/ctgan/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      319 2023-05-10 22:06:03.000000 ctgan-0.7.3.dev0/ctgan/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4415 2022-10-07 17:29:33.000000 ctgan-0.7.3.dev0/ctgan/__main__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2457 2022-08-17 21:26:32.000000 ctgan-0.7.3.dev0/ctgan/data.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6203 2022-08-17 21:26:32.000000 ctgan-0.7.3.dev0/ctgan/data_sampler.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10417 2023-01-20 22:22:05.000000 ctgan-0.7.3.dev0/ctgan/data_transformer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2023-05-09 17:51:59.000000 ctgan-0.7.3.dev0/ctgan/demo.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 00:07:21.012491 ctgan-0.7.3.dev0/ctgan/synthesizers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      258 2022-10-07 17:29:33.000000 ctgan-0.7.3.dev0/ctgan/synthesizers/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5287 2023-02-25 01:28:14.000000 ctgan-0.7.3.dev0/ctgan/synthesizers/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18827 2023-05-24 23:35:47.000000 ctgan-0.7.3.dev0/ctgan/synthesizers/ctgan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6953 2022-10-07 17:29:33.000000 ctgan-0.7.3.dev0/ctgan/synthesizers/tvae.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 00:07:21.011685 ctgan-0.7.3.dev0/ctgan.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    17473 2023-05-25 00:07:20.000000 ctgan-0.7.3.dev0/ctgan.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      922 2023-05-25 00:07:20.000000 ctgan-0.7.3.dev0/ctgan.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-05-25 00:07:20.000000 ctgan-0.7.3.dev0/ctgan.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       46 2023-05-25 00:07:20.000000 ctgan-0.7.3.dev0/ctgan.egg-info/entry_points.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-05-25 00:07:20.000000 ctgan-0.7.3.dev0/ctgan.egg-info/not-zip-safe
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1098 2023-05-25 00:07:20.000000 ctgan-0.7.3.dev0/ctgan.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        6 2023-05-25 00:07:20.000000 ctgan-0.7.3.dev0/ctgan.egg-info/top_level.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1302 2023-05-25 00:07:21.016137 ctgan-0.7.3.dev0/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3420 2023-05-24 23:35:47.000000 ctgan-0.7.3.dev0/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 00:07:21.007591 ctgan-0.7.3.dev0/tests/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 00:07:21.012985 ctgan-0.7.3.dev0/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       38 2023-05-10 22:06:03.000000 ctgan-0.7.3.dev0/tests/integration/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 00:07:21.013720 ctgan-0.7.3.dev0/tests/integration/synthesizer/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       58 2023-05-10 22:06:03.000000 ctgan-0.7.3.dev0/tests/integration/synthesizer/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9212 2023-05-09 17:51:59.000000 ctgan-0.7.3.dev0/tests/integration/synthesizer/test_ctgan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4316 2023-05-09 17:51:59.000000 ctgan-0.7.3.dev0/tests/integration/synthesizer/test_tvae.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1296 2022-08-17 21:26:32.000000 ctgan-0.7.3.dev0/tests/integration/test_data_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 00:07:21.014228 ctgan-0.7.3.dev0/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       27 2023-05-09 00:17:46.000000 ctgan-0.7.3.dev0/tests/unit/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-25 00:07:21.015403 ctgan-0.7.3.dev0/tests/unit/synthesizer/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       28 2022-10-07 17:29:33.000000 ctgan-0.7.3.dev0/tests/unit/synthesizer/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3593 2022-08-17 21:26:32.000000 ctgan-0.7.3.dev0/tests/unit/synthesizer/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11121 2022-10-07 17:29:33.000000 ctgan-0.7.3.dev0/tests/unit/synthesizer/test_ctgan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3367 2022-10-07 17:29:33.000000 ctgan-0.7.3.dev0/tests/unit/synthesizer/test_tvae.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    20075 2022-08-17 21:26:32.000000 ctgan-0.7.3.dev0/tests/unit/test_data_transformer.py
```

### Comparing `ctgan-0.7.2.dev1/CONTRIBUTING.rst` & `ctgan-0.7.3.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.2.dev1/HISTORY.md` & `ctgan-0.7.3.dev0/HISTORY.md`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.2.dev1/LICENSE` & `ctgan-0.7.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.2.dev1/PKG-INFO` & `ctgan-0.7.3.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctgan
-Version: 0.7.2.dev1
+Version: 0.7.3.dev0
 Summary: Create tabular synthetic data using a conditional GAN
 Home-page: https://github.com/sdv-dev/CTGAN
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: ctgan CTGAN
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ctgan Version: 0.7.2.dev1 Summary: Create tabular
+Metadata-Version: 2.1 Name: ctgan Version: 0.7.3.dev0 Summary: Create tabular
 synthetic data using a conditional GAN Home-page: https://github.com/sdv-dev/
 CTGAN Author: DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1
 Keywords: ctgan CTGAN Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: Free for
 non-commercial use Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `ctgan-0.7.2.dev1/README.md` & `ctgan-0.7.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.2.dev1/ctgan/__main__.py` & `ctgan-0.7.3.dev0/ctgan/__main__.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.2.dev1/ctgan/data.py` & `ctgan-0.7.3.dev0/ctgan/data.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.2.dev1/ctgan/data_sampler.py` & `ctgan-0.7.3.dev0/ctgan/data_sampler.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.2.dev1/ctgan/data_transformer.py` & `ctgan-0.7.3.dev0/ctgan/data_transformer.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.2.dev1/ctgan/synthesizers/base.py` & `ctgan-0.7.3.dev0/ctgan/synthesizers/base.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.2.dev1/ctgan/synthesizers/ctgan.py` & `ctgan-0.7.3.dev0/ctgan/synthesizers/ctgan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """CTGAN module."""
 
 import warnings
 
 import numpy as np
 import pandas as pd
 import torch
-from packaging import version
 from torch import optim
 from torch.nn import BatchNorm1d, Dropout, LeakyReLU, Linear, Module, ReLU, Sequential, functional
 
 from ctgan.data_sampler import DataSampler
 from ctgan.data_transformer import DataTransformer
 from ctgan.synthesizers.base import BaseSynthesizer, random_state
 
@@ -193,23 +192,20 @@
                 but will be differentiated as if it is the soft sample in autograd
             dim (int):
                 A dimension along which softmax will be computed. Default: -1.
 
         Returns:
             Sampled tensor of same shape as logits from the Gumbel-Softmax distribution.
         """
-        if version.parse(torch.__version__) < version.parse('1.2.0'):
-            for i in range(10):
-                transformed = functional.gumbel_softmax(logits, tau=tau, hard=hard,
-                                                        eps=eps, dim=dim)
-                if not torch.isnan(transformed).any():
-                    return transformed
-            raise ValueError('gumbel_softmax returning NaN.')
+        for _ in range(10):
+            transformed = functional.gumbel_softmax(logits, tau=tau, hard=hard, eps=eps, dim=dim)
+            if not torch.isnan(transformed).any():
+                return transformed
 
-        return functional.gumbel_softmax(logits, tau=tau, hard=hard, eps=eps, dim=dim)
+        raise ValueError('gumbel_softmax returning NaN.')
 
     def _apply_activate(self, data):
         """Apply proper activation function to the output of the generator."""
         data_t = []
         st = 0
         for column_info in self._transformer.output_info_list:
             for span_info in column_info:
@@ -377,15 +373,15 @@
                     y_fake = discriminator(fake_cat)
                     y_real = discriminator(real_cat)
 
                     pen = discriminator.calc_gradient_penalty(
                         real_cat, fake_cat, self._device, self.pac)
                     loss_d = -(torch.mean(y_real) - torch.mean(y_fake))
 
-                    optimizerD.zero_grad()
+                    optimizerD.zero_grad(set_to_none=False)
                     pen.backward(retain_graph=True)
                     loss_d.backward()
                     optimizerD.step()
 
                 fakez = torch.normal(mean=mean, std=std)
                 condvec = self._data_sampler.sample_condvec(self._batch_size)
 
@@ -408,15 +404,15 @@
                 if condvec is None:
                     cross_entropy = 0
                 else:
                     cross_entropy = self._cond_loss(fake, c1, m1)
 
                 loss_g = -torch.mean(y_fake) + cross_entropy
 
-                optimizerG.zero_grad()
+                optimizerG.zero_grad(set_to_none=False)
                 loss_g.backward()
                 optimizerG.step()
 
             if self._verbose:
                 print(f'Epoch {i+1}, Loss G: {loss_g.detach().cpu(): .4f},'  # noqa: T001
                       f'Loss D: {loss_d.detach().cpu(): .4f}',
                       flush=True)
```

### Comparing `ctgan-0.7.2.dev1/ctgan/synthesizers/tvae.py` & `ctgan-0.7.3.dev0/ctgan/synthesizers/tvae.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.2.dev1/ctgan.egg-info/PKG-INFO` & `ctgan-0.7.3.dev0/ctgan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctgan
-Version: 0.7.2.dev1
+Version: 0.7.3.dev0
 Summary: Create tabular synthetic data using a conditional GAN
 Home-page: https://github.com/sdv-dev/CTGAN
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: ctgan CTGAN
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ctgan Version: 0.7.2.dev1 Summary: Create tabular
+Metadata-Version: 2.1 Name: ctgan Version: 0.7.3.dev0 Summary: Create tabular
 synthetic data using a conditional GAN Home-page: https://github.com/sdv-dev/
 CTGAN Author: DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1
 Keywords: ctgan CTGAN Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: Free for
 non-commercial use Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `ctgan-0.7.2.dev1/ctgan.egg-info/SOURCES.txt` & `ctgan-0.7.3.dev0/ctgan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.2.dev1/ctgan.egg-info/requires.txt` & `ctgan-0.7.3.dev0/ctgan.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 packaging<22,>=20
 rdt<2.0,>=1.3.0
 
 [:python_version < "3.10"]
 numpy<2,>=1.20.0
 pandas>=1.1.3
-torch<2,>=1.8.0
+torch>=1.8.0
 
 [:python_version >= "3.10"]
 numpy<2,>=1.23.3
 pandas>=1.3.4
 scikit-learn<2,>=1.1.3
-torch<2,>=1.11.0
+torch>=1.11.0
 
 [dev]
 pip>=9.0.1
 bumpversion<0.6,>=0.5.3
 watchdog<0.11,>=0.8.3
 flake8<4,>=3.7.7
 isort<5,>=4.3.4
```

### Comparing `ctgan-0.7.2.dev1/setup.cfg` & `ctgan-0.7.3.dev0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.7.2.dev1
+current_version = 0.7.3.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `ctgan-0.7.2.dev1/setup.py` & `ctgan-0.7.3.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 install_requires = [
     'packaging>=20,<22',
     "numpy>=1.20.0,<2;python_version<'3.10'",
     "numpy>=1.23.3,<2;python_version>='3.10'",
     "pandas>=1.1.3;python_version<'3.10'",
     "pandas>=1.3.4;python_version>='3.10'",
     "scikit-learn>=1.1.3,<2;python_version>='3.10'",
-    "torch>=1.8.0,<2;python_version<'3.10'",
-    "torch>=1.11.0,<2;python_version>='3.10'",
+    "torch>=1.8.0;python_version<'3.10'",
+    "torch>=1.11.0;python_version>='3.10'",
     'rdt>=1.3.0,<2.0',
 ]
 
 setup_requires = [
     'pytest-runner>=2.11.1',
 ]
 
@@ -113,10 +113,10 @@
     name='ctgan',
     packages=find_packages(include=['ctgan', 'ctgan.*']),
     python_requires='>=3.7,<3.11',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/CTGAN',
-    version='0.7.2.dev1',
+    version='0.7.3.dev0',
     zip_safe=False,
 )
```

### Comparing `ctgan-0.7.2.dev1/tests/integration/synthesizer/test_ctgan.py` & `ctgan-0.7.3.dev0/tests/integration/synthesizer/test_ctgan.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.2.dev1/tests/integration/synthesizer/test_tvae.py` & `ctgan-0.7.3.dev0/tests/integration/synthesizer/test_tvae.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.2.dev1/tests/integration/test_data_transformer.py` & `ctgan-0.7.3.dev0/tests/integration/test_data_transformer.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.2.dev1/tests/unit/synthesizer/test_base.py` & `ctgan-0.7.3.dev0/tests/unit/synthesizer/test_base.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.2.dev1/tests/unit/synthesizer/test_ctgan.py` & `ctgan-0.7.3.dev0/tests/unit/synthesizer/test_ctgan.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.2.dev1/tests/unit/synthesizer/test_tvae.py` & `ctgan-0.7.3.dev0/tests/unit/synthesizer/test_tvae.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.7.2.dev1/tests/unit/test_data_transformer.py` & `ctgan-0.7.3.dev0/tests/unit/test_data_transformer.py`

 * *Files identical despite different names*

