# Comparing `tmp/pydiverse-pipedag-0.2.4.tar.gz` & `tmp/pydiverse-pipedag-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiverse-pipedag-0.2.4.tar", max compression
+gzip compressed data, was "pydiverse-pipedag-0.3.0.tar", max compression
```

## Comparing `pydiverse-pipedag-0.2.4.tar` & `pydiverse-pipedag-0.3.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
--rw-r--r--   0        0        0     1517 2022-08-30 10:19:17.882077 pydiverse-pipedag-0.2.4/LICENSE
--rw-r--r--   0        0        0     7028 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.2.4/docs/package/README.md
--rw-r--r--   0        0        0     3466 2023-05-05 12:50:21.019475 pydiverse-pipedag-0.2.4/pyproject.toml
--rw-r--r--   0        0        0       13 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.4/src/pydiverse/.gitignore
--rw-r--r--   0        0        0      204 2022-12-07 13:24:39.752944 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/__init__.py
--rw-r--r--   0        0        0      749 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/_typing.py
--rw-r--r--   0        0        0       61 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/__init__.py
--rw-r--r--   0        0        0     5277 2023-05-05 10:44:44.012529 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/blob.py
--rw-r--r--   0        0        0    10555 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/lock.py
--rw-r--r--   0        0        0      177 2022-08-30 10:19:17.886078 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/__init__.py
--rw-r--r--   0        0        0    19418 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/base.py
--rw-r--r--   0        0        0     7232 2023-03-31 15:18:57.058051 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/dict.py
--rw-r--r--   0        0        0    79713 2023-05-05 10:44:44.012529 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/sql.py
--rw-r--r--   0        0        0       45 2023-01-06 19:08:19.182839 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/util/__init__.py
--rw-r--r--   0        0        0     1274 2023-01-06 19:08:19.182839 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py
--rw-r--r--   0        0        0    40345 2023-05-05 10:44:44.012529 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/util/sql_ddl.py
--rw-r--r--   0        0        0      342 2022-12-15 12:57:17.081298 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/context/__init__.py
--rw-r--r--   0        0        0     6241 2023-02-07 12:13:02.783303 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/context/context.py
--rw-r--r--   0        0        0    25109 2023-05-05 10:44:44.012529 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/context/run_context.py
--rw-r--r--   0        0        0      164 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/core/__init__.py
--rw-r--r--   0        0        0     9075 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/core/flow.py
--rw-r--r--   0        0        0     2512 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/core/result.py
--rw-r--r--   0        0        0     5714 2023-04-16 20:40:25.256504 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/core/stage.py
--rw-r--r--   0        0        0     6308 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/core/task.py
--rw-r--r--   0        0        0      285 2022-12-14 22:29:15.934795 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/engine/__init__.py
--rw-r--r--   0        0        0      648 2022-12-15 12:19:12.124658 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/engine/base.py
--rw-r--r--   0        0        0     6516 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/engine/prefect.py
--rw-r--r--   0        0        0     1380 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/engine/sequential.py
--rw-r--r--   0        0        0     1079 2022-12-14 22:31:58.730527 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/errors/__init__.py
--rw-r--r--   0        0        0      124 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/__init__.py
--rw-r--r--   0        0        0     8463 2023-04-17 10:28:16.433476 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/cache.py
--rw-r--r--   0        0        0     4332 2023-05-05 10:44:44.012529 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/container.py
--rw-r--r--   0        0        0     7739 2023-04-16 20:40:25.256504 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/core.py
--rw-r--r--   0        0        0     2039 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/metadata.py
--rw-r--r--   0        0        0    16598 2023-03-31 15:18:57.066051 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/store.py
--rw-r--r--   0        0        0       37 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/util/__init__.py
--rw-r--r--   0        0        0     1104 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/util/cache.py
--rw-r--r--   0        0        0     4231 2023-05-05 10:44:44.012529 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/util/json.py
--rw-r--r--   0        0        0      228 2023-01-14 15:50:16.896380 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/__init__.py
--rw-r--r--   0        0        0    14721 2023-04-16 20:40:25.256504 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/config.py
--rw-r--r--   0        0        0     2061 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/deep_map.py
--rw-r--r--   0        0        0     1435 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/deep_merge.py
--rw-r--r--   0        0        0      880 2022-12-14 22:31:58.730527 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/disposable.py
--rw-r--r--   0        0        0     1707 2022-12-15 13:01:08.984954 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/import_.py
--rw-r--r--   0        0        0     8982 2023-02-08 18:46:59.148930 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/ipc.py
--rw-r--r--   0        0        0      818 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/naming.py
--rw-r--r--   0        0        0     9297 2023-05-05 12:51:14.349947 pydiverse-pipedag-0.2.4/setup.py
--rw-r--r--   0        0        0     9432 2023-05-05 12:51:14.350385 pydiverse-pipedag-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1517 2022-08-30 10:19:17.882077 pydiverse-pipedag-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7358 2023-05-25 11:51:49.744305 pydiverse-pipedag-0.3.0/docs/package/README.md
+-rw-r--r--   0        0        0     3426 2023-05-25 11:51:49.756305 pydiverse-pipedag-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       13 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.3.0/src/pydiverse/.gitignore
+-rw-r--r--   0        0        0      204 2022-12-07 13:24:39.752944 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/__init__.py
+-rw-r--r--   0        0        0      749 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/_typing.py
+-rw-r--r--   0        0        0       88 2023-05-25 11:51:49.744305 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/__init__.py
+-rw-r--r--   0        0        0     5288 2023-05-25 11:51:49.744305 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/blob.py
+-rw-r--r--   0        0        0    10555 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/lock.py
+-rw-r--r--   0        0        0      177 2022-08-30 10:19:17.886078 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/__init__.py
+-rw-r--r--   0        0        0    20065 2023-05-25 11:51:49.744305 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/base.py
+-rw-r--r--   0        0        0     7267 2023-05-25 11:51:49.744305 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/dict.py
+-rw-r--r--   0        0        0    81824 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/sql.py
+-rw-r--r--   0        0        0       45 2023-01-06 19:08:19.182839 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/util/__init__.py
+-rw-r--r--   0        0        0     1274 2023-01-06 19:08:19.182839 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py
+-rw-r--r--   0        0        0      456 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/util/pandas.py
+-rw-r--r--   0        0        0    40408 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/util/sql_ddl.py
+-rw-r--r--   0        0        0    12334 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table_cache.py
+-rw-r--r--   0        0        0      342 2022-12-15 12:57:17.081298 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/context/__init__.py
+-rw-r--r--   0        0        0     7886 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/context/context.py
+-rw-r--r--   0        0        0    25109 2023-05-05 10:44:44.012529 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/context/run_context.py
+-rw-r--r--   0        0        0      164 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/core/__init__.py
+-rw-r--r--   0        0        0     9075 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/core/flow.py
+-rw-r--r--   0        0        0     2512 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/core/result.py
+-rw-r--r--   0        0        0     5714 2023-04-16 20:40:25.256504 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/core/stage.py
+-rw-r--r--   0        0        0     6308 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/core/task.py
+-rw-r--r--   0        0        0      285 2022-12-14 22:29:15.934795 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/engine/__init__.py
+-rw-r--r--   0        0        0      648 2022-12-15 12:19:12.124658 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/engine/base.py
+-rw-r--r--   0        0        0     6516 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/engine/prefect.py
+-rw-r--r--   0        0        0     1380 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/engine/sequential.py
+-rw-r--r--   0        0        0     1079 2022-12-14 22:31:58.730527 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/errors/__init__.py
+-rw-r--r--   0        0        0      124 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/__init__.py
+-rw-r--r--   0        0        0     8965 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/cache.py
+-rw-r--r--   0        0        0     4332 2023-05-05 10:44:44.012529 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/container.py
+-rw-r--r--   0        0        0     7940 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/core.py
+-rw-r--r--   0        0        0     2039 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/metadata.py
+-rw-r--r--   0        0        0    17651 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/store.py
+-rw-r--r--   0        0        0       37 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/util/__init__.py
+-rw-r--r--   0        0        0     1104 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/util/cache.py
+-rw-r--r--   0        0        0     4231 2023-05-05 10:44:44.012529 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/util/json.py
+-rw-r--r--   0        0        0      228 2023-01-14 15:50:16.896380 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/__init__.py
+-rw-r--r--   0        0        0    15639 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/config.py
+-rw-r--r--   0        0        0     2061 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/deep_map.py
+-rw-r--r--   0        0        0     1435 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/deep_merge.py
+-rw-r--r--   0        0        0      880 2022-12-14 22:31:58.730527 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/disposable.py
+-rw-r--r--   0        0        0     1707 2022-12-15 13:01:08.984954 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/import_.py
+-rw-r--r--   0        0        0     8982 2023-02-08 18:46:59.148930 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/ipc.py
+-rw-r--r--   0        0        0     1553 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/naming.py
+-rw-r--r--   0        0        0     9604 2023-05-25 11:52:05.977180 pydiverse-pipedag-0.3.0/setup.py
+-rw-r--r--   0        0        0     9743 2023-05-25 11:52:05.977721 pydiverse-pipedag-0.3.0/PKG-INFO
```

### Comparing `pydiverse-pipedag-0.2.4/LICENSE` & `pydiverse-pipedag-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/docs/package/README.md` & `pydiverse-pipedag-0.3.0/docs/package/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -107,16 +107,17 @@
 
 Create a file called `pipedag.yaml` in the same directory:
 
 ```yaml
 name: pipedag_tests
 table_store_connections:
   postgres:
-    # Postgres: this can be used after running `docker-compose up`
-    url: "postgresql://{$POSTGRES_USERNAME}:{$POSTGRES_PASSWORD}@127.0.0.1:6543/{instance_id}"
+    args:
+      # Postgres: this can be used after running `docker-compose up`  
+      url: "postgresql://{$POSTGRES_USERNAME}:{$POSTGRES_PASSWORD}@127.0.0.1:6543/{instance_id}"
 
 instances:
   __any__:
     # listen-interface for pipedag context server which synchronizes some task state during DAG execution
     network_interface: "127.0.0.1"
     # classes to be materialized to table store even without pipedag Table wrapper (we have loose coupling between
     # pipedag and pydiverse.transform, so consider adding 'pydiverse.transform.Table' in your config)
@@ -125,29 +126,40 @@
 
     instance_id: pipedag_default
     table_store:
       class: "pydiverse.pipedag.backend.table.SQLTableStore"
 
       # Postgres: this can be used after running `docker-compose up`
       table_store_connection: postgres
-      create_database_if_not_exists: True
-
-      # print select statements before being encapsualted in materialize expressions and tables before writing to
-      # database
-      print_materialize: true
-      # print final sql statements
-      print_sql: true
+      args:
+        create_database_if_not_exists: True
+        
+        # print select statements before being encapsualted in materialize expressions and tables before writing to
+        # database
+        print_materialize: true
+        # print final sql statements
+        print_sql: true
+
+      local_table_cache:
+        store_input: true
+        store_output: true
+        use_stored_input_as_cache: true
+        class: "pydiverse.pipedag.backend.table_cache.ParquetTableCache"
+        args:
+          base_path: "/tmp/pipedag/table_cache"
 
     blob_store:
       class: "pydiverse.pipedag.backend.blob.FileBlobStore"
-      base_path: "/tmp/pipedag/blobs"
+      args:
+        base_path: "/tmp/pipedag/blobs"
 
     lock_manager:
       class: "pydiverse.pipedag.backend.lock.ZooKeeperLockManager"
-      hosts: "localhost:2181"
+      args:
+        hosts: "localhost:2181"
 
     orchestration:
       class: "pydiverse.pipedag.engine.SequentialEngine"
 ```
 
 If you don't have a postgres, Microsoft SQL Server, or IBM DB2 database at hand, you can
 start a postgres database with the following `docker-compose.yaml` file:
