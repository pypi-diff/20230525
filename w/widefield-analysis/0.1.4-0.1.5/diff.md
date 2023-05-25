# Comparing `tmp/widefield_analysis-0.1.4.tar.gz` & `tmp/widefield_analysis-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widefield_analysis-0.1.4.tar", max compression
+gzip compressed data, was "widefield_analysis-0.1.5.tar", max compression
```

## Comparing `widefield_analysis-0.1.4.tar` & `widefield_analysis-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       55 2023-03-28 09:53:25.190532 widefield_analysis-0.1.4/README.md
--rw-r--r--   0        0        0      497 2023-05-25 12:17:00.863264 widefield_analysis-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 08:46:58.435982 widefield_analysis-0.1.4/widefield_analysis/__init__.py
--rw-r--r--   0        0        0     3364 2023-03-31 13:15:08.809441 widefield_analysis-0.1.4/widefield_analysis/animation.py
--rw-r--r--   0        0        0     2150 2023-05-25 12:16:10.303648 widefield_analysis-0.1.4/widefield_analysis/baseline.py
--rw-r--r--   0        0        0     3897 2023-05-25 12:06:22.820394 widefield_analysis-0.1.4/widefield_analysis/files.py
--rw-r--r--   0        0        0     1409 2023-05-25 11:53:43.138754 widefield_analysis-0.1.4/widefield_analysis/filter.py
--rw-r--r--   0        0        0      739 2023-03-31 09:51:47.977442 widefield_analysis-0.1.4/widefield_analysis/resample.py
--rw-r--r--   0        0        0      876 2023-05-25 12:06:23.564388 widefield_analysis-0.1.4/widefield_analysis/smooth.py
--rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 widefield_analysis-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-03-28 09:53:25.190532 widefield_analysis-0.1.5/README.md
+-rw-r--r--   0        0        0      497 2023-05-25 12:34:33.923034 widefield_analysis-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-28 08:46:58.435982 widefield_analysis-0.1.5/widefield_analysis/__init__.py
+-rw-r--r--   0        0        0     3364 2023-03-31 13:15:08.809441 widefield_analysis-0.1.5/widefield_analysis/animation.py
+-rw-r--r--   0        0        0     2293 2023-05-25 12:34:15.923177 widefield_analysis-0.1.5/widefield_analysis/baseline.py
+-rw-r--r--   0        0        0     3897 2023-05-25 12:06:22.820394 widefield_analysis-0.1.5/widefield_analysis/files.py
+-rw-r--r--   0        0        0     1409 2023-05-25 11:53:43.138754 widefield_analysis-0.1.5/widefield_analysis/filter.py
+-rw-r--r--   0        0        0      739 2023-03-31 09:51:47.977442 widefield_analysis-0.1.5/widefield_analysis/resample.py
+-rw-r--r--   0        0        0      876 2023-05-25 12:06:23.564388 widefield_analysis-0.1.5/widefield_analysis/smooth.py
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 widefield_analysis-0.1.5/PKG-INFO
```

### Comparing `widefield_analysis-0.1.4/widefield_analysis/animation.py` & `widefield_analysis-0.1.5/widefield_analysis/animation.py`

 * *Files identical despite different names*

### Comparing `widefield_analysis-0.1.4/widefield_analysis/baseline.py` & `widefield_analysis-0.1.5/widefield_analysis/baseline.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,14 @@
             print("Last baseline scales movie until ending.")
             scale_end = n_frames
         else:
             scale_end = baselines.loc[is_next, "first_frame"].values[0]
 
         n_baseline = baseline_end - baseline_start
         n_scale = scale_end - scale_start
-        print(f"Baseline {current_baseline} {baseline_start}:{baseline_end} ({n_baseline}) scales {scale_start}:{scale_end} ({n_scale})")
 
         baseline_movie = movie[baseline_start:baseline_end, :, :]
         scale_movie = movie[scale_start:scale_end]
 
         if method == "mean":
             baseline_image = np.mean(baseline_movie, axis=0)
         elif method == "median":
@@ -50,9 +49,11 @@
         else:
             raise ValueError(f"{method=} unknown")
         scale_movie = (scale_movie - baseline_image) / baseline_image
 
         if apply_limits:
             scale_movie[scale_movie < -absolute_limit] = -absolute_limit
             scale_movie[scale_movie > absolute_limit] = absolute_limit
+        print(f"Baseline {current_baseline} {baseline_start}:{baseline_end} ({n_baseline}) scales {scale_start}:{scale_end} ({n_scale})")
+        print(f"\tAfter scaling: from {np.nanmin(scale_movie):.1f} to {np.nanmax(scale_movie)} dF/F ({apply_limits=}, {absolute_limit=:.1f})")
         movie[scale_start:scale_end, :, :] = scale_movie
     return movie
```

### Comparing `widefield_analysis-0.1.4/widefield_analysis/files.py` & `widefield_analysis-0.1.5/widefield_analysis/files.py`

 * *Files identical despite different names*

### Comparing `widefield_analysis-0.1.4/widefield_analysis/filter.py` & `widefield_analysis-0.1.5/widefield_analysis/filter.py`

 * *Files identical despite different names*

### Comparing `widefield_analysis-0.1.4/widefield_analysis/resample.py` & `widefield_analysis-0.1.5/widefield_analysis/resample.py`

 * *Files identical despite different names*

### Comparing `widefield_analysis-0.1.4/widefield_analysis/smooth.py` & `widefield_analysis-0.1.5/widefield_analysis/smooth.py`

 * *Files identical despite different names*

### Comparing `widefield_analysis-0.1.4/PKG-INFO` & `widefield_analysis-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widefield-analysis
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Mathis
 Author-email: mathis.bassler@protonmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

