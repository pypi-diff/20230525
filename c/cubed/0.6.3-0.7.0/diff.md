# Comparing `tmp/cubed-0.6.3.tar.gz` & `tmp/cubed-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubed-0.6.3.tar", last modified: Fri May 19 11:17:54 2023, max compression
+gzip compressed data, was "cubed-0.7.0.tar", last modified: Thu May 25 11:02:26 2023, max compression
```

## Comparing `cubed-0.6.3.tar` & `cubed-0.7.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.267562 cubed-0.6.3/
--rw-r--r--   0 tom        (501) staff       (20)    11358 2023-05-16 07:59:53.000000 cubed-0.6.3/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)     1868 2023-05-19 11:17:54.267632 cubed-0.6.3/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      939 2023-02-21 09:42:15.000000 cubed-0.6.3/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.256810 cubed-0.6.3/cubed/
--rw-r--r--   0 tom        (501) staff       (20)      846 2023-05-05 10:22:49.000000 cubed-0.6.3/cubed/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.259121 cubed-0.6.3/cubed/array_api/
--rw-r--r--   0 tom        (501) staff       (20)     3578 2023-02-16 11:53:37.000000 cubed-0.6.3/cubed/array_api/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    12924 2023-02-16 11:53:37.000000 cubed-0.6.3/cubed/array_api/array_object.py
--rw-r--r--   0 tom        (501) staff       (20)       81 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/array_api/constants.py
--rw-r--r--   0 tom        (501) staff       (20)     8760 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/array_api/creation_functions.py
--rw-r--r--   0 tom        (501) staff       (20)      751 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/array_api/data_type_functions.py
--rw-r--r--   0 tom        (501) staff       (20)      471 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/array_api/dtypes.py
--rw-r--r--   0 tom        (501) staff       (20)    11395 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/array_api/elementwise_functions.py
--rw-r--r--   0 tom        (501) staff       (20)       83 2023-02-16 11:53:37.000000 cubed-0.6.3/cubed/array_api/indexing_functions.py
--rw-r--r--   0 tom        (501) staff       (20)     4016 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/array_api/linear_algebra_functions.py
--rw-r--r--   0 tom        (501) staff       (20)     9132 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/array_api/manipulation_functions.py
--rw-r--r--   0 tom        (501) staff       (20)     1010 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/array_api/searching_functions.py
--rw-r--r--   0 tom        (501) staff       (20)     3693 2023-03-17 17:46:35.000000 cubed-0.6.3/cubed/array_api/statistical_functions.py
--rw-r--r--   0 tom        (501) staff       (20)      479 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/array_api/utility_functions.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.259813 cubed-0.6.3/cubed/core/
--rw-r--r--   0 tom        (501) staff       (20)      431 2023-02-17 17:56:56.000000 cubed-0.6.3/cubed/core/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    11826 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/core/array.py
--rw-r--r--   0 tom        (501) staff       (20)     5531 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/core/gufunc.py
--rw-r--r--   0 tom        (501) staff       (20)    26650 2023-05-19 08:43:28.000000 cubed-0.6.3/cubed/core/ops.py
--rw-r--r--   0 tom        (501) staff       (20)    11573 2023-05-19 08:43:28.000000 cubed-0.6.3/cubed/core/plan.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.260500 cubed-0.6.3/cubed/extensions/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/extensions/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1164 2023-05-19 08:43:28.000000 cubed-0.6.3/cubed/extensions/history.py
--rw-r--r--   0 tom        (501) staff       (20)     2738 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/extensions/timeline.py
--rw-r--r--   0 tom        (501) staff       (20)     1439 2023-02-16 11:53:37.000000 cubed-0.6.3/cubed/extensions/tqdm.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.261086 cubed-0.6.3/cubed/primitive/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/primitive/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    10932 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/primitive/blockwise.py
--rw-r--r--   0 tom        (501) staff       (20)     1853 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/primitive/rechunk.py
--rw-r--r--   0 tom        (501) staff       (20)      355 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/primitive/types.py
--rw-r--r--   0 tom        (501) staff       (20)     1381 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/random.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.261829 cubed-0.6.3/cubed/runtime/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/runtime/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      953 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/runtime/backup.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.263041 cubed-0.6.3/cubed/runtime/executors/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/runtime/executors/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     8292 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/runtime/executors/beam.py
--rw-r--r--   0 tom        (501) staff       (20)     9228 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/runtime/executors/lithops.py
--rw-r--r--   0 tom        (501) staff       (20)     3460 2023-03-27 13:45:10.000000 cubed-0.6.3/cubed/runtime/executors/modal.py
--rw-r--r--   0 tom        (501) staff       (20)     6115 2023-05-10 09:39:13.000000 cubed-0.6.3/cubed/runtime/executors/modal_async.py
--rw-r--r--   0 tom        (501) staff       (20)     1279 2023-02-16 11:53:37.000000 cubed-0.6.3/cubed/runtime/executors/python.py
--rw-r--r--   0 tom        (501) staff       (20)     4187 2023-05-10 09:39:13.000000 cubed-0.6.3/cubed/runtime/executors/python_async.py
--rw-r--r--   0 tom        (501) staff       (20)     3620 2023-03-17 17:46:35.000000 cubed-0.6.3/cubed/runtime/pipeline.py
--rw-r--r--   0 tom        (501) staff       (20)      251 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/runtime/types.py
--rw-r--r--   0 tom        (501) staff       (20)      118 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/runtime/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.264359 cubed-0.6.3/cubed/tests/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/tests/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.264718 cubed-0.6.3/cubed/tests/primitive/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/tests/primitive/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     6323 2023-05-19 11:15:54.000000 cubed-0.6.3/cubed/tests/primitive/test_blockwise.py
--rw-r--r--   0 tom        (501) staff       (20)     2505 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/tests/primitive/test_rechunk.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.265197 cubed-0.6.3/cubed/tests/runtime/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/tests/runtime/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      860 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/tests/runtime/test_backup.py
--rw-r--r--   0 tom        (501) staff       (20)     4014 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/tests/runtime/test_lithops.py
--rw-r--r--   0 tom        (501) staff       (20)     4691 2023-03-27 13:45:10.000000 cubed-0.6.3/cubed/tests/runtime/test_modal_async.py
--rw-r--r--   0 tom        (501) staff       (20)    16651 2023-02-16 11:53:37.000000 cubed-0.6.3/cubed/tests/test_array_api.py
--rw-r--r--   0 tom        (501) staff       (20)    14469 2023-05-19 11:15:54.000000 cubed-0.6.3/cubed/tests/test_core.py
--rw-r--r--   0 tom        (501) staff       (20)     3024 2023-02-21 09:41:17.000000 cubed-0.6.3/cubed/tests/test_gufunc.py
--rw-r--r--   0 tom        (501) staff       (20)     1450 2023-02-16 11:53:37.000000 cubed-0.6.3/cubed/tests/test_indexing.py
--rw-r--r--   0 tom        (501) staff       (20)     6778 2023-05-19 08:43:28.000000 cubed-0.6.3/cubed/tests/test_mem_utilization.py
--rw-r--r--   0 tom        (501) staff       (20)     2393 2023-02-16 11:53:37.000000 cubed-0.6.3/cubed/tests/test_optimization.py
--rw-r--r--   0 tom        (501) staff       (20)     1221 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/tests/test_random.py
--rw-r--r--   0 tom        (501) staff       (20)     2292 2023-05-19 11:15:54.000000 cubed-0.6.3/cubed/tests/test_utils.py
--rw-r--r--   0 tom        (501) staff       (20)     2861 2023-05-19 11:15:54.000000 cubed-0.6.3/cubed/tests/utils.py
--rw-r--r--   0 tom        (501) staff       (20)     4494 2023-05-19 11:15:54.000000 cubed-0.6.3/cubed/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.265323 cubed-0.6.3/cubed/vendor/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/vendor/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.265777 cubed-0.6.3/cubed/vendor/dask/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/dask/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.266386 cubed-0.6.3/cubed/vendor/dask/array/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/dask/array/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    17366 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/dask/array/core.py
--rw-r--r--   0 tom        (501) staff       (20)     1685 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/dask/array/gufunc.py
--rw-r--r--   0 tom        (501) staff       (20)     4670 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/dask/array/reshape.py
--rw-r--r--   0 tom        (501) staff       (20)      543 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/dask/array/utils.py
--rw-r--r--   0 tom        (501) staff       (20)    14901 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/dask/blockwise.py
--rw-r--r--   0 tom        (501) staff       (20)      608 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/dask/core.py
--rw-r--r--   0 tom        (501) staff       (20)     2221 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/dask/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.267219 cubed-0.6.3/cubed/vendor/rechunker/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/vendor/rechunker/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    13197 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/vendor/rechunker/algorithm.py
--rw-r--r--   0 tom        (501) staff       (20)    12312 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/rechunker/api.py
--rw-r--r--   0 tom        (501) staff       (20)      309 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/vendor/rechunker/compat.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.267455 cubed-0.6.3/cubed/vendor/rechunker/executors/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/vendor/rechunker/executors/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      923 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/vendor/rechunker/executors/python.py
--rw-r--r--   0 tom        (501) staff       (20)     3421 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/vendor/rechunker/types.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.257462 cubed-0.6.3/cubed.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)     1868 2023-05-19 11:17:54.000000 cubed-0.6.3/cubed.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     2506 2023-05-19 11:17:54.000000 cubed-0.6.3/cubed.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-05-19 11:17:54.000000 cubed-0.6.3/cubed.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)      407 2023-05-19 11:17:54.000000 cubed-0.6.3/cubed.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)        6 2023-05-19 11:17:54.000000 cubed-0.6.3/cubed.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)     1652 2023-05-19 11:17:18.000000 cubed-0.6.3/pyproject.toml
--rw-r--r--   0 tom        (501) staff       (20)     1195 2023-05-19 11:17:54.268182 cubed-0.6.3/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      289 2023-05-16 07:59:53.000000 cubed-0.6.3/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.278348 cubed-0.7.0/
+-rw-r--r--   0 tom        (501) staff       (20)    11358 2023-05-16 07:59:53.000000 cubed-0.7.0/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)     1843 2023-05-25 11:02:26.278428 cubed-0.7.0/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      939 2023-02-21 09:42:15.000000 cubed-0.7.0/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.262299 cubed-0.7.0/cubed/
+-rw-r--r--   0 tom        (501) staff       (20)      846 2023-05-05 10:22:49.000000 cubed-0.7.0/cubed/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.266378 cubed-0.7.0/cubed/array_api/
+-rw-r--r--   0 tom        (501) staff       (20)     3578 2023-02-16 11:53:37.000000 cubed-0.7.0/cubed/array_api/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    12924 2023-02-16 11:53:37.000000 cubed-0.7.0/cubed/array_api/array_object.py
+-rw-r--r--   0 tom        (501) staff       (20)       81 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/array_api/constants.py
+-rw-r--r--   0 tom        (501) staff       (20)     8762 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/array_api/creation_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)      751 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/array_api/data_type_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)      471 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/array_api/dtypes.py
+-rw-r--r--   0 tom        (501) staff       (20)    11395 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/array_api/elementwise_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)       83 2023-02-16 11:53:37.000000 cubed-0.7.0/cubed/array_api/indexing_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)     4016 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/array_api/linear_algebra_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)     9144 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/array_api/manipulation_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)     1010 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/array_api/searching_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)     3693 2023-03-17 17:46:35.000000 cubed-0.7.0/cubed/array_api/statistical_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)      479 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/array_api/utility_functions.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.267608 cubed-0.7.0/cubed/core/
+-rw-r--r--   0 tom        (501) staff       (20)      431 2023-02-17 17:56:56.000000 cubed-0.7.0/cubed/core/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    12389 2023-05-25 11:00:24.000000 cubed-0.7.0/cubed/core/array.py
+-rw-r--r--   0 tom        (501) staff       (20)     5532 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/core/gufunc.py
+-rw-r--r--   0 tom        (501) staff       (20)    26890 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/core/ops.py
+-rw-r--r--   0 tom        (501) staff       (20)    11664 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/core/plan.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.268300 cubed-0.7.0/cubed/extensions/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/extensions/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3230 2023-05-25 11:00:24.000000 cubed-0.7.0/cubed/extensions/history.py
+-rw-r--r--   0 tom        (501) staff       (20)     2738 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/extensions/timeline.py
+-rw-r--r--   0 tom        (501) staff       (20)     1439 2023-02-16 11:53:37.000000 cubed-0.7.0/cubed/extensions/tqdm.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.268982 cubed-0.7.0/cubed/primitive/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/primitive/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    11045 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/primitive/blockwise.py
+-rw-r--r--   0 tom        (501) staff       (20)     2031 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/primitive/rechunk.py
+-rw-r--r--   0 tom        (501) staff       (20)      356 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/primitive/types.py
+-rw-r--r--   0 tom        (501) staff       (20)     1401 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/random.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.269852 cubed-0.7.0/cubed/runtime/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/runtime/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      953 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/runtime/backup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.271328 cubed-0.7.0/cubed/runtime/executors/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/runtime/executors/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     8292 2023-03-17 13:01:21.000000 cubed-0.7.0/cubed/runtime/executors/beam.py
+-rw-r--r--   0 tom        (501) staff       (20)     9240 2023-05-25 11:00:24.000000 cubed-0.7.0/cubed/runtime/executors/lithops.py
+-rw-r--r--   0 tom        (501) staff       (20)     3538 2023-05-25 11:00:24.000000 cubed-0.7.0/cubed/runtime/executors/modal.py
+-rw-r--r--   0 tom        (501) staff       (20)     6193 2023-05-25 11:00:24.000000 cubed-0.7.0/cubed/runtime/executors/modal_async.py
+-rw-r--r--   0 tom        (501) staff       (20)     1279 2023-02-16 11:53:37.000000 cubed-0.7.0/cubed/runtime/executors/python.py
+-rw-r--r--   0 tom        (501) staff       (20)     4241 2023-05-25 11:00:24.000000 cubed-0.7.0/cubed/runtime/executors/python_async.py
+-rw-r--r--   0 tom        (501) staff       (20)     3632 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/runtime/pipeline.py
+-rw-r--r--   0 tom        (501) staff       (20)      251 2023-03-17 13:01:21.000000 cubed-0.7.0/cubed/runtime/types.py
+-rw-r--r--   0 tom        (501) staff       (20)      118 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/runtime/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.273375 cubed-0.7.0/cubed/tests/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/tests/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.273887 cubed-0.7.0/cubed/tests/primitive/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/tests/primitive/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     6787 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/tests/primitive/test_blockwise.py
+-rw-r--r--   0 tom        (501) staff       (20)     2893 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/tests/primitive/test_rechunk.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.274635 cubed-0.7.0/cubed/tests/runtime/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/tests/runtime/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      860 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/tests/runtime/test_backup.py
+-rw-r--r--   0 tom        (501) staff       (20)     4014 2022-10-17 16:19:52.000000 cubed-0.7.0/cubed/tests/runtime/test_lithops.py
+-rw-r--r--   0 tom        (501) staff       (20)     4691 2023-03-27 13:45:10.000000 cubed-0.7.0/cubed/tests/runtime/test_modal_async.py
+-rw-r--r--   0 tom        (501) staff       (20)    16663 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/tests/test_array_api.py
+-rw-r--r--   0 tom        (501) staff       (20)    14506 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/tests/test_core.py
+-rw-r--r--   0 tom        (501) staff       (20)     3028 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/tests/test_gufunc.py
+-rw-r--r--   0 tom        (501) staff       (20)     1454 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/tests/test_indexing.py
+-rw-r--r--   0 tom        (501) staff       (20)     5287 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/tests/test_mem_utilization.py
+-rw-r--r--   0 tom        (501) staff       (20)     2397 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/tests/test_optimization.py
+-rw-r--r--   0 tom        (501) staff       (20)     1225 2023-05-25 08:48:11.000000 cubed-0.7.0/cubed/tests/test_random.py
+-rw-r--r--   0 tom        (501) staff       (20)     2310 2023-05-25 11:00:24.000000 cubed-0.7.0/cubed/tests/test_utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     2867 2023-05-25 11:00:24.000000 cubed-0.7.0/cubed/tests/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     4508 2023-05-25 11:00:24.000000 cubed-0.7.0/cubed/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.274872 cubed-0.7.0/cubed/vendor/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.7.0/cubed/vendor/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.275682 cubed-0.7.0/cubed/vendor/dask/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/dask/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.276741 cubed-0.7.0/cubed/vendor/dask/array/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/dask/array/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    17366 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/dask/array/core.py
+-rw-r--r--   0 tom        (501) staff       (20)     1685 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/dask/array/gufunc.py
+-rw-r--r--   0 tom        (501) staff       (20)     4670 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/dask/array/reshape.py
+-rw-r--r--   0 tom        (501) staff       (20)      543 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/dask/array/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)    14901 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/dask/blockwise.py
+-rw-r--r--   0 tom        (501) staff       (20)      608 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/dask/core.py
+-rw-r--r--   0 tom        (501) staff       (20)     2221 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/dask/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.277809 cubed-0.7.0/cubed/vendor/rechunker/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.7.0/cubed/vendor/rechunker/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    13197 2023-03-17 13:01:21.000000 cubed-0.7.0/cubed/vendor/rechunker/algorithm.py
+-rw-r--r--   0 tom        (501) staff       (20)    12312 2023-03-21 10:44:51.000000 cubed-0.7.0/cubed/vendor/rechunker/api.py
+-rw-r--r--   0 tom        (501) staff       (20)      309 2023-03-17 13:01:21.000000 cubed-0.7.0/cubed/vendor/rechunker/compat.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.278167 cubed-0.7.0/cubed/vendor/rechunker/executors/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.7.0/cubed/vendor/rechunker/executors/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      923 2023-03-17 13:01:21.000000 cubed-0.7.0/cubed/vendor/rechunker/executors/python.py
+-rw-r--r--   0 tom        (501) staff       (20)     3421 2023-03-17 13:01:21.000000 cubed-0.7.0/cubed/vendor/rechunker/types.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-25 11:02:26.263122 cubed-0.7.0/cubed.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)     1843 2023-05-25 11:02:26.000000 cubed-0.7.0/cubed.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     2506 2023-05-25 11:02:26.000000 cubed-0.7.0/cubed.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-05-25 11:02:26.000000 cubed-0.7.0/cubed.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)      369 2023-05-25 11:02:26.000000 cubed-0.7.0/cubed.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)        6 2023-05-25 11:02:26.000000 cubed-0.7.0/cubed.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)     1611 2023-05-25 11:01:22.000000 cubed-0.7.0/pyproject.toml
+-rw-r--r--   0 tom        (501) staff       (20)     1195 2023-05-25 11:02:26.279006 cubed-0.7.0/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      289 2023-05-16 07:59:53.000000 cubed-0.7.0/setup.py
```

### Comparing `cubed-0.6.3/LICENSE` & `cubed-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/PKG-INFO` & `cubed-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubed
-Version: 0.6.3
+Version: 0.7.0
 Summary: Bounded-memory serverless distributed N-dimensional array processing
 Author-email: Tom White <tom.e.white@gmail.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/tomwhite/cubed
 Project-URL: documentation, https://tomwhite.github.io/cubed
 Project-URL: repository, https://github.com/tomwhite/cubed
 Classifier: Development Status :: 3 - Alpha
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: diagnostics
 Provides-Extra: beam
 Provides-Extra: lithops
 Provides-Extra: modal
