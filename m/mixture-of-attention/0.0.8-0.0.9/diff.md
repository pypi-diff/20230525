# Comparing `tmp/mixture-of-attention-0.0.8.tar.gz` & `tmp/mixture-of-attention-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixture-of-attention-0.0.8.tar", last modified: Tue May 16 18:44:51 2023, max compression
+gzip compressed data, was "mixture-of-attention-0.0.9.tar", last modified: Tue May 16 20:08:26 2023, max compression
```

## Comparing `mixture-of-attention-0.0.8.tar` & `mixture-of-attention-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:44:51.912309 mixture-of-attention-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 18:44:40.000000 mixture-of-attention-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 18:44:51.912309 mixture-of-attention-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-16 18:44:40.000000 mixture-of-attention-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:44:51.912309 mixture-of-attention-0.0.8/mixture_of_attention/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 18:44:40.000000 mixture-of-attention-0.0.8/mixture_of_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-16 18:44:40.000000 mixture-of-attention-0.0.8/mixture_of_attention/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-05-16 18:44:40.000000 mixture-of-attention-0.0.8/mixture_of_attention/mixture_of_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:44:51.912309 mixture-of-attention-0.0.8/mixture_of_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 18:44:51.000000 mixture-of-attention-0.0.8/mixture_of_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-16 18:44:51.000000 mixture-of-attention-0.0.8/mixture_of_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:44:51.000000 mixture-of-attention-0.0.8/mixture_of_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 18:44:51.000000 mixture-of-attention-0.0.8/mixture_of_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 18:44:51.000000 mixture-of-attention-0.0.8/mixture_of_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 18:44:51.912309 mixture-of-attention-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-16 18:44:40.000000 mixture-of-attention-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:08:26.092334 mixture-of-attention-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 20:08:07.000000 mixture-of-attention-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 20:08:26.092334 mixture-of-attention-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-16 20:08:07.000000 mixture-of-attention-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:08:26.092334 mixture-of-attention-0.0.9/mixture_of_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 20:08:07.000000 mixture-of-attention-0.0.9/mixture_of_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-16 20:08:07.000000 mixture-of-attention-0.0.9/mixture_of_attention/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-05-16 20:08:07.000000 mixture-of-attention-0.0.9/mixture_of_attention/mixture_of_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:08:26.092334 mixture-of-attention-0.0.9/mixture_of_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 20:08:26.000000 mixture-of-attention-0.0.9/mixture_of_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-16 20:08:26.000000 mixture-of-attention-0.0.9/mixture_of_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:08:26.000000 mixture-of-attention-0.0.9/mixture_of_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 20:08:26.000000 mixture-of-attention-0.0.9/mixture_of_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 20:08:26.000000 mixture-of-attention-0.0.9/mixture_of_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 20:08:26.092334 mixture-of-attention-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-16 20:08:07.000000 mixture-of-attention-0.0.9/setup.py
```

### Comparing `mixture-of-attention-0.0.8/LICENSE` & `mixture-of-attention-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mixture-of-attention-0.0.8/PKG-INFO` & `mixture-of-attention-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-attention
-Version: 0.0.8
+Version: 0.0.9
 Summary: Mixture of Attention
 Home-page: https://github.com/lucidrains/mixture-of-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,mixture-of-experts,routed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mixture-of-attention-0.0.8/README.md` & `mixture-of-attention-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,17 +39,18 @@
 context_mask = torch.ones((1, 512)).bool()
 
 mixture_of_attn(x, context = context, mask = mask) # (1, 1024, 512)
 ```
 
 ## Todo
 
+- [x] allow for local attention to be automatically included, either for grouped attention, or use `LocalMHA` from `local-attention` repository in parallel, weighted properly
+
 - [ ] try dynamic routing tokens, using projection of masked mean-pooled queries
 - [ ] make it work for autoregressive
-- [ ] allow for local attention to be automatically included, either for grouped attention, or use `LocalMHA` from `local-attention` repository in parallel, weighted properly
 
 ## Citations
 
 ```bibtex
 @inproceedings{Ainslie2023CoLT5FL,
     title   = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
     author  = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai},