```

### Comparing `pydiverse-pipedag-0.2.4/pyproject.toml` & `pydiverse-pipedag-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydiverse-pipedag"
-version = "0.2.4"
+version = "0.3.0"
 description = "A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files."
 authors = [
   "QuantCo, Inc.",
   "Nicolas Camenisch <garnele007@gmail.com>",
   "Martin Trautmann <windiana@users.sf.net>",
 ]
 license = "BSD-3-Clause"
@@ -30,14 +30,15 @@
 structlog = ">=22.1.0"
 tomli = ">=2.0.1"
 pynng = ">=0.7.1"
 msgpack = ">=1.0.4"
 packaging = ">=21.3"
 python-box = ">=6.1.0"
 PyYAML = ">=6.0"
+pyarrow = ">=11.0.0"
 
 filelock = { version = ">=3.7.1", optional = true }
 kazoo = { version = ">=2.8.0", optional = true }
 
 Sphinx = { version = ">=5.1.1", optional = true }
 sphinx-rtd-theme = { version = ">=1.0.0", optional = true }
 sphinxcontrib-apidoc = { version=">=0.3.0", optional = true }
@@ -47,29 +48,28 @@
 ibm-db = { version = ">=3.1.4", optional = true }
 ibm-db-sa = { version = ">=0.3.8", optional = true }
 pydiverse-transform = { version = ">=0.1.1", optional = true }
 ibis = { version = ">=3.2.0", optional = true }
 ibis-framework = {extras = ["mssql", "postgres"], version = "^5.1.0", optional = true }
 tidypolars = { version = ">=0.2.19", optional = true }
 connectorx = { version=">=0.3.1", optional = true }
-pyarrow = { version=">=11.0.0", optional = true }
 polars = { version=">=0.16.18,<0.17", optional = true }
 prefect = { version = ">=1.3,<2", optional = true }
 # for prefect 2 (radical change of paradigmns especially in task graph display => not ideal for rather linear pipeline)
 # prefect = { version = "prefect>=2.0,<3", optional = true }
 
 [tool.poetry.extras]
 filelock = ["filelock"]
 zookeeper = ["kazoo"]
 docs = ["Sphinx", "sphinx-rtd-theme", "sphinxcontrib-apidoc"]
 mssql = ["pyodbc", "pytsql"]
 ibm_db2 = ["ibm-db", "ibm-db-sa"]
 pdtransform = ["pydiverse-transform"]
 ibis = ["ibis", "ibis-framework"]
-polars = ["tidypolars", "polars", "connectorx", "pyarrow"]
+polars = ["tidypolars", "polars", "connectorx"]
 prefect = ["prefect", "docker-compose"]
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.2.0"
 pytest-mock = ">=3.10.0"
 pytest-timeout = ">=2.1.0"
 black = "^23.3.0"
```

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/_typing.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/_typing.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/blob.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/blob.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 class FileBlobStore(BaseBlobStore):
     """File based blob store
 
     The FileBlobStore stores blobs in a folder structure on a file system.
     In the base directory there will be two folders for every stage, one
     for the base and one for the transaction stage. Inside those folders the
     blobs will be stored as pickled files:
-    `/base_path/STAGE_NAME/BLOB_NAME.pkl`.
+    `base_path/instance_id/STAGE_NAME/BLOB_NAME.pkl`.
 
     To commit a stage, the only thing that has to be done is to rename
     the appropriate folders.
     """
 
     @classmethod
     def _init_conf_(cls, config: dict[str, Any]):
```

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/lock.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/lock.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/base.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from pydiverse.pipedag.materialize.metadata import (
     LazyTableMetadata,
     RawSqlMetadata,
     TaskMetadata,
 )
 from pydiverse.pipedag.materialize.util import compute_cache_key
 from pydiverse.pipedag.util import Disposable, requires
+from pydiverse.pipedag.util.naming import NameDisambiguator
 
 if TYPE_CHECKING:
     from pydiverse.pipedag import Stage
     from pydiverse.pipedag.materialize.core import MaterializingTask, TaskInfo
 
 
 class _TableStoreMeta(ABCMeta):
@@ -36,56 +37,19 @@
         cls._REGISTERED_TABLES = []
         cls._M_TABLE_CACHE = {}
         cls._R_TABLE_CACHE = {}
 
         return cls
 
 
-class BaseTableStore(Disposable, metaclass=_TableStoreMeta):
-    """Table store base class
-
-    The table store is responsible for storing and retrieving various types
-    of tabular data. Additionally, it also has to manage all task metadata,
-    This includes storing it, but also cleaning up stale metadata.
-
-    A store must use a table's name (`table.name`) and stage (`table.stage`)
-    as the primary keys for storing and retrieving it. This means that
-    two different `Table` objects can be used to store and retrieve the same
-    data as long as they have the same name and stage.
-
-    The same is also true for the task metadata where the task `stage`,
-    `version` and `cache_key` act as the primary keys (those values are
-    stored both in the task object and the metadata object).
-
-    To implement the stage transaction and commit mechanism, a technique
-    called schema swapping is used:
-
-    All outputs from materializing tasks get materialized into a temporary
-    empty schema (`stage.transaction_name`) and only if all tasks have
-    finished running *successfully* you swap the 'base schema' (original stage,
-    or cache) with the 'transaction schema'. This is usually done by renaming
-    them.
-
-    """
-
+class TableHookResolver(Disposable, metaclass=_TableStoreMeta):
     _REGISTERED_TABLES: list[TableHook]
     _M_TABLE_CACHE: dict[type, TableHook]
     _R_TABLE_CACHE: dict[type, TableHook]
 
-    def __init__(self):
-        self.logger = structlog.get_logger(type(self).__name__)
-
-    def setup(self):
-        """Setup function
-
-        This function gets called at the beginning of a flow run.
-        Unlike the __init__ method, a lock is acquired before
-        the setup method gets called to prevent race conditions.
-        """
-
     @classmethod
     def register_table(cls, *requirements: Any):
         """Decorator to register a `TableHook`
 
         Each table store should be able to handle tables of various different
         types (e.g. a pandas dataframe, a sqlalchemy select statement, a
         pydiverse transform table, ...). To add table type specific logic to
@@ -138,14 +102,107 @@
             return self._R_TABLE_CACHE[type_]
         for hook in self._REGISTERED_TABLES:
             if hook.can_retrieve(type_):
                 self._R_TABLE_CACHE[type_] = hook
                 return hook
         raise TypeError(f"Can't retrieve Table as type {type_}")
 
+    def store_table(
+        self,
+        table: Table,
+        task: MaterializingTask | None,
+        task_info: TaskInfo | None,
+        use_transaction_name=True,
+    ):
+        """Stores a table in the associated transaction stage
+
+        The store must convert the table object (`table.obj`) to the correct
+        internal type. This means, that in some cases it first has to
+        evaluate a lazy object. For example: if a sql based table store
+        receives a sql query to store, it has to execute it first.
+
+        The implementation details of this get handled by the registered
+        TableHooks.
+        """
+        _ = task  # not needed in this kind of store_table, yet
+        hook = self.get_m_table_hook(type(table.obj))
+        stage_name = (
+            table.stage.transaction_name if use_transaction_name else table.stage.name
+        )
+        hook.materialize(self, table, stage_name, task_info)
+
+    def retrieve_table_obj(
+        self,
+        table: Table,
+        as_type: type[T],
+        namer: NameDisambiguator | None = None,
+        use_transaction_name=True,
+    ) -> T:
+        """Loads a table from the store
+
+        Retrieves the table from the store, converts it to the correct
+        If the stage hasn't yet been committed, the table must be retrieved
+        from the transaction, else it must be retrieved from the committed
+        stage.
+
+        :raises TypeError: if the retrieved table can't be converted to
+            the requested type.
+        """
+
+        if as_type is None:
+            raise TypeError(
+                "Missing 'as_type' argument. You must specify a type to be able "
+                "to dematerialize a Table."
+            )
+
+        hook = self.get_r_table_hook(as_type)
+        stage_name = (
+            table.stage.current_name if use_transaction_name else table.stage.name
+        )
+        return hook.retrieve(self, table, stage_name, as_type, namer)
+
+
+class BaseTableStore(TableHookResolver):
+    """Table store base class
+
+    The table store is responsible for storing and retrieving various types
+    of tabular data. Additionally, it also has to manage all task metadata,
+    This includes storing it, but also cleaning up stale metadata.
+
+    A store must use a table's name (`table.name`) and stage (`table.stage`)
+    as the primary keys for storing and retrieving it. This means that
+    two different `Table` objects can be used to store and retrieve the same
+    data as long as they have the same name and stage.
+
+    The same is also true for the task metadata where the task `stage`,
+    `version` and `cache_key` act as the primary keys (those values are
+    stored both in the task object and the metadata object).
+
+    To implement the stage transaction and commit mechanism, a technique
+    called schema swapping is used:
+
+    All outputs from materializing tasks get materialized into a temporary
+    empty schema (`stage.transaction_name`) and only if all tasks have
+    finished running *successfully* you swap the 'base schema' (original stage,
+    or cache) with the 'transaction schema'. This is usually done by renaming
+    them.
+
+    """
+
+    def __init__(self):
+        self.logger = structlog.get_logger(type(self).__name__)
+
+    def setup(self):
+        """Setup function
+
+        This function gets called at the beginning of a flow run.
+        Unlike the __init__ method, a lock is acquired before
+        the setup method gets called to prevent race conditions.
+        """
+
     # Stage
 
     @abstractmethod
     def init_stage(self, stage: Stage):
         """Initialize a stage transaction
 
         When working with schema swapping:
@@ -166,29 +223,14 @@
 
         Additionally, the metadata associated with the transaction schema should
         replace the metadata of the base schema. The latter can be discarded.
         """
 
     # Materialize
 
-    def store_table(self, table: Table, task: MaterializingTask, task_info: TaskInfo):
-        """Stores a table in the associated transaction stage
-
-        The store must convert the table object (`table.obj`) to the correct
-        internal type. This means, that in some cases it first has to
-        evaluate a lazy object. For example: if a sql based table store
-        receives a sql query to store, it has to execute it first.
-
-        The implementation details of this get handled by the registered
-        TableHooks.
-        """
-        _ = task  # not needed in this kind of store_table, yet
-        hook = self.get_m_table_hook(type(table.obj))
-        hook.materialize(self, table, table.stage.transaction_name, task_info)
-
     def execute_raw_sql(self, raw_sql: RawSql):
         """Executed raw SQL statements in the associated transaction stage
 
         This method is overridden by actual table stores that can handle raw SQL.
         """
 
         raise NotImplementedError(
@@ -302,37 +344,14 @@
     @abstractmethod
     def delete_table_from_transaction(self, table: Table):
         """Delete a table from the transaction
 
         If the table doesn't exist in the transaction stage, fail silently.
         """
 
-    # Dematerialize
-
-    def retrieve_table_obj(self, table: Table, as_type: type[T]) -> T:
-        """Loads a table from the store
-
-        Retrieves the table from the store, converts it to the correct
-        If the stage hasn't yet been committed, the table must be retrieved
-        from the transaction, else it must be retrieved from the committed
-        stage.
-
-        :raises TypeError: if the retrieved table can't be converted to
-            the requested type.
-        """
-
-        if as_type is None:
-            raise TypeError(
-                "Missing 'as_type' argument. You must specify a type to be able "
-                "to dematerialize a Table."
-            )
-
-        hook = self.get_r_table_hook(as_type)
-        return hook.retrieve(self, table, table.stage.current_name, as_type)
-
     # Metadata
 
     @abstractmethod
     def store_task_metadata(self, metadata: TaskMetadata, stage: Stage):
         """Stores the metadata of a task
 
         The metadata must always be stored in such a way that it is
@@ -472,23 +491,29 @@
             be stored - can either be `stage.name` or `stage.transaction_name`.
         :param task_info: Information about task execution
         """
 
     @classmethod
     @abstractmethod
     def retrieve(
-        cls, store: StoreT, table: Table, stage_name: str, as_type: type[T]
+        cls,
+        store: StoreT,
+        table: Table,
+        stage_name: str,
+        as_type: type[T],
+        namer: NameDisambiguator | None = None,
     ) -> T:
         """Retrieve a table from the store
 
         :param store: The store in which the table is stored
         :param table: The table which should get retrieved
         :param stage_name: The name of the stage from which te table should
             be retrieved
         :param as_type: The type as which the table is to be retrieved
+        :param namer: Helper object which ensures unique alias names
         :return: The retrieved table (converted to the correct type)
         """
 
     @classmethod
     def auto_table(cls, obj: T) -> Table[T]:
         """Wrap an object inside a `Table`
```

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/dict.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/dict.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,23 +141,23 @@
 
     @classmethod
     def materialize(
         cls,
         store,
         table: Table[pd.DataFrame],
         stage_name,
-        task_info: TaskInfo,
+        task_info: TaskInfo | None,
     ):
         _ = task_info
         if table.name is not None:
             table.obj.attrs["name"] = table.name
         store.store[stage_name][table.name] = table.obj
 
     @classmethod
-    def retrieve(cls, store, table, stage_name, as_type):
+    def retrieve(cls, store, table, stage_name, as_type, namer):
         return store.store[stage_name][table.name].copy()
 
     @classmethod
     def auto_table(cls, obj: pd.DataFrame):
         if name := obj.attrs.get("name"):
             return Table(obj, name)
         return super().auto_table(obj)
@@ -184,27 +184,27 @@
 
     @classmethod
     def materialize(
         cls,
         store,
         table: Table[pdt.Table],
         stage_name,
-        task_info: TaskInfo,
+        task_info: TaskInfo | None,
     ):
         _ = task_info
         from pydiverse.transform.core.verbs import collect
 
         table.obj = table.obj >> collect()
         # noinspection PyTypeChecker
         return PandasTableHook.materialize(store, table, stage_name, task_info)
 
     @classmethod
-    def retrieve(cls, store, table, stage_name, as_type):
+    def retrieve(cls, store, table, stage_name, as_type, namer):
         from pydiverse.transform.eager import PandasTableImpl
 
-        df = PandasTableHook.retrieve(store, table, stage_name, pd.DataFrame)
+        df = PandasTableHook.retrieve(store, table, stage_name, pd.DataFrame, namer)
         return pdt.Table(PandasTableImpl(table.name, df))
 
     @classmethod
     def auto_table(cls, obj: pdt.Table):
         # noinspection PyProtectedMember
         return Table(obj, obj._impl.name)
```

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/sql.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import pandas as pd
 import sqlalchemy as sa
 import sqlalchemy.exc
 import sqlalchemy.sql.elements
 from sqlalchemy.dialects.mssql import DATETIME2
 
 from pydiverse.pipedag import Stage, Table
+from pydiverse.pipedag._typing import T
 from pydiverse.pipedag.backend.table.base import BaseTableStore, TableHook
 from pydiverse.pipedag.backend.table.util import engine_dispatch
 from pydiverse.pipedag.backend.table.util.sql_ddl import (
     AddIndex,
     AddPrimaryKey,
     ChangeColumnNullable,
     ChangeColumnTypes,
@@ -53,14 +54,15 @@
 from pydiverse.pipedag.materialize.metadata import (
     LazyTableMetadata,
     RawSqlMetadata,
     TaskMetadata,
 )
 from pydiverse.pipedag.materialize.util import compute_cache_key
 from pydiverse.pipedag.util.ipc import human_thread_id
+from pydiverse.pipedag.util.naming import NameDisambiguator
 
 
 class SQLTableStore(BaseTableStore):
     """Table store that materializes tables to a SQL database
 
     Uses schema swapping for transactions:
     Creates a schema for each stage and a temporary schema for each
@@ -68,14 +70,15 @@
     renaming them.
     """
 
     METADATA_SCHEMA = "pipedag_metadata"
 
     @classmethod
     def _init_conf_(cls, config: dict[str, Any]):
+        config = config.copy()
         engine_url = config.pop("url")
         return cls(engine_url, **config)
 
     def __init__(
         self,
         engine_url: str,
         create_database_if_not_exists: bool = False,
@@ -349,14 +352,25 @@
             with conn.begin():
                 for part in split_ddl_statement(query_str):
                     self._execute(part, conn)
             return
 
         return self._execute(query, conn)
 
+    @engine_dispatch
+    def name_adj(self, name: str):
+        # some dialects need to replace all lowercase names by uppercase because
+        # they create uppercase table names by default
+        return name
+
+    @name_adj.dialect("ibm_db_sa")
+    def _name_adj_ibm_db_sa(self, name: str):
+        # DB2 creates tables uppercase if all lowercase given
+        return name.upper() if name.islower() else name
+
     def add_indexes(
         self, table: Table, schema: Schema, *, early_not_null_possible: bool = False
     ):
         if table.primary_key is not None:
             key = table.primary_key
             if isinstance(key, str):
                 key = [key]
@@ -472,23 +486,27 @@
     # ):
     #     self.execute(AddIndex(table_name, schema, index, name))
 
     def copy_indexes(
         self, src_table: str, src_schema: Schema, dest_table: str, dest_schema: Schema
     ):
         inspector = sa.inspect(self.engine)
-        pk_constraint = inspector.get_pk_constraint(src_table, schema=src_schema.get())
+        pk_constraint = inspector.get_pk_constraint(
+            self.name_adj(src_table), schema=self.name_adj(src_schema.get())
+        )
         if len(pk_constraint["constrained_columns"]) > 0:
             self.add_primary_key(
                 dest_table,
                 dest_schema,
                 pk_constraint["constrained_columns"],
                 name=pk_constraint["name"],
             )
-        indexes = inspector.get_indexes(src_table, schema=src_schema.get())
+        indexes = inspector.get_indexes(
+            self.name_adj(src_table), schema=self.name_adj(src_schema.get())
+        )
         for index in indexes:
             if len(index["include_columns"]) > 0:
                 self.logger.warning(
                     "Perfect index recreation in caching is not net implemented",
                     table=dest_table,
                     schema=dest_schema.get(),
                     include_columns=index["include_columns"],
@@ -507,15 +525,17 @@
                 dest_table, dest_schema, index["column_names"], index["name"]
             )
 
     def reflect_sql_types(
         self, col_names: Iterable[str], table_name: str, schema: Schema
     ):
         inspector = sa.inspect(self.engine)
-        columns = inspector.get_columns(table_name, schema=schema.get())
+        columns = inspector.get_columns(
+            self.name_adj(table_name), schema=self.name_adj(schema.get())
+        )
         types = {d["name"]: d["type"] for d in columns}
         sql_types = [types[col] for col in col_names]
         return sql_types
 
     @staticmethod
     def format_sql_string(query_str: str) -> str:
         return textwrap.dedent(query_str).strip()
@@ -648,17 +668,21 @@
 
         with self.engine_connect() as conn:
             if self.avoid_drop_create_schema:
                 # empty tansaction_schema by deleting all tables and views
                 # Attention: similar code in sql_ddl.py:visit_drop_schema_ibm_db_sa
                 # for drop.cascade=True
                 inspector = sa.inspect(self.engine)
-                for table in inspector.get_table_names(schema=transaction_schema.get()):
+                for table in inspector.get_table_names(
+                    schema=self.name_adj(transaction_schema.get())
+                ):
                     self.execute(DropTable(table, schema=transaction_schema))
-                for view in inspector.get_view_names(schema=transaction_schema.get()):
+                for view in inspector.get_view_names(
+                    schema=self.name_adj(transaction_schema.get())
+                ):
                     self.execute(DropView(view, schema=transaction_schema))
                 self.drop_all_dialect_specific(schema=transaction_schema)
             else:
                 self.execute(cs_base, conn=conn)
                 self.execute(ds_trans, conn=conn)
                 self.execute(cs_trans, conn=conn)
 
@@ -861,15 +885,17 @@
         dest_schema: Schema,
         src_schema: Schema,
         src_tables: Iterable[sa.Table],
     ):
         _ = src_schema  # only needed by other dialects
         for table in src_tables:
             self.execute(
-                CreateViewAsSelect(table.name, dest_schema, sa.select(table)),
+                CreateViewAsSelect(
+                    table.name, dest_schema, sa.select("*").select_from(table)
+                ),
                 conn=conn,
             )
 
     @_create_read_views.dialect("ibm_db_sa")
     def _create_read_views_ibm_db_sa(
         self, conn, dest_schema, src_schema: Schema, src_tables: Iterable[sa.Table]
     ):
@@ -898,15 +924,17 @@
                     .where(table.c.stage == stage.name)
                     .values(in_transaction_schema=False)
                 )
 
     def copy_table_to_transaction(self, table: Table):
         stage = table.stage
         schema_name = self.get_schema(stage.name).get()
-        has_table = sa.inspect(self.engine).has_table(table.name, schema=schema_name)
+        has_table = sa.inspect(self.engine).has_table(
+            self.name_adj(table.name), schema=self.name_adj(schema_name)
+        )
         if not has_table:
             raise RuntimeError(
                 f"Can't copy table '{table.name}' (schema: '{stage.name}')"
                 " to transaction because no such table exists."
             )
 
         try:
@@ -1005,15 +1033,17 @@
                 f" '{dest_schema.get()}') in place of alias."
             )
             raise RuntimeError(msg) from _e
 
     def copy_lazy_table_to_transaction(self, metadata: LazyTableMetadata, table: Table):
         stage = table.stage
         schema_name = self.get_schema(metadata.stage).get()
