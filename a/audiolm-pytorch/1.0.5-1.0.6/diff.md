# Comparing `tmp/audiolm-pytorch-1.0.5.tar.gz` & `tmp/audiolm-pytorch-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiolm-pytorch-1.0.5.tar", last modified: Thu May 25 01:45:34 2023, max compression
+gzip compressed data, was "audiolm-pytorch-1.0.6.tar", last modified: Thu May 25 01:46:47 2023, max compression
```

## Comparing `audiolm-pytorch-1.0.5.tar` & `audiolm-pytorch-1.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:45:34.470135 audiolm-pytorch-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-25 01:45:23.000000 audiolm-pytorch-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-25 01:45:34.470135 audiolm-pytorch-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-05-25 01:45:23.000000 audiolm-pytorch-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:45:34.470135 audiolm-pytorch-1.0.5/audiolm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-25 01:45:23.000000 audiolm-pytorch-1.0.5/audiolm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65656 2023-05-25 01:45:23.000000 audiolm-pytorch-1.0.5/audiolm_pytorch/audiolm_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-05-25 01:45:23.000000 audiolm-pytorch-1.0.5/audiolm_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-25 01:45:23.000000 audiolm-pytorch-1.0.5/audiolm_pytorch/encodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-25 01:45:23.000000 audiolm-pytorch-1.0.5/audiolm_pytorch/hubert_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-25 01:45:23.000000 audiolm-pytorch-1.0.5/audiolm_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30110 2023-05-25 01:45:23.000000 audiolm-pytorch-1.0.5/audiolm_pytorch/soundstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-25 01:45:23.000000 audiolm-pytorch-1.0.5/audiolm_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)    42310 2023-05-25 01:45:23.000000 audiolm-pytorch-1.0.5/audiolm_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-25 01:45:23.000000 audiolm-pytorch-1.0.5/audiolm_pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 01:45:23.000000 audiolm-pytorch-1.0.5/audiolm_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-25 01:45:23.000000 audiolm-pytorch-1.0.5/audiolm_pytorch/vq_wav2vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:45:34.470135 audiolm-pytorch-1.0.5/audiolm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-25 01:45:34.000000 audiolm-pytorch-1.0.5/audiolm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-25 01:45:34.000000 audiolm-pytorch-1.0.5/audiolm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 01:45:34.000000 audiolm-pytorch-1.0.5/audiolm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-25 01:45:34.000000 audiolm-pytorch-1.0.5/audiolm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 01:45:34.000000 audiolm-pytorch-1.0.5/audiolm_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 01:45:34.470135 audiolm-pytorch-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-25 01:45:23.000000 audiolm-pytorch-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:46:47.122420 audiolm-pytorch-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-25 01:46:47.122420 audiolm-pytorch-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:46:47.122420 audiolm-pytorch-1.0.6/audiolm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65656 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/audiolm_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/encodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/hubert_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30165 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/soundstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42310 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/vq_wav2vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:46:47.122420 audiolm-pytorch-1.0.6/audiolm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-25 01:46:47.000000 audiolm-pytorch-1.0.6/audiolm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-25 01:46:47.000000 audiolm-pytorch-1.0.6/audiolm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 01:46:47.000000 audiolm-pytorch-1.0.6/audiolm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-25 01:46:47.000000 audiolm-pytorch-1.0.6/audiolm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 01:46:47.000000 audiolm-pytorch-1.0.6/audiolm_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 01:46:47.122420 audiolm-pytorch-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/setup.py
```

### Comparing `audiolm-pytorch-1.0.5/LICENSE` & `audiolm-pytorch-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.5/PKG-INFO` & `audiolm-pytorch-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.0.5
+Version: 1.0.6
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.0.5/README.md` & `audiolm-pytorch-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.5/audiolm_pytorch/__init__.py` & `audiolm-pytorch-1.0.6/audiolm_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.5/audiolm_pytorch/audiolm_pytorch.py` & `audiolm-pytorch-1.0.6/audiolm_pytorch/audiolm_pytorch.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.5/audiolm_pytorch/data.py` & `audiolm-pytorch-1.0.6/audiolm_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.5/audiolm_pytorch/encodec.py` & `audiolm-pytorch-1.0.6/audiolm_pytorch/encodec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.5/audiolm_pytorch/hubert_kmeans.py` & `audiolm-pytorch-1.0.6/audiolm_pytorch/hubert_kmeans.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.5/audiolm_pytorch/optimizer.py` & `audiolm-pytorch-1.0.6/audiolm_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.5/audiolm_pytorch/soundstream.py` & `audiolm-pytorch-1.0.6/audiolm_pytorch/soundstream.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,14 +425,15 @@
         codebook_size = 1024,
         rq_num_quantizers = 8,
         rq_commitment_weight = 1.,
         rq_ema_decay = 0.95,
         rq_quantize_dropout_multiple_of = 1,
         rq_groups = 1,
         rq_stochastic_sample_codes = False,
+        rq_kwargs: dict = {},
         input_channels = 1,
         discr_multi_scales = (1, 0.5, 0.25),
         stft_normalized = False,
         enc_cycle_dilations = (1, 3, 9),
         dec_cycle_dilations = (1, 3, 9),
         multi_spectral_window_powers_of_two = tuple(range(6, 12)),
         multi_spectral_n_ffts = 512,
@@ -517,15 +518,16 @@
             decay = rq_ema_decay,
             commitment_weight = rq_commitment_weight,
             quantize_dropout_multiple_of = rq_quantize_dropout_multiple_of,
             kmeans_init = True,
             threshold_ema_dead_code = 2,
             quantize_dropout = True,
             quantize_dropout_cutoff_index = quantize_dropout_cutoff_index,
-            stochastic_sample_codes = rq_stochastic_sample_codes
+            stochastic_sample_codes = rq_stochastic_sample_codes,
+            **rq_kwargs
         )
 
         self.decoder_film = FiLM(codebook_dim, dim_cond = 2)
 
         self.decoder_attn = LocalTransformer(**attn_kwargs) if use_local_attn else None
 
         decoder_blocks = []
```

### Comparing `audiolm-pytorch-1.0.5/audiolm_pytorch/t5.py` & `audiolm-pytorch-1.0.6/audiolm_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.5/audiolm_pytorch/trainer.py` & `audiolm-pytorch-1.0.6/audiolm_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.5/audiolm_pytorch/vq_wav2vec.py` & `audiolm-pytorch-1.0.6/audiolm_pytorch/vq_wav2vec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.5/audiolm_pytorch.egg-info/PKG-INFO` & `audiolm-pytorch-1.0.6/audiolm_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.0.5
+Version: 1.0.6
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.0.5/audiolm_pytorch.egg-info/SOURCES.txt` & `audiolm-pytorch-1.0.6/audiolm_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.5/setup.py` & `audiolm-pytorch-1.0.6/setup.py`

 * *Files identical despite different names*

