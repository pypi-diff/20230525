# Comparing `tmp/edu_segmentation-0.0.64.tar.gz` & `tmp/edu_segmentation-0.0.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edu_segmentation-0.0.64.tar", max compression
+gzip compressed data, was "edu_segmentation-0.0.65.tar", max compression
```

## Comparing `edu_segmentation-0.0.64.tar` & `edu_segmentation-0.0.65.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     3248 2023-04-28 16:15:32.248369 edu_segmentation-0.0.64/edu_segmentation/__init__.py
--rw-r--r--   0        0        0      325 2023-04-27 10:53:24.371538 edu_segmentation-0.0.64/edu_segmentation/bart_tokenizer.py
--rw-r--r--   0        0        0      671 2023-04-27 12:36:01.129982 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc
--rw-r--r--   0        0        0      231 2023-04-27 10:53:25.896516 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/config.py
--rw-r--r--   0        0        0     4321 2023-04-27 10:53:25.927765 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/import_data_bert.py
--rw-r--r--   0        0        0     4882 2023-04-27 10:53:25.959014 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py
--rw-r--r--   0        0        0     3312 2023-04-27 10:53:25.990406 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/postagging.py
--rw-r--r--   0        0        0     3226 2023-04-27 10:53:26.030012 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/postagging_new.py
--rw-r--r--   0        0        0    85404 2023-04-27 10:53:26.056731 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/python38bert_modelling.py
--rw-r--r--   0        0        0     6409 2023-04-27 10:53:26.103614 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/solver.py
--rw-r--r--   0        0        0     6978 2023-04-27 10:53:26.134865 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/solver_postag.py
--rw-r--r--   0        0        0      537 2023-04-27 10:53:26.166114 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/test_model.py
--rw-r--r--   0        0        0     1023 2023-04-27 10:53:26.197363 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/train_model.py
--rw-r--r--   0        0        0     1313 2023-04-27 10:53:26.228615 edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/train_model_postag.py
--rw-r--r--   0        0        0      298 2023-04-27 10:53:24.434065 edu_segmentation-0.0.64/edu_segmentation/config.py
--rw-r--r--   0        0        0     3930 2023-04-28 12:33:56.340151 edu_segmentation-0.0.64/edu_segmentation/import_data_bart.py
--rw-r--r--   0        0        0        0 2023-04-27 16:13:15.942549 edu_segmentation-0.0.64/edu_segmentation/initial_dep.txt
--rw-r--r--   0        0        0     2572 2023-04-27 16:14:15.149001 edu_segmentation-0.0.64/edu_segmentation/initial_dep_conda.txt
--rw-r--r--   0        0        0    12186 2023-04-27 10:53:24.480926 edu_segmentation-0.0.64/edu_segmentation/model.py
--rw-r--r--   0        0        0   590031 2023-04-27 10:53:24.340305 edu_segmentation-0.0.64/edu_segmentation/model_dependencies/all_vocabulary.pickle
--rw-r--r--   0        0        0    11216 2023-04-27 10:53:24.512189 edu_segmentation-0.0.64/edu_segmentation/model_dependencies/model_bart_v2.py
--rw-r--r--   0        0        0     1510 2023-04-28 12:35:01.251942 edu_segmentation-0.0.64/edu_segmentation/model_dependencies/train_segbot_bart.py
--rw-r--r--   0        0        0     2584 2023-04-28 09:07:59.951990 edu_segmentation-0.0.64/edu_segmentation/requirements.txt
--rw-r--r--   0        0        0     4364 2023-04-28 16:04:21.009998 edu_segmentation-0.0.64/edu_segmentation/run_segbot.py
--rw-r--r--   0        0        0     8583 2023-05-25 11:52:09.892681 edu_segmentation-0.0.64/edu_segmentation/run_segbot_bart.py
--rw-r--r--   0        0        0     8974 2023-04-27 10:53:24.652797 edu_segmentation-0.0.64/edu_segmentation/solver.py
--rw-r--r--   0        0        0    10912 2023-05-25 11:53:51.052894 edu_segmentation-0.0.64/edu_segmentation/solver_bart.py
--rw-r--r--   0        0        0      589 2023-05-25 11:54:16.242430 edu_segmentation-0.0.64/pyproject.toml
--rw-r--r--   0        0        0      737 2023-04-28 16:39:16.999884 edu_segmentation-0.0.64/readme.md
--rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 edu_segmentation-0.0.64/PKG-INFO
+-rw-r--r--   0        0        0     3248 2023-04-28 16:15:32.248369 edu_segmentation-0.0.65/edu_segmentation/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-27 10:53:24.371538 edu_segmentation-0.0.65/edu_segmentation/bart_tokenizer.py
+-rw-r--r--   0        0        0      671 2023-04-27 12:36:01.129982 edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc
+-rw-r--r--   0        0        0      231 2023-04-27 10:53:25.896516 edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/config.py
+-rw-r--r--   0        0        0     4321 2023-04-27 10:53:25.927765 edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/import_data_bert.py
+-rw-r--r--   0        0        0     4882 2023-04-27 10:53:25.959014 edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py
+-rw-r--r--   0        0        0     3312 2023-04-27 10:53:25.990406 edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/postagging.py
+-rw-r--r--   0        0        0     3226 2023-04-27 10:53:26.030012 edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/postagging_new.py
+-rw-r--r--   0        0        0    85404 2023-04-27 10:53:26.056731 edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/python38bert_modelling.py
+-rw-r--r--   0        0        0     6409 2023-04-27 10:53:26.103614 edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/solver.py
+-rw-r--r--   0        0        0     6978 2023-04-27 10:53:26.134865 edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/solver_postag.py
+-rw-r--r--   0        0        0      537 2023-04-27 10:53:26.166114 edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/test_model.py
+-rw-r--r--   0        0        0     1023 2023-04-27 10:53:26.197363 edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/train_model.py
+-rw-r--r--   0        0        0     1313 2023-04-27 10:53:26.228615 edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/train_model_postag.py
+-rw-r--r--   0        0        0      298 2023-04-27 10:53:24.434065 edu_segmentation-0.0.65/edu_segmentation/config.py
+-rw-r--r--   0        0        0     3930 2023-04-28 12:33:56.340151 edu_segmentation-0.0.65/edu_segmentation/import_data_bart.py
+-rw-r--r--   0        0        0        0 2023-04-27 16:13:15.942549 edu_segmentation-0.0.65/edu_segmentation/initial_dep.txt
+-rw-r--r--   0        0        0     2572 2023-04-27 16:14:15.149001 edu_segmentation-0.0.65/edu_segmentation/initial_dep_conda.txt
+-rw-r--r--   0        0        0    12186 2023-04-27 10:53:24.480926 edu_segmentation-0.0.65/edu_segmentation/model.py
+-rw-r--r--   0        0        0   590031 2023-04-27 10:53:24.340305 edu_segmentation-0.0.65/edu_segmentation/model_dependencies/all_vocabulary.pickle
+-rw-r--r--   0        0        0    11216 2023-04-27 10:53:24.512189 edu_segmentation-0.0.65/edu_segmentation/model_dependencies/model_bart_v2.py
+-rw-r--r--   0        0        0     1510 2023-04-28 12:35:01.251942 edu_segmentation-0.0.65/edu_segmentation/model_dependencies/train_segbot_bart.py
+-rw-r--r--   0        0        0     2584 2023-04-28 09:07:59.951990 edu_segmentation-0.0.65/edu_segmentation/requirements.txt
+-rw-r--r--   0        0        0     4364 2023-04-28 16:04:21.009998 edu_segmentation-0.0.65/edu_segmentation/run_segbot.py
+-rw-r--r--   0        0        0     8687 2023-05-25 12:46:03.675282 edu_segmentation-0.0.65/edu_segmentation/run_segbot_bart.py
+-rw-r--r--   0        0        0     8974 2023-04-27 10:53:24.652797 edu_segmentation-0.0.65/edu_segmentation/solver.py
+-rw-r--r--   0        0        0    10912 2023-05-25 11:53:51.052894 edu_segmentation-0.0.65/edu_segmentation/solver_bart.py
+-rw-r--r--   0        0        0      589 2023-05-25 12:49:49.299821 edu_segmentation-0.0.65/pyproject.toml
+-rw-r--r--   0        0        0      737 2023-04-28 16:39:16.999884 edu_segmentation-0.0.65/readme.md
+-rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 edu_segmentation-0.0.65/PKG-INFO
```

### Comparing `edu_segmentation-0.0.64/edu_segmentation/__init__.py` & `edu_segmentation-0.0.65/edu_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc` & `edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/import_data_bert.py` & `edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/import_data_bert.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py` & `edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/postagging.py` & `edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/postagging.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/postagging_new.py` & `edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/postagging_new.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/python38bert_modelling.py` & `edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/python38bert_modelling.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/solver.py` & `edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/solver.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/solver_postag.py` & `edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/solver_postag.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/test_model.py` & `edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/test_model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/train_model.py` & `edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/train_model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/BERTTokenClassification/train_model_postag.py` & `edu_segmentation-0.0.65/edu_segmentation/BERTTokenClassification/train_model_postag.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/import_data_bart.py` & `edu_segmentation-0.0.65/edu_segmentation/import_data_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/initial_dep_conda.txt` & `edu_segmentation-0.0.65/edu_segmentation/initial_dep_conda.txt`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/model.py` & `edu_segmentation-0.0.65/edu_segmentation/model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/model_dependencies/all_vocabulary.pickle` & `edu_segmentation-0.0.65/edu_segmentation/model_dependencies/all_vocabulary.pickle`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/model_dependencies/model_bart_v2.py` & `edu_segmentation-0.0.65/edu_segmentation/model_dependencies/model_bart_v2.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/model_dependencies/train_segbot_bart.py` & `edu_segmentation-0.0.65/edu_segmentation/model_dependencies/train_segbot_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/requirements.txt` & `edu_segmentation-0.0.65/edu_segmentation/requirements.txt`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/run_segbot.py` & `edu_segmentation-0.0.65/edu_segmentation/run_segbot.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/run_segbot_bart.py` & `edu_segmentation-0.0.65/edu_segmentation/run_segbot_bart.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,16 @@
     return all_tokens, all_masks, all_boundaries
 
 
 def get_inference(inputstring):
     """
     Load trained model and run the inference on each input sequence
     """
+    if len(inputstring)==1:
+        return  [['0,1', f'{inputstring}']]
     X_in, X_mask, Y_in = parse_input(inputstring)
     segments = []
     directory_to_look = os.path.join(
         os.path.dirname(__file__), "model_dependencies/model_segbot_bart.torchsave"
     )
     mymodel = torch.load(directory_to_look)
     mymodel.use_cuda = False
@@ -171,15 +173,15 @@
             seg = TOKENIZER.decode(X_in[i][start_b[j] : END])
             segments.append([f"{str(start_b[j])},{str(end_b[j])}", seg])
             # print(seg)
 
         # time_taken = time.time() - start_time
 
         # print("--- %s seconds ---" % (time.time() - start_time))
-
+    print('segments:', segments)
     return segments
 
 
 # if __name__ == '__main__':
 # sent="In ASEAN, there are currently government initiatives to encourage renewable energy, with Singapore predicting that hydrogen could supply up to half of the power needs in Singapore by 2050 and Thailand with a Hydrogen goal of 10 Kilotons of oil equivalent in total by 2036."
 # sent="Furthermore, the current advancements in technology for hydrogen energy is able to reduce costs in terms of production and storage of hydrogen energy. As the technology continues to improve, it is expected to further lower the cost of production, achieving economies of scale."
 # sent='Singapore recently announced that it is moving to a new Covid-19 innoculation strategy, with the focus on an individual’s vaccination being up-to-date, similar to how influenza jabs are administered seasonally. This comes as the country fights another wave of coronavirus infections, spurred by the emergence of the Omicron XBB sub-variant. '
```

