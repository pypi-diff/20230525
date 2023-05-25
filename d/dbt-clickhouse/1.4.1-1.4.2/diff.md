# Comparing `tmp/dbt-clickhouse-1.4.1.tar.gz` & `tmp/dbt-clickhouse-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-clickhouse-1.4.1.tar", last modified: Thu May 11 16:26:47 2023, max compression
+gzip compressed data, was "dbt-clickhouse-1.4.2.tar", last modified: Thu May 25 09:35:40 2023, max compression
```

## Comparing `dbt-clickhouse-1.4.1.tar` & `dbt-clickhouse-1.4.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.686782 dbt-clickhouse-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-05-11 16:26:47.686782 dbt-clickhouse-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14799 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.678781 dbt-clickhouse-1.4.1/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.678781 dbt-clickhouse-1.4.1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.682782 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/dbclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/httpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    14979 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/nativeclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.678781 dbt-clickhouse-1.4.1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.682782 dbt-clickhouse-1.4.1/dbt/include/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.682782 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.682782 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.686782 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/s3.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/view.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/persist_docs.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.686782 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/schema_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/schema_tests/relationships.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.686782 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/utils/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/utils/utils.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.686782 dbt-clickhouse-1.4.1/dbt_clickhouse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-05-11 16:26:47.000000 dbt-clickhouse-1.4.1/dbt_clickhouse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-11 16:26:47.000000 dbt-clickhouse-1.4.1/dbt_clickhouse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:26:47.000000 dbt-clickhouse-1.4.1/dbt_clickhouse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-11 16:26:47.000000 dbt-clickhouse-1.4.1/dbt_clickhouse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-11 16:26:47.000000 dbt-clickhouse-1.4.1/dbt_clickhouse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:26:47.686782 dbt-clickhouse-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:35:40.633093 dbt-clickhouse-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-05-25 09:35:40.633093 dbt-clickhouse-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14799 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:35:40.625093 dbt-clickhouse-1.4.2/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:35:40.625093 dbt-clickhouse-1.4.2/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:35:40.629093 dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/dbclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14979 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/nativeclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:35:40.625093 dbt-clickhouse-1.4.2/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:35:40.629093 dbt-clickhouse-1.4.2/dbt/include/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/include/clickhouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/include/clickhouse/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:35:40.629093 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:35:40.629093 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:35:40.629093 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/materializations/s3.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/materializations/view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/persist_docs.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:35:40.629093 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/schema_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/schema_tests/relationships.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:35:40.629093 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/utils/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/utils/utils.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:35:40.633093 dbt-clickhouse-1.4.2/dbt_clickhouse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-05-25 09:35:40.000000 dbt-clickhouse-1.4.2/dbt_clickhouse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-25 09:35:40.000000 dbt-clickhouse-1.4.2/dbt_clickhouse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:35:40.000000 dbt-clickhouse-1.4.2/dbt_clickhouse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-25 09:35:40.000000 dbt-clickhouse-1.4.2/dbt_clickhouse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 09:35:40.000000 dbt-clickhouse-1.4.2/dbt_clickhouse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:35:40.633093 dbt-clickhouse-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-25 09:35:37.000000 dbt-clickhouse-1.4.2/setup.py
```

### Comparing `dbt-clickhouse-1.4.1/LICENSE` & `dbt-clickhouse-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/PKG-INFO` & `dbt-clickhouse-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickhouse
-Version: 1.4.1
+Version: 1.4.2
 Summary: The Clickhouse plugin for dbt (data build tool)
 Home-page: https://github.com/ClickHouse/dbt-clickhouse
 Author: ClickHouse Inc.
 Author-email: guy@clickhouse.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dbt-clickhouse-1.4.1/README.md` & `dbt-clickhouse-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/__init__.py` & `dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/column.py` & `dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/column.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/connections.py` & `dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/credentials.py` & `dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/dbclient.py` & `dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/dbclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         if credentials.cluster_mode or credentials.database_engine == 'Replicated':
             self._conn_settings['database_replicated_enforce_synchronous_settings'] = '1'
             self._conn_settings['insert_quorum'] = 'auto'
         self._conn_settings['mutations_sync'] = '2'
         self._client = self._create_client(credentials)
         check_exchange = credentials.check_exchange and not credentials.cluster_mode
         try:
-            self._ensure_database(credentials.database_engine)
+            self._ensure_database(credentials.database_engine, credentials.cluster)
             self.server_version = self._server_version()
             self.has_lw_deletes, self.use_lw_deletes = self._check_lightweight_deletes(
                 credentials.use_lw_deletes
             )
             self.atomic_exchange = not check_exchange or self._check_atomic_exchange()
         except Exception as ex:
             self.close()
@@ -126,23 +126,24 @@
             return True, True
         except DbtDatabaseError as ex:
             logger.warning(
                 'use_lw_deletes requested but cannot enable on this ClickHouse server %s', str(ex)
             )
             return False, False
 
-    def _ensure_database(self, database_engine) -> None:
+    def _ensure_database(self, database_engine, cluster_name) -> None:
         if not self.database:
             return
         check_db = f'EXISTS DATABASE {self.database}'
         try:
             db_exists = self.command(check_db)
             if not db_exists:
                 engine_clause = f' ENGINE {database_engine} ' if database_engine else ''
-                self.command(f'CREATE DATABASE {self.database}{engine_clause}')
+                cluster_clause = f' ON CLUSTER {cluster_name} ' if cluster_name is not None else ''
+                self.command(f'CREATE DATABASE {self.database}{cluster_clause}{engine_clause}')
                 db_exists = self.command(check_db)
                 if not db_exists:
                     raise FailedToConnectError(
                         f'Failed to create database {self.database} for unknown reason'
                     )
         except DbtDatabaseError as ex:
             raise FailedToConnectError(
```

### Comparing `dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/httpclient.py` & `dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/httpclient.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/impl.py` & `dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/nativeclient.py` & `dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/nativeclient.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/relation.py` & `dbt-clickhouse-1.4.2/dbt/adapters/clickhouse/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/adapters/apply_grants.sql` & `dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/adapters/relation.sql` & `dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/adapters.sql` & `dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/adapters.sql`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,14 @@
     alter table {{ relation }} {{ on_cluster_clause()}} modify column {{ adapter.quote(column_name) }} {{ new_column_type }}
   {% endcall %}
 {% endmacro %}
 
 {% macro exchange_tables_atomic(old_relation, target_relation, obj_types='TABLES') %}
 
   {%- if adapter.get_clickhouse_cluster_name() is not none and obj_types == 'TABLES' %}
-    {% do run_query("SYSTEM SYNC REPLICA "+ target_relation.identifier + on_cluster_clause()) %}
+    {% do run_query("SYSTEM SYNC REPLICA " + on_cluster_clause() + target_relation.schema + '.' + target_relation.identifier) %}
   {%- endif %}
   
   {%- call statement('exchange_tables_atomic') -%}
     EXCHANGE {{ obj_types }} {{ old_relation }} AND {{ target_relation }} {{ on_cluster_clause()}}
   {% endcall %}
 {% endmacro %}
```

### Comparing `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/catalog.sql` & `dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/incremental.sql` & `dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/s3.sql` & `dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/materializations/s3.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/seed.sql` & `dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/snapshot.sql` & `dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/table.sql` & `dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/view.sql` & `dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/persist_docs.sql` & `dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/utils/utils.sql` & `dbt-clickhouse-1.4.2/dbt/include/clickhouse/macros/utils/utils.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/dbt_clickhouse.egg-info/PKG-INFO` & `dbt-clickhouse-1.4.2/dbt_clickhouse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickhouse
-Version: 1.4.1
+Version: 1.4.2
 Summary: The Clickhouse plugin for dbt (data build tool)
 Home-page: https://github.com/ClickHouse/dbt-clickhouse
 Author: ClickHouse Inc.
 Author-email: guy@clickhouse.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dbt-clickhouse-1.4.1/dbt_clickhouse.egg-info/SOURCES.txt` & `dbt-clickhouse-1.4.2/dbt_clickhouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.1/setup.py` & `dbt-clickhouse-1.4.2/setup.py`

 * *Files identical despite different names*

