# Comparing `tmp/acryl-executor-0.0.3rc7.tar.gz` & `tmp/acryl-executor-0.0.3rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acryl-executor-0.0.3rc7.tar", last modified: Sat Jul 30 00:51:21 2022, max compression
+gzip compressed data, was "acryl-executor-0.0.3rc8.tar", last modified: Wed Aug 17 20:57:50 2022, max compression
```

## Comparing `acryl-executor-0.0.3rc7.tar` & `acryl-executor-0.0.3rc8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 00:51:21.222318 acryl-executor-0.0.3rc7/
--rw-r--r--   0 runner    (1001) docker     (121)    13582 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-07-30 00:51:21.222318 acryl-executor-0.0.3rc7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 00:51:21.218318 acryl-executor-0.0.3rc7/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1273 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/scripts/ingestion_common.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      832 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/scripts/run_ingest.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1154 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/scripts/run_test_connection.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-07-30 00:51:21.226318 acryl-executor-0.0.3rc7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4117 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 00:51:21.218318 acryl-executor-0.0.3rc7/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 00:51:21.218318 acryl-executor-0.0.3rc7/src/acryl/
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-07-30 00:51:13.000000 acryl-executor-0.0.3rc7/src/acryl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5645 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 00:51:21.218318 acryl-executor-0.0.3rc7/src/acryl/executor/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 00:51:21.218318 acryl-executor-0.0.3rc7/src/acryl/executor/common/
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/common/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 00:51:21.218318 acryl-executor-0.0.3rc7/src/acryl/executor/context/
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1600 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/context/execution_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/context/executor_context.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 00:51:21.218318 acryl-executor-0.0.3rc7/src/acryl/executor/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3179 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/dispatcher/default_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/dispatcher/dispatcher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 00:51:21.222318 acryl-executor-0.0.3rc7/src/acryl/executor/execution/
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7695 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/execution/default_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/execution/executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/execution/in_mem_ingestion_task.py
--rw-r--r--   0 runner    (1001) docker     (121)     8475 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/execution/reporting_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     4750 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/execution/sub_process_ingestion_task.py
--rw-r--r--   0 runner    (1001) docker     (121)     4276 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/execution/sub_process_task_common.py
--rw-r--r--   0 runner    (1001) docker     (121)     4820 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/execution/sub_process_test_connection_task.py
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/execution/task.py
--rw-r--r--   0 runner    (1001) docker     (121)     4852 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/execution/task_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 00:51:21.222318 acryl-executor-0.0.3rc7/src/acryl/executor/report/
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2433 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/report/execution_report.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 00:51:21.222318 acryl-executor-0.0.3rc7/src/acryl/executor/request/
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/request/execution_request.py
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/request/signal_request.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 00:51:21.222318 acryl-executor-0.0.3rc7/src/acryl/executor/result/
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/result/execution_result.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 00:51:21.222318 acryl-executor-0.0.3rc7/src/acryl/executor/secret/
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2970 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/secret/datahub_secret_store.py
--rw-r--r--   0 runner    (1001) docker     (121)     2299 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/secret/datahub_secrets_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/secret/environment_secret_store.py
--rw-r--r--   0 runner    (1001) docker     (121)     1699 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/secret/secret_store.py
--rw-r--r--   0 runner    (1001) docker     (121)     5345 2022-07-30 00:50:43.000000 acryl-executor-0.0.3rc7/src/acryl/executor/secret/secret_store_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 00:51:21.222318 acryl-executor-0.0.3rc7/src/acryl_executor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-07-30 00:51:21.000000 acryl-executor-0.0.3rc7/src/acryl_executor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1919 2022-07-30 00:51:21.000000 acryl-executor-0.0.3rc7/src/acryl_executor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-30 00:51:21.000000 acryl-executor-0.0.3rc7/src/acryl_executor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-07-30 00:51:21.000000 acryl-executor-0.0.3rc7/src/acryl_executor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-30 00:51:20.000000 acryl-executor-0.0.3rc7/src/acryl_executor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-07-30 00:51:21.000000 acryl-executor-0.0.3rc7/src/acryl_executor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-07-30 00:51:21.000000 acryl-executor-0.0.3rc7/src/acryl_executor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:57:50.732157 acryl-executor-0.0.3rc8/
+-rw-r--r--   0 runner    (1001) docker     (121)    13582 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2097 2022-08-17 20:57:50.732157 acryl-executor-0.0.3rc8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      819 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:57:50.728157 acryl-executor-0.0.3rc8/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1273 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/scripts/ingestion_common.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      832 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/scripts/run_ingest.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1154 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/scripts/run_test_connection.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-08-17 20:57:50.732157 acryl-executor-0.0.3rc8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4117 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:57:50.728157 acryl-executor-0.0.3rc8/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:57:50.728157 acryl-executor-0.0.3rc8/src/acryl/
+-rw-r--r--   0 runner    (1001) docker     (121)      907 2022-08-17 20:57:43.000000 acryl-executor-0.0.3rc8/src/acryl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5645 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:57:50.728157 acryl-executor-0.0.3rc8/src/acryl/executor/
+-rw-r--r--   0 runner    (1001) docker     (121)      579 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:57:50.728157 acryl-executor-0.0.3rc8/src/acryl/executor/common/
+-rw-r--r--   0 runner    (1001) docker     (121)      578 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      684 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/common/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:57:50.728157 acryl-executor-0.0.3rc8/src/acryl/executor/context/
+-rw-r--r--   0 runner    (1001) docker     (121)      578 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1600 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/context/execution_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/context/executor_context.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:57:50.728157 acryl-executor-0.0.3rc8/src/acryl/executor/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (121)      578 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3179 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/dispatcher/default_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/dispatcher/dispatcher.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:57:50.732157 acryl-executor-0.0.3rc8/src/acryl/executor/execution/
+-rw-r--r--   0 runner    (1001) docker     (121)      578 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7699 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/execution/default_executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/execution/executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/execution/in_mem_ingestion_task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9492 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/execution/reporting_executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5848 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/execution/sub_process_ingestion_task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4413 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/execution/sub_process_task_common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4820 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/execution/sub_process_test_connection_task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/execution/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4852 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/execution/task_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:57:50.732157 acryl-executor-0.0.3rc8/src/acryl/executor/report/
+-rw-r--r--   0 runner    (1001) docker     (121)      578 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2433 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/report/execution_report.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:57:50.732157 acryl-executor-0.0.3rc8/src/acryl/executor/request/
+-rw-r--r--   0 runner    (1001) docker     (121)      578 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/request/execution_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)      923 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/request/signal_request.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:57:50.732157 acryl-executor-0.0.3rc8/src/acryl/executor/result/
+-rw-r--r--   0 runner    (1001) docker     (121)      578 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2021 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/result/execution_result.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:57:50.732157 acryl-executor-0.0.3rc8/src/acryl/executor/secret/
+-rw-r--r--   0 runner    (1001) docker     (121)      578 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2970 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/secret/datahub_secret_store.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2299 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/secret/datahub_secrets_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/secret/environment_secret_store.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1699 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/secret/secret_store.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5345 2022-08-17 20:57:10.000000 acryl-executor-0.0.3rc8/src/acryl/executor/secret/secret_store_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 20:57:50.732157 acryl-executor-0.0.3rc8/src/acryl_executor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2097 2022-08-17 20:57:50.000000 acryl-executor-0.0.3rc8/src/acryl_executor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1919 2022-08-17 20:57:50.000000 acryl-executor-0.0.3rc8/src/acryl_executor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-17 20:57:50.000000 acryl-executor-0.0.3rc8/src/acryl_executor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      137 2022-08-17 20:57:50.000000 acryl-executor-0.0.3rc8/src/acryl_executor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-17 20:57:50.000000 acryl-executor-0.0.3rc8/src/acryl_executor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2022-08-17 20:57:50.000000 acryl-executor-0.0.3rc8/src/acryl_executor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-08-17 20:57:50.000000 acryl-executor-0.0.3rc8/src/acryl_executor.egg-info/top_level.txt
```

### Comparing `acryl-executor-0.0.3rc7/LICENSE` & `acryl-executor-0.0.3rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/PKG-INFO` & `acryl-executor-0.0.3rc8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acryl-executor
-Version: 0.0.3rc7
+Version: 0.0.3rc8
 Summary: An library used within Acryl Agents to execute tasks
 Home-page: https://datahubproject.io/
 License: Apache License 2.0
 Project-URL: Documentation, https://datahubproject.io/docs/
 Project-URL: Source, https://github.com/linkedin/datahub
 Project-URL: Changelog, https://github.com/linkedin/datahub/releases
 Classifier: Programming Language :: Python