-Provides-Extra: complete
 Provides-Extra: test
 Provides-Extra: test-modal
 License-File: LICENSE
 
 # Cubed
 
 **_Note: this is a proof-of-concept, and many things are incomplete or don't work._**
```

### Comparing `cubed-0.6.3/README.md` & `cubed-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/__init__.py` & `cubed-0.7.0/cubed/__init__.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/array_api/__init__.py` & `cubed-0.7.0/cubed/array_api/__init__.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/array_api/array_object.py` & `cubed-0.7.0/cubed/array_api/array_object.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/array_api/creation_functions.py` & `cubed-0.7.0/cubed/array_api/creation_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     chunksize = to_chunksize(chunks)[0]
 
     return map_direct(
         _eye,
         shape=shape,
         dtype=dtype,
         chunks=chunks,
-        extra_required_mem=0,
+        extra_projected_mem=0,
         spec=spec,
         k=k,
         chunksize=chunksize,
     )
 
 
 def _eye(x, *arrays, k=None, chunksize=None, block_id=None):
@@ -186,15 +186,15 @@
         return asarray(0.0, dtype=dtype, spec=spec)
 
     return map_direct(
         _linspace,
         shape=shape,
         dtype=dtype,
         chunks=chunks,
-        extra_required_mem=0,
+        extra_projected_mem=0,
         spec=spec,
         size=chunksize,
         start=start,
         step=step,
         endpoint=endpoint,
         linspace_dtype=dtype,
     )
