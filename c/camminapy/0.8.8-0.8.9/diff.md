# Comparing `tmp/camminapy-0.8.8.tar.gz` & `tmp/camminapy-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camminapy-0.8.8.tar", max compression
+gzip compressed data, was "camminapy-0.8.9.tar", max compression
```

## Comparing `camminapy-0.8.8.tar` & `camminapy-0.8.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2023-05-25 08:57:11.658456 camminapy-0.8.8/LICENSE
--rw-r--r--   0        0        0      177 2023-05-25 09:38:05.904312 camminapy-0.8.8/README.rst
--rw-r--r--   0        0        0      232 2023-05-25 09:36:38.187302 camminapy-0.8.8/camminapy/__init__.py
--rw-r--r--   0        0        0      343 2023-05-25 09:40:51.581748 camminapy-0.8.8/camminapy/data/__init__.py
--rw-r--r--   0        0        0     3352 2023-05-25 09:45:00.408123 camminapy-0.8.8/camminapy/data/resample.py
--rw-r--r--   0        0        0       63 2023-05-25 09:24:37.675451 camminapy-0.8.8/camminapy/plot/__init__.py
--rw-r--r--   0        0        0     2583 2023-05-25 09:25:59.612697 camminapy-0.8.8/camminapy/plot/footer.py
--rw-r--r--   0        0        0        0 2023-05-25 08:57:11.673431 camminapy-0.8.8/camminapy/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-05-25 08:57:11.672848 camminapy-0.8.8/camminapy/utils/config.py
--rw-r--r--   0        0        0      721 2023-05-25 08:57:11.674539 camminapy-0.8.8/camminapy/utils/logger.py
--rw-r--r--   0        0        0     1011 2023-05-25 09:45:14.244541 camminapy-0.8.8/pyproject.toml
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 camminapy-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-25 08:57:11.658456 camminapy-0.8.9/LICENSE
+-rw-r--r--   0        0        0      177 2023-05-25 09:38:05.904312 camminapy-0.8.9/README.rst
+-rw-r--r--   0        0        0      232 2023-05-25 09:36:38.187302 camminapy-0.8.9/camminapy/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-25 09:40:51.581748 camminapy-0.8.9/camminapy/data/__init__.py
+-rw-r--r--   0        0        0     3390 2023-05-25 10:23:04.781864 camminapy-0.8.9/camminapy/data/resample.py
+-rw-r--r--   0        0        0       63 2023-05-25 09:24:37.675451 camminapy-0.8.9/camminapy/plot/__init__.py
+-rw-r--r--   0        0        0     2583 2023-05-25 09:25:59.612697 camminapy-0.8.9/camminapy/plot/footer.py
+-rw-r--r--   0        0        0        0 2023-05-25 08:57:11.673431 camminapy-0.8.9/camminapy/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-25 08:57:11.672848 camminapy-0.8.9/camminapy/utils/config.py
+-rw-r--r--   0        0        0      721 2023-05-25 08:57:11.674539 camminapy-0.8.9/camminapy/utils/logger.py
+-rw-r--r--   0        0        0     1031 2023-05-25 10:23:16.719298 camminapy-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 camminapy-0.8.9/PKG-INFO
```

### Comparing `camminapy-0.8.8/LICENSE` & `camminapy-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.8/camminapy/data/resample.py` & `camminapy-0.8.9/camminapy/data/resample.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,16 @@
     interpolation_column: str,
     interpolation_step: float,
     group_column: str,
 ) -> pd.DataFrame:
     """
     Pandas wrapper for groupwise resampling.
 
+    NOTE: This does alter the index!
+
     See `resample_dataframe_grouped_polars` for details.
     """
     return resample_dataframe_grouped_polars(
         pl.DataFrame(df),
         interpolation_column,
         interpolation_step,
         group_column,
```

### Comparing `camminapy-0.8.8/camminapy/plot/footer.py` & `camminapy-0.8.9/camminapy/plot/footer.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.8/camminapy/utils/config.py` & `camminapy-0.8.9/camminapy/utils/config.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.8/camminapy/utils/logger.py` & `camminapy-0.8.9/camminapy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.8/pyproject.toml` & `camminapy-0.8.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "camminapy"
-version = "0.8.8"
+version = "0.8.9"
 description = "Personal helper functions and code snippets."
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 readme = "README.rst"
 repository = "https://github.com/thomascamminady/camminapy"
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 altair = "^5.0.0"
 gitpython = "^3.1.31"
 polars = "^0.17.15"
+pyarrow = "^12.0.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.0.1"
 ruff = "^0.0.253"
 black = "^23.1.0"
 pyclean = "^2.2.0"
 pre-commit = "^3.1.1"
```

### Comparing `camminapy-0.8.8/PKG-INFO` & `camminapy-0.8.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: camminapy
-Version: 0.8.8
+Version: 0.8.9
 Summary: Personal helper functions and code snippets.
 Home-page: https://github.com/thomascamminady/camminapy
 Author: Thomas Camminady
 Author-email: 0milieux_member@icloud.com
 Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: altair (>=5.0.0,<6.0.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: polars (>=0.17.15,<0.18.0)
+Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Project-URL: Repository, https://github.com/thomascamminady/camminapy
 Description-Content-Type: text/x-rst
 
 =========
 camminapy
 =========
```

