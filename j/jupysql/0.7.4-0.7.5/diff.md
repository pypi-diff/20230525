# Comparing `tmp/jupysql-0.7.4.tar.gz` & `tmp/jupysql-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupysql-0.7.4.tar", last modified: Fri Apr 28 17:26:23 2023, max compression
+gzip compressed data, was "jupysql-0.7.5.tar", last modified: Wed May 24 22:55:07 2023, max compression
```

## Comparing `jupysql-0.7.4.tar` & `jupysql-0.7.5.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 idomi      (501) staff       (20)        0 2023-04-28 17:26:23.758298 jupysql-0.7.4/
--rw-r--r--   0 idomi      (501) staff       (20)    11820 2023-03-13 20:16:41.000000 jupysql-0.7.4/LICENSE
--rw-r--r--   0 idomi      (501) staff       (20)       52 2022-12-28 16:23:15.000000 jupysql-0.7.4/MANIFEST.in
--rw-r--r--   0 idomi      (501) staff       (20)     3017 2023-04-28 17:26:23.758382 jupysql-0.7.4/PKG-INFO
--rw-r--r--   0 idomi      (501) staff       (20)     2354 2023-04-06 15:26:02.000000 jupysql-0.7.4/README.md
--rw-r--r--   0 idomi      (501) staff       (20)      701 2023-04-21 18:56:18.000000 jupysql-0.7.4/pyproject.toml
--rw-r--r--   0 idomi      (501) staff       (20)      120 2023-04-28 17:26:23.758697 jupysql-0.7.4/setup.cfg
--rw-r--r--   0 idomi      (501) staff       (20)     2166 2023-04-28 16:54:46.000000 jupysql-0.7.4/setup.py
-drwxr-xr-x   0 idomi      (501) staff       (20)        0 2023-04-28 17:26:23.749342 jupysql-0.7.4/src/
-drwxr-xr-x   0 idomi      (501) staff       (20)        0 2023-04-28 17:26:23.752275 jupysql-0.7.4/src/jupysql.egg-info/
--rw-r--r--   0 idomi      (501) staff       (20)     3017 2023-04-28 17:26:23.000000 jupysql-0.7.4/src/jupysql.egg-info/PKG-INFO
--rw-r--r--   0 idomi      (501) staff       (20)      836 2023-04-28 17:26:23.000000 jupysql-0.7.4/src/jupysql.egg-info/SOURCES.txt
--rw-r--r--   0 idomi      (501) staff       (20)        1 2023-04-28 17:26:23.000000 jupysql-0.7.4/src/jupysql.egg-info/dependency_links.txt
--rw-r--r--   0 idomi      (501) staff       (20)        1 2022-12-28 16:24:18.000000 jupysql-0.7.4/src/jupysql.egg-info/not-zip-safe
--rw-r--r--   0 idomi      (501) staff       (20)      522 2023-04-28 17:26:23.000000 jupysql-0.7.4/src/jupysql.egg-info/requires.txt
--rw-r--r--   0 idomi      (501) staff       (20)        4 2023-04-28 17:26:23.000000 jupysql-0.7.4/src/jupysql.egg-info/top_level.txt
-drwxr-xr-x   0 idomi      (501) staff       (20)        0 2023-04-28 17:26:23.756136 jupysql-0.7.4/src/sql/
--rw-r--r--   0 idomi      (501) staff       (20)      169 2023-04-28 17:09:04.000000 jupysql-0.7.4/src/sql/__init__.py
--rw-r--r--   0 idomi      (501) staff       (20)      544 2023-04-21 18:56:18.000000 jupysql-0.7.4/src/sql/_patch.py
--rw-r--r--   0 idomi      (501) staff       (20)    10319 2023-04-18 13:56:12.000000 jupysql-0.7.4/src/sql/_testing.py
--rw-r--r--   0 idomi      (501) staff       (20)     2899 2023-03-03 16:02:07.000000 jupysql-0.7.4/src/sql/column_guesser.py
--rw-r--r--   0 idomi      (501) staff       (20)     2964 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/command.py
--rw-r--r--   0 idomi      (501) staff       (20)    17908 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/connection.py
--rw-r--r--   0 idomi      (501) staff       (20)     1159 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/exceptions.py
-drwxr-xr-x   0 idomi      (501) staff       (20)        0 2023-04-28 17:26:23.756851 jupysql-0.7.4/src/sql/ggplot/
--rw-r--r--   0 idomi      (501) staff       (20)      248 2023-03-31 19:06:22.000000 jupysql-0.7.4/src/sql/ggplot/__init__.py
--rw-r--r--   0 idomi      (501) staff       (20)      446 2023-03-31 19:06:22.000000 jupysql-0.7.4/src/sql/ggplot/aes.py
--rw-r--r--   0 idomi      (501) staff       (20)     1092 2023-04-21 18:56:18.000000 jupysql-0.7.4/src/sql/ggplot/facet_wrap.py
-drwxr-xr-x   0 idomi      (501) staff       (20)        0 2023-04-28 17:26:23.758173 jupysql-0.7.4/src/sql/ggplot/geom/
--rw-r--r--   0 idomi      (501) staff       (20)      158 2023-03-31 19:06:22.000000 jupysql-0.7.4/src/sql/ggplot/geom/__init__.py
--rw-r--r--   0 idomi      (501) staff       (20)      327 2023-03-23 19:57:06.000000 jupysql-0.7.4/src/sql/ggplot/geom/geom.py
--rw-r--r--   0 idomi      (501) staff       (20)      463 2023-03-31 19:06:22.000000 jupysql-0.7.4/src/sql/ggplot/geom/geom_boxplot.py
--rw-r--r--   0 idomi      (501) staff       (20)     1060 2023-03-31 19:06:22.000000 jupysql-0.7.4/src/sql/ggplot/geom/geom_histogram.py
--rw-r--r--   0 idomi      (501) staff       (20)     2412 2023-03-31 19:06:22.000000 jupysql-0.7.4/src/sql/ggplot/ggplot.py
--rw-r--r--   0 idomi      (501) staff       (20)    10405 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/inspect.py
--rw-r--r--   0 idomi      (501) staff       (20)    15400 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/magic.py
--rw-r--r--   0 idomi      (501) staff       (20)     9161 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/magic_cmd.py
--rw-r--r--   0 idomi      (501) staff       (20)     2692 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/magic_plot.py
--rw-r--r--   0 idomi      (501) staff       (20)     2923 2023-04-18 13:56:12.000000 jupysql-0.7.4/src/sql/parse.py
--rw-r--r--   0 idomi      (501) staff       (20)    15764 2023-04-21 18:56:18.000000 jupysql-0.7.4/src/sql/plot.py
--rw-r--r--   0 idomi      (501) staff       (20)    16714 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/run.py
--rw-r--r--   0 idomi      (501) staff       (20)     4949 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/store.py
--rw-r--r--   0 idomi      (501) staff       (20)      326 2023-03-03 16:02:07.000000 jupysql-0.7.4/src/sql/telemetry.py
--rw-r--r--   0 idomi      (501) staff       (20)     6923 2023-04-27 15:28:18.000000 jupysql-0.7.4/src/sql/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:55:07.356754 jupysql-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-05-24 22:54:48.000000 jupysql-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-24 22:54:48.000000 jupysql-0.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-24 22:55:07.356754 jupysql-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-24 22:54:48.000000 jupysql-0.7.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-24 22:54:48.000000 jupysql-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-24 22:55:07.356754 jupysql-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-24 22:54:48.000000 jupysql-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:55:07.344754 jupysql-0.7.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:55:07.348754 jupysql-0.7.5/src/jupysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-24 22:55:06.000000 jupysql-0.7.5/src/jupysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-24 22:55:06.000000 jupysql-0.7.5/src/jupysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:55:06.000000 jupysql-0.7.5/src/jupysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:55:06.000000 jupysql-0.7.5/src/jupysql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-24 22:55:06.000000 jupysql-0.7.5/src/jupysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-24 22:55:06.000000 jupysql-0.7.5/src/jupysql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:55:07.356754 jupysql-0.7.5/src/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/column_guesser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18567 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:55:07.356754 jupysql-0.7.5/src/sql/ggplot/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/ggplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/ggplot/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/ggplot/facet_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:55:07.356754 jupysql-0.7.5/src/sql/ggplot/geom/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/ggplot/geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/ggplot/geom/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/ggplot/geom/geom_boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/ggplot/geom/geom_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/ggplot/ggplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16597 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/magic_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/magic_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16139 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18198 2023-05-24 22:54:49.000000 jupysql-0.7.5/src/sql/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-24 22:54:49.000000 jupysql-0.7.5/src/sql/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-24 22:54:49.000000 jupysql-0.7.5/src/sql/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-05-24 22:54:49.000000 jupysql-0.7.5/src/sql/util.py
```

### Comparing `jupysql-0.7.4/LICENSE` & `jupysql-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.4/PKG-INFO` & `jupysql-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.7.4
+Version: 0.7.5
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.7.4 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.7.5 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `jupysql-0.7.4/README.md` & `jupysql-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.4/pyproject.toml` & `jupysql-0.7.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.4/setup.py` & `jupysql-0.7.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 with open("src/sql/__init__.py", "rb") as f:
     VERSION = str(
         ast.literal_eval(_version_re.search(f.read().decode("utf-8")).group(1))
     )
 
 install_requires = [
     "prettytable",
-    "ipython<=8.12.0; python_version == '3.8'",
+    # IPython dropped support for Python 3.8
+    "ipython<=8.12.0; python_version <= '3.8'",
+    "ipython",
     "sqlalchemy",
     "sqlparse",
     "ipython-genutils>=0.1.0",
     "sqlglot",
     "jinja2",
     "sqlglot>=11.3.7",
     "ploomber-core>=0.2.7",
@@ -33,15 +35,15 @@
     "pytest",
     "pandas",
     "polars==0.17.2",  # 04/18/23 this breaks our CI
     "invoke",
     "pkgmt",
     "twine",
     # tests
-    "duckdb",
+    "duckdb<0.8.0",
     "duckdb-engine",
     "pyodbc",
     # sql.plot module tests
     "matplotlib",
     "black",
     # for %%sql --interact
     "ipywidgets",
```