-        has_table = sa.inspect(self.engine).has_table(metadata.name, schema=schema_name)
+        has_table = sa.inspect(self.engine).has_table(
+            self.name_adj(metadata.name), schema=self.name_adj(schema_name)
+        )
         if not has_table:
             msg = (
                 f"Can't copy lazy table '{metadata.name}' (schema:"
                 f" '{metadata.stage}') to transaction because no such table"
                 " exists."
             )
             self.logger.error(msg)
@@ -1059,15 +1089,15 @@
         :param include_everything: If True, we might include stored procedures,
             functions and other database objects that have a schema associated name.
             Currently, this only makes a difference for dialect=mssql.
         :return: list of view names [and other objects]
         """
         _ = include_everything  # not used in this implementation
         inspector = sa.inspect(self.engine)
-        return inspector.get_view_names(schema)
+        return inspector.get_view_names(self.name_adj(schema))
 
     @get_view_names.dialect("mssql")
     def _get_view_names_mssql(self, schema: str, *, include_everything=False):
         if not include_everything:
             return self.get_view_names.original(
                 self, schema, include_everything=include_everything
             )
@@ -1401,15 +1431,15 @@
         :param include_everything: If True, we might include stored procedures,
             functions and other database objects that have a schema associated name.
         :return: list of tables [and other objects]
         """
         inspector = sa.inspect(self.engine)
         schema = self.get_schema(stage.transaction_name).get()
 
-        table_names = inspector.get_table_names(schema)
+        table_names = inspector.get_table_names(self.name_adj(schema))
         view_names = self.get_view_names(schema, include_everything=include_everything)
 
         return table_names + view_names
 
     def get_stage_hash(self, stage: Stage) -> str:
         """Compute hash that represents entire stage's output metadata."""
         # We only need to look in tasks_table since the output_json column is updated
@@ -1444,19 +1474,19 @@
 
     @classmethod
     def materialize(
         cls,
         store,
         table: Table[sa.sql.elements.TextClause | sa.Text],
         stage_name,
-        task_info: TaskInfo,
+        task_info: TaskInfo | None,
     ):
         obj = table.obj
-        if isinstance(table.obj, sa.Table):
-            obj = sa.select(table.obj)
+        if isinstance(table.obj, (sa.Table, sa.sql.selectable.Alias)):
+            obj = sa.select("*").select_from(table.obj)
 
         source_tables = [
             dict(
                 name=tbl.name,
                 schema=store.get_schema(
                     tbl.stage.transaction_name
                     if tbl.stage in task_info.open_stages
@@ -1474,38 +1504,41 @@
                 early_not_null=table.primary_key,
                 source_tables=source_tables,
             )
         )
         store.add_indexes(table, schema, early_not_null_possible=True)
 
     @classmethod
-    def retrieve(cls, store, table, stage_name, as_type):
+    def retrieve(
+        cls, store, table, stage_name, as_type: type[sa.Table], namer=None
+    ) -> sa.sql.selectable.Selectable:
         table_name = table.name
         schema = store.get_schema(stage_name).get()
         table_name, schema = store.resolve_aliases(table_name, schema)
+        tbl = None
         for retry_iteration in range(4):
             # retry operation since it might have been terminated as a deadlock victim
             try:
                 tbl = sa.Table(
                     table_name,
                     sa.MetaData(),
                     schema=schema,
                     autoload_with=store.engine,
-                )
+                ).alias(namer.get_name(table_name))
                 break
             except (sa.exc.SQLAlchemyError, sa.exc.DBAPIError):
                 if retry_iteration == 3:
                     raise
                 time.sleep(retry_iteration * retry_iteration * 1.2)
         return tbl
 
     @classmethod
     def lazy_query_str(cls, store, obj) -> str:
         if isinstance(obj, sa.sql.selectable.FromClause):
-            query = sa.select(sa.text("*")).select_from(obj)
+            query = sa.select("*").select_from(obj)
         else:
             query = obj
         query_str = str(
             query.compile(store.engine, compile_kwargs={"literal_binds": True})
         )
         # hacky way to canonicalize query (despite __tmp/__even/__odd suffixes
         # and alias resolution)
@@ -1582,25 +1615,14 @@
         table_name = parts[2]
         table_name, schema = _resolve_alias_mssql(
             conn, table_name, schema, _iteration=_iteration + 1
         )
     return table_name, schema
 
 
