# Comparing `tmp/s2aff-0.56.tar.gz` & `tmp/s2aff-0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.56.tar", last modified: Mon May 22 23:40:33 2023, max compression
+gzip compressed data, was "s2aff-0.57.tar", last modified: Thu May 25 05:36:04 2023, max compression
```

## Comparing `s2aff-0.56.tar` & `s2aff-0.57.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 23:40:33.662602 s2aff-0.56/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.56/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-22 23:40:33.662469 s2aff-0.56/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.56/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 23:40:33.655631 s2aff-0.56/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.56/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.56/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.56/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 23:40:33.655813 s2aff-0.56/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.56/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 23:40:33.658991 s2aff-0.56/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11539 2023-05-22 22:51:54.000000 s2aff-0.56/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-16 14:48:02.000000 s2aff-0.56/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.56/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.56/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.56/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.56/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13725 2023-05-22 17:08:00.000000 s2aff-0.56/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    36032 2023-05-22 13:35:44.000000 s2aff-0.56/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.56/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 23:40:33.660340 s2aff-0.56/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.56/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.56/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.56/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 23:40:33.659794 s2aff-0.56/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-22 23:40:33.000000 s2aff-0.56/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-22 23:40:33.000000 s2aff-0.56/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-22 23:40:33.000000 s2aff-0.56/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-22 23:40:33.000000 s2aff-0.56/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-22 23:40:33.000000 s2aff-0.56/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 23:40:33.662191 s2aff-0.56/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.56/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.56/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.56/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.56/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.56/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.56/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.56/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-22 23:40:33.662650 s2aff-0.56/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-22 23:40:08.000000 s2aff-0.56/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-25 05:36:04.594043 s2aff-0.57/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.57/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-25 05:36:04.593761 s2aff-0.57/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.57/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-25 05:36:04.585375 s2aff-0.57/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.57/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.57/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.57/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-25 05:36:04.585692 s2aff-0.57/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.57/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-25 05:36:04.589559 s2aff-0.57/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    12258 2023-05-25 05:23:52.000000 s2aff-0.57/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-16 14:48:02.000000 s2aff-0.57/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.57/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.57/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.57/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.57/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13725 2023-05-22 17:08:00.000000 s2aff-0.57/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    37613 2023-05-25 03:36:35.000000 s2aff-0.57/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.57/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-25 05:36:04.591478 s2aff-0.57/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.57/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.57/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.57/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-25 05:36:04.590723 s2aff-0.57/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-25 05:36:04.000000 s2aff-0.57/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-25 05:36:04.000000 s2aff-0.57/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-25 05:36:04.000000 s2aff-0.57/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-25 05:36:04.000000 s2aff-0.57/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-25 05:36:04.000000 s2aff-0.57/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-25 05:36:04.593396 s2aff-0.57/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.57/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.57/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.57/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.57/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.57/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.57/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.57/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-25 05:36:04.594118 s2aff-0.57/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-25 05:35:26.000000 s2aff-0.57/setup.py
```

### Comparing `s2aff-0.56/LICENSE` & `s2aff-0.57/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/README.md` & `s2aff-0.57/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/data/combine_gold.py` & `s2aff-0.57/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/data/download_latest_ror.py` & `s2aff-0.57/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/s2aff/__init__.py` & `s2aff-0.57/s2aff/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         self.pairwise_model_delta_threshold = pairwise_model_delta_threshold
         self.no_ror_output_text = no_ror_output_text
         self.no_candidates_output_text = no_candidates_output_text
         self.number_of_top_candidates_to_return = number_of_top_candidates_to_return
         self.look_for_grid_and_isni = True
         set_s2aff_vars(self.ror_index, self.look_for_grid_and_isni, self.no_candidates_output_text, self.pairwise_model, self.top_k_first_stage, self.pairwise_model_threshold, self.no_ror_output_text, self.pairwise_model_delta_threshold, self.number_of_top_candidates_to_return)
 
