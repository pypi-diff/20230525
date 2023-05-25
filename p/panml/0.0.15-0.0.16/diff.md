# Comparing `tmp/panml-0.0.15.tar.gz` & `tmp/panml-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-0.0.15.tar", last modified: Sun May 21 12:16:10 2023, max compression
+gzip compressed data, was "panml-0.0.16.tar", last modified: Wed May 24 12:20:27 2023, max compression
```

## Comparing `panml-0.0.15.tar` & `panml-0.0.16.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-21 12:16:10.834049 panml-0.0.15/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-0.0.15/LICENSE
--rw-r--r--   0 williamzheng   (501) staff       (20)     1713 2023-05-21 12:16:10.834296 panml-0.0.15/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)     5031 2023-05-14 05:40:36.000000 panml-0.0.15/README.md
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-21 12:16:10.826260 panml-0.0.15/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-0.0.15/panml/__init__.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-21 12:16:10.829948 panml-0.0.15/panml/core/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.15/panml/core/__init__.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-21 12:16:10.830918 panml-0.0.15/panml/core/clustering/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.15/panml/core/clustering/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     8786 2023-05-21 05:11:31.000000 panml-0.0.15/panml/core/clustering/faiss.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-21 12:16:10.832395 panml-0.0.15/panml/core/llm/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.15/panml/core/llm/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    14264 2023-05-21 12:13:49.000000 panml-0.0.15/panml/core/llm/huggingface.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    11105 2023-05-21 05:11:31.000000 panml-0.0.15/panml/core/llm/openai.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     4728 2023-05-21 12:13:49.000000 panml-0.0.15/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     3307 2023-05-21 05:11:31.000000 panml-0.0.15/panml/search.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-21 12:16:10.829340 panml-0.0.15/panml.egg-info/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1713 2023-05-21 12:16:10.000000 panml-0.0.15/panml.egg-info/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)      449 2023-05-21 12:16:10.000000 panml-0.0.15/panml.egg-info/SOURCES.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-05-21 12:16:10.000000 panml-0.0.15/panml.egg-info/dependency_links.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)      215 2023-05-21 12:16:10.000000 panml-0.0.15/panml.egg-info/requires.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-05-21 12:16:10.000000 panml-0.0.15/panml.egg-info/top_level.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-05-21 12:16:10.835352 panml-0.0.15/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     2742 2023-05-21 12:14:56.000000 panml-0.0.15/setup.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-21 12:16:10.833439 panml-0.0.15/test/
--rw-r--r--   0 williamzheng   (501) staff       (20)     2765 2023-05-19 12:08:24.000000 panml-0.0.15/test/test_ModelPack.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    10200 2023-05-21 05:11:31.000000 panml-0.0.15/test/test_VectorEngine.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-24 12:20:27.166432 panml-0.0.16/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-0.0.16/LICENSE
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1713 2023-05-24 12:20:27.166595 panml-0.0.16/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)     5230 2023-05-21 13:17:47.000000 panml-0.0.16/README.md
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-24 12:20:27.160509 panml-0.0.16/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-0.0.16/panml/__init__.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-24 12:20:27.162967 panml-0.0.16/panml/core/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.16/panml/core/__init__.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-24 12:20:27.163736 panml-0.0.16/panml/core/clustering/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.16/panml/core/clustering/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-05-24 12:19:14.000000 panml-0.0.16/panml/core/clustering/faiss.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-24 12:20:27.165155 panml-0.0.16/panml/core/llm/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.16/panml/core/llm/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14599 2023-05-24 12:19:14.000000 panml-0.0.16/panml/core/llm/huggingface.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    11140 2023-05-24 12:19:14.000000 panml-0.0.16/panml/core/llm/openai.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)      537 2023-05-24 12:19:14.000000 panml-0.0.16/panml/core/llm/prompt_template.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     4764 2023-05-24 12:19:14.000000 panml-0.0.16/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     3343 2023-05-24 12:19:14.000000 panml-0.0.16/panml/search.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-24 12:20:27.162681 panml-0.0.16/panml.egg-info/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1713 2023-05-24 12:20:27.000000 panml-0.0.16/panml.egg-info/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)      483 2023-05-24 12:20:27.000000 panml-0.0.16/panml.egg-info/SOURCES.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-05-24 12:20:27.000000 panml-0.0.16/panml.egg-info/dependency_links.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)      215 2023-05-24 12:20:27.000000 panml-0.0.16/panml.egg-info/requires.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-05-24 12:20:27.000000 panml-0.0.16/panml.egg-info/top_level.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-05-24 12:20:27.167791 panml-0.0.16/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2742 2023-05-24 12:19:14.000000 panml-0.0.16/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-24 12:20:27.166150 panml-0.0.16/test/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2765 2023-05-19 12:08:24.000000 panml-0.0.16/test/test_ModelPack.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    10200 2023-05-21 05:11:31.000000 panml-0.0.16/test/test_VectorEngine.py
```

### Comparing `panml-0.0.15/LICENSE` & `panml-0.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `panml-0.0.15/PKG-INFO` & `panml-0.0.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 0.0.15
+Version: 0.0.16
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-0.0.15/README.md` & `panml-0.0.16/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-## PanML: A simple generative AI/ML development toolkit
+## PanML: A high level generative AI/ML development library
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
 [![](https://dcbadge.vercel.app/api/server/QpquRMDq?compact=true&style=flat)](https://discord.gg/QpquRMDq)
 
 ## Goal
 This package aims to make analysis and experimentation of generative AI/ML models more accessible, by providing a simple and consistent interface to foundation models for Data Scientists, Machine Learning Engineers and Software Developers. It's a work in progress, so very much open for collaboration and contribution. 
 <br><br>
 **Current supported generative AI/ML category** <br>
 *Language models (fine tuning, prompt engineering, prompt tuning, model evaluation)*
 <br><br>
 **Current supported foundation models** <br>
-*[HuggingFace Hub](https://huggingface.co) - open source collections of GPT-2, FLAN-T5, EleutherAI, Cerebras, StabilityAI, H2O, Salesforce language models* <br>
-*[OpenAI](https://openai.com) - text-davinci-002, text-davinci-003 (GPT3/3.5 base completions model) language models*
+*[HuggingFace Hub](https://huggingface.co) - open source LLMs from Google, EleutherAI, Cerebras, StabilityAI, H2O, Salesforce, and others, see [supported models](https://github.com/Pan-ML/panml/wiki/8.-Supported-models)* <br>
+*[OpenAI](https://openai.com) - text-davinci-002/003, GPT3/3.5, see [supported models](https://github.com/Pan-ML/panml/wiki/8.-Supported-models) *
 <br><br>
 **Current supported evals** <br>
 *Coming later...*
 <br>
 
 ## Installation
 ```bash
 git clone https://github.com/Pan-ML/panml.git
 ```
 
 ## Usage
-Check out the [Quick start guide](https://github.com/Pan-ML/panml/wiki/1.-Quick-start-guide) or other examples in [Wiki](https://github.com/Pan-ML/panml/wiki)
+See [quick start guide](https://github.com/Pan-ML/panml/wiki/1.-Quick-start-guide) or other examples in [Wiki](https://github.com/Pan-ML/panml/wiki).
 
 ### Importing the module
 ```python
 # Import panml
 from panml.models import ModelPack
 
 # Import other modules/packages as required