-def adj_pandas_types(df: pd.DataFrame):
-    df = df.copy()
-    for col in df.dtypes.loc[lambda x: x == int].index:
-        df[col] = df[col].astype(pd.Int64Dtype())
-    for col in df.dtypes.loc[lambda x: x == bool].index:
-        df[col] = df[col].astype(pd.BooleanDtype())
-    for col in df.dtypes.loc[lambda x: x == object].index:
-        df[col] = df[col].astype(pd.StringDtype())
-    return df
-
-
 @SQLTableStore.register_table(pd)
 class PandasTableHook(TableHook[SQLTableStore]):
     """
     Materalize pandas->sql and retrieve sql->pandas.
 
     We like to limit the use of types, so operations can be implemented reliably
     without the use of pandas dtype=object where every row can have different type:
@@ -1629,15 +1651,15 @@
 
     @classmethod
     def materialize(
         cls,
         store,
         table: Table[pd.DataFrame],
         stage_name,
-        task_info: TaskInfo,
+        task_info: TaskInfo | None,
     ):
         # we might try to avoid this copy for speedup / saving RAM
         df = table.obj.copy()
         schema = store.get_schema(stage_name)
         if store.print_materialize:
             store.logger.info(
                 f"Writing table '{schema.get()}.{table.name}':\n{table.obj}"
@@ -1721,15 +1743,22 @@
                 else:
                     cols[name] = sa.func.least(
                         max_date, sa.func.greatest(min_date, cols[name])
                     ).label(name)
         return cols, year_cols
 
     @classmethod
-    def retrieve(cls, store, table, stage_name, as_type):
+    def retrieve(
+        cls,
+        store: SQLTableStore,
+        table: Table,
+        stage_name: str,
+        as_type: type[pd.DataFrame],
+        namer: NameDisambiguator | None = None,
+    ) -> pd.DataFrame:
         schema = store.get_schema(stage_name).get()
         with store.engine.connect() as conn:
             table_name = table.name
             table_name, schema = store.resolve_aliases(table_name, schema)
             for retry_iteration in range(4):
                 # retry operation since it might have been terminated as a
                 # deadlock victim
@@ -1794,15 +1823,15 @@
 
     @classmethod
     def materialize(
         cls,
         store,
         table: Table[polars.dataframe.DataFrame],
         stage_name,
-        task_info: TaskInfo,
+        task_info: TaskInfo | None,
     ):
         schema = store.get_schema(stage_name)
         if store.print_materialize:
             store.logger.info(
                 f"Writing table '{schema.get()}.{table.name}':\n{table.obj}"
             )
         table_name = table.name
@@ -1819,24 +1848,32 @@
         #     table_name = ibm_db_sa_fix_name(table_name)
         table.obj.to_pandas(use_pyarrow_extension_array=True).to_sql(
             name=table_name, con=store.engine, schema=schema.get(), index=False
         )
         store.add_indexes(table, schema)
 
     @classmethod
-    def retrieve(cls, store, table, stage_name, as_type):
+    def retrieve(
+        cls,
+        store: SQLTableStore,
+        table: Table,
+        stage_name: str,
+        as_type: type[polars.dataframe.DataFrame],
+        namer: NameDisambiguator | None = None,
+    ) -> polars.dataframe.DataFrame:
         schema = store.get_schema(stage_name).get()
         table_name = table.name
         table_name, schema = store.resolve_aliases(table_name, schema)
         conn = str(store.engine_url_obj)
         df = polars.read_database(f'SELECT * FROM {schema}."{table_name}"', conn)
         return df
 
     @classmethod
     def auto_table(cls, obj: polars.dataframe.DataFrame):
+        # currently, we don't know how to store a table name inside polars dataframe
         return super().auto_table(obj)
 
 
 try:
     # optional dependency to polars
     import tidypolars
 except ImportError as e:
@@ -1856,27 +1893,37 @@
 
     @classmethod
     def materialize(
         cls,
         store,
         table: Table[tidypolars.Tibble],
         stage_name,
-        task_info: TaskInfo,
+        task_info: TaskInfo | None,
     ):
+        tibble = table.obj
+        table.obj = None
         table = copy.deepcopy(table)
-        table.obj = table.obj.to_polars()
+        table.obj = tibble.to_polars()
         PolarsTableHook.materialize(store, table, stage_name, task_info)
 
     @classmethod
-    def retrieve(cls, store, table, stage_name, as_type):
-        df = PolarsTableHook.retrieve(store, table, stage_name, as_type)
+    def retrieve(
+        cls,
+        store: SQLTableStore,
+        table: Table,
+        stage_name: str,
+        as_type: type[tidypolars.Tibble],
+        namer: NameDisambiguator | None = None,
+    ) -> tidypolars.Tibble:
+        df = PolarsTableHook.retrieve(store, table, stage_name, as_type, namer)
         return tidypolars.from_polars(df)
 
     @classmethod
     def auto_table(cls, obj: tidypolars.Tibble):
+        # currently, we don't know how to store a table name inside tidypolars tibble
         return super().auto_table(obj)
 
 
 try:
     # optional dependency to pydiverse-transform
     import pydiverse.transform as pdt
 except ImportError as e:
@@ -1896,42 +1943,53 @@
         from pydiverse.transform.eager import PandasTableImpl
         from pydiverse.transform.lazy import SQLTableImpl
 
         return issubclass(type_, (PandasTableImpl, SQLTableImpl))
 
     @classmethod
     def materialize(
-        cls, store, table: Table[pdt.Table], stage_name, task_info: TaskInfo
+        cls, store, table: Table[pdt.Table], stage_name, task_info: TaskInfo | None
     ):
         from pydiverse.transform.eager import PandasTableImpl
         from pydiverse.transform.lazy import SQLTableImpl
 
         t = table.obj
+        table.obj = None
+        table = copy.deepcopy(table)
         if isinstance(t._impl, PandasTableImpl):
             from pydiverse.transform.core.verbs import collect
 
             table.obj = t >> collect()
             # noinspection PyTypeChecker
             return PandasTableHook.materialize(store, table, stage_name, task_info)
         if isinstance(t._impl, SQLTableImpl):
             table.obj = t._impl.build_select()
             # noinspection PyTypeChecker
             return SQLAlchemyTableHook.materialize(store, table, stage_name, task_info)
         raise NotImplementedError
 
     @classmethod
-    def retrieve(cls, store, table, stage_name, as_type):
+    def retrieve(
+        cls,
+        store: SQLTableStore,
+        table: Table,
+        stage_name: str,
+        as_type: type[T],
+        namer: NameDisambiguator | None = None,
+    ) -> T:
         from pydiverse.transform.eager import PandasTableImpl
         from pydiverse.transform.lazy import SQLTableImpl
 
         if issubclass(as_type, PandasTableImpl):
-            df = PandasTableHook.retrieve(store, table, stage_name, pd.DataFrame)
+            df = PandasTableHook.retrieve(store, table, stage_name, pd.DataFrame, namer)
             return pdt.Table(PandasTableImpl(table.name, df))
         if issubclass(as_type, SQLTableImpl):
-            sa_tbl = SQLAlchemyTableHook.retrieve(store, table, stage_name, sa.Table)
+            sa_tbl = SQLAlchemyTableHook.retrieve(
+                store, table, stage_name, sa.Table, namer
+            )
             return pdt.Table(SQLTableImpl(store.engine, sa_tbl))
         raise NotImplementedError
 
     @classmethod
     def auto_table(cls, obj: pdt.Table):
         return Table(obj, obj._impl.name)
 
@@ -1996,22 +2054,36 @@
 
     @classmethod
     def can_retrieve(cls, type_) -> bool:
         return issubclass(type_, ibis_types.Table)
 
     @classmethod
     def materialize(
-        cls, store, table: Table[ibis_types.Table], stage_name, task_info: TaskInfo
+        cls,
+        store,
+        table: Table[ibis_types.Table],
+        stage_name,
+        task_info: TaskInfo | None,
     ):
         t = table.obj
-        table.obj = sa.text(cls.lazy_query_str(store, t))
-        return SQLAlchemyTableHook.materialize(store, table, stage_name, task_info)
+        table.obj = None
+        # noinspection PyTypeChecker
+        sa_table = copy.deepcopy(table)  # type: Table[sa.Text]
+        sa_table.obj = sa.text(cls.lazy_query_str(store, t))
+        return SQLAlchemyTableHook.materialize(store, sa_table, stage_name, task_info)
 
     @classmethod
-    def retrieve(cls, store, table, stage_name, as_type):
+    def retrieve(
+        cls,
+        store: SQLTableStore,
+        table: Table,
+        stage_name: str,
+        as_type: type[ibis_types.Table],
+        namer: NameDisambiguator | None = None,
+    ) -> ibis_types.Table:
         con = cls.get_con(store)
         table_name = table.name
         schema = store.get_schema(stage_name).get()
         table_name, schema = store.resolve_aliases(table_name, schema)
         for retry_iteration in range(4):
             # retry operation since it might have been terminated as a deadlock victim
             try:
```

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/util/sql_ddl.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/util/sql_ddl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1148,14 +1148,15 @@
     ]
     statements.append(f"call sysproc.admin_cmd('REORG TABLE {schema}.{table}')")
     return statements
 
 
 def ibm_db_sa_fix_name(name):
     # DB2 seems to create tables uppercase if all lowercase given
+    # TODO: consider moving this replacement to call in sql.py
     return name.upper() if name.islower() else name
 
 
 STATEMENT_SEPERATOR = "; -- PYDIVERSE-PIPEDAG-SPLIT\n"
 
 
 def join_ddl_statements(statements, compiler, **kw):
```

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/context/context.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/context/context.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,16 +16,14 @@
     from pydiverse.pipedag.core import Flow, Stage, Task
     from pydiverse.pipedag.engine.base import OrchestrationEngine
     from pydiverse.pipedag.materialize.metadata import TaskMetadata
 
 import structlog
 from attrs import define, frozen
 
-logger = structlog.get_logger()
-
 
 class BaseContext:
     _context_var: ClassVar[ContextVar]
     _token: Token = None
     _enter_counter: int = 0
     _lock: Lock = Lock()
 
@@ -125,14 +123,15 @@
     pipedag_name: str
     flow_name: str
     instance_name: str
 
     # per instance attributes
     fail_fast: bool
     strict_result_get_locking: bool
+    ignore_task_version: bool
     instance_id: str  # may be used as database name or locking ID
     stage_commit_technique: StageCommitTechnique
     network_interface: str
     attrs: dict[str, Any]
 
     @cached_property
     def auto_table(self) -> tuple[type, ...]:
@@ -141,21 +140,60 @@
     @cached_property
     def auto_blob(self) -> tuple[type, ...]:
         return tuple(map(import_object, self.config_dict.get("auto_blob", ())))
 
     @cached_property
     def store(self):
         # Load objects referenced in config
-        table_store = load_object(self.config_dict["table_store"])
-        blob_store = load_object(self.config_dict["blob_store"])
+        try:
+            from pydiverse.pipedag.backend.table_cache import LocalTableCache
+
+            table_store = load_object(self.config_dict["table_store"])
+            if "local_table_cache" in self.config_dict["table_store"]:
+                local_cache_cfg = self.config_dict["table_store"]["local_table_cache"]
+                local_table_cache = LocalTableCache(
+                    load_object(local_cache_cfg),
+                    local_cache_cfg.get("store_input", True),
+                    local_cache_cfg.get("store_output", False),
+                    local_cache_cfg.get("use_stored_input_as_cache", True),
+                )
+                unknown_attributes = set(local_cache_cfg.keys()) - {
+                    "class",
+                    "args",
+                    "store_input",
+                    "store_output",
+                    "use_stored_input_as_cache",
+                }
+                if len(unknown_attributes) > 0:
+                    raise AttributeError(
+                        (
+                            "Unknown attributes in local_table_cache config:"
+                            f" {unknown_attributes}"
+                        ),
+                    )
+            else:
+                local_table_cache = LocalTableCache(
+                    None,
+                    store_input=False,
+                    store_output=False,
+                    use_stored_input_as_cache=False,
+                )
+        except Exception as e:
+            raise RuntimeError("Failed loading table_store") from e
+
+        try:
+            blob_store = load_object(self.config_dict["blob_store"])
+        except Exception as e:
+            raise RuntimeError("Failed loading blob_store") from e
         from pydiverse.pipedag.materialize.store import PipeDAGStore
 
         return PipeDAGStore(
             table=table_store,
             blob=blob_store,
+            local_table_cache=local_table_cache,
         )
 
     def create_lock_manager(self) -> BaseLockManager:
         return load_object(self.config_dict["lock_manager"])
 
     def create_orchestration_engine(self) -> OrchestrationEngine:
         return load_object(self.config_dict["orchestration"])
```

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/context/run_context.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/context/run_context.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/core/flow.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/core/flow.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/core/result.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/core/result.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/core/stage.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/core/stage.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/core/task.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/core/task.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/engine/base.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/engine/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/engine/prefect.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/engine/prefect.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/engine/sequential.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/engine/sequential.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/errors/__init__.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/cache.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
+import copy
+import uuid
 from dataclasses import dataclass
 from datetime import datetime
 from typing import TYPE_CHECKING, Any
 
-from pydiverse.pipedag.context import RunContext
+from pydiverse.pipedag.context import ConfigContext, RunContext
 from pydiverse.pipedag.errors import CacheError
 from pydiverse.pipedag.materialize.container import RawSql
 from pydiverse.pipedag.materialize.metadata import (
     LazyTableMetadata,
     RawSqlMetadata,
     TaskMetadata,
 )
@@ -93,45 +95,53 @@
     @staticmethod
     def cache_lookup(
         store: BaseTableStore,
         task: MaterializingTask,
         input_hash: str,
         cache_fn_hash: str,
     ):
-        # Check the cache
-        try:
-            # `cache_fn_hash` is not used for cache retrieval if ignore_fresh_input
-            # is set to True. In that case, cache_metadata.cache_fn_hash may be
-            # different form the cache_fn_hash of the current task run.
-            cached_output, cache_metadata = store.retrieve_cached_output(
-                task, input_hash, cache_fn_hash
-            )
-            if not task.lazy:
-                # Task isn't lazy -> copy cache to transaction stage
-                store.copy_cached_output_to_transaction_stage(
-                    cached_output, cache_metadata, task
+        if (
+            not ConfigContext.get().ignore_task_version and task.version is not None
+        ) or task.lazy:
+            # Check the cache
+            try:
+                # `cache_fn_hash` is not used for cache retrieval if ignore_fresh_input
+                # is set to True. In that case, cache_metadata.cache_fn_hash may be
+                # different form the cache_fn_hash of the current task run.
+                cached_output, cache_metadata = store.retrieve_cached_output(
+                    task, input_hash, cache_fn_hash
                 )
-                task.logger.info("Found task in cache. Using cached result.")
-            task_cache_key = CacheManager.task_cache_key(
-                task, cache_metadata.input_hash, cache_metadata.cache_fn_hash
-            )
-            return TaskCacheInfo(
-                task,
-                cache_metadata.input_hash,
-                cache_metadata.cache_fn_hash,
-                task_cache_key,
-                cached_output,
-                cache_metadata,
-                _is_cache_valid=True,
-            )
-        except CacheError as e:
-            task.logger.info(
-                "Failed to retrieve task from cache.",
-                exception=str(e),
-            )
+                if not task.lazy:
+                    # Task isn't lazy -> copy cache to transaction stage
+                    store.copy_cached_output_to_transaction_stage(
+                        cached_output, cache_metadata, task
+                    )
+                    task.logger.info("Found task in cache. Using cached result.")
+                task_cache_key = CacheManager.task_cache_key(
+                    task, cache_metadata.input_hash, cache_metadata.cache_fn_hash
+                )
+                return TaskCacheInfo(
+                    task,
+                    cache_metadata.input_hash,
+                    cache_metadata.cache_fn_hash,
+                    task_cache_key,
+                    cached_output,
+                    cache_metadata,
+                    _is_cache_valid=True,
+                )
+            except CacheError as e:
+                task.logger.info(
+                    "Failed to retrieve task from cache.",
+                    exception=str(e),
+                )
+        else:
+            if not task.lazy:
+                # choose a deliberately random version since caching was disabled
+                task = copy.deepcopy(task)
+                task.version = uuid.uuid4().hex
         new_task_cache_key = CacheManager.task_cache_key(
             task, input_hash, cache_fn_hash
         )
         return TaskCacheInfo(
             task,
             input_hash,
             cache_fn_hash,
```

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/container.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/container.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/core.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,18 @@
     :param fn: The run method of this task
     :key name: The name of this task
     :key input_type: The data type to convert table objects to when passed
         to this task.
     :key version: The version of this task. Unless this task is lazy, you
         always have to bump / change the version number to ensure that
         the new implementation gets used. Else a cached result might be used
-        instead.
+        instead. version=None and lazy=False means the task is never cached
+        but outputs are still materialized.
+        In addition, see also option ignore_task_version in pipedag config
+        documentation.
     :key cache: An explicit function for validating cache validity. If the output
         of this function changes while the source parameters are the same (e.g.
         the source is a filepath and `cache` loads data from this file), then the
         cache will be deemed invalid and is not used.
     :key lazy: Boolean indicating if this task should be lazy. A lazy task is
         a task that always gets executed, and if it produces a lazy table
         (e.g. a SQL query), the backend can compare the generated output
```

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/metadata.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/metadata.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/store.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/store.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
+import copy
 import itertools
 import json
 from typing import Any, Callable
 
 import structlog
 
 from pydiverse.pipedag import Blob, Stage, Table, backend
-from pydiverse.pipedag._typing import Materializable
+from pydiverse.pipedag._typing import Materializable, T
 from pydiverse.pipedag.context import ConfigContext, RunContext
 from pydiverse.pipedag.context.run_context import StageState
 from pydiverse.pipedag.errors import DuplicateNameError, StageError
 from pydiverse.pipedag.materialize.container import RawSql
 from pydiverse.pipedag.materialize.core import MaterializingTask, TaskInfo
 from pydiverse.pipedag.materialize.metadata import TaskMetadata
 from pydiverse.pipedag.materialize.util import json as json_util
 from pydiverse.pipedag.util import Disposable, deep_map
 from pydiverse.pipedag.util.config import PipedagConfig
+from pydiverse.pipedag.util.naming import NameDisambiguator
 
 
 class PipeDAGStore(Disposable):
     """Main storage interface for materializing tasks
 
     Depending on the use case, the store can be configured using different
     backends for storing tables, blobs and managing locks.