@@ -29,17 +29,16 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # acryl-executor
 Remote execution agent used for running DataHub tasks. 
 
 
-```
-cd src
-python3 -m venv venv
+```bash
+python3 -m venv --upgrade-deps venv
 source venv/bin/activate
 pip3 install .
 ```
 
 ## Notes
 
 By default, this library comes with a set of default task implementations:
```

### Comparing `acryl-executor-0.0.3rc7/README.md` & `acryl-executor-0.0.3rc8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # acryl-executor
 Remote execution agent used for running DataHub tasks. 
 
 
-```
-cd src
-python3 -m venv venv
+```bash
+python3 -m venv --upgrade-deps venv
 source venv/bin/activate
 pip3 install .
 ```
 
 ## Notes
 
 By default, this library comes with a set of default task implementations:
```

### Comparing `acryl-executor-0.0.3rc7/scripts/ingestion_common.sh` & `acryl-executor-0.0.3rc8/scripts/ingestion_common.sh`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/scripts/run_ingest.sh` & `acryl-executor-0.0.3rc8/scripts/run_ingest.sh`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/scripts/run_test_connection.sh` & `acryl-executor-0.0.3rc8/scripts/run_test_connection.sh`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/setup.cfg` & `acryl-executor-0.0.3rc8/setup.cfg`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/setup.py` & `acryl-executor-0.0.3rc8/setup.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/__init__.py` & `acryl-executor-0.0.3rc8/src/acryl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # To be published at https://pypi.org/project/acryl-datahub/.
 __package_name__ = "acryl-executor"
