# Comparing `tmp/event2vec-0.0.1.tar.gz` & `tmp/event2vec-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event2vec-0.0.1.tar", max compression
+gzip compressed data, was "event2vec-0.0.3.tar", max compression
```

## Comparing `event2vec-0.0.1.tar` & `event2vec-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,17 @@
--rw-r--r--   0        0        0    15731 2022-12-15 13:18:56.917210 event2vec-0.0.1/LICENSE
--rw-r--r--   0        0        0      808 2023-03-10 15:07:08.679767 event2vec-0.0.1/README.md
--rw-r--r--   0        0        0      242 2023-02-23 10:17:18.166984 event2vec-0.0.1/bin/config.cfg
--rw-r--r--   0        0        0     5976 2023-02-23 10:17:17.246981 event2vec-0.0.1/bin/submit_i2b2.py
--rw-r--r--   0        0        0     5367 2023-02-23 10:17:17.250981 event2vec-0.0.1/bin/submit_omop.py
--rw-r--r--   0        0        0       17 2022-12-15 13:18:57.013213 event2vec-0.0.1/event2vec/__init__.py
--rw-r--r--   0        0        0     1148 2023-02-23 19:18:55.166181 event2vec-0.0.1/event2vec/concept_proximity.py
--rw-r--r--   0        0        0     1131 2023-02-23 10:17:17.250981 event2vec-0.0.1/event2vec/config.py
--rw-r--r--   0        0        0     6425 2023-02-23 19:18:55.226177 event2vec-0.0.1/event2vec/nomenclatures.py
--rw-r--r--   0        0        0    18348 2023-03-10 14:42:24.441004 event2vec-0.0.1/event2vec/svd_ppmi.py
--rw-r--r--   0        0        0     4423 2023-03-12 18:44:08.301322 event2vec-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2649 1970-01-01 00:00:00.000000 event2vec-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    15731 2023-03-14 22:29:01.448203 event2vec-0.0.3/LICENSE
+-rw-r--r--   0        0        0      762 2023-03-14 22:29:01.448203 event2vec-0.0.3/README.md
+-rw-r--r--   0        0        0      242 2023-03-14 22:29:01.448203 event2vec-0.0.3/bin/config.cfg
+-rw-r--r--   0        0        0     5993 2023-04-21 19:43:26.765843 event2vec-0.0.3/bin/submit_i2b2.py
+-rw-r--r--   0        0        0     5384 2023-04-21 19:43:24.325844 event2vec-0.0.3/bin/submit_omop.py
+-rw-r--r--   0        0        0       17 2023-03-14 22:29:01.778203 event2vec-0.0.3/event2vec/__init__.py
+-rw-r--r--   0        0        0     1148 2023-03-14 22:29:01.778203 event2vec-0.0.3/event2vec/concept_proximity.py
+-rw-r--r--   0        0        0     1411 2023-05-25 16:23:01.245183 event2vec-0.0.3/event2vec/config.py
+-rw-r--r--   0        0        0     3999 2023-04-21 19:54:05.145765 event2vec-0.0.3/event2vec/cooccurrence_matrix_pandas.py
+-rw-r--r--   0        0        0     7099 2023-04-22 02:17:00.822933 event2vec-0.0.3/event2vec/cooccurrence_matrix_spark.py
+-rw-r--r--   0        0        0     1818 2023-05-25 19:08:52.021601 event2vec-0.0.3/event2vec/datasets.py
+-rw-r--r--   0        0        0    20044 2023-05-25 19:30:10.891144 event2vec-0.0.3/event2vec/event_transformer.py
+-rw-r--r--   0        0        0     6425 2023-03-14 22:29:01.778203 event2vec-0.0.3/event2vec/nomenclatures.py
+-rw-r--r--   0        0        0     6867 2023-05-25 15:46:49.565958 event2vec-0.0.3/event2vec/svd_ppmi.py
+-rw-r--r--   0        0        0     1687 2023-05-25 17:48:17.793351 event2vec-0.0.3/event2vec/utils.py
+-rw-r--r--   0        0        0     4602 2023-05-25 17:34:06.453631 event2vec-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 event2vec-0.0.3/PKG-INFO
```

### Comparing `event2vec-0.0.1/LICENSE` & `event2vec-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.1/README.md` & `event2vec-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -8,16 +8,11 @@
 
 Electronic Health Record and claims contain sequences of care: every contact
 between a patient and a healthcare system (either hospital, either insurance) is
 recorded in a central database. Medical terminologies are often used to encode
 the type of care : diagnoses, acts, drugs, laboratory, ...
 
 Such healthcare trajectories can be viewed as sequence of tokens, similarly to
-sequences of words. Embeddings techniques .
+sequences of words.
 
 This package propose to use matrix factorization as a simple and efficient way
 to build event embedding from a medical observational database.
-
-
-## Features
-
-- TODO
```

### Comparing `event2vec-0.0.1/bin/submit_i2b2.py` & `event2vec-0.0.3/bin/submit_i2b2.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from eds_scikit import improve_performances
 from eds_scikit.io import HiveData
 from edstoolbox import SparkApp
 from loguru import logger
 from pyspark.sql import SparkSession
 
 from event2vec.config import DIR2DATA, DIR2RESULTS
-from event2vec.svd_ppmi import event2vec
+from event2vec.cooccurrence_matrix_spark import event2vec
 
 app = SparkApp("event2vec")
 
 
 @app.submit
 def run(spark, sql, config):
     """
```

### Comparing `event2vec-0.0.1/bin/submit_omop.py` & `event2vec-0.0.3/bin/submit_omop.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from eds_scikit import improve_performances
 from eds_scikit.io import HiveData
 from edstoolbox import SparkApp
 from loguru import logger
 from pyspark.sql import SparkSession
 
 from event2vec.config import DIR2DATA, DIR2RESULTS
-from event2vec.svd_ppmi import event2vec
+from event2vec.cooccurrence_matrix_spark import event2vec
 
 app = SparkApp("event2vec")
 
 
 @app.submit
 def run(spark, sql, config):
     """
```

### Comparing `event2vec-0.0.1/event2vec/concept_proximity.py` & `event2vec-0.0.3/event2vec/concept_proximity.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.1/event2vec/nomenclatures.py` & `event2vec-0.0.3/event2vec/nomenclatures.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.1/event2vec/svd_ppmi.py` & `event2vec-0.0.3/event2vec/event_transformer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,501 +1,585 @@
-import json
-import os
-from datetime import datetime
-from itertools import chain
-from pathlib import Path
-from typing import Dict, List, Tuple
+from typing import List, Union
 
 import numpy as np
 import pandas as pd
