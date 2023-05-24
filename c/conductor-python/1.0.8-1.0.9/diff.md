# Comparing `tmp/conductor-python-1.0.8.tar.gz` & `tmp/conductor-python-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conductor-python-1.0.8.tar", last modified: Sun Feb 20 21:54:40 2022, max compression
+gzip compressed data, was "conductor-python-1.0.9.tar", last modified: Tue Feb 22 18:08:40 2022, max compression
```

## Comparing `conductor-python-1.0.8.tar` & `conductor-python-1.0.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-20 21:54:40.212470 conductor-python-1.0.8/
--rw-r--r--   0 gardusig   (501) staff       (20)    11357 2022-02-01 00:57:09.000000 conductor-python-1.0.8/LICENSE
--rw-r--r--   0 gardusig   (501) staff       (20)     9380 2022-02-20 21:54:40.212583 conductor-python-1.0.8/PKG-INFO
--rw-r--r--   0 gardusig   (501) staff       (20)     8589 2022-02-20 21:41:51.000000 conductor-python-1.0.8/README.md
--rw-r--r--   0 gardusig   (501) staff       (20)      104 2022-02-10 12:38:53.000000 conductor-python-1.0.8/pyproject.toml
--rw-r--r--   0 gardusig   (501) staff       (20)      903 2022-02-20 21:54:40.213085 conductor-python-1.0.8/setup.cfg
-drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-20 21:54:40.200237 conductor-python-1.0.8/src/
-drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-20 21:54:40.201008 conductor-python-1.0.8/src/conductor/
--rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-11 17:02:14.000000 conductor-python-1.0.8/src/conductor/__init__.py
-drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-20 21:54:40.201160 conductor-python-1.0.8/src/conductor/client/
--rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-11 17:02:14.000000 conductor-python-1.0.8/src/conductor/client/__init__.py
--rw-r--r--   0 gardusig   (501) staff       (20)      730 2022-02-17 19:44:10.000000 conductor-python-1.0.8/src/conductor/client/__main__.py
-drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-20 21:54:40.201764 conductor-python-1.0.8/src/conductor/client/automator/
--rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-11 17:02:14.000000 conductor-python-1.0.8/src/conductor/client/automator/__init__.py
--rw-r--r--   0 gardusig   (501) staff       (20)     1173 2022-02-20 18:37:12.000000 conductor-python-1.0.8/src/conductor/client/automator/task_handler.py
--rw-r--r--   0 gardusig   (501) staff       (20)     5493 2022-02-20 21:25:59.000000 conductor-python-1.0.8/src/conductor/client/automator/task_runner.py
-drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-20 21:54:40.202070 conductor-python-1.0.8/src/conductor/client/configuration/
--rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-14 21:01:31.000000 conductor-python-1.0.8/src/conductor/client/configuration/__init__.py
--rw-r--r--   0 gardusig   (501) staff       (20)     5146 2022-02-17 19:44:10.000000 conductor-python-1.0.8/src/conductor/client/configuration/configuration.py
-drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-20 21:54:40.202942 conductor-python-1.0.8/src/conductor/client/http/
--rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-11 17:02:14.000000 conductor-python-1.0.8/src/conductor/client/http/__init__.py
-drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-20 21:54:40.204762 conductor-python-1.0.8/src/conductor/client/http/api/
--rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-11 17:02:14.000000 conductor-python-1.0.8/src/conductor/client/http/api/__init__.py
--rw-r--r--   0 gardusig   (501) staff       (20)    17824 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/api/admin_resource_api.py
--rw-r--r--   0 gardusig   (501) staff       (20)    17638 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/api/event_resource_api.py
--rw-r--r--   0 gardusig   (501) staff       (20)     3444 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/api/health_check_resource_api.py
--rw-r--r--   0 gardusig   (501) staff       (20)    34631 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/api/metadata_resource_api.py
--rw-r--r--   0 gardusig   (501) staff       (20)    16605 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/api/queue_admin_resource_api.py
--rw-r--r--   0 gardusig   (501) staff       (20)    55041 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/api/task_resource_api.py
--rw-r--r--   0 gardusig   (501) staff       (20)    18978 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/api/workflow_bulk_resource_api.py
--rw-r--r--   0 gardusig   (501) staff       (20)    84613 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/api/workflow_resource_api.py
--rw-r--r--   0 gardusig   (501) staff       (20)    24092 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/api_client.py
-drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-20 21:54:40.209640 conductor-python-1.0.8/src/conductor/client/http/models/
--rw-r--r--   0 gardusig   (501) staff       (20)     1863 2022-02-11 17:02:14.000000 conductor-python-1.0.8/src/conductor/client/http/models/__init__.py
--rw-r--r--   0 gardusig   (501) staff       (20)     6095 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/action.py
--rw-r--r--   0 gardusig   (501) staff       (20)     4030 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/bulk_response.py
--rw-r--r--   0 gardusig   (501) staff       (20)     6333 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/event_handler.py
--rw-r--r--   0 gardusig   (501) staff       (20)     3435 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/external_storage_location.py
--rw-r--r--   0 gardusig   (501) staff       (20)     4148 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/health.py
--rw-r--r--   0 gardusig   (501) staff       (20)     4714 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/health_check_status.py
--rw-r--r--   0 gardusig   (501) staff       (20)     4853 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/poll_data.py
--rw-r--r--   0 gardusig   (501) staff       (20)     6519 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/rerun_workflow_request.py
--rw-r--r--   0 gardusig   (501) staff       (20)     3571 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/search_result_task.py
--rw-r--r--   0 gardusig   (501) staff       (20)     3676 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/search_result_task_summary.py
--rw-r--r--   0 gardusig   (501) staff       (20)     3631 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/search_result_workflow.py
--rw-r--r--   0 gardusig   (501) staff       (20)     3736 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/search_result_workflow_summary.py
--rw-r--r--   0 gardusig   (501) staff       (20)     3701 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/skip_task_request.py
--rw-r--r--   0 gardusig   (501) staff       (20)     5630 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/start_workflow.py
--rw-r--r--   0 gardusig   (501) staff       (20)     8587 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/start_workflow_request.py
--rw-r--r--   0 gardusig   (501) staff       (20)     5274 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/sub_workflow_params.py
--rw-r--r--   0 gardusig   (501) staff       (20)    34199 2022-02-15 18:52:42.000000 conductor-python-1.0.8/src/conductor/client/http/models/task.py
--rw-r--r--   0 gardusig   (501) staff       (20)    20768 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/task_def.py
--rw-r--r--   0 gardusig   (501) staff       (20)     4915 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/task_details.py
--rw-r--r--   0 gardusig   (501) staff       (20)     4082 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/task_exec_log.py
--rw-r--r--   0 gardusig   (501) staff       (20)    10845 2022-02-15 13:19:45.000000 conductor-python-1.0.8/src/conductor/client/http/models/task_result.py
--rw-r--r--   0 gardusig   (501) staff       (20)    17247 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/task_summary.py
--rw-r--r--   0 gardusig   (501) staff       (20)    24174 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/workflow.py
--rw-r--r--   0 gardusig   (501) staff       (20)    17716 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/workflow_def.py
--rw-r--r--   0 gardusig   (501) staff       (20)    17359 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/workflow_summary.py
--rw-r--r--   0 gardusig   (501) staff       (20)    26964 2022-02-14 21:06:29.000000 conductor-python-1.0.8/src/conductor/client/http/models/workflow_task.py
--rw-r--r--   0 gardusig   (501) staff       (20)    12701 2022-02-17 19:44:10.000000 conductor-python-1.0.8/src/conductor/client/http/rest.py
-drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-20 21:54:40.209921 conductor-python-1.0.8/src/conductor/client/worker/
--rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-11 17:02:14.000000 conductor-python-1.0.8/src/conductor/client/worker/__init__.py
-drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-20 21:54:40.210759 conductor-python-1.0.8/src/conductor/client/worker/sample/
--rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-20 21:53:45.000000 conductor-python-1.0.8/src/conductor/client/worker/sample/__init__.py
--rw-r--r--   0 gardusig   (501) staff       (20)      267 2022-02-17 19:44:10.000000 conductor-python-1.0.8/src/conductor/client/worker/sample/faulty_execution_worker.py
--rw-r--r--   0 gardusig   (501) staff       (20)      668 2022-02-17 19:44:10.000000 conductor-python-1.0.8/src/conductor/client/worker/sample/simple_python_worker.py
--rw-r--r--   0 gardusig   (501) staff       (20)     1008 2022-02-16 12:44:42.000000 conductor-python-1.0.8/src/conductor/client/worker/worker_interface.py
-drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-20 21:54:40.211462 conductor-python-1.0.8/src/conductor_python.egg-info/
--rw-r--r--   0 gardusig   (501) staff       (20)     9380 2022-02-20 21:54:40.000000 conductor-python-1.0.8/src/conductor_python.egg-info/PKG-INFO
--rw-r--r--   0 gardusig   (501) staff       (20)     2964 2022-02-20 21:54:40.000000 conductor-python-1.0.8/src/conductor_python.egg-info/SOURCES.txt
--rw-r--r--   0 gardusig   (501) staff       (20)        1 2022-02-20 21:54:40.000000 conductor-python-1.0.8/src/conductor_python.egg-info/dependency_links.txt
--rw-r--r--   0 gardusig   (501) staff       (20)       63 2022-02-20 21:54:40.000000 conductor-python-1.0.8/src/conductor_python.egg-info/requires.txt
--rw-r--r--   0 gardusig   (501) staff       (20)       14 2022-02-20 21:54:40.000000 conductor-python-1.0.8/src/conductor_python.egg-info/top_level.txt
-drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-20 21:54:40.211600 conductor-python-1.0.8/src/tst/
--rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-17 19:44:10.000000 conductor-python-1.0.8/src/tst/__init__.py
-drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-20 21:54:40.212200 conductor-python-1.0.8/src/tst/automator/
--rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-17 19:44:10.000000 conductor-python-1.0.8/src/tst/automator/__init__.py
--rw-r--r--   0 gardusig   (501) staff       (20)     1583 2022-02-20 21:08:26.000000 conductor-python-1.0.8/src/tst/automator/test_task_handler.py
--rw-r--r--   0 gardusig   (501) staff       (20)     7192 2022-02-20 21:34:16.000000 conductor-python-1.0.8/src/tst/automator/test_task_runner.py
+drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-22 18:08:40.406465 conductor-python-1.0.9/
+-rw-r--r--   0 gardusig   (501) staff       (20)    11357 2022-02-01 00:57:09.000000 conductor-python-1.0.9/LICENSE
+-rw-r--r--   0 gardusig   (501) staff       (20)     6967 2022-02-22 18:08:40.406587 conductor-python-1.0.9/PKG-INFO
+-rw-r--r--   0 gardusig   (501) staff       (20)     6176 2022-02-22 18:07:56.000000 conductor-python-1.0.9/README.md
+-rw-r--r--   0 gardusig   (501) staff       (20)      104 2022-02-10 12:38:53.000000 conductor-python-1.0.9/pyproject.toml
+-rw-r--r--   0 gardusig   (501) staff       (20)      903 2022-02-22 18:08:40.407022 conductor-python-1.0.9/setup.cfg
+drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-22 18:08:40.392804 conductor-python-1.0.9/src/
+drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-22 18:08:40.394238 conductor-python-1.0.9/src/conductor/
+-rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-11 17:02:14.000000 conductor-python-1.0.9/src/conductor/__init__.py
+drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-22 18:08:40.394448 conductor-python-1.0.9/src/conductor/client/
+-rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-11 17:02:14.000000 conductor-python-1.0.9/src/conductor/client/__init__.py
+-rw-r--r--   0 gardusig   (501) staff       (20)      679 2022-02-22 18:07:56.000000 conductor-python-1.0.9/src/conductor/client/__main__.py
+drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-22 18:08:40.395057 conductor-python-1.0.9/src/conductor/client/automator/
+-rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-11 17:02:14.000000 conductor-python-1.0.9/src/conductor/client/automator/__init__.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     1319 2022-02-22 18:07:56.000000 conductor-python-1.0.9/src/conductor/client/automator/task_handler.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     5596 2022-02-22 18:07:56.000000 conductor-python-1.0.9/src/conductor/client/automator/task_runner.py
+drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-22 18:08:40.395289 conductor-python-1.0.9/src/conductor/client/configuration/
+-rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-14 21:01:31.000000 conductor-python-1.0.9/src/conductor/client/configuration/__init__.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     5146 2022-02-17 19:44:10.000000 conductor-python-1.0.9/src/conductor/client/configuration/configuration.py
+drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-22 18:08:40.396068 conductor-python-1.0.9/src/conductor/client/http/
+-rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-11 17:02:14.000000 conductor-python-1.0.9/src/conductor/client/http/__init__.py
+drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-22 18:08:40.398119 conductor-python-1.0.9/src/conductor/client/http/api/
+-rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-11 17:02:14.000000 conductor-python-1.0.9/src/conductor/client/http/api/__init__.py
+-rw-r--r--   0 gardusig   (501) staff       (20)    17824 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/api/admin_resource_api.py
+-rw-r--r--   0 gardusig   (501) staff       (20)    17638 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/api/event_resource_api.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     3444 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/api/health_check_resource_api.py
+-rw-r--r--   0 gardusig   (501) staff       (20)    34631 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/api/metadata_resource_api.py
+-rw-r--r--   0 gardusig   (501) staff       (20)    16605 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/api/queue_admin_resource_api.py
+-rw-r--r--   0 gardusig   (501) staff       (20)    55041 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/api/task_resource_api.py
+-rw-r--r--   0 gardusig   (501) staff       (20)    18978 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/api/workflow_bulk_resource_api.py
+-rw-r--r--   0 gardusig   (501) staff       (20)    84613 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/api/workflow_resource_api.py
+-rw-r--r--   0 gardusig   (501) staff       (20)    24092 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/api_client.py
+drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-22 18:08:40.404569 conductor-python-1.0.9/src/conductor/client/http/models/
+-rw-r--r--   0 gardusig   (501) staff       (20)     1863 2022-02-11 17:02:14.000000 conductor-python-1.0.9/src/conductor/client/http/models/__init__.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     6095 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/action.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     4030 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/bulk_response.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     6333 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/event_handler.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     3435 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/external_storage_location.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     4148 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/health.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     4714 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/health_check_status.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     4853 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/poll_data.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     6519 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/rerun_workflow_request.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     3571 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/search_result_task.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     3676 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/search_result_task_summary.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     3631 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/search_result_workflow.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     3736 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/search_result_workflow_summary.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     3701 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/skip_task_request.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     5630 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/start_workflow.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     8587 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/start_workflow_request.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     5274 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/sub_workflow_params.py
+-rw-r--r--   0 gardusig   (501) staff       (20)    34199 2022-02-15 18:52:42.000000 conductor-python-1.0.9/src/conductor/client/http/models/task.py
+-rw-r--r--   0 gardusig   (501) staff       (20)    20768 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/task_def.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     4915 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/task_details.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     4082 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/task_exec_log.py
+-rw-r--r--   0 gardusig   (501) staff       (20)    10845 2022-02-15 13:19:45.000000 conductor-python-1.0.9/src/conductor/client/http/models/task_result.py
+-rw-r--r--   0 gardusig   (501) staff       (20)    17247 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/task_summary.py
+-rw-r--r--   0 gardusig   (501) staff       (20)    24174 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/workflow.py
+-rw-r--r--   0 gardusig   (501) staff       (20)    17716 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/workflow_def.py
+-rw-r--r--   0 gardusig   (501) staff       (20)    17359 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/workflow_summary.py
+-rw-r--r--   0 gardusig   (501) staff       (20)    26964 2022-02-14 21:06:29.000000 conductor-python-1.0.9/src/conductor/client/http/models/workflow_task.py
+-rw-r--r--   0 gardusig   (501) staff       (20)    12701 2022-02-17 19:44:10.000000 conductor-python-1.0.9/src/conductor/client/http/rest.py
+drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-22 18:08:40.404883 conductor-python-1.0.9/src/conductor/client/worker/
+-rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-11 17:02:14.000000 conductor-python-1.0.9/src/conductor/client/worker/__init__.py
+drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-22 18:08:40.405248 conductor-python-1.0.9/src/conductor/client/worker/sample/
+-rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-21 02:10:25.000000 conductor-python-1.0.9/src/conductor/client/worker/sample/__init__.py
+-rw-r--r--   0 gardusig   (501) staff       (20)      190 2022-02-22 18:07:56.000000 conductor-python-1.0.9/src/conductor/client/worker/sample/faulty_execution_worker.py
+-rw-r--r--   0 gardusig   (501) staff       (20)      322 2022-02-22 18:07:56.000000 conductor-python-1.0.9/src/conductor/client/worker/sample/simple_python_worker.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     1647 2022-02-22 18:07:56.000000 conductor-python-1.0.9/src/conductor/client/worker/worker_interface.py
+drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-22 18:08:40.405819 conductor-python-1.0.9/src/conductor_python.egg-info/
+-rw-r--r--   0 gardusig   (501) staff       (20)     6967 2022-02-22 18:08:40.000000 conductor-python-1.0.9/src/conductor_python.egg-info/PKG-INFO
+-rw-r--r--   0 gardusig   (501) staff       (20)     2964 2022-02-22 18:08:40.000000 conductor-python-1.0.9/src/conductor_python.egg-info/SOURCES.txt
+-rw-r--r--   0 gardusig   (501) staff       (20)        1 2022-02-22 18:08:40.000000 conductor-python-1.0.9/src/conductor_python.egg-info/dependency_links.txt
+-rw-r--r--   0 gardusig   (501) staff       (20)       63 2022-02-22 18:08:40.000000 conductor-python-1.0.9/src/conductor_python.egg-info/requires.txt
+-rw-r--r--   0 gardusig   (501) staff       (20)       14 2022-02-22 18:08:40.000000 conductor-python-1.0.9/src/conductor_python.egg-info/top_level.txt
+drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-22 18:08:40.405926 conductor-python-1.0.9/src/tst/
+-rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-17 19:44:10.000000 conductor-python-1.0.9/src/tst/__init__.py
+drwxr-xr-x   0 gardusig   (501) staff       (20)        0 2022-02-22 18:08:40.406274 conductor-python-1.0.9/src/tst/automator/
+-rw-r--r--   0 gardusig   (501) staff       (20)        0 2022-02-17 19:44:10.000000 conductor-python-1.0.9/src/tst/automator/__init__.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     1589 2022-02-22 18:07:56.000000 conductor-python-1.0.9/src/tst/automator/test_task_handler.py
+-rw-r--r--   0 gardusig   (501) staff       (20)     7293 2022-02-22 18:07:56.000000 conductor-python-1.0.9/src/tst/automator/test_task_runner.py
```

### Comparing `conductor-python-1.0.8/LICENSE` & `conductor-python-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/README.md` & `conductor-python-1.0.9/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,263 +1,157 @@
 # Conductor Python
 
 Software Development Kit for Netflix Conductor, written on and providing support for Python.
 
 ## Quick Guide
 
