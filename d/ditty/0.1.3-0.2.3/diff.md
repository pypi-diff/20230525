# Comparing `tmp/ditty-0.1.3.tar.gz` & `tmp/ditty-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ditty-0.1.3.tar", last modified: Tue May 23 04:18:44 2023, max compression
+gzip compressed data, was "ditty-0.2.3.tar", last modified: Thu May 25 03:32:43 2023, max compression
```

## Comparing `ditty-0.1.3.tar` & `ditty-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-23 04:18:44.773838 ditty-0.1.3/
--rw-rw-r--   0 crow      (1000) crow      (1000)    11357 2023-05-20 22:13:26.000000 ditty-0.1.3/LICENSE
--rw-rw-r--   0 crow      (1000) crow      (1000)     3170 2023-05-23 04:18:44.773838 ditty-0.1.3/PKG-INFO
--rw-rw-r--   0 crow      (1000) crow      (1000)     2872 2023-05-23 04:03:46.000000 ditty-0.1.3/README.md
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-23 04:18:44.773838 ditty-0.1.3/lib/
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-23 04:18:44.773838 ditty-0.1.3/lib/ditty/
--rw-rw-r--   0 crow      (1000) crow      (1000)        0 2023-05-21 15:10:10.000000 ditty-0.1.3/lib/ditty/__init__.py
--rw-rw-r--   0 crow      (1000) crow      (1000)     4966 2023-05-23 04:18:09.000000 ditty-0.1.3/lib/ditty/data.py
--rw-rw-r--   0 crow      (1000) crow      (1000)     5428 2023-05-23 04:17:38.000000 ditty-0.1.3/lib/ditty/pipeline.py
--rw-rw-r--   0 crow      (1000) crow      (1000)     4775 2023-05-23 04:17:21.000000 ditty-0.1.3/lib/ditty/trainer.py
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-23 04:18:44.773838 ditty-0.1.3/lib/ditty.egg-info/
--rw-rw-r--   0 crow      (1000) crow      (1000)     3170 2023-05-23 04:18:44.000000 ditty-0.1.3/lib/ditty.egg-info/PKG-INFO
--rw-rw-r--   0 crow      (1000) crow      (1000)      283 2023-05-23 04:18:44.000000 ditty-0.1.3/lib/ditty.egg-info/SOURCES.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)        1 2023-05-23 04:18:44.000000 ditty-0.1.3/lib/ditty.egg-info/dependency_links.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)       56 2023-05-23 04:18:44.000000 ditty-0.1.3/lib/ditty.egg-info/requires.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)        6 2023-05-23 04:18:44.000000 ditty-0.1.3/lib/ditty.egg-info/top_level.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)      103 2023-05-23 04:18:44.773838 ditty-0.1.3/setup.cfg
--rw-rw-r--   0 crow      (1000) crow      (1000)      639 2023-05-23 04:18:17.000000 ditty-0.1.3/setup.py
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-25 03:32:43.948102 ditty-0.2.3/
+-rw-rw-r--   0 crow      (1000) crow      (1000)    11357 2023-05-20 22:13:26.000000 ditty-0.2.3/LICENSE
+-rw-rw-r--   0 crow      (1000) crow      (1000)     3170 2023-05-25 03:32:43.948102 ditty-0.2.3/PKG-INFO
+-rw-rw-r--   0 crow      (1000) crow      (1000)     2872 2023-05-23 04:03:46.000000 ditty-0.2.3/README.md
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-25 03:32:43.948102 ditty-0.2.3/lib/
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-25 03:32:43.948102 ditty-0.2.3/lib/ditty/
+-rw-rw-r--   0 crow      (1000) crow      (1000)        0 2023-05-21 15:10:10.000000 ditty-0.2.3/lib/ditty/__init__.py
+-rw-rw-r--   0 crow      (1000) crow      (1000)     5164 2023-05-23 17:35:55.000000 ditty-0.2.3/lib/ditty/data.py
+-rw-rw-r--   0 crow      (1000) crow      (1000)     5670 2023-05-25 02:45:06.000000 ditty-0.2.3/lib/ditty/pipeline.py
+-rw-rw-r--   0 crow      (1000) crow      (1000)     6168 2023-05-25 00:24:18.000000 ditty-0.2.3/lib/ditty/trainer.py
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-25 03:32:43.948102 ditty-0.2.3/lib/ditty.egg-info/
+-rw-rw-r--   0 crow      (1000) crow      (1000)     3170 2023-05-25 03:32:43.000000 ditty-0.2.3/lib/ditty.egg-info/PKG-INFO
+-rw-rw-r--   0 crow      (1000) crow      (1000)      283 2023-05-25 03:32:43.000000 ditty-0.2.3/lib/ditty.egg-info/SOURCES.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)        1 2023-05-25 03:32:43.000000 ditty-0.2.3/lib/ditty.egg-info/dependency_links.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)       56 2023-05-25 03:32:43.000000 ditty-0.2.3/lib/ditty.egg-info/requires.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)        6 2023-05-25 03:32:43.000000 ditty-0.2.3/lib/ditty.egg-info/top_level.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)      103 2023-05-25 03:32:43.948102 ditty-0.2.3/setup.cfg
+-rw-rw-r--   0 crow      (1000) crow      (1000)      639 2023-05-25 03:32:10.000000 ditty-0.2.3/setup.py
```

### Comparing `ditty-0.1.3/LICENSE` & `ditty-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ditty-0.1.3/PKG-INFO` & `ditty-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ditty
-Version: 0.1.3
+Version: 0.2.3
 Home-page: https://github.com/iantbutler01/ditty
 Author: Ian T Butler (KinglyCrow)
 Author-email: iantbutler01@gmail.com
 License: Apache V2
 Keywords: finetuning,llm,nlp,machine learning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ditty-0.1.3/README.md` & `ditty-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ditty-0.1.3/lib/ditty/data.py` & `ditty-0.2.3/lib/ditty/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import torch
 from torch.utils.data import DataLoader, RandomSampler
 import datasets
 from transformers.trainer_pt_utils import (
     LabelSmoother,
     LengthGroupedSampler,
 )
