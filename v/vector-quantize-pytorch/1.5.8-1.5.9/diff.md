# Comparing `tmp/vector_quantize_pytorch-1.5.8.tar.gz` & `tmp/vector_quantize_pytorch-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.5.8.tar", last modified: Wed May 24 14:28:34 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.5.9.tar", last modified: Wed May 24 16:45:35 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.5.8.tar` & `vector_quantize_pytorch-1.5.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:28:34.000207 vector_quantize_pytorch-1.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-24 14:28:20.000000 vector_quantize_pytorch-1.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-24 14:28:34.000207 vector_quantize_pytorch-1.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-05-24 14:28:20.000000 vector_quantize_pytorch-1.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 14:28:34.000207 vector_quantize_pytorch-1.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-24 14:28:20.000000 vector_quantize_pytorch-1.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:28:34.000207 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-24 14:28:20.000000 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-24 14:28:20.000000 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-24 14:28:20.000000 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    24652 2023-05-24 14:28:20.000000 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:28:34.000207 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-24 14:28:33.000000 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-24 14:28:33.000000 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:28:33.000000 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 14:28:33.000000 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-24 14:28:33.000000 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:45:35.015181 vector_quantize_pytorch-1.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-24 16:45:21.000000 vector_quantize_pytorch-1.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-24 16:45:35.015181 vector_quantize_pytorch-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-05-24 16:45:21.000000 vector_quantize_pytorch-1.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:45:35.015181 vector_quantize_pytorch-1.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-24 16:45:21.000000 vector_quantize_pytorch-1.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:45:35.011181 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-24 16:45:21.000000 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-24 16:45:21.000000 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-24 16:45:21.000000 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25918 2023-05-24 16:45:21.000000 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:45:35.015181 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-24 16:45:34.000000 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-24 16:45:34.000000 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:45:34.000000 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 16:45:34.000000 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-24 16:45:34.000000 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.5.8/LICENSE` & `vector_quantize_pytorch-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.8/PKG-INFO` & `vector_quantize_pytorch-1.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.5.8
+Version: 1.5.9
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.5.8/README.md` & `vector_quantize_pytorch-1.5.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -66,16 +66,17 @@
 import torch
 from vector_quantize_pytorch import ResidualVQ
 
 residual_vq = ResidualVQ(
     dim = 256,
     num_quantizers = 8,
     codebook_size = 1024,
-    sample_codebook_temp = 0.1, # temperature for stochastically sampling codes, 0 would be equivalent to non-stochastic
-    shared_codebook = True      # whether to share the codebooks for all quantizers or not
+    stochastic_sample_codes = True,
+    sample_codebook_temp = 0.1,         # temperature for stochastically sampling codes, 0 would be equivalent to non-stochastic
+    shared_codebook = True              # whether to share the codebooks for all quantizers or not
 )
 
 x = torch.randn(1, 1024, 256)
 quantized, indices, commit_loss = residual_vq(x)
 
 # (1, 1024, 256), (8, 1, 1024), (8, 1)
 # (batch, seq, dim), (quantizer, batch, seq), (quantizer, batch)
@@ -402,7 +403,16 @@
 @inproceedings{Yang2023HiFiCodecGV,
     title   = {HiFi-Codec: Group-residual Vector quantization for High Fidelity Audio Codec},
     author  = {Dongchao Yang and Songxiang Liu and Rongjie Huang and Jinchuan Tian and Chao Weng and Yuexian Zou},
     year    = {2023}
 }
 ```
 
+```bibtex
+@article{Liu2023BridgingDA,
+    title   = {Bridging Discrete and Backpropagation: Straight-Through and Beyond},
+    author  = {Liyuan Liu and Chengyu Dong and Xiaodong Liu and Bin Yu and Jianfeng Gao},
+    journal = {ArXiv},
+    year    = {2023},
+    volume  = {abs/2304.08612}
+}
+```
```

#### html2text {}

