# Comparing `tmp/event2vec-0.0.3.tar.gz` & `tmp/event2vec-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event2vec-0.0.3.tar", max compression
+gzip compressed data, was "event2vec-0.0.31.tar", max compression
```

## Comparing `event2vec-0.0.3.tar` & `event2vec-0.0.31.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    15731 2023-03-14 22:29:01.448203 event2vec-0.0.3/LICENSE
--rw-r--r--   0        0        0      762 2023-03-14 22:29:01.448203 event2vec-0.0.3/README.md
--rw-r--r--   0        0        0      242 2023-03-14 22:29:01.448203 event2vec-0.0.3/bin/config.cfg
--rw-r--r--   0        0        0     5993 2023-04-21 19:43:26.765843 event2vec-0.0.3/bin/submit_i2b2.py
--rw-r--r--   0        0        0     5384 2023-04-21 19:43:24.325844 event2vec-0.0.3/bin/submit_omop.py
--rw-r--r--   0        0        0       17 2023-03-14 22:29:01.778203 event2vec-0.0.3/event2vec/__init__.py
--rw-r--r--   0        0        0     1148 2023-03-14 22:29:01.778203 event2vec-0.0.3/event2vec/concept_proximity.py
--rw-r--r--   0        0        0     1411 2023-05-25 16:23:01.245183 event2vec-0.0.3/event2vec/config.py
--rw-r--r--   0        0        0     3999 2023-04-21 19:54:05.145765 event2vec-0.0.3/event2vec/cooccurrence_matrix_pandas.py
--rw-r--r--   0        0        0     7099 2023-04-22 02:17:00.822933 event2vec-0.0.3/event2vec/cooccurrence_matrix_spark.py
--rw-r--r--   0        0        0     1818 2023-05-25 19:08:52.021601 event2vec-0.0.3/event2vec/datasets.py
--rw-r--r--   0        0        0    20044 2023-05-25 19:30:10.891144 event2vec-0.0.3/event2vec/event_transformer.py
--rw-r--r--   0        0        0     6425 2023-03-14 22:29:01.778203 event2vec-0.0.3/event2vec/nomenclatures.py
--rw-r--r--   0        0        0     6867 2023-05-25 15:46:49.565958 event2vec-0.0.3/event2vec/svd_ppmi.py
--rw-r--r--   0        0        0     1687 2023-05-25 17:48:17.793351 event2vec-0.0.3/event2vec/utils.py
--rw-r--r--   0        0        0     4602 2023-05-25 17:34:06.453631 event2vec-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 event2vec-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    15731 2023-03-14 22:29:01.448203 event2vec-0.0.31/LICENSE
+-rw-r--r--   0        0        0      762 2023-03-14 22:29:01.448203 event2vec-0.0.31/README.md
+-rw-r--r--   0        0        0      242 2023-03-14 22:29:01.448203 event2vec-0.0.31/bin/config.cfg
+-rw-r--r--   0        0        0     5993 2023-04-21 19:43:26.765843 event2vec-0.0.31/bin/submit_i2b2.py
+-rw-r--r--   0        0        0     5384 2023-04-21 19:43:24.325844 event2vec-0.0.31/bin/submit_omop.py
+-rw-r--r--   0        0        0       17 2023-03-14 22:29:01.778203 event2vec-0.0.31/event2vec/__init__.py
+-rw-r--r--   0        0        0     1148 2023-03-14 22:29:01.778203 event2vec-0.0.31/event2vec/concept_proximity.py
+-rw-r--r--   0        0        0     1411 2023-05-25 16:23:01.245183 event2vec-0.0.31/event2vec/config.py
+-rw-r--r--   0        0        0     3999 2023-04-21 19:54:05.145765 event2vec-0.0.31/event2vec/cooccurrence_matrix_pandas.py
+-rw-r--r--   0        0        0     7099 2023-04-22 02:17:00.822933 event2vec-0.0.31/event2vec/cooccurrence_matrix_spark.py
+-rw-r--r--   0        0        0     1818 2023-05-25 19:08:52.021601 event2vec-0.0.31/event2vec/datasets.py
+-rw-r--r--   0        0        0    20171 2023-05-25 20:05:43.830384 event2vec-0.0.31/event2vec/event_transformer.py
+-rw-r--r--   0        0        0     6425 2023-03-14 22:29:01.778203 event2vec-0.0.31/event2vec/nomenclatures.py
+-rw-r--r--   0        0        0     6867 2023-05-25 20:21:37.250039 event2vec-0.0.31/event2vec/svd_ppmi.py
+-rw-r--r--   0        0        0     2040 2023-05-25 20:07:29.250350 event2vec-0.0.31/event2vec/utils.py
+-rw-r--r--   0        0        0     4603 2023-05-25 20:51:34.289397 event2vec-0.0.31/pyproject.toml
+-rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 event2vec-0.0.31/PKG-INFO
```

### Comparing `event2vec-0.0.3/LICENSE` & `event2vec-0.0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.3/README.md` & `event2vec-0.0.31/README.md`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.3/bin/submit_i2b2.py` & `event2vec-0.0.31/bin/submit_i2b2.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.3/bin/submit_omop.py` & `event2vec-0.0.31/bin/submit_omop.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.3/event2vec/concept_proximity.py` & `event2vec-0.0.31/event2vec/concept_proximity.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.3/event2vec/config.py` & `event2vec-0.0.31/event2vec/config.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.3/event2vec/cooccurrence_matrix_pandas.py` & `event2vec-0.0.31/event2vec/cooccurrence_matrix_pandas.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.3/event2vec/cooccurrence_matrix_spark.py` & `event2vec-0.0.31/event2vec/cooccurrence_matrix_spark.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.3/event2vec/datasets.py` & `event2vec-0.0.31/event2vec/datasets.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.3/event2vec/event_transformer.py` & `event2vec-0.0.31/event2vec/event_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pathlib import Path
 from typing import List, Union
 
 import numpy as np
 import pandas as pd
 import scipy.sparse as sp
 from loguru import logger
 from sklearn.base import BaseEstimator
@@ -235,27 +236,29 @@
         return X_embedded_df
 
 
 class Event2vecPretrained(Event2vecFeaturizer):
     def __init__(
         self,
         event: pd.DataFrame,
-        path2embedding: str,
+        embeddings: Union[str, Path, pd.DataFrame],
         colname_demographics: str = None,
         colname_code: str = COLNAME_SOURCE_CODE,
         n_min_events: int = 10,
         decay_half_life_in_days: np.array = np.array([0]),
     ) -> None:
         self.event = event
-        self.path2embedding = path2embedding
         self.colname_code = colname_code
         self.n_min_events = n_min_events
         self.colname_demographics = colname_demographics
         self.decay_half_life_in_days = decay_half_life_in_days
-        self.embedding = pd.read_parquet(self.path2embedding)
+        if isinstance(embeddings, str) | isinstance(embeddings, Path):
+            self.embeddings = pd.read_parquet(embeddings)
+        else:
+            self.embeddings = embeddings
 
     def fit(
         self,
         X: pd.DataFrame,
         y: pd.DataFrame = None,
         vocabulary: List[str] = None,
         static_features: List[str] = None,
@@ -266,18 +269,18 @@
         self.static_features_ = static_features
         if vocabulary is None:
             vocabulary = build_vocabulary(
                 event=X_event,
                 n_min_events=self.n_min_events,
             )
         self.vocabulary_ = list(
-            set(self.embedding.columns).intersection(set(vocabulary))
+            set(self.embeddings.columns).intersection(set(vocabulary))
         )
         #
-        self.embedding_ = self.embedding
+        self.embedding_ = self.embeddings
         return self
 
 
 ## Utils ##
 def build_vocabulary(
     event: pd.DataFrame,
     colname_code: str = COLNAME_SOURCE_CODE,
```

