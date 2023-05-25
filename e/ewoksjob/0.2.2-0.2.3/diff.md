# Comparing `tmp/ewoksjob-0.2.2.tar.gz` & `tmp/ewoksjob-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksjob-0.2.2.tar", last modified: Thu May 18 07:29:48 2023, max compression
+gzip compressed data, was "dist/ewoksjob-0.2.3.tar", last modified: Thu May 25 20:39:50 2023, max compression
```

## Comparing `ewoksjob-0.2.2.tar` & `ewoksjob-0.2.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2627 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/apps/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/apps/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1654 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/apps/ewoks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/client/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/client/celery/
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/client/celery/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/client/celery/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/client/celery/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/client/dummy_workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/client/local/
--rw-rw-rw-   0 root         (0) root         (0)      374 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/client/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4410 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/client/local/pool.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/client/local/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/client/local/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5172 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/events/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-18 07:29:42.000000 ewoksjob-0.2.2/src/ewoksjob/events/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/events/handlers/
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/events/handlers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1904 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/events/handlers/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/events/readers/
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/events/readers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5423 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/events/readers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/events/readers/redis.py
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/events/readers/sqlite3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-18 07:29:42.000000 ewoksjob-0.2.2/src/ewoksjob/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4472 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2092 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_cancel.py
--rw-rw-rw-   0 root         (0) root         (0)     2391 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      665 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_convert.py
--rw-rw-rw-   0 root         (0) root         (0)     1365 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_convert_and_execute.py
--rw-rw-rw-   0 root         (0) root         (0)     2617 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_events.py
--rw-rw-rw-   0 root         (0) root         (0)      961 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_execute.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_execute_and_upload.py
--rw-rw-rw-   0 root         (0) root         (0)     1814 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_feedback.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_future.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_futures.py
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_task_discovery.py
--rw-rw-rw-   0 root         (0) root         (0)      989 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/worker/
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1557 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/worker/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     5824 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/worker/options.py
--rw-rw-rw-   0 root         (0) root         (0)     7410 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/worker/process.py
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/worker/process_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/worker/slurm.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/worker/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2627 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1708 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      835 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2627 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1687 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/src/ewoksjob/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-25 20:33:57.000000 ewoksjob-0.2.3/src/ewoksjob/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/src/ewoksjob/apps/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/apps/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/apps/ewoks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/src/ewoksjob/client/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/src/ewoksjob/client/celery/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/client/celery/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/client/celery/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/client/celery/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/client/dummy_workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/src/ewoksjob/client/local/
+-rw-rw-rw-   0 root         (0) root         (0)      374 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/client/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4410 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/client/local/pool.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/client/local/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/client/local/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5172 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/src/ewoksjob/events/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 20:39:44.000000 ewoksjob-0.2.3/src/ewoksjob/events/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/src/ewoksjob/events/handlers/
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/events/handlers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/events/handlers/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/src/ewoksjob/events/readers/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/events/readers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5423 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/events/readers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/events/readers/redis.py
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/events/readers/sqlite3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/src/ewoksjob/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 20:39:44.000000 ewoksjob-0.2.3/src/ewoksjob/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4472 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/tests/test_cancel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2391 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      665 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/tests/test_convert.py
+-rw-rw-rw-   0 root         (0) root         (0)     1365 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/tests/test_convert_and_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2617 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/tests/test_events.py
+-rw-rw-rw-   0 root         (0) root         (0)      961 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/tests/test_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/tests/test_execute_and_upload.py
+-rw-rw-rw-   0 root         (0) root         (0)     1814 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/tests/test_feedback.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/tests/test_future.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/tests/test_futures.py
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/tests/test_task_discovery.py
+-rw-rw-rw-   0 root         (0) root         (0)      989 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/src/ewoksjob/worker/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/worker/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5824 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/worker/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     7410 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/worker/process.py
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/worker/process_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/worker/slurm.py
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-05-25 20:03:10.000000 ewoksjob-0.2.3/src/ewoksjob/worker/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/src/ewoksjob.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2627 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/src/ewoksjob.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/src/ewoksjob.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/src/ewoksjob.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/src/ewoksjob.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      851 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/src/ewoksjob.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-25 20:39:50.000000 ewoksjob-0.2.3/src/ewoksjob.egg-info/top_level.txt
```

### Comparing `ewoksjob-0.2.2/LICENSE.md` & `ewoksjob-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/PKG-INFO` & `ewoksjob-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksjob
-Version: 0.2.2
+Version: 0.2.3
 Summary: Asynchronous and distributed scheduling of Ewoks workflows from python
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksjob/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksjob/
 Project-URL: Documentation, https://ewoksjob.readthedocs.io/
