# Comparing `tmp/widefield_analysis-0.1.3.tar.gz` & `tmp/widefield_analysis-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widefield_analysis-0.1.3.tar", max compression
+gzip compressed data, was "widefield_analysis-0.1.4.tar", max compression
```

## Comparing `widefield_analysis-0.1.3.tar` & `widefield_analysis-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       55 2023-03-28 09:53:25.190532 widefield_analysis-0.1.3/README.md
--rw-r--r--   0        0        0      497 2023-05-25 12:02:20.818385 widefield_analysis-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 08:46:58.435982 widefield_analysis-0.1.3/widefield_analysis/__init__.py
--rw-r--r--   0        0        0     3364 2023-03-31 13:15:08.809441 widefield_analysis-0.1.3/widefield_analysis/animation.py
--rw-r--r--   0        0        0     4142 2023-05-10 08:26:55.916576 widefield_analysis-0.1.3/widefield_analysis/files.py
--rw-r--r--   0        0        0     1409 2023-05-25 11:53:43.138754 widefield_analysis-0.1.3/widefield_analysis/filter.py
--rw-r--r--   0        0        0      739 2023-03-31 09:51:47.977442 widefield_analysis-0.1.3/widefield_analysis/resample.py
--rw-r--r--   0        0        0      832 2023-03-28 09:15:07.411967 widefield_analysis-0.1.3/widefield_analysis/smooth.py
--rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 widefield_analysis-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-03-28 09:53:25.190532 widefield_analysis-0.1.4/README.md
+-rw-r--r--   0        0        0      497 2023-05-25 12:17:00.863264 widefield_analysis-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-28 08:46:58.435982 widefield_analysis-0.1.4/widefield_analysis/__init__.py
+-rw-r--r--   0        0        0     3364 2023-03-31 13:15:08.809441 widefield_analysis-0.1.4/widefield_analysis/animation.py
+-rw-r--r--   0        0        0     2150 2023-05-25 12:16:10.303648 widefield_analysis-0.1.4/widefield_analysis/baseline.py
+-rw-r--r--   0        0        0     3897 2023-05-25 12:06:22.820394 widefield_analysis-0.1.4/widefield_analysis/files.py
+-rw-r--r--   0        0        0     1409 2023-05-25 11:53:43.138754 widefield_analysis-0.1.4/widefield_analysis/filter.py
+-rw-r--r--   0        0        0      739 2023-03-31 09:51:47.977442 widefield_analysis-0.1.4/widefield_analysis/resample.py
+-rw-r--r--   0        0        0      876 2023-05-25 12:06:23.564388 widefield_analysis-0.1.4/widefield_analysis/smooth.py
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 widefield_analysis-0.1.4/PKG-INFO
```

### Comparing `widefield_analysis-0.1.3/widefield_analysis/animation.py` & `widefield_analysis-0.1.4/widefield_analysis/animation.py`

 * *Files identical despite different names*

### Comparing `widefield_analysis-0.1.3/widefield_analysis/files.py` & `widefield_analysis-0.1.4/widefield_analysis/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,13 +107,7 @@
     """
     file_stems = [file.stem for file in tif_files]
     stem_endings = [stem.split("_")[-1] for stem in file_stems]
     stem_endings = [int(ending) for ending in stem_endings]
     sort_vector = np.argsort(stem_endings)
     sorted_files = np.asarray(tif_files)[sort_vector]
     return sorted_files
-
-
-if __name__ == "__main__":
-    SOURCE_FOLDER = Path("/home/mathis/Code/gitlab/labnas/data/mapping_with_shielding")
-    TARGET_PARENT = Path("/home/mathis/Code/gitlab/labnas/data/")
-    convert_tif_folder_into_file(SOURCE_FOLDER, TARGET_PARENT)
```

### Comparing `widefield_analysis-0.1.3/widefield_analysis/filter.py` & `widefield_analysis-0.1.4/widefield_analysis/filter.py`

 * *Files identical despite different names*

### Comparing `widefield_analysis-0.1.3/widefield_analysis/resample.py` & `widefield_analysis-0.1.4/widefield_analysis/resample.py`

 * *Files identical despite different names*

### Comparing `widefield_analysis-0.1.3/widefield_analysis/smooth.py` & `widefield_analysis-0.1.4/widefield_analysis/smooth.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Smooth movies with gaussian kernels."""
+
 import numpy as np
 from scipy.ndimage import gaussian_filter
 from tqdm import tqdm
 
 
 def smooth_spatially(raw_movie: np.ndarray, sigma: float) -> np.ndarray:
     """Apply gaussian kernel convolution to each frame separately."""
```

### Comparing `widefield_analysis-0.1.3/PKG-INFO` & `widefield_analysis-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widefield-analysis
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Mathis
 Author-email: mathis.bassler@protonmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

