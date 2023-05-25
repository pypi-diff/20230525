# Comparing `tmp/panml-0.0.16.tar.gz` & `tmp/panml-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-0.0.16.tar", last modified: Wed May 24 12:20:27 2023, max compression
+gzip compressed data, was "panml-0.0.17.tar", last modified: Thu May 25 02:47:34 2023, max compression
```

## Comparing `panml-0.0.16.tar` & `panml-0.0.17.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-24 12:20:27.166432 panml-0.0.16/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-0.0.16/LICENSE
--rw-r--r--   0 williamzheng   (501) staff       (20)     1713 2023-05-24 12:20:27.166595 panml-0.0.16/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)     5230 2023-05-21 13:17:47.000000 panml-0.0.16/README.md
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-24 12:20:27.160509 panml-0.0.16/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-0.0.16/panml/__init__.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-24 12:20:27.162967 panml-0.0.16/panml/core/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.16/panml/core/__init__.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-24 12:20:27.163736 panml-0.0.16/panml/core/clustering/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.16/panml/core/clustering/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-05-24 12:19:14.000000 panml-0.0.16/panml/core/clustering/faiss.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-24 12:20:27.165155 panml-0.0.16/panml/core/llm/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.16/panml/core/llm/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    14599 2023-05-24 12:19:14.000000 panml-0.0.16/panml/core/llm/huggingface.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    11140 2023-05-24 12:19:14.000000 panml-0.0.16/panml/core/llm/openai.py
--rw-r--r--   0 williamzheng   (501) staff       (20)      537 2023-05-24 12:19:14.000000 panml-0.0.16/panml/core/llm/prompt_template.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     4764 2023-05-24 12:19:14.000000 panml-0.0.16/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     3343 2023-05-24 12:19:14.000000 panml-0.0.16/panml/search.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-24 12:20:27.162681 panml-0.0.16/panml.egg-info/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1713 2023-05-24 12:20:27.000000 panml-0.0.16/panml.egg-info/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)      483 2023-05-24 12:20:27.000000 panml-0.0.16/panml.egg-info/SOURCES.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-05-24 12:20:27.000000 panml-0.0.16/panml.egg-info/dependency_links.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)      215 2023-05-24 12:20:27.000000 panml-0.0.16/panml.egg-info/requires.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-05-24 12:20:27.000000 panml-0.0.16/panml.egg-info/top_level.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-05-24 12:20:27.167791 panml-0.0.16/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     2742 2023-05-24 12:19:14.000000 panml-0.0.16/setup.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-24 12:20:27.166150 panml-0.0.16/test/
--rw-r--r--   0 williamzheng   (501) staff       (20)     2765 2023-05-19 12:08:24.000000 panml-0.0.16/test/test_ModelPack.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    10200 2023-05-21 05:11:31.000000 panml-0.0.16/test/test_VectorEngine.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-25 02:47:34.037246 panml-0.0.17/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-0.0.17/LICENSE
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1713 2023-05-25 02:47:34.037485 panml-0.0.17/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)     5230 2023-05-21 13:17:47.000000 panml-0.0.17/README.md
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-25 02:47:34.027633 panml-0.0.17/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-0.0.17/panml/__init__.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-25 02:47:34.031698 panml-0.0.17/panml/core/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.17/panml/core/__init__.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-25 02:47:34.032768 panml-0.0.17/panml/core/clustering/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.17/panml/core/clustering/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-05-24 12:19:14.000000 panml-0.0.17/panml/core/clustering/faiss.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-25 02:47:34.035241 panml-0.0.17/panml/core/llm/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.17/panml/core/llm/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14848 2023-05-25 02:26:09.000000 panml-0.0.17/panml/core/llm/huggingface.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    11140 2023-05-25 02:25:41.000000 panml-0.0.17/panml/core/llm/openai.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)      537 2023-05-24 12:19:14.000000 panml-0.0.17/panml/core/llm/prompt_template.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     4764 2023-05-24 12:19:14.000000 panml-0.0.17/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     3343 2023-05-24 12:19:14.000000 panml-0.0.17/panml/search.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-25 02:47:34.030930 panml-0.0.17/panml.egg-info/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1713 2023-05-25 02:47:33.000000 panml-0.0.17/panml.egg-info/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)      483 2023-05-25 02:47:33.000000 panml-0.0.17/panml.egg-info/SOURCES.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-05-25 02:47:33.000000 panml-0.0.17/panml.egg-info/dependency_links.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)      215 2023-05-25 02:47:33.000000 panml-0.0.17/panml.egg-info/requires.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-05-25 02:47:33.000000 panml-0.0.17/panml.egg-info/top_level.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-05-25 02:47:34.038557 panml-0.0.17/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2742 2023-05-25 02:26:09.000000 panml-0.0.17/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-25 02:47:34.036688 panml-0.0.17/test/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     3414 2023-05-25 02:26:09.000000 panml-0.0.17/test/test_ModelPack.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-0.0.17/test/test_VectorEngine.py
```

### Comparing `panml-0.0.16/LICENSE` & `panml-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `panml-0.0.16/PKG-INFO` & `panml-0.0.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 0.0.16
+Version: 0.0.17
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-0.0.16/README.md` & `panml-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `panml-0.0.16/panml/core/clustering/faiss.py` & `panml-0.0.17/panml/core/clustering/faiss.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.16/panml/core/llm/huggingface.py` & `panml-0.0.17/panml/core/llm/huggingface.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,28 @@
     # Initialize class variables
     def __init__(self, model: str, input_block_size: int, padding_length: int, tokenizer_batch: bool, source: str, model_args: dict) -> None:
         self.model_name = model
         self.padding_length = padding_length
         self.input_block_size = input_block_size
         self.tokenizer_batch = tokenizer_batch
         self.device = 'cpu'