-import pyspark.ml.feature as ml_feature
-import pyspark.sql.functions as func
+import scipy.sparse as sp
 from loguru import logger
-from pyarrow import parquet as pq
-from pyspark.mllib.linalg import DenseVector
-from pyspark.sql import DataFrame, SparkSession, Window
-from scipy.sparse import csr_matrix, save_npz
-from scipy.sparse.linalg import svds
-from sklearn.feature_extraction.text import CountVectorizer
+from sklearn.base import BaseEstimator
 
-
-def days_to_seconds(days: int) -> int:
-    return days * 86400
+from event2vec.config import (
+    COLNAME_FOLLOWUP_START,
+    COLNAME_PERSON,
+    COLNAME_SOURCE_CODE,
+    COLNAME_START,
+    COLNAME_VALUE,
+    OBSERVATION_END,
+    OBSERVATION_START,
+)
+
+# TODO: separate pyspark and pandas scripts
+from event2vec.svd_ppmi import event2vec
+
+# TODO: These transformers should  rely on a batch version of sklearn
+# Countvectorizer instead of the inefficient make_count.
+# This could better exploit the sparsity of the count encoding. I
+# could take inspiration from
+# https://github1s.com/scikit-learn/scikit-learn/blob/baf828ca1/sklearn/feature_extraction/_dict_vectorizer.py
+# and populate only non-null indices.
+
+
+class EventTransformerMixin:
+    """Mixin class for all event transformers that requires y at the transform
+    step (to align the person id with the features)."""
+
+    def fit_transform(self, X, y=None, **fit_params):
+        """
+        Fit to data, then transform it.
+
+        Fits transformer to `X` and `y` with optional parameters `fit_params`
+        and returns a transformed version of `X`.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            Input samples.
+
+        y :  array-like of shape (n_samples,) or (n_samples, n_outputs),
+            Target values.
+
+        **fit_params : dict
+            Additional fit parameters.
+
+        Returns
+        -------
+        X_new : ndarray array of shape (n_samples, n_features_new)
+            Transformed array.
+        """
+        # fit method of arity 2 (supervised transformation)
+
+        return self.fit(X, y, **fit_params).transform(X)
+
+
+class OneHotEvent(EventTransformerMixin, BaseEstimator):
+    """
+    From a event table, create a vocabulary at fit, and pivot the data for a
+    count one-hot encoding, ie. count for each code in the vocabulary, and for
+    each patient if the event is present or not.
+    """
+
+    def __init__(
+        self,
+        event: pd.DataFrame,
+        n_min_events: int = 10,
+        colname_demographics: List[str] = None,
+        decay_half_life_in_days: np.array = np.array([0]),
+    ) -> None:
+        self.event = event
+        self.n_min_events = n_min_events
+        self.colname_demographics = colname_demographics
+        self.decay_half_life_in_days = decay_half_life_in_days
+
+    def fit(
+        self,
+        X: pd.DataFrame,
+        y: pd.DataFrame = None,
+        vocabulary: List[str] = None,
+        static_features: List[str] = None,
+    ):
+        X_event = self.event.merge(
+            X[[COLNAME_PERSON]], on=COLNAME_PERSON, how="inner"
+        )
+        self.static_features_ = static_features
+        if vocabulary is None:
+            self.vocabulary_ = build_vocabulary(
+                event=X_event,
+                n_min_events=self.n_min_events,
+            )
+        else:
+            self.vocabulary_ = vocabulary
+        return self
+
+    def transform(self, X: pd.DataFrame) -> np.array:
+        X_event = self.event.merge(
+            X[[COLNAME_PERSON]], on=COLNAME_PERSON, how="inner"
+        )
+        X_counts = make_counts(
+            event=X_event,
+            person_id=X[[COLNAME_PERSON]],
+            decay_half_life_in_days=self.decay_half_life_in_days,
+            vocabulary=self.vocabulary_,
+            sparse=True,
+        ).toarray()
+
+        X_columns = []
+        for decay in self.decay_half_life_in_days:
+            for code_ in self.vocabulary_:
+                X_columns.append(f"{code_}__decay_{decay}")
+
+        X_df = pd.DataFrame(X_counts, columns=X_columns)
+        if self.static_features_ is not None:
+            X_df = pd.concat([X[self.static_features_], X_df], axis=1)
+
+        return X_df
+
+
+class Event2vecFeaturizer(EventTransformerMixin, BaseEstimator):
+    """
+    Transformer for the event2vec model.
+    """
+
+    def __init__(
+        self,
+        event: pd.DataFrame,
+        output_dir: str = None,
+        colname_code: str = COLNAME_SOURCE_CODE,
+        colname_demographics: List[str] = None,
+        window_radius_in_days=30,
+        window_orientation: str = "center",
+        matrix_type: str = "numpy",
+        backend="pandas",
+        d: int = 300,
+        smoothing_factor: float = 0.75,
+        k: int = 1,
+        n_min_events: int = 10,
+        decay_half_life_in_days: np.array = np.array([0]),
+    ) -> None:
+        self.event = event
+        self.output_dir = output_dir
+        self.colname_code = colname_code
+        self.window_orientation = window_orientation
+        self.window_radius_in_days = window_radius_in_days
+        self.matrix_type = matrix_type
+        self.backend = backend
+        self.d = d
+        self.smoothing_factor = smoothing_factor
+        self.k = k
+        self.n_min_events = n_min_events
+        self.colname_demographics = colname_demographics
+        self.decay_half_life_in_days = decay_half_life_in_days
+
+    def fit(
+        self,
+        X: pd.DataFrame,
+        y: pd.DataFrame = None,
+        vocabulary: List[str] = None,
+        static_features: List[str] = None,
+    ):
+        X_event = self.event.merge(
+            X[[COLNAME_PERSON]], on=COLNAME_PERSON, how="inner"
+        )
+        self.static_features_ = static_features
+        if vocabulary is None:
+            self.vocabulary_ = build_vocabulary(
+                event=X_event,
+                n_min_events=self.n_min_events,
+            )
+        else:
+            self.vocabulary_ = vocabulary
+        restricted_event = restrict_to_vocabulary(
+            event=X_event,
+            vocabulary=self.vocabulary_,
+        )
+        embedding = event2vec(
+            events=restricted_event,
+            output_dir=self.output_dir,
+            colname_concept=self.colname_code,
+            window_radius_in_days=self.window_radius_in_days,
+            window_orientation=self.window_orientation,
+            matrix_type=self.matrix_type,
+            backend=self.backend,
+            d=self.d,
+            smoothing_factor=self.smoothing_factor,
+            k=self.k,
+        )
+        for v in self.vocabulary_:
+            if v not in embedding.columns:
+                embedding[v] = np.zeros(shape=embedding.shape[0])
+        # order the columns to correspond to the vocabulary.
+        self.embedding_ = embedding[self.vocabulary_]
+        return self
+
+    def transform(self, X: pd.DataFrame) -> np.array:
+        # passing the person ids is necessary to aligne make_counts aggregated
+        # rows with the person ids in y.
+        X_event = self.event.merge(
+            X[[COLNAME_PERSON]], on=COLNAME_PERSON, how="inner"
+        )
+        X_counts = make_counts(
+            event=X_event,
+            person_id=X[[COLNAME_PERSON]],
+            decay_half_life_in_days=self.decay_half_life_in_days,
+            vocabulary=self.vocabulary_,
+            sparse=True,
+        )
+        embedding_array_ = sp.csr_matrix(
+            self.embedding_[self.vocabulary_].values
+        )
+
+        embedding_accumulator = [embedding_array_.transpose()] * len(
+            self.decay_half_life_in_days
+        )
+        embedding_repeated = sp.block_diag(embedding_accumulator)
+        X_embedded = X_counts.dot(embedding_repeated)
+        X_embedded = X_embedded.toarray()
+
+        X_embedded_columns = []
+        embedding_dimension = embedding_array_.shape[0]
+        for decay_ in self.decay_half_life_in_days:
+            for i in range(embedding_dimension):
+                X_embedded_columns.append(f"dim_{i}__decay_{decay_}")
+        X_embedded_df = pd.DataFrame(X_embedded, columns=X_embedded_columns)
+        if self.static_features_ is not None:
+            X_embedded_df = pd.concat(
+                [X[self.static_features_], X_embedded_df], axis=1
+            )
+        return X_embedded_df
+
+
+class Event2vecPretrained(Event2vecFeaturizer):
+    def __init__(
+        self,
+        event: pd.DataFrame,
+        path2embedding: str,
+        colname_demographics: str = None,
+        colname_code: str = COLNAME_SOURCE_CODE,
+        n_min_events: int = 10,
+        decay_half_life_in_days: np.array = np.array([0]),
+    ) -> None:
+        self.event = event
+        self.path2embedding = path2embedding
+        self.colname_code = colname_code
+        self.n_min_events = n_min_events
+        self.colname_demographics = colname_demographics
+        self.decay_half_life_in_days = decay_half_life_in_days
+        self.embedding = pd.read_parquet(self.path2embedding)
+
+    def fit(
+        self,
+        X: pd.DataFrame,
+        y: pd.DataFrame = None,
+        vocabulary: List[str] = None,
+        static_features: List[str] = None,
+    ):
+        X_event = self.event.merge(
+            X[[COLNAME_PERSON]], on=COLNAME_PERSON, how="inner"
+        )
+        self.static_features_ = static_features
+        if vocabulary is None:
+            vocabulary = build_vocabulary(
+                event=X_event,
+                n_min_events=self.n_min_events,
+            )
+        self.vocabulary_ = list(
+            set(self.embedding.columns).intersection(set(vocabulary))
+        )
+        #
+        self.embedding_ = self.embedding
+        return self
+
+
+## Utils ##
+def build_vocabulary(
+    event: pd.DataFrame,
+    colname_code: str = COLNAME_SOURCE_CODE,
+    n_min_events: int = 10,
+) -> List:
+    n_event_by_code = (
+        event[colname_code]
+        .value_counts()
+        .to_frame(name="n_events")
+        .reset_index()
+        .rename(columns={"index": colname_code})
+    )
+    restricted_codes = n_event_by_code[
+        n_event_by_code["n_events"] >= n_min_events
+    ]
+    return restricted_codes[colname_code].values
 
 
-def join_lists(list_2d: List[List[str]]) -> List[str]:
-    return list(chain(*list_2d))
+def restrict_to_vocabulary(
+    event: pd.DataFrame,
+    vocabulary: List,
+    colname_code: str = COLNAME_SOURCE_CODE,
+) -> pd.DataFrame:
+    restricted_event = event.merge(
+        pd.DataFrame(vocabulary, columns=[colname_code]),
+        on=colname_code,
+        how="inner",
+    )
+    return restricted_event
 
 
-WINDOW_CENTER_LABEL = "center"
-WINDOW_BACKWARD_LABEL = "backward"
+def get_feature_sparsity(X: np.array):  # pragma: no cover
+    return (X == 0).sum() / (X.shape[0] * X.shape[1])
 
 
-def _get_window(radius_in_days: float, window_orientation: str, backend: str):
-    """Create the window context for the cooccurrence matrix, adapted for each
-    backend: in days for pandas, in seconds for spark.
+def _assert_event_columns(
+    event: pd.DataFrame, other_required_columns: List[str] = None
+):
+    """Check that the event table has the required columns.
 
     Args:
-        radius_in_days (float): _description_
-        window_orientation (str): _description_
-        backend (str): Either pandas or spark
+        event (pd.DataFrame): _description_
+        other_required_columns (List[str], optional): _description_. Defaults to None.
 
     Raises:
         ValueError: _description_
-
-    Returns:
-        _type_: _description_
-    """
-    if backend == "spark":
-        # timesecond are necessary for the window function of spark
-        radius_ = days_to_seconds(radius_in_days)
-        # chose window orientation
-    elif backend == "pandas":
-        # radius_ = pd.to_timedelta(radius_in_days, unit="d")
-        radius_ = radius_in_days
-    if window_orientation == WINDOW_CENTER_LABEL:
-        window_start = -radius_ / 2
-        window_end = radius_ / 2
-    elif window_orientation == WINDOW_BACKWARD_LABEL:
-        window_start = -radius_
-        window_end = 0
-    else:
-        raise ValueError(
-            f"Choose window_orientation in {[WINDOW_CENTER_LABEL, WINDOW_BACKWARD_LABEL]}"
-        )
-    if backend == "spark":
-        window_start = int(window_start)
-        window_end = int(window_end)
-    return window_start, window_end
-
-
-def build_cooccurrence_matrix_pd(
-    events: DataFrame,
-    output_dir: str = None,
-    radius_in_days: int = 30,
-    window_orientation: str = "center",
-    colname_concept: str = "event_source_concept_id",
-) -> Tuple[np.array, np.array, Dict]:
-    """
-    Pandas method for building the cooccurrence matrix in-memory.
-
-    Parameters
-    ----------
-    events : DataFrame
-        _description_
-    output_dir : str, optional
-        _description_, by default None
-    radius_in_days : int, optional
-        _description_, by default 30
-    window_orientation : str, optional
-        _description_, by default "center"
-    colname_concept : str, optional
-        _description_, by default "event_source_concept_id"
-
-    Returns
-    -------
-    Tuple[np.array, np.array, Dict]
-        _description_
     """
-    window_start, window_end = _get_window(
-        radius_in_days=radius_in_days,
-        window_orientation=window_orientation,
-        backend="pandas",
-    )
-    window = window_end - window_start
-    if window_orientation == WINDOW_CENTER_LABEL:
-        center = True
-    elif window_orientation == WINDOW_BACKWARD_LABEL:
-        center = False
-    else:
+    expected_columns = [COLNAME_PERSON, COLNAME_SOURCE_CODE, COLNAME_START]
+    if other_required_columns is not None:
+        expected_columns += other_required_columns
+    missing_columns = set(expected_columns).difference(set(event.columns))
+    if len(missing_columns) > 0:
         raise ValueError(
-            f"Choose window_orientation in {[WINDOW_CENTER_LABEL, WINDOW_BACKWARD_LABEL]}"
+            f"Missing columns {missing_columns} in the event table."
         )
-    events_sorted = events.sort_values(["person_id", "start"])
-    events_in_window = events_sorted.groupby("person_id")[
-        [colname_concept, "start"]
-    ].rolling(
-        on="start", window=str(window) + "D", center=center, closed="both"
-    )
-    sep_tok = "<SEP>"
-    windowed_events = [
-        sep_tok.join(w.tolist()) for w in events_in_window[colname_concept]
-    ]
-    # TODO: we can do better than joining the word and then making the
-    # countvectorizer split them. Eg. build a dummy analyzer that does nothing
-    transformer = CountVectorizer(analyzer=lambda x: x.split(sep_tok))
-    logger.info("Fit, transform events with count vectorizer model")
-    sparse_counts = transformer.fit_transform(windowed_events)
-    logger.info(f"Vocabulary of length {len(transformer.vocabulary_)}")
-    encoder = transformer.vocabulary_
-    decoder = transformer.get_feature_names()
-    vocabulary_size = len(encoder.keys())
-    # TODO: is it less efficient than a join ?
-    context_encoded = (
-        events_sorted[colname_concept].apply(lambda x: encoder[x]).values
-    )
-    n_words = sparse_counts.sum(axis=0)
-    n_contexts = np.unique(context_encoded, return_counts=True)[1]
-    # use ultra fast sparse matrix product
-    rows = np.arange(len(context_encoded))
-    cols = context_encoded
-    values = np.ones(len(context_encoded))
-    context_matrix = csr_matrix(
-        (values, (rows, cols)),
-        shape=(len(context_encoded), vocabulary_size),
-    ).transpose()
-    sparse_cooccurrence = context_matrix.dot(sparse_counts)
-    # Have to withdraw the diagonal to avoid double counting
-    cooccurrence_matrix = sparse_cooccurrence - csr_matrix(np.diag(n_contexts))
-    if output_dir is not None:
-        logger.info(
-            f"Saving coocurrence_matrix, event_count and vocabulary at {output_dir}"
-        )
-        Path(output_dir).mkdir(parents=True, exist_ok=True)
-        path2matrix = str(Path(output_dir) / "sparse_matrix.npz")
-        logger.info(f"Saving cooccurrence matrix as parquet at: {path2matrix}")
-        save_npz(path2matrix, cooccurrence_matrix)
-        with open(os.path.join(output_dir, "vocabulary.json"), "w") as file:
-            json.dump(encoder, file)
-        np.save(os.path.join(output_dir, "event_count.npy"), n_contexts)
-    return cooccurrence_matrix, n_contexts, encoder
-
-
-def build_cooccurrence_matrix_spark(
-    events: DataFrame,
-    output_dir: str = None,
-    radius_in_days: int = 30,
-    window_orientation: str = "center",
-    matrix_type: str = "numpy",
-    colname_concept: str = "event_source_concept_id",
-) -> Tuple[np.array, np.array, Dict]:
-    """
-    Description: Leverage spark backend to compute cooccurrence matrix for an
-    event table.
 
