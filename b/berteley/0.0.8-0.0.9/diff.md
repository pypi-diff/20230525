# Comparing `tmp/berteley-0.0.8.tar.gz` & `tmp/berteley-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "berteley-0.0.8.tar", last modified: Tue May  2 16:29:39 2023, max compression
+gzip compressed data, was "berteley-0.0.9.tar", last modified: Wed May 17 22:39:43 2023, max compression
```

## Comparing `berteley-0.0.8.tar` & `berteley-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:29:39.364173 berteley-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-02 16:29:29.000000 berteley-0.0.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-02 16:29:29.000000 berteley-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-02 16:29:29.000000 berteley-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-02 16:29:39.364173 berteley-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-02 16:29:29.000000 berteley-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:29:39.364173 berteley-0.0.8/berteley/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-02 16:29:29.000000 berteley-0.0.8/berteley/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-02 16:29:39.364173 berteley-0.0.8/berteley/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-02 16:29:29.000000 berteley-0.0.8/berteley/berteley_stopwords.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-05-02 16:29:29.000000 berteley-0.0.8/berteley/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-05-02 16:29:29.000000 berteley-0.0.8/berteley/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:29:29.000000 berteley-0.0.8/berteley/recommendation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:29:39.360169 berteley-0.0.8/berteley.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-02 16:29:39.000000 berteley-0.0.8/berteley.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-02 16:29:39.000000 berteley-0.0.8/berteley.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:29:39.000000 berteley-0.0.8/berteley.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:29:39.000000 berteley-0.0.8/berteley.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-02 16:29:39.000000 berteley-0.0.8/berteley.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 16:29:39.000000 berteley-0.0.8/berteley.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:29:39.360169 berteley-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-02 16:29:29.000000 berteley-0.0.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-02 16:29:29.000000 berteley-0.0.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:29:39.364173 berteley-0.0.8/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-02 16:29:29.000000 berteley-0.0.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-02 16:29:39.364173 berteley-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-02 16:29:29.000000 berteley-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:29:39.364173 berteley-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:29:29.000000 berteley-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-02 16:29:29.000000 berteley-0.0.8/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-02 16:29:29.000000 berteley-0.0.8/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:29:29.000000 berteley-0.0.8/tests/test_recommendation.py
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-05-02 16:29:29.000000 berteley-0.0.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:39:43.194898 berteley-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-17 22:39:34.000000 berteley-0.0.9/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-17 22:39:34.000000 berteley-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-17 22:39:34.000000 berteley-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-17 22:39:43.194898 berteley-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-17 22:39:34.000000 berteley-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:39:43.194898 berteley-0.0.9/berteley/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-17 22:39:34.000000 berteley-0.0.9/berteley/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-17 22:39:43.194898 berteley-0.0.9/berteley/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-17 22:39:34.000000 berteley-0.0.9/berteley/berteley_stopwords.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-05-17 22:39:34.000000 berteley-0.0.9/berteley/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-05-17 22:39:34.000000 berteley-0.0.9/berteley/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:39:34.000000 berteley-0.0.9/berteley/recommendation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:39:43.194898 berteley-0.0.9/berteley.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-17 22:39:43.000000 berteley-0.0.9/berteley.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-17 22:39:43.000000 berteley-0.0.9/berteley.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:39:43.000000 berteley-0.0.9/berteley.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:39:43.000000 berteley-0.0.9/berteley.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-17 22:39:43.000000 berteley-0.0.9/berteley.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 22:39:43.000000 berteley-0.0.9/berteley.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:39:43.194898 berteley-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-17 22:39:34.000000 berteley-0.0.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-17 22:39:34.000000 berteley-0.0.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:39:43.194898 berteley-0.0.9/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-17 22:39:34.000000 berteley-0.0.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-17 22:39:43.194898 berteley-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-17 22:39:34.000000 berteley-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:39:43.194898 berteley-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:39:34.000000 berteley-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-17 22:39:34.000000 berteley-0.0.9/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-17 22:39:34.000000 berteley-0.0.9/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:39:34.000000 berteley-0.0.9/tests/test_recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-05-17 22:39:34.000000 berteley-0.0.9/versioneer.py
```

### Comparing `berteley-0.0.8/LICENSE` & `berteley-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `berteley-0.0.8/PKG-INFO` & `berteley-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berteley
-Version: 0.0.8
+Version: 0.0.9
 Summary: Topic modeling for scientific articles
 Home-page: https://github.com/lbl-camera/berteley
 Author: Eric Chagnon, Ronald J. Pandolfi, Daniela Ushizima
 Author-email: echagnon@lbl.gov
 License: BSD license
 Keywords: berteley
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `berteley-0.0.8/README.md` & `berteley-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `berteley-0.0.8/berteley/models.py` & `berteley-0.0.9/berteley/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,27 +116,28 @@
         topic_sizes
                 a dictionary with key: topic number and the value: the number of documents assigned the said topic
         topic_model
                 the fitted BERTopic model
         topic_words
                 a dictionary with key: the topic number and the value: a list of strings
         """
-
+    opts = dict()
+    
     if not isinstance(embedding_model, SentenceTransformer) and not isinstance(n_gram_type, tuple):
-        embedding_model, n_gram_range = initialize_model(embedding_model, nr_topics, n_gram_type, verbose)
+        embedding_model, opts['n_gram_range'] = initialize_model(embedding_model, nr_topics, n_gram_type, verbose)
 
     if not isinstance(data, list) or (isinstance(data, list) and not isinstance(data[0], str)):
         raise TypeError("Data must be a list of strings")
 
     topic_model = BERTopic(embedding_model=embedding_model,
                            nr_topics=nr_topics,
-                           n_gram_range=n_gram_range,
-                           verbose=verbose)
+                           verbose=verbose, 
+                           **opts)
     topics, probabilities = topic_model.fit_transform(data)
-    metrics = _calculate_metrics(data, topic_model, topics, n_gram_range)
+    metrics = _calculate_metrics(data, topic_model, topics, **opts)
     topic_sizes = _calculate_topic_sizes(topics)
     topic_words = topic_model.topic_representations_
 
     return topics, probabilities, metrics, topic_sizes, topic_model, topic_words
 
 
 def _calculate_topic_sizes(topics: List[int]):
@@ -179,15 +180,15 @@
         topic_words[k] = [x[0] for x in topic_dict[k]]
     word_list = list(topic_words.values())
     word_list.pop(0)
 
     # octis requires the texts input be in the form of a list of list of strings
     octis_texts = [sentence.split() for sentence in texts]
 
-    npmi = Coherence(texts=octis_texts, topk=10, measure='c_npmi')
+    npmi = Coherence(texts=octis_texts, topk=10, measure='c_v')
     topic_diversity = TopicDiversity(topk=10)
 
     # reformat the output of BERTopic to the proper format
     # {topics: [[topic, words, for, topic1], [topic, words, for, topic2], [etc, etc, etc]]}
     all_words = [word for words in octis_texts for word in words]
 
     # check if the model is bigram
@@ -252,15 +253,15 @@
                    for topic in range(len(set(topics)) - 1)]
 
     # Evaluate
     coherence_model = CoherenceModel(topics=topic_words,
                                      texts=tokens,
                                      corpus=corpus,
                                      dictionary=dictionary,
-                                     coherence='c_npmi')
+                                     coherence='c_v')
     coherence = coherence_model.get_coherence()
     return coherence
 
 
 def create_barcharts(topics, topic_model: BERTopic, path=""):
     """
     creates and saves the BERTopic barcharts
```