-    def predict(self, raw_affiliations, do_reranking_multiprocessing=False, mode='gpu', ner_predictions_input=None):
+    def predict(self, raw_affiliations, do_reranking_multiprocessing=False, mode='gpu', ner_predictions_input=None, sub_ror_index=None, sub_look_for_grid_and_isni=None, sub_no_candidates_output_text=None, sub_pairwise_model=None, sub_top_k_first_stage=None, sub_pairwise_model_threshold=None, sub_no_ror_output_text=None, sub_pairwise_model_delta_threshold=None, sub_number_of_top_candidates_to_return=None):
         """Predict function for raw affiliation strings
 
         :param raw_affiliations: a list of raw affiliation strings
 
         :return: a list of dictionaries with the following keys:
             "raw_affiliation": raw affiliation string
             "ner_prediction": raw NER prediction
@@ -190,14 +190,18 @@
 
         else:
             inputs_ = []
             for counter, (raw_affiliation, ner_prediction) in enumerate(zip(raw_affiliations, ner_predictions_input)):
                 inputs_.append((counter, raw_affiliation, ner_prediction, len(raw_affiliations)))
 
             if not do_reranking_multiprocessing:
-                return [process_item(input, ror_index=ror_index, look_for_grid_and_isni=look_for_grid_and_isni, no_candidates_output_text=no_candidates_output_text, pairwise_model=pairwise_model, top_k_first_stage=top_k_first_stage, pairwise_model_threshold=pairwise_model_threshold, no_ror_output_text=no_ror_output_text, pairwise_model_delta_threshold=pairwise_model_delta_threshold, number_of_top_candidates_to_return=number_of_top_candidates_to_return) for input in inputs_]
+                return [process_item(input, ror_index=sub_ror_index, look_for_grid_and_isni=sub_look_for_grid_and_isni, no_candidates_output_text=sub_no_candidates_output_text, pairwise_model=sub_pairwise_model, top_k_first_stage=sub_top_k_first_stage, pairwise_model_threshold=sub_pairwise_model_threshold, no_ror_output_text=sub_no_ror_output_text, pairwise_model_delta_threshold=sub_pairwise_model_delta_threshold, number_of_top_candidates_to_return=sub_number_of_top_candidates_to_return) for input in inputs_]
 
-            generator = reranking_multi(inputs_, ror_index=ror_index, look_for_grid_and_isni=look_for_grid_and_isni, no_candidates_output_text=no_candidates_output_text, pairwise_model=pairwise_model, top_k_first_stage=top_k_first_stage, pairwise_model_threshold=pairwise_model_threshold, no_ror_output_text=no_ror_output_text, pairwise_model_delta_threshold=pairwise_model_delta_threshold, number_of_top_candidates_to_return=number_of_top_candidates_to_return)
+            generator = reranking_multi(inputs_, ror_index=sub_ror_index, look_for_grid_and_isni=sub_look_for_grid_and_isni, no_candidates_output_text=sub_no_candidates_output_text, pairwise_model=sub_pairwise_model, top_k_first_stage=sub_top_k_first_stage, pairwise_model_threshold=sub_pairwise_model_threshold, no_ror_output_text=sub_no_ror_output_text, pairwise_model_delta_threshold=sub_pairwise_model_delta_threshold, number_of_top_candidates_to_return=sub_number_of_top_candidates_to_return)
+            set_s2aff_vars(sub_ror_index, sub_look_for_grid_and_isni, sub_no_candidates_output_text,
+                           sub_pairwise_model, sub_top_k_first_stage, sub_pairwise_model_threshold,
+                           sub_no_ror_output_text, sub_pairwise_model_delta_threshold,
+                           sub_number_of_top_candidates_to_return)
             outputs = []
             for r in generator:
                 outputs.append(r)
             return outputs
```

### Comparing `s2aff-0.56/s2aff/consts.py` & `s2aff-0.57/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/s2aff/data.py` & `s2aff-0.57/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/s2aff/features.py` & `s2aff-0.57/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/s2aff/file_cache.py` & `s2aff-0.57/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/s2aff/lightgbm_helpers.py` & `s2aff-0.57/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/s2aff/model.py` & `s2aff-0.57/s2aff/model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/s2aff/ror.py` & `s2aff-0.57/s2aff/ror.py`

 * *Files 20% similar despite different names*

```diff
@@ -406,167 +406,168 @@
             Note that the candidates are sometimes *not* fully sorted by score because arbitrarily
             scored candidates are inserted heuristically into the list to increase recall.
         """
         if type(main) is str:
             main = [main]
         ranked_before_dfs = []
         main_fixed_all = []
