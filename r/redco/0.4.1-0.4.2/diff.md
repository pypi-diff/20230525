# Comparing `tmp/redco-0.4.1.tar.gz` & `tmp/redco-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redco-0.4.1.tar", last modified: Sat May 13 23:54:41 2023, max compression
+gzip compressed data, was "redco-0.4.2.tar", last modified: Thu May 25 03:00:07 2023, max compression
```

## Comparing `redco-0.4.1.tar` & `redco-0.4.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-13 23:54:41.850000 redco-0.4.1/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)    11358 2023-04-19 06:11:18.000000 redco-0.4.1/LICENSE
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-05-13 23:54:41.850000 redco-0.4.1/PKG-INFO
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3375 2023-05-11 00:01:23.000000 redco-0.4.1/README.md
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-13 23:54:41.840000 redco-0.4.1/redco/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      693 2023-04-19 06:51:00.000000 redco-0.4.1/redco/__init__.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-13 23:54:41.840000 redco-0.4.1/redco/datasets/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      663 2023-04-19 06:51:00.000000 redco-0.4.1/redco/datasets/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      745 2023-04-19 06:51:00.000000 redco-0.4.1/redco/datasets/dataset.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1109 2023-04-19 06:51:00.000000 redco-0.4.1/redco/datasets/jsonl_dataset.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-13 23:54:41.840000 redco-0.4.1/redco/deployers/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      625 2023-04-19 06:51:00.000000 redco-0.4.1/redco/deployers/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2065 2023-04-19 06:51:00.000000 redco-0.4.1/redco/deployers/data_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     8044 2023-04-19 06:51:00.000000 redco-0.4.1/redco/deployers/deployer.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2656 2023-04-19 06:51:00.000000 redco-0.4.1/redco/deployers/log_utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-13 23:54:41.840000 redco-0.4.1/redco/deployers/model_parallel_utils/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      595 2023-04-19 06:51:00.000000 redco-0.4.1/redco/deployers/model_parallel_utils/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     5492 2023-05-11 00:14:31.000000 redco-0.4.1/redco/deployers/model_parallel_utils/mesh_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2468 2023-04-19 06:51:00.000000 redco-0.4.1/redco/deployers/model_parallel_utils/partition_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1835 2023-04-19 06:51:00.000000 redco-0.4.1/redco/deployers/opt_utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-13 23:54:41.840000 redco-0.4.1/redco/predictors/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      628 2023-04-19 06:51:00.000000 redco-0.4.1/redco/predictors/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4243 2023-04-19 06:51:00.000000 redco-0.4.1/redco/predictors/predictor.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1812 2023-04-19 06:51:00.000000 redco-0.4.1/redco/predictors/utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-13 23:54:41.840000 redco-0.4.1/redco/trainers/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      624 2023-04-19 06:51:00.000000 redco-0.4.1/redco/trainers/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)    12098 2023-04-19 06:51:00.000000 redco-0.4.1/redco/trainers/trainer.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2168 2023-04-19 06:51:00.000000 redco-0.4.1/redco/trainers/utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-13 23:54:41.840000 redco-0.4.1/redco.egg-info/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-05-13 23:54:41.000000 redco-0.4.1/redco.egg-info/PKG-INFO
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      735 2023-05-13 23:54:41.000000 redco-0.4.1/redco.egg-info/SOURCES.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)        1 2023-05-13 23:54:41.000000 redco-0.4.1/redco.egg-info/dependency_links.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)       21 2023-05-13 23:54:41.000000 redco-0.4.1/redco.egg-info/requires.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)        6 2023-05-13 23:54:41.000000 redco-0.4.1/redco.egg-info/top_level.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)       38 2023-05-13 23:54:41.850000 redco-0.4.1/setup.cfg
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1001 2023-05-13 23:52:43.000000 redco-0.4.1/setup.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-25 03:00:07.150000 redco-0.4.2/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)    11358 2023-04-19 06:11:18.000000 redco-0.4.2/LICENSE
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-05-25 03:00:07.150000 redco-0.4.2/PKG-INFO
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3375 2023-05-13 23:56:05.000000 redco-0.4.2/README.md
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-25 03:00:07.140000 redco-0.4.2/redco/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      693 2023-04-19 06:51:00.000000 redco-0.4.2/redco/__init__.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-25 03:00:07.150000 redco-0.4.2/redco/datasets/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      663 2023-04-19 06:51:00.000000 redco-0.4.2/redco/datasets/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      745 2023-04-19 06:51:00.000000 redco-0.4.2/redco/datasets/dataset.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1109 2023-04-19 06:51:00.000000 redco-0.4.2/redco/datasets/jsonl_dataset.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-25 03:00:07.150000 redco-0.4.2/redco/deployers/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      625 2023-04-19 06:51:00.000000 redco-0.4.2/redco/deployers/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2065 2023-04-19 06:51:00.000000 redco-0.4.2/redco/deployers/data_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     8051 2023-05-24 01:48:22.000000 redco-0.4.2/redco/deployers/deployer.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2656 2023-04-19 06:51:00.000000 redco-0.4.2/redco/deployers/log_utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-25 03:00:07.150000 redco-0.4.2/redco/deployers/model_parallel_utils/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      595 2023-04-19 06:51:00.000000 redco-0.4.2/redco/deployers/model_parallel_utils/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     5493 2023-05-24 01:48:22.000000 redco-0.4.2/redco/deployers/model_parallel_utils/mesh_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2468 2023-04-19 06:51:00.000000 redco-0.4.2/redco/deployers/model_parallel_utils/partition_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1835 2023-04-19 06:51:00.000000 redco-0.4.2/redco/deployers/opt_utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-25 03:00:07.150000 redco-0.4.2/redco/predictors/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      628 2023-04-19 06:51:00.000000 redco-0.4.2/redco/predictors/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4243 2023-04-19 06:51:00.000000 redco-0.4.2/redco/predictors/predictor.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1812 2023-04-19 06:51:00.000000 redco-0.4.2/redco/predictors/utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-25 03:00:07.150000 redco-0.4.2/redco/trainers/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      624 2023-04-19 06:51:00.000000 redco-0.4.2/redco/trainers/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)    12098 2023-04-19 06:51:00.000000 redco-0.4.2/redco/trainers/trainer.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2168 2023-04-19 06:51:00.000000 redco-0.4.2/redco/trainers/utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-25 03:00:07.140000 redco-0.4.2/redco.egg-info/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-05-25 03:00:05.000000 redco-0.4.2/redco.egg-info/PKG-INFO
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      735 2023-05-25 03:00:07.000000 redco-0.4.2/redco.egg-info/SOURCES.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)        1 2023-05-25 03:00:05.000000 redco-0.4.2/redco.egg-info/dependency_links.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)       21 2023-05-25 03:00:06.000000 redco-0.4.2/redco.egg-info/requires.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)        6 2023-05-25 03:00:06.000000 redco-0.4.2/redco.egg-info/top_level.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)       38 2023-05-25 03:00:07.150000 redco-0.4.2/setup.cfg
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1001 2023-05-25 02:59:09.000000 redco-0.4.2/setup.py
```

### Comparing `redco-0.4.1/LICENSE` & `redco-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redco-0.4.1/PKG-INFO` & `redco-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redco
-Version: 0.4.1
+Version: 0.4.2
 Summary: UNKNOWN
 Home-page: https://github.com/tanyuqian/redco
 Author: Bowen Tan
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -51,13 +51,13 @@
 
 ### Exemplar large model settings
 
 The table below shows runnable model LLM finetuning on different kinds of servers. Numbers inside the brackets are the maximum length in training. All the settings are with full precision (fp32) and Adam optimizer.
 
 | 2 $\times$ 1080Ti <br/>(2 $\times$ 10G) | 4 $\times$ A100 <br/>(4 $\times$ 40G) | 2 $\times$ TPU-v4 <br/>(2 hosts $\times$ 4 chips $\times$ 32G) | 16 $\times$ TPU-v4 <br/>(16 hosts $\times$ 4 chips $\times$ 32G) |
 |-----------------------------------------|---------------------------------------|----------------------------------------------------------------|------------------------------------------------------------------|