### Comparing `jupysql-0.7.4/src/jupysql.egg-info/PKG-INFO` & `jupysql-0.7.5/src/jupysql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.7.4
+Version: 0.7.5
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.7.4 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.7.5 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `jupysql-0.7.4/src/jupysql.egg-info/SOURCES.txt` & `jupysql-0.7.5/src/jupysql.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 src/jupysql.egg-info/top_level.txt
 src/sql/__init__.py
 src/sql/_patch.py
 src/sql/_testing.py
 src/sql/column_guesser.py
 src/sql/command.py
 src/sql/connection.py
+src/sql/error_message.py
 src/sql/exceptions.py
 src/sql/inspect.py
 src/sql/magic.py
 src/sql/magic_cmd.py
 src/sql/magic_plot.py
 src/sql/parse.py
 src/sql/plot.py
```

### Comparing `jupysql-0.7.4/src/jupysql.egg-info/requires.txt` & `jupysql-0.7.5/src/jupysql.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 prettytable
+ipython
 sqlalchemy
 sqlparse
 ipython-genutils>=0.1.0
 sqlglot
 jinja2
 sqlglot>=11.3.7
 ploomber-core>=0.2.7
 
 [:python_version < "3.8"]
 importlib-metadata
 
-[:python_version == "3.8"]
+[:python_version <= "3.8"]
 ipython<=8.12.0
 
 [dev]
 flake8
 pytest
 pandas
 polars==0.17.2
 invoke
 pkgmt
 twine