-In case you have already set up Conductor and got it running, you can quickly onboard to it with these steps:
-1. Install Conductor Python SDK from pypi:
+1. Create a virtual environment
     ```shell
-    $ python3 -m pip install conductor-python
+    $ virtualenv conductor
+    $ source conductor/bin/activate
+    $ python3 -m pip list
+    Package    Version
+    ---------- -------
+    pip        22.0.3
+    setuptools 60.6.0
+    wheel      0.37.1
     ```
-2. Run Conductor Python SDK:
+1. Install latest version of `conductor-python` from pypi
     ```shell
-    $ python3 -m conductor.client
+    $ python3 -m pip install conductor-python
+    Collecting conductor-python
+    Collecting certifi>=14.05.14
+    Collecting urllib3>=1.15.1
+    Requirement already satisfied: setuptools>=21.0.0 in ./conductor/lib/python3.8/site-packages (from conductor-python) (60.6.0)
+    Collecting six>=1.10
+    Installing collected packages: certifi, urllib3, six, conductor-python
+    Successfully installed certifi-2021.10.8 conductor-python-1.0.7 six-1.16.0 urllib3-1.26.8
     ```
+2. Create a worker capable of executing a `Task`. Example:
+    ```python
+    from conductor.client.worker.worker_interface import WorkerInterface
 
-### Custom worker
 
-In order to:
-* Create a custom python worker, it should inherit from `WorkerInterface` and implement the execution method. Example:
-  ```python
-  from conductor.client.http.models.task_result import TaskResult
-  from conductor.client.worker.worker_interface import WorkerInterface
-
-
-  class SimplePythonWorker(WorkerInterface):
-      def __init__(self):
-          super().__init__('simple_python_worker')
-
-      def execute(self, task):
-          task_result = TaskResult(
-              task_id=task.task_id,
-              workflow_instance_id=task.workflow_instance_id,
-              worker_id=self.get_task_definition_name()
-          )
-          self.__execute(task_result)
-          task_result.status = 'COMPLETED'
-          return task_result
-
-      def __execute(self, task_result):
-          task_result.add_output_data('key', 'value')
-  ```
-* Run, you should create a main method to instantiate a `TaskHandler` object with your implemented workers. Example:
+    class SimplePythonWorker(WorkerInterface):
+        def execute(self, task):
+            task_result = self.get_task_result_from_task(task)
+            task_result.add_output_data('key', 'value')
+            task_result.status = 'COMPLETED'
+            return task_result
+    ```
+    * The `add_output_data` is the most relevant part, since you can store information in a dictionary, which will be sent within `TaskResult` as your execution response to Conductor
+3. Create a main method to start polling tasks to execute with your worker. Example:
     ```python
     from conductor.client.automator.task_handler import TaskHandler
     from conductor.client.configuration.configuration import Configuration
+    from conductor.client.worker.sample.faulty_execution_worker import FaultyExecutionWorker
     from conductor.client.worker.sample.simple_python_worker import SimplePythonWorker
-    import logging
-
-    logger = logging.getLogger(
-        Configuration.get_logging_formatted_name(
-            __name__
-        )
-    )
 
 
     def main():
-        configuration = Configuration(
-            debug=True
-        )
-        configuration.apply_logging_config()
-        workers = [SimplePythonWorker()] * 3
-        logger.debug(f'Created workers: {workers}')
-        with TaskHandler(configuration, workers) as task_handler:
-            logger.debug(f'Created task_handler: {task_handler}')
+        configuration = Configuration(debug=True)
+        task_definition_name = 'python_example_task'
+        workers = [
+            SimplePythonWorker(task_definition_name),
+            FaultyExecutionWorker(task_definition_name)
+        ]
+        with TaskHandler(workers, configuration) as task_handler:
             task_handler.start()
 
 
     if __name__ == '__main__':
         main()
     ```