-    :param events: event dataframe
-    :param output_dir:
-    :param radius_in_days: size of the context window in days, this is to be thought as the radius
-    around the central word of reference. Depending of the orientation of the window, the size of
-    window will be 2 * radius_in_days if centered
-    :param window_orientation: choose position of the reference word in the context window:
-        ['centered', 'future'], this changes the focus of the co-occurrence matrix.
-        NB : The future configuration leads to an asymetric cooccurrence matrix.
-    :param matrix_type:
-    :return:
-        - cooccurrence_matrix, matrix of cooccurrence of size VxV  where V is the vocabulary size
-         with M[i, j] = #|i and j occurs in a window of size window_in_days|
-        - event_count, array of size V with the number of single occurrence of each word
-        - label2ix, dictionary of size V giving the correspondence between a word and its index in
-        the matrix
-    """
 
-    window_start, window_end = _get_window(
-        radius_in_days=radius_in_days,
-        window_orientation=window_orientation,
-        backend="spark",
-    )
-    # little hack of the rangeBetween function
-    w = (
-        Window.partitionBy("person_id")
-        .orderBy(func.col("start").cast("long"))
-        .rangeBetween(window_start, window_end)
-    )
-    events_in_window = events.withColumn(
-        "cooccurrence", func.collect_list(func.col(colname_concept)).over(w)
-    )
+# function tested in the test_experiences.py
+def make_counts(
+    event: pd.DataFrame,
+    person_id: pd.DataFrame,
+    decay_half_life_in_days: np.array = np.array([0, 7]),
+    vocabulary: List[str] = None,
+    sparse: bool = True,
+) -> Union[np.array, sp.csr_matrix]:  # pragma: no cover
+    """Count the event by person and by code with an option to weigth
+    exponentially the counts with respect to the start of followup date.
 
-    codes_vectorizer = ml_feature.CountVectorizer(
-        inputCol="cooccurrence", outputCol="cooccurrence_ohe", minDF=0
-    )
+    The exponential decay is parametrized by a half-life.
 
