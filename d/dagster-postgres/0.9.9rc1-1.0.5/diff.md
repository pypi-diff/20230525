# Comparing `tmp/dagster-postgres-0.9.9rc1.tar.gz` & `tmp/dagster-postgres-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-postgres-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:07 2020, max compression
+gzip compressed data, was "dagster-postgres-1.0.5.tar", last modified: Fri Aug 26 13:46:55 2022, max compression
```

## Comparing `dagster-postgres-0.9.9rc1.tar` & `dagster-postgres-1.0.5.tar`

### file list

```diff
@@ -1,79 +1,33 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)      148 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      579 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      134 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/
--rw-r--r--   0 bobchen    (501) staff       (20)      391 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/
--rw-r--r--   0 bobchen    (501) staff       (20)       47 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/
--rw-r--r--   0 bobchen    (501) staff       (20)      195 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/README
--rw-r--r--   0 bobchen    (501) staff       (20)     1034 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/alembic.ini
--rw-r--r--   0 bobchen    (501) staff       (20)     1984 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/env.py
--rw-r--r--   0 bobchen    (501) staff       (20)      494 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/script.py.mako
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/
--rw-r--r--   0 bobchen    (501) staff       (20)     1088 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/07f83cc13695_create_run_id_idx.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1108 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/1ebdd7a9686f_add_step_key_pipeline_name.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2759 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/567bc23fd1ac_.py
--rw-r--r--   0 bobchen    (501) staff       (20)      871 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/5c18fd3c2957_scheduler_update.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1541 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/727ffe943a9f_add_asset_key.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1486 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/8f8dba68fd3b_cascade_run_deletion.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1335 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/c63a27054f08_add_snapshots_to_run_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     8688 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/event_log.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4953 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/pynotify.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/
--rw-r--r--   0 bobchen    (501) staff       (20)       44 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/
--rw-r--r--   0 bobchen    (501) staff       (20)      195 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/README
--rw-r--r--   0 bobchen    (501) staff       (20)     1034 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/alembic.ini
--rw-r--r--   0 bobchen    (501) staff       (20)     1969 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/env.py
--rw-r--r--   0 bobchen    (501) staff       (20)      494 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/script.py.mako
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/
--rw-r--r--   0 bobchen    (501) staff       (20)     1088 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/07f83cc13695_create_run_id_idx.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1108 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/1ebdd7a9686f_add_step_key_pipeline_name.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2759 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/567bc23fd1ac_.py
--rw-r--r--   0 bobchen    (501) staff       (20)      871 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/5c18fd3c2957_scheduler_update.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1541 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/727ffe943a9f_add_asset_key.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1486 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/8f8dba68fd3b_cascade_run_deletion.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1335 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/c63a27054f08_add_snapshots_to_run_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2898 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/run_storage.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/
--rw-r--r--   0 bobchen    (501) staff       (20)       54 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/
--rw-r--r--   0 bobchen    (501) staff       (20)      195 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/README
--rw-r--r--   0 bobchen    (501) staff       (20)     1034 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/alembic.ini
--rw-r--r--   0 bobchen    (501) staff       (20)     1969 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/env.py
--rw-r--r--   0 bobchen    (501) staff       (20)      494 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/script.py.mako
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/
--rw-r--r--   0 bobchen    (501) staff       (20)     1088 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/07f83cc13695_create_run_id_idx.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1108 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/1ebdd7a9686f_add_step_key_pipeline_name.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2759 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/567bc23fd1ac_.py
--rw-r--r--   0 bobchen    (501) staff       (20)      871 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/5c18fd3c2957_scheduler_update.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1541 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/727ffe943a9f_add_asset_key.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1486 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/8f8dba68fd3b_cascade_run_deletion.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1335 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/c63a27054f08_add_snapshots_to_run_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2891 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/schedule_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1576 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      579 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)     3392 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       24 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       40 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/compat_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/compat_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     8220 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/compat_tests/test_back_compat.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1234 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/compat_tests/test_migration_scripts.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2118 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)    17189 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/test_event_log.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2102 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/test_instance.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4840 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/test_run_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)      384 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/test_schedule_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)       94 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1335 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:55.640939 dagster-postgres-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-postgres-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      132 2022-08-26 13:33:01.000000 dagster-postgres-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      638 2022-08-26 13:46:55.640939 dagster-postgres-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      134 2022-08-26 13:33:01.000000 dagster-postgres-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:55.628939 dagster-postgres-1.0.5/dagster_postgres/
+-rw-r--r--   0 root         (0) root         (0)      481 2022-08-26 13:33:01.000000 dagster-postgres-1.0.5/dagster_postgres/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:55.628939 dagster-postgres-1.0.5/dagster_postgres/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1039 2022-08-26 13:33:01.000000 dagster-postgres-1.0.5/dagster_postgres/alembic/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:55.632938 dagster-postgres-1.0.5/dagster_postgres/event_log/
+-rw-r--r--   0 root         (0) root         (0)       95 2022-08-26 13:33:01.000000 dagster-postgres-1.0.5/dagster_postgres/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10884 2022-08-26 13:33:01.000000 dagster-postgres-1.0.5/dagster_postgres/event_log/event_log.py
+-rw-r--r--   0 root         (0) root         (0)     5254 2022-08-26 13:33:01.000000 dagster-postgres-1.0.5/dagster_postgres/event_log/event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-postgres-1.0.5/dagster_postgres/py.typed
+-rw-r--r--   0 root         (0) root         (0)     4738 2022-08-26 13:33:01.000000 dagster-postgres-1.0.5/dagster_postgres/pynotify.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:55.636939 dagster-postgres-1.0.5/dagster_postgres/run_storage/
+-rw-r--r--   0 root         (0) root         (0)       44 2022-08-26 13:33:01.000000 dagster-postgres-1.0.5/dagster_postgres/run_storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7058 2022-08-26 13:33:01.000000 dagster-postgres-1.0.5/dagster_postgres/run_storage/run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:55.636939 dagster-postgres-1.0.5/dagster_postgres/schedule_storage/
+-rw-r--r--   0 root         (0) root         (0)       54 2022-08-26 13:33:01.000000 dagster-postgres-1.0.5/dagster_postgres/schedule_storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5682 2022-08-26 13:33:01.000000 dagster-postgres-1.0.5/dagster_postgres/schedule_storage/schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3868 2022-08-26 13:33:01.000000 dagster-postgres-1.0.5/dagster_postgres/storage.py
+-rw-r--r--   0 root         (0) root         (0)     4982 2022-08-26 13:33:01.000000 dagster-postgres-1.0.5/dagster_postgres/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-postgres-1.0.5/dagster_postgres/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:55.628939 dagster-postgres-1.0.5/dagster_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      638 2022-08-26 13:46:55.000000 dagster-postgres-1.0.5/dagster_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      797 2022-08-26 13:46:55.000000 dagster-postgres-1.0.5/dagster_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:55.000000 dagster-postgres-1.0.5/dagster_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:55.000000 dagster-postgres-1.0.5/dagster_postgres.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       31 2022-08-26 13:46:55.000000 dagster-postgres-1.0.5/dagster_postgres.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2022-08-26 13:46:55.000000 dagster-postgres-1.0.5/dagster_postgres.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      151 2022-08-26 13:46:55.640939 dagster-postgres-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1471 2022-08-26 13:33:01.000000 dagster-postgres-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-postgres-0.9.9rc1/LICENSE` & `dagster-postgres-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9rc1/PKG-INFO` & `dagster-postgres-1.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-postgres
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: A Dagster integration for postgres
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-postgres
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/alembic.ini` & `dagster-postgres-1.0.5/dagster_postgres/alembic/alembic.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [alembic]
 # path to migration scripts
