# Comparing `tmp/dbt-spark-1.6.0b1.tar.gz` & `tmp/dbt-spark-1.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-spark-1.6.0b1.tar", last modified: Fri May 12 20:59:40 2023, max compression
+gzip compressed data, was "dbt-spark-1.6.0b2.tar", last modified: Thu May 25 20:00:18 2023, max compression
```

## Comparing `dbt-spark-1.6.0b1.tar` & `dbt-spark-1.6.0b2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.069594 dbt-spark-1.6.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-12 20:59:40.069594 dbt-spark-1.6.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.061594 dbt-spark-1.6.0b1/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.061594 dbt-spark-1.6.0b1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.065594 dbt-spark-1.6.0b1/dbt/adapters/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/adapters/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/adapters/spark/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/adapters/spark/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    21120 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/adapters/spark/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    19051 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/adapters/spark/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/adapters/spark/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/adapters/spark/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/adapters/spark/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.061594 dbt-spark-1.6.0b1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.065594 dbt-spark-1.6.0b1/dbt/include/spark/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.065594 dbt-spark-1.6.0b1/dbt/include/spark/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/apply_grants.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.065594 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.065594 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/incremental/validate.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.069594 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/assert_not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.069594 dbt-spark-1.6.0b1/dbt_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-12 20:59:40.000000 dbt-spark-1.6.0b1/dbt_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-12 20:59:40.000000 dbt-spark-1.6.0b1/dbt_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:59:40.000000 dbt-spark-1.6.0b1/dbt_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:59:40.000000 dbt-spark-1.6.0b1/dbt_spark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-12 20:59:40.000000 dbt-spark-1.6.0b1/dbt_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-12 20:59:40.000000 dbt-spark-1.6.0b1/dbt_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 20:59:40.069594 dbt-spark-1.6.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.755314 dbt-spark-1.6.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-25 20:00:18.751314 dbt-spark-1.6.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.747314 dbt-spark-1.6.0b2/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.747314 dbt-spark-1.6.0b2/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.747314 dbt-spark-1.6.0b2/dbt/adapters/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/adapters/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/adapters/spark/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/adapters/spark/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21120 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/adapters/spark/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19485 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/adapters/spark/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/adapters/spark/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/adapters/spark/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/adapters/spark/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.747314 dbt-spark-1.6.0b2/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.747314 dbt-spark-1.6.0b2/dbt/include/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.751314 dbt-spark-1.6.0b2/dbt/include/spark/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    14681 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/apply_grants.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.751314 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.751314 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.751314 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/assert_not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/dbt/include/spark/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:18.751314 dbt-spark-1.6.0b2/dbt_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-25 20:00:18.000000 dbt-spark-1.6.0b2/dbt_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-25 20:00:18.000000 dbt-spark-1.6.0b2/dbt_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:00:18.000000 dbt-spark-1.6.0b2/dbt_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:00:18.000000 dbt-spark-1.6.0b2/dbt_spark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-25 20:00:18.000000 dbt-spark-1.6.0b2/dbt_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 20:00:18.000000 dbt-spark-1.6.0b2/dbt_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 20:00:18.755314 dbt-spark-1.6.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-25 20:00:06.000000 dbt-spark-1.6.0b2/setup.py
```

### Comparing `dbt-spark-1.6.0b1/PKG-INFO` & `dbt-spark-1.6.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-spark
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: The Apache Spark adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-spark Version: 1.6.0b1 Summary: The Apache
+Metadata-Version: 2.1 Name: dbt-spark Version: 1.6.0b2 Summary: The Apache
 Spark adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dbt-spark-1.6.0b1/README.md` & `dbt-spark-1.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/dbt/adapters/spark/column.py` & `dbt-spark-1.6.0b2/dbt/adapters/spark/column.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/dbt/adapters/spark/connections.py` & `dbt-spark-1.6.0b2/dbt/adapters/spark/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/dbt/adapters/spark/impl.py` & `dbt-spark-1.6.0b2/dbt/adapters/spark/impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import re
 from concurrent.futures import Future
 from dataclasses import dataclass
 from typing import Any, Dict, Iterable, List, Optional, Union, Type, Tuple, Callable