-    logger.info("Fit count vectorizer model")
-    codes_vectorizer_model = codes_vectorizer.fit(events_in_window)
-    logger.info(
-        "Vocabulary of length {}".format(
-            len(codes_vectorizer_model.vocabulary)
-        )
-    )
-    logger.info("Transform events with count vectorizer model")
-    events_ohe = codes_vectorizer_model.transform(events_in_window)
-    label2ix = {
-        label: i
-        for (label, i) in zip(
-            codes_vectorizer_model.vocabulary,
-            range(len(codes_vectorizer_model.vocabulary)),
-        )
-    }
-    # adding ix for future reduced key
-    mapping_expr = func.create_map(
-        [func.lit(x) for x in chain(*label2ix.items())]
-    )
-    events_ohe_with_ix = events_ohe.withColumn(
-        "ix", mapping_expr.getItem(func.col(colname_concept)).cast("int")
-    )
-    # sort by item ix and get back raw counts (suppres
-    # s item ignored by count vectorizer)
-    event_count = np.array(
-        events_ohe_with_ix.groupBy("ix")
-        .count()
-        .filter(~func.col("ix").isNull())
-        .sort(func.col("ix"))
-        .drop("ix")
-        .collect()
-    ).reshape(-1)
-
-    # aggregate one line per item and sort by item index
-    events_ohe_grouped = (
-        events_ohe_with_ix.select("ix", "cooccurrence_ohe")
-        .rdd.mapValues(lambda v: v.toArray())
-        .reduceByKey(lambda x, y: x + y)
-        .mapValues(lambda x: DenseVector(x))
-        .toDF(["ix", "cooccurrence_ohe"])
-    )
-    # remove excluded code from count_vectorizer and sort by ix
-    events_ohe_grouped_sorted = events_ohe_grouped.filter(
-        ~func.col("ix").isNull()
-    ).sort(func.col("ix").asc())
-    # collect and reshape the cooccurrence matrix
-    if matrix_type == "numpy":
-        logger.info("Collect co-occurrence matrix as numpy")
-        x_3d = np.array(
-            events_ohe_grouped_sorted.select("cooccurrence_ohe").collect()
-        )
-        rows, idx, vocab_size = x_3d.shape
-        # Have to withdraw the diagonal to avoid double counting
-        cooccurrence_matrix = x_3d.reshape(rows, rows) - np.diag(event_count)
-
-    elif matrix_type == "parquet":
-        # user = os.getenv("USER")
-        # hdfs_path +
-        # hdfs_path = f"hdfs://bbsedsi/user/{user}/"
-        spark = SparkSession.builder.getOrCreate()
-        path2spark_matrix = str(output_dir) + "/spark_matrix.parquet"
-
-        logger.info(f"Saving cooccurrence matrix at: {path2spark_matrix}")
-        events_ohe_grouped_sorted.write.mode("overwrite").parquet(
-            path2spark_matrix
-        )
-        logger.info(f"Saving event count at: {path2spark_matrix}")
-
-        spark.createDataFrame(
-            pd.DataFrame({"event_count": event_count})
-        ).write.mode("overwrite").parquet(
-            str(output_dir) + "/event_count.parquet"
-        )
-        # TODO: could ty to use [spark.ml.sparse to create sparse
-        # matrix](https://spark.apache.org/docs/latest/mllib-dimensionality-reduction.html#svd-example)
-        # https://spark.apache.org/docs/latest/api/java/org/apache/spark/ml/linalg/SparseMatrix.html
-
-        # The cooccurrence matrix has to be sorted because it has been saved
-        # with random row order depending on the workers.
-        matrix_before_stacking = spark.read.parquet(path2spark_matrix).sort(
-            "ix"
-        )
-        cooccurrence_matrix = np.vstack(
-            matrix_before_stacking.toPandas()["cooccurrence_ohe"].values
-        ) - np.diag(event_count)
-    else:
-        raise NotImplementedError(
-            "Matrix collection should be either numpy or parquet"
-        )
+    Args:
+        event (pd.DataFrame): _description_
+        colname_code (str, optional): _description_. Defaults to COLNAME_SOURCE_CODE.
+        decay_half_life_in_days (List[int], optional): _description_. Defaults to [0, 7].
+        vocabulary (str, optional): _description_. Defaults to None.
+        batch (int, optional): Allow to batch the . Defaults to 5000.
+    Raises:
+        ValueError: _description_
 
