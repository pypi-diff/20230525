# Comparing `tmp/selfcheckgpt-0.1.2.tar.gz` & `tmp/selfcheckgpt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfcheckgpt-0.1.2.tar", last modified: Thu Mar 23 23:31:42 2023, max compression
+gzip compressed data, was "selfcheckgpt-0.1.3.tar", last modified: Thu May 25 14:47:15 2023, max compression
```

## Comparing `selfcheckgpt-0.1.2.tar` & `selfcheckgpt-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwsr-x   0 pm574    (44166) pm574    (44167)        0 2023-03-23 23:31:42.000000 selfcheckgpt-0.1.2/
--rw-rw-r--   0 pm574    (44166) pm574    (44167)     1426 2023-03-23 22:46:15.000000 selfcheckgpt-0.1.2/DESCRIPTION.txt
--rw-rw-r--   0 pm574    (44166) pm574    (44167)     1073 2023-03-22 00:15:36.000000 selfcheckgpt-0.1.2/LICENSE
--rw-rw-r--   0 pm574    (44166) pm574    (44167)       40 2023-03-22 15:18:29.000000 selfcheckgpt-0.1.2/MANIFEST.in
--rw-rw-r--   0 pm574    (44166) pm574    (44167)     2001 2023-03-23 23:31:42.000000 selfcheckgpt-0.1.2/PKG-INFO
--rw-rw-r--   0 pm574    (44166) pm574    (44167)     3351 2023-03-23 22:55:51.000000 selfcheckgpt-0.1.2/README.md
-drwxrwsr-x   0 pm574    (44166) pm574    (44167)        0 2023-03-23 23:31:42.000000 selfcheckgpt-0.1.2/selfcheckgpt/
--rw-rw-r--   0 pm574    (44166) pm574    (44167)       45 2023-03-23 20:55:46.000000 selfcheckgpt-0.1.2/selfcheckgpt/__init__.py
--rw-rw-r--   0 pm574    (44166) pm574    (44167)    13420 2023-03-23 21:47:27.000000 selfcheckgpt-0.1.2/selfcheckgpt/modeling_mqag.py
--rw-rw-r--   0 pm574    (44166) pm574    (44167)    11042 2023-03-23 21:03:01.000000 selfcheckgpt-0.1.2/selfcheckgpt/modeling_selfcheck.py
--rw-rw-r--   0 pm574    (44166) pm574    (44167)     3349 2023-03-23 20:58:52.000000 selfcheckgpt-0.1.2/selfcheckgpt/utils.py
--rw-rw-r--   0 pm574    (44166) pm574    (44167)       22 2023-03-23 22:56:07.000000 selfcheckgpt-0.1.2/selfcheckgpt/version.py
-drwxrwsr-x   0 pm574    (44166) pm574    (44167)        0 2023-03-23 23:31:42.000000 selfcheckgpt-0.1.2/selfcheckgpt.egg-info/
--rw-rw-r--   0 pm574    (44166) pm574    (44167)     2001 2023-03-23 23:31:42.000000 selfcheckgpt-0.1.2/selfcheckgpt.egg-info/PKG-INFO
--rw-rw-r--   0 pm574    (44166) pm574    (44167)      369 2023-03-23 23:31:42.000000 selfcheckgpt-0.1.2/selfcheckgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 pm574    (44166) pm574    (44167)        1 2023-03-23 23:31:42.000000 selfcheckgpt-0.1.2/selfcheckgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 pm574    (44166) pm574    (44167)       56 2023-03-23 23:31:42.000000 selfcheckgpt-0.1.2/selfcheckgpt.egg-info/requires.txt
--rw-rw-r--   0 pm574    (44166) pm574    (44167)       13 2023-03-23 23:31:42.000000 selfcheckgpt-0.1.2/selfcheckgpt.egg-info/top_level.txt
--rw-rw-r--   0 pm574    (44166) pm574    (44167)       38 2023-03-23 23:31:42.000000 selfcheckgpt-0.1.2/setup.cfg
--rw-rw-r--   0 pm574    (44166) pm574    (44167)     1152 2023-03-23 20:56:37.000000 selfcheckgpt-0.1.2/setup.py
+drwxrwsr-x   0 pm574    (44166) pm574    (44167)        0 2023-05-25 14:47:15.000000 selfcheckgpt-0.1.3/
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)     1426 2023-03-23 22:46:15.000000 selfcheckgpt-0.1.3/DESCRIPTION.txt
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)     1073 2023-03-22 00:15:36.000000 selfcheckgpt-0.1.3/LICENSE
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)       40 2023-03-22 15:18:29.000000 selfcheckgpt-0.1.3/MANIFEST.in
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)     2001 2023-05-25 14:47:15.000000 selfcheckgpt-0.1.3/PKG-INFO
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)     6232 2023-05-25 14:17:07.000000 selfcheckgpt-0.1.3/README.md
+drwxrwsr-x   0 pm574    (44166) pm574    (44167)        0 2023-05-25 14:47:14.000000 selfcheckgpt-0.1.3/selfcheckgpt/
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)       45 2023-03-23 20:55:46.000000 selfcheckgpt-0.1.3/selfcheckgpt/__init__.py
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)    13292 2023-03-27 14:34:54.000000 selfcheckgpt-0.1.3/selfcheckgpt/modeling_mqag.py
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)     6285 2023-05-25 14:31:33.000000 selfcheckgpt-0.1.3/selfcheckgpt/modeling_ngram.py
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)    12130 2023-05-25 14:17:07.000000 selfcheckgpt-0.1.3/selfcheckgpt/modeling_selfcheck.py
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)     3317 2023-03-27 14:34:54.000000 selfcheckgpt-0.1.3/selfcheckgpt/utils.py
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)       22 2023-03-30 22:06:16.000000 selfcheckgpt-0.1.3/selfcheckgpt/version.py
+drwxrwsr-x   0 pm574    (44166) pm574    (44167)        0 2023-05-25 14:47:15.000000 selfcheckgpt-0.1.3/selfcheckgpt.egg-info/
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)     2001 2023-05-25 14:47:14.000000 selfcheckgpt-0.1.3/selfcheckgpt.egg-info/PKG-INFO
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)      400 2023-05-25 14:47:14.000000 selfcheckgpt-0.1.3/selfcheckgpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)        1 2023-05-25 14:47:14.000000 selfcheckgpt-0.1.3/selfcheckgpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)       61 2023-05-25 14:47:14.000000 selfcheckgpt-0.1.3/selfcheckgpt.egg-info/requires.txt
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)       13 2023-05-25 14:47:14.000000 selfcheckgpt-0.1.3/selfcheckgpt.egg-info/top_level.txt
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)       38 2023-05-25 14:47:15.000000 selfcheckgpt-0.1.3/setup.cfg
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)     1164 2023-03-30 22:05:51.000000 selfcheckgpt-0.1.3/setup.py
```

### Comparing `selfcheckgpt-0.1.2/DESCRIPTION.txt` & `selfcheckgpt-0.1.3/DESCRIPTION.txt`

 * *Files identical despite different names*

### Comparing `selfcheckgpt-0.1.2/LICENSE` & `selfcheckgpt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `selfcheckgpt-0.1.2/PKG-INFO` & `selfcheckgpt-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcheckgpt
-Version: 0.1.2
+Version: 0.1.3
 Summary: SelfCheckGPT: Assessing text-based responses from LLMs
 Home-page: https://github.com/potsawee/selfcheckgpt
 Author: Potsawee Manakul
 Author-email: m.potsawee@gmail.com
 License: MIT
 Keywords: selfcheckgpt
 Platform: UNKNOWN
```

