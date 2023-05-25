# Comparing `tmp/ncconvert-0.1.2.tar.gz` & `tmp/ncconvert-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncconvert-0.1.2.tar", last modified: Tue May  9 23:57:43 2023, max compression
+gzip compressed data, was "ncconvert-0.1.3.tar", last modified: Thu May 25 21:51:55 2023, max compression
```

## Comparing `ncconvert-0.1.2.tar` & `ncconvert-0.1.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:57:43.839316 ncconvert-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-09 23:57:31.000000 ncconvert-0.1.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:57:43.831315 ncconvert-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:57:43.835315 ncconvert-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-09 23:57:31.000000 ncconvert-0.1.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-09 23:57:31.000000 ncconvert-0.1.2/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-09 23:57:31.000000 ncconvert-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-09 23:57:31.000000 ncconvert-0.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-09 23:57:31.000000 ncconvert-0.1.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-09 23:57:43.839316 ncconvert-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-09 23:57:31.000000 ncconvert-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-09 23:57:31.000000 ncconvert-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 23:57:43.839316 ncconvert-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-09 23:57:31.000000 ncconvert-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:57:43.831315 ncconvert-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:57:43.835315 ncconvert-0.1.2/src/ncconvert/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-09 23:57:31.000000 ncconvert-0.1.2/src/ncconvert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-09 23:57:31.000000 ncconvert-0.1.2/src/ncconvert/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 23:57:43.000000 ncconvert-0.1.2/src/ncconvert/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-09 23:57:31.000000 ncconvert-0.1.2/src/ncconvert/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-09 23:57:31.000000 ncconvert-0.1.2/src/ncconvert/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-09 23:57:31.000000 ncconvert-0.1.2/src/ncconvert/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 23:57:31.000000 ncconvert-0.1.2/src/ncconvert/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-09 23:57:31.000000 ncconvert-0.1.2/src/ncconvert/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:57:43.839316 ncconvert-0.1.2/src/ncconvert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-09 23:57:43.000000 ncconvert-0.1.2/src/ncconvert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-09 23:57:43.000000 ncconvert-0.1.2/src/ncconvert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 23:57:43.000000 ncconvert-0.1.2/src/ncconvert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-09 23:57:43.000000 ncconvert-0.1.2/src/ncconvert.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-09 23:57:43.000000 ncconvert-0.1.2/src/ncconvert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 23:57:43.000000 ncconvert-0.1.2/src/ncconvert.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:57:43.839316 ncconvert-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-09 23:57:31.000000 ncconvert-0.1.2/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-09 23:57:31.000000 ncconvert-0.1.2/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-09 23:57:31.000000 ncconvert-0.1.2/test/test_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-09 23:57:31.000000 ncconvert-0.1.2/test/test_parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:55.665022 ncconvert-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-25 21:51:45.000000 ncconvert-0.1.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:55.657022 ncconvert-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:55.661022 ncconvert-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-25 21:51:45.000000 ncconvert-0.1.3/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-25 21:51:45.000000 ncconvert-0.1.3/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-25 21:51:45.000000 ncconvert-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-25 21:51:45.000000 ncconvert-0.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-25 21:51:45.000000 ncconvert-0.1.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-25 21:51:55.661022 ncconvert-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-25 21:51:45.000000 ncconvert-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-25 21:51:45.000000 ncconvert-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:51:55.665022 ncconvert-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-25 21:51:45.000000 ncconvert-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:55.661022 ncconvert-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:55.661022 ncconvert-0.1.3/src/ncconvert/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-25 21:51:45.000000 ncconvert-0.1.3/src/ncconvert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-25 21:51:45.000000 ncconvert-0.1.3/src/ncconvert/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 21:51:55.000000 ncconvert-0.1.3/src/ncconvert/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-25 21:51:45.000000 ncconvert-0.1.3/src/ncconvert/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-25 21:51:45.000000 ncconvert-0.1.3/src/ncconvert/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-25 21:51:45.000000 ncconvert-0.1.3/src/ncconvert/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:45.000000 ncconvert-0.1.3/src/ncconvert/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-25 21:51:45.000000 ncconvert-0.1.3/src/ncconvert/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:55.661022 ncconvert-0.1.3/src/ncconvert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-25 21:51:55.000000 ncconvert-0.1.3/src/ncconvert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-25 21:51:55.000000 ncconvert-0.1.3/src/ncconvert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:51:55.000000 ncconvert-0.1.3/src/ncconvert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-25 21:51:55.000000 ncconvert-0.1.3/src/ncconvert.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-25 21:51:55.000000 ncconvert-0.1.3/src/ncconvert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 21:51:55.000000 ncconvert-0.1.3/src/ncconvert.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:55.661022 ncconvert-0.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-25 21:51:45.000000 ncconvert-0.1.3/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-25 21:51:45.000000 ncconvert-0.1.3/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-25 21:51:45.000000 ncconvert-0.1.3/test/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-25 21:51:45.000000 ncconvert-0.1.3/test/test_parquet.py
```

### Comparing `ncconvert-0.1.2/.github/workflows/pypi.yml` & `ncconvert-0.1.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.2/.github/workflows/pytest.yml` & `ncconvert-0.1.3/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.2/LICENSE.md` & `ncconvert-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.2/PKG-INFO` & `ncconvert-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncconvert
-Version: 0.1.2
+Version: 0.1.3
 Summary: Convert netCDF to other formats.
 Author-email: tsdat <tsdat@pnnl.gov>
 License: # Time Series Data Utilities
         
         Copyright © 2023, Battelle Memorial Institute
         
         Licensed under a Simplified BSD 2-Clause License;
```

### Comparing `ncconvert-0.1.2/README.md` & `ncconvert-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.2/pyproject.toml` & `ncconvert-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 keywords = ["netCDF", "cdf", "nc"]
 license = {file = "LICENSE.md"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "xarray[io]",
-  "pandas[hdf5, parquet, feather, spss, excel]",
+  "pandas[parquet]",
 ]
 
 [project.optional-dependencies]
 dev = [
   "pytest",
   "coverage",
   "build",
```

### Comparing `ncconvert-0.1.2/src/ncconvert/cli.py` & `ncconvert-0.1.3/src/ncconvert/cli.py`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.2/src/ncconvert/csv.py` & `ncconvert-0.1.3/src/ncconvert/csv.py`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.2/src/ncconvert/parquet.py` & `ncconvert-0.1.3/src/ncconvert/parquet.py`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.2/src/ncconvert/utils.py` & `ncconvert-0.1.3/src/ncconvert/utils.py`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.2/src/ncconvert.egg-info/PKG-INFO` & `ncconvert-0.1.3/src/ncconvert.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncconvert
-Version: 0.1.2
+Version: 0.1.3
 Summary: Convert netCDF to other formats.
 Author-email: tsdat <tsdat@pnnl.gov>
 License: # Time Series Data Utilities
         
         Copyright © 2023, Battelle Memorial Institute
         
         Licensed under a Simplified BSD 2-Clause License;
```

### Comparing `ncconvert-0.1.2/src/ncconvert.egg-info/SOURCES.txt` & `ncconvert-0.1.3/src/ncconvert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.2/test/conftest.py` & `ncconvert-0.1.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.2/test/test_cli.py` & `ncconvert-0.1.3/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.2/test/test_csv.py` & `ncconvert-0.1.3/test/test_csv.py`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.2/test/test_parquet.py` & `ncconvert-0.1.3/test/test_parquet.py`

 * *Files identical despite different names*

