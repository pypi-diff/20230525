# Comparing `tmp/neofuzz-0.1.2.tar.gz` & `tmp/neofuzz-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neofuzz-0.1.2.tar", max compression
+gzip compressed data, was "neofuzz-0.1.3.tar", max compression
```

## Comparing `neofuzz-0.1.2.tar` & `neofuzz-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-03-22 12:44:38.279428 neofuzz-0.1.2/LICENSE
--rw-r--r--   0        0        0     3324 2023-04-04 13:47:12.230257 neofuzz-0.1.2/README.md
--rw-r--r--   0        0        0       93 2023-04-04 13:58:50.523417 neofuzz-0.1.2/neofuzz/__init__.py
--rw-r--r--   0        0        0    13418 2023-04-04 13:34:30.465010 neofuzz-0.1.2/neofuzz/process.py
--rw-r--r--   0        0        0      458 2023-04-04 13:59:10.595451 neofuzz-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 neofuzz-0.1.2/setup.py
--rw-r--r--   0        0        0     3955 1970-01-01 00:00:00.000000 neofuzz-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-03-22 12:44:38.279428 neofuzz-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5488 2023-05-25 12:23:34.282570 neofuzz-0.1.3/README.md
+-rw-r--r--   0        0        0       93 2023-04-04 13:58:50.523417 neofuzz-0.1.3/neofuzz/__init__.py
+-rw-r--r--   0        0        0    13324 2023-05-25 11:59:41.367811 neofuzz-0.1.3/neofuzz/process.py
+-rw-r--r--   0        0        0      458 2023-05-25 12:22:50.610406 neofuzz-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6307 1970-01-01 00:00:00.000000 neofuzz-0.1.3/setup.py
+-rw-r--r--   0        0        0     6119 1970-01-01 00:00:00.000000 neofuzz-0.1.3/PKG-INFO
```

### Comparing `neofuzz-0.1.2/LICENSE` & `neofuzz-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neofuzz-0.1.2/neofuzz/process.py` & `neofuzz-0.1.3/neofuzz/process.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,126 +13,128 @@
 
     Parameters
     ----------
     vectorizer: sklearn vectorizer
         Some kind of vectorizer model that can vectorize strings.
         You could use tf-idf, bow or even a Pipeline that
         has multiple steps.
-    metric: string or callable (optional, default='euclidean')
+    metric: string or callable, default 'euclidean'
         The metric to use for computing nearest neighbors. If a callable is
         used it must be a numba njit compiled function. Supported metrics
         include:
-            * euclidean
-            * manhattan
-            * chebyshev
-            * minkowski
-            * canberra
-            * braycurtis
-            * mahalanobis
-            * wminkowski
-            * seuclidean
-            * cosine
-            * correlation
-            * haversine
-            * hamming
-            * jaccard
-            * dice
-            * russelrao
-            * kulsinski
-            * rogerstanimoto
-            * sokalmichener
-            * sokalsneath
-            * yule
-            * hellinger
-            * wasserstein-1d
+
+        * euclidean
+        * manhattan
+        * chebyshev
+        * minkowski
+        * canberra
+        * braycurtis
+        * mahalanobis
+        * wminkowski
+        * seuclidean
+        * cosine
+        * correlation
+        * haversine
+        * hamming
+        * jaccard
+        * dice
+        * russelrao
+        * kulsinski
+        * rogerstanimoto
+        * sokalmichener
+        * sokalsneath
+        * yule
+        * hellinger
+        * wasserstein-1d
+
         Metrics that take arguments (such as minkowski, mahalanobis etc.)
         can have arguments passed via the metric_kwds dictionary. At this
         time care must be taken and dictionary elements must be ordered
         appropriately; this will hopefully be fixed in the future.
-    metric_kwds: dict (optional, default {})
+    metric_kwds: dict, default {}
         Arguments to pass on to the metric, such as the ``p`` value for
         Minkowski distance.
-    n_neighbors: int (optional, default=30)
+    n_neighbors: int, default 30
         The number of neighbors to use in k-neighbor graph graph_data structure
         used for fast approximate nearest neighbor search. Larger values
         will result in more accurate search results at the cost of
         computation time.