### Comparing `selfcheckgpt-0.1.2/selfcheckgpt/modeling_mqag.py` & `selfcheckgpt-0.1.3/selfcheckgpt/modeling_mqag.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from transformers import LongformerTokenizer, LongformerForMultipleChoice
 from selfcheckgpt.utils import prepare_qa_input, prepare_distractor_input, prepare_answering_input
 from selfcheckgpt.utils import MQAGConfig, get_prob_distances
 
 # ---------------------------------------------------------------------------------------- #
 # Functions for Question Generation & Answering
 def question_generation_sentence_level(
-        g1_model,
-        g1_tokenizer,
-        g2_model,
-        g2_tokenizer,
-        sentence,
-        passage,
-        num_questions_per_sent,
-        device,
+    g1_model,
+    g1_tokenizer,
+    g2_model,
+    g2_tokenizer,
+    sentence,
+    passage,
+    num_questions_per_sent,
+    device,
 ):
     qa_input_ids = prepare_qa_input(
             g1_tokenizer,
             context=sentence,
             device=device,
     )
     num_valid_questions = 0
@@ -73,21 +73,21 @@
             'options': options,
         }
         questions.append(question_item)
     return questions
 
 
 def question_generation_sampling(
-        g1_model,
-        g1_tokenizer,
-        g2_model,
-        g2_tokenizer,
-        context,
-        num_questions,
-        device,
+    g1_model,
+    g1_tokenizer,
+    g2_model,
+    g2_tokenizer,
+    context,
+    num_questions,
+    device,
 ):
     qa_input_ids = prepare_qa_input(
             g1_tokenizer,
             context=context,
             device=device,
     )
     max_repeated_sampling = int(num_questions * 1.5) # sometimes generated question+answer is invalid