-__version__ = "0.0.3rc7"
+__version__ = "0.0.3rc8"
 
 def is_dev_mode() -> bool:
     return __version__ == "0.0.0.dev0"
 
 
 def nice_version_name() -> str:
     if is_dev_mode():
```

### Comparing `acryl-executor-0.0.3rc7/src/acryl/__main__.py` & `acryl-executor-0.0.3rc8/src/acryl/__main__.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/__init__.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/common/__init__.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/common/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/common/config.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/common/config.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/context/__init__.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/context/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/context/execution_context.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/context/execution_context.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/context/executor_context.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/context/executor_context.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/dispatcher/__init__.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/dispatcher/default_dispatcher.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/dispatcher/default_dispatcher.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/dispatcher/dispatcher.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/dispatcher/dispatcher.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/execution/__init__.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/execution/default_executor.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/execution/default_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import logging
 import traceback
 import asyncio
 import logging
 import nest_asyncio
 
-from typing import Dict, List
+from typing import Any, Dict, List
 from acryl.executor.common.config import ConfigModel
 from acryl.executor.execution.executor import Executor
 from acryl.executor.report.execution_report import ExecutionReport
 from acryl.executor.context.executor_context import ExecutorContext
 from acryl.executor.context.execution_context import ExecutionContext
 from acryl.executor.execution.task import Task, TaskConfig
 from acryl.executor.execution.task_registry import TaskRegistry
@@ -55,15 +55,15 @@
     # Patch the primary event loop to permit multiple runs 
     nest_asyncio.apply(event_loop)
 
 
     # Tasks
     task_registry: TaskRegistry = TaskRegistry()
     task_instances: Dict[str, Task] = {}
-    task_futures: Dict[str, List[any]] = {} 
+    task_futures: Dict[str, List[Any]] = {}
 
     # Secret Stores 
     secret_stores: List[SecretStore] = []
 
     def __init__(self, config: DefaultExecutorConfig) -> None:
         # Register the tasks 
         self.id = config.id