-    n_trees: int (optional, default=None)
+    n_trees: int, default None
         This implementation uses random projection forests for initializing the index
         build process.
         This parameter controls the number of trees in that forest.
         A larger number will result in more accurate neighbor computation
         at the cost of performance.
         The default of None means a value will be chosen based on the
         size of the graph_data.
-    leaf_size: int (optional, default=None)
+    leaf_size: int, default None
         The maximum number of points in a leaf for the random projection trees.
         The default of None means a value will be chosen based on n_neighbors.
-    pruning_degree_multiplier: float (optional, default=1.5)
+    pruning_degree_multiplier: float, default 1.5
         How aggressively to prune the graph.
         Since the search graph is undirected
         (and thus includes nearest neighbors and reverse nearest neighbors)
         vertices can have very high degree
         -- the graph will be pruned such that no
         vertex has degree greater than
         ``pruning_degree_multiplier * n_neighbors``.
-    diversify_prob: float (optional, default=1.0)
+    diversify_prob: float, default 1.0
         The search graph get "diversified" by removing potentially unnecessary
         edges. This controls the volume of edges removed.
         A value of 0.0 ensures that no edges get removed,
         and larger values result in significantly more
         aggressive edge removal.
         A value of 1.0 will prune all edges that it can.
-    tree_init: bool (optional, default=True)
+    tree_init: bool, default True
         Whether to use random projection trees for initialization.
-    init_graph: np.ndarray (optional, default=None)
+    init_graph: np.ndarray, default None
         2D array of indices of candidate neighbours of the shape
         (data.shape[0], n_neighbours). If the j-th neighbour of the i-th
         instances is unknown, use init_graph[i, j] = -1
-    init_dist: np.ndarray (optional, default=None)
+    init_dist: np.ndarray, default None
         2D array with the same shape as init_graph,
         such that metric(data[i], data[init_graph[i, j]]) equals
         init_dist[i, j]
-    random_state: int, RandomState instance or None, optional (default: None)
+    random_state: int, RandomState instance or None, default None
         If int, random_state is the seed used by the random number generator;
         If RandomState instance, random_state is the random number generator;
         If None, the random number generator is the RandomState instance used
         by `np.random`.
-    algorithm: string (optional, default='standard')
+    algorithm: str, default 'standard'
         This implementation provides an alternative algorithm for
         construction of the k-neighbors graph used as a search index. The
         alternative algorithm can be fast for large ``n_neighbors`` values.
         The``'alternative'`` algorithm has been deprecated and is no longer
         available.
-    low_memory: boolean (optional, default=True)
+    low_memory: boolean, default True
         Whether to use a lower memory, but more computationally expensive
         approach to index construction.
-    max_candidates: int (optional, default=None)
+    max_candidates: int, default None
         Internally each "self-join" keeps a maximum number of candidates (
         nearest neighbors and reverse nearest neighbors) to be considered.
         This value controls this aspect of the algorithm. Larger values will
         provide more accurate search results later, but potentially at
         non-negligible computation cost in building the index. Don't tweak
         this value unless you know what you're doing.
-    n_iters: int (optional, default=None)
+    n_iters: int, default None
         The maximum number of NN-descent iterations to perform. The
         NN-descent algorithm can abort early if limited progress is being
         made, so this only controls the worst case. Don't tweak
         this value unless you know what you're doing. The default of None means
         a value will be chosen based on the size of the graph_data.
-    delta: float (optional, default=0.001)
+    delta: float, default 0.001
         Controls the early abort due to limited progress. Larger values
         will result in earlier aborts, providing less accurate indexes,
         and less accurate searching. Don't tweak this value unless you know
         what you're doing.
-    n_jobs: int or None, optional (default=None)
+    n_jobs: int or None, default None
         The number of parallel jobs to run for neighbors index construction.
         ``None`` means 1 unless in a :obj:`joblib.parallel_backend` context.
         ``-1`` means using all processors.
-    compressed: bool (optional, default=False)
+    compressed: bool, default False
         Whether to prune out data not needed for searching the index. This will
         result in a significantly smaller index, particularly useful
         for saving,
         but will remove information that might otherwise be useful.
     """
 
     def __init__(
@@ -191,15 +193,21 @@
 
         Parameters
         ----------
         options: iterable of str
             All options in which we want search.
         """
         self.options = np.array(options)