-duckdb
+duckdb<0.8.0
 duckdb-engine
 pyodbc
 matplotlib
 black
 ipywidgets
 
 [integration]
 flake8
 pytest
 pandas
 polars==0.17.2
 invoke
 pkgmt
 twine
-duckdb
+duckdb<0.8.0
 duckdb-engine
 pyodbc
 matplotlib
 black
 ipywidgets
 dockerctx
 pyarrow
```

### Comparing `jupysql-0.7.4/src/sql/_patch.py` & `jupysql-0.7.5/src/sql/_patch.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.4/src/sql/_testing.py` & `jupysql-0.7.5/src/sql/_testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
 
 client = docker.from_env()
 
 
 def database_ready(
     database,
-    timeout=20,
+    timeout=60,
     poll_freq=0.5,
 ):
     """Wait until the container is ready to receive connections.
 
 
     :type host: str
     :type port: int
```

### Comparing `jupysql-0.7.4/src/sql/column_guesser.py` & `jupysql-0.7.5/src/sql/column_guesser.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.4/src/sql/command.py` & `jupysql-0.7.5/src/sql/command.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.4/src/sql/connection.py` & `jupysql-0.7.5/src/sql/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import os
 from difflib import get_close_matches
 
 import sqlalchemy
 from sqlalchemy.engine import Engine
-from sqlalchemy.exc import NoSuchModuleError
+from sqlalchemy.exc import NoSuchModuleError, OperationalError
 from IPython.core.error import UsageError
 import difflib
 import sqlglot
 
 from sql.store import store
 from sql.telemetry import telemetry
 from sql import exceptions
+from sql.error_message import detail
+from ploomber_core.exceptions import modify_exceptions
 
-PLOOMBER_SUPPORT_LINK_STR = (
-    "For technical support: https://ploomber.io/community"
-    "\nDocumentation: https://jupysql.ploomber.io/en/latest/connecting.html"
+PLOOMBER_DOCS_LINK_STR = (
+    "Documentation: https://jupysql.ploomber.io/en/latest/connecting.html"
 )
 IS_SQLALCHEMY_ONE = int(sqlalchemy.__version__.split(".")[0]) == 1
 
 # Check Full List: https://docs.sqlalchemy.org/en/20/dialects
 MISSING_PACKAGE_LIST_EXCEPT_MATCHERS = {
     # SQLite
     "sqlite": "sqlite",
@@ -120,25 +121,63 @@
 
     # the active connection
     current = None
 
     # all connections
     connections = {}
 
+    def __init__(self, engine, alias=None):
+        self.url = engine.url
+        self.name = self.assign_name(engine)
+        self.dialect = self.url.get_dialect()
+        self.engine = engine
+
+        if IS_SQLALCHEMY_ONE:
+            self.metadata = sqlalchemy.MetaData(bind=engine)
+
+        url = (
+            repr(sqlalchemy.MetaData(bind=engine).bind.url)
+            if IS_SQLALCHEMY_ONE
+            else repr(engine.url)
+        )
+
+        self.session = self._create_session(engine, url)
+
+        self.connections[alias or url] = self
+
+        self.connect_args = None
+        self.alias = alias
+        Connection.current = self
+
     @classmethod
     def _suggest_fix_no_module_found(module_name):
         DEFAULT_PREFIX = "\n\n"
 
         prefix = DEFAULT_PREFIX
         suffix = "To fix it:"
         suggest_str = "Install X package and try again"
         options = [f"{prefix}{suffix}", suggest_str]
         return "\n\n".join(options)
 
     @classmethod
+    @modify_exceptions
+    def _create_session(cls, engine, connect_str):
+        try:
+            session = engine.connect()
+            return session
+        except OperationalError as e:
+            detailed_msg = detail(e)
+            if detailed_msg is not None:
+                raise exceptions.UsageError(detailed_msg)
+            else:
+                print(e)
+        except Exception as e:
+            raise cls._error_invalid_connection_info(e, connect_str) from e
+
+    @classmethod
     def _suggest_fix(cls, env_var, connect_str=None):
         """
         Returns an error message that we can display to the user
         to tell them how to pass the connection string
         """
         DEFAULT_PREFIX = "\n\n"
 
@@ -176,51 +215,33 @@
 
         if env_var:
             options.append("Set the environment variable $DATABASE_URL")
 
         if len(options) >= 3:
             options.insert(-1, "OR")
 
-        options.append(PLOOMBER_SUPPORT_LINK_STR)
+        options.append(PLOOMBER_DOCS_LINK_STR)
 
         return "\n\n".join(options)
 
     @classmethod
     def _error_no_connection(cls):
         """Error when there isn't any connection"""