```

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/execution/executor.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/execution/executor.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/execution/in_mem_ingestion_task.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/execution/in_mem_ingestion_task.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/execution/reporting_executor.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/execution/reporting_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import time
 import signal
 
 from acryl.executor.execution.default_executor import DefaultExecutor, DefaultExecutorConfig
 from acryl.executor.execution.task import TaskConfig
 from acryl.executor.request.signal_request import SignalRequest
 from acryl.executor.request.execution_request import ExecutionRequest
-from acryl.executor.result.execution_result import ExecutionResult
+from acryl.executor.result.execution_result import ExecutionResult, Type
 from acryl.executor.secret.secret_store import SecretStoreConfig
 from datahub.metadata.schema_classes import ExecutionRequestResultClass, ExecutionRequestKeyClass, ExecutionRequestSignalClass, StructuredExecutionReportClass
 from datahub.metadata.com.linkedin.pegasus2avro.mxe import (
     GenericAspectClass
 )
 from datahub.emitter.mcp import MetadataChangeProposalWrapper
 from datahub.emitter.serialization_helper import pre_json_transform
@@ -74,14 +74,15 @@
         start_time_ms = round(time.time() * 1000)
 
         # Build & emit an ACK mcp
         kickoff_mcp = self._build_kickoff_mcp(request, start_time_ms)
         self._datahub_graph.emit_mcp(kickoff_mcp)
 
         # Execute the request  
+        request.progress_callback = lambda partial_report: self._datahub_graph.emit_mcp(self._build_progress_mcp(request, start_time_ms, partial_report=partial_report))
         exec_result = super().execute(request)
 
         # Execution has completed. Report the status. Only consider the first task in the list. 
         # TODO: Support timed out state. 
         status = exec_result.type.name
 
         # Capture the report
@@ -112,27 +113,45 @@
                 self._datahub_graph.emit_mcp(cancellation_mcp)
             
     # Builds an MCP to report the start of execution request handling 
     def _build_kickoff_mcp(self, exec_request: ExecutionRequest, start_time_ms: int) -> MetadataChangeProposalWrapper: 
         assert exec_request.exec_id, f"Missing exec_id for request {exec_request}"
         key_aspect = self._build_execution_request_key_aspect(exec_request.exec_id)
         result_aspect = self._build_execution_request_result_aspect(
-            status="RUNNING",
+            status=Type.RUNNING.name,
             start_time_ms=start_time_ms
         )
 
         return MetadataChangeProposalWrapper(
             entityType=DATAHUB_EXECUTION_REQUEST_ENTITY_NAME,
             changeType="UPSERT",
             auditHeader=None,
             entityKeyAspect=key_aspect,
             aspectName=DATAHUB_EXECUTION_REQUEST_RESULT_ASPECT_NAME,
             aspect=result_aspect
         )
 
+    def _build_progress_mcp(self, exec_request: ExecutionRequest, start_time_ms: int, partial_report: str) -> MetadataChangeProposalWrapper:
+        assert exec_request.exec_id, f"Missing exec_id for request {exec_request}"
+        key_aspect = self._build_execution_request_key_aspect(exec_request.exec_id)
+        result_aspect = self._build_execution_request_result_aspect(
+            status=Type.RUNNING.name,
+            start_time_ms=start_time_ms,
+            report=partial_report,
+        )
+
+        return MetadataChangeProposalWrapper(
+            entityType=DATAHUB_EXECUTION_REQUEST_ENTITY_NAME,
+            changeType="UPSERT",
+            auditHeader=None,
+            entityKeyAspect=key_aspect,
+            aspectName=DATAHUB_EXECUTION_REQUEST_RESULT_ASPECT_NAME,
+            aspect=result_aspect
+        )
+
     # Builds an MCP to report the completion of execution request handling 
     def _build_completion_mcp(self, exec_request: ExecutionRequest, status: str, start_time_ms: int, duration_ms: int, report: str, structured_report: Optional[str]) -> MetadataChangeProposalWrapper: 
         key_aspect = self._build_execution_request_key_aspect(exec_request.exec_id or "missing execution id")
         result_aspect = self._build_execution_request_result_aspect(
             status=status,
             start_time_ms=start_time_ms,
             duration_ms=duration_ms,
@@ -151,15 +170,15 @@
 
     # Builds an MCP to report the completion of execution request handling 
     def _build_empty_cancel_mcp(self, exec_id: str) -> MetadataChangeProposalWrapper: 
         key_aspect = self._build_execution_request_key_aspect(exec_id)
 
         # TODO: Determine whether this is the "right" thing to do.
         result_aspect = self._build_execution_request_result_aspect(
-            status="CANCELLED",
+            status=Type.CANCELLED.name,
             start_time_ms=0, # TODO: Make start time optional
             duration_ms=None,
             report="No active execution request found."
         )
 
         return MetadataChangeProposalWrapper(
             entityType=DATAHUB_EXECUTION_REQUEST_ENTITY_NAME,
```

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/execution/sub_process_ingestion_task.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/execution/sub_process_test_connection_task.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,115 +8,111 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
 import sys
 import subprocess
+import os
 import logging
 import asyncio
 from collections import deque
-from acryl.executor.execution.sub_process_task_common import SubProcessTaskUtil
 from acryl.executor.execution.task import Task
 from acryl.executor.execution.task import TaskError
-from acryl.executor.result.execution_result import Type
 from acryl.executor.context.executor_context import ExecutorContext
 from acryl.executor.context.execution_context import ExecutionContext
 from acryl.executor.common.config import ConfigModel
+from acryl.executor.execution.sub_process_task_common import SubProcessTaskUtil
+from typing import List
 
 logger = logging.getLogger(__name__)
 
-class SubProcessIngestionTaskConfig(ConfigModel):
+class SubProcessTestConnectionTaskConfig(ConfigModel):
     tmp_dir: str = "/tmp/datahub/ingest"
-    heartbeat_time_seconds: int = 10
-    max_log_lines: int = SubProcessTaskUtil.MAX_LOG_LINES
 
-class SubProcessIngestionTaskArgs(ConfigModel):
+class SubProcessTestConnectionTaskArgs(ConfigModel):
     recipe: str
     version: str = "latest"
 
-class SubProcessIngestionTask(Task):
+class SubProcessTestConnectionTask(Task):
 