-        
+        main_total_time = time.time()
+        other_times = [0]*22
         for m in main:
-            
+            this_time = time.time()
             main_fixed = [i for i in m.lower().replace(",", "").split(" ") if i not in STOPWORDS] # 1
-            
-            
+            other_times[0] = time.time()-this_time
+            this_time = time.time()
             main_fixed = " ".join([INVERTED_ABBREVIATION_DICTIONARY.get(word, word) for word in main_fixed]) # 2
-            
+            other_times[1] = time.time()-this_time
             main_fixed_all.append(main_fixed)
             if len(main_fixed) > 0:
-                
+                this_time = time.time()
                 ranked_words_before = jaccard_word_nns( # 3
                     main_fixed,
                     self.word_index,
                     idf_weight=self.idf_weight,
                     max_intersection_denominator=self.max_intersection_denominator,
                     word_multiplier=self.word_multiplier,
                     sort=False,
                 )
-                
-                
+                other_times[2] = time.time()-this_time
+                this_time = time.time()
                 ranked_ngrams_before = jaccard_ngram_nns( # 4
                     main_fixed,
                     self.ngram_index,
                     ns=self.ns,
                     idf_weight=self.idf_weight,
                     max_intersection_denominator=self.max_intersection_denominator,
                     sort=False,
                 )
-                
-                
+                other_times[3] = time.time()-this_time
+                this_time = time.time()
                 ranked_before = sum_list_of_list_of_tuples( # 5
                     [ranked_words_before, ranked_ngrams_before], use_log=self.word_multiplier == "log"
                 )
-                
+                other_times[4] = time.time()-this_time
                 if len(ranked_before) > 0:
-                    
+                    this_time = time.time()
                     ranked_before_df = pd.DataFrame(list(ranked_before.items()), columns=[0, 1]).set_index(0) # 6
-                    
+                    other_times[5] = time.time() - this_time
                     if self.word_multiplier == "log":
-                        
+                        this_time = time.time()
                         ranked_before_df = ranked_before_df[ # 7
                             ranked_before_df[1] > np.log1p(self.score_based_early_cutoff)
                         ]
-                        
+                        other_times[6] = time.time() - this_time
                     else:
-                        
+                        this_time = time.time()
                         ranked_before_df = ranked_before_df[ranked_before_df[1] > self.score_based_early_cutoff] # 8
-                        
+                        other_times[7] = time.time() - this_time
                     ranked_before_dfs.append(ranked_before_df)
         if len(ranked_before_dfs) > 0:
-            
+            this_time = time.time()
             x = pd.concat(ranked_before_dfs, axis=1).fillna(0).max(1) # 9
-            
+            other_times[8] = time.time() - this_time
         else:
             return [], []
-        
+        this_time = time.time()
         ranked_before = list(zip(x.index, x)) # 10
-        
-        
+        other_times[9] = time.time() - this_time
+        this_time = time.time()
         ranked_before = sorted(ranked_before, key=itemgetter(1), reverse=True) # 11
-        
+        other_times[10] = time.time() - this_time
 
         # we have multiple appearances of the same grid id
         # keep only the first appearance in the ranked list
         # 12
-        
+        this_time = time.time()
         ranked_unique = []
         seen_rors = set()
         for ror_id, score in ranked_before:
             ror_id = ror_id.split("__")[0]
             if ror_id not in seen_rors:
                 ranked_unique.append((ror_id, score))
                 seen_rors.add(ror_id)
-        
+        other_times[11] = time.time() - this_time
 
         # insert early candidates in position self.insert_early_candidates_ind if not seen already
         if self.insert_early_candidates_ind is not None:
-            
+            this_time = time.time()
             early_candidates_tuples = [(i, -0.1) for i in early_candidates if i not in seen_rors] # 13