@@ -45,14 +45,15 @@
 ```
 ```
 # Output
 'hello world is a place where people can live and work together, and where people can live and work together, and where people can live and work together'
 ```
 
 ### Fine tune custom LLM
+For more examples, see [fine tuning your LLM](https://github.com/Pan-ML/panml/wiki/3.-Fine-tuning-your-LLM).
 ```python
 # Specify train args
 train_args = {
     'title': 'my_tuned_gpt2',
     'num_train_epochs' : 5,
     'mlm': False,
     'optimizer': 'adamw_torch',
@@ -71,15 +72,15 @@
 y = x
 
 # Train model
 lm.fit(x, y, train_args, instruct=False)
 ```
 
 ### Prompt chain engineering
-Create model pack from OpenAI model description and API key
+Create model pack from OpenAI model description and API key.
 ```python
 lm = ModelPack(model='text-davinci-002', source='openai', api_key=<your_openai_key>)
 
 prompts = [
     {'prepend': 'you are a sports coach'},
     {'prepend': 'produce a daily exercise plan for one week'},
     {'prepend': 'summarise to the original question'},
```

### Comparing `panml-0.0.15/panml/core/clustering/faiss.py` & `panml-0.0.16/panml/core/clustering/faiss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 # Dependencies for data processing and general machine learning implementations
 import numpy as np
 import pandas as pd
 from typing import Union
 
 # Dependencies for vector search
 import faiss
@@ -163,15 +165,21 @@
 
         Returns: 
         list of the top k documents
         '''
         # Catch input exceptions
         if not isinstance(query, str):
             raise TypeError('Input query needs to be of type: string')
+        else:
+            if len(query) < 1:
+                raise ValueError('Input query cannot be empty')
         if not isinstance(k, int):
             raise TypeError('Input number of returned documents needs to be of type int')
+        else:
+            if k < 1:
+                raise ValueError('Input k cannot be less than 1')
             
         if k > len(self.corpus):
             k = len(self.corpus) # cap the max k to the maximum number of documents in the corpus store
         query_vector = self._get_embedding([query], self.model_emb_source) # embed input vector
         D, I = self.vectors.search(query_vector, k) # perform vector search
         return list(np.array(self.corpus)[I][0])
```

### Comparing `panml-0.0.15/panml/core/llm/huggingface.py` & `panml-0.0.16/panml/core/llm/huggingface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import pandas as pd
 import torch
 from typing import Union
 from transformers import AutoModelForCausalLM, AutoModelForSeq2SeqLM, AutoModelForMaskedLM, AutoTokenizer
 from transformers import TrainingArguments, Trainer, Seq2SeqTrainer, DataCollatorForLanguageModeling, DataCollatorForSeq2Seq
 from datasets import Dataset
 
@@ -12,19 +13,19 @@
     '''
     # Initialize class variables
     def __init__(self, model: str, input_block_size: int, padding_length: int, tokenizer_batch: bool, source: str, model_args: dict) -> None:
         self.model_name = model
         self.padding_length = padding_length
         self.input_block_size = input_block_size
         self.tokenizer_batch = tokenizer_batch
+        self.device = 'cpu'
         self.train_default_args = ['title', 'num_train_epochs', 'optimizer', 'mlm', 
                                    'per_device_train_batch_size', 'per_device_eval_batch_size',
                                    'warmup_steps', 'weight_decay', 'logging_steps', 
                                    'output_dir', 'logging_dir', 'save_model']
-        
         if source == 'huggingface':
             if 'flan' in self.model_name:
                 self.model_hf = AutoModelForSeq2SeqLM.from_pretrained(self.model_name, **model_args)
             elif 'bert' in self.model_name:
                 self.model_hf = AutoModelForMaskedLM.from_pretrained(self.model_name, **model_args)
             else:
                 self.model_hf = AutoModelForCausalLM.from_pretrained(self.model_name, **model_args)
@@ -35,30 +36,35 @@
                 self.model_hf = AutoModelForMaskedLM.from_pretrained(self.model_name, **model_args, local_files_only=True)
             else:
                 self.model_hf = AutoModelForCausalLM.from_pretrained(self.model_name, **model_args, local_files_only=True)
         if self.model_hf.config.tokenizer_class:
             self.tokenizer = AutoTokenizer.from_pretrained(self.model_hf.config.tokenizer_class.lower().replace('tokenizer', ''), mirror='https://huggingface.co')
         else:
             self.tokenizer = AutoTokenizer.from_pretrained(self.model_name, mirror='https://huggingface.co')
-        
-        if self.tokenizer.pad_token is None:
-            self.tokenizer.pad_token = self.model_hf.config.eos_token_id
-    
+
+        # Set model on GPU if available and specified
+        if 'gpu' in model_args:
+            self.device = 'cuda' if torch.cuda.is_available() and model_args['gpu'] else 'cpu'
+            print('Model processing is set on GPU')
+        else:
+            print('Model processing is set on CPU')
+        self.model_hf.to(torch.device(self.device))
+
     # Embed text
     def embedding(self, text: str) -> torch.Tensor:
         '''
         Gets the embedding of the text using open source collections of models from HuggingFace Hub
 
         Args:
         text: text of the input
 
         Returns:
         torch tensor containing the embedding array
         '''
-        token_ids = self.tokenizer.encode(text, return_tensors='pt')
+        token_ids = self.tokenizer.encode(text, return_tensors='pt').to(torch.device(self.device))
         
         # # Get embeddings
         # if 'flan' in self.model_hf.name_or_path: 
         #     emb = self.model_hf.shared.weight[token_ids[0]] # embeddings for FLAN
         # else: 
         #     emb = self.model_hf.transformer.wte.weight[token_ids[0]] # embeddings for GPT2
             
@@ -102,15 +108,15 @@
             
         output_context = {
             'text': None,
             'probability': None,
             'perplexity': None,
         }
         
-        input_ids = self.tokenizer.encode(text, return_tensors='pt')
+        input_ids = self.tokenizer.encode(text, return_tensors='pt').to(torch.device(self.device))
         output = self.model_hf.generate(input_ids, 
                                         max_length=max_length,
                                         pad_token_id=self.model_hf.config.eos_token_id,
                                         num_return_sequences=num_return_sequences, 
                                         temperature=temperature,
                                         top_p=top_p,
                                         top_k=top_k,
```

### Comparing `panml-0.0.15/panml/core/llm/openai.py` & `panml-0.0.16/panml/core/llm/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import pandas as pd
 import torch
 from typing import Union
 import openai
 
 # OpenAI model class
 class OpenAIModelPack:
```

### Comparing `panml-0.0.15/panml/models.py` & `panml-0.0.16/panml/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 # Dependencies for data processing and general machine learning implementations
 import torch
 from typing import Union
 
 # Dependencies for specialised language model implementations
 from transformers import AutoTokenizer
 from panml.core.llm.huggingface import HuggingFaceModelPack
```

### Comparing `panml-0.0.15/panml/search.py` & `panml-0.0.16/panml/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 # Dependencies for data processing and general machine learning implementations
 import torch
 import torch.nn.functional as F
 from typing import Union
 
 # Dependencies for vector search
 from panml.core.clustering.faiss import FAISSVectorEngine
```

### Comparing `panml-0.0.15/panml.egg-info/PKG-INFO` & `panml-0.0.16/panml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 0.0.15
+Version: 0.0.16
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-0.0.15/setup.py` & `panml-0.0.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 setup(
   name = 'panml', # package name     
   packages = find_packages(exclude=['test']), # package name
-  version = '0.0.15', # version
+  version = '0.0.16', # version
   license = 'MIT', # license
   description = 'PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.', # short description about the package
   long_description = 'PanML aims to make analysis and experimentation of generative AI/ML models more accessible, by providing a simple and consistent interface to foundation models for Data Scientists, Machine Learning Engineers and Software Developers. \
                       The package provides various assistive tools to work with generative language models, such as prompt engineering, fine tuning and others. \
                       \n\nQuick start guide: https://github.com/Pan-ML/panml/wiki/1.-Quick-start-guide \
                       \n\nDocumentation/Wiki: https://github.com/Pan-ML/panml/wiki', # long description
   author = 'PanML team', # team name
```

### Comparing `panml-0.0.15/test/test_ModelPack.py` & `panml-0.0.16/test/test_ModelPack.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.15/test/test_VectorEngine.py` & `panml-0.0.16/test/test_VectorEngine.py`

 * *Files identical despite different names*

