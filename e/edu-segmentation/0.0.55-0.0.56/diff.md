# Comparing `tmp/edu_segmentation-0.0.55.tar.gz` & `tmp/edu_segmentation-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edu_segmentation-0.0.55.tar", max compression
+gzip compressed data, was "edu_segmentation-0.0.56.tar", max compression
```

## Comparing `edu_segmentation-0.0.55.tar` & `edu_segmentation-0.0.56.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     3248 2023-04-28 16:15:32.248369 edu_segmentation-0.0.55/edu_segmentation/__init__.py
--rw-r--r--   0        0        0      325 2023-04-27 10:53:24.371538 edu_segmentation-0.0.55/edu_segmentation/bart_tokenizer.py
--rw-r--r--   0        0        0      671 2023-04-27 12:36:01.129982 edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc
--rw-r--r--   0        0        0      231 2023-04-27 10:53:25.896516 edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/config.py
--rw-r--r--   0        0        0     4321 2023-04-27 10:53:25.927765 edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/import_data_bert.py
--rw-r--r--   0        0        0     4882 2023-04-27 10:53:25.959014 edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py
--rw-r--r--   0        0        0     3312 2023-04-27 10:53:25.990406 edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/postagging.py
--rw-r--r--   0        0        0     3226 2023-04-27 10:53:26.030012 edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/postagging_new.py
--rw-r--r--   0        0        0    85404 2023-04-27 10:53:26.056731 edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/python38bert_modelling.py
--rw-r--r--   0        0        0     6409 2023-04-27 10:53:26.103614 edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/solver.py
--rw-r--r--   0        0        0     6978 2023-04-27 10:53:26.134865 edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/solver_postag.py
--rw-r--r--   0        0        0      537 2023-04-27 10:53:26.166114 edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/test_model.py
--rw-r--r--   0        0        0     1023 2023-04-27 10:53:26.197363 edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/train_model.py
--rw-r--r--   0        0        0     1313 2023-04-27 10:53:26.228615 edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/train_model_postag.py
--rw-r--r--   0        0        0      298 2023-04-27 10:53:24.434065 edu_segmentation-0.0.55/edu_segmentation/config.py
--rw-r--r--   0        0        0     3930 2023-04-28 12:33:56.340151 edu_segmentation-0.0.55/edu_segmentation/import_data_bart.py
--rw-r--r--   0        0        0        0 2023-04-27 16:13:15.942549 edu_segmentation-0.0.55/edu_segmentation/initial_dep.txt
--rw-r--r--   0        0        0     2572 2023-04-27 16:14:15.149001 edu_segmentation-0.0.55/edu_segmentation/initial_dep_conda.txt
--rw-r--r--   0        0        0    12186 2023-04-27 10:53:24.480926 edu_segmentation-0.0.55/edu_segmentation/model.py
--rw-r--r--   0        0        0   590031 2023-04-27 10:53:24.340305 edu_segmentation-0.0.55/edu_segmentation/model_dependencies/all_vocabulary.pickle
--rw-r--r--   0        0        0    11216 2023-04-27 10:53:24.512189 edu_segmentation-0.0.55/edu_segmentation/model_dependencies/model_bart_v2.py
--rw-r--r--   0        0        0     1510 2023-04-28 12:35:01.251942 edu_segmentation-0.0.55/edu_segmentation/model_dependencies/train_segbot_bart.py
--rw-r--r--   0        0        0     2584 2023-04-28 09:07:59.951990 edu_segmentation-0.0.55/edu_segmentation/requirements.txt
--rw-r--r--   0        0        0     4364 2023-04-28 16:04:21.009998 edu_segmentation-0.0.55/edu_segmentation/run_segbot.py
--rw-r--r--   0        0        0     7227 2023-04-28 15:36:38.336217 edu_segmentation-0.0.55/edu_segmentation/run_segbot_bart.py
--rw-r--r--   0        0        0     8974 2023-04-27 10:53:24.652797 edu_segmentation-0.0.55/edu_segmentation/solver.py
--rw-r--r--   0        0        0     9549 2023-04-27 10:53:24.694580 edu_segmentation-0.0.55/edu_segmentation/solver_bart.py
--rw-r--r--   0        0        0      589 2023-04-28 16:41:26.502975 edu_segmentation-0.0.55/pyproject.toml
--rw-r--r--   0        0        0      737 2023-04-28 16:39:16.999884 edu_segmentation-0.0.55/readme.md
--rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 edu_segmentation-0.0.55/PKG-INFO
+-rw-r--r--   0        0        0     3248 2023-04-28 16:15:32.248369 edu_segmentation-0.0.56/edu_segmentation/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-27 10:53:24.371538 edu_segmentation-0.0.56/edu_segmentation/bart_tokenizer.py
+-rw-r--r--   0        0        0      671 2023-04-27 12:36:01.129982 edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc
+-rw-r--r--   0        0        0      231 2023-04-27 10:53:25.896516 edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/config.py
+-rw-r--r--   0        0        0     4321 2023-04-27 10:53:25.927765 edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/import_data_bert.py
+-rw-r--r--   0        0        0     4882 2023-04-27 10:53:25.959014 edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py
+-rw-r--r--   0        0        0     3312 2023-04-27 10:53:25.990406 edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/postagging.py
+-rw-r--r--   0        0        0     3226 2023-04-27 10:53:26.030012 edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/postagging_new.py
+-rw-r--r--   0        0        0    85404 2023-04-27 10:53:26.056731 edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/python38bert_modelling.py
+-rw-r--r--   0        0        0     6409 2023-04-27 10:53:26.103614 edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/solver.py
+-rw-r--r--   0        0        0     6978 2023-04-27 10:53:26.134865 edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/solver_postag.py
+-rw-r--r--   0        0        0      537 2023-04-27 10:53:26.166114 edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/test_model.py
+-rw-r--r--   0        0        0     1023 2023-04-27 10:53:26.197363 edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/train_model.py
+-rw-r--r--   0        0        0     1313 2023-04-27 10:53:26.228615 edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/train_model_postag.py
+-rw-r--r--   0        0        0      298 2023-04-27 10:53:24.434065 edu_segmentation-0.0.56/edu_segmentation/config.py
+-rw-r--r--   0        0        0     3930 2023-04-28 12:33:56.340151 edu_segmentation-0.0.56/edu_segmentation/import_data_bart.py
+-rw-r--r--   0        0        0        0 2023-04-27 16:13:15.942549 edu_segmentation-0.0.56/edu_segmentation/initial_dep.txt
+-rw-r--r--   0        0        0     2572 2023-04-27 16:14:15.149001 edu_segmentation-0.0.56/edu_segmentation/initial_dep_conda.txt
+-rw-r--r--   0        0        0    12186 2023-04-27 10:53:24.480926 edu_segmentation-0.0.56/edu_segmentation/model.py
+-rw-r--r--   0        0        0   590031 2023-04-27 10:53:24.340305 edu_segmentation-0.0.56/edu_segmentation/model_dependencies/all_vocabulary.pickle
+-rw-r--r--   0        0        0    11216 2023-04-27 10:53:24.512189 edu_segmentation-0.0.56/edu_segmentation/model_dependencies/model_bart_v2.py
+-rw-r--r--   0        0        0     1510 2023-04-28 12:35:01.251942 edu_segmentation-0.0.56/edu_segmentation/model_dependencies/train_segbot_bart.py
+-rw-r--r--   0        0        0     2584 2023-04-28 09:07:59.951990 edu_segmentation-0.0.56/edu_segmentation/requirements.txt
+-rw-r--r--   0        0        0     4364 2023-04-28 16:04:21.009998 edu_segmentation-0.0.56/edu_segmentation/run_segbot.py
+-rw-r--r--   0        0        0     7965 2023-05-25 09:03:16.858967 edu_segmentation-0.0.56/edu_segmentation/run_segbot_bart.py
+-rw-r--r--   0        0        0     8974 2023-04-27 10:53:24.652797 edu_segmentation-0.0.56/edu_segmentation/solver.py
+-rw-r--r--   0        0        0     9549 2023-04-27 10:53:24.694580 edu_segmentation-0.0.56/edu_segmentation/solver_bart.py
+-rw-r--r--   0        0        0      589 2023-05-25 09:10:29.731645 edu_segmentation-0.0.56/pyproject.toml
+-rw-r--r--   0        0        0      737 2023-04-28 16:39:16.999884 edu_segmentation-0.0.56/readme.md
+-rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 edu_segmentation-0.0.56/PKG-INFO
```

### Comparing `edu_segmentation-0.0.55/edu_segmentation/__init__.py` & `edu_segmentation-0.0.56/edu_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc` & `edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/import_data_bert.py` & `edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/import_data_bert.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py` & `edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/postagging.py` & `edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/postagging.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/postagging_new.py` & `edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/postagging_new.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/python38bert_modelling.py` & `edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/python38bert_modelling.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/solver.py` & `edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/solver.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/solver_postag.py` & `edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/solver_postag.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/test_model.py` & `edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/test_model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/train_model.py` & `edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/train_model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/BERTTokenClassification/train_model_postag.py` & `edu_segmentation-0.0.56/edu_segmentation/BERTTokenClassification/train_model_postag.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/import_data_bart.py` & `edu_segmentation-0.0.56/edu_segmentation/import_data_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/initial_dep_conda.txt` & `edu_segmentation-0.0.56/edu_segmentation/initial_dep_conda.txt`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/model.py` & `edu_segmentation-0.0.56/edu_segmentation/model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/model_dependencies/all_vocabulary.pickle` & `edu_segmentation-0.0.56/edu_segmentation/model_dependencies/all_vocabulary.pickle`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/model_dependencies/model_bart_v2.py` & `edu_segmentation-0.0.56/edu_segmentation/model_dependencies/model_bart_v2.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/model_dependencies/train_segbot_bart.py` & `edu_segmentation-0.0.56/edu_segmentation/model_dependencies/train_segbot_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/requirements.txt` & `edu_segmentation-0.0.56/edu_segmentation/requirements.txt`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/run_segbot.py` & `edu_segmentation-0.0.56/edu_segmentation/run_segbot.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/run_segbot_bart.py` & `edu_segmentation-0.0.56/edu_segmentation/run_segbot_bart.py`

 * *Files 5% similar despite different names*

