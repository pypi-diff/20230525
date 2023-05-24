# Comparing `tmp/kedro-graphql-0.2.0.tar.gz` & `tmp/kedro-graphql-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-graphql-0.2.0.tar", last modified: Mon May 22 20:49:53 2023, max compression
+gzip compressed data, was "kedro-graphql-0.3.0.tar", last modified: Wed May 24 22:27:35 2023, max compression
```

## Comparing `kedro-graphql-0.2.0.tar` & `kedro-graphql-0.3.0.tar`

### file list

```diff
@@ -1,60 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 20:49:53.108714 kedro-graphql-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.100714 kedro-graphql-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/kedro_graphql/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/kedro_graphql/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/backends/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/celeryapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/celeryconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/kedro_graphql/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/example/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/pipeline_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/kedro_graphql/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/kedro_graphql/pipelines/example00/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/pipelines/example00/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/pipelines/example00/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/pipelines/example00/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/kedro_graphql/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/plugins/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/kedro_graphql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-05-22 20:49:53.000000 kedro-graphql-0.2.0/src/kedro_graphql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-22 20:49:53.000000 kedro-graphql-0.2.0/src/kedro_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:49:53.000000 kedro-graphql-0.2.0/src/kedro_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-22 20:49:53.000000 kedro-graphql-0.2.0/src/kedro_graphql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-22 20:49:53.000000 kedro-graphql-0.2.0/src/kedro_graphql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 20:49:53.000000 kedro-graphql-0.2.0/src/kedro_graphql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/tests/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/tests/pipelines/example00/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/pipelines/example00/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/pipelines/example00/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/test_schema_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/test_schema_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/test_schema_subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.413492 kedro-graphql-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-05-24 22:27:35.413492 kedro-graphql-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-24 22:27:35.413492 kedro-graphql-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.397492 kedro-graphql-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.401492 kedro-graphql-0.3.0/src/kedro_graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.405492 kedro-graphql-0.3.0/src/kedro_graphql/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/backends/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/celeryapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/celeryconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.405492 kedro-graphql-0.3.0/src/kedro_graphql/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/example/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.405492 kedro-graphql-0.3.0/src/kedro_graphql/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/logs/json_log_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/logs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/pipeline_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.409492 kedro-graphql-0.3.0/src/kedro_graphql/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.409492 kedro-graphql-0.3.0/src/kedro_graphql/pipelines/example00/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/pipelines/example00/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/pipelines/example00/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/pipelines/example00/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.409492 kedro-graphql-0.3.0/src/kedro_graphql/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/plugins/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.405492 kedro-graphql-0.3.0/src/kedro_graphql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-05-24 22:27:35.000000 kedro-graphql-0.3.0/src/kedro_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-24 22:27:35.000000 kedro-graphql-0.3.0/src/kedro_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:27:35.000000 kedro-graphql-0.3.0/src/kedro_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-24 22:27:35.000000 kedro-graphql-0.3.0/src/kedro_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-24 22:27:35.000000 kedro-graphql-0.3.0/src/kedro_graphql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 22:27:35.000000 kedro-graphql-0.3.0/src/kedro_graphql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.409492 kedro-graphql-0.3.0/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.413492 kedro-graphql-0.3.0/src/tests/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.413492 kedro-graphql-0.3.0/src/tests/pipelines/example00/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/pipelines/example00/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/pipelines/example00/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/test_schema_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/test_schema_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/test_schema_subscription.py
```

### Comparing `kedro-graphql-0.2.0/LICENSE.txt` & `kedro-graphql-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.2.0/PKG-INFO` & `kedro-graphql-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-graphql
-Version: 0.2.0
+Version: 0.3.0
 Summary: Kedro helps you build production-ready data and analytics pipelines
 Author: opensean
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://github.com/opensean/kedro-graphql
 Project-URL: Source, https://github.com/opensean/kedro-graphql
 Keywords: pipelines,machine learning,data pipelines,data science,data engineering
 Classifier: Programming Language :: Python :: 3.10