+        if 'gpu' in model_args: # set model processing on GPU else defaults on CPU
+            if not isinstance(model_args['gpu'], bool):
+                raise TypeError('Input model args, gpu needs to be of type: boolean')
+            set_gpu = model_args.pop('gpu')
+            if torch.cuda.is_available() and set_gpu: 
+                self.device = 'cuda'
+            else:
+                print('CUDA is not available')
+        print(f'Model processing is set on {self.device.upper()}')
         self.train_default_args = ['title', 'num_train_epochs', 'optimizer', 'mlm', 
                                    'per_device_train_batch_size', 'per_device_eval_batch_size',
                                    'warmup_steps', 'weight_decay', 'logging_steps', 
                                    'output_dir', 'logging_dir', 'save_model']
+
         if source == 'huggingface':
             if 'flan' in self.model_name:
                 self.model_hf = AutoModelForSeq2SeqLM.from_pretrained(self.model_name, **model_args)
             elif 'bert' in self.model_name:
                 self.model_hf = AutoModelForMaskedLM.from_pretrained(self.model_name, **model_args)
             else:
                 self.model_hf = AutoModelForCausalLM.from_pretrained(self.model_name, **model_args)
@@ -38,19 +48,14 @@
                 self.model_hf = AutoModelForCausalLM.from_pretrained(self.model_name, **model_args, local_files_only=True)
         if self.model_hf.config.tokenizer_class:
             self.tokenizer = AutoTokenizer.from_pretrained(self.model_hf.config.tokenizer_class.lower().replace('tokenizer', ''), mirror='https://huggingface.co')
         else:
             self.tokenizer = AutoTokenizer.from_pretrained(self.model_name, mirror='https://huggingface.co')
 
         # Set model on GPU if available and specified