```diff
@@ -23,51 +23,52 @@
 Furthermore, this_paper uses Residual-VQ to construct the RQ-VAE, for
 generating high resolution images with more compressed codes. They make two
 modifications. The first is to share the codebook across all quantizers. The
 second is to stochastically sample the codes rather than always taking the
 closest match. You can use both of these features with two extra keyword
 arguments. ```python import torch from vector_quantize_pytorch import
 ResidualVQ residual_vq = ResidualVQ( dim = 256, num_quantizers = 8,
-codebook_size = 1024, sample_codebook_temp = 0.1, # temperature for
-stochastically sampling codes, 0 would be equivalent to non-stochastic
-shared_codebook = True # whether to share the codebooks for all quantizers or
-not ) x = torch.randn(1, 1024, 256) quantized, indices, commit_loss =
-residual_vq(x) # (1, 1024, 256), (8, 1, 1024), (8, 1) # (batch, seq, dim),
-(quantizer, batch, seq), (quantizer, batch) ``` A_recent_paper further proposes
-to do residual VQ on groups of the feature dimension, showing equivalent
-results to Encodec while using far fewer codebooks. You can use it by importing
-`GroupedResidualVQ` ```python import torch from vector_quantize_pytorch import
-GroupedResidualVQ residual_vq = GroupedResidualVQ( dim = 256, num_quantizers =
-8, # specify number of quantizers groups = 2, codebook_size = 1024, # codebook
-size ) x = torch.randn(1, 1024, 256) quantized, indices, commit_loss =
-residual_vq(x) # (1, 1024, 256), (1, 1024, 8), (1, 8) # (batch, seq, dim),
-(groups, batch, seq, quantizer), (groups, batch, quantizer) ``` ##
-Initialization The SoundStream paper proposes that the codebook should be
-initialized by the kmeans centroids of the first batch. You can easily turn on
-this feature with one flag `kmeans_init = True`, for either `VectorQuantize` or
-`ResidualVQ` class ```python import torch from vector_quantize_pytorch import
-ResidualVQ residual_vq = ResidualVQ( dim = 256, codebook_size = 256,
-num_quantizers = 4, kmeans_init = True, # set to True kmeans_iters = 10 #
-number of kmeans iterations to calculate the centroids for the codebook on init
-) x = torch.randn(1, 1024, 256) quantized, indices, commit_loss = residual_vq
-(x) ``` ## Increasing codebook usage This repository will contain a few
-techniques from various papers to combat "dead" codebook entries, which is a
-common problem when using vector quantizers. ### Lower codebook dimension The
-Improved_VQGAN_paper proposes to have the codebook kept in a lower dimension.
-The encoder values are projected down before being projected back to high
-dimensional after quantization. You can set this with the `codebook_dim`
-hyperparameter. ```python import torch from vector_quantize_pytorch import
-VectorQuantize vq = VectorQuantize( dim = 256, codebook_size = 256,
-codebook_dim = 16 # paper proposes setting this to 32 or as low as 8 to
-increase codebook usage ) x = torch.randn(1, 1024, 256) quantized, indices,
-commit_loss = vq(x) ``` ### Cosine similarity The Improved_VQGAN_paper also
-proposes to l2 normalize the codes and the encoded vectors, which boils down to
-using cosine similarity for the distance. They claim enforcing the vectors on a
-sphere leads to improvements in code usage and downstream reconstruction. You
-can turn this on by setting `use_cosine_sim = True` ```python import torch from
+codebook_size = 1024, stochastic_sample_codes = True, sample_codebook_temp =
+0.1, # temperature for stochastically sampling codes, 0 would be equivalent to
+non-stochastic shared_codebook = True # whether to share the codebooks for all
+quantizers or not ) x = torch.randn(1, 1024, 256) quantized, indices,
+commit_loss = residual_vq(x) # (1, 1024, 256), (8, 1, 1024), (8, 1) # (batch,
+seq, dim), (quantizer, batch, seq), (quantizer, batch) ``` A_recent_paper
+further proposes to do residual VQ on groups of the feature dimension, showing
+equivalent results to Encodec while using far fewer codebooks. You can use it
+by importing `GroupedResidualVQ` ```python import torch from
+vector_quantize_pytorch import GroupedResidualVQ residual_vq =
+GroupedResidualVQ( dim = 256, num_quantizers = 8, # specify number of
+quantizers groups = 2, codebook_size = 1024, # codebook size ) x = torch.randn
+(1, 1024, 256) quantized, indices, commit_loss = residual_vq(x) # (1, 1024,
+256), (1, 1024, 8), (1, 8) # (batch, seq, dim), (groups, batch, seq,
+quantizer), (groups, batch, quantizer) ``` ## Initialization The SoundStream
+paper proposes that the codebook should be initialized by the kmeans centroids
+of the first batch. You can easily turn on this feature with one flag
+`kmeans_init = True`, for either `VectorQuantize` or `ResidualVQ` class
+```python import torch from vector_quantize_pytorch import ResidualVQ
+residual_vq = ResidualVQ( dim = 256, codebook_size = 256, num_quantizers = 4,
+kmeans_init = True, # set to True kmeans_iters = 10 # number of kmeans
+iterations to calculate the centroids for the codebook on init ) x =
+torch.randn(1, 1024, 256) quantized, indices, commit_loss = residual_vq(x) ```
+## Increasing codebook usage This repository will contain a few techniques from
+various papers to combat "dead" codebook entries, which is a common problem
+when using vector quantizers. ### Lower codebook dimension The Improved_VQGAN
+paper proposes to have the codebook kept in a lower dimension. The encoder
+values are projected down before being projected back to high dimensional after
+quantization. You can set this with the `codebook_dim` hyperparameter.
+```python import torch from vector_quantize_pytorch import VectorQuantize vq =
+VectorQuantize( dim = 256, codebook_size = 256, codebook_dim = 16 # paper
+proposes setting this to 32 or as low as 8 to increase codebook usage ) x =
+torch.randn(1, 1024, 256) quantized, indices, commit_loss = vq(x) ``` ###
+Cosine similarity The Improved_VQGAN_paper also proposes to l2 normalize the
+codes and the encoded vectors, which boils down to using cosine similarity for
+the distance. They claim enforcing the vectors on a sphere leads to
+improvements in code usage and downstream reconstruction. You can turn this on
+by setting `use_cosine_sim = True` ```python import torch from
 vector_quantize_pytorch import VectorQuantize vq = VectorQuantize( dim = 256,
 codebook_size = 256, use_cosine_sim = True # set this to True ) x = torch.randn
 (1, 1024, 256) quantized, indices, commit_loss = vq(x) ``` ### Expiring stale
 codes Finally, the SoundStream paper has a scheme where they replace codes that
 have hits below a certain threshold with randomly selected vector from the
 current batch. You can set this threshold with `threshold_ema_dead_code`
 keyword. ```python import torch from vector_quantize_pytorch import
@@ -174,8 +175,12 @@
 ```bibtex @inproceedings{Shen2023NaturalSpeech2L, title = {NaturalSpeech 2:
 Latent Diffusion Models are Natural and Zero-Shot Speech and Singing
 Synthesizers}, author = {Kai Shen and Zeqian Ju and Xu Tan and Yanqing Liu and
 Yichong Leng and Lei He and Tao Qin and Sheng Zhao and Jiang Bian}, year =
 {2023} } ``` ```bibtex @inproceedings{Yang2023HiFiCodecGV, title = {HiFi-Codec:
 Group-residual Vector quantization for High Fidelity Audio Codec}, author =
 {Dongchao Yang and Songxiang Liu and Rongjie Huang and Jinchuan Tian and Chao
-Weng and Yuexian Zou}, year = {2023} } ```
+Weng and Yuexian Zou}, year = {2023} } ``` ```bibtex @article
+{Liu2023BridgingDA, title = {Bridging Discrete and Backpropagation: Straight-
+Through and Beyond}, author = {Liyuan Liu and Chengyu Dong and Xiaodong Liu and
+Bin Yu and Jianfeng Gao}, journal = {ArXiv}, year = {2023}, volume = {abs/
+2304.08612} } ```
```