@@ -30,17 +32,19 @@
     between the different backends, the stages and the materializing tasks.
     """
 
     def __init__(
         self,
         table: backend.table.BaseTableStore,
         blob: backend.blob.BaseBlobStore,
+        local_table_cache: backend.table_cache.LocalTableCache,
     ):
         self.table_store = table
         self.blob_store = blob
+        self.local_table_cache = local_table_cache
 
         self.logger = structlog.get_logger()
         self.json_encoder = json.JSONEncoder(
             ensure_ascii=False,
             allow_nan=False,
             separators=(",", ":"),
             sort_keys=True,
@@ -52,14 +56,16 @@
         """
         Clean up and close all open resources.
 
         Don't use the store object any more after disposal!
         """
         self.table_store.dispose()
         self.blob_store.dispose()
+        if self.local_table_cache is not None:
+            self.local_table_cache.dispose()
         super().dispose()
 
     # ### Stage ### #
 
     def init_stage(self, stage: Stage):
         """Initializes the stage in all backends
 
@@ -100,22 +106,37 @@
             ctx.validate_stage_lock(stage)
             self.table_store.commit_stage(stage)
             self.blob_store.commit_stage(stage)
 
     # ### Materialization ### #
 
     def dematerialize_item(
-        self, item: Table | Blob | Any, as_type: type, ctx: RunContext = None
+        self,
+        item: Table | Blob | Any,
+        as_type: type[T],
+        ctx: RunContext | None = None,
+        namer: NameDisambiguator | None = None,
     ):
         if ctx is None:
             ctx = RunContext.get()
 
         if isinstance(item, Table):
             ctx.validate_stage_lock(item.stage)