```

### Comparing `cubed-0.6.3/cubed/array_api/data_type_functions.py` & `cubed-0.7.0/cubed/array_api/data_type_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/array_api/elementwise_functions.py` & `cubed-0.7.0/cubed/array_api/elementwise_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/array_api/linear_algebra_functions.py` & `cubed-0.7.0/cubed/array_api/linear_algebra_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/array_api/manipulation_functions.py` & `cubed-0.7.0/cubed/array_api/manipulation_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,23 +94,23 @@
     shape = a.shape[:axis] + (offsets[-1],) + a.shape[axis + 1 :]
     dtype = a.dtype
     chunks = normalize_chunks(to_chunksize(a.chunks), shape=shape, dtype=dtype)
 
     # memory allocated by reading one chunk from input array
     # note that although the output chunk will overlap multiple input chunks,
     # the chunks are read in series, reusing memory
-    extra_required_mem = a.chunkmem
+    extra_projected_mem = a.chunkmem
 
     return map_direct(
         _read_concat_chunk,
         *arrays,
         shape=shape,
         dtype=dtype,
         chunks=chunks,
-        extra_required_mem=extra_required_mem,
+        extra_projected_mem=extra_projected_mem,
         axis=axis,
         offsets=offsets,
     )
 
 
 def _read_concat_chunk(x, *arrays, axis=None, offsets=None, block_id=None):
     # determine the start and stop indexes for this block along the axis dimension
@@ -165,23 +165,23 @@
         if len(axes) != x.ndim:
             raise ValueError("axes don't match array")
     else:
         axes = tuple(range(x.ndim))[::-1]
     axes = tuple(d + x.ndim if d < 0 else d for d in axes)
 
     # extra memory copy due to Zarr enforcing C order on transposed array
-    extra_required_mem = x.chunkmem
+    extra_projected_mem = x.chunkmem
     return blockwise(
         np.transpose,
         axes,
         x,
         tuple(range(x.ndim)),
         dtype=x.dtype,
         axes=axes,
-        extra_required_mem=extra_required_mem,
+        extra_projected_mem=extra_projected_mem,
     )
 
 
 def reshape(x, /, shape):
     # based on dask reshape
 
     known_sizes = [s for s in shape if s != -1]
@@ -219,23 +219,23 @@
 
     inchunks = normalize_chunks(x.chunks, shape=x.shape, dtype=x.dtype)
     outchunks = normalize_chunks(chunks, shape=shape, dtype=x.dtype)
 
     # TODO: check number of chunks is unchanged
 
     # memory allocated by reading one chunk from input array
-    extra_required_mem = x.chunkmem
+    extra_projected_mem = x.chunkmem
 
     return map_direct(
         _reshape_chunk,
         x,
         shape=shape,
         dtype=x.dtype,
         chunks=outchunks,
-        extra_required_mem=extra_required_mem,
+        extra_projected_mem=extra_projected_mem,
         inchunks=inchunks,
         outchunks=outchunks,
     )
 
 
 def _reshape_chunk(e, x, inchunks=None, outchunks=None, block_id=None):
     in_keys = list(product(*[range(len(c)) for c in inchunks]))
@@ -258,23 +258,23 @@
     axis = validate_axis(axis, a.ndim + 1)
     shape = a.shape[:axis] + (len(arrays),) + a.shape[axis:]
     dtype = a.dtype
     chunks = a.chunks[:axis] + ((1,) * len(arrays),) + a.chunks[axis:]
 
     # memory allocated by reading one chunk from an input array
     # (output is already catered for in blockwise)
-    extra_required_mem = a.chunkmem
+    extra_projected_mem = a.chunkmem
 
     return map_direct(
         _read_stack_chunk,
         *arrays,
         shape=shape,
         dtype=dtype,
         chunks=chunks,
-        extra_required_mem=extra_required_mem,
+        extra_projected_mem=extra_projected_mem,
         axis=axis,
     )
 
 
 def _read_stack_chunk(x, *arrays, axis=None, block_id=None):
     array = arrays[block_id[axis]]
     idx = tuple(v for i, v in enumerate(block_id) if i != axis)
```

### Comparing `cubed-0.6.3/cubed/array_api/searching_functions.py` & `cubed-0.7.0/cubed/array_api/searching_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/array_api/statistical_functions.py` & `cubed-0.7.0/cubed/array_api/statistical_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/core/array.py` & `cubed-0.7.0/cubed/core/array.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass
 from operator import mul
 from typing import Optional, TypeVar
+from warnings import warn
 
 import numpy as np
 from toolz import map, reduce
 
 from cubed.runtime.pipeline import already_computed
 from cubed.runtime.types import Executor
 from cubed.utils import chunk_memory
@@ -37,17 +38,19 @@
         self.name = name
         self.zarray = zarray
         self._shape = zarray.shape
         self._dtype = zarray.dtype
         self._chunks = normalize_chunks(
             zarray.chunks, shape=self.shape, dtype=self.dtype
         )
-        # if no spec is supplied, use a default with local temp dir, a modest amount of memory (100MB),
-        # and a conservative amount of reserved memory (200MB)
-        self.spec = spec or Spec(None, max_mem=100_000_000, reserved_mem=200_000_000)
+        # if no spec is supplied, use a default with local temp dir,
+        # and a modest amount of memory (200MB, of which 100MB is reserved)
+        self.spec = spec or Spec(
+            None, allowed_mem=200_000_000, reserved_mem=100_000_000
+        )
         self.plan = plan
 
     @property
     def chunkmem(self):
         """Amount of memory in bytes that a single chunk uses."""
         return chunk_memory(self.dtype, self.chunksize)
 
@@ -187,30 +190,43 @@
 class Spec:
     """Specification of resources available to run a computation."""
 
     work_dir: Optional[str] = None
     """The directory path (specified as an fsspec URL) used for storing intermediate data."""
 
     max_mem: Optional[int] = None
-    """The maximum memory available to a worker for data use for the computation, in bytes."""
+    """**Deprecated**. The maximum memory available to a worker for data use for the computation, in bytes."""
+
+    allowed_mem: Optional[int] = None
+    """The total memory available to a worker for running a task, in bytes.
 
-    reserved_mem: Optional[int] = None
-    """The memory reserved on a worker for non-data use, in bytes.
+    This includes any ``reserved_mem`` that has been set."""
 
-    The sum of ``max_mem`` and ``reserved_mem`` should not exceed the total memory of the worker.
+    reserved_mem: int = 0
+    """The memory reserved on a worker for non-data use when running a task, in bytes.
 
     See ``cubed.measure_reserved_memory``.
     """
 
     executor: Executor = None
     """The default executor for running computations."""
 
     storage_options: dict = None  # type: ignore[assignment]
     """Storage options to be passed to fsspec"""
 
+    def __post_init__(self):
+        if self.max_mem is not None:
+            warn(
+                "`max_mem` is deprecated, please use `allowed_mem` instead",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+        if self.allowed_mem is None:
+            self.allowed_mem = (self.max_mem or 0) + self.reserved_mem
+
 
 class Callback:
     """Object to receive callback events during array computation."""
 
     def on_compute_start(self, dag):
         """Called when the computation is about to start.
 
@@ -260,19 +276,19 @@
 
     function_end_tstamp: Optional[float] = None
     """Timestamp of when the function finished executing on the remote worker."""
 
     task_result_tstamp: Optional[float] = None
     """Timestamp of when the result of the task was received by the client."""
 
-    peak_memory_start: Optional[int] = None
-    """Peak memory usage on the remote worker before the function starts executing."""
+    peak_measured_mem_start: Optional[int] = None
+    """Peak memory usage measured on the remote worker before the function starts executing."""
 
