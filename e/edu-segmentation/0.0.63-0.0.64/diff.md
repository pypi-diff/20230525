# Comparing `tmp/edu_segmentation-0.0.63.tar.gz` & `tmp/edu_segmentation-0.0.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edu_segmentation-0.0.63.tar", max compression
+gzip compressed data, was "edu_segmentation-0.0.64.tar", max compression
```

## Comparing `edu_segmentation-0.0.63.tar` & `edu_segmentation-0.0.64.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     3248 2023-04-28 16:15:32.248369 edu_segmentation-0.0.63/edu_segmentation/__init__.py
--rw-r--r--   0        0        0      325 2023-04-27 10:53:24.371538 edu_segmentation-0.0.63/edu_segmentation/bart_tokenizer.py
--rw-r--r--   0        0        0      671 2023-04-27 12:36:01.129982 edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc
--rw-r--r--   0        0        0      231 2023-04-27 10:53:25.896516 edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/config.py
--rw-r--r--   0        0        0     4321 2023-04-27 10:53:25.927765 edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/import_data_bert.py
--rw-r--r--   0        0        0     4882 2023-04-27 10:53:25.959014 edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py
--rw-r--r--   0        0        0     3312 2023-04-27 10:53:25.990406 edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/postagging.py
--rw-r--r--   0        0        0     3226 2023-04-27 10:53:26.030012 edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/postagging_new.py
--rw-r--r--   0        0        0    85404 2023-04-27 10:53:26.056731 edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/python38bert_modelling.py
--rw-r--r--   0        0        0     6409 2023-04-27 10:53:26.103614 edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/solver.py
--rw-r--r--   0        0        0     6978 2023-04-27 10:53:26.134865 edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/solver_postag.py
--rw-r--r--   0        0        0      537 2023-04-27 10:53:26.166114 edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/test_model.py
--rw-r--r--   0        0        0     1023 2023-04-27 10:53:26.197363 edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/train_model.py
--rw-r--r--   0        0        0     1313 2023-04-27 10:53:26.228615 edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/train_model_postag.py
--rw-r--r--   0        0        0      298 2023-04-27 10:53:24.434065 edu_segmentation-0.0.63/edu_segmentation/config.py
--rw-r--r--   0        0        0     3930 2023-04-28 12:33:56.340151 edu_segmentation-0.0.63/edu_segmentation/import_data_bart.py
--rw-r--r--   0        0        0        0 2023-04-27 16:13:15.942549 edu_segmentation-0.0.63/edu_segmentation/initial_dep.txt
--rw-r--r--   0        0        0     2572 2023-04-27 16:14:15.149001 edu_segmentation-0.0.63/edu_segmentation/initial_dep_conda.txt
--rw-r--r--   0        0        0    12186 2023-04-27 10:53:24.480926 edu_segmentation-0.0.63/edu_segmentation/model.py
--rw-r--r--   0        0        0   590031 2023-04-27 10:53:24.340305 edu_segmentation-0.0.63/edu_segmentation/model_dependencies/all_vocabulary.pickle
--rw-r--r--   0        0        0    11216 2023-04-27 10:53:24.512189 edu_segmentation-0.0.63/edu_segmentation/model_dependencies/model_bart_v2.py
--rw-r--r--   0        0        0     1510 2023-04-28 12:35:01.251942 edu_segmentation-0.0.63/edu_segmentation/model_dependencies/train_segbot_bart.py
--rw-r--r--   0        0        0     2584 2023-04-28 09:07:59.951990 edu_segmentation-0.0.63/edu_segmentation/requirements.txt
--rw-r--r--   0        0        0     4364 2023-04-28 16:04:21.009998 edu_segmentation-0.0.63/edu_segmentation/run_segbot.py
--rw-r--r--   0        0        0     7227 2023-05-25 10:26:55.834305 edu_segmentation-0.0.63/edu_segmentation/run_segbot_bart.py
--rw-r--r--   0        0        0     8974 2023-04-27 10:53:24.652797 edu_segmentation-0.0.63/edu_segmentation/solver.py
--rw-r--r--   0        0        0     9549 2023-05-25 10:27:05.194516 edu_segmentation-0.0.63/edu_segmentation/solver_bart.py
--rw-r--r--   0        0        0      589 2023-05-25 11:25:24.398786 edu_segmentation-0.0.63/pyproject.toml
--rw-r--r--   0        0        0      737 2023-04-28 16:39:16.999884 edu_segmentation-0.0.63/readme.md
--rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 edu_segmentation-0.0.63/PKG-INFO
+-rw-r--r--   0        0        0     3248 2023-04-28 16:15:32.248369 edu_segmentation-0.0.64/edu_segmentation/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-27 10:53:24.371538 edu_segmentation-0.0.64/edu_segmentation/bart_tokenizer.py
+-rw-r--r--   0        0        0      671 2023-04-27 12:36:01.129982 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc
+-rw-r--r--   0        0        0      231 2023-04-27 10:53:25.896516 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/config.py
+-rw-r--r--   0        0        0     4321 2023-04-27 10:53:25.927765 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/import_data_bert.py
+-rw-r--r--   0        0        0     4882 2023-04-27 10:53:25.959014 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py
+-rw-r--r--   0        0        0     3312 2023-04-27 10:53:25.990406 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/postagging.py
+-rw-r--r--   0        0        0     3226 2023-04-27 10:53:26.030012 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/postagging_new.py
+-rw-r--r--   0        0        0    85404 2023-04-27 10:53:26.056731 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/python38bert_modelling.py
+-rw-r--r--   0        0        0     6409 2023-04-27 10:53:26.103614 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/solver.py
+-rw-r--r--   0        0        0     6978 2023-04-27 10:53:26.134865 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/solver_postag.py
+-rw-r--r--   0        0        0      537 2023-04-27 10:53:26.166114 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/test_model.py
+-rw-r--r--   0        0        0     1023 2023-04-27 10:53:26.197363 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/train_model.py
+-rw-r--r--   0        0        0     1313 2023-04-27 10:53:26.228615 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/train_model_postag.py
+-rw-r--r--   0        0        0      298 2023-04-27 10:53:24.434065 edu_segmentation-0.0.64/edu_segmentation/config.py
+-rw-r--r--   0        0        0     3930 2023-04-28 12:33:56.340151 edu_segmentation-0.0.64/edu_segmentation/import_data_bart.py
+-rw-r--r--   0        0        0        0 2023-04-27 16:13:15.942549 edu_segmentation-0.0.64/edu_segmentation/initial_dep.txt
+-rw-r--r--   0        0        0     2572 2023-04-27 16:14:15.149001 edu_segmentation-0.0.64/edu_segmentation/initial_dep_conda.txt
+-rw-r--r--   0        0        0    12186 2023-04-27 10:53:24.480926 edu_segmentation-0.0.64/edu_segmentation/model.py
+-rw-r--r--   0        0        0   590031 2023-04-27 10:53:24.340305 edu_segmentation-0.0.64/edu_segmentation/model_dependencies/all_vocabulary.pickle
+-rw-r--r--   0        0        0    11216 2023-04-27 10:53:24.512189 edu_segmentation-0.0.64/edu_segmentation/model_dependencies/model_bart_v2.py
+-rw-r--r--   0        0        0     1510 2023-04-28 12:35:01.251942 edu_segmentation-0.0.64/edu_segmentation/model_dependencies/train_segbot_bart.py
+-rw-r--r--   0        0        0     2584 2023-04-28 09:07:59.951990 edu_segmentation-0.0.64/edu_segmentation/requirements.txt
+-rw-r--r--   0        0        0     4364 2023-04-28 16:04:21.009998 edu_segmentation-0.0.64/edu_segmentation/run_segbot.py
+-rw-r--r--   0        0        0     8583 2023-05-25 11:52:09.892681 edu_segmentation-0.0.64/edu_segmentation/run_segbot_bart.py
+-rw-r--r--   0        0        0     8974 2023-04-27 10:53:24.652797 edu_segmentation-0.0.64/edu_segmentation/solver.py
+-rw-r--r--   0        0        0    10912 2023-05-25 11:53:51.052894 edu_segmentation-0.0.64/edu_segmentation/solver_bart.py
+-rw-r--r--   0        0        0      589 2023-05-25 11:54:16.242430 edu_segmentation-0.0.64/pyproject.toml
+-rw-r--r--   0        0        0      737 2023-04-28 16:39:16.999884 edu_segmentation-0.0.64/readme.md
+-rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 edu_segmentation-0.0.64/PKG-INFO
```

### Comparing `edu_segmentation-0.0.63/edu_segmentation/__init__.py` & `edu_segmentation-0.0.64/edu_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc` & `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/import_data_bert.py` & `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/import_data_bert.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py` & `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/postagging.py` & `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/postagging.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/postagging_new.py` & `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/postagging_new.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/python38bert_modelling.py` & `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/python38bert_modelling.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/solver.py` & `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/solver.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/solver_postag.py` & `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/solver_postag.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/test_model.py` & `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/test_model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/train_model.py` & `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/train_model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/BERTTokenClassification/train_model_postag.py` & `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/train_model_postag.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/import_data_bart.py` & `edu_segmentation-0.0.64/edu_segmentation/import_data_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/initial_dep_conda.txt` & `edu_segmentation-0.0.64/edu_segmentation/initial_dep_conda.txt`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/model.py` & `edu_segmentation-0.0.64/edu_segmentation/model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/model_dependencies/all_vocabulary.pickle` & `edu_segmentation-0.0.64/edu_segmentation/model_dependencies/all_vocabulary.pickle`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/model_dependencies/model_bart_v2.py` & `edu_segmentation-0.0.64/edu_segmentation/model_dependencies/model_bart_v2.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/model_dependencies/train_segbot_bart.py` & `edu_segmentation-0.0.64/edu_segmentation/model_dependencies/train_segbot_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/requirements.txt` & `edu_segmentation-0.0.64/edu_segmentation/requirements.txt`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/run_segbot.py` & `edu_segmentation-0.0.64/edu_segmentation/run_segbot.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/run_segbot_bart.py` & `edu_segmentation-0.0.64/edu_segmentation/run_segbot_bart.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import warnings
 import re
 from typing import List
 
 import numpy as np
 
 import torch
@@ -10,45 +9,48 @@
 from .config import TEST_PATH, TOKENIZER
 from .import_data_bart import read_data
 from .solver_bart import TrainSolver
 
 import os
 import time
 import sys
-sys.path.insert(0, os.path.join(os.path.dirname(__file__),'model_dependencies'))
+
+sys.path.insert(0, os.path.join(os.path.dirname(__file__), "model_dependencies"))
 
 warnings.filterwarnings("ignore")
 
 start_time = time.time()
+
+
 def bart_tokenizer(text: str) -> List[int]:
-    '''
+    """
     :param text:
     :return:
     Add special tokens to the start and end of each sentence
     Pad & truncate all sentences to a single constant length.
     Explicitly differentiate real tokens from padding tokens with the “attention mask”.
 
-    '''
+    """
     tokens = TOKENIZER.encode_plus(
-        text,                      # Sentence to encode.
+        text,  # Sentence to encode.
         add_special_tokens=True,  # Add '[CLS]' and '[SEP]'
-        return_attention_mask=True,   # Construct attn. masks.
+        return_attention_mask=True,  # Construct attn. masks.
     )
 
-    dec = TOKENIZER.decode(tokens['input_ids'])
+    dec = TOKENIZER.decode(tokens["input_ids"])
     # print(dec)
 
     # remove sep tokens
-    return tokens['input_ids'][1:-1], tokens['attention_mask'][1:-1]
+    return tokens["input_ids"][1:-1], tokens["attention_mask"][1:-1]
 
 
 def parse_input(inputstring: str):
-    '''
+    """
     Split sentences by the full stop and form input sequences with a token length of 128
-    '''
+    """
     max_token_len = 128
 
     sentences = inputstring.split(" . ")
     all_tokens = []
     all_masks = []
     all_boundaries = []
 
@@ -91,15 +93,15 @@
             all_boundaries.append(np.asarray(cur_boundaries))
 
             cur_tokens = []
             cur_mask = []
             cur_boundaries = []
             cur = 0
 
-    if (cur_tokens != []):
+    if cur_tokens != []:
         pad_tokens_count = max_token_len - len(cur_tokens)
         pad = [1] * pad_tokens_count
         cur_tokens.extend(pad)
 
         mask_remaining = [0] * pad_tokens_count
         cur_mask.extend(mask_remaining)
 
@@ -110,79 +112,151 @@
         all_masks.append(np.asarray(cur_mask))
         all_boundaries.append(np.asarray(cur_boundaries))
 
     return all_tokens, all_masks, all_boundaries
 
 
 def get_inference(inputstring):
-    '''
+    """
     Load trained model and run the inference on each input sequence
-    '''
+    """
     X_in, X_mask, Y_in = parse_input(inputstring)
     segments = []
-    directory_to_look = os.path.join(os.path.dirname(__file__), 'model_dependencies/model_segbot_bart.torchsave')
+    directory_to_look = os.path.join(
+        os.path.dirname(__file__), "model_dependencies/model_segbot_bart.torchsave"
+    )
     mymodel = torch.load(directory_to_look)
     mymodel.use_cuda = False
 
     mymodel.eval()
 
-    mysolver = TrainSolver(mymodel, train_x='', train_x_mask='', train_y='', dev_x='',
-                           dev_x_mask='', dev_y='', save_path='',
-                           batch_size=1, eval_size=1, epoch=10, lr=0.00015, lr_decay_epoch=1, weight_decay=0.0002,
-                           use_cuda=False)
+    mysolver = TrainSolver(
+        mymodel,
+        train_x="",
+        train_x_mask="",
+        train_y="",
+        dev_x="",
+        dev_x_mask="",
+        dev_y="",
+        save_path="",
+        batch_size=1,
+        eval_size=1,
+        epoch=10,
+        lr=0.00015,
+        lr_decay_epoch=1,
+        weight_decay=0.0002,
+        use_cuda=False,
+    )
 
     for i in range(len(X_in)):
         start_time = time.time()
         cur_X_in = np.asarray([X_in[i]])
         cur_X_mask = np.asarray([X_mask[i]])
         cur_Y_in = np.asarray([Y_in[i]])
 
         all_visdata = []
 
-        test_batch_ave_loss, test_pre, test_rec, test_f1, visdata = mysolver.check_accuracy(
-            cur_X_in, cur_X_mask, cur_Y_in)
+        (
+            test_batch_ave_loss,
+            test_pre,
+            test_rec,
+            test_f1,
+            visdata,
+        ) = mysolver.check_accuracy(cur_X_in, cur_X_mask, cur_Y_in)
 
         start_b = visdata[3][0]
         end_b = visdata[2][0] + 1
 
         for j, END in enumerate(end_b):
             # print(start_b[j], end_b[j])
-            seg = TOKENIZER.decode(X_in[i][start_b[j]: END])
+            seg = TOKENIZER.decode(X_in[i][start_b[j] : END])
             segments.append([f"{str(start_b[j])},{str(end_b[j])}", seg])
             # print(seg)
 
         # time_taken = time.time() - start_time
-  
+
         # print("--- %s seconds ---" % (time.time() - start_time))
 
     return segments
 
 
 # if __name__ == '__main__':
-    #sent="In ASEAN, there are currently government initiatives to encourage renewable energy, with Singapore predicting that hydrogen could supply up to half of the power needs in Singapore by 2050 and Thailand with a Hydrogen goal of 10 Kilotons of oil equivalent in total by 2036."
-    #sent="Furthermore, the current advancements in technology for hydrogen energy is able to reduce costs in terms of production and storage of hydrogen energy. As the technology continues to improve, it is expected to further lower the cost of production, achieving economies of scale."
-    #sent='Singapore recently announced that it is moving to a new Covid-19 innoculation strategy, with the focus on an individual’s vaccination being up-to-date, similar to how influenza jabs are administered seasonally. This comes as the country fights another wave of coronavirus infections, spurred by the emergence of the Omicron XBB sub-variant. '
-    #     sent="Aerial warfare has been around for much longer than modern aircraft have. More than 1,000 years ago, armies in China used incendiary kites known as fire crows to rain fire and debris upon their enemies. Since then, everything from kites to hot air balloons and airplanes have been used to inflict damage from above."
+# sent="In ASEAN, there are currently government initiatives to encourage renewable energy, with Singapore predicting that hydrogen could supply up to half of the power needs in Singapore by 2050 and Thailand with a Hydrogen goal of 10 Kilotons of oil equivalent in total by 2036."
+# sent="Furthermore, the current advancements in technology for hydrogen energy is able to reduce costs in terms of production and storage of hydrogen energy. As the technology continues to improve, it is expected to further lower the cost of production, achieving economies of scale."
+# sent='Singapore recently announced that it is moving to a new Covid-19 innoculation strategy, with the focus on an individual’s vaccination being up-to-date, similar to how influenza jabs are administered seasonally. This comes as the country fights another wave of coronavirus infections, spurred by the emergence of the Omicron XBB sub-variant. '
+#     sent="Aerial warfare has been around for much longer than modern aircraft have. More than 1,000 years ago, armies in China used incendiary kites known as fire crows to rain fire and debris upon their enemies. Since then, everything from kites to hot air balloons and airplanes have been used to inflict damage from above."
+
+
+def run_segbot_bart(sent, granularity_level="default"):
+    results = []
+
+    if granularity_level == "conjunction_words":
+        conjunctions = [
+            "and",
+            "but",
+            "or",
+            "so",
+            "for",
+            "nor",
+            "yet",
+            "after",
+            "although",
+            "as",
+            "because",
+            "before",
+            "if",
+            "once",
+            "since",
+            "than",
+            "that",
+            "though",
+            "till",
+            "unless",
+            "until",
+            "when",
+            "where",
+            "whether",
+            "while",
+        ]
+        segments = []
+        current_segment = []
+        words = sent.split()
+
+        for word in words:
+            if word.lower() in conjunctions:
+                if current_segment:
+                    segments.append(" ".join(current_segment))
+                current_segment.clear()
+            else:
+                current_segment.append(word)
+
+        if current_segment:
+            segments.append(" ".join(current_segment))
+        for word in segments:
+            results.append(core_run_segbot_bart(word))
+    else:
+        results.append(core_run_segbot_bart(sent))
+    return results
+
 
-def run_segbot_bart():
+def core_run_segbot_bart(sent):
     print("----------- EDU Segmentation with Segbot with BART model: ----------")
-    sent = input("Enter text for EDU segmentation: \n")
-    sent = sent.replace(", ",  " , ").replace(". ",  " . ").replace(
-        "; ",  " ; ")
+    # sent = input("Enter text for EDU segmentation: \n")
+    sent = sent.replace(", ", " , ").replace(". ", " . ").replace("; ", " ; ")
     if sent[-1] == ".":
         sent = sent[:-1] + " ."
     print("\n")
     # print("---------- Start of EDU segmentation ----------")
     output_seg = get_inference(sent)
     print("EDU Segmentation Results:\n", output_seg)
     # print("---------- End of EDU segmentation ----------\n")
 
-    '''
+    """
     Get inference time by each new line of input
-    '''
+    """
     # all_files = os.listdir(TEST_PATH)
     # total = 0
     # for file in all_files:
     #     with open(TEST_PATH + file, 'r') as f:
     #         file_text = f.read()
     #         sentences = file_text.split("\n")
     #         total += len(sentences)
@@ -192,9 +266,7 @@
     #                 new_sent = sent.replace(" EDU_BREAK", "")
     #                 output_seg =  main_input_output(new_sent)
     #             except Exception as e:
     #                 print(e)
     # print(total)
     # print("Total inference time")
     # print("--- %s seconds ---" % (time.time() - start_time))
-
-
```

