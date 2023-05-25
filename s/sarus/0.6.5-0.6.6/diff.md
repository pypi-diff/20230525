# Comparing `tmp/sarus-0.6.5.tar.gz` & `tmp/sarus-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus-0.6.5.tar", last modified: Mon May 22 16:45:34 2023, max compression
+gzip compressed data, was "sarus-0.6.6.tar", last modified: Thu May 25 14:38:27 2023, max compression
```

## Comparing `sarus-0.6.5.tar` & `sarus-0.6.6.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.845399 sarus-0.6.5/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2022-09-14 12:56:20.000000 sarus-0.6.5/MANIFEST.in
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-05-22 16:45:34.845399 sarus-0.6.5/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.6.5/README.rst
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.6.5/pyproject.toml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.821399 sarus-0.6.5/sarus/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      544 2023-05-22 16:38:31.000000 sarus-0.6.5/sarus/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    12913 2023-05-22 16:34:35.000000 sarus-0.6.5/sarus/config.yaml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.825399 sarus-0.6.5/sarus/context/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/context/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3179 2023-05-15 07:50:17.000000 sarus-0.6.5/sarus/context/local_sdk.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-05-15 07:50:17.000000 sarus-0.6.5/sarus/context/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    14066 2023-05-22 16:34:35.000000 sarus-0.6.5/sarus/dataspec_wrapper.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-04-21 19:49:48.000000 sarus-0.6.5/sarus/debug.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.825399 sarus-0.6.5/sarus/imblearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/imblearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/imblearn/over_sampling.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/imblearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/imblearn/under_sampling.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.825399 sarus-0.6.5/sarus/legacy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/legacy/__init__.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.825399 sarus-0.6.5/sarus/legacy/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2023-01-27 14:38:46.000000 sarus-0.6.5/sarus/legacy/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    16606 2023-01-27 14:38:46.000000 sarus-0.6.5/sarus/legacy/pandas/dataframe.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.829399 sarus-0.6.5/sarus/legacy/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/legacy/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2022-12-01 13:21:20.000000 sarus-0.6.5/sarus/legacy/tensorflow/dataset.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/legacy/tensorflow/model.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.833399 sarus-0.6.5/sarus/manager/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/manager/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5490 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/manager/arrow_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1927 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/manager/arrow_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1296 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/manager/base_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3869 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/manager/cache_scalar_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     7609 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/manager/dataspec_api.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.833399 sarus-0.6.5/sarus/manager/ops/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/manager/ops/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      921 2023-04-21 19:49:48.000000 sarus-0.6.5/sarus/manager/ops/api.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3487 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/manager/parquet_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    21049 2023-05-15 16:20:25.000000 sarus-0.6.5/sarus/manager/sdk_manager.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2650 2023-05-22 16:34:35.000000 sarus-0.6.5/sarus/manager/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4729 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/manager/value_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1573 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/manager/value_remote.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.833399 sarus-0.6.5/sarus/numpy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/numpy/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/numpy/random.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/numpy/scalars.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.833399 sarus-0.6.5/sarus/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      822 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/pandas/core.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4918 2023-04-21 19:49:48.000000 sarus-0.6.5/sarus/pandas/dataframe.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/pandas/io.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.837399 sarus-0.6.5/sarus/pandas_profiling/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/pandas_profiling/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      377 2023-05-15 07:50:17.000000 sarus-0.6.5/sarus/pandas_profiling/profile_report.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.837399 sarus-0.6.5/sarus/plotly/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/plotly/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/plotly/express.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    55850 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/sarus.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.837399 sarus-0.6.5/sarus/scripts/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-04-21 19:49:48.000000 sarus-0.6.5/sarus/scripts/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4672 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/scripts/generate_op_list.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.841399 sarus-0.6.5/sarus/sklearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-04-21 19:49:48.000000 sarus-0.6.5/sarus/sklearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-05-15 07:50:17.000000 sarus-0.6.5/sarus/sklearn/cluster.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/sklearn/compose.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-05-15 07:50:17.000000 sarus-0.6.5/sarus/sklearn/decomposition.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-05-15 07:50:17.000000 sarus-0.6.5/sarus/sklearn/ensemble.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/sklearn/impute.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/sklearn/inspection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-04-21 19:49:48.000000 sarus-0.6.5/sarus/sklearn/linear_model.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/sklearn/metrics.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1073 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/sklearn/model_selection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/sklearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1571 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/sklearn/preprocessing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-04-21 19:49:48.000000 sarus-0.6.5/sarus/sklearn/svm.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.841399 sarus-0.6.5/sarus/skopt/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/skopt/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/skopt/searchcv.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.845399 sarus-0.6.5/sarus/std/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/std/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1600 2023-05-22 16:34:35.000000 sarus-0.6.5/sarus/std/types.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.845399 sarus-0.6.5/sarus/storage/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-01-27 14:38:46.000000 sarus-0.6.5/sarus/storage/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4552 2023-01-27 14:38:46.000000 sarus-0.6.5/sarus/storage/legacy_local.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.845399 sarus-0.6.5/sarus/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1831 2023-05-22 16:34:35.000000 sarus-0.6.5/sarus/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    10848 2023-05-15 16:20:25.000000 sarus-0.6.5/sarus/utils.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-04-21 19:49:48.000000 sarus-0.6.5/sarus/wrapper_factory.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.845399 sarus-0.6.5/sarus/xgboost/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/xgboost/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      754 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/xgboost/xgboost.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.821399 sarus-0.6.5/sarus.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-05-22 16:45:34.000000 sarus-0.6.5/sarus.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2086 2023-05-22 16:45:34.000000 sarus-0.6.5/sarus.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-05-22 16:45:34.000000 sarus-0.6.5/sarus.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.6.5/sarus.egg-info/not-zip-safe
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      344 2023-05-22 16:45:34.000000 sarus-0.6.5/sarus.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-05-22 16:45:34.000000 sarus-0.6.5/sarus.egg-info/top_level.txt
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1301 2023-05-22 16:45:34.845399 sarus-0.6.5/setup.cfg
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      106 2023-05-22 16:38:22.000000 sarus-0.6.5/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.845399 sarus-0.6.5/tests/
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2021-09-06 19:14:48.000000 sarus-0.6.5/tests/test_sanity.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.033366 sarus-0.6.6/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2023-05-23 10:20:26.000000 sarus-0.6.6/MANIFEST.in
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-05-25 14:38:27.033366 sarus-0.6.6/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.6.6/README.rst
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.6.6/pyproject.toml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.021366 sarus-0.6.6/sarus/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      544 2023-05-25 14:37:59.000000 sarus-0.6.6/sarus/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    12913 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/config.yaml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.021366 sarus-0.6.6/sarus/context/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/context/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3179 2023-05-25 13:23:23.000000 sarus-0.6.6/sarus/context/local_sdk.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/context/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13842 2023-05-25 13:23:26.000000 sarus-0.6.6/sarus/dataspec_wrapper.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/debug.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.021366 sarus-0.6.6/sarus/imblearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/imblearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/imblearn/over_sampling.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/imblearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/imblearn/under_sampling.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.021366 sarus-0.6.6/sarus/legacy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/legacy/__init__.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.021366 sarus-0.6.6/sarus/legacy/pandas/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2023-05-25 13:23:23.000000 sarus-0.6.6/sarus/legacy/pandas/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    16606 2023-05-25 13:23:23.000000 sarus-0.6.6/sarus/legacy/pandas/dataframe.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.025366 sarus-0.6.6/sarus/legacy/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/legacy/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/legacy/tensorflow/dataset.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/legacy/tensorflow/model.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.025366 sarus-0.6.6/sarus/manager/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/manager/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5490 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/manager/arrow_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1927 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/manager/arrow_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1296 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/manager/base_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3869 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/manager/cache_scalar_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     7609 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/manager/dataspec_api.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.025366 sarus-0.6.6/sarus/manager/ops/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/manager/ops/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      688 2023-05-25 13:23:26.000000 sarus-0.6.6/sarus/manager/ops/api.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3487 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/manager/parquet_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    20847 2023-05-25 13:23:26.000000 sarus-0.6.6/sarus/manager/sdk_manager.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2650 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/manager/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4729 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/manager/value_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1573 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/manager/value_remote.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.029366 sarus-0.6.6/sarus/numpy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/numpy/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/numpy/random.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/numpy/scalars.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.029366 sarus-0.6.6/sarus/pandas/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/pandas/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      822 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/pandas/core.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4843 2023-05-25 13:23:26.000000 sarus-0.6.6/sarus/pandas/dataframe.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/pandas/io.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.029366 sarus-0.6.6/sarus/pandas_profiling/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/pandas_profiling/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      377 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/pandas_profiling/profile_report.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.029366 sarus-0.6.6/sarus/plotly/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/plotly/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/plotly/express.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    55850 2023-05-25 13:23:23.000000 sarus-0.6.6/sarus/sarus.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.029366 sarus-0.6.6/sarus/scripts/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/scripts/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4672 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/scripts/generate_op_list.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.033366 sarus-0.6.6/sarus/sklearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/sklearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/sklearn/cluster.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/sklearn/compose.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/sklearn/decomposition.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/sklearn/ensemble.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/sklearn/impute.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/sklearn/inspection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/sklearn/linear_model.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/sklearn/metrics.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1073 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/sklearn/model_selection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/sklearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1571 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/sklearn/preprocessing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/sklearn/svm.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.033366 sarus-0.6.6/sarus/skopt/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/skopt/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/skopt/searchcv.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.033366 sarus-0.6.6/sarus/std/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/std/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1600 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/std/types.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.033366 sarus-0.6.6/sarus/storage/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-25 13:23:23.000000 sarus-0.6.6/sarus/storage/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4552 2023-05-25 13:23:23.000000 sarus-0.6.6/sarus/storage/legacy_local.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.033366 sarus-0.6.6/sarus/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1831 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    10848 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/utils.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/wrapper_factory.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.033366 sarus-0.6.6/sarus/xgboost/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/xgboost/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      754 2023-05-23 10:20:26.000000 sarus-0.6.6/sarus/xgboost/xgboost.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.021366 sarus-0.6.6/sarus.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-05-25 14:38:26.000000 sarus-0.6.6/sarus.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2086 2023-05-25 14:38:26.000000 sarus-0.6.6/sarus.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-05-25 14:38:26.000000 sarus-0.6.6/sarus.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.6.6/sarus.egg-info/not-zip-safe
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      344 2023-05-25 14:38:26.000000 sarus-0.6.6/sarus.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-05-25 14:38:26.000000 sarus-0.6.6/sarus.egg-info/top_level.txt
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1301 2023-05-25 14:38:27.037366 sarus-0.6.6/setup.cfg
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      106 2023-05-25 14:37:45.000000 sarus-0.6.6/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-25 14:38:27.033366 sarus-0.6.6/tests/
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2021-09-06 19:14:48.000000 sarus-0.6.6/tests/test_sanity.py
```

### Comparing `sarus-0.6.5/PKG-INFO` & `sarus-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.6.5
+Version: 0.6.6
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.6.5/README.rst` & `sarus-0.6.6/README.rst`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/config.yaml` & `sarus-0.6.6/sarus/config.yaml`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/context/local_sdk.py` & `sarus-0.6.6/sarus/context/local_sdk.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/dataspec_wrapper.py` & `sarus-0.6.6/sarus/dataspec_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,19 +235,14 @@
         if launch:
             computation = self.manager().dataspec_computation(alt_dataspec)
             if self.manager().status(dataspec, computation.task_name) is None:
                 self.manager().launch(alt_dataspec)
 
         return alt_dataspec, alt_policy
 
