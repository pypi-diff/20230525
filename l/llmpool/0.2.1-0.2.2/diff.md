# Comparing `tmp/llmpool-0.2.1-py3-none-any.whl.zip` & `tmp/llmpool-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9647 bytes, number of entries: 10
--rw-r--r--  2.0 unx      157 b- defN 23-May-13 14:12 llmpool/__init__.py
--rw-r--r--  2.0 unx     4202 b- defN 23-May-13 14:11 llmpool/local_model.py
+Zip file size: 9674 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      157 b- defN 23-May-25 02:29 llmpool/__init__.py
+-rw-r--r--  2.0 unx     4254 b- defN 23-May-25 02:28 llmpool/local_model.py
 -rw-r--r--  2.0 unx      668 b- defN 23-May-13 14:10 llmpool/model.py
 -rw-r--r--  2.0 unx     2817 b- defN 23-May-13 14:10 llmpool/model_pool.py
 -rw-r--r--  2.0 unx     2312 b- defN 23-May-13 14:10 llmpool/remote_model.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-13 14:12 llmpool-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2409 b- defN 23-May-13 14:12 llmpool-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-13 14:12 llmpool-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-May-13 14:12 llmpool-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      770 b- defN 23-May-13 14:12 llmpool-0.2.1.dist-info/RECORD
-10 files, 24792 bytes uncompressed, 8345 bytes compressed:  66.3%
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-25 02:29 llmpool-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2409 b- defN 23-May-25 02:29 llmpool-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-25 02:29 llmpool-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-May-25 02:29 llmpool-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      770 b- defN 23-May-25 02:29 llmpool-0.2.2.dist-info/RECORD
+10 files, 24844 bytes uncompressed, 8372 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: llmpool/model_pool.py
 Comment: 
 
 Filename: llmpool/remote_model.py
 Comment: 
 
-Filename: llmpool-0.2.1.dist-info/LICENSE
+Filename: llmpool-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: llmpool-0.2.1.dist-info/METADATA
+Filename: llmpool-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: llmpool-0.2.1.dist-info/WHEEL
+Filename: llmpool-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: llmpool-0.2.1.dist-info/top_level.txt
+Filename: llmpool-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: llmpool-0.2.1.dist-info/RECORD
+Filename: llmpool-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## llmpool/__init__.py

```diff
@@ -1,5 +1,5 @@
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 
 from .local_model import LocalLLModel, LocalLoRALLModel
 from .model_pool import LLModelPool
 from .remote_model import TxtGenIfLLModel
```

## llmpool/local_model.py

```diff
@@ -1,9 +1,10 @@
 from threading import Thread
 
+import torch
 from peft import PeftModel
 from transformers import GenerationConfig
 from transformers import AutoModel, AutoTokenizer
 from transformers import TextIteratorStreamer
 from optimum.bettertransformer import BetterTransformer
 
 from llmpool.model import LLModel
@@ -17,14 +18,15 @@
     ):
         super().__init__(name, gen_config, metadata)
 
         self.device = device
         self.tokenizer = tokenizer_cls.from_pretrained(base)
         self.model = model_cls.from_pretrained(
             base,
+            torch_dtype=torch.float16,
             load_in_8bit=load_in_8bit,
             device_map="auto",
         )
         
         if apply_bettertransformer:
             self.model = BetterTransformer.transform(self.model)
```

## Comparing `llmpool-0.2.1.dist-info/LICENSE` & `llmpool-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `llmpool-0.2.1.dist-info/METADATA` & `llmpool-0.2.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmpool
-Version: 0.2.1
+Version: 0.2.2
 Summary: Large Language Models' pool management library
 Home-page: https://github.com/deep-diver/LLM-Pool
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,instance pool,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `llmpool-0.2.1.dist-info/RECORD` & `llmpool-0.2.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-llmpool/__init__.py,sha256=5vUs-CGMOcTfpIwrt4HY1UuuYWnsKB7bHaAMl0tqA2g,157
-llmpool/local_model.py,sha256=xHxcG0L91T0xliZqsBHwTiPqXY2LXgQRemPejm2NFmU,4202
+llmpool/__init__.py,sha256=4vzpw9_m5-Rpcm3hiyXYjL8Dmf5rlV0HCrtwPb28Bfk,157
+llmpool/local_model.py,sha256=ShteTqd7A87Om4sRxOj9OhYrz8hJ9gA0-sO5bSFcirA,4254
 llmpool/model.py,sha256=iZPRIwUAd76bH__pDTcx9ef1-DY55F6etOROb44F1qk,668
 llmpool/model_pool.py,sha256=v5cwRDHSldPS_uO_9fS9nhZypNuTmfjXhqCL_KSRfmQ,2817
 llmpool/remote_model.py,sha256=Rw5tapaqbJ1V3Y9BrkA8z60yk_SvfSVN-PDPnsBN5SY,2312
-llmpool-0.2.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-llmpool-0.2.1.dist-info/METADATA,sha256=EImBNuepk1qRZfHEaqQQdsY6xTCowG_ssewL3Km__aE,2409
-llmpool-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-llmpool-0.2.1.dist-info/top_level.txt,sha256=1kKiMvue6u12IMQD92YMn4xdcQPDejrD0VuDl-pOCjE,8
-llmpool-0.2.1.dist-info/RECORD,,
+llmpool-0.2.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+llmpool-0.2.2.dist-info/METADATA,sha256=JrZC7_7wPPnlYrKC-BMPsEG-Q1tAbGjSalcsZREQsWI,2409
+llmpool-0.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+llmpool-0.2.2.dist-info/top_level.txt,sha256=1kKiMvue6u12IMQD92YMn4xdcQPDejrD0VuDl-pOCjE,8
+llmpool-0.2.2.dist-info/RECORD,,
```