```diff
@@ -159,25 +159,40 @@
 
 # if __name__ == '__main__':
     #sent="In ASEAN, there are currently government initiatives to encourage renewable energy, with Singapore predicting that hydrogen could supply up to half of the power needs in Singapore by 2050 and Thailand with a Hydrogen goal of 10 Kilotons of oil equivalent in total by 2036."
     #sent="Furthermore, the current advancements in technology for hydrogen energy is able to reduce costs in terms of production and storage of hydrogen energy. As the technology continues to improve, it is expected to further lower the cost of production, achieving economies of scale."
     #sent='Singapore recently announced that it is moving to a new Covid-19 innoculation strategy, with the focus on an individual’s vaccination being up-to-date, similar to how influenza jabs are administered seasonally. This comes as the country fights another wave of coronavirus infections, spurred by the emergence of the Omicron XBB sub-variant. '
     #     sent="Aerial warfare has been around for much longer than modern aircraft have. More than 1,000 years ago, armies in China used incendiary kites known as fire crows to rain fire and debris upon their enemies. Since then, everything from kites to hot air balloons and airplanes have been used to inflict damage from above."
 
-def run_segbot_bart():
+def run_segbot_bart(sent, granularity_level):
+    results = []
+    if granularity_level == "conjunction_words":
+        conjunctions = r"\b(and|but|or|nor|for|yet|so|although|because|since|unless|until|while|if|whether|after|before|when|as|as if|as long as|as soon as|as though|even if|even though|provided that|in order that|now that|once|so that|that|unless|whenever|where|wherever|whereas|while)\b"
+        splits = re.split(conjunctions, sent, flags=re.IGNORECASE)
+        splits = [s.strip() for s in splits if s.strip()]
+        for words_str in splits:
+            results.append(core_run_segbot_bart(words_str))
+    else:
+        results.append(core_run_segbot_bart(sent))
+    return results
+
+
+def core_run_segbot_bart(sent):
+
     print("----------- EDU Segmentation with Segbot with BART model: ----------")
-    sent = input("Enter text for EDU segmentation: \n")
+    # sent = input("Enter text for EDU segmentation: \n")
     sent = sent.replace(", ",  " , ").replace(". ",  " . ").replace(
         "; ",  " ; ")
     if sent[-1] == ".":
         sent = sent[:-1] + " ."
     print("\n")
     # print("---------- Start of EDU segmentation ----------")
     output_seg = get_inference(sent)
-    print("EDU Segmentation Results:\n", output_seg)
+    return output_seg
+    # print("EDU Segmentation Results:\n", output_seg)
     # print("---------- End of EDU segmentation ----------\n")
 
     '''
     Get inference time by each new line of input
     '''
     # all_files = os.listdir(TEST_PATH)
     # total = 0
```