### Comparing `berteley-0.0.8/berteley/preprocessing.py` & `berteley-0.0.9/berteley/preprocessing.py`

 * *Files identical despite different names*

### Comparing `berteley-0.0.8/berteley.egg-info/PKG-INFO` & `berteley-0.0.9/berteley.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berteley
-Version: 0.0.8
+Version: 0.0.9
 Summary: Topic modeling for scientific articles
 Home-page: https://github.com/lbl-camera/berteley
 Author: Eric Chagnon, Ronald J. Pandolfi, Daniela Ushizima
 Author-email: echagnon@lbl.gov
 License: BSD license
 Keywords: berteley
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `berteley-0.0.8/berteley.egg-info/SOURCES.txt` & `berteley-0.0.9/berteley.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `berteley-0.0.8/docs/Makefile` & `berteley-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `berteley-0.0.8/docs/make.bat` & `berteley-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `berteley-0.0.8/docs/source/conf.py` & `berteley-0.0.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `berteley-0.0.8/setup.py` & `berteley-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `berteley-0.0.8/tests/test_models.py` & `berteley-0.0.9/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `berteley-0.0.8/tests/test_preprocessing.py` & `berteley-0.0.9/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `berteley-0.0.8/versioneer.py` & `berteley-0.0.9/versioneer.py`

 * *Files identical despite different names*