-    config: SubProcessIngestionTaskConfig
+    config: SubProcessTestConnectionTaskConfig
     tmp_dir: str # Location where tmp files will be written (recipes) 
     ctx: ExecutorContext
 
     @classmethod
     def create(cls, config: dict, ctx: ExecutorContext) -> "Task":
-        return cls(SubProcessIngestionTaskConfig.parse_obj(config), ctx)
+        config_parsed = SubProcessTestConnectionTaskConfig.parse_obj(config)
+        return cls(config_parsed, ctx)
 
-    def __init__(self, config: SubProcessIngestionTaskConfig, ctx: ExecutorContext):
+    def __init__(self, config: SubProcessTestConnectionTaskConfig, ctx: ExecutorContext):
         self.config = config
         self.tmp_dir = config.tmp_dir
         self.ctx = ctx 
 
     async def execute(self, args: dict, ctx: ExecutionContext) -> None:
 
-        exec_id = ctx.exec_id # The unique execution id. 
+        exec_id = ctx.exec_id # The unique execution id.
 
         exec_out_dir = f"{self.tmp_dir}/{exec_id}"
 
         # 0. Validate arguments 
-        validated_args = SubProcessIngestionTaskArgs.parse_obj(args)
+        validated_args = SubProcessTestConnectionTaskArgs.parse_obj(args)
 
         # 1. Resolve the recipe (combine it with others)
-        recipe: dict = SubProcessTaskUtil._resolve_recipe(validated_args.recipe, ctx, self.ctx)
+        recipe: dict = SubProcessTaskUtil._resolve_recipe(validated_args.recipe, execution_ctx=ctx, executor_ctx=self.ctx)
 
         # 2. Write recipe file to local FS (requires write permissions to /tmp directory)
-        file_name: str = "recipe.yml"  
-        SubProcessTaskUtil._write_recipe_to_file(exec_out_dir, file_name, recipe)
+        recipe_file: str = "recipe.yml"  
+        SubProcessTaskUtil._write_recipe_to_file(exec_out_dir, recipe_file, recipe)
+        recipe_file_loc: str = f"{exec_out_dir}/{recipe_file}"
 
         # 3. Spin off subprocess to run the run_ingest.sh script
         datahub_version = validated_args.version # The version of DataHub CLI to use. 
         plugins = recipe["source"]["type"] # The source type -- ASSUMPTION ALERT: This should always correspond to the plugin name. 
-        command_script: str = "run_ingest.sh" # TODO: Make sure this is EXECUTABLE.  
-
-        stdout_lines: deque[str] = deque(maxlen=self.config.max_log_lines)
+        command_script: str = "run_test_connection.sh" # TODO: Make sure this is EXECUTABLE.  
+        report_out_file: str = f"{exec_out_dir}/connection_report.json"
+        stdout_lines: deque = deque(maxlen=SubProcessTaskUtil.MAX_LOG_LINES)
 
         # TODO: Inject a token into the recipe to run such that it "just works" (currently, a token is required)
-        report_out_file = f"{exec_out_dir}/ingestion_report.json"
-        ingest_process = subprocess.Popen([command_script, exec_id, datahub_version, plugins, self.tmp_dir, f"{exec_out_dir}/recipe.yml", report_out_file], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, text=True)
+
+        ingest_process = subprocess.Popen([command_script, exec_id, datahub_version, plugins, self.tmp_dir, recipe_file_loc, report_out_file], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, text=True)
 
         try: 
             while ingest_process.poll() is None:
                 assert ingest_process.stdout
                 line = ingest_process.stdout.readline()
 
                 sys.stdout.write(line)
                 stdout_lines.append(line)
-
                 await asyncio.sleep(0)
 
             return_code = ingest_process.poll()
 
         except asyncio.CancelledError:
             # Terminate the running child process 
             ingest_process.terminate()
-            raise
+            raise  
 
         finally:
             if os.path.exists(report_out_file):
                 with open(report_out_file,'r') as structured_report_fp:
                     ctx.get_report().set_structured_report(structured_report_fp.read())
 
             ctx.get_report().report_info(f"stdout={SubProcessTaskUtil._format_log_lines(stdout_lines)}")
             
-            # Cleanup by removing the recipe file
+            # Cleanup by removing the exec out directory
             SubProcessTaskUtil._remove_directory(exec_out_dir)
 
         if return_code != 0:
             # Failed
-            ctx.get_report().report_info("Failed to execute 'datahub ingest'")
-            raise TaskError("Failed to execute 'datahub ingest'") 
+            ctx.get_report().report_info("Failed to execute 'datahub test connection'")
+            raise TaskError("Failed to execute 'datahub test connection'") 
         
         # Report Successful execution