-        return UsageError("No active connection." + cls._suggest_fix(env_var=True))
+        err = UsageError("No active connection." + cls._suggest_fix(env_var=True))
+        err.modify_exception = True
+        return err
 
     @classmethod
     def _error_invalid_connection_info(cls, e, connect_str):
-        return UsageError(
+        err = UsageError(
             "An error happened while creating the connection: "
             f"{e}.{cls._suggest_fix(env_var=False, connect_str=connect_str)}"
         )
-
-    def __init__(self, engine, alias=None):
-        self.url = engine.url
-        self.name = self.assign_name(engine)
-        self.dialect = self.url.get_dialect()
-        self.session = engine.connect()
-
-        if IS_SQLALCHEMY_ONE:
-            self.metadata = sqlalchemy.MetaData(bind=engine)
-
-        self.connections[
-            alias
-            or (
-                repr(sqlalchemy.MetaData(bind=engine).bind.url)
-                if IS_SQLALCHEMY_ONE
-                else repr(engine.url)
-            )
-        ] = self
-
-        self.connect_args = None
-        self.alias = alias
-        Connection.current = self
+        err.modify_exception = True
+        return err
 
     @classmethod
     def from_connect_str(
         cls, connect_str=None, connect_args=None, creator=None, alias=None
     ):
         """Creates a new connection from a connection string"""
         connect_args = connect_args or {}
@@ -240,15 +261,15 @@
         except (ModuleNotFoundError, NoSuchModuleError) as e:
             suggestion_str = get_missing_package_suggestion_str(e)
             raise exceptions.MissingPackageError(
                 "\n\n".join(
                     [
                         str(e),
                         suggestion_str,
-                        PLOOMBER_SUPPORT_LINK_STR,
+                        PLOOMBER_DOCS_LINK_STR,
                     ]
                 )
             ) from e
         except Exception as e:
             raise cls._error_invalid_connection_info(e, connect_str) from e
 
         connection = cls(engine, alias=alias)
```

### Comparing `jupysql-0.7.4/src/sql/exceptions.py` & `jupysql-0.7.5/src/sql/exceptions.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.4/src/sql/ggplot/facet_wrap.py` & `jupysql-0.7.5/src/sql/ggplot/facet_wrap.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.4/src/sql/ggplot/geom/geom_histogram.py` & `jupysql-0.7.5/src/sql/ggplot/geom/geom_histogram.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.4/src/sql/ggplot/ggplot.py` & `jupysql-0.7.5/src/sql/ggplot/ggplot.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.4/src/sql/inspect.py` & `jupysql-0.7.5/src/sql/inspect.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.4/src/sql/magic.py` & `jupysql-0.7.5/src/sql/magic.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,17 @@
 from sql.store import store
 from sql.command import SQLCommand
 from sql.magic_plot import SqlPlotMagic
 from sql.magic_cmd import SqlCmdMagic
 from sql._patch import patch_ipython_usage_error
 from ploomber_core.dependencies import check_installed
 
+from sql.error_message import detail
 from traitlets.config.configurable import Configurable
-from traitlets import Bool, Int, Unicode, Dict, observe
+from traitlets import Bool, Int, TraitError, Unicode, Dict, observe, validate
 
 try:
     from pandas.core.frame import DataFrame, Series
 except ModuleNotFoundError:
     DataFrame = None
     Series = None
 
@@ -90,15 +91,15 @@
     )
     short_errors = Bool(
         True,
         config=True,
         help="Don't display the full traceback on SQL Programming Error",
     )
     displaylimit = Int(
-        None,
+        sql.run.DEFAULT_DISPLAYLIMIT_VALUE,
         config=True,
         allow_none=True,
         help=(
             "Automatically limit the number of rows "
             "displayed (full result set is still stored)"
         ),
     )