-    peak_memory_end: Optional[int] = None
-    """Peak memory usage on the remote worker after the function finishes executing."""
+    peak_measured_mem_end: Optional[int] = None
+    """Peak memory usage measured on the remote worker after the function finishes executing."""
 
 
 def check_array_specs(arrays):
     specs = [a.spec for a in arrays if hasattr(a, "spec")]
     if not all(s == specs[0] for s in specs):
         raise ValueError(
             f"Arrays must have same spec in single computation. Specs: {specs}"
@@ -333,17 +349,17 @@
     """
     plan = arrays_to_plan(*arrays)
     return plan.visualize(
         filename=filename, format=format, optimize_graph=optimize_graph
     )
 
 
-class PeakMemoryCallback(Callback):
+class PeakMeasuredMemoryCallback(Callback):
     def on_task_end(self, event):
-        self.peak_memory = event.peak_memory_end
+        self.peak_measured_mem = event.peak_measured_mem_end
 
 
 def measure_reserved_memory(executor):
     """Measures the reserved memory use for a given executor runtime.
 
     This is the memory used by the Python process for running a task,
     excluding any memory used for data for the computation. It can vary by
@@ -366,10 +382,10 @@
     int
         The memory used by the runtime in bytes.
     """
     import cubed.array_api as xp
 
     a = xp.ones((1,))
     b = xp.negative(a)
-    peak_memory_callback = PeakMemoryCallback()
-    b.compute(executor=executor, callbacks=[peak_memory_callback])
-    return peak_memory_callback.peak_memory
+    peak_measured_mem_callback = PeakMeasuredMemoryCallback()
+    b.compute(executor=executor, callbacks=[peak_measured_mem_callback])
+    return peak_measured_mem_callback.peak_measured_mem
```

### Comparing `cubed-0.6.3/cubed/core/gufunc.py` & `cubed-0.7.0/cubed/core/gufunc.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     `equivalent function <https://docs.dask.org/en/stable/generated/dask.array.gufunc.apply_gufunc.html>`_
     in Dask. Refer there for usage information.
 
     Current limitations: ``keepdims``, and ``allow_rechunk`` are not supported;
     and multiple outputs are not supported.
 
     Cubed assumes that ``func`` will allocate a new output array. However, if it allocates more memory
-    than than, then you need to tell Cubed about it by setting the ``extra_required_mem`` parameter
+    than than, then you need to tell Cubed about it by setting the ``extra_projected_mem`` parameter
     to the amount needed in bytes (per task).
     """
 
     # Currently the following parameters cannot be changed
     # keepdims = False
     allow_rechunk = False
```

### Comparing `cubed-0.6.3/cubed/core/ops.py` & `cubed-0.7.0/cubed/core/ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     return map_direct(
         _from_array,
         x,
         shape=x.shape,
         dtype=x.dtype,
         chunks=outchunks,
-        extra_required_mem=0,
+        extra_projected_mem=0,
         spec=spec,
         outchunks=outchunks,
         asarray=asarray,
     )
 
 
 def _from_array(e, x, outchunks=None, asarray=None, block_id=None):
@@ -252,40 +252,42 @@
     zargs = list(args)
     zargs[::2] = [a.zarray for a in arrays]
     in_names = [a.name for a in arrays]
 
     extra_source_arrays = kwargs.pop("extra_source_arrays", [])
     source_arrays = list(arrays) + list(extra_source_arrays)
 
-    extra_required_mem = kwargs.pop("extra_required_mem", 0)
+    extra_projected_mem = kwargs.pop("extra_projected_mem", 0)
 
     name = gensym()
     spec = check_array_specs(arrays)
     if target_store is None:
         target_store = new_temp_store(name=name, spec=spec)
     pipeline = primitive_blockwise(
         func,
         out_ind,
         *zargs,
-        max_mem=spec.max_mem,
+        allowed_mem=spec.allowed_mem,
+        reserved_mem=spec.reserved_mem,
         target_store=target_store,
         shape=shape,
         dtype=dtype,
         chunks=_chunks,
         new_axes=new_axes,
         in_names=in_names,
         out_name=name,
         **kwargs,
     )
     plan = Plan._new(
         name,
         "blockwise",
         pipeline.target_array,
         pipeline,
-        pipeline.required_mem + extra_required_mem,
+        pipeline.projected_mem + extra_projected_mem,
+        spec.reserved_mem,
         pipeline.num_tasks,
         *source_arrays,
     )
     from cubed.array_api import Array
 
     return Array(name, pipeline.target_array, spec, plan)
 
@@ -353,23 +355,23 @@
     where_list = [i for i, ind in enumerate(selection) if is_integer_list(ind)]
     if len(where_list) > 1:
         raise NotImplementedError("Only one integer array index is allowed.")
 
     # memory allocated by reading one chunk from input array
     # note that although the output chunk will overlap multiple input chunks, zarr will
     # read the chunks in series, reusing the buffer
-    extra_required_mem = x.chunkmem
+    extra_projected_mem = x.chunkmem
 
     out = map_direct(
         _read_index_chunk,
         x,
         shape=shape,
         dtype=dtype,
         chunks=chunks,
-        extra_required_mem=extra_required_mem,
+        extra_projected_mem=extra_projected_mem,
         target_chunks=chunks,
         selection=selection,
     )
 
     for axis in where_none:
         from cubed.array_api.manipulation_functions import expand_dims
 
@@ -526,15 +528,15 @@
         new_axes=new_axes,
         align_arrays=False,
         **kwargs,
     )
 
 
 def map_direct(
-    func, *args: "Array", shape, dtype, chunks, extra_required_mem, spec=None, **kwargs
+    func, *args: "Array", shape, dtype, chunks, extra_projected_mem, spec=None, **kwargs
 ) -> "Array":
     """
     Map a function across blocks of a new array, using side-input arrays to read directly from.
 
     Parameters
     ----------
     func : callable
@@ -544,17 +546,17 @@
         The side-input arrays that may be accessed directly in the function.
     shape : tuple
         Shape of the output array.
     dtype : np.dtype
         The ``dtype`` of the output array.
     chunks : tuple
         Chunk shape of blocks in the output array.
-    extra_required_mem : int
-        Extra memory required (in bytes) for each map task. This should take into account the
-        memory requirements for any reads from the side-input arrays (``args``).
+    extra_projected_mem : int
+        Extra memory projected to be needed (in bytes) for each map task. This should take into account the
+        memory allocations for any reads from the side-input arrays (``args``).
     spec : Spec
         Specification for the new array. If not specified, the one from the first side input
         (`args`) will be used (if any).
     """
 
     from cubed.array_api.creation_functions import empty
 
@@ -575,15 +577,15 @@
 
     return map_blocks(
         new_func(func),
         out,
         dtype=dtype,
         chunks=chunks,
         extra_source_arrays=args,
-        extra_required_mem=extra_required_mem,
+        extra_projected_mem=extra_projected_mem,
         **kwargs,
     )
 
 
 def rechunk(x, chunks, target_store=None):
     if x.chunks == normalize_chunks(chunks, x.shape, dtype=x.dtype):
         return x
@@ -591,24 +593,26 @@
     spec = x.spec
     if target_store is None:
         target_store = new_temp_store(name=name, spec=spec)
     temp_store = new_temp_store(name=f"{name}-intermediate", spec=spec)
     pipeline = primitive_rechunk(
         x.zarray,
         target_chunks=chunks,
-        max_mem=spec.max_mem,
+        allowed_mem=spec.allowed_mem,
+        reserved_mem=spec.reserved_mem,
         target_store=target_store,
         temp_store=temp_store,
     )
     plan = Plan._new(
         name,
         "rechunk",
         pipeline.target_array,
         pipeline,
-        pipeline.required_mem,
+        pipeline.projected_mem,
+        spec.reserved_mem,
         pipeline.num_tasks,
         x,
     )
 
     from cubed.array_api import Array
 
     return Array(name, pipeline.target_array, spec, plan)
@@ -633,15 +637,16 @@
     axis = validate_axis(axis, x.ndim)
     if intermediate_dtype is None:
         intermediate_dtype = dtype
 
     inds = tuple(range(x.ndim))
 
     result = x
-    max_mem = x.spec.max_mem
+    allowed_mem = x.spec.allowed_mem
+    max_mem = allowed_mem - x.spec.reserved_mem
 
     # reduce initial chunks (if any axis chunksize is > 1)
     if (
         any(s > 1 for i, s in enumerate(result.chunksize) if i in axis)
         or func != combine_func
     ):
         args = (result, inds)
@@ -672,15 +677,15 @@
                     target_chunks[i] = min(s, x.chunksize[i])
                 else:
                     # single axis: see how many result chunks fit in max_mem
                     # factor of 4 is memory for {compressed, uncompressed} x {input, output} (see rechunk.py)
                     target_chunk_size = (max_mem - chunk_mem) // (chunk_mem * 4)
                     if target_chunk_size <= 1:
                         raise ValueError(
-                            f"Not enough memory for reduction. Increase max_mem ({max_mem}) or decrease chunk size"
+                            f"Not enough memory for reduction. Increase allowed_mem ({allowed_mem}) or decrease chunk size"
                         )
                     target_chunks[i] = min(s, target_chunk_size)
         _target_chunks = tuple(target_chunks)
         result = rechunk(result, _target_chunks)
 
         # reduce chunks (if any axis chunksize is > 1)
         if any(s > 1 for i, s in enumerate(result.chunksize) if i in axis):
```

### Comparing `cubed-0.6.3/cubed/core/plan.py` & `cubed-0.7.0/cubed/core/plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     @classmethod
     def _new(
         cls,
         name,
         op_name,
         target,
         pipeline=None,
-        required_mem=None,
+        projected_mem=None,
+        reserved_mem=None,
         num_tasks=None,
         *source_arrays,
     ):
         # create an empty DAG or combine from sources
         if len(source_arrays) == 0:
             dag = nx.MultiDiGraph()
         else:
@@ -68,15 +69,16 @@
             dag.add_node(
                 name,
                 name=name,
                 op_name=op_name,
                 target=target,
                 stack_summaries=stack_summaries,
                 pipeline=pipeline,
-                required_mem=required_mem,
+                projected_mem=projected_mem,
+                reserved_mem=reserved_mem,
                 num_tasks=num_tasks,
             )
         for x in source_arrays:
             if hasattr(x, "name"):
                 dag.add_edge(x.name, name)
 
         return Plan(dag)
@@ -166,31 +168,31 @@
             for stage in pipeline.stages:
                 if stage.mappable is not None:
                     tasks += len(list(stage.mappable))
                 else:
                     tasks += 1
         return tasks
 
-    def max_required_mem(self, optimize_graph=True):
-        """Return the maximum required memory (for a task) to execute this plan."""
+    def max_projected_mem(self, optimize_graph=True):
+        """Return the maximum projected memory across all tasks to execute this plan."""
         dag = self.optimize().dag if optimize_graph else self.dag.copy()
-        required_mem_values = [
-            node["pipeline"].required_mem for _, node in visit_nodes(dag)
+        projected_mem_values = [
+            node["pipeline"].projected_mem for _, node in visit_nodes(dag)
         ]
-        return max(required_mem_values) if len(required_mem_values) > 0 else 0
+        return max(projected_mem_values) if len(projected_mem_values) > 0 else 0
 
     def visualize(
         self, filename="cubed", format=None, rankdir="TB", optimize_graph=True
     ):
         dag = self.optimize().dag if optimize_graph else self.dag.copy()
         dag.graph["graph"] = {
             "rankdir": rankdir,
             "label": (
                 f"num tasks: {self.num_tasks(optimize_graph=optimize_graph)}\n"
-                f"max required memory: {memory_repr(self.max_required_mem(optimize_graph=optimize_graph))}"
+                f"max projected memory: {memory_repr(self.max_projected_mem(optimize_graph=optimize_graph))}"
             ),
             "labelloc": "bottom",
             "labeljust": "left",
             "fontsize": "10",
         }
         dag.graph["node"] = {"fontname": "helvetica", "shape": "box", "fontsize": "10"}
         for (n, d) in dag.nodes(data=True):
@@ -210,15 +212,15 @@
                 f"shape: {target.shape}\n"
                 f"chunks: {target.chunks}\n"
                 f"dtype: {target.dtype}\n"
                 f"chunk memory: {chunkmem}\n"
             )
             if "pipeline" in d:
                 pipeline = d["pipeline"]