@@ -140,26 +140,26 @@
         }
         questions.append(question_item)
         if num_valid_questions == num_questions:
             break
     return questions
 
 def question_generation_beamsearch(
-        g1_model,
-        g1_tokenizer,
-        g2_model,
-        g2_tokenizer,
-        context,
-        num_beams,
-        device,
+    g1_model,
+    g1_tokenizer,
+    g2_model,
+    g2_tokenizer,
+    context,
+    num_beams,
+    device,
 ):
     qa_input_ids = prepare_qa_input(
-            g1_tokenizer,
-            context=context,
-            device=device,
+        g1_tokenizer,
+        context=context,
+        device=device,
     )
     # Stage G.1: question+answer generation
     outputs = g1_model.generate(
         qa_input_ids,
         max_new_tokens=128,
         do_sample=False,
         num_beams=num_beams,
@@ -202,21 +202,21 @@
         'question': question,
         'options': options,
     }
     return [question_item]
 
 
 def answering(
-        a_model,
-        a_tokenizer,
-        question,
-        options,
-        context,
-        max_seq_length,
-        device,
+    a_model,
+    a_tokenizer,
+    question,
+    options,
+    context,
+    max_seq_length,
+    device,
 ):
     answering_given_passage = prepare_answering_input(
         tokenizer=a_tokenizer,
         question=question,
         options=options,
         context=context,
         device=device,
```

### Comparing `selfcheckgpt-0.1.2/selfcheckgpt/modeling_selfcheck.py` & `selfcheckgpt-0.1.3/selfcheckgpt/modeling_selfcheck.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 from transformers import logging
 logging.set_verbosity_error()
 
 from transformers import AutoTokenizer, AutoModelForSeq2SeqLM
 from transformers import LongformerTokenizer, LongformerForMultipleChoice, LongformerForSequenceClassification
 from selfcheckgpt.utils import MQAGConfig, expand_list1, expand_list2
 from selfcheckgpt.modeling_mqag import question_generation_sentence_level, answering
+from selfcheckgpt.modeling_ngram import UnigramModel, NgramModel
 
 # ---------------------------------------------------------------------------------------- #
 # Functions for counting
 def method_simple_counting(
-        prob,
-        u_score,
-        prob_s,
-        u_score_s,
-        num_samples,
-        AT,
+    prob,
+    u_score,
+    prob_s,
+    u_score_s,
+    num_samples,
+    AT,
 ):
     """
     simple counting method score => count_mismatch / (count_match + count_mismatch)
     :return score: 'inconsistency' score
     """
     # bad questions, i.e. not answerable given the passage
     if u_score < AT:
@@ -39,20 +40,20 @@
     if count_good_sample == 0:
         score = 0.5
     else:
         score = (count_good_sample-count_match) / count_good_sample
     return score
 
 def method_vanilla_bayes(
-        prob,
-        u_score,
-        prob_s,
-        u_score_s,
-        num_samples,
-        beta1, beta2, AT,
+    prob,
+    u_score,
+    prob_s,
+    u_score_s,
+    num_samples,
+    beta1, beta2, AT,
 ):
     """
     (vanilla) bayes method score: compute P(sentence is non-factual | count_match, count_mismatch)
     :return score: 'inconsistency' score
     """
     if u_score < AT:
         return 0.5
@@ -67,20 +68,20 @@
                 count_mismatch += 1
     gamma1 = beta2 / (1.0-beta1)
     gamma2 = beta1 / (1.0-beta2)
     score = (gamma2**count_mismatch) / ((gamma1**count_match) + (gamma2**count_mismatch))
     return score
 
 def method_bayes_with_alpha(
-        prob,
-        u_score,
-        prob_s,
-        u_score_s,
-        num_samples,
-        beta1, beta2,
+    prob,
+    u_score,
+    prob_s,
+    u_score_s,
+    num_samples,
+    beta1, beta2,
 ):
     """
     bayes method (with answerability score, i.e. soft-counting) score
     :return score: 'inconsistency' score
     """
     a_DT = np.argmax(prob)
     count_match, count_mismatch = 0, 0
@@ -93,20 +94,20 @@
             count_mismatch += ans_score
     gamma1 = beta2 / (1.0-beta1)
     gamma2 = beta1 / (1.0-beta2)
     score = (gamma2**count_mismatch) / ((gamma1**count_match) + (gamma2**count_mismatch))
     return score
 
 def answerability_scoring(
-        u_model,
-        u_tokenizer,
-        question,
-        context,
-        max_length,
-        device,
+    u_model,
+    u_tokenizer,
+    question,
+    context,
+    max_length,
+    device,
 ):
     """
     :return prob: prob -> 0.0 means unanswerable, prob -> 1.0 means answerable
     """
     input_text = question + ' ' + u_tokenizer.sep_token + ' ' + context
     inputs = u_tokenizer(input_text, max_length=max_length, truncation=True, return_tensors="pt")
     inputs = inputs.to(device)
@@ -159,21 +160,21 @@
         self.a_model.to(device)
         self.u_model.to(device)
         self.device = device
         print("SelfCheck-MQAG initialized to device", device)
 
     @torch.no_grad()
     def predict(
-            self,
-            sentences: List[str],
-            passage: str,
-            sampled_passages: List[str],
-            num_questions_per_sent: int = 5,
-            scoring_method: str = "bayes_with_alpha",
-            **kwargs,
+        self,
+        sentences: List[str],
+        passage: str,
+        sampled_passages: List[str],
+        num_questions_per_sent: int = 5,
+        scoring_method: str = "bayes_with_alpha",
+        **kwargs,
     ):
         """
         This function takes sentences (to be evaluated) with sampled passages (evidence), and return sent-level scores
         :param sentences: list[str] -- sentences to be evaluated, e.g. GPT text response spilt by spacy
         :param passage: str -- the passage to be evaluated, note that splitting(passage) ---> sentences
         :param sampled_passages: list[str] -- stochastically generated responses (without sentence splitting)
         :param num_questions_per_sent: int -- number of quetions to be generated per sentence
@@ -240,17 +241,17 @@
     def __init__(self, default_model="en"):
         self.nlp = spacy.load("en_core_web_sm")
         self.default_model = default_model # en => roberta-large
         print("SelfCheck-BERTScore initialized")
 
     @torch.no_grad()
     def predict(
-            self,
-            sentences: List[str],
-            sampled_passages: List[str],
+        self,
+        sentences: List[str],
+        sampled_passages: List[str],
     ):
         """
         This function takes sentences (to be evaluated) with sampled passages (evidence), and return sent-level scores
         :param sentences: list[str] -- sentences to be evaluated, e.g. GPT text response spilt by spacy
         :param sampled_passages: list[str] -- stochastically generated responses (without sentence splitting)
         :return sent_scores: sentence-level score which is 1.0 - bertscore
         """
@@ -272,7 +273,40 @@
             F1_arr_max_axis1 = F1_arr_max_axis1.numpy()
 
             bertscore_array[:,s] = F1_arr_max_axis1
 
         bertscore_mean_per_sent = bertscore_array.mean(axis=-1)
         one_minus_bertscore_mean_per_sent = 1.0 - bertscore_mean_per_sent
         return one_minus_bertscore_mean_per_sent
+
+class SelfCheckNgram:
+    """
+    SelfCheckGPT (Ngram variant): Checking LLM's text against its own sampled texts via ngram model
+    Note that this variant of SelfCheck score is not bounded in [0.0, 1.0]
+    """
+    def __init__(self, n: int, lowercase: bool = True):
+        """
+        :param n: n-gram model, n=1 is Unigram, n=2 is Bigram, etc.
+        :param lowercase: whether or not to lowercase when counting n-grams
+        """
+        self.n = n
+        self.lowercase = lowercase
+        print(f"SelfCheck-{n}gram initialized")
+
+    def predict(
+        self,
+        sentences: List[str],
+        passage: str,
+        sampled_passages: List[str],
+    ):
+        if self.n == 1:
+            ngram_model = UnigramModel(lowercase=self.lowercase)
+        elif self.n > 1:
+            ngram_model = NgramModel(n=self.n, lowercase=self.lowercase)
+        else:
+            raise ValueError("n must be integer >= 1")
+        ngram_model.add(passage)
+        for sampled_passge in sampled_passages:
+            ngram_model.add(sampled_passge)
+        ngram_model.train(k=0)
+        ngram_pred = ngram_model.evaluate(sentences)
+        return ngram_pred
```

### Comparing `selfcheckgpt-0.1.2/selfcheckgpt/utils.py` & `selfcheckgpt-0.1.3/selfcheckgpt/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,44 +6,44 @@
     generation2: str = "potsawee/t5-large-generation-race-Distractor"
     answering: str = "potsawee/longformer-large-4096-answering-race"
     answerability: str = "potsawee/longformer-large-4096-answerable-squad2"
 
 # Question Generation & Answering Input Processing
 def prepare_qa_input(t5_tokenizer, context, device):
     """
-        input: context
-        output: question <sep> answer
+    input: context
+    output: question <sep> answer
     """
     encoding = t5_tokenizer(
         [context],
         return_tensors="pt",
     )
     input_ids = encoding.input_ids.to(device)
     return input_ids
 
 
 def prepare_distractor_input(t5_tokenizer, context, question, answer, device, separator='<sep>'):
     """
-        input: question <sep> answer <sep> article
-        output: distractor1 <sep> distractor2 <sep> distractor3
+    input: question <sep> answer <sep> article
+    output: distractor1 <sep> distractor2 <sep> distractor3
     """
     input_text = question + ' ' + separator + ' ' + answer + ' ' + separator + ' ' + context
     encoding = t5_tokenizer(
         [input_text],
         return_tensors="pt",
     )
     input_ids = encoding.input_ids.to(device)
     return input_ids
 
 
 def prepare_answering_input(
-        tokenizer, # longformer_tokenizer
-        question, options, context,
-        device, max_seq_length=4096,
-    ):
+    tokenizer, # longformer_tokenizer
+    question, options, context,
+    device, max_seq_length=4096,
+):
     c_plus_q = context + ' ' + tokenizer.bos_token + ' ' + question
     c_plus_q_4 = [c_plus_q] * len(options)
 
     tokenized_examples = tokenizer(
         c_plus_q_4, options,
         max_length=max_seq_length,
         padding="longest",
```

### Comparing `selfcheckgpt-0.1.2/selfcheckgpt.egg-info/PKG-INFO` & `selfcheckgpt-0.1.3/selfcheckgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcheckgpt
-Version: 0.1.2
+Version: 0.1.3
 Summary: SelfCheckGPT: Assessing text-based responses from LLMs
 Home-page: https://github.com/potsawee/selfcheckgpt
 Author: Potsawee Manakul
 Author-email: m.potsawee@gmail.com
 License: MIT
 Keywords: selfcheckgpt
 Platform: UNKNOWN
```

### Comparing `selfcheckgpt-0.1.2/setup.py` & `selfcheckgpt-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 REQUIREMENTS = [
     "transformers>=4.11.3",
     "torch>=1.10",
     "numpy",
     "bert_score",
     "spacy",
+    "nltk",
 ]
 
 # some more details
 CLASSIFIERS = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