-| BART-Large (1024)                       | T5-XL-3B (1024)                       | T5-XL-11B (512)                                                | OPT-66B (512)                                                    |
+| BART-Large (1024)                       | LLaMA-7B (1024)                       | T5-XL-11B (512)                                                | OPT-66B (512)                                                    |
 | GPT2-Large (512)                        | GPT-J-6B (1024)                       | OPT-13B (1024)                                                 |                                                                  |
 
 Go to [example/language_modeling](examples%2Flanguage_modeling) and [examples/text_to_text](examples%2Ftext_to_text) to try them out!
```

### Comparing `redco-0.4.1/README.md` & `redco-0.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,11 +39,11 @@
 
 ### Exemplar large model settings
 
 The table below shows runnable model LLM finetuning on different kinds of servers. Numbers inside the brackets are the maximum length in training. All the settings are with full precision (fp32) and Adam optimizer.
 
 | 2 $\times$ 1080Ti <br/>(2 $\times$ 10G) | 4 $\times$ A100 <br/>(4 $\times$ 40G) | 2 $\times$ TPU-v4 <br/>(2 hosts $\times$ 4 chips $\times$ 32G) | 16 $\times$ TPU-v4 <br/>(16 hosts $\times$ 4 chips $\times$ 32G) |
 |-----------------------------------------|---------------------------------------|----------------------------------------------------------------|------------------------------------------------------------------|