-        ctx.get_report().report_info("Successfully executed 'datahub ingest'")
+        ctx.get_report().report_info("Successfully executed 'datahub test connection'")
 
 
     def close(self) -> None:
-        pass
-
-    
-
+        pass
```

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/execution/sub_process_task_common.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/execution/sub_process_task_common.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,19 @@
 
 class SubProcessTaskUtil:
 
     MAX_LOG_LINES = 2000
 
     @staticmethod
     def _format_log_lines(lines: Sequence[str]) -> str: 
-        return "".join(lines)
+        text = "".join(lines)
+        if len(lines) > SubProcessTaskUtil.MAX_LOG_LINES:
+            text = f"[earlier logs truncated...]\n{text}"
+
+        return text
 
     @staticmethod
     def _resolve_secrets(secret_names: List[str], ctx: ExecutorContext) -> dict:
         # Attempt to resolve secret using by checking each configured secret store.
         secret_stores = ctx.get_secret_stores()
         final_secret_values = dict({})
```

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/execution/sub_process_test_connection_task.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/execution/sub_process_ingestion_task.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,111 +8,144 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from asyncio import tasks
+import os
 import sys
 import subprocess
-import os
 import logging
 import asyncio
 from collections import deque
+from acryl.executor.execution.sub_process_task_common import SubProcessTaskUtil
 from acryl.executor.execution.task import Task
 from acryl.executor.execution.task import TaskError
+from acryl.executor.result.execution_result import Type
 from acryl.executor.context.executor_context import ExecutorContext
 from acryl.executor.context.execution_context import ExecutionContext
 from acryl.executor.common.config import ConfigModel
-from acryl.executor.execution.sub_process_task_common import SubProcessTaskUtil
-from typing import List
 
 logger = logging.getLogger(__name__)
 
-class SubProcessTestConnectionTaskConfig(ConfigModel):
+class SubProcessIngestionTaskConfig(ConfigModel):
     tmp_dir: str = "/tmp/datahub/ingest"
+    heartbeat_time_seconds: int = 2
+    max_log_lines: int = SubProcessTaskUtil.MAX_LOG_LINES
 
-class SubProcessTestConnectionTaskArgs(ConfigModel):
+class SubProcessIngestionTaskArgs(ConfigModel):
     recipe: str
     version: str = "latest"
 
-class SubProcessTestConnectionTask(Task):
+class SubProcessIngestionTask(Task):
 
-    config: SubProcessTestConnectionTaskConfig
+    config: SubProcessIngestionTaskConfig
     tmp_dir: str # Location where tmp files will be written (recipes) 
     ctx: ExecutorContext
 
     @classmethod
     def create(cls, config: dict, ctx: ExecutorContext) -> "Task":
-        config_parsed = SubProcessTestConnectionTaskConfig.parse_obj(config)
-        return cls(config_parsed, ctx)
+        return cls(SubProcessIngestionTaskConfig.parse_obj(config), ctx)
 
-    def __init__(self, config: SubProcessTestConnectionTaskConfig, ctx: ExecutorContext):
+    def __init__(self, config: SubProcessIngestionTaskConfig, ctx: ExecutorContext):
         self.config = config
         self.tmp_dir = config.tmp_dir
         self.ctx = ctx 
 
     async def execute(self, args: dict, ctx: ExecutionContext) -> None:
 
-        exec_id = ctx.exec_id # The unique execution id.
+        exec_id = ctx.exec_id # The unique execution id. 
 
         exec_out_dir = f"{self.tmp_dir}/{exec_id}"
 
         # 0. Validate arguments 
-        validated_args = SubProcessTestConnectionTaskArgs.parse_obj(args)
+        validated_args = SubProcessIngestionTaskArgs.parse_obj(args)
 
         # 1. Resolve the recipe (combine it with others)
-        recipe: dict = SubProcessTaskUtil._resolve_recipe(validated_args.recipe, execution_ctx=ctx, executor_ctx=self.ctx)
+        recipe: dict = SubProcessTaskUtil._resolve_recipe(validated_args.recipe, ctx, self.ctx)
 
         # 2. Write recipe file to local FS (requires write permissions to /tmp directory)
-        recipe_file: str = "recipe.yml"  
-        SubProcessTaskUtil._write_recipe_to_file(exec_out_dir, recipe_file, recipe)
-        recipe_file_loc: str = f"{exec_out_dir}/{recipe_file}"
+        file_name: str = "recipe.yml"  
+        SubProcessTaskUtil._write_recipe_to_file(exec_out_dir, file_name, recipe)
 
         # 3. Spin off subprocess to run the run_ingest.sh script
         datahub_version = validated_args.version # The version of DataHub CLI to use. 
         plugins = recipe["source"]["type"] # The source type -- ASSUMPTION ALERT: This should always correspond to the plugin name. 