### Comparing `edu_segmentation-0.0.64/edu_segmentation/solver.py` & `edu_segmentation-0.0.65/edu_segmentation/solver.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/edu_segmentation/solver_bart.py` & `edu_segmentation-0.0.65/edu_segmentation/solver_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/pyproject.toml` & `edu_segmentation-0.0.65/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edu_segmentation"
-version = "v0.0.64"
+version = "v0.0.65"
 description = "To improve EDU segmentation performance using Segbot. As Segbot has an encoder-decoder model architecture, we can replace bidirectional GRU encoder with generative pretraining models such as BART and T5. Evaluate the new model using the RST dataset by using few-shot based settings (e.g. 100 examples) to train the model, instead of using the full dataset."
 authors = ["Your Name <you@example.com>"]
 readme = "readme.md"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `edu_segmentation-0.0.64/readme.md` & `edu_segmentation-0.0.65/readme.md`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.64/PKG-INFO` & `edu_segmentation-0.0.65/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edu-segmentation
-Version: 0.0.64
+Version: 0.0.65
 Summary: To improve EDU segmentation performance using Segbot. As Segbot has an encoder-decoder model architecture, we can replace bidirectional GRU encoder with generative pretraining models such as BART and T5. Evaluate the new model using the RST dataset by using few-shot based settings (e.g. 100 examples) to train the model, instead of using the full dataset.
 Author: Your Name
 Author-email: you@example.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