-| BART-Large (1024)                       | T5-XL-3B (1024)                       | T5-XL-11B (512)                                                | OPT-66B (512)                                                    |
+| BART-Large (1024)                       | LLaMA-7B (1024)                       | T5-XL-11B (512)                                                | OPT-66B (512)                                                    |
 | GPT2-Large (512)                        | GPT-J-6B (1024)                       | OPT-13B (1024)                                                 |                                                                  |
 
 Go to [example/language_modeling](examples%2Flanguage_modeling) and [examples/text_to_text](examples%2Ftext_to_text) to try them out!
```

### Comparing `redco-0.4.1/redco/__init__.py` & `redco-0.4.2/redco/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.1/redco/datasets/__init__.py` & `redco-0.4.2/redco/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.1/redco/datasets/dataset.py` & `redco-0.4.2/redco/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.1/redco/datasets/jsonl_dataset.py` & `redco-0.4.2/redco/datasets/jsonl_dataset.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.1/redco/deployers/__init__.py` & `redco-0.4.2/redco/deployers/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.1/redco/deployers/data_utils.py` & `redco-0.4.2/redco/deployers/data_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.1/redco/deployers/deployer.py` & `redco-0.4.2/redco/deployers/deployer.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from .opt_utils import get_multistep_adamw_optimizer
 from .log_utils import get_logger, log_info, save_outputs
 from .model_parallel_utils.mesh_utils import (
     get_mesh,
     shard_params_and_opt_state,
     gather_params_to_cpu,
     get_param_spec,
-    guess_shard_rules)
+    get_sharding_rules)
 
 
 class Deployer:
     def __init__(self,
                  jax_seed,
                  n_model_shards=1,
                  verbose=True,
@@ -137,26 +137,26 @@
             global_batch_size=global_batch_size,
             n_epochs=n_epochs,
             learning_rate=learning_rate,
             accumulate_grad_batches=accumulate_grad_batches,
             warmup_rate=warmup_rate,
             weight_decay=weight_decay)
 
-    def guess_shard_rules(self, params):
+    def get_sharding_rules(self, params):
         if self._mesh is None:
             return None
         else:
-            shard_rules = guess_shard_rules(
+            sharding_rules = get_sharding_rules(
                 params=params, mesh_model_shards=self._mesh.shape['mp'])
 
             self.log_info(
-                info='\n'.join([f'{t}' for t in shard_rules]),
-                title='Guessed shard rules')
+                info='\n'.join([f'{t}' for t in sharding_rules]),
+                title='Sharding rules')
 