+
 from typing_extensions import TypeAlias
 
 import agate
-from dbt.contracts.relation import RelationType
 
 import dbt
 import dbt.exceptions
 
 from dbt.adapters.base import AdapterConfig, PythonJobHelper
-from dbt.adapters.base.impl import catch_as_completed
-from dbt.contracts.connection import AdapterResponse
+from dbt.adapters.base.impl import catch_as_completed, ConstraintSupport
 from dbt.adapters.sql import SQLAdapter
 from dbt.adapters.spark import SparkConnectionManager
 from dbt.adapters.spark import SparkRelation
 from dbt.adapters.spark import SparkColumn
 from dbt.adapters.spark.python_submissions import (
     JobClusterPythonJobHelper,
     AllPurposeClusterPythonJobHelper,
 )
 from dbt.adapters.base import BaseRelation
 from dbt.clients.agate_helper import DEFAULT_TYPE_TESTER
+from dbt.contracts.connection import AdapterResponse
+from dbt.contracts.graph.nodes import ConstraintType
+from dbt.contracts.relation import RelationType
 from dbt.events import AdapterLogger
 from dbt.utils import executor, AttrDict
 
 logger = AdapterLogger("Spark")
 
 GET_COLUMNS_IN_RELATION_RAW_MACRO_NAME = "get_columns_in_relation_raw"
 LIST_SCHEMAS_MACRO_NAME = "list_schemas"
@@ -75,22 +77,31 @@
         "stats:rows:value",
         "stats:rows:description",
         "stats:rows:include",
     )
     INFORMATION_COLUMNS_REGEX = re.compile(r"^ \|-- (.*): (.*) \(nullable = (.*)\b", re.MULTILINE)
     INFORMATION_OWNER_REGEX = re.compile(r"^Owner: (.*)$", re.MULTILINE)
     INFORMATION_STATISTICS_REGEX = re.compile(r"^Statistics: (.*)$", re.MULTILINE)
+
     HUDI_METADATA_COLUMNS = [
         "_hoodie_commit_time",
         "_hoodie_commit_seqno",
         "_hoodie_record_key",
         "_hoodie_partition_path",
         "_hoodie_file_name",
     ]
 
+    CONSTRAINT_SUPPORT = {
+        ConstraintType.check: ConstraintSupport.NOT_ENFORCED,
+        ConstraintType.not_null: ConstraintSupport.NOT_ENFORCED,
+        ConstraintType.unique: ConstraintSupport.NOT_ENFORCED,
+        ConstraintType.primary_key: ConstraintSupport.NOT_ENFORCED,
+        ConstraintType.foreign_key: ConstraintSupport.NOT_ENFORCED,
+    }
+
     Relation: TypeAlias = SparkRelation
     RelationInfo = Tuple[str, str, str]
     Column: TypeAlias = SparkColumn
     ConnectionManager: TypeAlias = SparkConnectionManager
     AdapterSpecificConfigs: TypeAlias = SparkConfig
 
     @classmethod
```

### Comparing `dbt-spark-1.6.0b1/dbt/adapters/spark/python_submissions.py` & `dbt-spark-1.6.0b2/dbt/adapters/spark/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/dbt/adapters/spark/relation.py` & `dbt-spark-1.6.0b2/dbt/adapters/spark/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/dbt/adapters/spark/session.py` & `dbt-spark-1.6.0b2/dbt/adapters/spark/session.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/dbt/include/spark/macros/adapters.sql` & `dbt-spark-1.6.0b2/dbt/include/spark/macros/adapters.sql`

 * *Files 2% similar despite different names*

```diff
@@ -179,35 +179,31 @@
 {% macro persist_constraints(relation, model) %}
   {{ return(adapter.dispatch('persist_constraints', 'dbt')(relation, model)) }}
 {% endmacro %}
 
 {% macro spark__persist_constraints(relation, model) %}
   {%- set contract_config = config.get('contract') -%}
   {% if contract_config.enforced and config.get('file_format', 'delta') == 'delta' %}