### Comparing `edu_segmentation-0.0.55/edu_segmentation/solver.py` & `edu_segmentation-0.0.56/edu_segmentation/solver.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/edu_segmentation/solver_bart.py` & `edu_segmentation-0.0.56/edu_segmentation/solver_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/pyproject.toml` & `edu_segmentation-0.0.56/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edu_segmentation"
-version = "v0.0.55"
+version = "v0.0.56"
 description = "To improve EDU segmentation performance using Segbot. As Segbot has an encoder-decoder model architecture, we can replace bidirectional GRU encoder with generative pretraining models such as BART and T5. Evaluate the new model using the RST dataset by using few-shot based settings (e.g. 100 examples) to train the model, instead of using the full dataset."
 authors = ["Your Name <you@example.com>"]
 readme = "readme.md"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `edu_segmentation-0.0.55/readme.md` & `edu_segmentation-0.0.56/readme.md`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.55/PKG-INFO` & `edu_segmentation-0.0.56/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edu-segmentation
-Version: 0.0.55
+Version: 0.0.56
 Summary: To improve EDU segmentation performance using Segbot. As Segbot has an encoder-decoder model architecture, we can replace bidirectional GRU encoder with generative pretraining models such as BART and T5. Evaluate the new model using the RST dataset by using few-shot based settings (e.g. 100 examples) to train the model, instead of using the full dataset.
 Author: Your Name
 Author-email: you@example.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