-            
-            
+            other_times[12] = time.time() - this_time
+            this_time = time.time()
             ranked_unique = ( # 14
                 ranked_unique[: self.insert_early_candidates_ind]
                 + early_candidates_tuples
                 + ranked_unique[self.insert_early_candidates_ind :]
             )
-            
+            other_times[13] = time.time() - this_time
 
         if len(ranked_unique) == 0:
             return [], []
 
         # if we have address text, we can find the RORs that have at least one word in that text
         if address != "" and len(address) > 0:
             if type(address) is list:
-                
+                this_time = time.time()
                 address = " ".join(address) # 15
-                
-            
+                other_times[14] = time.time() - this_time
+            this_time = time.time()
             address_fixed_tokens = set([i for i in address.lower().replace(",", "").split(" ") if i not in STOPWORDS]) # 16
-            
+            other_times[15] = time.time() - this_time
 
             # 17
-            
+            this_time = time.time()
             inverted = self.address_index["full_index"]
             acceptable_rors = set()
             for unigram in address_fixed_tokens:
                 if unigram in inverted:
                     acceptable_rors.update(inverted[unigram])
-            
+            other_times[16] = time.time() - this_time
 
             # 18
-            
+            this_time = time.time()
             ranked_after_address_filter = [i for i in ranked_unique if i[0] in acceptable_rors]
-            
+            other_times[17] = time.time() - this_time
 
             if len(ranked_after_address_filter) == 0:
                 ranked_after_address_filter = ranked_unique
             else:
                 # reinsert top from ranked_unique that were removed, just in case the address was wrong
-                
+                this_time = time.time()
                 ranked_removed = [i for i in ranked_unique if i[0] not in acceptable_rors] # 19
-                
+                other_times[18] = time.time() - this_time
                 if len(ranked_removed) > 0:
                     # reinsert the ones that all are close to top score
                     ranked_removed_top_score = self.reinsert_cutoff_frac * ranked_after_address_filter[0][1]
                     # artificially setting the score to distinguish from "real" top
-                    
+                    this_time = time.time()
                     ranked_removed_to_reinsert = [ # 20
                         (i[0], -0.15) for i in ranked_removed if i[1] >= ranked_removed_top_score
                     ]
-                    
+                    other_times[19] = time.time() - this_time
                     if self.insert_early_candidates_ind is not None:
                         insert_ind = len(early_candidates_tuples) + self.insert_early_candidates_ind + 10
                     else:
                         insert_ind = len(early_candidates_tuples) + 10
-                    
+                    this_time = time.time()
                     ranked_after_address_filter = ( # 21
                         ranked_after_address_filter[:insert_ind]
                         + ranked_removed_to_reinsert
                         + ranked_after_address_filter[insert_ind:]
                     )
-                    
+                    other_times[20] = time.time() - this_time
         else:
             ranked_after_address_filter = ranked_unique
 
-        
+        this_time = time.time()
         candidates, scores = list(zip(*ranked_after_address_filter)) # 22
-        
+        other_times[21] = time.time() - this_time
 
-        #print("TOTAL TIME:", time.time()-main_total_time)
-        #for ind_ in range(len(other_times)):
-            #print(f"TIME FOR SECTION {ind_+1}: {other_times[ind_]}")
+        print("TOTAL TIME:", time.time()-main_total_time)
+        for ind_ in range(len(other_times)):
+            print(f"TIME FOR SECTION {ind_+1}: {other_times[ind_]}")
         return candidates, scores
 
     def parse_ror_entry_into_single_string(
         self, ror_id, use_separator_tokens=True, shuffle_names=False, special_tokens_dict=get_special_tokens_dict()
     ):
         if ror_id not in self.ror_dict:
             # assuming that this is just not a ror_id and instead a string of some affiliation
@@ -681,73 +682,73 @@
     sort=False,
 ):
 
     lengths = ngram_index["lengths_index"]
     inverted = ngram_index["inverted_index"]
 
     intersections = Counter()
-    
+    ngram_time = time.time()
     candidate_ngrams, candidate_ngram_weights = get_text_ngrams(candidate, weights_lookup_f=idf_weight, ns=ns)