-        if 'gpu' in model_args:
-            self.device = 'cuda' if torch.cuda.is_available() and model_args['gpu'] else 'cpu'
-            print('Model processing is set on GPU')
-        else:
-            print('Model processing is set on CPU')
         self.model_hf.to(torch.device(self.device))
 
     # Embed text
     def embedding(self, text: str) -> torch.Tensor:
         '''
         Gets the embedding of the text using open source collections of models from HuggingFace Hub
```

### Comparing `panml-0.0.16/panml/core/llm/openai.py` & `panml-0.0.17/panml/core/llm/openai.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.16/panml/core/llm/prompt_template.py` & `panml-0.0.17/panml/core/llm/prompt_template.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.16/panml/models.py` & `panml-0.0.17/panml/models.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.16/panml/search.py` & `panml-0.0.17/panml/search.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.16/panml.egg-info/PKG-INFO` & `panml-0.0.17/panml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 0.0.16
+Version: 0.0.17
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-0.0.16/setup.py` & `panml-0.0.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 setup(
   name = 'panml', # package name     
   packages = find_packages(exclude=['test']), # package name
-  version = '0.0.16', # version
+  version = '0.0.17', # version
   license = 'MIT', # license
   description = 'PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.', # short description about the package
   long_description = 'PanML aims to make analysis and experimentation of generative AI/ML models more accessible, by providing a simple and consistent interface to foundation models for Data Scientists, Machine Learning Engineers and Software Developers. \
                       The package provides various assistive tools to work with generative language models, such as prompt engineering, fine tuning and others. \
                       \n\nQuick start guide: https://github.com/Pan-ML/panml/wiki/1.-Quick-start-guide \
                       \n\nDocumentation/Wiki: https://github.com/Pan-ML/panml/wiki', # long description
   author = 'PanML team', # team name
```

### Comparing `panml-0.0.16/test/test_ModelPack.py` & `panml-0.0.17/test/test_ModelPack.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,8 +56,21 @@
     
     # Test case: handle model and source correct match input
     print('Setup test_modelpack_correct_model_source_flan_input')
     def test_modelpack_correct_model_source_flan_input(self):
         # test valid model and source match combo 2
         m = ModelPack(model='google/flan-t5-small', source='huggingface')
 
+    # Test case: handle model GPU invalid type
+    print('Setup test_modelpack_incorrect_model_gpu_input')
+    def test_modelpack_incorrect_model_gpu_input(self):
+        # test invalid GPU setting input
+        with self.assertRaises(TypeError):
+            m = ModelPack(model='google/flan-t5-small', source='huggingface', model_args={'gpu': 1})
+
+    # Test case: handle model GPU correct input
+    print('Setup test_modelpack_correct_model_gpu_input')
+    def test_modelpack_correct_model_gpu_input(self):
+        # test valid GPU setting input
+        m = ModelPack(model='google/flan-t5-small', source='huggingface', model_args={'gpu': True})
+
```

### Comparing `panml-0.0.16/test/test_VectorEngine.py` & `panml-0.0.17/test/test_VectorEngine.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,35 @@
         # test invalid corpus query input type
         with self.assertRaises(TypeError):
             m = VectorEngine(model='distilbert-base-nli-stsb-mean-tokens', source='faiss')
             TEST_SAMPLE = []
             m.store(TEST_CORPUS_1, model_name=None)
             output = m.search(TEST_SAMPLE, 3)
 
+        # test invalid corpus query input is empty
+        with self.assertRaises(ValueError):
+            m = VectorEngine(model='distilbert-base-nli-stsb-mean-tokens', source='faiss')
+            TEST_SAMPLE = ''
+            m.store(TEST_CORPUS_1, model_name=None)
+            output = m.search(TEST_SAMPLE, 3)
+
+        # test invalid corpus k input type
+        with self.assertRaises(TypeError):
+            m = VectorEngine(model='distilbert-base-nli-stsb-mean-tokens', source='faiss')
+            TEST_SAMPLE = 'white rabbit'
+            m.store(TEST_CORPUS_1, model_name=None)
+            output = m.search(TEST_SAMPLE, 0.1)
+
+        # test invalid corpus k input is less than 1
+        with self.assertRaises(ValueError):
+            m = VectorEngine(model='distilbert-base-nli-stsb-mean-tokens', source='faiss')
+            TEST_SAMPLE = 'white rabbit'
+            m.store(TEST_CORPUS_1, model_name=None)
+            output = m.search(TEST_SAMPLE, -1)
+
     # Test case: validate FAISS vector search functionality
     print('Setup test_faiss_hf_vector_search')
     def test_faiss_hf_vector_search(self):
         # test sample input
         TEST_SAMPLES = [
             {
                 'text': 'white rabbit',
```