-            return shard_rules
+            return sharding_rules
 
     def get_params_spec(self, params, shard_rules):
         return get_param_spec(params=params, shard_rules=shard_rules)
 
     def shard_params_and_opt_state(self, params, params_spec, optimizer):
         return shard_params_and_opt_state(
             params=params,
```

### Comparing `redco-0.4.1/redco/deployers/log_utils.py` & `redco-0.4.2/redco/deployers/log_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.1/redco/deployers/model_parallel_utils/__init__.py` & `redco-0.4.2/redco/deployers/model_parallel_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.1/redco/deployers/model_parallel_utils/mesh_utils.py` & `redco-0.4.2/redco/deployers/model_parallel_utils/mesh_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         with jax.default_device(jax.devices('cpu')[0]):
             return jax.tree_util.tree_map(
                 lambda gather_fn, param: jax.device_get(gather_fn(param)),
                 gather_fns,
                 params)
 
 
-def guess_shard_rules(params, mesh_model_shards, investigate_depth=2):
+def get_sharding_rules(params, mesh_model_shards, investigate_depth=2):
     shard_rules = {
         ('(bias|scale)',): None,
         ('embedding',): P('mp', None),
     }
 
     last_dense_mp_dim = None
     flat_params = flatten_dict(params)
```

### Comparing `redco-0.4.1/redco/deployers/model_parallel_utils/partition_utils.py` & `redco-0.4.2/redco/deployers/model_parallel_utils/partition_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.1/redco/deployers/opt_utils.py` & `redco-0.4.2/redco/deployers/opt_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.1/redco/predictors/__init__.py` & `redco-0.4.2/redco/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.1/redco/predictors/predictor.py` & `redco-0.4.2/redco/predictors/predictor.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.1/redco/predictors/utils.py` & `redco-0.4.2/redco/predictors/utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.1/redco/trainers/__init__.py` & `redco-0.4.2/redco/trainers/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.1/redco/trainers/trainer.py` & `redco-0.4.2/redco/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.1/redco/trainers/utils.py` & `redco-0.4.2/redco/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.1/redco.egg-info/PKG-INFO` & `redco-0.4.2/redco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redco
-Version: 0.4.1
+Version: 0.4.2
 Summary: UNKNOWN
 Home-page: https://github.com/tanyuqian/redco
 Author: Bowen Tan
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -51,13 +51,13 @@
 
 ### Exemplar large model settings
 
 The table below shows runnable model LLM finetuning on different kinds of servers. Numbers inside the brackets are the maximum length in training. All the settings are with full precision (fp32) and Adam optimizer.
 
 | 2 $\times$ 1080Ti <br/>(2 $\times$ 10G) | 4 $\times$ A100 <br/>(4 $\times$ 40G) | 2 $\times$ TPU-v4 <br/>(2 hosts $\times$ 4 chips $\times$ 32G) | 16 $\times$ TPU-v4 <br/>(16 hosts $\times$ 4 chips $\times$ 32G) |
 |-----------------------------------------|---------------------------------------|----------------------------------------------------------------|------------------------------------------------------------------|
-| BART-Large (1024)                       | T5-XL-3B (1024)                       | T5-XL-11B (512)                                                | OPT-66B (512)                                                    |
+| BART-Large (1024)                       | LLaMA-7B (1024)                       | T5-XL-11B (512)                                                | OPT-66B (512)                                                    |
 | GPT2-Large (512)                        | GPT-J-6B (1024)                       | OPT-13B (1024)                                                 |                                                                  |
 
 Go to [example/language_modeling](examples%2Flanguage_modeling) and [examples/text_to_text](examples%2Ftext_to_text) to try them out!
```

### Comparing `redco-0.4.1/redco.egg-info/SOURCES.txt` & `redco-0.4.2/redco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redco-0.4.1/setup.py` & `redco-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  limitations under the License.
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="redco",
-    version="0.4.1",
+    version="0.4.2",
     author="Bowen Tan",
     packages=find_packages(),
     install_requires=['jax', 'flax', 'optax', 'numpy'],
     include_package_data=True,
     python_requires=">=3.8",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