-
-## Full installation guide
-
-### Set up Conductor
-
-1. Clone Netflix Conductor repository: https://github.com/Netflix/conductor
-    ```shell
-    $ git clone https://github.com/Netflix/conductor.git
-    ```
-2. Start Conductor server by running this command at the repo root folder (`/conductor`):
-    ```shell
-    $ ./gradlew bootRun
-    ```
-3. Start Conductor UI by running this command at the UI folder (`/conductor/ui`):
-    ```shell
-    $ yarn install
-    $ yarn run start
-    ```
-
-You should be able to access:
-* Conductor API:
-  * http://localhost:8080/swagger-ui/index.html
-* Conductor UI:
-  * http://localhost:5000
-
-### Run
-
-#### Create new task
-
-You need to define a *Task* within *Conductor* that your `Python Worker` is capable of running.
-
-Make a POST request to `/metadata/taskdefs` endpoint at your conductor server.
-* URL example: `http://localhost:8080/api/metadata/taskdefs`
-* Task Definition example:
-    ```json
-    [
-      {
-        "name": "simple_python_worker",
-        "description": "Simple Python Worker",
-        "retryCount": 3,
-        "retryLogic": "FIXED",
-        "retryDelaySeconds": 10,
-        "timeoutSeconds": 300,
-        "timeoutPolicy": "TIME_OUT_WF",
-        "responseTimeoutSeconds": 180,
-        "ownerEmail": "example@example.com"
-      }
-    ]
-    ```
-* Command example:
+    * This example contains two workers, each with a different execution method, capable of running the same `task_definition_name`
+4. Now that you have implemented the example, you can start the Conductor server locally:
+      1. Clone [Netflix Conductor repository](https://github.com/Netflix/conductor):
+          ```shell
+          $ git clone https://github.com/Netflix/conductor.git
+          $ cd conductor/
+          ```
+      2. Start the Conductor server:
+          ```shell
+          /conductor$ ./gradlew bootRun
+          ```
+      3. Start Conductor UI:
+          ```shell
+          /conductor$ cd ui/
+          /conductor/ui$ yarn install
+          /conductor/ui$ yarn run start
+          ```
+      You should be able to access:
+      * Conductor API:
+        * http://localhost:8080/swagger-ui/index.html
+      * Conductor UI:
+        * http://localhost:5000
+5. Create a `Task` within `Conductor`. Example:
     ```shell
     $ curl -X 'POST' \
         'http://localhost:8080/api/metadata/taskdefs' \
         -H 'accept: */*' \
         -H 'Content-Type: application/json' \
         -d '[
         {
-          "name": "simple_python_worker",
-          "description": "Simple Python Worker",
+          "name": "python_task_example",
+          "description": "Python task example",
           "retryCount": 3,
           "retryLogic": "FIXED",
           "retryDelaySeconds": 10,
           "timeoutSeconds": 300,
           "timeoutPolicy": "TIME_OUT_WF",
           "responseTimeoutSeconds": 180,
           "ownerEmail": "example@example.com"
         }
       ]'
     ```
-
-#### Create new workflow
-
-You need to define a *Workflow* within *Conductor* that contains the *Task* you had just defined.
-
-Make a POST request to `/metadata/workflow` endpoint at your conductor server.
-* URL example: `http://localhost:8080/api/metadata/workflow`
-* Workflow Definition example:
-    ```json
-    {
-      "createTime": 1634021619147,
-      "updateTime": 1630694890267,
-      "name": "simple_workflow_with_python_worker",
-      "description": "Simple Workflow with Python Worker",
-      "version": 1,
-      "tasks": [
-        {
-          "name": "simple_python_worker",
-          "taskReferenceName": "simple_python_worker_ref_1",
-          "inputParameters": {},
-          "type": "SIMPLE"
-        }
-      ],
-      "inputParameters": [],
-      "outputParameters": {
-        "workerOutput": "${simple_python_worker_ref_1.output}"
-      },
-      "schemaVersion": 2,
-      "restartable": true,
-      "ownerEmail": "example@example.com",
-      "timeoutPolicy": "ALERT_ONLY",
-      "timeoutSeconds": 0
-    }
-    ```
-* Command example:
+6. Create a `Workerflow` within `Conductor`. Example:
     ```shell
     $ curl -X 'POST' \
         'http://localhost:8080/api/metadata/workflow' \
         -H 'accept: */*' \
         -H 'Content-Type: application/json' \
         -d '{
         "createTime": 1634021619147,
         "updateTime": 1630694890267,
-        "name": "simple_workflow_with_python_worker",
-        "description": "Simple Workflow with Python Worker",
+        "name": "workflow_with_python_task_example",
+        "description": "Workflow with Python Task example",
         "version": 1,
         "tasks": [
           {
-            "name": "simple_python_worker",
-            "taskReferenceName": "simple_python_worker_ref_1",
+            "name": "python_task_example",
+            "taskReferenceName": "python_task_example_ref_1",
             "inputParameters": {},
             "type": "SIMPLE"
           }
         ],
         "inputParameters": [],
         "outputParameters": {
-          "workerOutput": "${simple_python_worker_ref_1.output}"
+          "workerOutput": "${python_task_example_ref_1.output}"
         },
         "schemaVersion": 2,
         "restartable": true,
         "ownerEmail": "example@example.com",
         "timeoutPolicy": "ALERT_ONLY",
         "timeoutSeconds": 0
       }'
     ```
-
-#### Start new workflow
-
-Now that you have defined a *Task* and a *Workflow* within *Conductor*, you should be able to run it.
-
-Make a POST request to `/workflow/{name}` endpoint at your conductor server.
-* URL example: `http://localhost:8080/api/workflow/simple_workflow_with_python_worker`
-  * Priority should be empty
-  * Request body should be empty, like: `{}`
-* Command example:
+1. Start a new workflow:
     ```shell
     $ curl -X 'POST' \
-        'http://localhost:8080/api/workflow/simple_workflow_with_python_worker' \
+        'http://localhost:8080/api/workflow/workflow_with_python_task_example' \
         -H 'accept: text/plain' \
         -H 'Content-Type: application/json' \
         -d '{}'
     ```
-* Create a bunch of workflows:
-    ```shell
-    $ export CREATE_WORKFLOW_SHORTCUT="curl -X 'POST' \
-        'http://localhost:8080/api/workflow/simple_workflow_with_python_worker' \
-        -H 'accept: text/plain' \
-        -H 'Content-Type: application/json' \
-        -d '{}' \
-        -s"
+    You should receive a *Workflow ID* at the *Response body*
+    * *Workflow ID* example: `8ff0bc06-4413-4c94-b27a-b3210412a914`
     
-    $ for idx in {1..100}; do \
-        echo "Creating workflow ${idx}"; \
-        workflow_id=$(eval "${CREATE_WORKFLOW_SHORTCUT}"); \
-        echo "workflow_id=${workflow_id}"; \
-      done
-    ```
-    * Expected output example:
-        ```shell
-        Creating workflow 1
-        workflow_id=6dd2c86b-5ce6-487a-9a65-632139da1345
-        Creating workflow 2
-        workflow_id=b0ddfdcf-0c4a-4fd3-892c-97fc38c46d63
-        ...
-        ```
-
-You should receive a *Workflow ID* at the *Response body*
-* *Workflow ID* example: `8ff0bc06-4413-4c94-b27a-b3210412a914`
-
-#### See workflow execution
-
-Now you must be able to see its execution through the UI.
-* URL: 
-  * prefix: `http://localhost:5001/execution`
-  * suffix: `${workflow_id}`
-* Example: `http://localhost:5001/execution/8ff0bc06-4413-4c94-b27a-b3210412a914`
+    Now you must be able to see its execution through the UI.
+    * Example: `http://localhost:5000/execution/8ff0bc06-4413-4c94-b27a-b3210412a914`
+1. Run your Python file with the `main` method
 
 ### Unit Tests
 
 #### Simple validation
 
 ```shell
 /conductor-python/src$ python3 -m unittest -v
```

### Comparing `conductor-python-1.0.8/setup.cfg` & `conductor-python-1.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = conductor-python
-version = 1.0.8
+version = 1.0.9
 author = Gustavo Gardusi
 author_email = gustavo.gardusi@gmail.com
 description = Netflix Conductor Python SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/conductor-sdk/conductor-python
 classifiers =
```

### Comparing `conductor-python-1.0.8/src/conductor/client/__main__.py` & `conductor-python-1.0.9/src/conductor/client/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 from conductor.client.automator.task_handler import TaskHandler
 from conductor.client.configuration.configuration import Configuration
+from conductor.client.worker.sample.faulty_execution_worker import FaultyExecutionWorker
 from conductor.client.worker.sample.simple_python_worker import SimplePythonWorker
-import logging
-
-logger = logging.getLogger(
-    Configuration.get_logging_formatted_name(
-        __name__
-    )
-)
 
 
 def main():
-    configuration = Configuration(
-        debug=True
-    )
-    configuration.apply_logging_config()
-    workers = [SimplePythonWorker()] * 3
-    logger.debug(f'Created workers: {workers}')
-    with TaskHandler(configuration, workers) as task_handler:
-        logger.debug(f'Created task_handler: {task_handler}')
+    configuration = Configuration(debug=True)
+    task_definition_name = 'python_task_definition_name'
+    workers = [
+        SimplePythonWorker(task_definition_name),
+        FaultyExecutionWorker(task_definition_name)
+    ]
+    with TaskHandler(workers, configuration) as task_handler:
         task_handler.start()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `conductor-python-1.0.8/src/conductor/client/automator/task_runner.py` & `conductor-python-1.0.9/src/conductor/client/automator/task_runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,58 +11,54 @@
     Configuration.get_logging_formatted_name(
         __name__
     )
 )
 
 
 class TaskRunner:
-    def __init__(self, configuration, worker):
-        if not isinstance(configuration, Configuration):
+    def __init__(self, worker: WorkerInterface, configuration: Configuration = None):
+        if configuration != None and not isinstance(configuration, Configuration):
             raise Exception('Invalid configuration')
         if not isinstance(worker, WorkerInterface):
             raise Exception('Invalid worker')
         self.configuration = configuration
         self.worker = worker
 
-    def run(self):
-        self.configuration.apply_logging_config()
+    def run(self) -> None:
+        if self.configuration != None:
+            self.configuration.apply_logging_config()
         while True:
             self.run_once()
 
-    def run_once(self):
+    def run_once(self) -> None:
         task = self.__poll_task()
         if task != None:
             task_result = self.__execute_task(task)
             self.__update_task(task_result)
         self.__wait_for_polling_interval()
 
-    def __poll_task(self):
+    def __poll_task(self) -> Task:
         task_definition_name = self.worker.get_task_definition_name()
         logger.info(f'Polling task for: {task_definition_name}')
-        task_resource_api = TaskResourceApi(
-            ApiClient(
-                configuration=self.configuration
-            )
-        )
         try:
-            task = task_resource_api.poll(
+            task = self.__get_task_resource_api().poll(
                 tasktype=task_definition_name
             )
         except Exception:
             return None
         message = 'Polled task for worker: {task_definition_name}, identity: {identity}'
         logger.debug(
             message.format(
                 task_definition_name=task_definition_name,
                 identity=self.worker.get_identity()
             )
         )
         return task
 
-    def __execute_task(self, task):
+    def __execute_task(self, task: Task) -> TaskResult:
         if not isinstance(task, Task):
             return None
         logger.info(
             'Executing task, id: {task_id}, workflow_instance_id: {workflow_instance_id}, worker: {worker_name}'.format(
                 task_id=task.task_id,
                 workflow_instance_id=task.workflow_instance_id,
                 worker_name=self.worker.get_task_definition_name()
@@ -91,31 +87,26 @@
                     workflow_instance_id=task.workflow_instance_id,
                     worker_name=self.worker.get_task_definition_name(),
                     reason=str(e)
                 )
             )
         return task_result
 
-    def __update_task(self, task_result):
+    def __update_task(self, task_result: TaskResult):
         if not isinstance(task_result, TaskResult):
             return None
         logger.debug(
             'Updating task, id: {task_id}, workflow_instance_id: {workflow_instance_id}, worker: {worker_name}'.format(
                 task_id=task_result.task_id,
                 workflow_instance_id=task_result.workflow_instance_id,
                 worker_name=self.worker.get_task_definition_name()
             )
         )
-        task_resource_api = TaskResourceApi(
-            ApiClient(
-                configuration=self.configuration
-            )
-        )
         try:
-            response = task_resource_api.update_task(
+            response = self.__get_task_resource_api().update_task(
                 body=task_result
             )
         except Exception as e:
             logger.warning(
                 'Failed to update task, id: {task_id}, workflow_instance_id: {workflow_instance_id}, worker: {worker_name}, reason: {reason}'.format(
                     task_id=task_result.task_id,
                     workflow_instance_id=task_result.workflow_instance_id,
@@ -130,11 +121,18 @@
                 workflow_instance_id=task_result.workflow_instance_id,
                 worker_name=self.worker.get_task_definition_name(),
                 response=str(response)
             )
         )
         return response
 
-    def __wait_for_polling_interval(self):
+    def __wait_for_polling_interval(self) -> None:
         polling_interval = self.worker.get_polling_interval_in_seconds()
         logger.debug(f'Sleep for {polling_interval} seconds')
         time.sleep(polling_interval)
+
+    def __get_task_resource_api(self) -> TaskResourceApi:
+        return TaskResourceApi(
+            ApiClient(
+                configuration=self.configuration
+            )
+        )
```

### Comparing `conductor-python-1.0.8/src/conductor/client/configuration/configuration.py` & `conductor-python-1.0.9/src/conductor/client/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/api/admin_resource_api.py` & `conductor-python-1.0.9/src/conductor/client/http/api/admin_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/api/event_resource_api.py` & `conductor-python-1.0.9/src/conductor/client/http/api/event_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/api/health_check_resource_api.py` & `conductor-python-1.0.9/src/conductor/client/http/api/health_check_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/api/metadata_resource_api.py` & `conductor-python-1.0.9/src/conductor/client/http/api/metadata_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/api/queue_admin_resource_api.py` & `conductor-python-1.0.9/src/conductor/client/http/api/queue_admin_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/api/task_resource_api.py` & `conductor-python-1.0.9/src/conductor/client/http/api/task_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/api/workflow_bulk_resource_api.py` & `conductor-python-1.0.9/src/conductor/client/http/api/workflow_bulk_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/api/workflow_resource_api.py` & `conductor-python-1.0.9/src/conductor/client/http/api/workflow_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/api_client.py` & `conductor-python-1.0.9/src/conductor/client/http/api_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/__init__.py` & `conductor-python-1.0.9/src/conductor/client/http/models/__init__.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/action.py` & `conductor-python-1.0.9/src/conductor/client/http/models/action.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/bulk_response.py` & `conductor-python-1.0.9/src/conductor/client/http/models/bulk_response.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/event_handler.py` & `conductor-python-1.0.9/src/conductor/client/http/models/event_handler.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/external_storage_location.py` & `conductor-python-1.0.9/src/conductor/client/http/models/external_storage_location.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/health.py` & `conductor-python-1.0.9/src/conductor/client/http/models/health.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/health_check_status.py` & `conductor-python-1.0.9/src/conductor/client/http/models/health_check_status.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/poll_data.py` & `conductor-python-1.0.9/src/conductor/client/http/models/poll_data.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/rerun_workflow_request.py` & `conductor-python-1.0.9/src/conductor/client/http/models/rerun_workflow_request.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/search_result_task.py` & `conductor-python-1.0.9/src/conductor/client/http/models/search_result_task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/search_result_task_summary.py` & `conductor-python-1.0.9/src/conductor/client/http/models/search_result_task_summary.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/search_result_workflow.py` & `conductor-python-1.0.9/src/conductor/client/http/models/search_result_workflow.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/search_result_workflow_summary.py` & `conductor-python-1.0.9/src/conductor/client/http/models/search_result_workflow_summary.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/skip_task_request.py` & `conductor-python-1.0.9/src/conductor/client/http/models/skip_task_request.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/start_workflow.py` & `conductor-python-1.0.9/src/conductor/client/http/models/start_workflow.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/start_workflow_request.py` & `conductor-python-1.0.9/src/conductor/client/http/models/start_workflow_request.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/sub_workflow_params.py` & `conductor-python-1.0.9/src/conductor/client/http/models/sub_workflow_params.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/task.py` & `conductor-python-1.0.9/src/conductor/client/http/models/task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/task_def.py` & `conductor-python-1.0.9/src/conductor/client/http/models/task_def.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/task_details.py` & `conductor-python-1.0.9/src/conductor/client/http/models/task_details.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/task_exec_log.py` & `conductor-python-1.0.9/src/conductor/client/http/models/task_exec_log.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/task_result.py` & `conductor-python-1.0.9/src/conductor/client/http/models/task_result.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/task_summary.py` & `conductor-python-1.0.9/src/conductor/client/http/models/task_summary.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/workflow.py` & `conductor-python-1.0.9/src/conductor/client/http/models/workflow.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/workflow_def.py` & `conductor-python-1.0.9/src/conductor/client/http/models/workflow_def.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/workflow_summary.py` & `conductor-python-1.0.9/src/conductor/client/http/models/workflow_summary.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/models/workflow_task.py` & `conductor-python-1.0.9/src/conductor/client/http/models/workflow_task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor/client/http/rest.py` & `conductor-python-1.0.9/src/conductor/client/http/rest.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/conductor_python.egg-info/SOURCES.txt` & `conductor-python-1.0.9/src/conductor_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conductor-python-1.0.8/src/tst/automator/test_task_handler.py` & `conductor-python-1.0.9/src/tst/automator/test_task_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,9 +38,9 @@
                     self.assertTrue(
                         isinstance(process, multiprocessing.Process)
                     )
 
     def __get_valid_task_handler(self):
         return TaskHandler(
             configuration=Configuration(),
-            workers=[SimplePythonWorker()]
+            workers=[SimplePythonWorker('task')]
         )
```

### Comparing `conductor-python-1.0.8/src/tst/automator/test_task_runner.py` & `conductor-python-1.0.9/src/tst/automator/test_task_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,29 +23,29 @@
         logging.disable(logging.NOTSET)
 
     def test_initialization_with_invalid_configuration(self):
         expected_exception = Exception('Invalid configuration')
         with self.assertRaises(Exception) as context:
             TaskRunner(
                 configuration=None,
-                worker=SimplePythonWorker()
+                worker=self.__get_valid_worker()
             )
             self.assertEqual(expected_exception, context.exception)
 
     def test_initialization_with_invalid_worker(self):
         expected_exception = Exception('Invalid worker')
         with self.assertRaises(Exception) as context:
             TaskRunner(
                 configuration=Configuration(),
                 worker=None
             )
             self.assertEqual(expected_exception, context.exception)
 
     def test_run_once(self):
-        expected_time = SimplePythonWorker().get_polling_interval_in_seconds()
+        expected_time = self.__get_valid_worker().get_polling_interval_in_seconds()
         with patch.object(
             TaskResourceApi,
             'poll',
             return_value=self.__get_valid_task()
         ):
             with patch.object(
                 TaskResourceApi,
@@ -83,15 +83,15 @@
 
     def test_execute_task_with_invalid_task(self):
         task_runner = self.__get_valid_task_runner()
         task_result = task_runner._TaskRunner__execute_task(None)
         self.assertEqual(task_result, None)
 
     def test_execute_task_with_faulty_execution_worker(self):
-        worker = FaultyExecutionWorker()
+        worker = FaultyExecutionWorker('task')
         expected_task_result = TaskResult(
             task_id=self.TASK_ID,
             workflow_instance_id=self.WORKFLOW_INSTANCE_ID,
             worker_id=worker.get_task_definition_name(),
             status='FAILED',
             reason_for_incompletion='faulty execution'
         )
@@ -101,15 +101,15 @@
         )
         task = self.__get_valid_task()
         task_result = task_runner._TaskRunner__execute_task(task)
         self.assertEqual(task_result, expected_task_result)
 
     def test_execute_task(self):
         expected_task_result = self.__get_valid_task_result()
-        worker = SimplePythonWorker()
+        worker = self.__get_valid_worker()
         task_runner = TaskRunner(
             configuration=Configuration(),
             worker=worker
         )
         task = self.__get_valid_task()
         task_result = task_runner._TaskRunner__execute_task(task)
         self.assertEqual(task_result, expected_task_result)
@@ -155,37 +155,40 @@
         ):
             task_runner = self.__get_valid_task_runner()
             with self.assertRaises(Exception) as context:
                 task_runner._TaskRunner__wait_for_polling_interval()
                 self.assertEqual(expected_exception, context.exception)
 
     def test_wait_for_polling_interval(self):
-        expected_time = SimplePythonWorker().get_polling_interval_in_seconds()
+        expected_time = self.__get_valid_worker().get_polling_interval_in_seconds()
         task_runner = self.__get_valid_task_runner()
         start_time = time.time()
         task_runner._TaskRunner__wait_for_polling_interval()
         finish_time = time.time()
         spent_time = finish_time - start_time
         self.assertGreater(spent_time, expected_time)
 
     def __get_valid_task_runner(self):
         return TaskRunner(
             configuration=Configuration(),
-            worker=SimplePythonWorker()
+            worker=self.__get_valid_worker()
         )
 
     def __get_valid_task(self):
         return Task(
             task_id=self.TASK_ID,
             workflow_instance_id=self.WORKFLOW_INSTANCE_ID
         )
 
     def __get_valid_task_result(self):
         return TaskResult(
             task_id=self.TASK_ID,
             workflow_instance_id=self.WORKFLOW_INSTANCE_ID,
-            worker_id=SimplePythonWorker().get_task_definition_name(),
+            worker_id=self.__get_valid_worker().get_identity(),
             status='COMPLETED',
             output_data={
                 'key': 'value'
             }
         )
+
+    def __get_valid_worker(self):
+        return SimplePythonWorker('task')
```