-            return self.table_store.retrieve_table_obj(item, as_type=as_type)
+            if self.local_table_cache.has_cache_table(item, as_type):
+                return self.local_table_cache.retrieve_table_obj(item, as_type, namer)
+            else:
+                obj = self.table_store.retrieve_table_obj(
+                    item, as_type=as_type, namer=namer
+                )
+                table = copy.deepcopy(item)
+                table.obj = obj
+                self.local_table_cache.store_table(
+                    table, task=None, task_info=None, is_input=True
+                )
+                return obj
         elif isinstance(item, Blob):
             ctx.validate_stage_lock(item.stage)
             return self.blob_store.retrieve_blob(item)
         return item
 
     def dematerialize_task_inputs(
         self,
@@ -133,19 +154,22 @@
         :param kwargs: The keyword arguments
         :return: A tuple with the dematerialized args and kwargs
         """
 
         ctx = RunContext.get()
 
         input_tables = []
+        namer = NameDisambiguator(prefix="t")
 
         def dematerialize_mapper(x):
             if isinstance(x, Table):
                 input_tables.append(x)
-            return self.dematerialize_item(x, as_type=task.input_type, ctx=ctx)
+            return self.dematerialize_item(
+                x, as_type=task.input_type, ctx=ctx, namer=namer
+            )
 
         d_args = deep_map(args, dematerialize_mapper)
         d_kwargs = deep_map(kwargs, dematerialize_mapper)
 
         return d_args, d_kwargs, input_tables
 
     def materialize_task(
@@ -261,14 +285,17 @@
                 output_json, self.table_store, stage
             )
 
         def store_table(table: Table):
             if task.lazy:
                 self.table_store.store_table_lazy(table, task, task_info)
             else:
+                self.local_table_cache.store_table(
+                    table, task, task_info, is_input=False
+                )
                 self.table_store.store_table(table, task, task_info)
 
         # Materialize
         self._check_names(task, tables, blobs)
         self._store_task_transaction(
             task,
             tables,
```

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/util/cache.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/util/cache.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/util/json.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/util/json.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/config.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -101,20 +101,21 @@
             instance=instance,
             flow=flow,
             default={
                 "fail_fast": False,
                 "network_interface": "127.0.0.1",
                 "per_user_template": "{id}_{username}",
                 "strict_result_get_locking": True,
+                "ignore_task_version": False,
                 "stage_commit_technique": "SCHEMA_SWAP",
                 "auto_table": [],
                 "auto_blob": [],
                 "attrs": {},
             },
-        )
+        ).copy()
 
         # check enums
         # Alternative: could be a feature of __get_merged_config_dict
         # in case default value is set to Enum
         from pydiverse.pipedag.context.context import StageCommitTechnique
 
         config["stage_commit_technique"] = (
@@ -146,49 +147,58 @@
                 {
                     "username": getpass.getuser(),
                     "id": config["instance_id"],
                 },
             )
 
         # Handle url_attrs_file
-        url_attrs_file = _pop(config, "table_store", "url_attrs_file", default=None)
+        url_attrs_file = _pop(
+            config, "table_store", "args", "url_attrs_file", default=None
+        )
         if url_attrs_file is not None:
             with open(url_attrs_file, encoding="utf-8") as fh:
                 url_attrs = yaml.safe_load(fh)
 
-            url = _get(config, "table_store", "url")
+            url = _get(config, "table_store", "args", "url")
             url = expand_variables(url, url_attrs, skip_missing=True)
-            _set(config, url, "table_store", "url")
+            _set(config, url, "table_store", "args", "url")
 
         # Finally, expand all normal variables
         config = self.__expand_variables(config)
 
         # Construct final ConfigContext
         config_context = ConfigContext(
             config_dict=config,
             pipedag_name=self.name,
             flow_name=flow,
             strict_result_get_locking=config["strict_result_get_locking"],
+            ignore_task_version=config["ignore_task_version"],
             instance_name=instance,
             instance_id=config["instance_id"],
             stage_commit_technique=stage_commit_technique,
             fail_fast=config["fail_fast"],
             network_interface=config["network_interface"],
             attrs=Box(config["attrs"], frozen_box=True),
         )
 
-        # Make sure @cached_property store is set up and loaded
-        # and throw config errors early.
-        with config_context:
-            _ = config_context.store
-            _ = config_context.auto_table
-            _ = config_context.auto_blob
-
-            config_context.create_orchestration_engine().dispose()
-            config_context.create_lock_manager().dispose()
+        try:
+            # Make sure @cached_property store is set up and loaded
+            # and throw config errors early.
+            with config_context:
+                _ = config_context.store
+                _ = config_context.auto_table
+                _ = config_context.auto_blob
+
+                config_context.create_orchestration_engine().dispose()
+                config_context.create_lock_manager().dispose()
+        except Exception as e:
+            raise RuntimeError(
+                "Error while creating backend objects from pipedag config "
+                f"(instance={instance}, flow={flow}): {self.path}"
+            ) from e
 
         return config_context
 
     def __get_merged_config_dict(self, instance, flow, default=None):
         search_paths = [
             ("instances", "__any__"),
             ("instances", instance),
@@ -225,32 +235,32 @@
                 merged = deep_merge(merged, d)
 
         return merged
 
     @staticmethod
     def __expand_environment_variables(*, inout_config):
         locations = [
-            ("table_store", "url"),
-            ("table_store", "url_attrs_file"),
+            ("table_store", "args", "url"),
+            ("table_store", "args", "url_attrs_file"),
         ]
 
         for location in locations:
             value: str = _get(inout_config, location, default=None)
             if value is None:
                 continue
 
             value = expand_environment_variables(value)
             _set(inout_config, value, location)
 
     def __expand_variables(self, config) -> dict[str, Any]:
         out_config = copy.deepcopy(config)
         locations = [
-            ("table_store", "url"),
-            ("table_store", "schema_prefix"),
-            ("table_store", "schema_suffix"),
+            ("table_store", "args", "url"),
+            ("table_store", "args", "schema_prefix"),
+            ("table_store", "args", "schema_suffix"),
         ]
 
         # TODO: Decide on a list of available variables
         variables = {
             "username": getpass.getuser(),
             "instance_id": config.get("instance_id"),
             "name": self.name,
@@ -363,34 +373,47 @@
     return re.sub(r"\{[a-zA-Z_]+[a-zA-Z0-9_]*\}", var_sub, string)
 
 
 def load_object(config_dict: dict):
     """Instantiates an instance of an object given
 
     The import path (module.Class) should be specified as the "class" value
-    of the dict. The rest of the dict get used as the instance config.
+    of the dict. The args section of the dict get used as the instance config.
 
     If the class defines a `_init_conf_` function, it gets called using the
     config values, otherwise they just get passed to the class initializer.
 
     >>> # module.Class(argument="value")
     >>> load_object({
     >>>     "class": "module.Class",
-    >>>     "argument": "value",
+    >>>     "args": {
+    >>>         "argument": "value",
+    >>>     },
     >>> })
     """
 
-    config_dict = config_dict.copy()
-    cls = import_object(config_dict.pop("class"))
+    if "class" not in config_dict:
+        raise RuntimeError(
+            "Attribute 'class' is missing in configuration "
+            "section that supports multiple backends\n"
+            f"config section: {config_dict}"
+        )
+    cls = import_object(config_dict["class"])
 
+    args = config_dict.get("args", {})
+    if not isinstance(args, dict):
+        raise TypeError(
+            f"Invalid type for args section: {type(args)}\n"
+            f"config section: {config_dict}"
+        )
     try:
         init_conf = cls._init_conf_
-        return init_conf(config_dict)
+        return init_conf(args)
     except AttributeError:
-        return cls(**config_dict)
+        return cls(**args)
 
 
 # Nested Dictionary Utilities
 
 
 def _flatten(items):
     for x in items:
```

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/deep_map.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/deep_map.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/deep_merge.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/deep_merge.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/disposable.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/disposable.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/import_.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/import_.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/ipc.py` & `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/ipc.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.4/setup.py` & `pydiverse-pipedag-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,41 +25,39 @@
 ['PyYAML>=6.0',
  'SQLAlchemy>=1.4.39',
  'attrs>=22.1.0',
  'msgpack>=1.0.4',
  'networkx>=2.8',
  'packaging>=21.3',
  'pandas>=1.4.3',
+ 'pyarrow>=11.0.0',
  'pynng>=0.7.1',
  'python-box>=6.1.0',
  'structlog>=22.1.0',
  'tomli>=2.0.1',
  'typing-extensions>=4.1.0,<5']
 
 extras_require = \
 {'docs': ['Sphinx>=5.1.1',
           'sphinx-rtd-theme>=1.0.0',
           'sphinxcontrib-apidoc>=0.3.0'],
  'filelock': ['filelock>=3.7.1'],
- 'ibis': ['ibis>=3.2.0', 'ibis-framework[mssql,postgres]>=5.1.0,<6.0.0'],
+ 'ibis': ['ibis>=3.2.0', 'ibis-framework[postgres,mssql]>=5.1.0,<6.0.0'],
  'ibm_db2': ['ibm-db>=3.1.4', 'ibm-db-sa>=0.3.8'],
  'mssql': ['pyodbc>=4.0.35', 'pytsql>=1.1.4'],
  'pdtransform': ['pydiverse-transform>=0.1.1'],
- 'polars': ['tidypolars>=0.2.19',
-            'connectorx>=0.3.1',
-            'pyarrow>=11.0.0',
-            'polars>=0.16.18,<0.17'],
+ 'polars': ['tidypolars>=0.2.19', 'connectorx>=0.3.1', 'polars>=0.16.18,<0.17'],
  'prefect': ['prefect>=1.3,<2'],
  'zookeeper': ['kazoo>=2.8.0']}
 
 setup_kwargs = {
     'name': 'pydiverse-pipedag',
-    'version': '0.2.4',
+    'version': '0.3.0',
     'description': 'A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files.',
-    'long_description': '# pydiverse.pipedag\n\n[![CI](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/ci.yml/badge.svg)](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/ci.yml)\n\nA pipeline orchestration library executing tasks within one python session. It takes care of SQL table\n(de)materialization, caching and cache invalidation. Blob storage is supported as well for example\nfor storing model files.\n\nThis is an early stage version 0.x which lacks documentation. Please contact\nhttps://github.com/orgs/pydiverse/teams/code-owners if you like to become an early adopter\nor to contribute early stage usage examples.\n\n## Usage\n\npydiverse.pipedag can either be installed via pypi with `pip install pydiverse-pipedag` or via conda-forge\nwith `conda install pydiverse-pipedag -c conda-forge`.\n\n## Example\n\nA flow can look like this (i.e. put this in a file named `run_pipeline.py`):\n\n```python\nfrom pydiverse.pipedag import materialize, Table, Flow, Stage\nimport sqlalchemy as sa\nimport pandas as pd\n\nfrom pydiverse.pipedag.context import StageLockContext, RunContext\nfrom pydiverse.pipedag.util import setup_structlog\n\n\n@materialize(lazy=True)\ndef lazy_task_1():\n    return sa.select([sa.literal(1).label("x"), sa.literal(2).label("y")])\n\n\n@materialize(lazy=True, input_type=sa.Table)\ndef lazy_task_2(input1: sa.Table, input2: sa.Table):\n    query = sa.select([(input1.c.x * 5).label("x5"), input2.c.a]).select_from(\n        input1.outerjoin(input2, input2.c.x == input1.c.x)\n    )\n    return Table(query, name="task_2_out", primary_key=["a"])\n\n\n@materialize(lazy=True, input_type=sa.Table)\ndef lazy_task_3(input: sa.Table, my_stage: Stage):\n    return sa.text(f"SELECT * FROM {my_stage.transaction_name}.{input.name}")\n\n\n@materialize(lazy=True, input_type=sa.Table)\ndef lazy_task_4(input: sa.Table, prev_stage: Stage):\n    return sa.text(f"SELECT * FROM {prev_stage.name}.{input.name}")\n\n\n@materialize(nout=2, version="1.0.0")\ndef eager_inputs():\n    dfA = pd.DataFrame(\n        {\n            "a": [0, 1, 2, 4],\n            "b": [9, 8, 7, 6],\n        }\n    )\n    dfB = pd.DataFrame(\n        {\n            "a": [2, 1, 0, 1],\n            "x": [1, 1, 2, 2],\n        }\n    )\n    return Table(dfA, "dfA"), Table(dfB, "dfB_%%")\n\n\n@materialize(version="1.0.0", input_type=pd.DataFrame)\ndef eager_task(tbl1: pd.DataFrame, tbl2: pd.DataFrame):\n    return tbl1.merge(tbl2, on="x")\n\n\ndef main():\n    with Flow() as f:\n        with Stage("stage_1"):\n            lazy_1 = lazy_task_1()\n            a, b = eager_inputs()\n\n        with Stage("stage_2") as stage2:\n            lazy_2 = lazy_task_2(lazy_1, b)\n            lazy_3 = lazy_task_3(lazy_2, stage2)\n            eager = eager_task(lazy_1, b)\n\n        with Stage("stage_3"):\n            lazy_4 = lazy_task_4(lazy_2, stage2)\n        _ = lazy_3, lazy_4, eager  # unused terminal output tables\n\n    # Run flow\n    result = f.run()\n    assert result.successful\n\n    # Run in a different way for testing\n    with StageLockContext():\n        result = f.run()\n        assert result.successful\n        assert result.get(lazy_1, as_type=pd.DataFrame)["x"][0] == 1\n\n\nif __name__ == "__main__":\n    # initialize logging\n    setup_structlog()\n    main()\n```\n\nCreate a file called `pipedag.yaml` in the same directory:\n\n```yaml\nname: pipedag_tests\ntable_store_connections:\n  postgres:\n    # Postgres: this can be used after running `docker-compose up`\n    url: "postgresql://{$POSTGRES_USERNAME}:{$POSTGRES_PASSWORD}@127.0.0.1:6543/{instance_id}"\n\ninstances:\n  __any__:\n    # listen-interface for pipedag context server which synchronizes some task state during DAG execution\n    network_interface: "127.0.0.1"\n    # classes to be materialized to table store even without pipedag Table wrapper (we have loose coupling between\n    # pipedag and pydiverse.transform, so consider adding \'pydiverse.transform.Table\' in your config)\n    auto_table: ["pandas.DataFrame", "sqlalchemy.sql.elements.TextClause", "sqlalchemy.sql.selectable.Selectable"]\n    fail_fast: true\n\n    instance_id: pipedag_default\n    table_store:\n      class: "pydiverse.pipedag.backend.table.SQLTableStore"\n\n      # Postgres: this can be used after running `docker-compose up`\n      table_store_connection: postgres\n      create_database_if_not_exists: True\n\n      # print select statements before being encapsualted in materialize expressions and tables before writing to\n      # database\n      print_materialize: true\n      # print final sql statements\n      print_sql: true\n\n    blob_store:\n      class: "pydiverse.pipedag.backend.blob.FileBlobStore"\n      base_path: "/tmp/pipedag/blobs"\n\n    lock_manager:\n      class: "pydiverse.pipedag.backend.lock.ZooKeeperLockManager"\n      hosts: "localhost:2181"\n\n    orchestration:\n      class: "pydiverse.pipedag.engine.SequentialEngine"\n```\n\nIf you don\'t have a postgres, Microsoft SQL Server, or IBM DB2 database at hand, you can\nstart a postgres database with the following `docker-compose.yaml` file:\n\n```yaml\nversion: "3.9"\nservices:\n  postgres:\n    image: postgres\n    environment:\n      POSTGRES_USER: sa\n      POSTGRES_PASSWORD: Pydiverse23\n      POSTGRES_PORT: 6543\n    ports:\n      - 6543:5432\n  zoo:\n    image: zookeeper\n    environment:\n      ZOO_4LW_COMMANDS_WHITELIST: ruok\n      ZOO_MAX_CLIENT_CNXNS: 100\n    ports:\n      - 2181:2181\n```\n\nRun `docker-compose up` in the directory of your `docker-compose.yaml` and then execute\nthe flow script as follows with a shell like `bash` and a python environment that\nincludes `pydiverse-pipedag`, `pandas`, and `sqlalchemy`:\n\n```bash\nexport POSTGRES_USERNAME=sa\nexport POSTGRES_PASSWORD=Pydiverse23\npython run_pipeline.py\n```\n\nFinally, you may connect to your localhost postgres database `pipedag_default` and\nlook at tables in schemas `stage_1`..`stage_3`.\n\nIf you don\'t have a SQL UI at hand, you may use `psql` command line tool inside the docker container.\nCheck out the `NAMES` column in `docker ps` output. If the name of your postgres container is\n`example_postgres_1`, then you can look at output tables like this:\n\n```bash\ndocker exec example_postgres_1 psql --username=sa --dbname=pipedag_default -c \'select * from stage_1.dfa;\'\n```\n\nOr more interactively:\n\n```bash\ndocker exec -t -i example_postgres_1 bash\npsql --username=sa --dbname=pipedag_default\n\\dt stage_*.*\nselect * from stage_2.task_2_out;\n```\n\n## Troubleshooting\n\n### Installing mssql odbc driver for linux\n\nInstalling with\ninstructions [here](https://docs.microsoft.com/en-us/sql/connect/odbc/linux-mac/installing-the-microsoft-odbc-driver-for-sql-server?view=sql-server-ver16#suse18)\nworked.\nBut `odbcinst -j` revealed that it installed the configuration in `/etc/unixODBC/*`. But conda installed pyodbc brings\nits own `odbcinst` executable and that shows odbc config files are expected in `/etc/*`. Symlinks were enough to fix the\nproblem. Try `python -c \'import pyodbc;print(pyodbc.drivers())\'` and see whether you get more than an empty list.\nFurthermore, make sure you use 127.0.0.1 instead of localhost. It seems that /etc/hosts is ignored.\n',
+    'long_description': '# pydiverse.pipedag\n\n[![CI](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/ci.yml/badge.svg)](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/ci.yml)\n\nA pipeline orchestration library executing tasks within one python session. It takes care of SQL table\n(de)materialization, caching and cache invalidation. Blob storage is supported as well for example\nfor storing model files.\n\nThis is an early stage version 0.x which lacks documentation. Please contact\nhttps://github.com/orgs/pydiverse/teams/code-owners if you like to become an early adopter\nor to contribute early stage usage examples.\n\n## Usage\n\npydiverse.pipedag can either be installed via pypi with `pip install pydiverse-pipedag` or via conda-forge\nwith `conda install pydiverse-pipedag -c conda-forge`.\n\n## Example\n\nA flow can look like this (i.e. put this in a file named `run_pipeline.py`):\n\n```python\nfrom pydiverse.pipedag import materialize, Table, Flow, Stage\nimport sqlalchemy as sa\nimport pandas as pd\n\nfrom pydiverse.pipedag.context import StageLockContext, RunContext\nfrom pydiverse.pipedag.util import setup_structlog\n\n\n@materialize(lazy=True)\ndef lazy_task_1():\n    return sa.select([sa.literal(1).label("x"), sa.literal(2).label("y")])\n\n\n@materialize(lazy=True, input_type=sa.Table)\ndef lazy_task_2(input1: sa.Table, input2: sa.Table):\n    query = sa.select([(input1.c.x * 5).label("x5"), input2.c.a]).select_from(\n        input1.outerjoin(input2, input2.c.x == input1.c.x)\n    )\n    return Table(query, name="task_2_out", primary_key=["a"])\n\n\n@materialize(lazy=True, input_type=sa.Table)\ndef lazy_task_3(input: sa.Table, my_stage: Stage):\n    return sa.text(f"SELECT * FROM {my_stage.transaction_name}.{input.name}")\n\n\n@materialize(lazy=True, input_type=sa.Table)\ndef lazy_task_4(input: sa.Table, prev_stage: Stage):\n    return sa.text(f"SELECT * FROM {prev_stage.name}.{input.name}")\n\n\n@materialize(nout=2, version="1.0.0")\ndef eager_inputs():\n    dfA = pd.DataFrame(\n        {\n            "a": [0, 1, 2, 4],\n            "b": [9, 8, 7, 6],\n        }\n    )\n    dfB = pd.DataFrame(\n        {\n            "a": [2, 1, 0, 1],\n            "x": [1, 1, 2, 2],\n        }\n    )\n    return Table(dfA, "dfA"), Table(dfB, "dfB_%%")\n\n\n@materialize(version="1.0.0", input_type=pd.DataFrame)\ndef eager_task(tbl1: pd.DataFrame, tbl2: pd.DataFrame):\n    return tbl1.merge(tbl2, on="x")\n\n\ndef main():\n    with Flow() as f:\n        with Stage("stage_1"):\n            lazy_1 = lazy_task_1()\n            a, b = eager_inputs()\n\n        with Stage("stage_2") as stage2:\n            lazy_2 = lazy_task_2(lazy_1, b)\n            lazy_3 = lazy_task_3(lazy_2, stage2)\n            eager = eager_task(lazy_1, b)\n\n        with Stage("stage_3"):\n            lazy_4 = lazy_task_4(lazy_2, stage2)\n        _ = lazy_3, lazy_4, eager  # unused terminal output tables\n\n    # Run flow\n    result = f.run()\n    assert result.successful\n\n    # Run in a different way for testing\n    with StageLockContext():\n        result = f.run()\n        assert result.successful\n        assert result.get(lazy_1, as_type=pd.DataFrame)["x"][0] == 1\n\n\nif __name__ == "__main__":\n    # initialize logging\n    setup_structlog()\n    main()\n```\n\nCreate a file called `pipedag.yaml` in the same directory:\n\n```yaml\nname: pipedag_tests\ntable_store_connections:\n  postgres:\n    args:\n      # Postgres: this can be used after running `docker-compose up`  \n      url: "postgresql://{$POSTGRES_USERNAME}:{$POSTGRES_PASSWORD}@127.0.0.1:6543/{instance_id}"\n\ninstances:\n  __any__:\n    # listen-interface for pipedag context server which synchronizes some task state during DAG execution\n    network_interface: "127.0.0.1"\n    # classes to be materialized to table store even without pipedag Table wrapper (we have loose coupling between\n    # pipedag and pydiverse.transform, so consider adding \'pydiverse.transform.Table\' in your config)\n    auto_table: ["pandas.DataFrame", "sqlalchemy.sql.elements.TextClause", "sqlalchemy.sql.selectable.Selectable"]\n    fail_fast: true\n\n    instance_id: pipedag_default\n    table_store:\n      class: "pydiverse.pipedag.backend.table.SQLTableStore"\n\n      # Postgres: this can be used after running `docker-compose up`\n      table_store_connection: postgres\n      args:\n        create_database_if_not_exists: True\n        \n        # print select statements before being encapsualted in materialize expressions and tables before writing to\n        # database\n        print_materialize: true\n        # print final sql statements\n        print_sql: true\n\n      local_table_cache:\n        store_input: true\n        store_output: true\n        use_stored_input_as_cache: true\n        class: "pydiverse.pipedag.backend.table_cache.ParquetTableCache"\n        args:\n          base_path: "/tmp/pipedag/table_cache"\n\n    blob_store:\n      class: "pydiverse.pipedag.backend.blob.FileBlobStore"\n      args:\n        base_path: "/tmp/pipedag/blobs"\n\n    lock_manager:\n      class: "pydiverse.pipedag.backend.lock.ZooKeeperLockManager"\n      args:\n        hosts: "localhost:2181"\n\n    orchestration:\n      class: "pydiverse.pipedag.engine.SequentialEngine"\n```\n\nIf you don\'t have a postgres, Microsoft SQL Server, or IBM DB2 database at hand, you can\nstart a postgres database with the following `docker-compose.yaml` file:\n\n```yaml\nversion: "3.9"\nservices:\n  postgres:\n    image: postgres\n    environment:\n      POSTGRES_USER: sa\n      POSTGRES_PASSWORD: Pydiverse23\n      POSTGRES_PORT: 6543\n    ports:\n      - 6543:5432\n  zoo:\n    image: zookeeper\n    environment:\n      ZOO_4LW_COMMANDS_WHITELIST: ruok\n      ZOO_MAX_CLIENT_CNXNS: 100\n    ports:\n      - 2181:2181\n```\n\nRun `docker-compose up` in the directory of your `docker-compose.yaml` and then execute\nthe flow script as follows with a shell like `bash` and a python environment that\nincludes `pydiverse-pipedag`, `pandas`, and `sqlalchemy`:\n\n```bash\nexport POSTGRES_USERNAME=sa\nexport POSTGRES_PASSWORD=Pydiverse23\npython run_pipeline.py\n```\n\nFinally, you may connect to your localhost postgres database `pipedag_default` and\nlook at tables in schemas `stage_1`..`stage_3`.\n\nIf you don\'t have a SQL UI at hand, you may use `psql` command line tool inside the docker container.\nCheck out the `NAMES` column in `docker ps` output. If the name of your postgres container is\n`example_postgres_1`, then you can look at output tables like this:\n\n```bash\ndocker exec example_postgres_1 psql --username=sa --dbname=pipedag_default -c \'select * from stage_1.dfa;\'\n```\n\nOr more interactively:\n\n```bash\ndocker exec -t -i example_postgres_1 bash\npsql --username=sa --dbname=pipedag_default\n\\dt stage_*.*\nselect * from stage_2.task_2_out;\n```\n\n## Troubleshooting\n\n### Installing mssql odbc driver for linux\n\nInstalling with\ninstructions [here](https://docs.microsoft.com/en-us/sql/connect/odbc/linux-mac/installing-the-microsoft-odbc-driver-for-sql-server?view=sql-server-ver16#suse18)\nworked.\nBut `odbcinst -j` revealed that it installed the configuration in `/etc/unixODBC/*`. But conda installed pyodbc brings\nits own `odbcinst` executable and that shows odbc config files are expected in `/etc/*`. Symlinks were enough to fix the\nproblem. Try `python -c \'import pyodbc;print(pyodbc.drivers())\'` and see whether you get more than an empty list.\nFurthermore, make sure you use 127.0.0.1 instead of localhost. It seems that /etc/hosts is ignored.\n',
     'author': 'QuantCo, Inc.',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `pydiverse-pipedag-0.2.4/PKG-INFO` & `pydiverse-pipedag-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydiverse-pipedag
-Version: 0.2.4
+Version: 0.3.0
 Summary: A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files.
 License: BSD-3-Clause
 Author: QuantCo, Inc.
 Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -26,25 +26,25 @@
 Requires-Dist: PyYAML (>=6.0)
 Requires-Dist: SQLAlchemy (>=1.4.39)
 Requires-Dist: Sphinx (>=5.1.1); extra == "docs"
 Requires-Dist: attrs (>=22.1.0)
 Requires-Dist: connectorx (>=0.3.1); extra == "polars"
 Requires-Dist: filelock (>=3.7.1); extra == "filelock"
 Requires-Dist: ibis (>=3.2.0); extra == "ibis"
-Requires-Dist: ibis-framework[mssql,postgres] (>=5.1.0,<6.0.0); extra == "ibis"
+Requires-Dist: ibis-framework[postgres,mssql] (>=5.1.0,<6.0.0); extra == "ibis"
 Requires-Dist: ibm-db (>=3.1.4); extra == "ibm_db2"
 Requires-Dist: ibm-db-sa (>=0.3.8); extra == "ibm_db2"
 Requires-Dist: kazoo (>=2.8.0); extra == "zookeeper"
 Requires-Dist: msgpack (>=1.0.4)
 Requires-Dist: networkx (>=2.8)
 Requires-Dist: packaging (>=21.3)
 Requires-Dist: pandas (>=1.4.3)
 Requires-Dist: polars (>=0.16.18,<0.17); extra == "polars"
 Requires-Dist: prefect (>=1.3,<2); extra == "prefect"
-Requires-Dist: pyarrow (>=11.0.0); extra == "polars"
+Requires-Dist: pyarrow (>=11.0.0)
 Requires-Dist: pydiverse-transform (>=0.1.1); extra == "pdtransform"
 Requires-Dist: pynng (>=0.7.1)
 Requires-Dist: pyodbc (>=4.0.35); extra == "mssql"
 Requires-Dist: python-box (>=6.1.0)
 Requires-Dist: pytsql (>=1.1.4); extra == "mssql"
 Requires-Dist: sphinx-rtd-theme (>=1.0.0); extra == "docs"
 Requires-Dist: sphinxcontrib-apidoc (>=0.3.0); extra == "docs"
@@ -163,16 +163,17 @@
 
 Create a file called `pipedag.yaml` in the same directory:
 
 ```yaml
 name: pipedag_tests
 table_store_connections:
   postgres:
-    # Postgres: this can be used after running `docker-compose up`
-    url: "postgresql://{$POSTGRES_USERNAME}:{$POSTGRES_PASSWORD}@127.0.0.1:6543/{instance_id}"
+    args:
+      # Postgres: this can be used after running `docker-compose up`  
+      url: "postgresql://{$POSTGRES_USERNAME}:{$POSTGRES_PASSWORD}@127.0.0.1:6543/{instance_id}"
 
 instances:
   __any__:
     # listen-interface for pipedag context server which synchronizes some task state during DAG execution
     network_interface: "127.0.0.1"
     # classes to be materialized to table store even without pipedag Table wrapper (we have loose coupling between
     # pipedag and pydiverse.transform, so consider adding 'pydiverse.transform.Table' in your config)
@@ -181,29 +182,40 @@
 
     instance_id: pipedag_default
     table_store:
       class: "pydiverse.pipedag.backend.table.SQLTableStore"
 
       # Postgres: this can be used after running `docker-compose up`
       table_store_connection: postgres
-      create_database_if_not_exists: True
-
-      # print select statements before being encapsualted in materialize expressions and tables before writing to
-      # database
-      print_materialize: true
-      # print final sql statements
-      print_sql: true
+      args:
+        create_database_if_not_exists: True
+        
+        # print select statements before being encapsualted in materialize expressions and tables before writing to
+        # database
+        print_materialize: true
+        # print final sql statements
+        print_sql: true
+
+      local_table_cache:
+        store_input: true
+        store_output: true
+        use_stored_input_as_cache: true
+        class: "pydiverse.pipedag.backend.table_cache.ParquetTableCache"
+        args:
+          base_path: "/tmp/pipedag/table_cache"
 
     blob_store:
       class: "pydiverse.pipedag.backend.blob.FileBlobStore"
-      base_path: "/tmp/pipedag/blobs"
+      args:
+        base_path: "/tmp/pipedag/blobs"
 
     lock_manager:
       class: "pydiverse.pipedag.backend.lock.ZooKeeperLockManager"
-      hosts: "localhost:2181"
+      args:
+        hosts: "localhost:2181"
 
     orchestration:
       class: "pydiverse.pipedag.engine.SequentialEngine"
 ```
 
 If you don't have a postgres, Microsoft SQL Server, or IBM DB2 database at hand, you can
 start a postgres database with the following `docker-compose.yaml` file:
```