-    #print("NGRAM TIME", time.time()-ngram_time)
+    print("NGRAM TIME", time.time()-ngram_time)
     # one issue is when the same ngram appears in a long affiliation string
     # many times, it ends up being overweighted
     # hack mitigation: we keep each ngram only once, but the weight
     # is its max weight
-    
-    
+    rest_of_jacc = time.time()
+    first_loop = time.time()
     candidate_ngrams_unique = set()
     ngram_largest_weight = {}
     for ngram, weight in zip(candidate_ngrams, candidate_ngram_weights):
         if ngram not in candidate_ngrams_unique:
             candidate_ngrams_unique.add(ngram)
             ngram_largest_weight[ngram] = np.maximum(weight, ngram_largest_weight.get(ngram, 0))
-    #print("FIRST LOOP TIME:", time.time()-first_loop)
+    print("FIRST LOOP TIME:", time.time()-first_loop)
 
-    #print(len(inverted), len(candidate_ngrams_unique), len(lengths), len(candidate_ngrams))
-    
+    print(len(inverted), len(candidate_ngrams_unique), len(lengths), len(candidate_ngrams))
+    second_loop = time.time()
     intersections = defaultdict(float)
     weights_in_inverted = 0
     candidate_ngrams_in_inverted = []
     for ng, inverted_ng in ((ng, inverted.get(ng)) for ng in candidate_ngrams_unique):
         if inverted_ng is not None:
             weight = ngram_largest_weight.get(ng, 0)
             for ror_id in inverted_ng:
                 intersections[ror_id] += weight
             weights_in_inverted += weight
-    #print("SECOND LOOP TIME:", time.time()-second_loop)
+    print("SECOND LOOP TIME:", time.time()-second_loop)
 
     if idf_weight is not None:
-        
+        sum_time = time.time()
         num_candidate_ngrams = np.sum(candidate_ngram_weights)
         num_relevant_candidate_ngrams = weights_in_inverted
-        #print("SUM TIME:", time.time()-sum_time)
+        print("SUM TIME:", time.time()-sum_time)
     else:
-        #print("UH OH!!")
+        print("UH OH!!")
         num_candidate_ngrams = len(candidate_ngrams)
         num_relevant_candidate_ngrams = len(candidate_ngrams_in_inverted)
 
-    
+    jaccards_time = time.time()
     if max_intersection_denominator:
-        #print("IF RAN")
+        print("IF RAN")
         jaccards = [
             (grid, intersection / (num_relevant_candidate_ngrams + lengths[grid] - intersection))
             for grid, intersection in intersections.items()
         ]
     else:
-        #print("ELSE RAN")
+        print("ELSE RAN")
         jaccards = [
             (grid, intersection / (num_candidate_ngrams + lengths[grid] - intersection))
             for grid, intersection in intersections.items()
         ]
 
-    #print("JACCARDS BUILD TIME", time.time()-jaccards_time)
+    print("JACCARDS BUILD TIME", time.time()-jaccards_time)
     if sort:
         jaccards = sorted(jaccards, key=itemgetter(1), reverse=True)
 
-    #print("REST OF JACCARD", time.time()-rest_of_jacc)
+    print("REST OF JACCARD", time.time()-rest_of_jacc)
     return jaccards
 
 
 def jaccard_word_nns(
     candidate,
     word_index,
     idf_weight=None,
```

### Comparing `s2aff-0.56/s2aff/text.py` & `s2aff-0.57/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/s2aff/timo/integration_test.py` & `s2aff-0.57/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/s2aff/timo/interface.py` & `s2aff-0.57/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/s2aff.egg-info/SOURCES.txt` & `s2aff-0.57/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.57/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.57/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/scripts/generate_lightgbm_training_data.py` & `s2aff-0.57/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/scripts/train_lightgbm_reranker.py` & `s2aff-0.57/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/scripts/train_ner_model.py` & `s2aff-0.57/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/scripts/update_openalex_works_counts.py` & `s2aff-0.57/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.56/setup.py` & `s2aff-0.57/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.56",
+    version="0.57",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