-        command_script: str = "run_test_connection.sh" # TODO: Make sure this is EXECUTABLE.  
-        report_out_file: str = f"{exec_out_dir}/connection_report.json"
-        stdout_lines: deque = deque(maxlen=SubProcessTaskUtil.MAX_LOG_LINES)
+        command_script: str = "run_ingest.sh" # TODO: Make sure this is EXECUTABLE.  
+
+        stdout_lines: deque[str] = deque(maxlen=self.config.max_log_lines)
 
         # TODO: Inject a token into the recipe to run such that it "just works" (currently, a token is required)
+        report_out_file = f"{exec_out_dir}/ingestion_report.json"
 
-        ingest_process = subprocess.Popen([command_script, exec_id, datahub_version, plugins, self.tmp_dir, recipe_file_loc, report_out_file], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, text=True)
+        logger.info(f'Starting ingestion subprocess for exec_id={exec_id} ({plugins})')
+        ingest_process = await asyncio.create_subprocess_exec(
+            *[command_script, exec_id, datahub_version, plugins, self.tmp_dir, f"{exec_out_dir}/recipe.yml", report_out_file],
+            stdout=asyncio.subprocess.PIPE,
+            stderr=asyncio.subprocess.STDOUT,
+        )
 
-        try: 
-            while ingest_process.poll() is None:
+        # 4. Monitor and report progress.
+        running = True
+
+        async def _read_output_lines() -> None:
+            while True:
                 assert ingest_process.stdout
-                line = ingest_process.stdout.readline()
+                line_bytes = await ingest_process.stdout.readline()
+                if not line_bytes:
+                    nonlocal running
+                    running = False
+                    break
+                line = line_bytes.decode("utf-8")
 
                 sys.stdout.write(line)
                 stdout_lines.append(line)
-                await asyncio.sleep(0)
 
-            return_code = ingest_process.poll()
+                await asyncio.sleep(0)
+        
+        async def _report_progress() -> None:
+            while True:
+                if not running:
+                    break
+
+                await asyncio.sleep(self.config.heartbeat_time_seconds)
+
+                # Report progress
+                if ctx.request.progress_callback:
+                    # TODO maybe use the normal report field here?
+                    ctx.request.progress_callback(f"stdout={SubProcessTaskUtil._format_log_lines(stdout_lines)}")
 
+                await asyncio.sleep(0)
+        
+        try: 
+            await tasks.gather(_read_output_lines(), _report_progress(), ingest_process.wait())
         except asyncio.CancelledError:
             # Terminate the running child process 
             ingest_process.terminate()
-            raise  
-
+            raise
         finally:
             if os.path.exists(report_out_file):
                 with open(report_out_file,'r') as structured_report_fp:
                     ctx.get_report().set_structured_report(structured_report_fp.read())
 
             ctx.get_report().report_info(f"stdout={SubProcessTaskUtil._format_log_lines(stdout_lines)}")
             
-            # Cleanup by removing the exec out directory
+            # Cleanup by removing the recipe file
             SubProcessTaskUtil._remove_directory(exec_out_dir)
-
+        
+        return_code = ingest_process.returncode
         if return_code != 0:
             # Failed
-            ctx.get_report().report_info("Failed to execute 'datahub test connection'")
-            raise TaskError("Failed to execute 'datahub test connection'") 
+            ctx.get_report().report_info("Failed to execute 'datahub ingest'")
+            raise TaskError("Failed to execute 'datahub ingest'") 
         
         # Report Successful execution
-        ctx.get_report().report_info("Successfully executed 'datahub test connection'")
+        ctx.get_report().report_info("Successfully executed 'datahub ingest'")
 
 
     def close(self) -> None:
-        pass
+        pass
+
+    
+
```

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/execution/task.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/execution/task.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/execution/task_registry.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/execution/task_registry.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/report/__init__.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/report/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/report/execution_report.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/report/execution_report.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/request/__init__.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/request/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/request/execution_request.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/request/signal_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,19 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List, Union, Optional
 from pydantic import BaseModel
 
-class ExecutionRequest(BaseModel):
-    # Optional executor id to target. Fallbacks back the default (local) executor. 
-    executor_id: str = "default"
+class SignalRequest(BaseModel):
+    # The execution request to signal
+    exec_id: str
 
-    # Optional run execution id provided by the caller
-    exec_id: Union[str, None]
+    # Optional executor id to target. falls back the default (local) executor. 
+    executor_id: str = "default"
 
-    # The name of the task to be executed
-    name: str
-    
-    # Arguments to provide the task to be executed
-    args: dict
+    # The signal to send to the executor (e.g. KILL)
+    signal: str
```

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/request/signal_request.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/request/execution_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,19 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import List, Union, Optional
+from typing import Callable, List, Union, Optional
 from pydantic import BaseModel
 