### Comparing `vector_quantize_pytorch-1.5.8/setup.py` & `vector_quantize_pytorch-1.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.5.8',
+  version = '1.5.9',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
```

### Comparing `vector_quantize_pytorch-1.5.8/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.5.9/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.8/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.5.9/vector_quantize_pytorch/residual_vq.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.8/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.5.9/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from functools import partial
+
 import torch
 from torch import nn, einsum
 import torch.nn.functional as F
 import torch.distributed as distributed
 from torch.cuda.amp import autocast
 
 from einops import rearrange, repeat, pack, unpack
@@ -36,19 +38,49 @@
     nn.init.kaiming_uniform_(t)
     return t
 
 def gumbel_noise(t):
     noise = torch.zeros_like(t).uniform_(0, 1)
     return -log(-log(noise))
 
-def gumbel_sample(t, temperature = 1., dim = -1):
-    if temperature == 0:
-        return t.argmax(dim = dim)
+def gumbel_sample(
+    logits,
+    temperature = 1.,
+    stochastic = False,
+    straight_through = False,
+    reinmax = False,
+    dim = -1
+):
+    dtype, size = logits.dtype, logits.shape[dim]
+
+    if stochastic:
+        logits = logits + gumbel_noise(logits)
+
+    ind = logits.argmax(dim = dim)
+    one_hot = F.one_hot(ind, size).type(dtype)
 