-    {% do alter_table_add_constraints(relation, model.columns) %}
+    {% do alter_table_add_constraints(relation, model.constraints) %}
     {% do alter_column_set_constraints(relation, model.columns) %}
   {% endif %}
 {% endmacro %}
 
 {% macro alter_table_add_constraints(relation, constraints) %}
   {{ return(adapter.dispatch('alter_table_add_constraints', 'dbt')(relation, constraints)) }}
 {% endmacro %}
 
-{% macro spark__alter_table_add_constraints(relation, column_dict) %}
-
-  {% for column_name in column_dict %}
-    {% set constraints = column_dict[column_name]['constraints'] %}
-    {% for constraint in constraints %}
-      {% if constraint.type == 'check' and not is_incremental() %}
-        {%- set constraint_hash = local_md5(column_name ~ ";" ~ constraint.expression ~ ";" ~ loop.index) -%}
-        {% call statement() %}
-          alter table {{ relation }} add constraint {{ constraint_hash }} check {{ constraint.expression }};
-        {% endcall %}
-      {% endif %}
-    {% endfor %}
+{% macro spark__alter_table_add_constraints(relation, constraints) %}
+  {% for constraint in constraints %}
+    {% if constraint.type == 'check' and not is_incremental() %}
+      {%- set constraint_hash = local_md5(column_name ~ ";" ~ constraint.expression ~ ";" ~ loop.index) -%}
+      {% call statement() %}
+        alter table {{ relation }} add constraint {{ constraint.name if constraint.name else constraint_hash }} check {{ constraint.expression }};
+      {% endcall %}
+    {% endif %}
   {% endfor %}
 {% endmacro %}
 
 {% macro alter_column_set_constraints(relation, column_dict) %}
   {{ return(adapter.dispatch('alter_column_set_constraints', 'dbt')(relation, column_dict)) }}
 {% endmacro %}
```

### Comparing `dbt-spark-1.6.0b1/dbt/include/spark/macros/apply_grants.sql` & `dbt-spark-1.6.0b2/dbt/include/spark/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/incremental/column_helpers.sql` & `dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/incremental/incremental.sql` & `dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/incremental/strategies.sql` & `dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/incremental/validate.sql` & `dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/seed.sql` & `dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/snapshot.sql` & `dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/table.sql` & `dbt-spark-1.6.0b2/dbt/include/spark/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/dateadd.sql` & `dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/datediff.sql` & `dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/listagg.sql` & `dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/split_part.sql` & `dbt-spark-1.6.0b2/dbt/include/spark/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/dbt/include/spark/profile_template.yml` & `dbt-spark-1.6.0b2/dbt/include/spark/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/dbt_spark.egg-info/PKG-INFO` & `dbt-spark-1.6.0b2/dbt_spark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-spark
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: The Apache Spark adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-spark Version: 1.6.0b1 Summary: The Apache
+Metadata-Version: 2.1 Name: dbt-spark Version: 1.6.0b2 Summary: The Apache
 Spark adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dbt-spark-1.6.0b1/dbt_spark.egg-info/SOURCES.txt` & `dbt-spark-1.6.0b2/dbt_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b1/setup.py` & `dbt-spark-1.6.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-spark"
-package_version = "1.6.0b1"
+package_version = "1.6.0b2"
 dbt_core_version = _get_dbt_core_version()
 description = """The Apache Spark adapter plugin for dbt"""
 
 odbc_extras = ["pyodbc~=4.0.30"]
 pyhive_extras = [
     "PyHive[hive]>=0.6.0,<0.7.0",
     "thrift>=0.11.0,<0.17.0",
```