@@ -140,14 +141,34 @@
 
         Configurable.__init__(self, config=shell.config)
         Magics.__init__(self, shell=shell)
 
         # Add ourself to the list of module configurable via %config
         self.shell.configurables.append(self)
 
+    # To verify displaylimit is valid positive integer
+    # If:
+    #   None -> We treat it as 0 (no limit)
+    #   Positive Integer -> Pass
+    #   Negative Integer -> raise Error
+    @validate("displaylimit")
+    def _valid_displaylimit(self, proposal):
+        if proposal["value"] is None:
+            print("displaylimit: Value None will be treated as 0 (no limit)")
+            return 0
+        try:
+            value = int(proposal["value"])
+            if value < 0:
+                raise TraitError(
+                    "{}: displaylimit cannot be a negative integer".format(value)
+                )
+            return value
+        except ValueError:
+            raise TraitError("{}: displaylimit is not an integer".format(value))
+
     @observe("autopandas", "autopolars")
     def _mutex_autopandas_autopolars(self, change):
         # When enabling autopandas or autopolars, automatically disable the
         # other one in case it was enabled and print a warning
         if change["new"]:
             other = "autopolars" if change["name"] == "autopandas" else "autopandas"
             if getattr(self, other):
@@ -257,14 +278,15 @@
 
         """
         return self._execute(
             line=line, cell=cell, local_ns=local_ns, is_interactive_mode=False
         )
 
     @telemetry.log_call("execute", payload=True)
+    @modify_exceptions
     def _execute(self, payload, line, cell, local_ns, is_interactive_mode=False):
         def interactive_execute_wrapper(**kwargs):
             for key, value in kwargs.items():
                 local_ns[key] = value
             return self._execute(line, cell, local_ns, is_interactive_mode=True)
 
         """
