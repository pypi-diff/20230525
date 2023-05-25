# Comparing `tmp/dagster-duckdb-pandas-0.19.5.tar.gz` & `tmp/dagster-duckdb-pandas-0.19.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-pandas-0.19.5.tar", last modified: Thu May 18 20:49:41 2023, max compression
+gzip compressed data, was "dagster-duckdb-pandas-0.19.6.tar", last modified: Thu May 25 17:25:16 2023, max compression
```

## Comparing `dagster-duckdb-pandas-0.19.5.tar` & `dagster-duckdb-pandas-0.19.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:41.893679 dagster-duckdb-pandas-0.19.5/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-05-18 20:38:07.000000 dagster-duckdb-pandas-0.19.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-18 20:38:07.000000 dagster-duckdb-pandas-0.19.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      685 2023-05-18 20:49:41.893679 dagster-duckdb-pandas-0.19.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      142 2023-05-18 20:38:07.000000 dagster-duckdb-pandas-0.19.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:41.893679 dagster-duckdb-pandas-0.19.5/dagster_duckdb_pandas/
--rw-r--r--   0 root         (0) root         (0)      374 2023-05-18 20:38:07.000000 dagster-duckdb-pandas-0.19.5/dagster_duckdb_pandas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7058 2023-05-18 20:38:07.000000 dagster-duckdb-pandas-0.19.5/dagster_duckdb_pandas/duckdb_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-18 20:38:07.000000 dagster-duckdb-pandas-0.19.5/dagster_duckdb_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-18 20:38:07.000000 dagster-duckdb-pandas-0.19.5/dagster_duckdb_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:41.893679 dagster-duckdb-pandas-0.19.5/dagster_duckdb_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      685 2023-05-18 20:49:41.000000 dagster-duckdb-pandas-0.19.5/dagster_duckdb_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2023-05-18 20:49:41.000000 dagster-duckdb-pandas-0.19.5/dagster_duckdb_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:49:41.000000 dagster-duckdb-pandas-0.19.5/dagster_duckdb_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:49:41.000000 dagster-duckdb-pandas-0.19.5/dagster_duckdb_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-18 20:49:41.000000 dagster-duckdb-pandas-0.19.5/dagster_duckdb_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 20:49:41.000000 dagster-duckdb-pandas-0.19.5/dagster_duckdb_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      132 2023-05-18 20:49:41.893679 dagster-duckdb-pandas-0.19.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1438 2023-05-18 20:38:07.000000 dagster-duckdb-pandas-0.19.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:25:16.261670 dagster-duckdb-pandas-0.19.6/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-05-25 17:16:50.000000 dagster-duckdb-pandas-0.19.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-25 17:16:50.000000 dagster-duckdb-pandas-0.19.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      685 2023-05-25 17:25:16.261670 dagster-duckdb-pandas-0.19.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      142 2023-05-25 17:16:50.000000 dagster-duckdb-pandas-0.19.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:25:16.261670 dagster-duckdb-pandas-0.19.6/dagster_duckdb_pandas/
+-rw-r--r--   0 root         (0) root         (0)      374 2023-05-25 17:16:50.000000 dagster-duckdb-pandas-0.19.6/dagster_duckdb_pandas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7058 2023-05-25 17:16:50.000000 dagster-duckdb-pandas-0.19.6/dagster_duckdb_pandas/duckdb_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-25 17:16:50.000000 dagster-duckdb-pandas-0.19.6/dagster_duckdb_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-25 17:16:50.000000 dagster-duckdb-pandas-0.19.6/dagster_duckdb_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:25:16.261670 dagster-duckdb-pandas-0.19.6/dagster_duckdb_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      685 2023-05-25 17:25:16.000000 dagster-duckdb-pandas-0.19.6/dagster_duckdb_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2023-05-25 17:25:16.000000 dagster-duckdb-pandas-0.19.6/dagster_duckdb_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:25:16.000000 dagster-duckdb-pandas-0.19.6/dagster_duckdb_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:25:16.000000 dagster-duckdb-pandas-0.19.6/dagster_duckdb_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-25 17:25:16.000000 dagster-duckdb-pandas-0.19.6/dagster_duckdb_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-25 17:25:16.000000 dagster-duckdb-pandas-0.19.6/dagster_duckdb_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2023-05-25 17:25:16.261670 dagster-duckdb-pandas-0.19.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-05-25 17:16:50.000000 dagster-duckdb-pandas-0.19.6/setup.py
```

### Comparing `dagster-duckdb-pandas-0.19.5/LICENSE` & `dagster-duckdb-pandas-0.19.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pandas-0.19.5/PKG-INFO` & `dagster-duckdb-pandas-0.19.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pandas
-Version: 0.19.5
+Version: 0.19.6
 Summary: Package for storing Pandas DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-pandas-0.19.5/dagster_duckdb_pandas/duckdb_pandas_type_handler.py` & `dagster-duckdb-pandas-0.19.6/dagster_duckdb_pandas/duckdb_pandas_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pandas-0.19.5/dagster_duckdb_pandas.egg-info/PKG-INFO` & `dagster-duckdb-pandas-0.19.6/dagster_duckdb_pandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pandas
-Version: 0.19.5
+Version: 0.19.6
 Summary: Package for storing Pandas DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-pandas-0.19.5/setup.py` & `dagster-duckdb-pandas-0.19.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,13 +31,13 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_pandas_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.3.5",
-        "dagster-duckdb==0.19.5",
+        "dagster==1.3.6",
+        "dagster-duckdb==0.19.6",
         "pandas<2",  # See: https://github.com/dagster-io/dagster/issues/13339
     ],
     zip_safe=False,
 )
```