-    return ((t / temperature) + gumbel_noise(t)).argmax(dim = dim)
+    assert not (reinmax and not straight_through), 'reinmax can only be turned on if using straight through gumbel softmax'
+
+    if not straight_through:
+        return ind, one_hot
+
+    # use reinmax for better second-order accuracy - https://arxiv.org/abs/2304.08612
+    # algorithm 2
+
+    if reinmax:
+        π0 = logits.softmax(dim = dim)
+        π1 = (one_hot + (logits / temperature).softmax(dim = dim)) / 2
+        π1 = ((π1.log() - logits).detach() + logits).softmax(dim = 1)
+        π2 = 2 * π1 - 0.5 * π0
+        one_hot = π2 - π2.detach() + one_hot
+    else:
+        π1 = (logits / temperature).softmax(dim = dim)
+        one_hot = one_hot + π1 - π1.detach()
+
+    return ind, one_hot
 
 def laplace_smoothing(x, n_categories, eps = 1e-5, dim = -1):
     denom = x.sum(dim = dim, keepdim = True)
     return (x + eps) / (denom + n_categories * eps)
 
 def sample_vectors(samples, num):
     num_samples, device = samples.shape[0], samples.device
@@ -196,15 +228,17 @@
         sync_kmeans = True,
         decay = 0.8,
         eps = 1e-5,
         threshold_ema_dead_code = 2,
         reset_cluster_size = None,
         use_ddp = False,
         learnable_codebook = False,
-        sample_codebook_temp = 0
+        sample_codebook_temp = 0,
+        straight_through = False,
+        gumbel_sample = gumbel_sample
     ):
         super().__init__()
         self.transform_input = identity
 
         self.decay = decay
         init_fn = uniform_init if not kmeans_init else torch.zeros
         embed = init_fn(num_codebooks, codebook_size, dim)
@@ -212,15 +246,17 @@
         self.codebook_size = codebook_size
         self.num_codebooks = num_codebooks
 
         self.kmeans_iters = kmeans_iters
         self.eps = eps
         self.threshold_ema_dead_code = threshold_ema_dead_code
         self.reset_cluster_size = default(reset_cluster_size, threshold_ema_dead_code)
-        self.sample_codebook_temp = sample_codebook_temp
+
+        assert callable(gumbel_sample)
+        self.gumbel_sample = gumbel_sample
 
         assert not (use_ddp and num_codebooks > 1 and kmeans_init), 'kmeans init is not compatible with multiple codebooks in distributed environment for now'
 
         self.sample_fn = sample_vectors_distributed if use_ddp and sync_kmeans else batched_sample_vectors
         self.kmeans_all_reduce_fn = distributed.all_reduce if use_ddp and sync_kmeans else noop
         self.all_reduce_fn = distributed.all_reduce if use_ddp else noop
 
@@ -291,16 +327,15 @@
 
         self.init_embed_(flatten)
 
         embed = self.embed if not self.learnable_codebook else self.embed.detach()
 
         dist = -torch.cdist(flatten, embed, p = 2)
 
-        embed_ind = gumbel_sample(dist, dim = -1, temperature = self.sample_codebook_temp)
-        embed_onehot = F.one_hot(embed_ind, self.codebook_size).type(dtype)
+        embed_ind, embed_onehot = self.gumbel_sample(dist, dim = -1)
         embed_ind = unpack_one(embed_ind, ps, 'h *')
 
         quantize = batched_embedding(embed_ind, self.embed)
 
         if self.training:
             cluster_size = embed_onehot.sum(dim = 1)
 
@@ -335,15 +370,15 @@
         sync_kmeans = True,
         decay = 0.8,
         eps = 1e-5,
         threshold_ema_dead_code = 2,
         reset_cluster_size = None,
         use_ddp = False,
         learnable_codebook = False,