```

#### html2text {}

```diff
@@ -13,23 +13,23 @@
 pip install mixture-of-attention ``` ## Usage ```python import torch from
 mixture_of_attention import MixtureOfAttention mixture_of_attn =
 MixtureOfAttention( dim = 512, dim_context = 256, num_routed_queries = 16,
 num_routed_key_values = 16, num_experts = 2, dim_head = 64, heads = 8 ) x =
 torch.randn(1, 1024, 512) mask = torch.ones((1, 1024)).bool() context =
 torch.randn(1, 512, 256) context_mask = torch.ones((1, 512)).bool()
 mixture_of_attn(x, context = context, mask = mask) # (1, 1024, 512) ``` ## Todo
-- [ ] try dynamic routing tokens, using projection of masked mean-pooled
-queries - [ ] make it work for autoregressive - [ ] allow for local attention
-to be automatically included, either for grouped attention, or use `LocalMHA`
-from `local-attention` repository in parallel, weighted properly ## Citations
-```bibtex @inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range
-Transformers with Conditional Computation}, author = {Joshua Ainslie and Tao
-Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury
-Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and
-Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ``` ```bibtex @inproceedings
-{dao2022flashattention, title = {Flash{A}ttention: Fast and Memory-Efficient
-Exact Attention with {IO}-Awareness}, author = {Dao, Tri and Fu, Daniel Y. and
-Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher}, booktitle = {Advances
-in Neural Information Processing Systems}, year = {2022} } ``` ```bibtex
-@article{Wright2015CoordinateDA, title = {Coordinate descent algorithms},
-author = {Stephen J. Wright}, journal = {Mathematical Programming}, year =
-{2015}, volume = {151}, pages = {3-34} } ```
+- [x] allow for local attention to be automatically included, either for
+grouped attention, or use `LocalMHA` from `local-attention` repository in
+parallel, weighted properly - [ ] try dynamic routing tokens, using projection
+of masked mean-pooled queries - [ ] make it work for autoregressive ##
+Citations ```bibtex @inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster
+Long-Range Transformers with Conditional Computation}, author = {Joshua Ainslie
+and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and
+Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay
+and Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ``` ```bibtex
+@inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast and
+Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri and
+Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
+booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
+} ``` ```bibtex @article{Wright2015CoordinateDA, title = {Coordinate descent
+algorithms}, author = {Stephen J. Wright}, journal = {Mathematical
+Programming}, year = {2015}, volume = {151}, pages = {3-34} } ```
```

### Comparing `mixture-of-attention-0.0.8/mixture_of_attention/attend.py` & `mixture-of-attention-0.0.9/mixture_of_attention/attend.py`

 * *Files identical despite different names*

### Comparing `mixture-of-attention-0.0.8/mixture_of_attention/mixture_of_attention.py` & `mixture-of-attention-0.0.9/mixture_of_attention/mixture_of_attention.py`

 * *Files 18% similar despite different names*

```diff
@@ -193,14 +193,16 @@
     def __init__(
         self,
         dim,
         *,
         num_routed_queries,
         num_routed_key_values,
         dim_context = None,
+        local_attn = False,
+        local_attn_window_size = None,
         num_experts = 2,
         dim_head = 64,
         heads = 8,
         dropout = 0.,
         use_triton = True,
         flash_attn = True,
         prenorm = True,
@@ -209,14 +211,26 @@
         super().__init__()
         dim_context = default(dim_context, dim)
         self.num_routed_queries = num_routed_queries
         self.num_routed_key_values = num_routed_key_values
 
         self.null_routed_token = nn.Parameter(torch.randn(1, 1, dim))
 
+        self.local_attn = None
+
+        if local_attn:
+            assert exists(local_attn_window_size)
+            self.local_attn = LocalMHA(
+                dim = dim,
+                dim_head = dim_head,
+                heads = heads,
+                prenorm = prenorm,
+                window_size = local_attn_window_size
+            )
+
         self.query_router = CoordinateDescentRouter(
             dim,
             num_routing_tokens = num_experts,
             use_triton = use_triton,
             **kwargs
         )
 
@@ -250,15 +264,19 @@
         context_mask = None,
         num_routed_queries = None,
         num_routed_key_values = None
     ):
         num_routed_queries = default(num_routed_queries, self.num_routed_queries)
         num_routed_key_values = default(num_routed_key_values, self.num_routed_key_values)
 
