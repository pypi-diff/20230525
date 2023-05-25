# Comparing `tmp/camminapy-0.8.7.tar.gz` & `tmp/camminapy-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camminapy-0.8.7.tar", max compression
+gzip compressed data, was "camminapy-0.8.8.tar", max compression
```

## Comparing `camminapy-0.8.7.tar` & `camminapy-0.8.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2023-05-25 08:57:11.658456 camminapy-0.8.7/LICENSE
--rw-r--r--   0        0        0      177 2023-05-25 09:38:05.904312 camminapy-0.8.7/README.rst
--rw-r--r--   0        0        0      232 2023-05-25 09:36:38.187302 camminapy-0.8.7/camminapy/__init__.py
--rw-r--r--   0        0        0      343 2023-05-25 09:40:51.581748 camminapy-0.8.7/camminapy/data/__init__.py
--rw-r--r--   0        0        0     3331 2023-05-25 09:40:19.166193 camminapy-0.8.7/camminapy/data/resample.py
--rw-r--r--   0        0        0       63 2023-05-25 09:24:37.675451 camminapy-0.8.7/camminapy/plot/__init__.py
--rw-r--r--   0        0        0     2583 2023-05-25 09:25:59.612697 camminapy-0.8.7/camminapy/plot/footer.py
--rw-r--r--   0        0        0        0 2023-05-25 08:57:11.673431 camminapy-0.8.7/camminapy/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-05-25 08:57:11.672848 camminapy-0.8.7/camminapy/utils/config.py
--rw-r--r--   0        0        0      721 2023-05-25 08:57:11.674539 camminapy-0.8.7/camminapy/utils/logger.py
--rw-r--r--   0        0        0     1011 2023-05-25 09:41:27.897268 camminapy-0.8.7/pyproject.toml
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 camminapy-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-25 08:57:11.658456 camminapy-0.8.8/LICENSE
+-rw-r--r--   0        0        0      177 2023-05-25 09:38:05.904312 camminapy-0.8.8/README.rst
+-rw-r--r--   0        0        0      232 2023-05-25 09:36:38.187302 camminapy-0.8.8/camminapy/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-25 09:40:51.581748 camminapy-0.8.8/camminapy/data/__init__.py
+-rw-r--r--   0        0        0     3352 2023-05-25 09:45:00.408123 camminapy-0.8.8/camminapy/data/resample.py
+-rw-r--r--   0        0        0       63 2023-05-25 09:24:37.675451 camminapy-0.8.8/camminapy/plot/__init__.py
+-rw-r--r--   0        0        0     2583 2023-05-25 09:25:59.612697 camminapy-0.8.8/camminapy/plot/footer.py
+-rw-r--r--   0        0        0        0 2023-05-25 08:57:11.673431 camminapy-0.8.8/camminapy/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-25 08:57:11.672848 camminapy-0.8.8/camminapy/utils/config.py
+-rw-r--r--   0        0        0      721 2023-05-25 08:57:11.674539 camminapy-0.8.8/camminapy/utils/logger.py
+-rw-r--r--   0        0        0     1011 2023-05-25 09:45:14.244541 camminapy-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 camminapy-0.8.8/PKG-INFO
```

### Comparing `camminapy-0.8.7/LICENSE` & `camminapy-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.7/camminapy/data/resample.py` & `camminapy-0.8.8/camminapy/data/resample.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         `interpolation_column` is spaced as `interpolation_step` and all other
         data is interpolated onto that timeline.
     """
     interpolation_points = pl.DataFrame(
         {
             interpolation_column: np.arange(
                 df.min()[0, interpolation_column],
-                df.max()[0, interpolation_column],
+                df.max()[0, interpolation_column] + interpolation_step,
                 step=interpolation_step,
             )
         }
     )
 
     interpolated_df = interpolation_points.join(
         interpolation_points.join(df, on=[interpolation_column], how="outer")
```

### Comparing `camminapy-0.8.7/camminapy/plot/footer.py` & `camminapy-0.8.8/camminapy/plot/footer.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.7/camminapy/utils/config.py` & `camminapy-0.8.8/camminapy/utils/config.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.7/camminapy/utils/logger.py` & `camminapy-0.8.8/camminapy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.7/pyproject.toml` & `camminapy-0.8.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "camminapy"
-version = "0.8.7"
+version = "0.8.8"
 description = "Personal helper functions and code snippets."
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 readme = "README.rst"
 repository = "https://github.com/thomascamminady/camminapy"
 
 
 [tool.poetry.dependencies]
```

### Comparing `camminapy-0.8.7/PKG-INFO` & `camminapy-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camminapy
-Version: 0.8.7
+Version: 0.8.8
 Summary: Personal helper functions and code snippets.
 Home-page: https://github.com/thomascamminady/camminapy
 Author: Thomas Camminady
 Author-email: 0milieux_member@icloud.com
 Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

