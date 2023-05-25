# Comparing `tmp/widefield_analysis-0.1.2.tar.gz` & `tmp/widefield_analysis-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widefield_analysis-0.1.2.tar", max compression
+gzip compressed data, was "widefield_analysis-0.1.3.tar", max compression
```

## Comparing `widefield_analysis-0.1.2.tar` & `widefield_analysis-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       55 2023-03-28 09:53:25.190532 widefield_analysis-0.1.2/README.md
--rw-r--r--   0        0        0      497 2023-05-17 10:08:31.435369 widefield_analysis-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 08:46:58.435982 widefield_analysis-0.1.2/widefield_analysis/__init__.py
--rw-r--r--   0        0        0     3364 2023-03-31 13:15:08.809441 widefield_analysis-0.1.2/widefield_analysis/animation.py
--rw-r--r--   0        0        0     4142 2023-05-10 08:26:55.916576 widefield_analysis-0.1.2/widefield_analysis/files.py
--rw-r--r--   0        0        0     1405 2023-03-28 09:06:15.591145 widefield_analysis-0.1.2/widefield_analysis/filter.py
--rw-r--r--   0        0        0      739 2023-03-31 09:51:47.977442 widefield_analysis-0.1.2/widefield_analysis/resample.py
--rw-r--r--   0        0        0      832 2023-03-28 09:15:07.411967 widefield_analysis-0.1.2/widefield_analysis/smooth.py
--rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 widefield_analysis-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-03-28 09:53:25.190532 widefield_analysis-0.1.3/README.md
+-rw-r--r--   0        0        0      497 2023-05-25 12:02:20.818385 widefield_analysis-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-28 08:46:58.435982 widefield_analysis-0.1.3/widefield_analysis/__init__.py
+-rw-r--r--   0        0        0     3364 2023-03-31 13:15:08.809441 widefield_analysis-0.1.3/widefield_analysis/animation.py
+-rw-r--r--   0        0        0     4142 2023-05-10 08:26:55.916576 widefield_analysis-0.1.3/widefield_analysis/files.py
+-rw-r--r--   0        0        0     1409 2023-05-25 11:53:43.138754 widefield_analysis-0.1.3/widefield_analysis/filter.py
+-rw-r--r--   0        0        0      739 2023-03-31 09:51:47.977442 widefield_analysis-0.1.3/widefield_analysis/resample.py
+-rw-r--r--   0        0        0      832 2023-03-28 09:15:07.411967 widefield_analysis-0.1.3/widefield_analysis/smooth.py
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 widefield_analysis-0.1.3/PKG-INFO
```

### Comparing `widefield_analysis-0.1.2/widefield_analysis/animation.py` & `widefield_analysis-0.1.3/widefield_analysis/animation.py`

 * *Files identical despite different names*

### Comparing `widefield_analysis-0.1.2/widefield_analysis/files.py` & `widefield_analysis-0.1.3/widefield_analysis/files.py`

 * *Files identical despite different names*

### Comparing `widefield_analysis-0.1.2/widefield_analysis/filter.py` & `widefield_analysis-0.1.3/widefield_analysis/filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     butterworth_filter = signal.butter(
         N=filter_order,
         Wn=[start_freq, end_freq],
         output="sos",
         btype="bandpass",
         fs=frame_rate,
     )
-    filtered_movie = signal.sosfilt(butterworth_filter, movie, axis=0)
+    filtered_movie = signal.sosfiltfilt(butterworth_filter, movie, axis=0)
     return filtered_movie
 
 
 def remove_high_frequencies(movie: np.ndarray, frame_rate: float, cutoff_freq: float, filter_order: int = 1) -> np.ndarray:
     """Remove high frequencies from movie."""
     butterworth_filter = signal.butter(
         N=filter_order,
```

### Comparing `widefield_analysis-0.1.2/widefield_analysis/resample.py` & `widefield_analysis-0.1.3/widefield_analysis/resample.py`

 * *Files identical despite different names*

### Comparing `widefield_analysis-0.1.2/widefield_analysis/smooth.py` & `widefield_analysis-0.1.3/widefield_analysis/smooth.py`

 * *Files identical despite different names*

### Comparing `widefield_analysis-0.1.2/PKG-INFO` & `widefield_analysis-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widefield-analysis
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Mathis
 Author-email: mathis.bassler@protonmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