-from transformers.trainer_utils import seed_worker, RemoveColumnsCollator
+from transformers.trainer_utils import RemoveColumnsCollator, set_seed
 from transformers.data.data_collator import DataCollator, DataCollatorWithPadding, DataCollatorForLanguageModeling, default_data_collator
 from transformers import PreTrainedTokenizerBase
 from typing import Callable
 
 from logging import getLogger
 
 logger = getLogger()
@@ -99,14 +99,22 @@
 
         for op_name, func, kwargs in pipeline:
             op = getattr(self.dataset, op_name)
             self.dataset = op(func, **kwargs)
 
         return self._get_dataloader()        
 
+    def _seed_worker(self):
+        if not self.seed:
+            worker_seed = torch.initial_seed() % 2**32
+        else:
+            worker_seed = self.seed
+
+        set_seed(worker_seed)
+    
     def _get_dataloader(self) -> DataLoader:
         """
         Returns a [`~torch.utils.data.DataLoader`].
 
         Will use no sampler if `dataset` does not implement `__len__`, a random sampler (adapted to distributed
         training if necessary) otherwise.
 
@@ -133,9 +141,9 @@
             dataset,
             batch_size=self.batch_size,
             sampler=sampler,
             collate_fn=data_collator,
             drop_last=self.dataloader_drop_last,
             num_workers=self.dataloader_num_workers,
             pin_memory=self.dataloader_pin_memory,
-            worker_init_fn=seed_worker,
+            worker_init_fn=self._seed_worker,
         )
```

### Comparing `ditty-0.1.3/lib/ditty/pipeline.py` & `ditty-0.2.3/lib/ditty/pipeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,41 +23,43 @@
         self,
         output_dir="./output",
         dataset_name="code_search_net",
         dataset_language="python",
         model_name_or_path="theblackcat102/pythia-3b-deduped-sft-r1",
         hf_hub_token=None,
         hf_hub_model_id=None,
-        accelerated=True,
         fp16=True,
         l8bit=True,
         seed=None,
         batch_size=4,
         grad_accum=4,
         push_to_hub=True,
-        fp32_cpu_offload=True,
+        fp32_cpu_offload=False,
+        load_checkpoint=True,
+        checkpoint_every=1000,
     ):
         self.output_dir = output_dir
         self.dataset_name = dataset_name
         self.dataset_language = dataset_language
         self.model_name_or_path = model_name_or_path
         self.hf_hub_token = hf_hub_token
         self.hf_hub_model_id = hf_hub_model_id
-        self.accelerated = accelerated
         self.fp16 = fp16
         self.seed = seed
         self.epochs = 1
         self.max_steps = None
         self.l8bit = l8bit
         self.push_to_hub = push_to_hub
         self.batch_size = batch_size
         self.grad_accum = grad_accum
         self.block_size = 2048
         self.fp32_cpu_offload = fp32_cpu_offload
         self.bb_conf = BitsAndBytesConfig(load_in_8bit=l8bit, llm_int8_enable_fp32_cpu_offload=fp32_cpu_offload)
+        self.checkpoint_every = checkpoint_every
+        self.load_checkpoint = load_checkpoint
 
     def dataset(self) -> DataLoader:
         '''
         Subclass Pipeline and customize for your own dataset.
         '''
 
         data = Data(
@@ -87,31 +89,33 @@
             [
                 ("filter", filter_longer, {}),
                 (
                     "map",
                     lambda sample: self.tokenizer(
                         sample["whole_func_string"], padding="max_length", max_length=self.block_size
                     ),
-                    dict(batched=True, remove_columns=columns),
+                    dict(batched=True, remove_columns=columns, num_proc=8),
                 ),
-                ("map", truncate, {}),
+                ("map", truncate, dict(num_proc=8)),
             ]
         )
         return dataloader
 
     def run(self):
         self.tokenizer = AutoTokenizer.from_pretrained(self.model_name_or_path)
         if self.tokenizer.pad_token_id is None:
             self.tokenizer.pad_token_id = self.tokenizer.eos_token_id
 
+        data = self.dataset()
+
         self.model = AutoModelForCausalLM.from_pretrained(
             self.model_name_or_path,
             device_map="auto",
             load_in_8bit=self.l8bit,
-        ).cuda()
+        )
 
         target_modules = None
         if "gpt-neox" in self.model_name_or_path:
             target_modules = ["query_key_value", "xxx"]
 
         peft_config = LoraConfig(
             task_type=TaskType.CAUSAL_LM,
@@ -140,15 +144,14 @@
 
             setattr(self.model, "embed_out", CastOutputToFloat(output_embedding_layer))
 
         self.model = get_peft_model(self.model, peft_config)
 
         ### Training
 
-        data = self.dataset()
 
         self.model.gradient_checkpointing_enable()
         self.model.config.use_cache = False  # silence the warnings. Please re-enable for inference!
 
         adam_beta1 = 0.9
         adam_beta2 = 0.999
         adam_epsilon = 1e-08
@@ -159,17 +162,20 @@
         optimizer = torch.optim.AdamW(self.model.parameters(), lr=0.97e-5, **adam_kwargs)
 
         trainer = Trainer(
             model=self.model,
             optimizer=optimizer,
             dataset=data,
             device="cuda",
-            accelerate=self.accelerated,
             grad_accum=self.grad_accum,
             fp16=self.fp16,
+            output_dir=self.output_dir,
+            checkpoint_every=self.checkpoint_every,
+            load_checkpoint=self.load_checkpoint,
+            seed=self.seed,
         )
 
         trainer.train(epochs=self.epochs, max_steps=self.max_steps if self.max_steps else None)
 
         # ## Share adapters on the 🤗 Hub
         if self.push_to_hub:
             self.model.push_to_hub(self.output_dir, use_auth_token=True)
```

### Comparing `ditty-0.1.3/lib/ditty.egg-info/PKG-INFO` & `ditty-0.2.3/lib/ditty.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ditty
-Version: 0.1.3
+Version: 0.2.3
 Home-page: https://github.com/iantbutler01/ditty
 Author: Ian T Butler (KinglyCrow)
 Author-email: iantbutler01@gmail.com
 License: Apache V2
 Keywords: finetuning,llm,nlp,machine learning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ditty-0.1.3/setup.py` & `ditty-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='ditty',
-    version='0.1.3',
+    version='0.2.3',
     license='Apache V2',
     author="Ian T Butler (KinglyCrow)",
     author_email='iantbutler01@gmail.com',
     packages=find_packages('lib'),
     package_dir={'': 'lib'},
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