```

### Comparing `ewoksjob-0.2.2/README.md` & `ewoksjob-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/setup.cfg` & `ewoksjob-0.2.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 [options]
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	celery[tblib] >= 5,!=5.3.0rc1
+	kombu !=5.3.0rc1
 	importlib-metadata<5.0; python_version<"3.8"
 	ewoksutils >=0.1.1
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
```

### Comparing `ewoksjob-0.2.2/src/ewoksjob/__main__.py` & `ewoksjob-0.2.3/src/ewoksjob/__main__.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/apps/ewoks.py` & `ewoksjob-0.2.3/src/ewoksjob/apps/ewoks.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/client/celery/__init__.py` & `ewoksjob-0.2.3/src/ewoksjob/client/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/client/celery/tasks.py` & `ewoksjob-0.2.3/src/ewoksjob/client/celery/tasks.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/client/celery/utils.py` & `ewoksjob-0.2.3/src/ewoksjob/client/celery/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/client/dummy_workflow.py` & `ewoksjob-0.2.3/src/ewoksjob/client/dummy_workflow.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/client/local/pool.py` & `ewoksjob-0.2.3/src/ewoksjob/client/local/pool.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/client/local/tasks.py` & `ewoksjob-0.2.3/src/ewoksjob/client/local/tasks.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/client/local/utils.py` & `ewoksjob-0.2.3/src/ewoksjob/client/local/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/config.py` & `ewoksjob-0.2.3/src/ewoksjob/config.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/events/handlers/redis.py` & `ewoksjob-0.2.3/src/ewoksjob/events/handlers/redis.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/events/readers/__init__.py` & `ewoksjob-0.2.3/src/ewoksjob/events/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/events/readers/base.py` & `ewoksjob-0.2.3/src/ewoksjob/events/readers/base.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/events/readers/redis.py` & `ewoksjob-0.2.3/src/ewoksjob/events/readers/redis.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/events/readers/sqlite3.py` & `ewoksjob-0.2.3/src/ewoksjob/events/readers/sqlite3.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/tests/conftest.py` & `ewoksjob-0.2.3/src/ewoksjob/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/tests/test_cancel.py` & `ewoksjob-0.2.3/src/ewoksjob/tests/test_cancel.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/tests/test_config.py` & `ewoksjob-0.2.3/src/ewoksjob/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/tests/test_convert.py` & `ewoksjob-0.2.3/src/ewoksjob/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/tests/test_convert_and_execute.py` & `ewoksjob-0.2.3/src/ewoksjob/tests/test_convert_and_execute.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/tests/test_events.py` & `ewoksjob-0.2.3/src/ewoksjob/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/tests/test_execute.py` & `ewoksjob-0.2.3/src/ewoksjob/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/tests/test_execute_and_upload.py` & `ewoksjob-0.2.3/src/ewoksjob/tests/test_execute_and_upload.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/tests/test_feedback.py` & `ewoksjob-0.2.3/src/ewoksjob/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/tests/test_future.py` & `ewoksjob-0.2.3/src/ewoksjob/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/tests/test_futures.py` & `ewoksjob-0.2.3/src/ewoksjob/tests/test_futures.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/tests/utils.py` & `ewoksjob-0.2.3/src/ewoksjob/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/worker/errors.py` & `ewoksjob-0.2.3/src/ewoksjob/worker/errors.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/worker/options.py` & `ewoksjob-0.2.3/src/ewoksjob/worker/options.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/worker/process.py` & `ewoksjob-0.2.3/src/ewoksjob/worker/process.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/worker/slurm.py` & `ewoksjob-0.2.3/src/ewoksjob/worker/slurm.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob/worker/task.py` & `ewoksjob-0.2.3/src/ewoksjob/worker/task.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob.egg-info/PKG-INFO` & `ewoksjob-0.2.3/src/ewoksjob.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksjob
-Version: 0.2.2
+Version: 0.2.3
 Summary: Asynchronous and distributed scheduling of Ewoks workflows from python
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksjob/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksjob/
 Project-URL: Documentation, https://ewoksjob.readthedocs.io/
```

### Comparing `ewoksjob-0.2.2/src/ewoksjob.egg-info/SOURCES.txt` & `ewoksjob-0.2.3/src/ewoksjob.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.2/src/ewoksjob.egg-info/requires.txt` & `ewoksjob-0.2.3/src/ewoksjob.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 celery[tblib]!=5.3.0rc1,>=5
+kombu!=5.3.0rc1
 ewoksutils>=0.1.1
 
 [:python_version < "3.8"]
 importlib-metadata<5.0
 
 [beacon]
 blissdata
```