-    def delete_from_server(self) -> None:
-        """Delete a DataSpec from the server's storage."""
-        dataspec = self.dataspec(kind=DataSpecVariant.ALTERNATIVE)
-        self.manager()._delete_remote(dataspec.uuid())
-
     def delete_from_local(self) -> None:
         """Delete a DataSpec from the local storage."""
         dataspec = self.dataspec(kind=DataSpecVariant.ALTERNATIVE)
         self.manager()._delete_local(dataspec.uuid())
 
     def __eval_policy__(self) -> str:
         """The alternative dataspec's privacy policy."""
```

### Comparing `sarus-0.6.5/sarus/debug.py` & `sarus-0.6.6/sarus/debug.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/imblearn/over_sampling.py` & `sarus-0.6.6/sarus/imblearn/over_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/imblearn/pipeline.py` & `sarus-0.6.6/sarus/imblearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/imblearn/under_sampling.py` & `sarus-0.6.6/sarus/imblearn/under_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/legacy/pandas/dataframe.py` & `sarus-0.6.6/sarus/legacy/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/legacy/tensorflow/dataset.py` & `sarus-0.6.6/sarus/legacy/tensorflow/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/legacy/tensorflow/model.py` & `sarus-0.6.6/sarus/legacy/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/manager/arrow_local.py` & `sarus-0.6.6/sarus/manager/arrow_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/manager/arrow_remote.py` & `sarus-0.6.6/sarus/manager/arrow_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/manager/base_remote.py` & `sarus-0.6.6/sarus/manager/base_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/manager/cache_scalar_local.py` & `sarus-0.6.6/sarus/manager/cache_scalar_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/manager/dataspec_api.py` & `sarus-0.6.6/sarus/manager/dataspec_api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/manager/ops/api.py` & `sarus-0.6.6/sarus/manager/ops/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,15 +22,7 @@
             f"Error while retrieving synthetic data. "
             f"Gateway answer was: \n{resp}"
         )
 
     synthetic_table = pq.ParquetFile(io.BytesIO(resp.content)).read()
 
     return synthetic_table