-class SignalRequest(BaseModel):
-    # The execution request to signal
-    exec_id: str
+ExecutionProgressCallback = Callable[[str], None]
 
-    # Optional executor id to target. falls back the default (local) executor. 
+
+class ExecutionRequest(BaseModel):
+    # Optional executor id to target. Fallbacks back the default (local) executor.
     executor_id: str = "default"
 
-    # The signal to send to the executor (e.g. KILL)
-    signal: str
+    # Optional run execution id provided by the caller
+    exec_id: Union[str, None]
+
+    # The name of the task to be executed
+    name: str
+
+    # Arguments to provide the task to be executed
+    args: dict
+
+    # Callback to report progress.
+    progress_callback: Optional[ExecutionProgressCallback] = None
```

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/result/__init__.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/result/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/result/execution_result.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/result/execution_result.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from typing import List, Optional
  
 class Type(Enum):
     SUCCESS = 1
     FAILURE = 2
     TIMEOUT = 3
     CANCELLED = 4
+    RUNNING = 5
 
 class ExecutionResult:
 
     # Result type, success or failure
     type: Type
 
     # Execution context
```

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/secret/__init__.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/secret/datahub_secret_store.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/secret/datahub_secret_store.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/secret/datahub_secrets_client.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/secret/datahub_secrets_client.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/secret/environment_secret_store.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/secret/environment_secret_store.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/secret/secret_store.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/secret/secret_store.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl/executor/secret/secret_store_registry.py` & `acryl-executor-0.0.3rc8/src/acryl/executor/secret/secret_store_registry.py`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl_executor.egg-info/PKG-INFO` & `acryl-executor-0.0.3rc8/src/acryl_executor.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acryl-executor
-Version: 0.0.3rc7
+Version: 0.0.3rc8
 Summary: An library used within Acryl Agents to execute tasks
 Home-page: https://datahubproject.io/
 License: Apache License 2.0
 Project-URL: Documentation, https://datahubproject.io/docs/
 Project-URL: Source, https://github.com/linkedin/datahub
 Project-URL: Changelog, https://github.com/linkedin/datahub/releases
 Classifier: Programming Language :: Python
@@ -29,17 +29,16 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # acryl-executor
 Remote execution agent used for running DataHub tasks. 
 
 
-```
-cd src
-python3 -m venv venv
+```bash
+python3 -m venv --upgrade-deps venv
 source venv/bin/activate
 pip3 install .
 ```
 
 ## Notes
 
 By default, this library comes with a set of default task implementations:
```

### Comparing `acryl-executor-0.0.3rc7/src/acryl_executor.egg-info/SOURCES.txt` & `acryl-executor-0.0.3rc8/src/acryl_executor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acryl-executor-0.0.3rc7/src/acryl_executor.egg-info/requires.txt` & `acryl-executor-0.0.3rc8/src/acryl_executor.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-sqlalchemy-stubs>=0.4
-pydantic>=1.5.1
-acryl-datahub[datahub-rest]>=0.8.41.1rc2
 nest-asyncio>=1.5.4
+pydantic>=1.5.1
 mypy_extensions>=0.4.3
+acryl-datahub[datahub-rest]>=0.8.41.1rc2
+sqlalchemy-stubs>=0.4
 
 [:python_version < "3.7"]
 dataclasses>=0.6
 
 [:python_version < "3.8"]
 typing_extensions>=3.7.4
 
 [dev]
-mypy<0.920,>=0.901
-pytest>=6.2.2
-flake8>=3.8.3
-sqlalchemy-stubs>=0.4
+freezegun
+types-requests
 mypy_extensions>=0.4.3
 requests-mock
-types-requests
-nest-asyncio>=1.5.4
-freezegun
+flake8-tidy-imports>=4.3.0
+types-toml
+pytest>=6.2.2
+types-freezegun
 types-PyYAML
 pydantic>=1.5.1
-types-freezegun
+types-dataclasses
 acryl-datahub[datahub-rest]>=0.8.41.1rc2
-types-toml
-flake8-tidy-imports>=4.3.0
+sqlalchemy-stubs>=0.4
+nest-asyncio>=1.5.4
+flake8>=3.8.3
 types-python-dateutil
-types-dataclasses
+mypy<0.920,>=0.901
 
 [dev:python_version < "3.7"]
 dataclasses>=0.6
 
 [dev:python_version < "3.8"]
 typing_extensions>=3.7.4
```