-        sample_codebook_temp = 0.
+        gumbel_sample = gumbel_sample
     ):
         super().__init__()
         self.transform_input = l2norm
 
         self.decay = decay
 
         if not kmeans_init:
@@ -354,15 +389,17 @@
         self.codebook_size = codebook_size
         self.num_codebooks = num_codebooks
 
         self.kmeans_iters = kmeans_iters
         self.eps = eps
         self.threshold_ema_dead_code = threshold_ema_dead_code
         self.reset_cluster_size = default(reset_cluster_size, threshold_ema_dead_code)
-        self.sample_codebook_temp = sample_codebook_temp
+
+        assert callable(gumbel_sample)
+        self.gumbel_sample = gumbel_sample
 
         self.sample_fn = sample_vectors_distributed if use_ddp and sync_kmeans else batched_sample_vectors
         self.kmeans_all_reduce_fn = distributed.all_reduce if use_ddp and sync_kmeans else noop
         self.all_reduce_fn = distributed.all_reduce if use_ddp else noop
 
         self.register_buffer('initted', torch.Tensor([not kmeans_init]))
         self.register_buffer('cluster_size', torch.zeros(num_codebooks, codebook_size))
@@ -433,16 +470,15 @@
         flatten, ps = pack_one(x, 'h * d')
 
         self.init_embed_(flatten)
 
         embed = self.embed if not self.learnable_codebook else self.embed.detach()
 
         dist = einsum('h n d, h c d -> h n c', flatten, embed)
-        embed_ind = gumbel_sample(dist, dim = -1, temperature = self.sample_codebook_temp)
-        embed_onehot = F.one_hot(embed_ind, self.codebook_size).type(dtype)
+        embed_ind, embed_onehot = self.gumbel_sample(dist, dim = -1)
         embed_ind = unpack_one(embed_ind, ps, 'h *')
 
         quantize = batched_embedding(embed_ind, self.embed)
 
         if self.training:
             bins = embed_onehot.sum(dim = 1)
             self.all_reduce_fn(bins)
@@ -487,16 +523,19 @@
         channel_last = True,
         accept_image_fmap = False,
         commitment_weight = 1.,
         commitment_use_cross_entropy_loss = False,
         orthogonal_reg_weight = 0.,
         orthogonal_reg_active_codes_only = False,
         orthogonal_reg_max_codes = None,
+        stochastic_sample_codes = False,
         sample_codebook_temp = 0.,
-        sync_codebook = False
+        straight_through = False,
+        reinmax = False,  # using reinmax for improved straight-through, assuming straight through helps at all
+        sync_codebook = False,
     ):
         super().__init__()
         self.dim = dim
         self.heads = heads
         self.separate_codebook_per_head = separate_codebook_per_head
 
         codebook_dim = default(codebook_dim, dim)
@@ -513,27 +552,35 @@
         has_codebook_orthogonal_loss = orthogonal_reg_weight > 0
         self.orthogonal_reg_weight = orthogonal_reg_weight
         self.orthogonal_reg_active_codes_only = orthogonal_reg_active_codes_only
         self.orthogonal_reg_max_codes = orthogonal_reg_max_codes
 
         codebook_class = EuclideanCodebook if not use_cosine_sim else CosineSimCodebook
 
+        gumbel_sample_fn = partial(
+            gumbel_sample,
+            stochastic = stochastic_sample_codes,
+            temperature = sample_codebook_temp,
+            reinmax = reinmax,
+            straight_through = straight_through
+        )
+
         self._codebook = codebook_class(
             dim = codebook_dim,
             num_codebooks = heads if separate_codebook_per_head else 1,
             codebook_size = codebook_size,
             kmeans_init = kmeans_init,
             kmeans_iters = kmeans_iters,
             sync_kmeans = sync_kmeans,
             decay = decay,
             eps = eps,
             threshold_ema_dead_code = threshold_ema_dead_code,
             use_ddp = sync_codebook,
             learnable_codebook = has_codebook_orthogonal_loss,
-            sample_codebook_temp = sample_codebook_temp
+            gumbel_sample = gumbel_sample_fn
         )
 
         self.codebook_size = codebook_size
 
         self.accept_image_fmap = accept_image_fmap
         self.channel_last = channel_last
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vector_quantize_pytorch-1.5.8/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.5.9/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.5.8
+Version: 1.5.9
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