-                tooltip += f"\ntask memory: {memory_repr(pipeline.required_mem)}"
+                tooltip += f"\nprojected memory: {memory_repr(pipeline.projected_mem)}"
                 tooltip += f"\ntasks: {pipeline.num_tasks}"
             if "stack_summaries" in d:
                 # add call stack information
                 stack_summaries = d["stack_summaries"]
 
                 first_cubed_i = min(
                     i for i, s in enumerate(stack_summaries) if s.is_cubed()
```

### Comparing `cubed-0.6.3/cubed/extensions/timeline.py` & `cubed-0.7.0/cubed/extensions/timeline.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/extensions/tqdm.py` & `cubed-0.7.0/cubed/extensions/tqdm.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/primitive/blockwise.py` & `cubed-0.7.0/cubed/primitive/blockwise.py`

 * *Files 9% similar despite different names*

```diff
@@ -77,15 +77,16 @@
     return get_item(chunks, key)
 
 
 def blockwise(
     func,
     out_ind,
     *args,
-    max_mem,
+    allowed_mem,
+    reserved_mem,
     target_store,
     shape,
     dtype,
     chunks,
     new_axes=None,
     in_names=None,
     out_name=None,
@@ -97,16 +98,18 @@
     ----------
     func : callable
         Function to apply to individual tuples of blocks
     out_ind : iterable
         Block pattern of the output, something like 'ijk' or (1, 2, 3)
     *args : sequence of Array, index pairs
         Sequence like (x, 'ij', y, 'jk', z, 'i')
-    max_mem : int
-        Maximum memory allowed for a single task of this operation, measured in bytes
+    allowed_mem : int
+        The memory available to a worker for running a task, in bytes. Includes ``reserved_mem``.
+    reserved_mem : int
+        The memory reserved on a worker for non-data use when running a task, in bytes
     target_store : string or zarr.Array
         Path to output Zarr store, or Zarr array
     shape : tuple
         The shape of the output array.
     dtype : np.dtype
         The ``dtype`` of the output array.
     chunks : tuple
@@ -114,17 +117,15 @@
     new_axes : dict
         New indexes and their dimension lengths
     **kwargs : dict
         Extra keyword arguments to pass to function
 
     Returns
     -------
-    pipeline:  Pipeline to run the operation
-    target:  ArrayProxy for the Zarr array output
-    required_mem: minimum memory required per-task, in bytes
+    CubedPipeline to run the operation
     """
 
     # Use dask's make_blockwise_graph
     arrays = args[::2]
     array_names = in_names or [f"in_{i}" for i in range(len(arrays))]
     array_map = {name: array for name, array in zip(array_names, arrays)}
 
@@ -185,37 +186,37 @@
         Stage(
             apply_blockwise,
             gensym("apply_blockwise"),
             mappable=output_blocks,
         )
     ]
 
-    # calculate memory requirement
-    required_mem = 0
+    # calculate projected memory
+    projected_mem = reserved_mem
     # inputs
     for array in arrays:  # inputs
         # memory for a compressed and an uncompressed input array chunk
         # - we assume compression has no effect (so it's an overestimate)
         # - ideally we'd be able to look at nbytes_stored,
         #   but this is not possible in general since the array has not been written yet
-        required_mem += chunk_memory(array.dtype, array.chunks) * 2
+        projected_mem += chunk_memory(array.dtype, array.chunks) * 2
     # output
     # memory for a compressed and an uncompressed output array chunk
     # - this assumes the blockwise function creates a new array)
     # - numcodecs uses a working output buffer that's the size of the array being compressed
-    required_mem += chunk_memory(dtype, chunksize) * 2
+    projected_mem += chunk_memory(dtype, chunksize) * 2
 
-    if required_mem > max_mem:
+    if projected_mem > allowed_mem:
         raise ValueError(
-            f"Blockwise memory ({required_mem}) exceeds max_mem ({max_mem})"
+            f"Projected blockwise memory ({projected_mem}) exceeds allowed_mem ({allowed_mem}), including reserved_mem ({reserved_mem})"
         )
 
     num_tasks = len(output_blocks)
 
-    return CubedPipeline(stages, spec, target_array, required_mem, num_tasks)
+    return CubedPipeline(stages, spec, target_array, projected_mem, num_tasks)
 
 
 # Code for fusing pipelines
 
 
 def is_fuse_candidate(pipeline):
     """
@@ -257,18 +258,18 @@
         return pipeline2.config.function(pipeline1.config.function(*args))
 
     read_proxies = pipeline1.config.reads_map
     write_proxy = pipeline2.config.write
     spec = BlockwiseSpec(fused_blockwise_func, fused_func, read_proxies, write_proxy)
 
     target_array = pipeline2.target_array
-    required_mem = max(pipeline1.required_mem, pipeline2.required_mem)
+    projected_mem = max(pipeline1.projected_mem, pipeline2.projected_mem)
     num_tasks = pipeline2.num_tasks
 
-    return CubedPipeline(stages, spec, target_array, required_mem, num_tasks)
+    return CubedPipeline(stages, spec, target_array, projected_mem, num_tasks)
 
 
 # blockwise functions
 
 
 def make_blockwise_function(
     func, output, out_indices, *arrind_pairs, numblocks=None, new_axes=None
```

### Comparing `cubed-0.6.3/cubed/primitive/rechunk.py` & `cubed-0.7.0/cubed/primitive/rechunk.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 from math import ceil, prod
 
 from cubed.runtime.pipeline import spec_to_pipeline
 from cubed.vendor.rechunker.api import _setup_rechunk
 
 
-def rechunk(source, target_chunks, max_mem, target_store, temp_store=None):
+def rechunk(
+    source, target_chunks, allowed_mem, reserved_mem, target_store, temp_store=None
+):
     """Rechunk a Zarr array to have target_chunks.
 
     Parameters
     ----------
     source : Zarr array
     target_chunks : tuple
         The desired chunks of the array after rechunking.
-    max_mem : int
-        Maximum memory allowed for a single task of this operation, measured in bytes
+    allowed_mem : int
+        The memory available to a worker for running a task, in bytes. Includes ``reserved_mem``.
+    reserved_mem : int
+        The memory reserved on a worker for non-data use when running a task, in bytes
     target_store : str
         Path to output Zarr store.
     temp_store : str, optional
         Path to temporary store for intermediate data.
 
     Returns
     -------
-    pipeline:  Pipeline to run the operation
-    target:  Array for the Zarr array output
-    required_mem: minimum memory required per-task, in bytes
+    CubedPipeline to run the operation
     """
 
     # rechunker doesn't take account of uncompressed and compressed copies of the
     # input and output array chunk/selection, so adjust appropriately
-    adjusted_max_mem = max_mem / 4
+    rechunker_max_mem = (allowed_mem - reserved_mem) / 4
 
     copy_specs, intermediate, target = _setup_rechunk(
         source=source,
         target_chunks=target_chunks,
-        max_mem=adjusted_max_mem,
+        max_mem=rechunker_max_mem,
         target_store=target_store,
         temp_store=temp_store,
     )
 
     # source is a Zarr array, so only a single copy spec
     if len(copy_specs) != 1:  # pragma: no cover
         raise ValueError(f"Source must be a Zarr array, but was {source}")
     copy_spec = copy_specs[0]
 
     num_tasks = total_chunks(copy_spec.write.array.shape, copy_spec.write.chunks)
     if intermediate is not None:
         num_tasks += total_chunks(copy_spec.read.array.shape, copy_spec.read.chunks)
 
-    return spec_to_pipeline(copy_spec, target, max_mem, num_tasks)
+    # we assume that rechunker is going to use all the memory it is allowed to
+    projected_mem = allowed_mem
+    return spec_to_pipeline(copy_spec, target, projected_mem, num_tasks)
 
 
 def total_chunks(shape, chunks):
     # cf rechunker's chunk_keys
     return prod(ceil(s / c) for s, c in zip(shape, chunks))
```

### Comparing `cubed-0.6.3/cubed/random.py` & `cubed-0.7.0/cubed/random.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,24 +13,24 @@
     """Return random floats in the half-open interval [0.0, 1.0)."""
     shape = normalize_shape(size)
     dtype = nxp.float64
     chunks = normalize_chunks(chunks, shape=shape, dtype=dtype)
     numblocks = tuple(map(len, chunks))
     root_seed = pyrandom.getrandbits(128)
 
-    # no extra memory required since input is an empty array whose
+    # no extra memory is projected to be needed since input is an empty array whose
     # memory is never allocated, see https://pythonspeed.com/articles/measuring-memory-python/#phantom-memory
-    extra_required_mem = 0
+    extra_projected_mem = 0
 
     return map_direct(
         _random,
         shape=shape,
         dtype=dtype,
         chunks=chunks,
-        extra_required_mem=extra_required_mem,
+        extra_projected_mem=extra_projected_mem,
         spec=spec,
         numblocks=numblocks,
         root_seed=root_seed,
     )
 
 
 def _random(x, *arrays, numblocks=None, root_seed=None, block_id=None):
```

### Comparing `cubed-0.6.3/cubed/runtime/backup.py` & `cubed-0.7.0/cubed/runtime/backup.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/runtime/executors/beam.py` & `cubed-0.7.0/cubed/runtime/executors/beam.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/runtime/executors/lithops.py` & `cubed-0.7.0/cubed/runtime/executors/lithops.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,16 +196,16 @@
 def lithops_stats_to_task_end_event(name, stats):
     return TaskEndEvent(
         array_name=name,
         task_create_tstamp=stats["host_job_create_tstamp"],
         function_start_tstamp=stats["worker_func_start_tstamp"],
         function_end_tstamp=stats["worker_func_end_tstamp"],
         task_result_tstamp=stats["host_status_done_tstamp"],
-        peak_memory_start=stats["worker_peak_memory_start"],
-        peak_memory_end=stats["worker_peak_memory_end"],
+        peak_measured_mem_start=stats["worker_peak_memory_start"],
+        peak_measured_mem_end=stats["worker_peak_memory_end"],
     )
 
 
 def build_stage_mappable_func(
     stage, config, name=None, callbacks=None, use_backups=False
 ):
     def sf(mappable):
```

### Comparing `cubed-0.6.3/cubed/runtime/executors/modal.py` & `cubed-0.7.0/cubed/runtime/executors/modal.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import modal
 from modal.exception import ConnectionError
 from tenacity import retry, retry_if_exception_type, stop_after_attempt
 
 from cubed.core.array import TaskEndEvent
 from cubed.core.plan import visit_nodes
 from cubed.runtime.types import DagExecutor
-from cubed.utils import peak_memory
+from cubed.utils import peak_measured_mem
 
 stub = modal.Stub()
 
 requirements_file = os.getenv("CUBED_MODAL_REQUIREMENTS_FILE")
 
 if requirements_file:
     image = modal.Image.debian_slim().pip_install_from_requirements(requirements_file)
@@ -39,25 +39,25 @@
     secret=modal.Secret.from_name("my-aws-secret"),
     memory=2000,
     retries=2,
     is_generator=True,
 )
 def run_remotely(input, func=None, config=None):
     print(f"running remotely on {input}")
-    peak_memory_start = peak_memory()
+    peak_measured_mem_start = peak_measured_mem()
     function_start_tstamp = time.time()
     result = func(input, config=config)
     function_end_tstamp = time.time()
-    peak_memory_end = peak_memory()
+    peak_measured_mem_end = peak_measured_mem()
     yield (
         result,
         function_start_tstamp,
         function_end_tstamp,
-        peak_memory_start,
-        peak_memory_end,
+        peak_measured_mem_start,
+        peak_measured_mem_end,
     )
 
 
 # This just retries the initial connection attempt, not the function calls
 @retry(
     retry=retry_if_exception_type((TimeoutError, ConnectionError)),
     stop=stop_after_attempt(3),
@@ -82,24 +82,24 @@
 def handle_callbacks(callbacks, array_name, result, task_create_tstamp):
     if callbacks is not None:
         task_result_tstamp = time.time()
         (
             res,
             function_start_tstamp,
             function_end_tstamp,
-            peak_memory_start,
-            peak_memory_end,
+            peak_measured_mem_start,
+            peak_measured_mem_end,
         ) = result
         task_stats = dict(
             task_create_tstamp=task_create_tstamp,
             function_start_tstamp=function_start_tstamp,
             function_end_tstamp=function_end_tstamp,
             task_result_tstamp=task_result_tstamp,
-            peak_memory_start=peak_memory_start,
-            peak_memory_end=peak_memory_end,
+            peak_measured_mem_start=peak_measured_mem_start,
+            peak_measured_mem_end=peak_measured_mem_end,
         )
         event = TaskEndEvent(array_name=array_name, **task_stats)
         [callback.on_task_end(event) for callback in callbacks]
 
 
 class ModalDagExecutor(DagExecutor):
     """An execution engine that uses Modal."""
```

### Comparing `cubed-0.6.3/cubed/runtime/executors/modal_async.py` & `cubed-0.7.0/cubed/runtime/executors/modal_async.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from modal.exception import ConnectionError
 from tenacity import retry, retry_if_exception_type, stop_after_attempt
 
 from cubed.core.array import TaskEndEvent
 from cubed.core.plan import visit_nodes
 from cubed.runtime.backup import should_launch_backup
 from cubed.runtime.types import DagExecutor
-from cubed.utils import peak_memory
+from cubed.utils import peak_measured_mem
 
 async_stub = modal.aio.AioStub()
 
 requirements_file = os.getenv("CUBED_MODAL_REQUIREMENTS_FILE")
 
 if requirements_file:
     image = modal.Image.debian_slim().pip_install_from_requirements(requirements_file)
@@ -41,25 +41,25 @@
     secret=modal.Secret.from_name("my-aws-secret"),
     memory=2000,
     retries=2,
     is_generator=True,
 )
 async def async_run_remotely(input, func=None, config=None):
     print(f"running remotely on {input}")
-    peak_memory_start = peak_memory()
+    peak_measured_mem_start = peak_measured_mem()
     function_start_tstamp = time.time()
     result = func(input, config=config)
     function_end_tstamp = time.time()
-    peak_memory_end = peak_memory()
+    peak_measured_mem_end = peak_measured_mem()
     yield (
         result,
         function_start_tstamp,
         function_end_tstamp,
-        peak_memory_start,
-        peak_memory_end,
+        peak_measured_mem_start,
+        peak_measured_mem_end,
     )
 
 
 # We need map_unordered for the use_backups implementation
 async def map_unordered(
     app_function, input, max_failures=3, use_backups=False, **kwargs
 ):
@@ -152,24 +152,24 @@
 def handle_callbacks(callbacks, array_name, result, task_create_tstamp):
     if callbacks is not None:
         task_result_tstamp = time.time()
         (
             res,
             function_start_tstamp,
             function_end_tstamp,
-            peak_memory_start,
-            peak_memory_end,
+            peak_measured_mem_start,
+            peak_measured_mem_end,
         ) = result
         task_stats = dict(
             task_create_tstamp=task_create_tstamp,
             function_start_tstamp=function_start_tstamp,
             function_end_tstamp=function_end_tstamp,
             task_result_tstamp=task_result_tstamp,
-            peak_memory_start=peak_memory_start,
-            peak_memory_end=peak_memory_end,
+            peak_measured_mem_start=peak_measured_mem_start,
+            peak_measured_mem_end=peak_measured_mem_end,
         )
         event = TaskEndEvent(array_name=array_name, **task_stats)
         [callback.on_task_end(event) for callback in callbacks]
 
 
 class AsyncModalDagExecutor(DagExecutor):
     """An execution engine that uses Modal's async API."""
```

### Comparing `cubed-0.6.3/cubed/runtime/executors/python.py` & `cubed-0.7.0/cubed/runtime/executors/python.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/runtime/executors/python_async.py` & `cubed-0.7.0/cubed/runtime/executors/python_async.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 
 from aiostream import stream
 from tenacity import retry, stop_after_attempt
 
 from cubed.core.array import TaskEndEvent
 from cubed.core.plan import visit_node_generations
 from cubed.runtime.types import DagExecutor
-from cubed.utils import peak_memory
+from cubed.utils import peak_measured_mem
 
 
 def execution_stats(func):
     """Measure timing information and peak memory usage of a function call."""
 
     def wrapper(*args, **kwargs):
-        peak_memory_start = peak_memory()
+        peak_measured_mem_start = peak_measured_mem()
         function_start_tstamp = time.time()
         result = func(*args, **kwargs)
         function_end_tstamp = time.time()
-        peak_memory_end = peak_memory()
+        peak_measured_mem_end = peak_measured_mem()
         return result, dict(
             function_start_tstamp=function_start_tstamp,
             function_end_tstamp=function_end_tstamp,
-            peak_memory_start=peak_memory_start,
-            peak_memory_end=peak_memory_end,
+            peak_measured_mem_start=peak_measured_mem_start,
+            peak_measured_mem_end=peak_measured_mem_end,
         )
 
     return wrapper
 
 
 @retry(stop=stop_after_attempt(3))
 @execution_stats
```

### Comparing `cubed-0.6.3/cubed/runtime/pipeline.py` & `cubed-0.7.0/cubed/runtime/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     if isinstance(chunk_key, list):
         chunk_key = tuple(chunk_key)
     data = np.asarray(config.intermediate.array[chunk_key])
     config.write.array[chunk_key] = data
 
 
 def spec_to_pipeline(
-    spec: CopySpec, target_array: Any, max_mem: int, num_tasks: int
+    spec: CopySpec, target_array: Any, projected_mem: int, num_tasks: int
 ) -> CubedPipeline:
     # typing won't work until we start using numpy types
     shape = spec.read.array.shape  # type: ignore
     if spec.intermediate.array is None:
         stages = [
             Stage(
                 copy_read_to_write,
@@ -84,15 +84,15 @@
             ),
             Stage(
                 copy_intermediate_to_write,
                 gensym("copy_intermediate_to_write"),
                 mappable=ChunkKeys(shape, spec.write.chunks),
             ),
         ]
-    return CubedPipeline(stages, spec, target_array, max_mem, num_tasks)
+    return CubedPipeline(stages, spec, target_array, projected_mem, num_tasks)
 
 
 def already_computed(node_dict):
     """
     Return True if the array for a node doesn't have a pipeline to compute it,
     or it has already been computed (all chunks are present).
     """
```

### Comparing `cubed-0.6.3/cubed/tests/primitive/test_blockwise.py` & `cubed-0.7.0/cubed/tests/primitive/test_blockwise.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,45 +10,48 @@
 
 
 @pytest.fixture(scope="module", params=[PythonPipelineExecutor()])
 def executor(request):
     return request.param
 
 
-def test_blockwise(tmp_path, executor):
+@pytest.mark.parametrize("reserved_mem", [0, 100])
+def test_blockwise(tmp_path, executor, reserved_mem):
     source1 = create_zarr(
         [0, 1, 2], dtype=int, chunks=2, store=tmp_path / "source1.zarr"
     )
     source2 = create_zarr(
         [10, 50, 100], dtype=int, chunks=2, store=tmp_path / "source2.zarr"
     )
-    max_mem = 1000
+    allowed_mem = 1000
     target_store = tmp_path / "target.zarr"
 
     pipeline = blockwise(
         np.outer,
         "ij",
         source1,
         "i",
         source2,
         "j",
-        max_mem=max_mem,
+        allowed_mem=allowed_mem,
+        reserved_mem=reserved_mem,
         target_store=target_store,
         shape=(3, 3),
         dtype=int,
         chunks=(2, 2),
     )
 
     assert pipeline.target_array.shape == (3, 3)
     assert pipeline.target_array.dtype == int
     assert pipeline.target_array.chunks == (2, 2)
 
     itemsize = np.dtype(int).itemsize
-    assert pipeline.required_mem == (
-        (itemsize * 2)  # source1 compressed chunk
+    assert pipeline.projected_mem == (
+        reserved_mem  # projected includes reserved
+        + (itemsize * 2)  # source1 compressed chunk
         + (itemsize * 2)  # source1 uncompressed chunk
         + (itemsize * 2)  # source2 compressed chunk
         + (itemsize * 2)  # source2 uncompressed chunk
         + (itemsize * 2 * 2)  # output compressed chunk
         + (itemsize * 2 * 2)  # output uncompressed chunk
     )
 
@@ -56,28 +59,29 @@
 
     execute_pipeline(pipeline, executor=executor)
 
     res = zarr.open(target_store)
     assert_array_equal(res[:], np.outer([0, 1, 2], [10, 50, 100]))
 
 
-def _permute_dims(x, /, axes, max_mem, target_store):
+def _permute_dims(x, /, axes, allowed_mem, reserved_mem, target_store):
     # From dask transpose
     if axes:
         if len(axes) != x.ndim:
             raise ValueError("axes don't match array")
     else:
         axes = tuple(range(x.ndim))[::-1]
     axes = tuple(d + x.ndim if d < 0 else d for d in axes)
     return blockwise(
         np.transpose,
         axes,
         x,
         tuple(range(x.ndim)),
-        max_mem=max_mem,
+        allowed_mem=allowed_mem,
+        reserved_mem=reserved_mem,
         target_store=target_store,
         shape=x.shape,
         dtype=x.dtype,
         chunks=x.chunks,
         axes=axes,
     )
 
@@ -85,27 +89,31 @@
 def test_blockwise_with_args(tmp_path, executor):
     source = create_zarr(
         [[1, 2, 3], [4, 5, 6], [7, 8, 9]],
         dtype=int,
         chunks=(2, 2),
         store=tmp_path / "source.zarr",
     )
-    max_mem = 1000
+    allowed_mem = 1000
     target_store = tmp_path / "target.zarr"
 
     pipeline = _permute_dims(
-        source, axes=(1, 0), max_mem=max_mem, target_store=target_store
+        source,
+        axes=(1, 0),
+        allowed_mem=allowed_mem,
+        reserved_mem=0,
+        target_store=target_store,
     )
 
     assert pipeline.target_array.shape == (3, 3)
     assert pipeline.target_array.dtype == int
     assert pipeline.target_array.chunks == (2, 2)
 
     itemsize = np.dtype(int).itemsize
-    assert pipeline.required_mem == (
+    assert pipeline.projected_mem == (
         (itemsize * 2 * 2)  # source compressed chunk
         + (itemsize * 2 * 2)  # source uncompressed chunk
         + (itemsize * 2 * 2)  # output compressed chunk
         + (itemsize * 2 * 2)  # output uncompressed chunk
     )
 
     assert pipeline.num_tasks == 4
@@ -114,35 +122,38 @@
 
     res = zarr.open(target_store)
     assert_array_equal(
         res[:], np.transpose(np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]]), axes=(1, 0))
     )
 
 
-def test_blockwise_max_mem_exceeded(tmp_path):
+@pytest.mark.parametrize("reserved_mem", [0, 10])
+def test_blockwise_allowed_mem_exceeded(tmp_path, reserved_mem):
     source1 = create_zarr(
         [0, 1, 2], dtype=np.int64, chunks=2, store=tmp_path / "source1.zarr"
     )
     source2 = create_zarr(
         [10, 50, 100], dtype=np.int64, chunks=2, store=tmp_path / "source2.zarr"
     )
-    max_mem = 100
+    allowed_mem = 100
     target_store = tmp_path / "target.zarr"
 
     with pytest.raises(
-        ValueError, match=r"Blockwise memory \(\d+\) exceeds max_mem \(100\)"
+        ValueError,
+        match=r"Projected blockwise memory \(\d+\) exceeds allowed_mem \(100\), including reserved_mem \(\d+\)",
     ):
         blockwise(
             np.outer,
             "ij",
             source1,
             "i",
             source2,
             "j",
-            max_mem=max_mem,
+            allowed_mem=allowed_mem,
+            reserved_mem=reserved_mem,
             target_store=target_store,
             shape=(3, 3),
             dtype=np.int64,
             chunks=(2, 2),
         )
```

### Comparing `cubed-0.6.3/cubed/tests/primitive/test_rechunk.py` & `cubed-0.7.0/cubed/tests/primitive/test_rechunk.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,84 +10,98 @@
 
 @pytest.fixture(scope="module", params=[PythonPipelineExecutor()])
 def executor(request):
     return request.param
 
 
 @pytest.mark.parametrize(
-    "shape, source_chunks, max_mem, target_chunks, expected_required_mem, expected_num_tasks",
+    "shape, source_chunks, allowed_mem, reserved_mem, target_chunks, expected_projected_mem, expected_num_tasks",
     [
         # one target chunk is made up of two source chunks
         (
             (4, 4),
             (1, 2),
             1000,
+            0,
+            (1, 4),
+            1000,
+            1,
+        ),
+        # everything still works with 100 bytes of reserved_mem
+        (
+            (4, 4),
+            (1, 2),
+            1000,
+            100,
             (1, 4),
             1000,
             1,
         ),
         # only enough memory for one source/target chunk
         (
             (4, 4),
             (1, 4),
             4 * 8 * 4,  # elts x itemsize x copies
+            0,
             (4, 1),
             4 * 8 * 4,  # elts x itemsize x copies
             8,
         ),
     ],
 )
 def test_rechunk(
     tmp_path,
     executor,
     shape,
     source_chunks,
-    max_mem,
+    allowed_mem,
+    reserved_mem,
     target_chunks,
-    expected_required_mem,
+    expected_projected_mem,
     expected_num_tasks,
 ):
     source = zarr.ones(shape, chunks=source_chunks, store=tmp_path / "source.zarr")
-    max_mem = max_mem
     target_store = tmp_path / "target.zarr"
     temp_store = tmp_path / "temp.zarr"
 
     pipeline = rechunk(
         source,
         target_chunks=target_chunks,
-        max_mem=max_mem,
+        allowed_mem=allowed_mem,
+        reserved_mem=reserved_mem,
         target_store=target_store,
         temp_store=temp_store,
     )
 
     assert pipeline.target_array.shape == shape
     assert pipeline.target_array.dtype == source.dtype
     assert pipeline.target_array.chunks == target_chunks
 
-    assert pipeline.required_mem == expected_required_mem
+    assert pipeline.projected_mem == expected_projected_mem
 
     assert pipeline.num_tasks == expected_num_tasks
 
     execute_pipeline(pipeline, executor=executor)
 
     res = zarr.open(target_store)
     assert_array_equal(res[:], np.ones(shape))
     assert res.chunks == target_chunks
 
 
-def test_rechunk_max_mem_exceeded(tmp_path):
+def test_rechunk_allowed_mem_exceeded(tmp_path):
     source = zarr.ones((4, 4), chunks=(2, 2), store=tmp_path / "source.zarr")
-    max_mem = 16
+    allowed_mem = 16
     target_store = tmp_path / "target.zarr"
     temp_store = tmp_path / "temp.zarr"
 
-    # max mem is reduced by a factor of 4 from 16 to 4
+    # cubed's allowed_mem is reduced by a factor of 4 for rechunker's max_mem from 16 to 4
     with pytest.raises(
         ValueError, match=r"Source chunk memory \(32\) exceeds max_mem \(4\)"
     ):
         rechunk(
             source,
             target_chunks=(4, 1),
-            max_mem=max_mem,
+            allowed_mem=allowed_mem,
+            reserved_mem=0,
             target_store=target_store,
             temp_store=temp_store,
         )
```

### Comparing `cubed-0.6.3/cubed/tests/runtime/test_backup.py` & `cubed-0.7.0/cubed/tests/runtime/test_backup.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/tests/runtime/test_lithops.py` & `cubed-0.7.0/cubed/tests/runtime/test_lithops.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/tests/runtime/test_modal_async.py` & `cubed-0.7.0/cubed/tests/runtime/test_modal_async.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/tests/test_array_api.py` & `cubed-0.7.0/cubed/tests/test_array_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import cubed.array_api as xp
 from cubed.array_api.manipulation_functions import reshape_chunks
 from cubed.tests.utils import ALL_EXECUTORS, MAIN_EXECUTORS, MODAL_EXECUTORS
 
 
 @pytest.fixture()
 def spec(tmp_path):
-    return cubed.Spec(tmp_path, max_mem=100000)
+    return cubed.Spec(tmp_path, allowed_mem=100000)
 
 
 @pytest.fixture(scope="module", params=MAIN_EXECUTORS)
 def executor(request):
     return request.param
 
 
@@ -289,15 +289,15 @@
     expected = np.matmul(x, y)
     assert_array_equal(c.compute(executor=executor), expected)
 
 
 @pytest.mark.cloud
 def test_matmul_cloud(executor):
     tmp_path = "gs://barry-zarr-test/matmul"
-    spec = cubed.Spec(tmp_path, max_mem=100000)
+    spec = cubed.Spec(tmp_path, allowed_mem=100000)
     try:
         a = xp.asarray(
             [[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12], [13, 14, 15, 16]],
             chunks=(2, 2),
             spec=spec,
         )
         b = xp.asarray(
@@ -314,15 +314,15 @@
         fs = fsspec.open(tmp_path).fs
         fs.rm(tmp_path, recursive=True)
 
 
 @pytest.mark.cloud
 def test_matmul_modal(modal_executor):
     tmp_path = "s3://cubed-unittest/matmul"
-    spec = cubed.Spec(tmp_path, max_mem=100000)
+    spec = cubed.Spec(tmp_path, allowed_mem=100000)
     try:
         a = xp.asarray(
             [[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12], [13, 14, 15, 16]],
             chunks=(2, 2),
             spec=spec,
         )
         b = xp.asarray(
```

### Comparing `cubed-0.6.3/cubed/tests/test_core.py` & `cubed-0.7.0/cubed/tests/test_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from cubed.primitive.blockwise import apply_blockwise
 from cubed.runtime.types import DagExecutor
 from cubed.tests.utils import MAIN_EXECUTORS, MODAL_EXECUTORS, TaskCounter, create_zarr
 
 
 @pytest.fixture()
 def spec(tmp_path):
-    return cubed.Spec(tmp_path, max_mem=100000)
+    return cubed.Spec(tmp_path, allowed_mem=100000)
 
 
 @pytest.fixture(scope="module", params=MAIN_EXECUTORS)
 def executor(request):
     return request.param
 
 
@@ -228,45 +228,45 @@
     b = xp.negative(a)
     assert_array_equal(
         b.compute(executor=executor),
         -np.ones((3, 3)),
     )
 
 
-def test_default_spec_max_mem_exceeded():
+def test_default_spec_allowed_mem_exceeded():
     # default spec fails for large computations
     a = xp.ones((100000, 100000), chunks=(10000, 10000))
     with pytest.raises(ValueError):
         xp.negative(a)
 
 
 def test_different_specs(tmp_path):
-    spec1 = cubed.Spec(tmp_path, max_mem=100000)
-    spec2 = cubed.Spec(tmp_path, max_mem=200000)
+    spec1 = cubed.Spec(tmp_path, allowed_mem=100000)
+    spec2 = cubed.Spec(tmp_path, allowed_mem=200000)
     a = xp.ones((3, 3), chunks=(2, 2), spec=spec1)
     b = xp.ones((3, 3), chunks=(2, 2), spec=spec2)
     with pytest.raises(ValueError):
         xp.add(a, b)
 
 
 def test_reduction_multiple_rounds(tmp_path, executor):
-    spec = cubed.Spec(tmp_path, max_mem=1000)
+    spec = cubed.Spec(tmp_path, allowed_mem=1000)
     a = xp.ones((100, 10), dtype=np.uint8, chunks=(1, 10), spec=spec)
     b = xp.sum(a, axis=0, dtype=np.uint8)
     # check that there is > 1 rechunk step
     rechunks = [
         n for (n, d) in b.plan.dag.nodes(data=True) if d["op_name"] == "rechunk"
     ]
     assert len(rechunks) > 1
-    assert b.plan.max_required_mem() == 1000
+    assert b.plan.max_projected_mem() == 1000
     assert_array_equal(b.compute(executor=executor), np.ones((100, 10)).sum(axis=0))
 
 
 def test_reduction_not_enough_memory(tmp_path):
-    spec = cubed.Spec(tmp_path, max_mem=50)
+    spec = cubed.Spec(tmp_path, allowed_mem=50)
     a = xp.ones((100, 10), dtype=np.uint8, chunks=(1, 10), spec=spec)
     with pytest.raises(ValueError, match=r"Not enough memory for reduction"):
         xp.sum(a, axis=0, dtype=np.uint8)
 
 
 def test_compute_multiple():
     a = xp.asarray([[1, 2, 3], [4, 5, 6], [7, 8, 9]], chunks=(2, 2))
@@ -291,16 +291,16 @@
 
     assert_array_equal(dc, dn)
     assert_array_equal(ec, en)
     assert_array_equal(gc, gn)
 
 
 def test_compute_multiple_different_specs(tmp_path):
-    spec1 = cubed.Spec(tmp_path, max_mem=100000)
-    spec2 = cubed.Spec(tmp_path, max_mem=200000)
+    spec1 = cubed.Spec(tmp_path, allowed_mem=100000)
+    spec2 = cubed.Spec(tmp_path, allowed_mem=200000)
 
     a1 = xp.ones((3, 3), chunks=(2, 2), spec=spec1)
     b1 = xp.ones((3, 3), chunks=(2, 2), spec=spec1)
     c1 = xp.add(a1, b1)
 
     a2 = xp.ones((3, 3), chunks=(2, 2), spec=spec2)
     b2 = xp.ones((3, 3), chunks=(2, 2), spec=spec2)
@@ -404,15 +404,15 @@
     assert task_counter.value == 4
 
 
 @pytest.mark.cloud
 def test_callbacks_modal(spec, modal_executor):
     task_counter = TaskCounter(check_timestamps=False)
     tmp_path = "s3://cubed-unittest/callbacks"
-    spec = cubed.Spec(tmp_path, max_mem=100000)
+    spec = cubed.Spec(tmp_path, allowed_mem=100000)
     try:
         a = xp.asarray([[1, 2, 3], [4, 5, 6], [7, 8, 9]], chunks=(2, 2), spec=spec)
         b = xp.asarray([[1, 1, 1], [1, 1, 1], [1, 1, 1]], chunks=(2, 2), spec=spec)
         c = xp.add(a, b)
         assert_array_equal(
             c.compute(executor=modal_executor, callbacks=[task_counter]),
             np.array([[2, 3, 4], [5, 6, 7], [8, 9, 10]]),
```

### Comparing `cubed-0.6.3/cubed/tests/test_gufunc.py` & `cubed-0.7.0/cubed/tests/test_gufunc.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import cubed
 import cubed.array_api as xp
 from cubed import apply_gufunc
 
 
 @pytest.fixture()
 def spec(tmp_path):
-    return cubed.Spec(tmp_path, max_mem=1000000)
+    return cubed.Spec(tmp_path, allowed_mem=1000000)
 
 
 @pytest.mark.parametrize("vectorize", [False, True])
 def test_apply_reduction(spec, vectorize):
     def stats(x):
         return np.mean(x, axis=-1)
```

### Comparing `cubed-0.6.3/cubed/tests/test_indexing.py` & `cubed-0.7.0/cubed/tests/test_indexing.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import cubed
 import cubed.array_api as xp
 
 
 @pytest.fixture()
 def spec(tmp_path):
-    return cubed.Spec(tmp_path, max_mem=100000)
+    return cubed.Spec(tmp_path, allowed_mem=100000)
 
 
 # Int array indexing is not a part of the array API, so test it separately.
 
 
 @pytest.mark.parametrize(
     "ind",
```

### Comparing `cubed-0.6.3/cubed/tests/test_optimization.py` & `cubed-0.7.0/cubed/tests/test_optimization.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import cubed
 import cubed.array_api as xp
 from cubed.tests.utils import TaskCounter
 
 
 @pytest.fixture()
 def spec(tmp_path):
-    return cubed.Spec(tmp_path, max_mem=100000)
+    return cubed.Spec(tmp_path, allowed_mem=100000)
 
 
 def test_fusion(spec):
     a = xp.asarray([[1, 2, 3], [4, 5, 6], [7, 8, 9]], chunks=(2, 2), spec=spec)
     b = xp.negative(a)
     c = xp.astype(b, np.float32)
     d = xp.negative(c)
```

### Comparing `cubed-0.6.3/cubed/tests/test_random.py` & `cubed-0.7.0/cubed/tests/test_random.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import cubed.array_api as xp
 import cubed.random
 from cubed.tests.utils import MAIN_EXECUTORS
 
 
 @pytest.fixture()
 def spec(tmp_path):
-    return cubed.Spec(tmp_path, max_mem=100000)
+    return cubed.Spec(tmp_path, allowed_mem=100000)
 
 
 @pytest.fixture(scope="module", params=MAIN_EXECUTORS)
 def executor(request):
     return request.param
```

### Comparing `cubed-0.6.3/cubed/tests/test_utils.py` & `cubed-0.7.0/cubed/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pytest
 
 from cubed.utils import (
     chunk_memory,
     extract_stack_summaries,
     join_path,
     memory_repr,
-    peak_memory,
+    peak_measured_mem,
     to_chunksize,
 )
 
 
 def test_chunk_memory():
     assert chunk_memory(np.int64, (3,)) == 24
     assert chunk_memory(np.int32, (3,)) == 12
@@ -53,16 +53,16 @@
     assert memory_repr(1_000) == "1.0 KB"
     assert memory_repr(9_999) == "10.0 KB"
     assert memory_repr(1_000_000) == "1.0 MB"
     assert memory_repr(1_000_000_000_000_000) == "1.0 PB"
 
 
 @pytest.mark.skipif(platform.system() == "Windows", reason="does not run on windows")
-def test_peak_memory():
-    assert peak_memory() > 0
+def test_peak_measured_mem():
+    assert peak_measured_mem() > 0
 
 
 def test_extract_stack_summaries():
     frame = inspect.currentframe()
     stack_summaries = extract_stack_summaries(frame)
     assert stack_summaries[-1].name == "test_extract_stack_summaries"
     assert stack_summaries[-1].module == "cubed.tests.test_utils"
```

### Comparing `cubed-0.6.3/cubed/tests/utils.py` & `cubed-0.7.0/cubed/tests/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ]
 
 # don't run all tests on every executor as it's too slow, so just have a subset
 MAIN_EXECUTORS = [PythonPipelineExecutor(), PythonDagExecutor()]
 
 
 if platform.system() != "Windows":
-    # AsyncPythonDagExecutor calls `peak_memory` which is not supported on Windows
+    # AsyncPythonDagExecutor calls `peak_measured_mem` which is not supported on Windows
     ALL_EXECUTORS.append(AsyncPythonDagExecutor())
 
 
 try:
     from cubed.runtime.executors.beam import BeamDagExecutor, BeamPipelineExecutor
 
     ALL_EXECUTORS.append(BeamDagExecutor())
```

### Comparing `cubed-0.6.3/cubed/utils.py` & `cubed-0.7.0/cubed/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,22 +66,22 @@
     num /= 1000.0
     for x in ["KB", "MB", "GB", "TB", "PB"]:
         if num < 1000.0:
             return f"{num:3.1f} {x}"
         num /= 1000.0
 
 
-def peak_memory():
-    """Return the peak memory usage in bytes.
+def peak_measured_mem():
+    """Measures the peak memory usage in bytes.
 
     Note: this function currently doesn't work on Windows.
     """
 
     if platform.system() == "Windows":
-        raise NotImplementedError("`peak_memory` is not implemented on Windows")
+        raise NotImplementedError("`peak_measured_mem` is not implemented on Windows")
 
     from resource import RUSAGE_SELF, getrusage
 
     ru_maxrss = getrusage(RUSAGE_SELF).ru_maxrss
     # note that on Linux ru_maxrss is in KiB, while on Mac it is in bytes
     # see https://pythonspeed.com/articles/estimating-memory-usage/#measuring-peak-memory-usage
     return ru_maxrss * 1024 if platform.system() == "Linux" else ru_maxrss
```

### Comparing `cubed-0.6.3/cubed/vendor/dask/array/core.py` & `cubed-0.7.0/cubed/vendor/dask/array/core.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/vendor/dask/array/gufunc.py` & `cubed-0.7.0/cubed/vendor/dask/array/gufunc.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/vendor/dask/array/reshape.py` & `cubed-0.7.0/cubed/vendor/dask/array/reshape.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/vendor/dask/array/utils.py` & `cubed-0.7.0/cubed/vendor/dask/array/utils.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/vendor/dask/blockwise.py` & `cubed-0.7.0/cubed/vendor/dask/blockwise.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/vendor/dask/core.py` & `cubed-0.7.0/cubed/vendor/dask/core.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/vendor/dask/utils.py` & `cubed-0.7.0/cubed/vendor/dask/utils.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/vendor/rechunker/algorithm.py` & `cubed-0.7.0/cubed/vendor/rechunker/algorithm.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/vendor/rechunker/api.py` & `cubed-0.7.0/cubed/vendor/rechunker/api.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/vendor/rechunker/executors/python.py` & `cubed-0.7.0/cubed/vendor/rechunker/executors/python.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed/vendor/rechunker/types.py` & `cubed-0.7.0/cubed/vendor/rechunker/types.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/cubed.egg-info/PKG-INFO` & `cubed-0.7.0/cubed.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubed
-Version: 0.6.3
+Version: 0.7.0
 Summary: Bounded-memory serverless distributed N-dimensional array processing
 Author-email: Tom White <tom.e.white@gmail.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/tomwhite/cubed
 Project-URL: documentation, https://tomwhite.github.io/cubed
 Project-URL: repository, https://github.com/tomwhite/cubed
 Classifier: Development Status :: 3 - Alpha
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: diagnostics
 Provides-Extra: beam
 Provides-Extra: lithops
 Provides-Extra: modal
-Provides-Extra: complete
 Provides-Extra: test
 Provides-Extra: test-modal
 License-File: LICENSE
 
 # Cubed
 
 **_Note: this is a proof-of-concept, and many things are incomplete or don't work._**
```

### Comparing `cubed-0.6.3/cubed.egg-info/SOURCES.txt` & `cubed-0.7.0/cubed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubed-0.6.3/pyproject.toml` & `cubed-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cubed"
-version = "0.6.3"
+version = "0.7.0"
 authors = [
     {name = "Tom White", email = "tom.e.white@gmail.com"},
 ]
 license = {text = "Apache License 2.0"}
 description = "Bounded-memory serverless distributed N-dimensional array processing"
 readme = {file = "README.md", content-type = "text/markdown"}
 classifiers = [
@@ -41,15 +41,14 @@
 beam = ["apache-beam", "gcsfs"]
 lithops = ["lithops[aws] >= 2.7.0"]
 modal = [
     "cubed[diagnostics]",
     "modal-client",
     "s3fs",
 ]
-complete = ["cubed[beam,lithops,modal]"]
 test = [
     "apache-beam",  # beam but not gcsfs as tests use local beam runner
     "cubed[diagnostics,lithops]",  # modal tests separate due to conflicting package reqs
     "dill",
     "pytest",
     "pytest-cov",
     "pytest-mock",
```

### Comparing `cubed-0.6.3/setup.cfg` & `cubed-0.7.0/setup.cfg`

 * *Files identical despite different names*