### Comparing `event2vec-0.0.3/event2vec/nomenclatures.py` & `event2vec-0.0.31/event2vec/nomenclatures.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.3/event2vec/svd_ppmi.py` & `event2vec-0.0.31/event2vec/svd_ppmi.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.3/event2vec/utils.py` & `event2vec-0.0.31/event2vec/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -55,7 +55,22 @@
     return window_start, window_end
 
 
 @dataclass
 class EventCohort:
     person: pd.DataFrame
     event: pd.DataFrame
+
+
+def get_embeddings_from_url(embedding_url):
+    """Get the embedding from a url.
+    The url should point to a parquet file with concept as columns and embedding
+    as rows.
+
+    Args:
+        embedding_url (str): _description_
+
+    Returns:
+        _type_: _description_
+    """
+    embeddings = pd.read_parquet(embedding_url)
+    return embeddings
```

### Comparing `event2vec-0.0.3/pyproject.toml` & `event2vec-0.0.31/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "event2vec"
-version = "0.0.3"
+version = "0.0.31"
 description = "event2vec"
 authors = ["Matthieu Doutreligne <matt.dout@gmail.com>"]
 license = "EUPL-v1.2"
 readme = "README.md"
 repository = "https://gitlab.com/strayMat/event2vec"
 homepage = "https://gitlab.com/strayMat/event2vec"
 include = ["bin"]
```

### Comparing `event2vec-0.0.3/PKG-INFO` & `event2vec-0.0.31/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event2vec
-Version: 0.0.3
+Version: 0.0.31
 Summary: event2vec
 Home-page: https://gitlab.com/strayMat/event2vec
 License: EUPL-v1.2
 Author: Matthieu Doutreligne
 Author-email: matt.dout@gmail.com
 Requires-Python: >=3.7.1,<3.11
 Classifier: Intended Audience :: Developers
```