-        dtm = self.vectorizer.fit_transform(self.options)
+        try:
+            self.vectorizer.fit(self.options)
+        except AttributeError:
+            print(
+                "Vectorizer could not be fitted, we assume it was pretrained."
+            )
+        dtm = self.vectorizer.transform(self.options)
         self.nearest_neighbours = pynndescent.NNDescent(
             dtm, **self.nearest_neighbours_kwargs
         )
         self.nearest_neighbours.prepare()
 
     def query(
         self, search_terms: Iterable[str], limit: int = 10
```

### Comparing `neofuzz-0.1.2/PKG-INFO` & `neofuzz-0.1.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,45 @@
-Metadata-Version: 2.1
-Name: neofuzz
-Version: 0.1.2
-Summary: Blazing fast fuzzy text search for Python.
-License: MIT
-Author: Márton Kardos
-Author-email: power.up1163@gmail.com
-Requires-Python: >=3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pynndescent (>=0.5.0,<0.6.0)
-Requires-Dist: scikit-learn (>=1.1.0,<1.3.0)
-Description-Content-Type: text/markdown
+# Neofuzz
 
-# neofuzz
+Blazing fast, lightweight and customizable fuzzy and semantic text search in Python.
 
-Blazing fast fuzzy text search for Python.
+## Introduction ([Documentation](https://x-tabdeveloping.github.io/neofuzz/))
+Neofuzz is a fuzzy search library based on vectorization and approximate nearest neighbour
+search techniques.
 
-## Introduction
+### Why is Neofuzz fast?
+Most fuzzy search libraries rely on optimizing the hell out of the same couple of fuzzy search algorithms (Hamming distance, Levenshtein distance). Sometimes unfortunately due to the complexity of these algorithms, no amount of optimization will get you the speed, that you want.
 
-neofuzz is a fuzzy search library based on vectorization and approximate nearest neighbour
-search techniques.
+Neofuzz makes the realization, that you can’t go above a certain speed limit by relying on traditional algorithms, and uses text vectorization and approximate nearest neighbour search in the vector space to speed up this process.
 
-What neofuzz is good at:
-  - Hella Fast.
-  - Repeated searches in the same space of options.
-  - Compatibility with already existing TheFuzz code.
-  - Incredible flexibility in the vectorization process.
-  - Complete control over the nearest neighbour algorithm's speed and accuracy.
-
-If you're looking for a scalable solution for searching the same, large dataset
-with lower quality of results but incredible speed, neofuzz is the thing you're looking for.
-
-What neofuzz is not good at:
-  - Exact and certainly correct results.
-  - Searching different databases in succession.
-  - Not the best fuzzy search algorithm.
-
-If you're looking for a library that's great for fuzzy searching small amount of data with a
-good fuzzy algorithm like levenshtein or hamming distance, neofuzz is probably not
-the thing for you.
+When it comes to the dilemma of speed versus accuracy, Neofuzz goes full-on speed.
 
-## Usage
+### When should I choose Neofuzz?
+ - You need to do repeated searches in the same corpus.
+ - Levenshtein and Hamming distance is simply not fast enough.
+ - You are willing to sacrifice the quality of the results for speed.
+ - You don’t mind that the up-front computation to index a corpus might take time.
+ - You have very long strings, where other methods would be impractical.
+ - You want to rely on semantic content.
+ - You need a drop-in replacement for TheFuzz.
+
+### When should I NOT choose Neofuzz?
+ - The corpus changes all the time, or you only want to do one search in a corpus. (It might still give speed-up in that case though.)
+ - You value the quality of the results over speed.
+ - You don’t mind slower searches in favor of no indexing.
+ - You have a small corpus with short strings.
 
-You can install neofuzz from PyPI:
+## [Usage](https://x-tabdeveloping.github.io/neofuzz/getting_started.html)
+
+You can install Neofuzz from PyPI:
 
 ```bash
 pip install neofuzz
 ```
 
-The base abstraction of neofuzz is the `Process`, which is a class aimed at replicating TheFuzz's API.
-
-A `Process` takes a vectorizer, that turns strings into vectorized form, and different parameters
-for fine-tuning the indexing process.
-
 If you want a plug-and play experience you can create a generally good quick and dirty
 process with the `char_ngram_process()` process.
 
 ```python
 from neofuzz import char_ngram_process
 
 # We create a process that takes character 1 to 5-grams as features for
@@ -83,42 +62,73 @@
  ('zu', 20),
  ('Zo', 18),
  ('blog_BuzzMachine', 18),
  ('LW_Todd_Bertuzzi', 18),
  ('OFU', 17)]
 ```
 
-If you want to use a custom vectorization process with dimentionality reduction for example,
-you are more than free to do so by creating your own custom `Process`
+## [Custom Processes](https://x-tabdeveloping.github.io/neofuzz/custom_vectorizer.html)
+
+You can customize Neofuzz’s behaviour by making a custom process.
+Under the hood every Neofuzz Process relies on the same two components:
+
+ - A vectorizer, which turns texts into a vectorized form, and can be fully customized.
+ - Approximate Nearest Neighbour search, which indexes the vector space and can find neighbours of a given vector very quickly. This component is fixed to be PyNNDescent, but all of its parameters are exposed in the API, so its behaviour can also be altered at will.
+
+### Words as Features
+
+If you’re more interested in the words/semantic content of the text you can also use them as features. This can be very useful especially with longer texts, such as literary works.
 
 ```python
 from neofuzz import Process
+from sklearn.feature_extraction.text import TfidfVectorizer
 
-from sklearn.decomposition import NMF
+ # Vectorization with words is the default in sklearn.
+ vectorizer = TfidfVectorizer()
+
+ # We use cosine distance because it's waay better for high-dimentional spaces.
+ process = Process(vectorizer, metric="cosine")
+```
+
+### Dimentionality Reduction
+
+You might find that the speed of your fuzzy search process is not sufficient. In this case it might be desirable to reduce the dimentionality of the produced vectors with some matrix decomposition method or topic model.
+
+Here for example I use NMF (excellent topic model and incredibly fast one too) too speed up my fuzzy search pipeline.
+
+```python
+from neofuzz import Process
 from sklearn.feature_extraction.text import TfidfVectorizer
-from sklearn.pipeline import make_pipeline
+from sklearn.decomposition import NMF
+from sklear.pipeline import make_pipeline
 
-# Let's say we have a list of sentences instead of words,
-# Then we can use token ngrams as features
-tf_idf = TfidfVectorizer(analyzer="word", stop_words="english", ngram_range=(1,3))
-# We use NMF for reducing the dimensionality of the vectors to 20
-# This could improve speed but takes more time to set up the index
+# Vectorization with tokens again
+vectorizer = TfidfVectorizer()
+# Dimentionality reduction method to 20 dimentions
 nmf = NMF(n_components=20)
+# Create a pipeline of the two
+pipeline = make_pipeline(vectorizer, nmf)
+
+process = Process(pipeline, metric="cosine")
+```
 
-# Our vectorizer is going to be a pipeline
-vectorizer = make_pipeline(tf_idf, nmf)
+### Semantic Search/Large Language Models
 
-# We create a process and index it with our corpus.
-process = Process(vectorizer, metric="cosine")
-process.index(sentences)
+With Neofuzz you can easily use semantic embeddings to your advantage, and can use both attention-based language models (Bert), just simple neural word or document embeddings (Word2Vec, Doc2Vec, FastText, etc.) or even OpenAI’s LLMs.
 
-# Then you can extract results
-process.extract("she ate the cat", limit=3)
--------------------------------------------
-[('She ate the Apple.', 65),
- ('The dog at the cat.', 42),
- ('She loves that cat', 30)]
+We recommend you try embetter, which has a lot of built-in sklearn compatible vectorizers.
+```bash
+pip install embetter
 ```
 
-## Documentation
-TODO
+```python
+from embetter.text import SentenceEncoder
+from neofuzz import Process
 
+# Here we will use a pretrained Bert sentence encoder as vectorizer
+vectorizer = SentenceEncoder("all-distilroberta-v1")
+# Then we make a process with the language model
+process = Process(vectorizer, metric="cosine")
+
+# Remember that the options STILL have to be indexed even though you have a pretrained vectorizer
+process.index(options)
+```
```

