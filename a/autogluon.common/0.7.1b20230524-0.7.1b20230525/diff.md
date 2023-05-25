# Comparing `tmp/autogluon.common-0.7.1b20230524.tar.gz` & `tmp/autogluon.common-0.7.1b20230525.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.common-0.7.1b20230524.tar", last modified: Wed May 24 09:04:08 2023, max compression
+gzip compressed data, was "autogluon.common-0.7.1b20230525.tar", last modified: Thu May 25 09:03:54 2023, max compression
```

## Comparing `autogluon.common-0.7.1b20230524.tar` & `autogluon.common-0.7.1b20230525.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:08.706606 autogluon.common-0.7.1b20230524/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-24 09:04:08.706606 autogluon.common-0.7.1b20230524/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:04:08.706606 autogluon.common-0.7.1b20230524/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:08.690605 autogluon.common-0.7.1b20230524/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:08.694606 autogluon.common-0.7.1b20230524/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:08.694606 autogluon.common-0.7.1b20230524/src/autogluon/common/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:08.698606 autogluon.common-0.7.1b20230524/src/autogluon/common/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/features/feature_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/features/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/features/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:08.702606 autogluon.common-0.7.1b20230524/src/autogluon/common/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/loaders/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/loaders/load_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/loaders/load_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/loaders/load_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/loaders/load_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/loaders/load_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/loaders/load_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/loaders/load_zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:08.702606 autogluon.common-0.7.1b20230524/src/autogluon/common/savers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/savers/save_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/savers/save_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/savers/save_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/savers/save_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/savers/save_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:08.706606 autogluon.common-0.7.1b20230524/src/autogluon/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/utils/compression_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/utils/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/utils/distribute_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/utils/lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/utils/multiprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/utils/nvutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/utils/resource_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/utils/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/utils/try_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-24 09:03:54.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-24 09:04:08.000000 autogluon.common-0.7.1b20230524/src/autogluon/common/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:08.694606 autogluon.common-0.7.1b20230524/src/autogluon.common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-24 09:04:08.000000 autogluon.common-0.7.1b20230524/src/autogluon.common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-24 09:04:08.000000 autogluon.common-0.7.1b20230524/src/autogluon.common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:04:08.000000 autogluon.common-0.7.1b20230524/src/autogluon.common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 09:04:08.000000 autogluon.common-0.7.1b20230524/src/autogluon.common.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-24 09:04:08.000000 autogluon.common-0.7.1b20230524/src/autogluon.common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 09:04:08.000000 autogluon.common-0.7.1b20230524/src/autogluon.common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:04:08.000000 autogluon.common-0.7.1b20230524/src/autogluon.common.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:54.041208 autogluon.common-0.7.1b20230525/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-25 09:03:54.041208 autogluon.common-0.7.1b20230525/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:03:54.041208 autogluon.common-0.7.1b20230525/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:54.033208 autogluon.common-0.7.1b20230525/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:54.033208 autogluon.common-0.7.1b20230525/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:54.037208 autogluon.common-0.7.1b20230525/src/autogluon/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:54.037208 autogluon.common-0.7.1b20230525/src/autogluon/common/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/features/feature_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/features/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/features/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:54.037208 autogluon.common-0.7.1b20230525/src/autogluon/common/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/loaders/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/loaders/load_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/loaders/load_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/loaders/load_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/loaders/load_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/loaders/load_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/loaders/load_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/loaders/load_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:54.037208 autogluon.common-0.7.1b20230525/src/autogluon/common/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/savers/save_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/savers/save_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/savers/save_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/savers/save_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/savers/save_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:54.041208 autogluon.common-0.7.1b20230525/src/autogluon/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/utils/compression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/utils/deprecated_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/utils/distribute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/utils/lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/utils/multiprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/utils/nvutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/utils/resource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/utils/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/utils/try_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-25 09:03:38.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-25 09:03:53.000000 autogluon.common-0.7.1b20230525/src/autogluon/common/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:54.037208 autogluon.common-0.7.1b20230525/src/autogluon.common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-25 09:03:53.000000 autogluon.common-0.7.1b20230525/src/autogluon.common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-25 09:03:53.000000 autogluon.common-0.7.1b20230525/src/autogluon.common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:03:53.000000 autogluon.common-0.7.1b20230525/src/autogluon.common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 09:03:53.000000 autogluon.common-0.7.1b20230525/src/autogluon.common.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-25 09:03:53.000000 autogluon.common-0.7.1b20230525/src/autogluon.common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 09:03:53.000000 autogluon.common-0.7.1b20230525/src/autogluon.common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:03:53.000000 autogluon.common-0.7.1b20230525/src/autogluon.common.egg-info/zip-safe
```

### Comparing `autogluon.common-0.7.1b20230524/LICENSE` & `autogluon.common-0.7.1b20230525/LICENSE`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/PKG-INFO` & `autogluon.common-0.7.1b20230525/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
-Version: 0.7.1b20230524
+Version: 0.7.1b20230525
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.common-0.7.1b20230524/setup.py` & `autogluon.common-0.7.1b20230525/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/features/feature_metadata.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/features/feature_metadata.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/features/infer_types.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/features/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/features/types.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/features/types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/loaders/_utils.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/loaders/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/loaders/load_pd.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/loaders/load_pd.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/loaders/load_pkl.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/loaders/load_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/loaders/load_pointer.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/loaders/load_pointer.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/loaders/load_s3.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/loaders/load_s3.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/loaders/load_str.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/loaders/load_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/loaders/load_zip.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/loaders/load_zip.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/savers/save_json.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/savers/save_json.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/savers/save_pd.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/savers/save_pd.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/savers/save_pkl.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/savers/save_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/savers/save_str.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/savers/save_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/space.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/space.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/utils/compression_utils.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/utils/compression_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/utils/deprecated.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/utils/deprecated_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import functools
 import inspect
 import warnings
-from typing import Any, Dict, Optional
+from typing import Any, Callable, Dict, Optional
 
 from packaging import version
 
 from ..version import __version__
 
 
 def _deprecation_warning(
@@ -34,15 +34,15 @@
 def Deprecated(
     min_version_to_warn: str,
     min_version_to_error: str,
     old: Optional[str] = None,
     new: Optional[str] = None,
     custom_warning_msg: Optional[str] = None,
     version_to_remove: Optional[str] = None,
-    _mock_version: Optional[str] = None
+    _ag_version: Optional[str] = None,
 ):
     """
     Decorator to add deprecation warnings or raise an error to the decorated object.
     Can be applied to both functions and classes.
 
     Parameters
     ----------
@@ -91,16 +91,16 @@
     >>> def old_func():
     >>>     ...
     """
 
     def _decorator(obj):
         error = False
         ag_version = __version__
-        if _mock_version is not None:
-            ag_version = _mock_version
+        if _ag_version is not None:
+            ag_version = _ag_version
         if version.parse(ag_version) < version.parse(min_version_to_warn):
             return obj
         if version.parse(ag_version) >= version.parse(min_version_to_error):
             error = True
         if inspect.isclass(obj):
             obj_init = obj.__init__
 
@@ -145,14 +145,15 @@
     for old_name, new_name in kwargs_mapping.items():
         if old_name in kwargs:
             if new_name is not None and new_name in kwargs:
                 raise ValueError(
                     f"{func_name} received both {old_name} and {new_name} as arguments."
                     f"{old_name} is deprecated, please use {new_name} instead."
                 )
+            print(error)
             _deprecation_warning(
                 old=old_name,
                 new=new_name,
                 custom_warning_msg=custom_warning_msg,
                 version_to_remove=version_to_remove,
                 error=error,
             )
@@ -162,15 +163,15 @@
 
 # Inspired by https://stackoverflow.com/questions/49802412/how-to-implement-deprecation-in-python-with-argument-alias
 def Deprecated_args(
     min_version_to_warn: str,
     min_version_to_error: str,
     custom_warning_msg: Optional[str] = None,
     version_to_remove: Optional[str] = None,
-    _mock_version: Optional[str] = None,
+    _ag_version: Optional[str] = None,
     **kwargs_mapping,
 ):
     """
     Decorator to add deprecation warnings or raise an error to deprecated arguments.
     If not raising error, will replace the deprecated argument with the new one.
 
     Parameters
@@ -210,16 +211,16 @@
     >>> def myfunc(deprecated_arg_with_no_replacement):  # This argument need to still exists for it to work
     >>>     ...
     """
 
     def _decorator(obj):
         error = False
         ag_version = __version__
-        if _mock_version is not None:
-            ag_version = _mock_version
+        if _ag_version is not None:
+            ag_version = _ag_version
         if version.parse(ag_version) < version.parse(min_version_to_warn):
             return obj
         if version.parse(ag_version) >= version.parse(min_version_to_error):
             error = True
 
         @functools.wraps(obj)
         def patched_obj_with_warning_msg(*args, **kwargs):
@@ -232,7 +233,23 @@
                 error=error,
             )
             return obj(*args, **kwargs)
 
         return patched_obj_with_warning_msg
 
     return _decorator
+
+
+def construct_deprecated_wrapper(ag_version) -> Callable:
+    """Return Deprecated decorator with ag_version as the local AG version for checking"""
+    def _decorator(*args, **kwargs):
+        return Deprecated(*args, _ag_version=ag_version, **kwargs)
+
+    return _decorator
+
+
+def construct_deprecated_args_wrapper(ag_version) -> Callable:
+    """Return Deprecated_args decorator with ag_version as the local AG version for checking"""
+    def _decorator(*args, **kwargs):
+        return Deprecated_args(*args, _ag_version=ag_version, **kwargs)
+
+    return _decorator
```

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/utils/distribute_utils.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/utils/distribute_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/utils/file_utils.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/utils/log_utils.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/utils/multiprocessing_utils.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/utils/multiprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/utils/nvutil.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/utils/nvutil.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/utils/pandas_utils.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/utils/resource_utils.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/utils/resource_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/utils/s3_utils.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/utils/try_import.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/utils/try_import.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon/common/utils/utils.py` & `autogluon.common-0.7.1b20230525/src/autogluon/common/utils/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from datetime import datetime
 
 import logging
 import os
 import platform
 import sys
