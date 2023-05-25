# Comparing `tmp/dbt-postgres-1.6.0b1.tar.gz` & `tmp/dbt-postgres-1.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-postgres-1.6.0b1.tar", last modified: Fri May 12 17:40:57 2023, max compression
+gzip compressed data, was "dbt-postgres-1.6.0b2.tar", last modified: Thu May 25 15:44:08 2023, max compression
```

## Comparing `dbt-postgres-1.6.0b1.tar` & `dbt-postgres-1.6.0b2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:57.594182 dbt-postgres-1.6.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-12 17:40:57.594182 dbt-postgres-1.6.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:57.590182 dbt-postgres-1.6.0b1/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:57.590182 dbt-postgres-1.6.0b1/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:57.590182 dbt-postgres-1.6.0b1/dbt/adapters/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/adapters/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/adapters/postgres/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/adapters/postgres/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/adapters/postgres/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/adapters/postgres/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/adapters/postgres/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:57.586182 dbt-postgres-1.6.0b1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:57.590182 dbt-postgres-1.6.0b1/dbt/include/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/include/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/include/postgres/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:57.590182 dbt-postgres-1.6.0b1/dbt/include/postgres/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/include/postgres/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/include/postgres/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:57.590182 dbt-postgres-1.6.0b1/dbt/include/postgres/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/include/postgres/macros/materializations/incremental_strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:57.590182 dbt-postgres-1.6.0b1/dbt/include/postgres/macros/materializations/materialized_view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/include/postgres/macros/materializations/materialized_view/create.sql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/include/postgres/macros/materializations/materialized_view/refresh.sql
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/include/postgres/macros/materializations/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/include/postgres/macros/relations.sql
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/include/postgres/macros/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:57.594182 dbt-postgres-1.6.0b1/dbt/include/postgres/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/include/postgres/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/include/postgres/macros/utils/columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/include/postgres/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/include/postgres/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/include/postgres/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/include/postgres/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/include/postgres/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/dbt/include/postgres/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:57.594182 dbt-postgres-1.6.0b1/dbt_postgres.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-12 17:40:57.000000 dbt-postgres-1.6.0b1/dbt_postgres.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-12 17:40:57.000000 dbt-postgres-1.6.0b1/dbt_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:40:57.000000 dbt-postgres-1.6.0b1/dbt_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:40:57.000000 dbt-postgres-1.6.0b1/dbt_postgres.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-12 17:40:57.000000 dbt-postgres-1.6.0b1/dbt_postgres.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-12 17:40:57.000000 dbt-postgres-1.6.0b1/dbt_postgres.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:40:57.594182 dbt-postgres-1.6.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-12 17:40:42.000000 dbt-postgres-1.6.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.744696 dbt-postgres-1.6.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-25 15:44:08.744696 dbt-postgres-1.6.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.740696 dbt-postgres-1.6.0b2/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.740696 dbt-postgres-1.6.0b2/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.740696 dbt-postgres-1.6.0b2/dbt/adapters/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/adapters/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/adapters/postgres/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/adapters/postgres/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/adapters/postgres/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/adapters/postgres/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/adapters/postgres/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.736696 dbt-postgres-1.6.0b2/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.740696 dbt-postgres-1.6.0b2/dbt/include/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.740696 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.740696 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/materializations/incremental_strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.740696 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/materializations/materialized_view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/materializations/materialized_view/create.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/materializations/materialized_view/refresh.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/relations.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.744696 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.744696 dbt-postgres-1.6.0b2/dbt_postgres.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-25 15:44:08.000000 dbt-postgres-1.6.0b2/dbt_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-25 15:44:08.000000 dbt-postgres-1.6.0b2/dbt_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:44:08.000000 dbt-postgres-1.6.0b2/dbt_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:44:08.000000 dbt-postgres-1.6.0b2/dbt_postgres.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-25 15:44:08.000000 dbt-postgres-1.6.0b2/dbt_postgres.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 15:44:08.000000 dbt-postgres-1.6.0b2/dbt_postgres.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:44:08.744696 dbt-postgres-1.6.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/setup.py
```

### Comparing `dbt-postgres-1.6.0b1/PKG-INFO` & `dbt-postgres-1.6.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-postgres
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: The postgres adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-postgres Version: 1.6.0b1 Summary: The postgres
+Metadata-Version: 2.1 Name: dbt-postgres Version: 1.6.0b2 Summary: The postgres
 adapter plugin for dbt (data build tool) Home-page: https://github.com/dbt-
 labs/dbt-core Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `dbt-postgres-1.6.0b1/README.md` & `dbt-postgres-1.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b1/dbt/adapters/postgres/__init__.py` & `dbt-postgres-1.6.0b2/dbt/adapters/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b1/dbt/adapters/postgres/connections.py` & `dbt-postgres-1.6.0b2/dbt/adapters/postgres/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b1/dbt/adapters/postgres/impl.py` & `dbt-postgres-1.6.0b2/dbt/adapters/postgres/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b1/dbt/adapters/postgres/relation.py` & `dbt-postgres-1.6.0b2/dbt/adapters/postgres/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b1/dbt/include/postgres/macros/adapters.sql` & `dbt-postgres-1.6.0b2/dbt/include/postgres/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b1/dbt/include/postgres/macros/catalog.sql` & `dbt-postgres-1.6.0b2/dbt/include/postgres/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b1/dbt/include/postgres/macros/materializations/snapshot_merge.sql` & `dbt-postgres-1.6.0b2/dbt/include/postgres/macros/materializations/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b1/dbt/include/postgres/macros/relations.sql` & `dbt-postgres-1.6.0b2/dbt/include/postgres/macros/relations.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b1/dbt/include/postgres/macros/timestamps.sql` & `dbt-postgres-1.6.0b2/dbt/include/postgres/macros/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b1/dbt/include/postgres/macros/utils/datediff.sql` & `dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b1/dbt/include/postgres/macros/utils/listagg.sql` & `dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b1/dbt_postgres.egg-info/PKG-INFO` & `dbt-postgres-1.6.0b2/dbt_postgres.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-postgres
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: The postgres adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-postgres Version: 1.6.0b1 Summary: The postgres
+Metadata-Version: 2.1 Name: dbt-postgres Version: 1.6.0b2 Summary: The postgres
 adapter plugin for dbt (data build tool) Home-page: https://github.com/dbt-
 labs/dbt-core Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `dbt-postgres-1.6.0b1/dbt_postgres.egg-info/SOURCES.txt` & `dbt-postgres-1.6.0b2/dbt_postgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b1/setup.py` & `dbt-postgres-1.6.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     # default to psycopg2-binary for all OSes/versions
     print(PSYCOPG2_MESSAGE)
     return "psycopg2-binary"
 
 
 package_name = "dbt-postgres"
-package_version = "1.6.0b1"
+package_version = "1.6.0b2"
 description = """The postgres adapter plugin for dbt (data build tool)"""
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 DBT_PSYCOPG2_NAME = _dbt_psycopg2_name()
```