-    if output_dir is not None:
-        logger.info(
-            f"Saving coocurrence_matrix, event_count and vocabulary at {output_dir}"
-        )
-        Path(output_dir).mkdir(parents=True, exist_ok=True)
-        with open(Path(output_dir) / "vocabulary.json", "w") as file:
-            json.dump(label2ix, file)
-        np.save(
-            Path(output_dir) / "cooccurrence_matrix.npy",
-            cooccurrence_matrix,
+    Returns:
+        Tuple(
+            Features: _description_,
+            person: _description_
         )
-        np.save(Path(output_dir) / "event_count.npy", event_count)
-    return cooccurrence_matrix, event_count, label2ix
-
-
-def sparse_to_array(v):
-    """
-    Description: udf to transform to dense vector spark sparse vector
-    :param v:
-    :return:
-    """
-    v = DenseVector(v)
-    new_array = list([float(x) for x in v])
-    return new_array
-
-
-def build_ppmi(
-    cooccurrence_matrix: np.array,
-    event_count: np.array,
-    smoothing_factor: float = 0.75,
-    k: int = 1,
-) -> np.array:
-    """
-    Description: Build the pmi matrix from the cooccurrence matrix M:
-    $$pmi = log[\frac{p(w,c)}{p(w)p(c)}]$$
-    # Take the raw item count as the Z denominator
-    # We might try some large definition of context where we throws up from the denominator
-    # all self-cooccurrence (ie windows of size 1 with an item alone)
-    # Our lines/columns do not sum to 1 because we exclude the column where there are counts of
-    # the line item co-occurring with the same occurrence of itself.
-    # The diagonal corresponds only to co-occurrences of the item with a different occurrence of
-    # itself.
-    :param cooccurrence_matrix:
-    :param item_count:
-    :param smoothing_factor:
-    :param k: shift value, default 1 which is log(1) = 0 shift.
-    :return:
     """
 
-    total_event_count = event_count.sum()
-    cooccurrence_ratio = cooccurrence_matrix / total_event_count
-    item_ratio = (event_count / total_event_count) ** smoothing_factor
-    inverse_item_ratio = 1 / item_ratio
-    pmi_matrix = np.log(
-        cooccurrence_ratio * np.outer(inverse_item_ratio, inverse_item_ratio)
-    )
-    ppmi = pmi_matrix - np.log(k)
-    ppmi[ppmi <= 0] = 0
-
-    return ppmi
-
-
-def build_embeddings(
-    ppmi: np.array, d: int, window_orientation="center", sparse: bool = True
-):
-    """
-    TODO should use pyspark.mlib if the matrix is too big for numpy
-    Description: perform symetric singular value reconstruction
-    :param window_orientation: choose position of the reference word in the context window:
-        ['centered', 'future'], this changes the focus of the co-occurrence matrix.
-        NB : The future configuration leads to an asymetric cooccurrence matrix.
-    :param ppmi:
-    :param d:
-    :return:
-    """
-    if window_orientation == WINDOW_CENTER_LABEL:
-        pass
-    elif window_orientation == WINDOW_BACKWARD_LABEL:
-        # TODO: I think that the symetrization is not necessary. A symmetric ppmi means word and context
-        # embeddings are the same. We could use different ones.
-        # Symetrization of the cooccurrence matrix
-        ppmi = (ppmi + np.transpose(ppmi)) / 2
-    else:
-        raise ValueError(
-            f"Choose window_orientation in {[WINDOW_CENTER_LABEL, WINDOW_BACKWARD_LABEL]}"
-        )
-    if d > ppmi.shape[0]:
-        raise Exception(
-            "Continuous vector dimension should be lower than vocabulary size!"
-        )
-    # TODO: Why not using [sklearn truncated
-    # svd ?](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.TruncatedSVD.html)
-
+    _assert_event_columns(
+        event, other_required_columns=[COLNAME_FOLLOWUP_START]
+    )
+
+    if vocabulary is None:
+        vocabulary = event[COLNAME_SOURCE_CODE].value_counts().index.values
+    X_accumulator = []
+    event[COLNAME_VALUE] = 1
+    event = person_id[[COLNAME_PERSON]].merge(
+        event,
+        on=COLNAME_PERSON,
+        how="inner",
+    )
+    event["delta_to_followup"] = (
+        pd.to_datetime(event[COLNAME_FOLLOWUP_START])
+        - pd.to_datetime(event[COLNAME_START])
+    ).astype("timedelta64[D]")
+    for half_life in decay_half_life_in_days:
+        if half_life < 0:
+            raise ValueError(f"half_life should be positive, got {half_life}")
+        # not necessary to set as a variable
+        if half_life > 0:
+            event[COLNAME_VALUE] = np.exp(
+                -event["delta_to_followup"] / half_life
+            )
+        decayed_X = get_event_aggregation(
+            event=event,
+            aggregation_periods="100",
+            aggregation_functions=[sum],
+            aggregation_col=COLNAME_PERSON,
+            vocabulary=vocabulary,
+            eps=0,
+        )
+        decayed_X.columns = [
+            col.replace("__sum__p100", "") for col in decayed_X.columns
+        ]
+        decayed_X = decayed_X[vocabulary]
+        decayed_X.columns = [
+            col + f"_count_decay_{half_life}" for col in decayed_X.columns
+        ]
+        # size N x vocabulary
+        decayed_X_aligned = (
+            person_id[[COLNAME_PERSON]]
+            .merge(decayed_X, on=COLNAME_PERSON, how="left")
+            .fillna(0)
+            .set_index(COLNAME_PERSON)
+        )
+        if sparse:
+            decayed_X_aligned = sp.csr_matrix(decayed_X_aligned)
+        X_accumulator.append(decayed_X_aligned)
     if sparse:
-        sparse_ppmi = csr_matrix(ppmi)
-        u_d, s_d, v_d = svds(sparse_ppmi, k=d)
+        X = sp.hstack(X_accumulator)
     else:
-        u, s, v = np.linalg.svd(ppmi)
-        u_d = u[:, :d]
-        v_d = v[:d, :]
-        s_d = s[:d]
-    embeddings = u_d.dot(np.diag(np.sqrt(s_d))) + v_d.transpose().dot(
-        np.diag(np.sqrt(s_d))
-    )
+        X = np.concatenate(X_accumulator, axis=1)
+    return X
 
-    return embeddings
 
+PERIOD_MAP = {"all": [100, 10, 25, 50, -10, -25, -50], "100": [100]}
 
-def event2vec(
-    events=DataFrame,
-    output_dir: str = None,
-    colname_concept: str = "event_source_concept_id",
-    window_radius_in_days=30,
-    window_orientation: str = "center",
-    matrix_type: str = "numpy",
-    backend="pandas",
-    d: int = 300,
-    smoothing_factor: float = 0.75,
-    k: int = 1,
-):
+
+def get_event_aggregation(
+    event: pd.DataFrame,
+    aggregation_periods: str = "100",
+    aggregation_functions: List = None,
+    aggregation_col: str = COLNAME_PERSON,
+    vocabulary: List[str] = None,
+    eps=1e-6,
+) -> pd.DataFrame:
     """
-    Wrapper around build_cooccurrence_matrix, build_ppmi and build_embeddings to
-    create concept embeddings from raw event codes.
+    Compute aggregate statistics by patient trajectory and chosen events over
+    different subsequences of the stay
 
-    Args:
-        events (_type_, optional): _description_. Defaults to DataFrame.
-        output_dir (str, optional): _description_. Defaults to None.
-        colname_concept (str, optional): _description_. Defaults to
-        "event_source_concept_id". window_radius_in_days (int, optional):
-        _description_. Defaults to 30. window_orientation (str, optional):
-        _description_. Defaults to "centered". matrix_type (str, optional):
-        _description_. Defaults to "numpy". d (int, optional): _description_.
-        Defaults to 300. smoothing_factor (float, optional): _description_.
-        Defaults to 0.75. k (int, optional): _description_. Defaults to 1.
 
-    Raises:
-        ValueError: _description_
+    Parameters
+    ----------
+    event : pd.DataFrame
+        _description_
+    aggregation_periods : str, optional
+        _description_, by default "all"
+    aggregation_functions : List, optional
+        _description_, by default None
+    aggregation_col : str, optional
+        By default, aggregate on COLNAME_PERSON, but could change the key.
+    vocabulary : str, optional
+        Details the code vocabulary taken into account, by default None so it is computed over all codes.
+    eps : _type_, optional
+        _description_, by default 1e-6
 
-    Returns:
-        _type_: _description_
+    Returns
+    -------
+    pd.DataFrame
+        _description_
     """
-    if backend == "spark":
-        (
-            cooccurrence_matrix,
-            event_count,
-            label2ix,
-        ) = build_cooccurrence_matrix_spark(
-            events,
-            output_dir=output_dir,
-            radius_in_days=window_radius_in_days,
-            colname_concept=colname_concept,
-            matrix_type=matrix_type,
-        )
-    elif backend == "pandas":
-        (
-            cooccurrence_matrix,
-            event_count,
-            label2ix,
-        ) = build_cooccurrence_matrix_pd(
-            events,
-            output_dir=output_dir,
-            radius_in_days=window_radius_in_days,
-            colname_concept=colname_concept,
-        )
-    if window_orientation not in [WINDOW_BACKWARD_LABEL, WINDOW_CENTER_LABEL]:
-        raise ValueError(
-            f"Choose window_orientation in {[WINDOW_BACKWARD_LABEL, WINDOW_CENTER_LABEL]}"
-        )
-    t_0 = datetime.now()
-    logger.info(
-        f"Shape of the co-occurrence matrix: {cooccurrence_matrix.shape}"
-    )
-    logger.info(
-        f"Build PPMI with smoothing factor {smoothing_factor} and shift {k}"
-    )
-    ppmi = build_ppmi(
-        cooccurrence_matrix=cooccurrence_matrix,
-        event_count=event_count,
-        smoothing_factor=smoothing_factor,
-        k=k,
-    )
-    logger.info("PPMI factorization with SVD")
-    event_embeddings = build_embeddings(
-        ppmi=ppmi, d=d, window_orientation=window_orientation
+    _assert_event_columns(
+        event, other_required_columns=[COLNAME_VALUE, aggregation_col]
     )
-    t_1 = datetime.now()
-    logger.info(
-        f"Embeddings of dimension {d} created from the co-occurrence matrix in {t_1 - t_0}"
-    )
-    embeddings_dict = dict(zip(label2ix.keys(), np.array(event_embeddings)))
-
-    embeddings_df = pd.DataFrame.from_dict(embeddings_dict, orient="columns")
-    if output_dir is not None:
-        path2emb = (
-            output_dir
-            / f"tuto_snds2vec_alpha={smoothing_factor}_k={k}_d={d}.parquet"
-        )
-        logger.info(f"Saving embeddings as parquet dataframe at {path2emb}")
-        embeddings_df.to_parquet(path2emb)
-    return embeddings_df
+    # TODO: truncation time should be computed from events
+    if aggregation_periods not in PERIOD_MAP.keys():
+        raise ValueError(f"Supported aggregation periods are {PERIOD_MAP}")
+    fake_lines = []
+
+    # need to fill the value for end of events
+    if vocabulary is not None:
+        code_whitelist = vocabulary.copy()
+        event_restricted = restrict_to_vocabulary(
+            event=event, vocabulary=code_whitelist
+        )
+    else:
+        code_whitelist = event[COLNAME_SOURCE_CODE].value_counts().index.values
+        event_restricted = event
+    for code in code_whitelist:
+        fake_line = event.iloc[0].copy()
+        fake_line[COLNAME_PERSON] = -1
+        fake_line[COLNAME_SOURCE_CODE] = code
+        fake_lines.append(fake_line)
+    # pandas magic: the casting is necessary to avoid type error in the groupby operation
+    fake_lines = pd.concat(fake_lines, axis=1).transpose()
+    if aggregation_functions is None:
+        aggregation_functions = [np.min, np.max, np.mean, np.std, len]
+        statistics_names = ["min", "max", "mean", "std", "skew", "count"]
+    elif type(aggregation_functions) == list:
+        statistics_names = [func.__name__ for func in aggregation_functions]
+    statistics_agg = [
+        pd.NamedAgg(COLNAME_VALUE, func) for func in aggregation_functions
+    ]
+    statistics_dict = dict(zip(statistics_names, statistics_agg))
+    periods = PERIOD_MAP[aggregation_periods]
+    for sub_period in periods:
+        if (sub_period <= -100) | (sub_period > 100):
+            raise ValueError(
+                f"period is a percentage and should be in ]-100, 100], got {sub_period}"
+            )
+    # add the delta observation as the difference between first and last
+    # event observed by person
+    first_event_datetime = (
+        event_restricted.sort_values(COLNAME_START)
+        .groupby(aggregation_col)
+        .agg(**{OBSERVATION_START: pd.NamedAgg(COLNAME_START, "first")})
+        .reset_index()
+    )
+    last_event_datetime = (
+        event_restricted.sort_values(COLNAME_START)
+        .groupby(aggregation_col)
+        .agg(**{OBSERVATION_END: pd.NamedAgg(COLNAME_START, "last")})
+        .reset_index()
+    )
+    events_of_interest = event_restricted.merge(
+        first_event_datetime, on=aggregation_col, how="inner"
+    ).merge(last_event_datetime, on=aggregation_col, how="inner")
+
+    events_of_interest["observation_delta"] = (
+        events_of_interest[OBSERVATION_END]
+        - events_of_interest[OBSERVATION_START]
+    ).astype("timedelta64[s]")
+    X = []
+    for sub_period in periods:
+        logger.info(f"Computing period {sub_period}")
+        events_of_interest["period_span_second"] = (
+            events_of_interest["observation_delta"] * sub_period / 100
+        )
+        if sub_period >= 0:
+            mask = (
+                (
+                    pd.to_datetime(events_of_interest[COLNAME_START])
+                    - pd.to_datetime(events_of_interest[OBSERVATION_START])
+                ).astype("timedelta64[s]")
+                >= -eps
+            ) & (
+                (
+                    pd.to_datetime(events_of_interest[COLNAME_START])
+                    - pd.to_datetime(events_of_interest[OBSERVATION_START])
+                ).astype("timedelta64[s]")
+                <= (events_of_interest["period_span_second"] + eps)
+            )
+        else:
+            mask = (
+                (
+                    pd.to_datetime(events_of_interest[COLNAME_START])
+                    - pd.to_datetime(events_of_interest[OBSERVATION_START])
+                ).astype("timedelta64[s]")
+                >= (
+                    (
+                        events_of_interest["observation_delta"]
+                        + events_of_interest["period_span_second"]
+                    )
+                    - eps
+                )
+            ) & (
+                (
+                    pd.to_datetime(events_of_interest[COLNAME_START])
+                    - pd.to_datetime(events_of_interest[OBSERVATION_END])
+                ).astype("timedelta64[s]")
+                <= eps + events_of_interest["observation_delta"]
+            )
+        period_events = events_of_interest.loc[mask, :]
+        period_events = pd.concat((period_events, fake_lines), axis=0)
+        period_statistics = (
+            period_events.groupby(by=[aggregation_col, COLNAME_SOURCE_CODE])
+            .agg(**statistics_dict)
+            .reset_index()
+        )
+        col_names = period_statistics[COLNAME_SOURCE_CODE].unique()
+        period_statistics = period_statistics.pivot(
+            index=aggregation_col,
+            columns=COLNAME_SOURCE_CODE,
+            values=statistics_names,
+        )
+        period_statistics.columns = np.array(
+            [
+                [
+                    col + "__" + stat_name + "__" + f"p{sub_period}"
+                    for col in col_names
+                ]
+                for stat_name in statistics_names
+            ]
+        ).flatten()
+        X.append(period_statistics)
+    X = pd.concat(X, axis=1)
+    return X.drop(-1, axis=0, errors="ignore")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `event2vec-0.0.1/pyproject.toml` & `event2vec-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "event2vec"
-version = "0.0.1"
+version = "0.0.3"
 description = "event2vec"
 authors = ["Matthieu Doutreligne <matt.dout@gmail.com>"]
 license = "EUPL-v1.2"
 readme = "README.md"
 repository = "https://gitlab.com/strayMat/event2vec"
 homepage = "https://gitlab.com/strayMat/event2vec"
 include = ["bin"]
@@ -14,48 +14,51 @@
 keywords = []
 classifiers = [
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 # [tool.poetry.urls]
 # Changelog = "https://gitlab.com/strayMat/event2vec/releases"
 
 [tool.poetry.dependencies]
-python = ">=3.7.1,<3.8"
+python = ">=3.7.1,<3.11"
 
 # Project-Specific
 python-dotenv = "^0.15.0"
 jedi = "^0.18.1"
-pandas = ">=1.3.0, <2.0.0"
-pyarrow = "0.17.0"
-numpy = ">=1.0.0, <1.20"
-#pyspark = "2.4.3" # unsolved strange error at install time, pip install afterwards
-tabulate = "^0.8.10"
+pandas = ">=1.3.0"
+pyarrow = ">=0.17.0"
+numpy = ">=1.0.0"
+# pyspark installation yields unsolved strange error with poetry,
+# it is advised to pip install this depency after a poetry install
+pyspark = { version = "2.4.3", optional = true, python = ">=3.7.1, <3.8"}
 loguru = "^0.6.0"
 matplotlib = "^3.5.0"
 plotly = "^5.11.0"
-scikit-learn = "1.0"
+scikit-learn = "^1.0"
 fastparquet = "^0.8.1"
 
 # Documentation
 importlib-metadata = { version = "^4.11.3", optional = true }
 pygments = { version = "^2.11.2", optional = true }
 sphinx = { version = "^4.4.0", optional = true }
 sphinx-autodoc-typehints = { version = "^1.17.0", optional = true }
 pydata-sphinx-theme = { version = "^0.8.0", optional = true }
 sphinxcontrib-apidoc = { version = "^0.3.0", optional = true }
 sphinx-click = { version = "^3.1.0", optional = true }
 myst-nb = {version = "^0.17.1", optional = true}
+tabulate = "^0.9.0"
 
 
 [tool.poetry.dev-dependencies]
 # Testing
 pytest = "^7.1.1"
 pytest-cov = "^3.0.0"
 pytest-mock = "^3.7.0"
@@ -85,15 +88,17 @@
     "sphinx",
     "sphinx-autodoc-typehints",
     "pydata-sphinx-theme",
     "sphinxcontrib-apidoc",
     "sphinx-click",
     "jinja2"
 ]
-
+spark = [
+    "spark"
+]
 
 [tool.poetry.scripts]
 cli = "bin.cli:cli"
 
 #################################################################################
 # Tooling configs                                                               #
 #################################################################################
@@ -157,13 +162,13 @@
 log_cli_level = "ERROR"
 log_cli_format = "%(message)s"
 log_file = "pytest.log"
 log_file_level = "INFO"
 log_file_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_file_date_format = "%Y-%m-%d %H:%M:%S"
 
-#[build-system]
-#requires = ["poetry-core>=1.0.0"]
-#build-backend = "poetry.core.masonry.api"
 [build-system]
-requires = ["setuptools>=40.8.0", "wheel"]
-build-backend = "setuptools.build_meta:__legacy__"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+#[build-system]
+#requires = ["setuptools>=40.8.0", "wheel"]
+#build-backend = "setuptools.build_meta:__legacy__"
```

### Comparing `event2vec-0.0.1/PKG-INFO` & `event2vec-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 Metadata-Version: 2.1
 Name: event2vec
-Version: 0.0.1
+Version: 0.0.3
 Summary: event2vec
 Home-page: https://gitlab.com/strayMat/event2vec
 License: EUPL-v1.2
 Author: Matthieu Doutreligne
 Author-email: matt.dout@gmail.com
-Requires-Python: >=3.7.1,<3.8
+Requires-Python: >=3.7.1,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
+Provides-Extra: spark
 Requires-Dist: fastparquet (>=0.8.1,<0.9.0)
 Requires-Dist: importlib-metadata (>=4.11.3,<5.0.0) ; extra == "docs"
 Requires-Dist: jedi (>=0.18.1,<0.19.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: matplotlib (>=3.5.0,<4.0.0)
 Requires-Dist: myst-nb (>=0.17.1,<0.18.0) ; extra == "docs"
-Requires-Dist: numpy (>=1.0.0,<1.20)
-Requires-Dist: pandas (>=1.3.0,<2.0.0)
+Requires-Dist: numpy (>=1.0.0)
+Requires-Dist: pandas (>=1.3.0)
 Requires-Dist: plotly (>=5.11.0,<6.0.0)
-Requires-Dist: pyarrow (==0.17.0)
+Requires-Dist: pyarrow (>=0.17.0)
 Requires-Dist: pydata-sphinx-theme (>=0.8.0,<0.9.0) ; extra == "docs"
 Requires-Dist: pygments (>=2.11.2,<3.0.0) ; extra == "docs"
+Requires-Dist: pyspark (==2.4.3) ; python_full_version >= "3.7.1" and python_version < "3.8"
 Requires-Dist: python-dotenv (>=0.15.0,<0.16.0)
-Requires-Dist: scikit-learn (==1.0)
+Requires-Dist: scikit-learn (>=1.0,<2.0)
 Requires-Dist: sphinx (>=4.4.0,<5.0.0) ; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints (>=1.17.0,<2.0.0) ; extra == "docs"
 Requires-Dist: sphinx-click (>=3.1.0,<4.0.0) ; extra == "docs"
 Requires-Dist: sphinxcontrib-apidoc (>=0.3.0,<0.4.0) ; extra == "docs"
-Requires-Dist: tabulate (>=0.8.10,<0.9.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://gitlab.com/strayMat/event2vec
 Description-Content-Type: text/markdown
 
 # event2vec
 
 **Documentation**: [https://straymat.gitlab.io/event2vec/](https://straymat.gitlab.io/event2vec/)
 
@@ -50,17 +56,12 @@
 
 Electronic Health Record and claims contain sequences of care: every contact
 between a patient and a healthcare system (either hospital, either insurance) is
 recorded in a central database. Medical terminologies are often used to encode
 the type of care : diagnoses, acts, drugs, laboratory, ...
 
 Such healthcare trajectories can be viewed as sequence of tokens, similarly to
-sequences of words. Embeddings techniques .
+sequences of words.
 
 This package propose to use matrix factorization as a simple and efficient way
 to build event embedding from a medical observational database.
 
-
-## Features
-
-- TODO
-
```