-
-
-def delete_dataspec(client: Client, uuid: str) -> requests.Response:
-    """Delete a DataSpec from the server."""
-    return client.session().delete(
-        url=f"{client.url()}/v2/dataspecs",
-        params={"uuid": uuid},
-    )
```

### Comparing `sarus-0.6.5/sarus/manager/parquet_local.py` & `sarus-0.6.6/sarus/manager/parquet_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/manager/sdk_manager.py` & `sarus-0.6.6/sarus/manager/sdk_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,18 +307,14 @@
             "dataspecs": visitor.dataspecs[::-1],
             "transforms": visitor.transforms,
             "attributes": visitor.attributes,
             "variant_constraints": visitor.variant_constraints,
             "edges": visitor.edges,
         }
 
-    def _delete_remote(self, uuid: str) -> requests.Response:
-        """Delete a DataSpec and referring items on the server."""
-        return api_ops.delete_dataspec(client=self.client(), uuid=uuid)
-
     def _delete_local(self, uuid: str) -> None:
         """Delete a DataSpec locally. MOCKs also have to be deleted."""
         would_delete = self.storage().all_referrings(uuid)
         additional_cleanup = []
         for uuid in would_delete:
             item = self.storage().referrable(uuid)
             if item.prototype() in [sp.Dataset, sp.Scalar]:
```

### Comparing `sarus-0.6.5/sarus/manager/typing.py` & `sarus-0.6.6/sarus/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/manager/value_local.py` & `sarus-0.6.6/sarus/manager/value_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/manager/value_remote.py` & `sarus-0.6.6/sarus/manager/value_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/numpy/scalars.py` & `sarus-0.6.6/sarus/numpy/scalars.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/pandas/core.py` & `sarus-0.6.6/sarus/pandas/core.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/pandas/dataframe.py` & `sarus-0.6.6/sarus/pandas/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,14 @@
     def columns(self):
         ...
 
     @sarus_property("pandas.PD_AXES")
     def axes(self):
         ...
 
-    @sarus_property("pandas.PD_DTYPES")
-    def dtypes(self):
-        ...
-
     @sarus_property("pandas.PD_INDEX")
     def index(self):
         ...
 
     @sarus_property("pandas.PD_SHAPE")
     def shape(self):
         ...
```

### Comparing `sarus-0.6.5/sarus/sarus.py` & `sarus-0.6.6/sarus/sarus.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/scripts/generate_op_list.py` & `sarus-0.6.6/sarus/scripts/generate_op_list.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/sklearn/__init__.py` & `sarus-0.6.6/sarus/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/sklearn/cluster.py` & `sarus-0.6.6/sarus/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/sklearn/compose.py` & `sarus-0.6.6/sarus/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/sklearn/decomposition.py` & `sarus-0.6.6/sarus/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/sklearn/ensemble.py` & `sarus-0.6.6/sarus/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/sklearn/impute.py` & `sarus-0.6.6/sarus/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/sklearn/linear_model.py` & `sarus-0.6.6/sarus/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/sklearn/model_selection.py` & `sarus-0.6.6/sarus/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/sklearn/pipeline.py` & `sarus-0.6.6/sarus/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/sklearn/preprocessing.py` & `sarus-0.6.6/sarus/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/sklearn/svm.py` & `sarus-0.6.6/sarus/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/skopt/searchcv.py` & `sarus-0.6.6/sarus/skopt/searchcv.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/std/types.py` & `sarus-0.6.6/sarus/std/types.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/storage/legacy_local.py` & `sarus-0.6.6/sarus/storage/legacy_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/typing.py` & `sarus-0.6.6/sarus/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/utils.py` & `sarus-0.6.6/sarus/utils.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/wrapper_factory.py` & `sarus-0.6.6/sarus/wrapper_factory.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus/xgboost/xgboost.py` & `sarus-0.6.6/sarus/xgboost/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/sarus.egg-info/PKG-INFO` & `sarus-0.6.6/sarus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.6.5
+Version: 0.6.6
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.6.5/sarus.egg-info/SOURCES.txt` & `sarus-0.6.6/sarus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarus-0.6.5/setup.cfg` & `sarus-0.6.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 [options]
 zip_safe = False
 python_requires = >=3.7, <3.11
 packages = find:
 include_package_data = True
 install_requires = 
-	sarus-data-spec-public==3.2.2
+	sarus-data-spec-public==3.2.4
 	matplotlib>=3.1
 	cloudpickle>=1.2, <2.1
 
 [options.extras_require]
 sklearn = 
 	scikit-learn==1.2.2
 	scipy==1.9.0
```