-from typing import Dict, Any
+from typing import Dict, Any, Optional
 
 from ..version import __version__
 try:
     from ..version import __lite__
 except ImportError:
     __lite__ = False
 
@@ -133,7 +133,37 @@
     return logs
 
 
 def bytes_to_mega_bytes(memory_amount: int) -> int:
     """ Utility to convert a number of bytes (int) into a number of mega bytes (int)
     """
     return memory_amount >> 20
+
+
+def check_saved_predictor_version(
+    version_current: str,
+    version_saved: str,
+    require_version_match: bool = True,
+    logger: Optional[logging.Logger] = None,
+) -> None:
+    if logger is None:
+        logger = logging.getLogger(__name__)
+
+    if version_saved != version_current:
+        logger.warning("")
+        logger.warning("############################## WARNING ##############################")
+        logger.warning(
+            "WARNING: AutoGluon version differs from the version used to create the predictor! "
+            "This may lead to instability and it is highly recommended the predictor be loaded "
+            "with the exact AutoGluon version it was created with."
+        )
+        logger.warning(f"\tPredictor Version: {version_saved}")
+        logger.warning(f"\tCurrent Version:   {version_current}")
+        logger.warning("############################## WARNING ##############################")
+        logger.warning("")
+
+        if require_version_match:
+            raise AssertionError(
+                f"Predictor was created on version {version_saved} but is being loaded with version {version_current}. "
+                f"Please ensure the versions match to avoid instability. While it is NOT recommended, "
+                f"this error can be bypassed by specifying `require_version_match=False`."
+            )
```

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon.common.egg-info/PKG-INFO` & `autogluon.common-0.7.1b20230525/src/autogluon.common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
-Version: 0.7.1b20230524
+Version: 0.7.1b20230525
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.common-0.7.1b20230524/src/autogluon.common.egg-info/SOURCES.txt` & `autogluon.common-0.7.1b20230525/src/autogluon.common.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 NOTICE
 setup.py
-src/autogluon/__init__.py
 src/autogluon.common.egg-info/PKG-INFO
 src/autogluon.common.egg-info/SOURCES.txt
 src/autogluon.common.egg-info/dependency_links.txt
 src/autogluon.common.egg-info/namespace_packages.txt
 src/autogluon.common.egg-info/requires.txt
 src/autogluon.common.egg-info/top_level.txt
 src/autogluon.common.egg-info/zip-safe
@@ -30,15 +29,15 @@
 src/autogluon/common/savers/save_pd.py
 src/autogluon/common/savers/save_pkl.py
 src/autogluon/common/savers/save_pointer.py
 src/autogluon/common/savers/save_str.py
 src/autogluon/common/utils/__init__.py
 src/autogluon/common/utils/compression_utils.py
 src/autogluon/common/utils/context.py
-src/autogluon/common/utils/deprecated.py
+src/autogluon/common/utils/deprecated_utils.py
 src/autogluon/common/utils/distribute_utils.py
 src/autogluon/common/utils/file_utils.py
 src/autogluon/common/utils/lite.py
 src/autogluon/common/utils/log_utils.py
 src/autogluon/common/utils/multiprocessing_utils.py
 src/autogluon/common/utils/nvutil.py
 src/autogluon/common/utils/pandas_utils.py
```

