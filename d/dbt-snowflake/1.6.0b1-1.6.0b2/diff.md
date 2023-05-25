# Comparing `tmp/dbt-snowflake-1.6.0b1.tar.gz` & `tmp/dbt-snowflake-1.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-snowflake-1.6.0b1.tar", last modified: Fri May 12 20:22:27 2023, max compression
+gzip compressed data, was "dbt-snowflake-1.6.0b2.tar", last modified: Thu May 25 21:25:52 2023, max compression
```

## Comparing `dbt-snowflake-1.6.0b1.tar` & `dbt-snowflake-1.6.0b2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.418135 dbt-snowflake-1.6.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-12 20:22:27.418135 dbt-snowflake-1.6.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.410135 dbt-snowflake-1.6.0b1/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.406135 dbt-snowflake-1.6.0b1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.410135 dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    20478 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.406135 dbt-snowflake-1.6.0b1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.410135 dbt-snowflake-1.6.0b1/dbt/include/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.414135 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.414135 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.414135 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.418135 dbt-snowflake-1.6.0b1/dbt_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-12 20:22:27.000000 dbt-snowflake-1.6.0b1/dbt_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-12 20:22:27.000000 dbt-snowflake-1.6.0b1/dbt_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:22:27.000000 dbt-snowflake-1.6.0b1/dbt_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:22:27.000000 dbt-snowflake-1.6.0b1/dbt_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-12 20:22:27.000000 dbt-snowflake-1.6.0b1/dbt_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-12 20:22:27.000000 dbt-snowflake-1.6.0b1/dbt_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 20:22:27.418135 dbt-snowflake-1.6.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.335729 dbt-snowflake-1.6.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-25 21:25:52.335729 dbt-snowflake-1.6.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.327728 dbt-snowflake-1.6.0b2/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.327728 dbt-snowflake-1.6.0b2/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.331728 dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20478 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.327728 dbt-snowflake-1.6.0b2/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.331728 dbt-snowflake-1.6.0b2/dbt/include/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.331728 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.331728 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.335729 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.335729 dbt-snowflake-1.6.0b2/dbt_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-25 21:25:52.000000 dbt-snowflake-1.6.0b2/dbt_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-25 21:25:52.000000 dbt-snowflake-1.6.0b2/dbt_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:25:52.000000 dbt-snowflake-1.6.0b2/dbt_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:25:52.000000 dbt-snowflake-1.6.0b2/dbt_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-25 21:25:52.000000 dbt-snowflake-1.6.0b2/dbt_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 21:25:52.000000 dbt-snowflake-1.6.0b2/dbt_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:25:52.335729 dbt-snowflake-1.6.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/setup.py
```

### Comparing `dbt-snowflake-1.6.0b1/LICENSE.md` & `dbt-snowflake-1.6.0b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b1/PKG-INFO` & `dbt-snowflake-1.6.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-snowflake
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: The Snowflake adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-snowflake
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.6.0b1 Summary: The
+Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.6.0b2 Summary: The
 Snowflake adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
 snowflake Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `dbt-snowflake-1.6.0b1/README.md` & `dbt-snowflake-1.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/__init__.py` & `dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/column.py` & `dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/column.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/connections.py` & `dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/impl.py` & `dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/adapters.sql` & `dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/catalog.sql` & `dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/incremental.sql` & `dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/merge.sql` & `dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/seed.sql` & `dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/table.sql` & `dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/table.sql`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 def materialize(session, df, target_relation):
     # make sure pandas exists
     import importlib.util
     package_name = 'pandas'
     if importlib.util.find_spec(package_name):
         import pandas
         if isinstance(df, pandas.core.frame.DataFrame):
+          session.use_database(target_relation.database)
+          session.use_schema(target_relation.schema)
           # session.write_pandas does not have overwrite function
           df = session.createDataFrame(df)
     {% set target_relation_name = resolve_model_name(target_relation) %}
     df.write.mode("overwrite").save_as_table('{{ target_relation_name }}', create_temp_table={{temporary}})
 
 def main(session):
     dbt = dbtObj(session.table)
```

### Comparing `dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/utils/timestamps.sql` & `dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b1/dbt/include/snowflake/profile_template.yml` & `dbt-snowflake-1.6.0b2/dbt/include/snowflake/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b1/dbt_snowflake.egg-info/PKG-INFO` & `dbt-snowflake-1.6.0b2/dbt_snowflake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-snowflake
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: The Snowflake adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-snowflake
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.6.0b1 Summary: The
+Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.6.0b2 Summary: The
 Snowflake adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
 snowflake Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `dbt-snowflake-1.6.0b1/dbt_snowflake.egg-info/SOURCES.txt` & `dbt-snowflake-1.6.0b2/dbt_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b1/setup.py` & `dbt-snowflake-1.6.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-snowflake"
-package_version = "1.6.0b1"
+package_version = "1.6.0b2"
 dbt_core_version = _get_dbt_core_version()
 description = """The Snowflake adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
```