-        if not exists(context):
+        is_cross_attn = exists(context)
+
+        assert not (exists(self.local_attn) and is_cross_attn), 'cannot do cross attention with local attention (only for self attention)'
+
+        if not is_cross_attn:
             # self attention if context and context mask not passed in
             context = x
             context_mask = mask
 
         num_queries = x.shape[-2]
         num_key_values = context.shape[-2]
 
@@ -273,17 +291,27 @@
             context = key_values,
             mask = key_value_mask,
             values_scale = key_value_scores,
         )
 
         attn_out = attn_out * query_scores
 
+        local_out = None
+        if exists(self.local_attn):
+            local_out = self.local_attn(x, mask = mask)
+
         need_route_queries = exists(query_indices)
 
         if not need_route_queries:
+            out = attn_out
+
+            if exists(local_out):
+                local_out = rearrange(local_out, 'b n d -> b 1 n d')
+                out = torch.cat((local_out, out), dim = 1)
+
             out = reduce(attn_out, 'b e n d -> b n d', 'mean')
 
             if exists(mask):
                 out = out.masked_fill(~mask[..., None], 0.)
 
             return out
 
@@ -296,24 +324,31 @@
         expanded_query_indices = repeat(query_indices, 'b n -> b n d', d = x.shape[-1])
 
         attn_out_summed = out.scatter_add(1, expanded_query_indices, attn_out)
 
         counts = counts.scatter_add(1, query_indices, torch.ones(attn_out.shape[:-1], device = self.device))
         counts = rearrange(counts, '... -> ... 1')
 
-        not_routed_mask = counts == 0
+        has_unrouted = not exists(local_out)
 
-        attn_out_summed = attn_out_summed.masked_fill(not_routed_mask, 0.)
-        scatter_meaned = attn_out_summed / counts.clamp(min = 1e-5)
+        if not has_unrouted:
+            counts = counts + 1
+            attn_out_summed = attn_out_summed + local_out
+        else:
+            not_routed_mask = counts == 0
+            attn_out_summed = attn_out_summed.masked_fill(not_routed_mask, 0.)
+
+        out = attn_out_summed / counts.clamp(min = 1e-5)
 
         # for the positions that were not routed, use a learned routing token instead of just 0s
 
-        out = torch.where(
-            not_routed_mask,
-            self.null_routed_token,
-            scatter_meaned,
-        )
+        if has_unrouted:
+            out = torch.where(
+                not_routed_mask,
+                self.null_routed_token,
+                out,
+            )
 
         if exists(mask):
             out = out.masked_fill(~mask[..., None], 0.)
 
         return out
```

### Comparing `mixture-of-attention-0.0.8/mixture_of_attention.egg-info/PKG-INFO` & `mixture-of-attention-0.0.9/mixture_of_attention.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-attention
-Version: 0.0.8
+Version: 0.0.9
 Summary: Mixture of Attention
 Home-page: https://github.com/lucidrains/mixture-of-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,mixture-of-experts,routed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mixture-of-attention-0.0.8/setup.py` & `mixture-of-attention-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'mixture-of-attention',
   packages = find_packages(exclude=[]),
-  version = '0.0.8',
+  version = '0.0.9',
   license='MIT',
   description = 'Mixture of Attention',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/mixture-of-attention',
   keywords = [
```