-script_location = .
+script_location = dagster:core/storage/alembic
 
 
 [post_write_hooks]
 # post_write_hooks defines scripts or Python functions that are run
 # on newly generated revision scripts.  See the documentation for further
 # detail and examples
 
 # format using "black" - use the console_scripts runner, against the "black" entrypoint
 hooks = black
 black.type = console_scripts
 black.entrypoint = black
-black.options = --line-length 100 --target-version py27 --target-version py36 --target-version py37 --target-version py38 -S --fast
+black.options = --line-length 100 --target-version py36 --target-version py37 --target-version py38 -S --fast
 
 # Logging configuration
 [loggers]
 keys = root,sqlalchemy,alembic
 
 [handlers]
 keys = console
```

### Comparing `dagster-postgres-0.9.9rc1/dagster_postgres/pynotify.py` & `dagster-postgres-1.0.5/dagster_postgres/pynotify.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,23 +21,25 @@
 # IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 # OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 # ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 # OTHER DEALINGS IN THE SOFTWARE.
 
 # For more information, please refer to <http://unlicense.org>
 
-from __future__ import absolute_import, division, print_function, unicode_literals
-
 import errno
 import os
 import select
 import signal
 import sys
+from threading import Event
+from typing import Iterator, List, Optional
+
+from psycopg2.extensions import Notify
 
-from dagster import check
+import dagster._check as check
 
 from .utils import get_conn
 
 
 def get_wakeup_fd():
     pipe_r, pipe_w = os.pipe()
     if "win" not in sys.platform:
@@ -68,81 +70,68 @@
 
 def construct_signals(arg):
     # function exists to consolidate and scope pylint directive
     return signal.Signals(arg)  # pylint: disable=no-member
 
 
 def await_pg_notifications(
-    conn_string,
-    channels=None,
-    timeout=5.0,
-    yield_on_timeout=False,
-    handle_signals=None,
-    exit_event=None,
-):
+    conn_string: str,
+    channels: Optional[List[str]] = None,
+    timeout: float = 5.0,
+    yield_on_timeout: bool = False,
+    exit_event: Optional[Event] = None,
+    started_event: Optional[Event] = None,
+) -> Iterator[Optional[Notify]]:
     """Subscribe to PostgreSQL notifications, and handle them
     in infinite-loop style.
-    On an actual message, returns the notification (with .pid,
-    .channel, and .payload attributes).
-    If you've enabled 'yield_on_timeout', yields None on timeout.
-    If you've enabled 'handle_keyboardinterrupt', yields False on
-    interrupt.
+
+    Args:
+        conn_string (str): connection string to PG DB
+        channels (Optional[List[str]], optional): List of channel names to listen to. Defaults to None.
+        timeout (float, optional): Timeout interval. Defaults to 5.0.
+        yield_on_timeout (bool, optional): Should the function yield on timeout. Defaults to False.
+        exit_event (Optional[Event], optional): Event that indicates that polling for new notifications should stop. Defaults to None.
+        started_event (Optional[Event], optional): Event that this function can set to notify that the subscription has been established. Defaults to None.
+
+    Yields:
+        Iterator[Optional[Notify]]: Can yield one of two types:
+            1: None, in case of timeout
+            2: Notify, in case of successful notification reception
     """
 
     check.str_param(conn_string, "conn_string")
     channels = None if channels is None else check.list_param(channels, "channels", of_type=str)
     check.float_param(timeout, "timeout")
     check.bool_param(yield_on_timeout, "yield_on_timeout")
 
     conn = get_conn(conn_string)
 
     if channels:
         start_listening(conn, channels)
 
-    signals_to_handle = handle_signals or []
-    original_handlers = {}
+    if started_event:
+        started_event.set()
 
     try:
-        if signals_to_handle:
-            original_handlers = {s: signal.signal(s, _empty_handler) for s in signals_to_handle}
-            wakeup = get_wakeup_fd()
-            listen_on = [conn, wakeup]
-        else:
-            listen_on = [conn]
-            wakeup = None
 
         while True and not (exit_event and exit_event.is_set()):
             try:
-                r, w, x = select.select(listen_on, [], [], max(0, timeout))
+                r, w, x = select.select([conn], [], [], max(0, timeout))
                 if (r, w, x) == ([], [], []):
                     if yield_on_timeout:
                         yield None
 
-                if wakeup is not None and wakeup in r:
-                    signal_byte = os.read(wakeup, 1)
-                    signal_int = int.from_bytes(signal_byte, sys.byteorder)
-                    yield signal_int
-
                 if conn in r:
                     conn.poll()
 
-                    notify_list = []
-                    while conn.notifies:
-                        notify_list.append(conn.notifies.pop())
-
+                    # copy the conn.notifies list/queue & empty it
+                    notify_list, conn.notifies = conn.notifies, []
                     for notif in notify_list:
                         yield notif
 
             except select.error as e:
-                e_num, _e_message = e  # pylint: disable=unpacking-non-sequence
-                if e_num == errno.EINTR:
+                if e.errno == errno.EINTR:
                     pass
                 else:
                     raise
     finally:
         conn.close()
-        for s in signals_to_handle or []:
-            if s in original_handlers:
-                # Commenting out to get pylint to pass
-                # https://github.com/dagster-io/dagster/issues/2510
-                # signal_name = construct_signals(s).name
-                signal.signal(s, original_handlers[s])
```

### Comparing `dagster-postgres-0.9.9rc1/dagster_postgres.egg-info/PKG-INFO` & `dagster-postgres-1.0.5/dagster_postgres.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-postgres
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: A Dagster integration for postgres
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-postgres
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-postgres-0.9.9rc1/setup.py` & `dagster-postgres-1.0.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,43 @@
+from typing import Dict
+
 from setuptools import find_packages, setup
 
 
-def get_version():
-    version = {}
-    with open("dagster_postgres/version.py") as fp:
+def get_version() -> str:
+    version: Dict[str, str] = {}
+    with open("dagster_postgres/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
 if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
     setup(
         name="dagster-postgres",
-        version=get_version(),
+        version=ver,
         author="Elementl",
         author_email="hello@elementl.com",
         license="Apache-2.0",
         description="A Dagster integration for postgres",
         url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-postgres",
         classifiers=[
-            "Programming Language :: Python :: 2.7",
-            "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: OS Independent",
         ],
-        packages=find_packages(exclude=["test"]),
+        packages=find_packages(exclude=["dagster_postgres_tests*"]),
         package_data={
             "dagster-postgres": [
-                "dagster_postgres/event_log/alembic/*",
-                "dagster_postgres/run_storage/alembic/*",
-                "dagster_postgres/schedule_storage/alembic/*",
+                "dagster_postgres/alembic/*",
             ]
         },
         include_package_data=True,
-        install_requires=["dagster", "psycopg2-binary"],
+        install_requires=["dagster==1.0.5", "psycopg2-binary"],
         zip_safe=False,
     )
```