@@ -20,16 +20,15 @@
 for serving kedro projects as a graphql api.  It leverages 
 [Strawberry](https://strawberry.rocks/), [FastAPI](https://fastapi.tiangolo.com/), 
 and [Celery](https://docs.celeryq.dev/en/stable/index.html) to turn any 
  [Kedro](https://docs.kedro.org/en/stable/) project into a GraphqlQL api 
  with features such as:
  
  - a distributed task queue
- - events
-   - subscribe to pipeline events (status updates) via GraphQL subscriptions 
+ - subscribe to pipline events and logs via GraphQL subscriptions
  - storage
    - persist and track all pipelines executed via the API
  - [additional features](#features)
 
 ```mermaid
 flowchart  TB
   api[GraphQL API\n<i>strawberry + FastAPI</i>]
@@ -140,14 +139,17 @@
 ```
 
 Start a worker (in another terminal).
 
 ```
 kedro gql -w
 ```
+
+### Start a pipeline
+
 Navigate to http://127.0.0.1:5000/graphql to access the graphql interface 
 and execute the following mutation:
 
 ```
 mutation MyMutation {
   pipeline(
     pipeline: {name: "example00", parameters: [{name: "example", value: "hello"}, {name: "duration", value: "10"}], inputs: {name: "text_in", type: "text.TextDataSet", filepath: "./data/01_raw/text_in.txt"}, outputs: {name: "text_out", type: "text.TextDataSet", filepath: "./data/02_intermediate/text_out.txt"}}
@@ -167,14 +169,16 @@
       "id": "6463991db98d7f8564ab15a0",
       "name": "example00"
     }
   }
 }
 ```
 
+### Subscribe to pipeline events
+
 Now execute the following subscription to track the progress:
 
 ```
 subscription MySubscription {
   pipeline(id: "6463991db98d7f8564ab15a0") {
     id
     result
@@ -184,14 +188,37 @@
     traceback
   }
 }
 ```
 
 ![subscription](docs/subscription.gif)
 
+
+### Susbscribe to pipeline logs
+
+Execute the following subscription to recieve log messages:
+
+
+```
+subscription {
+   	pipelineLogs(id:"6463991db98d7f8564ab15a0") {
+       id
+       message
+       messageId
+       taskId
+       time
+     }
+}
+```
+
+
+![logs subscription](docs/logs-subscription.gif)
+
+### Get the pipeline result
+
 Fetch the pipeline result with the following query:
 
 ```
 query MyQuery {
   pipeline(id: "6463991db98d7f8564ab15a0") {
     describe
     id
@@ -339,19 +366,19 @@
 
 
 This example adds a [CORSMiddleware](https://fastapi.tiangolo.com/tutorial/cors/#use-corsmiddleware).
 
 ```
 ## src/kedro_graphql/example/app.py
 from fastapi.middleware.cors import CORSMiddleware
-from kedro_graphql import KedroGraphql
+from kedro_graphql import KedroGraphQL
 
 
 
-class MyApp(KedroGraphql):
+class MyApp(KedroGraphQL):
 
     def __init__(self): 
         super(MyApp, self).__init__()
 
         origins = [
             "http://localhost",
             "http://localhost:8080",
@@ -390,15 +417,15 @@
 Configuration can be supplied via environment variables or a ```.env``` file.
 
 ```
 ## example .env file
 MONGO_URI = 'mongodb://root:example@localhost:27017/'
 MONGO_DB_NAME = 'pipelines'
 KEDRO_GRAPHQL_IMPORTS = "kedro_graphql.plugins.plugins"
-KEDRO_GRAPHQL_APP = "kedro_graphql.asgi.KedroGraphql"
+KEDRO_GRAPHQL_APP = "kedro_graphql.asgi.KedroGraphQL"
 ```
 
 ## How to install dependencies
 
 
 To install them, run:
 
@@ -428,12 +455,11 @@
 After this, if you'd like to update your project requirements, please update `src/requirements.txt` and re-run `kedro build-reqs`.
 
 [Further information about project dependencies](https://kedro.readthedocs.io/en/stable/kedro_project_setup/dependencies.html#project-specific-dependencies)
 
 
 ### TO DO
 
-- include EXCEPTION_STATES in kedro_graphql.events.PipelineEventMonitor to exit when task fails
 - support custom runners e.g. Argo Workflows, AWS Batch, etc...
 - document plan for supporting custom IOResolverPlugins 
-- extensible data model to capture additional metadata along with pipeline instance
+- document pipeline tags and implement "search" via tags and/or other fields
```

### Comparing `kedro-graphql-0.2.0/README.md` & `kedro-graphql-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 for serving kedro projects as a graphql api.  It leverages 
 [Strawberry](https://strawberry.rocks/), [FastAPI](https://fastapi.tiangolo.com/), 
 and [Celery](https://docs.celeryq.dev/en/stable/index.html) to turn any 
  [Kedro](https://docs.kedro.org/en/stable/) project into a GraphqlQL api 
  with features such as:
  
  - a distributed task queue
- - events
-   - subscribe to pipeline events (status updates) via GraphQL subscriptions 
+ - subscribe to pipline events and logs via GraphQL subscriptions
  - storage
    - persist and track all pipelines executed via the API
  - [additional features](#features)
 
 ```mermaid
 flowchart  TB
   api[GraphQL API\n<i>strawberry + FastAPI</i>]
@@ -126,14 +125,17 @@
 ```
 
 Start a worker (in another terminal).
 
 ```
 kedro gql -w
 ```
+
+### Start a pipeline
+
 Navigate to http://127.0.0.1:5000/graphql to access the graphql interface 
 and execute the following mutation:
 
 ```
 mutation MyMutation {
   pipeline(
     pipeline: {name: "example00", parameters: [{name: "example", value: "hello"}, {name: "duration", value: "10"}], inputs: {name: "text_in", type: "text.TextDataSet", filepath: "./data/01_raw/text_in.txt"}, outputs: {name: "text_out", type: "text.TextDataSet", filepath: "./data/02_intermediate/text_out.txt"}}
@@ -153,14 +155,16 @@
       "id": "6463991db98d7f8564ab15a0",
       "name": "example00"
     }
   }
 }
 ```
 
+### Subscribe to pipeline events
+
 Now execute the following subscription to track the progress:
 
 ```
 subscription MySubscription {
   pipeline(id: "6463991db98d7f8564ab15a0") {
     id
     result
@@ -170,14 +174,37 @@
     traceback
   }
 }
 ```
 
 ![subscription](docs/subscription.gif)
 
+
+### Susbscribe to pipeline logs
+
+Execute the following subscription to recieve log messages:
+
+
+```
+subscription {
+   	pipelineLogs(id:"6463991db98d7f8564ab15a0") {
+       id
+       message
+       messageId
+       taskId
+       time
+     }
+}
+```
+
+
+![logs subscription](docs/logs-subscription.gif)
+
+### Get the pipeline result
+
 Fetch the pipeline result with the following query:
 
 ```
 query MyQuery {
   pipeline(id: "6463991db98d7f8564ab15a0") {
     describe
     id
@@ -325,19 +352,19 @@
 
 
 This example adds a [CORSMiddleware](https://fastapi.tiangolo.com/tutorial/cors/#use-corsmiddleware).
 
 ```
 ## src/kedro_graphql/example/app.py
 from fastapi.middleware.cors import CORSMiddleware
-from kedro_graphql import KedroGraphql
+from kedro_graphql import KedroGraphQL
 
 
 
-class MyApp(KedroGraphql):
+class MyApp(KedroGraphQL):
 
     def __init__(self): 
         super(MyApp, self).__init__()
 
         origins = [
             "http://localhost",
             "http://localhost:8080",
@@ -376,15 +403,15 @@
 Configuration can be supplied via environment variables or a ```.env``` file.
 
 ```
 ## example .env file
 MONGO_URI = 'mongodb://root:example@localhost:27017/'
 MONGO_DB_NAME = 'pipelines'
 KEDRO_GRAPHQL_IMPORTS = "kedro_graphql.plugins.plugins"
-KEDRO_GRAPHQL_APP = "kedro_graphql.asgi.KedroGraphql"
+KEDRO_GRAPHQL_APP = "kedro_graphql.asgi.KedroGraphQL"
 ```
 
 ## How to install dependencies
 
 
 To install them, run:
 
@@ -414,12 +441,11 @@
 After this, if you'd like to update your project requirements, please update `src/requirements.txt` and re-run `kedro build-reqs`.
 
 [Further information about project dependencies](https://kedro.readthedocs.io/en/stable/kedro_project_setup/dependencies.html#project-specific-dependencies)
 
 
 ### TO DO
 
-- include EXCEPTION_STATES in kedro_graphql.events.PipelineEventMonitor to exit when task fails
 - support custom runners e.g. Argo Workflows, AWS Batch, etc...
 - document plan for supporting custom IOResolverPlugins 
-- extensible data model to capture additional metadata along with pipeline instance
+- document pipeline tags and implement "search" via tags and/or other fields
```

### Comparing `kedro-graphql-0.2.0/pyproject.toml` & `kedro-graphql-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.2.0/src/kedro_graphql/__main__.py` & `kedro-graphql-0.3.0/src/kedro_graphql/__main__.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.2.0/src/kedro_graphql/asgi.py` & `kedro-graphql-0.3.0/src/kedro_graphql/asgi.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from fastapi import FastAPI
 from strawberry.fastapi import GraphQLRouter
 from .backends import init_backend
 from .schema import build_schema       
-class KedroGraphql(FastAPI):
+class KedroGraphQL(FastAPI):
     def __init__(self):
-        super(KedroGraphql, self).__init__()
+        super(KedroGraphQL, self).__init__()
 
         self.backend = init_backend()
     
         @self.on_event("startup")
         def startup_backend():
             self.backend.startup()
```

### Comparing `kedro-graphql-0.2.0/src/kedro_graphql/backends/base.py` & `kedro-graphql-0.3.0/src/kedro_graphql/backends/base.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.2.0/src/kedro_graphql/backends/mongodb.py` & `kedro-graphql-0.3.0/src/kedro_graphql/backends/mongodb.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.2.0/src/kedro_graphql/commands.py` & `kedro-graphql-0.3.0/src/kedro_graphql/commands.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.2.0/src/kedro_graphql/config.py` & `kedro-graphql-0.3.0/src/kedro_graphql/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 conf_parameters = context.config_loader["parameters"]
 
 ## define defaults
 config = {
     "MONGO_URI": "mongodb://root:example@localhost:27017/",
     "MONGO_DB_NAME": "pipelines",
     "KEDRO_GRAPHQL_IMPORTS": "kedro_graphql.plugins.plugins,",
-    "KEDRO_GRAPHQL_APP": "kedro_graphql.asgi.KedroGraphql",
-    "KEDRO_GRAPHQL_BACKEND": "kedro_graphql.backends.mongodb.MongoBackend"
+    "KEDRO_GRAPHQL_APP": "kedro_graphql.asgi.KedroGraphQL",
+    "KEDRO_GRAPHQL_BACKEND": "kedro_graphql.backends.mongodb.MongoBackend",
+    "KEDRO_GRAPHQL_BROKER": "redis://localhost",
+    "KEDRO_GRAPHQL_CELERY_RESULT_BACKEND": "redis://localhost",
     }
 
 load_config = {
     **dotenv_values(".env"),  # load 
     **os.environ,  # override loaded values with environment variables
 }
```

### Comparing `kedro-graphql-0.2.0/src/kedro_graphql/decorators.py` & `kedro-graphql-0.3.0/src/kedro_graphql/decorators.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.2.0/src/kedro_graphql/events.py` & `kedro-graphql-0.3.0/src/kedro_graphql/events.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.2.0/src/kedro_graphql/example/app.py` & `kedro-graphql-0.3.0/src/kedro_graphql/example/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from fastapi.middleware.cors import CORSMiddleware
-from kedro_graphql import KedroGraphql
+from kedro_graphql import KedroGraphQL
 
 
-class MyApp(KedroGraphql):
+class MyApp(KedroGraphQL):
 
     def __init__(self): 
         super(MyApp, self).__init__()
 
         origins = [
             "http://localhost",
             "http://localhost:8080",
```

### Comparing `kedro-graphql-0.2.0/src/kedro_graphql/models.py` & `kedro-graphql-0.3.0/src/kedro_graphql/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,7 +244,14 @@
     id: str
     task_id: str
     status: str
     result: Optional[str] = None
     timestamp: str
     traceback: Optional[str] = None
 
+@strawberry.type
+class PipelineLogMessage:
+    id: str
+    message: str
+    message_id: str
+    task_id: str
+    time: str
```

### Comparing `kedro-graphql-0.2.0/src/kedro_graphql/plugins/plugins.py` & `kedro-graphql-0.3.0/src/kedro_graphql/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.2.0/src/kedro_graphql/schema.py` & `kedro-graphql-0.3.0/src/kedro_graphql/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from .events import PipelineEventMonitor
 import strawberry
 from strawberry.tools import merge_types
 from strawberry.types import Info
 from typing import AsyncGenerator, List
 from .celeryapp import app as APP_CELERY
 from .tasks import run_pipeline
-from .models import Parameter, ParameterInput, DataSet, DataSetInput, Pipeline, PipelineInput, PipelineEvent, PipelineTemplate, Tag, TagInput
+from .models import Parameter, DataSet, Pipeline, PipelineInput, PipelineEvent, PipelineLogMessage, PipelineTemplate, Tag
+from .logs.logger import logger, PipelineLogStream
 
 @strawberry.type
 class Query:
     @strawberry.field
     def pipeline_templates(self) -> List[PipelineTemplate]:
         pipes = []
         for k,v in PIPELINES.items():
@@ -62,28 +63,37 @@
                 "parameters": serial["parameters"]}
         )
         
         ## PLACE HOLDER for future reolver plugins
         ## testing plugin_resolvers, 
         #RESOLVER_PLUGINS["text_in"].__input__("called text_in resolver")
 
-        print(f'Starting {p.name} pipeline with task_id: ' + str(p.task_id))
+        logger.info(f'Starting {p.name} pipeline with task_id: ' + str(p.task_id))
         p = info.context["request"].app.backend.create(p)
-        print(p.id)
 
         return p
 
 
 @strawberry.type
 class Subscription:
     @strawberry.subscription
     async def pipeline(self, id: str, info: Info) -> AsyncGenerator[PipelineEvent, None]:
-        async for e in PipelineEventMonitor(app = APP_CELERY, task_id = info.context["request"].app.backend.load(id=id).task_id ).consume():
-            e["id"] = id
-            yield PipelineEvent(**e)
+        p  = info.context["request"].app.backend.load(id=id)
+        if p:
+            async for e in PipelineEventMonitor(app = APP_CELERY, task_id = p.task_id).consume():
+                e["id"] = id
+                yield PipelineEvent(**e)
+
+    @strawberry.subscription
+    async def pipeline_logs(self, id: str, info: Info) -> AsyncGenerator[PipelineLogMessage, None]:
+        p  = info.context["request"].app.backend.load(id=id)
+        if p:
+            async for e in PipelineLogStream(task_id = p.task_id ).consume():
+                e["id"] = id
+                yield PipelineLogMessage(**e)
 
 
 def build_schema():
     ComboQuery = merge_types("Query", tuple([Query] + TYPE_PLUGINS["query"]))
     ComboMutation = merge_types("Mutation", tuple([Mutation] + TYPE_PLUGINS["mutation"]))
     ComboSubscription = merge_types("Subscription", tuple([Subscription] + TYPE_PLUGINS["subscription"]))
```

### Comparing `kedro-graphql-0.2.0/src/kedro_graphql/settings.py` & `kedro-graphql-0.3.0/src/kedro_graphql/settings.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.2.0/src/kedro_graphql/tasks.py` & `kedro-graphql-0.3.0/src/kedro_graphql/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from kedro.framework.project import pipelines
 from kedro.io import DataCatalog
 from kedro.runner import SequentialRunner
 from celery import shared_task, Task
 from .backends import init_backend
 from fastapi.encoders import jsonable_encoder
 
-
 class KedroGraphqlTask(Task):
     _db = None
 
     @property
     def db(self):
         if self._db is None:
             self._db = init_backend()
@@ -94,18 +93,16 @@
 
         Returns:
             None: The return value of this handler is ignored.
         """
         self.db.update(task_id = task_id, values = {"status": status, "task_einfo": str(einfo)})
 
 
-
 @shared_task(bind = True, base = KedroGraphqlTask)
 def run_pipeline(self, name: str, inputs: dict, outputs: dict, parameters: dict):
-
     catalog = {**inputs, **outputs}
     io = DataCatalog().from_config(catalog = catalog)
 
     ## add parameters to DataCatalog e.g. {"params:myparam":"value"}
     params = {"params:"+k:v for k,v in parameters.items()}
     params["parameters"] = parameters
     io.add_feed_dict(params)
```

### Comparing `kedro-graphql-0.2.0/src/kedro_graphql.egg-info/PKG-INFO` & `kedro-graphql-0.3.0/src/kedro_graphql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-graphql
-Version: 0.2.0
+Version: 0.3.0
 Summary: Kedro helps you build production-ready data and analytics pipelines
 Author: opensean
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://github.com/opensean/kedro-graphql
 Project-URL: Source, https://github.com/opensean/kedro-graphql
 Keywords: pipelines,machine learning,data pipelines,data science,data engineering
 Classifier: Programming Language :: Python :: 3.10
@@ -20,16 +20,15 @@
 for serving kedro projects as a graphql api.  It leverages 
 [Strawberry](https://strawberry.rocks/), [FastAPI](https://fastapi.tiangolo.com/), 
 and [Celery](https://docs.celeryq.dev/en/stable/index.html) to turn any 
  [Kedro](https://docs.kedro.org/en/stable/) project into a GraphqlQL api 
  with features such as:
  
  - a distributed task queue
- - events
-   - subscribe to pipeline events (status updates) via GraphQL subscriptions 
+ - subscribe to pipline events and logs via GraphQL subscriptions
  - storage
    - persist and track all pipelines executed via the API
  - [additional features](#features)
 
 ```mermaid
 flowchart  TB
   api[GraphQL API\n<i>strawberry + FastAPI</i>]
@@ -140,14 +139,17 @@
 ```
 
 Start a worker (in another terminal).
 
 ```
 kedro gql -w
 ```
+
+### Start a pipeline
+
 Navigate to http://127.0.0.1:5000/graphql to access the graphql interface 
 and execute the following mutation:
 
 ```
 mutation MyMutation {
   pipeline(
     pipeline: {name: "example00", parameters: [{name: "example", value: "hello"}, {name: "duration", value: "10"}], inputs: {name: "text_in", type: "text.TextDataSet", filepath: "./data/01_raw/text_in.txt"}, outputs: {name: "text_out", type: "text.TextDataSet", filepath: "./data/02_intermediate/text_out.txt"}}
@@ -167,14 +169,16 @@
       "id": "6463991db98d7f8564ab15a0",
       "name": "example00"
     }
   }
 }
 ```
 
+### Subscribe to pipeline events
+
 Now execute the following subscription to track the progress:
 
 ```
 subscription MySubscription {
   pipeline(id: "6463991db98d7f8564ab15a0") {
     id
     result
@@ -184,14 +188,37 @@
     traceback
   }
 }
 ```
 
 ![subscription](docs/subscription.gif)
 
+
+### Susbscribe to pipeline logs
+
+Execute the following subscription to recieve log messages:
+
+
+```
+subscription {
+   	pipelineLogs(id:"6463991db98d7f8564ab15a0") {
+       id
+       message
+       messageId
+       taskId
+       time
+     }
+}
+```
+
+
+![logs subscription](docs/logs-subscription.gif)
+
+### Get the pipeline result
+
 Fetch the pipeline result with the following query:
 
 ```
 query MyQuery {
   pipeline(id: "6463991db98d7f8564ab15a0") {
     describe
     id
@@ -339,19 +366,19 @@
 
 
 This example adds a [CORSMiddleware](https://fastapi.tiangolo.com/tutorial/cors/#use-corsmiddleware).
 
 ```
 ## src/kedro_graphql/example/app.py
 from fastapi.middleware.cors import CORSMiddleware
-from kedro_graphql import KedroGraphql
+from kedro_graphql import KedroGraphQL
 
 
 
-class MyApp(KedroGraphql):
+class MyApp(KedroGraphQL):
 
     def __init__(self): 
         super(MyApp, self).__init__()
 
         origins = [
             "http://localhost",
             "http://localhost:8080",
@@ -390,15 +417,15 @@
 Configuration can be supplied via environment variables or a ```.env``` file.
 
 ```
 ## example .env file
 MONGO_URI = 'mongodb://root:example@localhost:27017/'
 MONGO_DB_NAME = 'pipelines'
 KEDRO_GRAPHQL_IMPORTS = "kedro_graphql.plugins.plugins"
-KEDRO_GRAPHQL_APP = "kedro_graphql.asgi.KedroGraphql"
+KEDRO_GRAPHQL_APP = "kedro_graphql.asgi.KedroGraphQL"
 ```
 
 ## How to install dependencies
 
 
 To install them, run:
 
@@ -428,12 +455,11 @@
 After this, if you'd like to update your project requirements, please update `src/requirements.txt` and re-run `kedro build-reqs`.
 
 [Further information about project dependencies](https://kedro.readthedocs.io/en/stable/kedro_project_setup/dependencies.html#project-specific-dependencies)
 
 
 ### TO DO
 
-- include EXCEPTION_STATES in kedro_graphql.events.PipelineEventMonitor to exit when task fails
 - support custom runners e.g. Argo Workflows, AWS Batch, etc...
 - document plan for supporting custom IOResolverPlugins 
-- extensible data model to capture additional metadata along with pipeline instance
+- document pipeline tags and implement "search" via tags and/or other fields
```

### Comparing `kedro-graphql-0.2.0/src/kedro_graphql.egg-info/SOURCES.txt` & `kedro-graphql-0.3.0/src/kedro_graphql.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,27 @@
 src/kedro_graphql.egg-info/requires.txt
 src/kedro_graphql.egg-info/top_level.txt
 src/kedro_graphql/backends/__init__.py
 src/kedro_graphql/backends/base.py
 src/kedro_graphql/backends/mongodb.py
 src/kedro_graphql/example/__init__.py
 src/kedro_graphql/example/app.py
+src/kedro_graphql/logs/__init__.py
+src/kedro_graphql/logs/json_log_formatter.py
+src/kedro_graphql/logs/logger.py
 src/kedro_graphql/pipelines/__init__.py
 src/kedro_graphql/pipelines/example00/__init__.py
 src/kedro_graphql/pipelines/example00/nodes.py
 src/kedro_graphql/pipelines/example00/pipeline.py
 src/kedro_graphql/plugins/__init__.py
 src/kedro_graphql/plugins/plugins.py
 src/tests/__init__.py
 src/tests/conftest.py
 src/tests/test_events.py
+src/tests/test_logs.py
 src/tests/test_run.py
 src/tests/test_schema_mutation.py
 src/tests/test_schema_query.py
 src/tests/test_schema_subscription.py
 src/tests/pipelines/__init__.py
 src/tests/pipelines/example00/__init__.py
 src/tests/pipelines/example00/test_pipeline.py
```

### Comparing `kedro-graphql-0.2.0/src/setup.py` & `kedro-graphql-0.3.0/src/setup.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.2.0/src/tests/conftest.py` & `kedro-graphql-0.3.0/src/tests/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -106,8 +106,44 @@
             "inputs": serial["inputs"], 
             "outputs": serial["outputs"], 
             "parameters": serial["parameters"]}
     )
 
     print(f'Starting {p.name} pipeline with task_id: ' + str(p.task_id))
     p = mock_backend.create(p)
+    return p
+
+@pytest.fixture
+def mock_pipeline2(mock_backend, tmp_path, mock_text_in, mock_text_out):
+
+    inputs = [{"name": "text_in", "type": "text.TextDataSet", "filepath": str(mock_text_in)}]
+    outputs = [{"name":"text_out", "type": "text.TextDataSet", "filepath": str(mock_text_out)}]
+    parameters = [{"name":"example", "value":"hello"}]
+    tags = [{"key": "author", "value": "opensean"},{"key":"package", "value":"kedro-graphql"}]
+
+    p = Pipeline(
+        name = "example00",
+        inputs = [DataSet(**i) for i in inputs],
+        outputs = [DataSet(**o) for o in outputs],
+        parameters = [Parameter(**p) for p in parameters],
+        tags = [Tag(**p) for p in tags],
+        task_name = str(run_pipeline),
+    )
+
+    serial = p.serialize()
+
+    result = run_pipeline.apply_async(kwargs = {"name": "example00", 
+                                                 "inputs": serial["inputs"], 
+                                                 "outputs": serial["outputs"],
+                                                 "parameters": serial["parameters"]}, countdown=0.1)
+    p.task_id = result.id
+    p.status = result.status
+    p.task_kwargs = str(
+            {"name": serial["name"], 
+            "inputs": serial["inputs"], 
+            "outputs": serial["outputs"], 
+            "parameters": serial["parameters"]}
+    )
+
+    print(f'Starting {p.name} pipeline with task_id: ' + str(p.task_id))
+    p = mock_backend.create(p)
     return p
```

### Comparing `kedro-graphql-0.2.0/src/tests/test_events.py` & `kedro-graphql-0.3.0/src/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.2.0/src/tests/test_run.py` & `kedro-graphql-0.3.0/src/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.2.0/src/tests/test_schema_mutation.py` & `kedro-graphql-0.3.0/src/tests/test_schema_mutation.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.2.0/src/tests/test_schema_query.py` & `kedro-graphql-0.3.0/src/tests/test_schema_query.py`

 * *Files identical despite different names*