@@ -405,19 +427,26 @@
 
                 # Return results into the default ipython _ variable
                 return result
 
         # JA: added DatabaseError for MySQL
         except (ProgrammingError, OperationalError, DatabaseError) as e:
             # Sqlite apparently return all errors as OperationalError :/
-
+            detailed_msg = detail(e, command.sql)
             if self.short_errors:
-                print(e)
+                if detailed_msg is not None:
+                    err = exceptions.UsageError(detailed_msg)
+                    raise err
+                else:
+                    print(e)
             else:
-                raise
+                if detailed_msg is not None:
+                    print(detailed_msg)
+                e.modify_exception = True
+                raise e
 
     legal_sql_identifier = re.compile(r"^[A-Za-z0-9#_$]+")
 
     @modify_exceptions
     def _persist_dataframe(self, raw, conn, user_ns, append=False, index=True):
         """Implements PERSIST, which writes a DataFrame to the RDBMS"""
         if not DataFrame:
```

### Comparing `jupysql-0.7.4/src/sql/magic_cmd.py` & `jupysql-0.7.5/src/sql/magic_cmd.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.4/src/sql/magic_plot.py` & `jupysql-0.7.5/src/sql/magic_plot.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.4/src/sql/parse.py` & `jupysql-0.7.5/src/sql/parse.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.4/src/sql/plot.py` & `jupysql-0.7.5/src/sql/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Plot using the SQL backend
 """
 from ploomber_core.dependencies import requires
 from ploomber_core.exceptions import modify_exceptions
 from jinja2 import Template
 
 from sql.util import flatten
+from sqlalchemy.exc import ProgrammingError
+from sql import exceptions
 
 try:
     import matplotlib.pyplot as plt
     from matplotlib.colors import Normalize
 except ModuleNotFoundError:
     plt = None
     Normalize = None
@@ -26,29 +28,39 @@
 
 
 def _summary_stats(conn, table, column, with_=None):
     """Compute percentiles and mean for boxplot"""
 
     if not conn:
         conn = sql.connection.Connection.current
+    driver = conn._get_curr_sqlalchemy_connection_info()["driver"]
 
     template = Template(
         """
     SELECT
     percentile_disc([0.25, 0.50, 0.75]) WITHIN GROUP \
     (ORDER BY "{{column}}") AS percentiles,
     AVG("{{column}}") AS mean,
     COUNT(*) AS N
     FROM "{{table}}"
 """
     )
 
     query = template.render(table=table, column=column)
 
-    values = conn.execute(query, with_).fetchone()
+    try:
+        values = conn.execute(query, with_).fetchone()
+    except ProgrammingError as e:
+        print(e)
+        raise exceptions.RuntimeError(
+            f"\nEnsure that percentile_disc function is available on {driver}."
+        )
+    except Exception as e:
+        raise e
+
     keys = ["q1", "med", "q3", "mean", "N"]
     return {k: float(v) for k, v in zip(keys, flatten(values))}
 
 
 def _whishi(conn, table, column, hival, with_=None):
     if not conn:
         conn = sql.connection.Connection.current
```

### Comparing `jupysql-0.7.4/src/sql/run.py` & `jupysql-0.7.5/src/sql/run.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 from sqlalchemy.orm import Session
 
 from sql.telemetry import telemetry
 import logging
 import warnings
 from collections.abc import Iterable
 
+DEFAULT_DISPLAYLIMIT_VALUE = 10
+
 
 def unduplicate_field_names(field_names):
     """Append a number to duplicate field names to make them unique."""
     res = []
     for k in field_names:
         if k in res:
             i = 1
@@ -96,85 +98,108 @@
     spaces = "&nbsp;" * len(match_obj.group(2))
     return "%s%s" % (match_obj.group(1), spaces)
 
 
 _cell_with_spaces_pattern = re.compile(r"(<td>)( {2,})")
 
 
-class ResultSet(list, ColumnGuesserMixin):
+class ResultSet(ColumnGuesserMixin):
     """
     Results of a SQL query.
 
     Can access rows listwise, or by string value of leftmost column.
     """
 
     def __init__(self, sqlaproxy, config):
         self.config = config
         self.keys = {}
+        self._results = []
 
-        is_sql_alchemy_results = not hasattr(sqlaproxy, "description")
+        # https://peps.python.org/pep-0249/#description
+        is_dbapi_results = hasattr(sqlaproxy, "description")
 
-        list.__init__(self, [])
         self.pretty = None
 
-        if is_sql_alchemy_results:
-            should_try_fetch_results = sqlaproxy.returns_rows
-        else:
+        if is_dbapi_results:
             should_try_fetch_results = True
+        else:
+            should_try_fetch_results = sqlaproxy.returns_rows
 
         if should_try_fetch_results:
-            if is_sql_alchemy_results:
+            # sql alchemy results
+            if not is_dbapi_results:
                 self.keys = sqlaproxy.keys()
             elif isinstance(sqlaproxy.description, Iterable):
                 self.keys = [i[0] for i in sqlaproxy.description]
             else:
                 self.keys = []
 
             if len(self.keys) > 0:
                 if isinstance(config.autolimit, int) and config.autolimit > 0:
-                    list.__init__(self, sqlaproxy.fetchmany(size=config.autolimit))
+                    self._results = sqlaproxy.fetchmany(size=config.autolimit)
                 else:
-                    list.__init__(self, sqlaproxy.fetchall())
+                    self._results = sqlaproxy.fetchall()
+
                 self.field_names = unduplicate_field_names(self.keys)
 
                 _style = None
+
                 if isinstance(config.style, str):
                     _style = prettytable.__dict__[config.style.upper()]
 
                 self.pretty = PrettyTable(self.field_names, style=_style)
 
     def _repr_html_(self):
         _cell_with_spaces_pattern = re.compile(r"(<td>)( {2,})")
         if self.pretty:
             self.pretty.add_rows(self)
             result = self.pretty.get_html_string()
             # to create clickable links
             result = html.unescape(result)
             result = _cell_with_spaces_pattern.sub(_nonbreaking_spaces, result)
-            if self.config.displaylimit and len(self) > self.config.displaylimit:
+            if len(self) > self.pretty.row_count:
                 HTML = (
                     '%s\n<span style="font-style:italic;text-align:center;">'
                     "%d rows, truncated to displaylimit of %d</span>"
+                    "<br>"
+                    '<span style="font-style:italic;text-align:center;">'
+                    "If you want to see more, please visit "
+                    '<a href="https://jupysql.ploomber.io/en/latest/api/configuration.html#displaylimit">displaylimit</a>'  # noqa: E501
+                    " configuration</span>"
                 )
-                result = HTML % (result, len(self), self.config.displaylimit)
+                result = HTML % (result, len(self), self.pretty.row_count)
             return result
         else:
             return None
 
+    def __len__(self):
+        return len(self._results)
+
+    def __iter__(self):
+        for result in self._results:
+            yield result
+
     def __str__(self, *arg, **kwarg):
-        self.pretty.add_rows(self)
+        if self.pretty:
+            self.pretty.add_rows(self)
         return str(self.pretty or "")
 
+    def __repr__(self) -> str:
+        return str(self)
+
+    def __eq__(self, another: object) -> bool:
+        return self._results == another
+
     def __getitem__(self, key):
         """
         Access by integer (row position within result set)
         or by string (value of leftmost column)
         """
         try:
-            return list.__getitem__(self, key)
+            return self._results[key]
         except TypeError:
             result = [row for row in self if row[0] == key]
             if not result:
                 raise KeyError(key)
             if len(result) > 1:
                 raise KeyError('%d results for "%s"' % (len(result), key))
             return result[0]
@@ -469,63 +494,96 @@
         return resultset.PolarsDataFrame(**config.polars_dataframe_kwargs)
     else:
         return resultset
     # returning only last result, intentionally
 
 
 def run(conn, sql, config):
+    """Run a SQL query with the given connection
+
+    Parameters
+    ----------
+    conn : sql.connection.Connection
+        The connection to use
+
+    sql : str
+        SQL query to execution
+
+    config
+        Configuration object
+    """
+    info = conn._get_curr_sqlalchemy_connection_info()
+
+    duckdb_autopandas = info and info.get("dialect") == "duckdb" and config.autopandas
+
     if not sql.strip():
         # returning only when sql is empty string
         return "Connected: %s" % conn.name
 
     for statement in sqlparse.split(sql):
         first_word = sql.strip().split()[0].lower()
         manual_commit = False
+
+        # attempting to run a transaction
         if first_word == "begin":
             raise exceptions.RuntimeError("JupySQL does not support transactions")
+
+        # postgres metacommand
         if first_word.startswith("\\") and is_postgres_or_redshift(conn.dialect):
             result = handle_postgres_special(conn, statement)
+
+        # regular query
         else:
-            txt = sqlalchemy.sql.text(statement)
             manual_commit = set_autocommit(conn, config)
-
             is_custom_connection = Connection.is_custom_connection(conn)
-            if is_custom_connection:
-                txt_ = str(txt)
+
+            # if regular sqlalchemy, pass a text object
+            if not is_custom_connection:
+                statement = sqlalchemy.sql.text(statement)
+
+            if duckdb_autopandas:
+                conn = conn.engine.raw_connection()
+                cursor = conn.cursor()
+                cursor.execute(str(statement))
+
             else:
-                txt_ = txt
-            # stringify txt to avoid TypeError:
-            # Boolean value of this clause is not defined
-            result = conn.session.execute(txt_)
-        _commit(conn=conn, config=config, manual_commit=manual_commit)
-        if result and config.feedback:
-            if hasattr(result, "rowcount"):
-                print(interpret_rowcount(result.rowcount))
+                result = conn.session.execute(statement)
+                _commit(conn=conn, config=config, manual_commit=manual_commit)
 
-    resultset = ResultSet(result, config)
-    return select_df_type(resultset, config)
+                if result and config.feedback:
+                    if hasattr(result, "rowcount"):
+                        print(interpret_rowcount(result.rowcount))
+
+    # bypass ResultSet and use duckdb's native method to return a pandas data frame
+    if duckdb_autopandas:
+        df = cursor.df()
+        conn.close()
+        return df
+    else:
+        resultset = ResultSet(result, config)
+        return select_df_type(resultset, config)
 
 
 def raw_run(conn, sql):
     return conn.session.execute(sqlalchemy.sql.text(sql))
 
 
 class PrettyTable(prettytable.PrettyTable):
     def __init__(self, *args, **kwargs):
         self.row_count = 0
-        self.displaylimit = None
+        self.displaylimit = DEFAULT_DISPLAYLIMIT_VALUE
         return super(PrettyTable, self).__init__(*args, **kwargs)
 
     def add_rows(self, data):
         if self.row_count and (data.config.displaylimit == self.displaylimit):
             return  # correct number of rows already present
         self.clear_rows()
         self.displaylimit = data.config.displaylimit
         if self.displaylimit == 0:
-            self.displaylimit = None  # TODO: remove this to make 0 really 0
+            self.displaylimit = None
         if self.displaylimit in (None, 0):
             self.row_count = len(data)
         else:
             self.row_count = min(len(data), self.displaylimit)
         for row in data[: self.displaylimit]:
             formatted_row = []
             for cell in row:
```

### Comparing `jupysql-0.7.4/src/sql/store.py` & `jupysql-0.7.5/src/sql/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Iterator, Iterable
 from collections.abc import MutableMapping
 from jinja2 import Template
 from ploomber_core.exceptions import modify_exceptions
 import sql.connection
-import warnings
 import difflib
 
 from sql import exceptions
 
 
 class SQLStore(MutableMapping):
     """Stores SQL scripts to render large queries with CTEs
@@ -89,20 +88,19 @@
 
     def __init__(self, store: SQLStore, query: str, with_: Iterable = None):
         self._store = store
         self._query = query
         self._with_ = with_ or []
 
         if any("-" in x for x in self._with_):
-            warnings.warn(
-                "Using hyphens will be deprecated soon, "
-                "please use "
+            raise exceptions.UsageError(
+                "Using hyphens is not allowed. "
+                "Please use "
                 + ", ".join(self._with_).replace("-", "_")
                 + " instead for the with argument.",
-                FutureWarning,
             )
 
     def __str__(self) -> str:
         """
         We use the ' (backtick symbol) to wrap the CTE alias if the dialect supports
         ` (backtick)
         """
```

### Comparing `jupysql-0.7.4/src/sql/util.py` & `jupysql-0.7.5/src/sql/util.py`

 * *Files identical despite different names*