### Comparing `edu_segmentation-0.0.63/edu_segmentation/solver.py` & `edu_segmentation-0.0.64/edu_segmentation/solver.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/edu_segmentation/solver_bart.py` & `edu_segmentation-0.0.64/edu_segmentation/solver_bart.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,368 +1,384 @@
-
-
 import torch.optim as optim
 import numpy as np
 import torch
 from torch.autograd import Variable
 
 import random
 from torch.nn.utils import clip_grad_norm
 import copy
 
 
 import os
 
 
-
-
 def get_decoder_index_XY(batchY):
-    '''
+    """
 
     :param batchY: like [0 0 1 0 0 0 0 1]
     :return:
-    '''
-
+    """
 
-    returnX =[]
-    returnY =[]
+    returnX = []
+    returnY = []
 
     for i in range(len(batchY)):
-
         curY = batchY[i]
 
-        index_1 = np.where(curY==1)
+        index_1 = np.where(curY == 1)
 
         decoderY = index_1[0]
 
-        if len(index_1[0]) ==1:
+        if len(index_1[0]) == 1:
             decoderX = np.array([0])
         else:
-            decoderX = np.append([0],decoderY[0:-1]+1)
+            decoderX = np.append([0], decoderY[0:-1] + 1)
 
         returnX.append(decoderX)
         returnY.append(decoderY)
 
     returnX = np.array(returnX)
     returnY = np.array(returnY)
 
-    return returnX,returnY
+    return returnX, returnY
 
-def align_variable_numpy(X,maxL,paddingNumber):
 
+def align_variable_numpy(X, maxL, paddingNumber):
     aligned = []
     for cur in X:
         ext_cur = []
         ext_cur.extend(cur)
         ext_cur.extend([paddingNumber] * (maxL - len(cur)))
         aligned.append(ext_cur)
     aligned = np.array(aligned)
 
     return aligned
 
 
-def sample_a_sorted_batch_from_numpy(numpyX,numpyX_mask,numpyY,batch_size,use_cuda):
-
-
+def sample_a_sorted_batch_from_numpy(numpyX, numpyX_mask, numpyY, batch_size, use_cuda):
     if batch_size != None:
         select_index = random.sample(range(len(numpyY)), batch_size)
     else:
         select_index = np.array(range(len(numpyY)))
 
     batch_x = copy.deepcopy(numpyX[select_index])
     batch_x_mask = copy.deepcopy(numpyX_mask[select_index])
     batch_y = copy.deepcopy(numpyY[select_index])
 
-    index_decoder_X,index_decoder_Y = get_decoder_index_XY(batch_y)
+    index_decoder_X, index_decoder_Y = get_decoder_index_XY(batch_y)
     # print(index_decoder_X, index_decoder_Y)
 
-
-
-
     all_lens = np.array([len(x) for x in batch_y])
     maxL = np.max(all_lens)
 
     idx = np.argsort(all_lens)
     idx = idx[::-1]  # decreasing
 
     batch_x = batch_x[idx]
     batch_x_mask = batch_x_mask[idx]
     batch_y = batch_y[idx]
     all_lens = all_lens[idx]
 
     index_decoder_X = index_decoder_X[idx]
     index_decoder_Y = index_decoder_Y[idx]
 
-
     numpy_batch_x = batch_x
 
-
-
     # batch_x = align_variable_numpy(batch_x,maxL,0)
     # batch_x_mask = align_variable_numpy(batch_x_mask, maxL, 0)
     # batch_y = align_variable_numpy(batch_y,maxL,2)
 
-
-
-
-
-
-
-
     batch_x = Variable(torch.from_numpy(batch_x.astype(np.int64)))
     batch_x_mask = Variable(torch.from_numpy(batch_x_mask.astype(np.int64)))
 
-
-
     if use_cuda:
         batch_x = batch_x.cuda()
 
-
-
-    return  numpy_batch_x,batch_x, batch_x_mask, batch_y,index_decoder_X,index_decoder_Y,all_lens,maxL
-
-
+    return (
+        numpy_batch_x,
+        batch_x,
+        batch_x_mask,
+        batch_y,
+        index_decoder_X,
+        index_decoder_Y,
+        all_lens,
+        maxL,
+    )
 
 
 class TrainSolver(object):
-    def __init__(self, model,train_x,train_x_mask,train_y,dev_x,dev_x_mask,dev_y,save_path,batch_size,eval_size,epoch, lr,lr_decay_epoch,weight_decay,use_cuda):
-
+    def __init__(
+        self,
+        model,
+        train_x,
+        train_x_mask,
+        train_y,
+        dev_x,
+        dev_x_mask,
+        dev_y,
+        save_path,
+        batch_size,
+        eval_size,
+        epoch,
+        lr,
+        lr_decay_epoch,
+        weight_decay,
+        use_cuda,
+    ):
         self.lr = lr
         self.model = model
         self.epoch = epoch
         self.train_x = train_x
         self.train_x_mask = train_x_mask
         self.train_y = train_y
         self.use_cuda = use_cuda
         self.batch_size = batch_size
         self.lr_decay_epoch = lr_decay_epoch
-        self.eval_size  = eval_size
-
+        self.eval_size = eval_size
 
         self.dev_x, self.dev_y = dev_x, dev_y
         self.dev_x_mask = dev_x_mask
 
         self.model = model
         self.save_path = save_path
-        self.weight_decay =weight_decay
-
-
-
+        self.weight_decay = weight_decay
 
     def sample_dev(self):
-
-        select_index = random.sample(range(len(self.train_y)),self.eval_size)
+        select_index = random.sample(range(len(self.train_y)), self.eval_size)
 
         test_tr_x = self.train_x[select_index]
         test_tr_x_mask = self.train_x_mask[select_index]
         test_tr_y = self.train_y[select_index]
 
-        return test_tr_x,test_tr_x_mask,test_tr_y
-
-
-
-
-
-
-
-    def get_batch_micro_metric(self,pre_b, ground_b):
-
-
+        return test_tr_x, test_tr_x_mask, test_tr_y
 
+    def get_batch_micro_metric(self, pre_b, ground_b):
         All_C = []
         All_R = []
         All_G = []
-        for i,cur_seq_y in enumerate(ground_b):
-            index_of_1 = np.where(cur_seq_y==1)[0]
+        for i, cur_seq_y in enumerate(ground_b):
+            index_of_1 = np.where(cur_seq_y == 1)[0]
             index_pre = pre_b[i]
 
-
-
             index_pre = np.array(index_pre)
             END_B = index_of_1[-1]
             index_pre = index_pre[index_pre != END_B]
             index_of_1 = index_of_1[index_of_1 != END_B]
 
             no_correct = len(np.intersect1d(list(index_of_1), list(index_pre)))
             All_C.append(no_correct)
             All_R.append(len(index_pre))
             All_G.append(len(index_of_1))
 
+        return All_C, All_R, All_G
 
-        return All_C,All_R,All_G
-
-
-
-
-
-    def get_batch_metric(self,pre_b, ground_b):
-
-        b_pr =[]
-        b_re =[]
-        b_f1 =[]
-        for i,cur_seq_y in enumerate(ground_b):
-            index_of_1 = np.where(cur_seq_y==1)[0]
+    def get_batch_metric(self, pre_b, ground_b):
+        b_pr = []
+        b_re = []
+        b_f1 = []
+        for i, cur_seq_y in enumerate(ground_b):
+            index_of_1 = np.where(cur_seq_y == 1)[0]
             index_pre = pre_b[i]
 
-            no_correct = len(np.intersect1d(index_of_1,index_pre))
+            no_correct = len(np.intersect1d(index_of_1, index_pre))
 
             cur_pre = no_correct / len(index_pre)
             cur_rec = no_correct / len(index_of_1)
-            cur_f1 = 2*cur_pre*cur_rec/ (cur_pre+cur_rec)
+            cur_f1 = 2 * cur_pre * cur_rec / (cur_pre + cur_rec)
 
             b_pr.append(cur_pre)
             b_re.append(cur_rec)
             b_f1.append(cur_f1)
 
-        return b_pr,b_re,b_f1
-
-
-
-    def check_accuracy(self,dataX,dataX_mask,dataY):
-
+        return b_pr, b_re, b_f1
 
+    def check_accuracy(self, dataX, dataX_mask, dataY):
         need_loop = int(np.ceil(len(dataY) / self.batch_size))
 
-        all_ave_loss =[]
-        all_boundary =[]
+        all_ave_loss = []
+        all_boundary = []
         all_boundary_start = []
         all_align_matrix = []
-        all_index_decoder_y =[]
+        all_index_decoder_y = []
         all_x_save = []
 
-        all_C =[]
-        all_R =[]
-        all_G =[]
+        all_C = []
+        all_R = []
+        all_G = []
         for lp in range(need_loop):
-            startN = lp*self.batch_size
-            endN =  (lp+1)*self.batch_size
+            startN = lp * self.batch_size
+            endN = (lp + 1) * self.batch_size
             if endN > len(dataY):
                 endN = len(dataY)
 
-            numpy_batch_x, batch_x, batch_x_mask, batch_y, index_decoder_X, index_decoder_Y, all_lens, maxL = sample_a_sorted_batch_from_numpy(
-                dataX[startN:endN], dataX_mask[startN:endN], dataY[startN:endN], None, self.use_cuda)
-
-
-            batch_ave_loss, batch_boundary, batch_boundary_start, batch_align_matrix = self.model.predict(batch_x, batch_x_mask,
-                                                                                                      index_decoder_Y,
-                                                                                                  all_lens)
-
-            all_ave_loss.extend([batch_ave_loss.data])  #[batch_ave_loss.data[0]]
+            (
+                numpy_batch_x,
+                batch_x,
+                batch_x_mask,
+                batch_y,
+                index_decoder_X,
+                index_decoder_Y,
+                all_lens,
+                maxL,
+            ) = sample_a_sorted_batch_from_numpy(
+                dataX[startN:endN],
+                dataX_mask[startN:endN],
+                dataY[startN:endN],
+                None,
+                self.use_cuda,
+            )
+
+            (
+                batch_ave_loss,
+                batch_boundary,
+                batch_boundary_start,
+                batch_align_matrix,
+            ) = self.model.predict(batch_x, batch_x_mask, index_decoder_Y, all_lens)
+
+            try:
+                all_ave_loss.extend([batch_ave_loss.data])  # [batch_ave_loss.data[0]]
+            except:
+                all_ave_loss.extend([batch_ave_loss])
             all_boundary.extend(batch_boundary)
             all_boundary_start.extend(batch_boundary_start)
             all_align_matrix.extend(batch_align_matrix)
             all_index_decoder_y.extend(index_decoder_Y)
             all_x_save.extend(numpy_batch_x)
 
-
-
-
-            ba_C,ba_R,ba_G = self.get_batch_micro_metric(batch_boundary,batch_y)
+            ba_C, ba_R, ba_G = self.get_batch_micro_metric(batch_boundary, batch_y)
 
             all_C.extend(ba_C)
             all_R.extend(ba_R)
             all_G.extend(ba_G)
 
+        ba_pre = np.sum(all_C) / np.sum(all_R)
+        ba_rec = np.sum(all_C) / np.sum(all_G)
+        ba_f1 = 2 * ba_pre * ba_rec / (ba_pre + ba_rec)
+
+        return (
+            np.mean(all_ave_loss),
+            ba_pre,
+            ba_rec,
+            ba_f1,
+            (
+                all_x_save,
+                all_index_decoder_y,
+                all_boundary,
+                all_boundary_start,
+                all_align_matrix,
+            ),
+        )
 
-        ba_pre = np.sum(all_C)/ np.sum(all_R)
-        ba_rec = np.sum(all_C)/ np.sum(all_G)
-        ba_f1 = 2*ba_pre*ba_rec/ (ba_pre+ba_rec)
-
-
-        return np.mean(all_ave_loss),ba_pre,ba_rec,ba_f1, (all_x_save,all_index_decoder_y,all_boundary, all_boundary_start, all_align_matrix)
-
-
-
-
-
-
-
-    def adjust_learning_rate(self,optimizer,epoch,lr_decay=0.5, lr_decay_epoch=50):
-
+    def adjust_learning_rate(self, optimizer, epoch, lr_decay=0.5, lr_decay_epoch=50):
         if (epoch % lr_decay_epoch == 0) and (epoch != 0):
             for param_group in optimizer.param_groups:
-                param_group['lr'] *= lr_decay
-
-
+                param_group["lr"] *= lr_decay
 
     def train(self):
-
         self.test_train_x, self.test_train_x_mask, self.test_train_y = self.sample_dev()
 
-        optimizer = optim.Adam(filter(lambda p: p.requires_grad, self.model.parameters()), lr=self.lr, weight_decay=self.weight_decay)
-
-
+        optimizer = optim.Adam(
+            filter(lambda p: p.requires_grad, self.model.parameters()),
+            lr=self.lr,
+            weight_decay=self.weight_decay,
+        )
 
         num_each_epoch = int(np.round(len(self.train_y) / self.batch_size))
 
         os.mkdir(self.save_path)
 
-        best_i =0
-        best_f1 =0
+        best_i = 0
+        best_f1 = 0
 
         for epoch in range(self.epoch):
-
             self.adjust_learning_rate(optimizer, epoch, 0.5, self.lr_decay_epoch)
 
             track_epoch_loss = []
             for iter in range(num_each_epoch):
                 print("epoch:%d,iteration:%d" % (epoch, iter))
 
-                numpy_batch_x, batch_x, batch_x_mask, batch_y, index_decoder_X, index_decoder_Y, all_lens, maxL = sample_a_sorted_batch_from_numpy(
-                    self.train_x, self.train_x_mask, self.train_y, self.batch_size, self.use_cuda)
+                (
+                    numpy_batch_x,
+                    batch_x,
+                    batch_x_mask,
+                    batch_y,
+                    index_decoder_X,
+                    index_decoder_Y,
+                    all_lens,
+                    maxL,
+                ) = sample_a_sorted_batch_from_numpy(
+                    self.train_x,
+                    self.train_x_mask,
+                    self.train_y,
+                    self.batch_size,
+                    self.use_cuda,
+                )
 
                 self.model.zero_grad()
 
                 if not np.any(index_decoder_X):
                     continue
 
-
-                neg_loss = self.model.neg_log_likelihood(batch_x, batch_x_mask, index_decoder_X, index_decoder_Y,all_lens)
-
-
+                neg_loss = self.model.neg_log_likelihood(
+                    batch_x, batch_x_mask, index_decoder_X, index_decoder_Y, all_lens
+                )
 
                 neg_loss_v = float(neg_loss.item())
                 print(neg_loss_v)
                 track_epoch_loss.append(neg_loss_v)
 
                 neg_loss.backward()
 
                 clip_grad_norm(self.model.parameters(), 5)
                 optimizer.step()
 
-
-            #TODO: after each epoch,check accuracy
-
+            # TODO: after each epoch,check accuracy
 
             self.model.eval()
 
-            tr_batch_ave_loss, tr_pre, tr_rec, tr_f1 ,visdata=    self.check_accuracy(self.test_train_x, self.test_train_x_mask, self.test_train_y)
-
-            dev_batch_ave_loss, dev_pre, dev_rec, dev_f1, visdata =self.check_accuracy(self.dev_x, self.dev_x_mask, self.dev_y)
+            tr_batch_ave_loss, tr_pre, tr_rec, tr_f1, visdata = self.check_accuracy(
+                self.test_train_x, self.test_train_x_mask, self.test_train_y
+            )
+
+            dev_batch_ave_loss, dev_pre, dev_rec, dev_f1, visdata = self.check_accuracy(
+                self.dev_x, self.dev_x_mask, self.dev_y
+            )
             print()
 
             if best_f1 < dev_f1:
                 best_f1 = dev_f1
                 best_rec = dev_rec
                 best_pre = dev_pre
                 best_i = epoch
 
-
-
-            save_data = [epoch,tr_batch_ave_loss,tr_pre,tr_rec,tr_f1,
-                         dev_batch_ave_loss,dev_pre,dev_rec,dev_f1]
-
-
-            save_file_name = 'bs_{}_es_{}_lr_{}_lrdc_{}_wd_{}_epoch_loss_acc_pk_wd.txt'.format(self.batch_size,self.eval_size,self.lr,self.lr_decay_epoch,self.weight_decay)
-            with open(os.path.join(self.save_path,save_file_name), 'a') as f:
-                f.write(','.join(map(str,save_data))+'\n')
-
-
-            torch.save(self.model, os.path.join(self.save_path,r'model_epoch_%d.torchsave'%(epoch)))
-
+            save_data = [
+                epoch,
+                tr_batch_ave_loss,
+                tr_pre,
+                tr_rec,
+                tr_f1,
+                dev_batch_ave_loss,
+                dev_pre,
+                dev_rec,
+                dev_f1,
+            ]
+
+            save_file_name = (
+                "bs_{}_es_{}_lr_{}_lrdc_{}_wd_{}_epoch_loss_acc_pk_wd.txt".format(
+                    self.batch_size,
+                    self.eval_size,
+                    self.lr,
+                    self.lr_decay_epoch,
+                    self.weight_decay,
+                )
+            )
+            with open(os.path.join(self.save_path, save_file_name), "a") as f:
+                f.write(",".join(map(str, save_data)) + "\n")
+
+            torch.save(
+                self.model,
+                os.path.join(self.save_path, r"model_epoch_%d.torchsave" % (epoch)),
+            )
 
             self.model.train()
 
-        return best_i,best_pre,best_rec,best_f1
-
-
-
+        return best_i, best_pre, best_rec, best_f1
```

### Comparing `edu_segmentation-0.0.63/pyproject.toml` & `edu_segmentation-0.0.64/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edu_segmentation"
-version = "v0.0.63"
+version = "v0.0.64"
 description = "To improve EDU segmentation performance using Segbot. As Segbot has an encoder-decoder model architecture, we can replace bidirectional GRU encoder with generative pretraining models such as BART and T5. Evaluate the new model using the RST dataset by using few-shot based settings (e.g. 100 examples) to train the model, instead of using the full dataset."
 authors = ["Your Name <you@example.com>"]
 readme = "readme.md"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `edu_segmentation-0.0.63/readme.md` & `edu_segmentation-0.0.64/readme.md`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.63/PKG-INFO` & `edu_segmentation-0.0.64/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edu-segmentation
-Version: 0.0.63
+Version: 0.0.64
 Summary: To improve EDU segmentation performance using Segbot. As Segbot has an encoder-decoder model architecture, we can replace bidirectional GRU encoder with generative pretraining models such as BART and T5. Evaluate the new model using the RST dataset by using few-shot based settings (e.g. 100 examples) to train the model, instead of using the full dataset.
 Author: Your Name
 Author-email: you@example.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

