# Comparing `tmp/dagster-aws-0.9.9rc1.tar.gz` & `tmp/dagster-aws-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-aws-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:21 2020, max compression
+gzip compressed data, was "dagster-aws-1.0.5.tar", last modified: Fri Aug 26 13:44:10 2022, max compression
```

## Comparing `dagster-aws-0.9.9rc1.tar` & `dagster-aws-1.0.5.tar`

### file list

```diff
@@ -1,92 +1,69 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)      165 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      632 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      119 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws/
--rw-r--r--   0 bobchen    (501) staff       (20)      154 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws/cloudwatch/
--rw-r--r--   0 bobchen    (501) staff       (20)       39 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/cloudwatch/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     9246 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/cloudwatch/loggers.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws/ecs/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/ecs/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     9702 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/ecs/client.py
--rw-r--r--   0 bobchen    (501) staff       (20)     6841 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/ecs/launcher.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws/emr/
--rw-r--r--   0 bobchen    (501) staff       (20)      227 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/emr/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    51135 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/emr/configs.py
--rw-r--r--   0 bobchen    (501) staff       (20)    16339 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/emr/emr.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2956 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/emr/emr_step_main.py
--rw-r--r--   0 bobchen    (501) staff       (20)      489 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/emr/main.py.template
--rw-r--r--   0 bobchen    (501) staff       (20)    13976 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/emr/pyspark_step_launcher.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3633 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/emr/types.py
--rw-r--r--   0 bobchen    (501) staff       (20)      602 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/emr/utils.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws/redshift/
--rw-r--r--   0 bobchen    (501) staff       (20)      145 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/redshift/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    16518 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/redshift/resources.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/
--rw-r--r--   0 bobchen    (501) staff       (20)      622 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7595 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/compute_log_manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1788 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/file_cache.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3216 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/file_manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1270 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/intermediate_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     5183 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/object_store.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4213 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2344 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/s3_fake_resource.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2411 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4660 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/system_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)      689 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/utils.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws/utils/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/utils/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws/utils/mrjob/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/utils/mrjob/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4449 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/utils/mrjob/log4j.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4843 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/utils/mrjob/retry.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3589 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/utils/mrjob/utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      632 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)     2610 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       71 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       30 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/cloudwatch_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/cloudwatch_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      665 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/cloudwatch_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3586 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/cloudwatch_tests/test_loggers.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/ecs_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/ecs_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     5302 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/ecs_tests/test_ecs_client.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1120 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7576 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/test_emr.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2152 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/test_emr_step_main.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7699 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/test_pyspark.py
--rw-r--r--   0 bobchen    (501) staff       (20)      958 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/test_pyspark_step_launcher.py
--rw-r--r--   0 bobchen    (501) staff       (20)      760 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/test_utils.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/redshift_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/redshift_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      102 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/redshift_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)     6642 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/redshift_tests/test_resources.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      102 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4218 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/test_compute_log_manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1722 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/test_file_handle_to_s3.py
--rw-r--r--   0 bobchen    (501) staff       (20)    15946 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/test_intermediate_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1052 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/test_object_store.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1441 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/test_s3_file_cache.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7083 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/test_s3_file_manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)       89 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/test_version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/utils_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/utils_tests/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/utils_tests/mrjob_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/utils_tests/mrjob_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3840 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/utils_tests/mrjob_tests/test_log4j.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2410 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/utils_tests/mrjob_tests/test_utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1184 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:10.244032 dagster-aws-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      194 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      737 2022-08-26 13:44:10.244032 dagster-aws-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      119 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:10.216031 dagster-aws-1.0.5/dagster_aws/
+-rw-r--r--   0 root         (0) root         (0)      155 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:10.216031 dagster-aws-1.0.5/dagster_aws/athena/
+-rw-r--r--   0 root         (0) root         (0)      154 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/athena/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10173 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/athena/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:10.220031 dagster-aws-1.0.5/dagster_aws/cloudwatch/
+-rw-r--r--   0 root         (0) root         (0)       39 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/cloudwatch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9127 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/cloudwatch/loggers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:10.220031 dagster-aws-1.0.5/dagster_aws/ecr/
+-rw-r--r--   0 root         (0) root         (0)       69 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/ecr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/ecr/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:10.224032 dagster-aws-1.0.5/dagster_aws/ecs/
+-rw-r--r--   0 root         (0) root         (0)       86 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/ecs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5535 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/ecs/container_context.py
+-rw-r--r--   0 root         (0) root         (0)    16795 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/ecs/launcher.py
+-rw-r--r--   0 root         (0) root         (0)     5578 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/ecs/tasks.py
+-rw-r--r--   0 root         (0) root         (0)     1700 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/ecs/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)      149 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/ecs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:10.228031 dagster-aws-1.0.5/dagster_aws/emr/
+-rw-r--r--   0 root         (0) root         (0)      227 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/emr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51135 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/emr/configs.py
+-rw-r--r--   0 root         (0) root         (0)   146725 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/emr/configs_spark.py
+-rw-r--r--   0 root         (0) root         (0)    16379 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/emr/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3066 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/emr/emr_step_main.py
+-rw-r--r--   0 root         (0) root         (0)      489 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/emr/main.py.template
+-rw-r--r--   0 root         (0) root         (0)    19626 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/emr/pyspark_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/emr/types.py
+-rw-r--r--   0 root         (0) root         (0)      607 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/emr/utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:10.232031 dagster-aws-1.0.5/dagster_aws/redshift/
+-rw-r--r--   0 root         (0) root         (0)      145 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/redshift/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16268 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/redshift/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:10.236032 dagster-aws-1.0.5/dagster_aws/s3/
+-rw-r--r--   0 root         (0) root         (0)      378 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/s3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8214 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/s3/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     3477 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/s3/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)     5061 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/s3/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/s3/ops.py
+-rw-r--r--   0 root         (0) root         (0)     4595 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/s3/resources.py
+-rw-r--r--   0 root         (0) root         (0)     2331 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/s3/s3_fake_resource.py
+-rw-r--r--   0 root         (0) root         (0)     1084 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/s3/sensor.py
+-rw-r--r--   0 root         (0) root         (0)      118 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/s3/solids.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/s3/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:10.240032 dagster-aws-1.0.5/dagster_aws/secretsmanager/
+-rw-r--r--   0 root         (0) root         (0)      143 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/secretsmanager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7956 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/secretsmanager/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/secretsmanager/secrets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:10.240032 dagster-aws-1.0.5/dagster_aws/utils/
+-rw-r--r--   0 root         (0) root         (0)      601 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:10.240032 dagster-aws-1.0.5/dagster_aws/utils/mrjob/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/utils/mrjob/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4421 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/utils/mrjob/log4j.py
+-rw-r--r--   0 root         (0) root         (0)     4803 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/utils/mrjob/retry.py
+-rw-r--r--   0 root         (0) root         (0)     3589 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/utils/mrjob/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/dagster_aws/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:10.216031 dagster-aws-1.0.5/dagster_aws.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      737 2022-08-26 13:44:10.000000 dagster-aws-1.0.5/dagster_aws.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1587 2022-08-26 13:44:10.000000 dagster-aws-1.0.5/dagster_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:44:10.000000 dagster-aws-1.0.5/dagster_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:44:10.000000 dagster-aws-1.0.5/dagster_aws.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      147 2022-08-26 13:44:10.000000 dagster-aws-1.0.5/dagster_aws.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-08-26 13:44:10.000000 dagster-aws-1.0.5/dagster_aws.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2022-08-26 13:44:10.244032 dagster-aws-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1772 2022-08-26 13:33:01.000000 dagster-aws-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-aws-0.9.9rc1/LICENSE` & `dagster-aws-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9rc1/dagster_aws/cloudwatch/loggers.py` & `dagster-aws-1.0.5/dagster_aws/cloudwatch/loggers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import datetime
 import logging
 
 import boto3
 
-from dagster import Field, StringSource, check, logger, seven
-from dagster.core.log_manager import coerce_valid_log_level
+from dagster import Field, StringSource
+from dagster import _check as check
+from dagster import _seven, logger
+from dagster._core.utils import coerce_valid_log_level
 
 # The maximum batch size is 1,048,576 bytes, and this size is calculated as the sum of all event
 # messages in UTF-8, plus 26 bytes for each log event.
 MAXIMUM_BATCH_SIZE = 1048576
 OVERHEAD = 26
 
 EPOCH = datetime.datetime(1970, 1, 1)
@@ -102,70 +104,71 @@
                 "{log_stream_name}".format(log_stream_name=self.log_stream_name)
             )
 
     def log_error(self, record, exc):
         logging.critical("Error while logging!")
         try:
             logging.error(
-                "Attempted to log: {record}".format(record=seven.json.dumps(record.__dict__))
+                "Attempted to log: {record}".format(record=_seven.json.dumps(record.__dict__))
             )
-        except Exception:  # pylint: disable=broad-except
+        except Exception:
             pass
         logging.exception(str(exc))
 
     def emit(self, record):
         self._emit(record, retry=False)
 
     def retry(self, record):
         self._emit(record, retry=True)
 
     def _emit(self, record, retry=False):
-        message = seven.json.dumps(record.__dict__)
+        message = _seven.json.dumps(record.__dict__)
         timestamp = millisecond_timestamp(
             datetime.datetime.strptime(record.dagster_meta["log_timestamp"], "%Y-%m-%dT%H:%M:%S.%f")
         )
         params = {
             "logGroupName": self.log_group_name,
             "logStreamName": self.log_stream_name,
             "logEvents": [{"timestamp": timestamp, "message": message}],
         }
         if self.sequence_token is not None:
             params["sequenceToken"] = self.sequence_token
 
+        res = None
         try:
             res = self.client.put_log_events(**params)
             self.sequence_token = res["nextSequenceToken"]
             log_events_rejected = res.get("rejectedLogEventsInfo")
             if log_events_rejected is not None:
                 logging.error("Cloudwatch logger: log events rejected: {res}".format(res=res))
         except self.client.exceptions.InvalidSequenceTokenException as exc:
             if not retry:
                 self.check_log_stream()
                 self.retry(record)
             else:
                 self.log_error(record, exc)
-        except self.client.exceptions.DataAlreadyAcceptedException as exc:
+        except self.client.exceptions.DataAlreadyAcceptedException:
             logging.error("Cloudwatch logger: log events already accepted: {res}".format(res=res))
-        except self.client.exceptions.InvalidParameterException as exc:
+        except self.client.exceptions.InvalidParameterException:
             logging.error(
                 "Cloudwatch logger: Invalid parameter exception while logging: {res}".format(
                     res=res
                 )
             )
-        except self.client.exceptions.ResourceNotFoundException as exc:
+        except self.client.exceptions.ResourceNotFoundException:
             logging.error(
                 "Cloudwatch logger: Resource not found. Check that the log stream or log group "
                 "was not deleted: {res}".format(res=res)
             )
-        except self.client.exceptions.ServiceUnavailableException as exc:
+        except self.client.exceptions.ServiceUnavailableException:
             if not retry:
                 self.retry(record)
             else:
                 logging.error("Cloudwatch logger: Service unavailable: {res}".format(res=res))
-        except self.client.exceptions.ServiceUnavailableException as exc:
+        except self.client.exceptions.ServiceUnavailableException:
             if not retry:
                 self.retry(record)
             else:
                 logging.error(
                     "Cloudwatch logger: Unrecognized client. Check your AWS access key id and "
                     "secret key: {res}".format(res=res)
                 )
@@ -191,39 +194,38 @@
 def cloudwatch_logger(init_context):
     """This logger provides support for sending Dagster logs to AWS CloudWatch.
 
     Example:
 
         .. code-block:: python
 
-            from dagster import ModeDefinition, execute_pipeline, pipeline, solid
+            from dagster import job, op
             from dagster_aws.cloudwatch import cloudwatch_logger
 
-            @solid
-            def hello_cloudwatch(context):
+            @op
+            def hello_op(context):
                 context.log.info('Hello, Cloudwatch!')
                 context.log.error('This is an error')
 
-            @pipeline(mode_defs=[ModeDefinition(logger_defs={'cloudwatch': cloudwatch_logger})])
-            def hello_cloudwatch_pipeline():
-                hello_cloudwatch()
-
-            execute_pipeline(
-                hello_cloudwatch_pipeline,
-                {
+            @job(logger_defs={'cloudwatch': cloudwatch_logger})
+            def hello_cloudwatch():
+                hello_op()
+
+            hello_cloudwatch.execute_in_process(
+                run_config={
                     'loggers': {
                         'cloudwatch': {
                             'config': {
                                 'log_group_name': '/dagster-test/test-cloudwatch-logging',
                                 'log_stream_name': 'test-logging',
                                 'aws_region': 'us-west-1'
                             }
                         }
                     }
-                },
+                }
             )
     """
     level = coerce_valid_log_level(init_context.logger_config["log_level"])
     name = init_context.logger_config["name"]
 
     klass = logging.getLoggerClass()
     logger_ = klass(name, level=level)
```

### Comparing `dagster-aws-0.9.9rc1/dagster_aws/emr/configs.py` & `dagster-aws-1.0.5/dagster_aws/emr/configs.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9rc1/dagster_aws/emr/emr.py` & `dagster-aws-1.0.5/dagster_aws/emr/emr.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import gzip
 import re
 from io import BytesIO
+from urllib.parse import urlparse
 
 import boto3
-import six
 from botocore.exceptions import WaiterError
 from dagster_aws.utils.mrjob.utils import _boto3_now, _wrap_aws_client, strip_microseconds
 
 import dagster
-from dagster import check
-from dagster.seven import urlparse
+import dagster._check as check
 
 from .types import EMR_CLUSTER_TERMINATED_STATES, EmrClusterState, EmrStepState
 
 # if we can't create or find our own service role, use the one
 # created by the AWS console and CLI
 _FALLBACK_SERVICE_ROLE = "EMR_DefaultRole"
 
@@ -46,15 +45,19 @@
 
 class EmrError(Exception):
     pass
 
 
 class EmrJobRunner:
     def __init__(
-        self, region, check_cluster_every=30, aws_access_key_id=None, aws_secret_access_key=None,
+        self,
+        region,
+        check_cluster_every=30,
+        aws_access_key_id=None,
+        aws_secret_access_key=None,
     ):
         """This object encapsulates various utilities for interacting with EMR clusters and invoking
         steps (jobs) on them.
 
         See also :py:class:`~dagster_aws.emr.EmrPySparkResource`, which wraps this job runner in a
         resource for pyspark workloads.
 
@@ -183,15 +186,16 @@
             % (", ".join("%s=%r" % (k, v) for k, v in sorted(cluster_config.items())))
         )
         cluster_id = emr_client.run_job_flow(**cluster_config)["JobFlowId"]
 
         log.info("Created new cluster %s" % cluster_id)
 
         # set EMR tags for the cluster
-        tags = cluster_config.get("Tags", {})
+        tags_items = cluster_config.get("Tags", [])
+        tags = {k: v for k, v in tags_items}
         tags["__dagster_version"] = dagster.__version__
         self.add_tags(log, tags, cluster_id)
         return cluster_id
 
     def describe_cluster(self, cluster_id):
         """Thin wrapper over boto3 describe_cluster.
 
@@ -408,17 +412,16 @@
         try:
             waiter.wait(
                 Bucket=log_bucket,
                 Key=log_key,
                 WaiterConfig={"Delay": waiter_delay, "MaxAttempts": waiter_max_attempts},
             )
         except WaiterError as err:
-            six.raise_from(
-                EmrError("EMR log file did not appear on S3 after waiting"), err,
-            )
+            raise EmrError("EMR log file did not appear on S3 after waiting") from err
+
         obj = BytesIO(s3.get_object(Bucket=log_bucket, Key=log_key)["Body"].read())
         gzip_file = gzip.GzipFile(fileobj=obj)
         return gzip_file.read().decode("utf-8")
 
 
 def _get_reason(cluster_or_step):
     """Get state change reason message."""
```

### Comparing `dagster-aws-0.9.9rc1/dagster_aws/emr/emr_step_main.py` & `dagster-aws-1.0.5/dagster_aws/emr/emr_step_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,20 @@
 import time
 from queue import Empty, Queue
 from threading import Thread
 
 import boto3
 from dagster_aws.s3.file_manager import S3FileHandle, S3FileManager
 
-from dagster.core.execution.plan.external_step import PICKLED_EVENTS_FILE_NAME, run_step_from_ref
-from dagster.core.instance import DagsterInstance
+from dagster._core.execution.plan.external_step import (
+    PICKLED_EVENTS_FILE_NAME,
+    external_instance_from_step_run_ref,
+    run_step_from_ref,
+)
+from dagster._serdes import serialize_value
 
 DONE = object()
 
 
 def main(step_run_ref_bucket, s3_dir_key):
     session = boto3.client("s3")
     file_manager = S3FileManager(session, step_run_ref_bucket, "")
@@ -23,32 +27,35 @@
 
     step_run_ref = pickle.loads(step_run_ref_data)
 
     events_bucket = step_run_ref_bucket
     events_s3_key = os.path.dirname(s3_dir_key) + "/" + PICKLED_EVENTS_FILE_NAME
 
     def put_events(events):
-        file_obj = io.BytesIO(pickle.dumps(events))
+        file_obj = io.BytesIO(pickle.dumps(serialize_value(events)))
         session.put_object(Body=file_obj, Bucket=events_bucket, Key=events_s3_key)
 
     # Set up a thread to handle writing events back to the plan process, so execution doesn't get
     # blocked on remote communication
     events_queue = Queue()
     event_writing_thread = Thread(
-        target=event_writing_loop, kwargs=dict(events_queue=events_queue, put_events_fn=put_events),
+        target=event_writing_loop,
+        kwargs=dict(events_queue=events_queue, put_events_fn=put_events),
     )
     event_writing_thread.start()
 
-    with DagsterInstance.ephemeral() as instance:
-        try:
-            for event in run_step_from_ref(step_run_ref, instance):
-                events_queue.put(event)
-        finally:
-            events_queue.put(DONE)
-            event_writing_thread.join()
+    try:
+        instance = external_instance_from_step_run_ref(
+            step_run_ref, event_listener_fn=events_queue.put
+        )
+        # consume iterator
+        list(run_step_from_ref(step_run_ref, instance))
+    finally:
+        events_queue.put(DONE)
+        event_writing_thread.join()
 
 
 def event_writing_loop(events_queue, put_events_fn):
     """
     Periodically check whether the step has posted any new events to the queue.  If they have,
     write ALL events (not just the new events) to an S3 bucket.
```

### Comparing `dagster-aws-0.9.9rc1/dagster_aws/emr/types.py` & `dagster-aws-1.0.5/dagster_aws/emr/types.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9rc1/dagster_aws/emr/utils.py` & `dagster-aws-1.0.5/dagster_aws/emr/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 
-from dagster import check
+import dagster._check as check
 
 
 def subset_run_config(run_config, solid_name):
     """Drops solid config for solids other than solid_name; this subsetting is required when
     executing a single solid on EMR to pass config validation.
     """
     check.dict_param(run_config, "run_config")
```

### Comparing `dagster-aws-0.9.9rc1/dagster_aws/redshift/resources.py` & `dagster-aws-1.0.5/dagster_aws/redshift/resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import abc
 from contextlib import contextmanager
 
 import psycopg2
 import psycopg2.extensions
-import six
 
-from dagster import Field, IntSource, StringSource, check, resource
+from dagster import Field, IntSource, StringSource
+from dagster import _check as check
+from dagster import resource
 
 
 class RedshiftError(Exception):
     pass
 
 
-class _BaseRedshiftResource(six.with_metaclass(abc.ABCMeta)):
+class _BaseRedshiftResource(abc.ABC):
     def __init__(self, context):  # pylint: disable=too-many-locals
         # Extract parameters from resource config
         self.conn_args = {
             k: context.resource_config.get(k)
             for k in (
                 "host",
                 "port",
@@ -27,15 +28,15 @@
                 "connect_timeout",
                 "sslmode",
             )
             if context.resource_config.get(k) is not None
         }
 
         self.autocommit = context.resource_config.get("autocommit")
-        self.log = context.log_manager
+        self.log = context.log
 
     @abc.abstractmethod
     def execute_query(self, query, fetch_results=False, cursor_factory=None, error_callback=None):
         pass
 
     @abc.abstractmethod
     def execute_queries(
@@ -64,31 +65,31 @@
 
         Returns:
             Optional[List[Tuple[Any, ...]]]: Results of the query, as a list of tuples, when
                 fetch_results is set. Otherwise return None.
         """
         check.str_param(query, "query")
         check.bool_param(fetch_results, "fetch_results")
-        check.opt_subclass_param(cursor_factory, "cursor_factory", psycopg2.extensions.cursor)
+        check.opt_class_param(
+            cursor_factory, "cursor_factory", superclass=psycopg2.extensions.cursor
+        )
         check.opt_callable_param(error_callback, "error_callback")
 
         with self._get_conn() as conn:
             with self._get_cursor(conn, cursor_factory=cursor_factory) as cursor:
                 try:
-                    six.ensure_str(query)
-
                     self.log.info("Executing query '{query}'".format(query=query))
                     cursor.execute(query)
 
                     if fetch_results and cursor.rowcount > 0:
                         return cursor.fetchall()
                     else:
                         self.log.info("Empty result from query")
 
-                except Exception as e:  # pylint: disable=broad-except
+                except Exception as e:
                     # If autocommit is disabled or not set (it is disabled by default), Redshift
                     # will be in the middle of a transaction at exception time, and because of
                     # the failure the current transaction will not accept any further queries.
                     #
                     # This conn.commit() call closes the open transaction before handing off
                     # control to the error callback, so that the user can issue additional
                     # queries. Notably, for e.g. pg_last_copy_id() to work, it requires you to
@@ -124,34 +125,34 @@
 
         Returns:
             Optional[List[List[Tuple[Any, ...]]]]: Results of the query, as a list of list of
                 tuples, when fetch_results is set. Otherwise return None.
         """
         check.list_param(queries, "queries", of_type=str)
         check.bool_param(fetch_results, "fetch_results")
-        check.opt_subclass_param(cursor_factory, "cursor_factory", psycopg2.extensions.cursor)
+        check.opt_class_param(
+            cursor_factory, "cursor_factory", superclass=psycopg2.extensions.cursor
+        )
         check.opt_callable_param(error_callback, "error_callback")
 
         results = []
         with self._get_conn() as conn:
             with self._get_cursor(conn, cursor_factory=cursor_factory) as cursor:
                 for query in queries:
-                    six.ensure_str(query)
-
                     try:
                         self.log.info("Executing query '{query}'".format(query=query))
                         cursor.execute(query)
 
                         if fetch_results and cursor.rowcount > 0:
                             results.append(cursor.fetchall())
                         else:
                             results.append([])
                             self.log.info("Empty result from query")
 
-                    except Exception as e:  # pylint: disable=broad-except
+                    except Exception as e:
                         # If autocommit is disabled or not set (it is disabled by default), Redshift
                         # will be in the middle of a transaction at exception time, and because of
                         # the failure the current transaction will not accept any further queries.
                         #
                         # This conn.commit() call closes the open transaction before handing off
                         # control to the error callback, so that the user can issue additional
                         # queries. Notably, for e.g. pg_last_copy_id() to work, it requires you to
@@ -166,23 +167,27 @@
                             raise
 
         if fetch_results:
             return results
 
     @contextmanager
     def _get_conn(self):
+        conn = None
         try:
             conn = psycopg2.connect(**self.conn_args)
             yield conn
         finally:
-            conn.close()
+            if conn:
+                conn.close()
 
     @contextmanager
     def _get_cursor(self, conn, cursor_factory=None):
-        check.opt_subclass_param(cursor_factory, "cursor_factory", psycopg2.extensions.cursor)
+        check.opt_class_param(
+            cursor_factory, "cursor_factory", superclass=psycopg2.extensions.cursor
+        )
 
         # Could be none, in which case we should respect the connection default. Otherwise
         # explicitly set to true/false.
         if self.autocommit is not None:
             conn.autocommit = self.autocommit
 
         with conn:
@@ -217,15 +222,17 @@
 
         Returns:
             Optional[List[Tuple[Any, ...]]]: Results of the query, as a list of tuples, when
                 fetch_results is set. Otherwise return None.
         """
         check.str_param(query, "query")
         check.bool_param(fetch_results, "fetch_results")
-        check.opt_subclass_param(cursor_factory, "cursor_factory", psycopg2.extensions.cursor)
+        check.opt_class_param(
+            cursor_factory, "cursor_factory", superclass=psycopg2.extensions.cursor
+        )
         check.opt_callable_param(error_callback, "error_callback")
 
         self.log.info("Executing query '{query}'".format(query=query))
         if fetch_results:
             return self.QUERY_RESULT
 
     def execute_queries(
@@ -248,15 +255,17 @@
 
         Returns:
             Optional[List[List[Tuple[Any, ...]]]]: Results of the query, as a list of list of
                 tuples, when fetch_results is set. Otherwise return None.
         """
         check.list_param(queries, "queries", of_type=str)
         check.bool_param(fetch_results, "fetch_results")
-        check.opt_subclass_param(cursor_factory, "cursor_factory", psycopg2.extensions.cursor)
+        check.opt_class_param(
+            cursor_factory, "cursor_factory", superclass=psycopg2.extensions.cursor
+        )
         check.opt_callable_param(error_callback, "error_callback")
 
         for query in queries:
             self.log.info("Executing query '{query}'".format(query=query))
         if fetch_results:
             return [self.QUERY_RESULT] * 3
 
@@ -269,18 +278,22 @@
 
     return {
         "host": Field(StringSource, description="Redshift host", is_required=True),
         "port": Field(
             IntSource, description="Redshift port", is_required=False, default_value=5439
         ),
         "user": Field(
-            StringSource, description="Username for Redshift connection", is_required=False,
+            StringSource,
+            description="Username for Redshift connection",
+            is_required=False,
         ),
         "password": Field(
-            StringSource, description="Password for Redshift connection", is_required=False,
+            StringSource,
+            description="Password for Redshift connection",
+            is_required=False,
         ),
         "database": Field(
             StringSource,
             description="Name of the default database to use. After login, you can use USE DATABASE"
             " to change the database.",
             is_required=False,
         ),
@@ -320,39 +333,30 @@
     """This resource enables connecting to a Redshift cluster and issuing queries against that
     cluster.
 
     Example:
 
         .. code-block:: python
 
-            from dagster import ModeDefinition, execute_solid, solid
+            from dagster import build_op_context, op
             from dagster_aws.redshift import redshift_resource
 
-            @solid(required_resource_keys={'redshift'})
-            def example_redshift_solid(context):
+            @op(required_resource_keys={'redshift'})
+            def example_redshift_op(context):
                 return context.resources.redshift.execute_query('SELECT 1', fetch_results=True)
 
-            result = execute_solid(
-                example_redshift_solid,
-                run_config={
-                    'resources': {
-                        'redshift': {
-                            'config': {
-                                'host': 'my-redshift-cluster.us-east-1.redshift.amazonaws.com',
-                                'port': 5439,
-                                'user': 'dagster',
-                                'password': 'dagster',
-                                'database': 'dev',
-                            }
-                        }
-                    }
-                },
-                mode_def=ModeDefinition(resource_defs={'redshift': redshift_resource}),
-            )
-            assert result.output_value() == [(1,)]
+            redshift_configured = redshift_resource.configured({
+                'host': 'my-redshift-cluster.us-east-1.redshift.amazonaws.com',
+                'port': 5439,
+                'user': 'dagster',
+                'password': 'dagster',
+                'database': 'dev',
+            })
+            context = build_op_context(resources={'redshift': redshift_configured})
+            assert example_redshift_op(context) == [(1,)]
 
     """
     return RedshiftResource(context)
 
 
 @resource(
     config_schema=define_redshift_config(),
```

### Comparing `dagster-aws-0.9.9rc1/dagster_aws/s3/compute_log_manager.py` & `dagster-aws-1.0.5/dagster_aws/s3/compute_log_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import os
 from contextlib import contextmanager
 
 import boto3
+from botocore.errorfactory import ClientError
 
-from dagster import Field, StringSource, check, seven
-from dagster.core.storage.compute_log_manager import (
+import dagster._seven as seven
+from dagster import Field, StringSource
+from dagster import _check as check
+from dagster._core.storage.compute_log_manager import (
     MAX_BYTES_FILE_READ,
     ComputeIOType,
     ComputeLogFileData,
     ComputeLogManager,
 )
-from dagster.core.storage.local_compute_log_manager import IO_TYPE_EXTENSION, LocalComputeLogManager
-from dagster.serdes import ConfigurableClass, ConfigurableClassData
-from dagster.utils import ensure_dir, ensure_file
+from dagster._core.storage.local_compute_log_manager import (
+    IO_TYPE_EXTENSION,
+    LocalComputeLogManager,
+)
+from dagster._serdes import ConfigurableClass, ConfigurableClassData
+from dagster._utils import ensure_dir, ensure_file
 
 
 class S3ComputeLogManager(ComputeLogManager, ConfigurableClass):
-    """Logs solid compute function stdout and stderr to S3.
+    """Logs compute function stdout and stderr to S3.
 
     Users should not instantiate this class directly. Instead, use a YAML block in ``dagster.yaml``
     such as the following:
 
     .. code-block:: YAML
 
         compute_logs:
@@ -30,54 +36,57 @@
             bucket: "mycorp-dagster-compute-logs"
             local_dir: "/tmp/cool"
             prefix: "dagster-test-"
             use_ssl: true
             verify: true
             verify_cert_path: "/path/to/cert/bundle.pem"
             endpoint_url: "http://alternate-s3-host.io"
+            skip_empty_files: true
 
     Args:
         bucket (str): The name of the s3 bucket to which to log.
         local_dir (Optional[str]): Path to the local directory in which to stage logs. Default:
-            ``dagster.seven.get_system_temp_directory()``.
+            ``dagster._seven.get_system_temp_directory()``.
         prefix (Optional[str]): Prefix for the log file keys.
         use_ssl (Optional[bool]): Whether or not to use SSL. Default True.
         verify (Optional[bool]): Whether or not to verify SSL certificates. Default True.
         verify_cert_path (Optional[str]): A filename of the CA cert bundle to use. Only used if
             `verify` set to False.
         endpoint_url (Optional[str]): Override for the S3 endpoint url.
+        skip_empty_files: (Optional[bool]): Skip upload of empty log files.
         inst_data (Optional[ConfigurableClassData]): Serializable representation of the compute
             log manager when newed up from config.
     """
 
     def __init__(
         self,
         bucket,
         local_dir=None,
         inst_data=None,
         prefix="dagster",
         use_ssl=True,
         verify=True,
         verify_cert_path=None,
         endpoint_url=None,
+        skip_empty_files=False,
     ):
         _verify = False if not verify else verify_cert_path
         self._s3_session = boto3.resource(
             "s3", use_ssl=use_ssl, verify=_verify, endpoint_url=endpoint_url
         ).meta.client
         self._s3_bucket = check.str_param(bucket, "bucket")
         self._s3_prefix = check.str_param(prefix, "prefix")
-        self._download_urls = {}
 
         # proxy calls to local compute log manager (for subscriptions, etc)
         if not local_dir:
             local_dir = seven.get_system_temp_directory()
 
         self.local_manager = LocalComputeLogManager(local_dir)
         self._inst_data = check.opt_inst_param(inst_data, "inst_data", ConfigurableClassData)
+        self._skip_empty_files = check.bool_param(skip_empty_files, "skip_empty_files")
 
     @contextmanager
     def _watch_logs(self, pipeline_run, step_key=None):
         # proxy watching to the local compute log manager, interacting with the filesystem
         with self.local_manager._watch_logs(  # pylint: disable=protected-access
             pipeline_run, step_key
         ):
@@ -93,14 +102,15 @@
             "bucket": StringSource,
             "local_dir": Field(StringSource, is_required=False),
             "prefix": Field(StringSource, is_required=False, default_value="dagster"),
             "use_ssl": Field(bool, is_required=False, default_value=True),
             "verify": Field(bool, is_required=False, default_value=True),
             "verify_cert_path": Field(StringSource, is_required=False),
             "endpoint_url": Field(StringSource, is_required=False),
+            "skip_empty_files": Field(bool, is_required=False, default_value=False),
         }
 
     @staticmethod
     def from_config_value(inst_data, config_value):
         return S3ComputeLogManager(inst_data=inst_data, **config_value)
 
     def get_local_path(self, run_id, key, io_type):
@@ -118,39 +128,46 @@
     def is_watch_completed(self, run_id, key):
         return self.local_manager.is_watch_completed(run_id, key)
 
     def download_url(self, run_id, key, io_type):
         if not self.is_watch_completed(run_id, key):
             return self.local_manager.download_url(run_id, key, io_type)
         key = self._bucket_key(run_id, key, io_type)
-        if key in self._download_urls:
-            return self._download_urls[key]
+
         url = self._s3_session.generate_presigned_url(
             ClientMethod="get_object", Params={"Bucket": self._s3_bucket, "Key": key}
         )
-        self._download_urls[key] = url
+
         return url
 
     def read_logs_file(self, run_id, key, io_type, cursor=0, max_bytes=MAX_BYTES_FILE_READ):
         if self._should_download(run_id, key, io_type):
             self._download_to_local(run_id, key, io_type)
         data = self.local_manager.read_logs_file(run_id, key, io_type, cursor, max_bytes)
         return self._from_local_file_data(run_id, key, io_type, data)
 
     def on_subscribe(self, subscription):
         self.local_manager.on_subscribe(subscription)
 
+    def on_unsubscribe(self, subscription):
+        self.local_manager.on_unsubscribe(subscription)
+
     def _should_download(self, run_id, key, io_type):
         local_path = self.get_local_path(run_id, key, io_type)
         if os.path.exists(local_path):
             return False
-        s3_objects = self._s3_session.list_objects(
-            Bucket=self._s3_bucket, Prefix=self._bucket_key(run_id, key, io_type)
-        )
-        return len(s3_objects) > 0
+
+        try:  # https://stackoverflow.com/a/38376288/14656695
+            self._s3_session.head_object(
+                Bucket=self._s3_bucket, Key=self._bucket_key(run_id, key, io_type)
+            )
+        except ClientError:
+            return False
+
+        return True
 
     def _from_local_file_data(self, run_id, key, io_type, local_file_data):
         is_complete = self.is_watch_completed(run_id, key)
         path = (
             "s3://{}/{}".format(self._s3_bucket, self._bucket_key(run_id, key, io_type))
             if is_complete
             else local_file_data.path
@@ -163,14 +180,17 @@
             local_file_data.size,
             self.download_url(run_id, key, io_type),
         )
 
     def _upload_from_local(self, run_id, key, io_type):
         path = self.get_local_path(run_id, key, io_type)
         ensure_file(path)
+        if self._skip_empty_files and os.stat(path).st_size == 0:
+            return
+
         key = self._bucket_key(run_id, key, io_type)
         with open(path, "rb") as data:
             self._s3_session.upload_fileobj(data, self._s3_bucket, key)
 
     def _download_to_local(self, run_id, key, io_type):
         path = self.get_local_path(run_id, key, io_type)
         ensure_dir(os.path.dirname(path))
@@ -186,7 +206,10 @@
             self._s3_prefix,
             "storage",
             run_id,
             "compute_logs",
             "{}.{}".format(key, extension),
         ]
         return "/".join(paths)  # s3 path delimiter
+
+    def dispose(self):
+        self.local_manager.dispose()
```

### Comparing `dagster-aws-0.9.9rc1/dagster_aws/s3/file_manager.py` & `dagster-aws-1.0.5/dagster_aws/s3/file_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 import io
 import uuid
 from contextlib import contextmanager
 
-from dagster import check, usable_as_dagster_type
-from dagster.core.storage.file_manager import (
+import dagster._check as check
+from dagster._core.storage.file_manager import (
     FileHandle,
     FileManager,
     TempfileManager,
     check_file_like_obj,
 )
 
 
-@usable_as_dagster_type
 class S3FileHandle(FileHandle):
-    def __init__(self, s3_bucket, s3_key):
+    """A reference to a file on S3."""
+
+    def __init__(self, s3_bucket: str, s3_key: str):
         self._s3_bucket = check.str_param(s3_bucket, "s3_bucket")
         self._s3_key = check.str_param(s3_key, "s3_key")
 
     @property
-    def s3_bucket(self):
+    def s3_bucket(self) -> str:
+        """str: The name of the S3 bucket."""
         return self._s3_bucket
 
     @property
-    def s3_key(self):
+    def s3_key(self) -> str:
+        """str: The S3 key."""
         return self._s3_key
 
     @property
-    def path_desc(self):
+    def path_desc(self) -> str:
+        """str: The file's S3 URL."""
         return self.s3_path
 
     @property
-    def s3_path(self):
+    def s3_path(self) -> str:
+        """str: The file's S3 URL."""
         return "s3://{bucket}/{key}".format(bucket=self.s3_bucket, key=self.s3_key)
 
 
 class S3FileManager(FileManager):
     def __init__(self, s3_session, s3_bucket, s3_base_key):
         self._s3_session = s3_session
         self._s3_bucket = check.str_param(s3_bucket, "s3_bucket")
@@ -62,15 +67,16 @@
     def read(self, file_handle, mode="rb"):
         check.inst_param(file_handle, "file_handle", S3FileHandle)
         check.str_param(mode, "mode")
         check.param_invariant(mode in {"r", "rb"}, "mode")
 
         self._download_if_not_cached(file_handle)
 
-        with open(self._get_local_path(file_handle), mode) as file_obj:
+        encoding = None if mode == "rb" else "utf-8"
+        with open(self._get_local_path(file_handle), mode, encoding=encoding) as file_obj:
             yield file_obj
 
     def _file_handle_cached(self, file_handle):
         return file_handle.s3_path in self._local_handle_cache
 
     def _get_local_path(self, file_handle):
         return self._local_handle_cache[file_handle.s3_path]
```

### Comparing `dagster-aws-0.9.9rc1/dagster_aws/s3/resources.py` & `dagster-aws-1.0.5/dagster_aws/s3/resources.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,69 +1,82 @@
-import boto3
-from botocore.handlers import disable_signing
-
 from dagster import Field, StringSource, resource
-from dagster.utils.merger import merge_dicts
+from dagster._utils.merger import merge_dicts
 
 from .file_manager import S3FileManager
+from .utils import construct_s3_client
 
 S3_SESSION_CONFIG = {
     "use_unsigned_session": Field(
         bool,
         description="Specifies whether to use an unsigned S3 session",
         is_required=False,
         default_value=False,
     ),
     "region_name": Field(
         str, description="Specifies a custom region for the S3 session", is_required=False
     ),
     "endpoint_url": Field(
-        str, description="Specifies a custom endpoint for the S3 session", is_required=False
+        StringSource,
+        description="Specifies a custom endpoint for the S3 session",
+        is_required=False,
+    ),
+    "max_attempts": Field(
+        int,
+        description="This provides Boto3's retry handler with a value of maximum retry attempts, "
+        "where the initial call counts toward the max_attempts value that you provide",
+        is_required=False,
+        default_value=5,
+    ),
+    "profile_name": Field(
+        str,
+        description="Specifies a profile to connect that session",
+        is_required=False,
     ),
 }
 
 
 @resource(S3_SESSION_CONFIG)
 def s3_resource(context):
-    """Resource that gives solids access to S3.
-
-    The underlying S3 session is created by calling :py:func:`boto3.resource('s3') <boto3:boto3.resource>`.
+    """Resource that gives access to S3.
 
-    Attach this resource definition to a :py:class:`~dagster.ModeDefinition` in order to make it
-    available to your solids.
+    The underlying S3 session is created by calling
+    :py:func:`boto3.session.Session(profile_name) <boto3:boto3.session>`.
+    The returned resource object is an S3 client, an instance of `botocore.client.S3`.
 
     Example:
 
         .. code-block:: python
 
-            from dagster import ModeDefinition, execute_solid, solid
+            from dagster import build_op_context, job, op
             from dagster_aws.s3 import s3_resource
 
-            @solid(required_resource_keys={'s3'})
-            def example_s3_solid(context):
+            @op(required_resource_keys={'s3'})
+            def example_s3_op(context):
                 return context.resources.s3.list_objects_v2(
                     Bucket='my-bucket',
                     Prefix='some-key'
                 )
 
-            result = execute_solid(
-                example_s3_solid,
+            @job(resource_defs={'s3': s3_resource})
+            def example_job(context):
+                example_s3_op()
+
+            example_job.execute_in_process(
                 run_config={
                     'resources': {
                         's3': {
                             'config': {
                                 'region_name': 'us-west-1',
                             }
                         }
                     }
-                },
-                mode_def=ModeDefinition(resource_defs={'s3': s3_resource}),
+                }
             )
 
-    Note that your solids must also declare that they require this resource with
+    Note that your ops must also declare that they require this resource with
     `required_resource_keys`, or it will not be initialized for the execution of their compute
     functions.
 
     You may configure this resource as follows:
 
     .. code-block:: YAML
 
@@ -73,57 +86,46 @@
               region_name: "us-west-1"
               # Optional[str]: Specifies a custom region for the S3 session. Default is chosen
               # through the ordinary boto credential chain.
               use_unsigned_session: false
               # Optional[bool]: Specifies whether to use an unsigned S3 session. Default: True
               endpoint_url: "http://localhost"
               # Optional[str]: Specifies a custom endpoint for the S3 session. Default is None.
+              profile_name: "dev"
+              # Optional[str]: Specifies a custom profile for S3 session. Default is default
+              # profile as specified in ~/.aws/credentials file
+
     """
-    use_unsigned_session = context.resource_config["use_unsigned_session"]
-    region_name = context.resource_config.get("region_name")
-    endpoint_url = context.resource_config.get("endpoint_url")
-
-    s3 = boto3.resource(  # pylint:disable=C0103
-        "s3", region_name=region_name, use_ssl=True, endpoint_url=endpoint_url
-    ).meta.client
-
-    if use_unsigned_session:
-        s3.meta.events.register("choose-signer.s3.*", disable_signing)
-    return s3
+    return construct_s3_client(
+        max_attempts=context.resource_config["max_attempts"],
+        region_name=context.resource_config.get("region_name"),
+        endpoint_url=context.resource_config.get("endpoint_url"),
+        use_unsigned_session=context.resource_config["use_unsigned_session"],
+        profile_name=context.resource_config.get("profile_name"),
+    )
 
 
 @resource(
     merge_dicts(
         S3_SESSION_CONFIG,
         {
             "s3_bucket": Field(StringSource),
             "s3_prefix": Field(StringSource, is_required=False, default_value="dagster"),
         },
     )
 )
 def s3_file_manager(context):
-    s3_session = _s3_session_from_config(context.resource_config)
+    """FileManager that provides abstract access to S3.
+
+    Implements the :py:class:`~dagster._core.storage.file_manager.FileManager` API.
+    """
     return S3FileManager(
-        s3_session=s3_session,
+        s3_session=construct_s3_client(
+            max_attempts=context.resource_config["max_attempts"],
+            region_name=context.resource_config.get("region_name"),
+            endpoint_url=context.resource_config.get("endpoint_url"),
+            use_unsigned_session=context.resource_config["use_unsigned_session"],
+            profile_name=context.resource_config.get("profile_name"),
+        ),
         s3_bucket=context.resource_config["s3_bucket"],
         s3_base_key=context.resource_config["s3_prefix"],
     )
-
-
-def _s3_session_from_config(config):
-    """
-    Args:
-        config: A configuration containing the fields in S3_SESSION_CONFIG.
-
-    Returns: A boto3 s3 session.
-    """
-    use_unsigned_session = config["use_unsigned_session"]
-    region_name = config.get("region_name")
-    endpoint_url = config.get("endpoint_url")
-
-    s3 = boto3.resource(  # pylint:disable=C0103
-        "s3", region_name=region_name, use_ssl=True, endpoint_url=endpoint_url
-    ).meta.client
-
-    if use_unsigned_session:
-        s3.meta.events.register("choose-signer.s3.*", disable_signing)
-    return s3
```

### Comparing `dagster-aws-0.9.9rc1/dagster_aws/s3/s3_fake_resource.py` & `dagster-aws-1.0.5/dagster_aws/s3/s3_fake_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 
 def create_s3_fake_resource(buckets=None):
     """Create a mock S3 session for test."""
     return S3FakeSession(buckets=buckets)
 
 
-class S3FakeSession(object):
+class S3FakeSession:
     """Stateful mock of a boto3 s3 session for test.
 
     Wraps a ``mock.MagicMock``. Buckets are implemented using an in-memory dict.
     """
 
     def __init__(self, buckets=None):
-        from dagster.seven import mock
+        from unittest import mock
 
         self.buckets = defaultdict(dict, buckets) if buckets else defaultdict(dict)
         self.mock_extras = mock.MagicMock()
 
     def head_bucket(self, Bucket, *args, **kwargs):  # pylint: disable=unused-argument
         self.mock_extras.head_bucket(*args, **kwargs)
```

### Comparing `dagster-aws-0.9.9rc1/dagster_aws/s3/solids.py` & `dagster-aws-1.0.5/dagster_aws/s3/ops.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+from typing import Dict
+
 from dagster import (
     AssetMaterialization,
-    EventMetadataEntry,
     Field,
     FileHandle,
-    InputDefinition,
+    In,
+    MetadataValue,
+    Out,
     Output,
-    OutputDefinition,
     StringSource,
-    check,
-    dagster_type_loader,
-    solid,
 )
-from dagster.core.types.dagster_type import PythonObjectDagsterType
+from dagster import _check as check
+from dagster import dagster_type_loader, op
+from dagster._core.types.dagster_type import PythonObjectDagsterType
 
 from .file_manager import S3FileHandle
 
 
-def dict_with_fields(name, fields):
+def dict_with_fields(name: str, fields: Dict[str, object]):
     check.str_param(name, "name")
     check.dict_param(fields, "fields", key_type=str)
     field_names = set(fields.keys())
 
     @dagster_type_loader(fields)
     def _input_schema(_context, value):
         check.dict_param(value, "value")
@@ -39,42 +40,42 @@
     fields={
         "bucket": Field(StringSource, description="S3 bucket name"),
         "key": Field(StringSource, description="S3 key name"),
     },
 )
 
 
-def last_key(key):
+def last_key(key: str) -> str:
     if "/" not in key:
         return key
     comps = key.split("/")
     return comps[-1]
 
 
-@solid(
+@op(
     config_schema={
         "Bucket": Field(
             StringSource, description="The name of the bucket to upload to.", is_required=True
         ),
         "Key": Field(
             StringSource, description="The name of the key to upload to.", is_required=True
         ),
     },
-    input_defs=[InputDefinition("file_handle", FileHandle, description="The file to upload.")],
-    output_defs=[OutputDefinition(name="s3_file_handle", dagster_type=S3FileHandle)],
+    ins={"file_handle": In(FileHandle, description="The file to upload.")},
+    out={"s3_file_handle": Out(S3FileHandle)},
     description="""Take a file handle and upload it to s3. Returns an S3FileHandle.""",
-    required_resource_keys={"s3"},
+    required_resource_keys={"s3", "file_manager"},
 )
 def file_handle_to_s3(context, file_handle):
     bucket = context.solid_config["Bucket"]
     key = context.solid_config["Key"]
 
-    with context.file_manager.read(file_handle, "rb") as fileobj:
+    with context.resources.file_manager.read(file_handle, "rb") as fileobj:
         context.resources.s3.upload_fileobj(fileobj, bucket, key)
         s3_file_handle = S3FileHandle(bucket, key)
 
         yield AssetMaterialization(
             asset_key=s3_file_handle.s3_path,
-            metadata_entries=[EventMetadataEntry.path(s3_file_handle.s3_path, label=last_key(key))],
+            metadata={last_key(key): MetadataValue.path(s3_file_handle.s3_path)},
         )
 
         yield Output(value=s3_file_handle, output_name="s3_file_handle")
```

### Comparing `dagster-aws-0.9.9rc1/dagster_aws/utils/mrjob/log4j.py` & `dagster-aws-1.0.5/dagster_aws/utils/mrjob/log4j.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Parse the log4j syslog format used by Hadoop."""
 import re
 from collections import namedtuple
 
-import six
-
 # log line format output by hadoop jar command
 _HADOOP_LOG4J_LINE_RE = re.compile(
     r"^\s*(?P<timestamp>\d\d\/\d\d\/\d\d \d\d\:\d\d\:\d\d)"
     r"\s+(?P<level>[A-Z]+)"
     r"\s+(?P<logger>\S+)"
     r"(\s+\((?P<thread>.*?)\))?"
     r"( - ?|: ?)"
@@ -95,15 +93,15 @@
     lines are assumed to be part of a multiline message if not pre-filtered).
     """
     last_record = None
     line_num = 0
 
     for line_num, line in enumerate(lines.split("\n")):
         # convert from bytes to unicode, if needed, and strip trailing newlines
-        line = six.ensure_str(line).rstrip("\r\n")
+        line = line.rstrip("\r\n")
 
         m = _HADOOP_LOG4J_LINE_RE.match(line) or _HADOOP_LOG4J_LINE_ALTERNATE_RE.match(line)
 
         if m:
             if last_record:
                 last_record = last_record._replace(num_lines=line_num - last_record.start_line)
                 yield last_record
```

### Comparing `dagster-aws-0.9.9rc1/dagster_aws/utils/mrjob/retry.py` & `dagster-aws-1.0.5/dagster_aws/utils/mrjob/retry.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 _DEFAULT_BACKOFF = 15
 _DEFAULT_MULTIPLIER = 1.5
 _DEFAULT_MAX_TRIES = 10
 _DEFAULT_MAX_BACKOFF = 1200  # 20 minutes
 
 
-class RetryWrapper(object):
+class RetryWrapper:
     """Handle transient errors, with configurable backoff.
 
     This class can wrap any object. The wrapped object will behave like
     the original one, except that if you call a function and it raises a
     retriable exception, we'll back off for a certain number of seconds
     and call the function again, until it succeeds or we get a non-retriable
     exception.
@@ -112,15 +112,15 @@
         def call_and_maybe_retry(*args, **kwargs):
             backoff = self.__backoff
             tries = 0
 
             while not self.__max_tries or tries < self.__max_tries:
                 try:
                     return f(*args, **kwargs)
-                except Exception as ex:  # pylint: disable=broad-except
+                except Exception as ex:
                     if self.__retry_if(ex) and (
                         tries < self.__max_tries - 1 or not self.__max_tries
                     ):
                         log.info("Got retriable error: %r" % ex)
                         log.info("Backing off for %.1f seconds" % backoff)
                         time.sleep(backoff)
                         tries += 1
```

### Comparing `dagster-aws-0.9.9rc1/dagster_aws/utils/mrjob/utils.py` & `dagster-aws-1.0.5/dagster_aws/utils/mrjob/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9rc1/dagster_aws.egg-info/SOURCES.txt` & `dagster-aws-1.0.5/dagster_aws.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,55 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 dagster_aws/__init__.py
+dagster_aws/py.typed
 dagster_aws/version.py
 dagster_aws.egg-info/PKG-INFO
 dagster_aws.egg-info/SOURCES.txt
 dagster_aws.egg-info/dependency_links.txt
 dagster_aws.egg-info/not-zip-safe
 dagster_aws.egg-info/requires.txt
 dagster_aws.egg-info/top_level.txt
+dagster_aws/athena/__init__.py
+dagster_aws/athena/resources.py
 dagster_aws/cloudwatch/__init__.py
 dagster_aws/cloudwatch/loggers.py
+dagster_aws/ecr/__init__.py
+dagster_aws/ecr/resources.py
 dagster_aws/ecs/__init__.py
-dagster_aws/ecs/client.py
+dagster_aws/ecs/container_context.py
 dagster_aws/ecs/launcher.py
+dagster_aws/ecs/tasks.py
+dagster_aws/ecs/test_utils.py
+dagster_aws/ecs/utils.py
 dagster_aws/emr/__init__.py
 dagster_aws/emr/configs.py
+dagster_aws/emr/configs_spark.py
 dagster_aws/emr/emr.py
 dagster_aws/emr/emr_step_main.py
 dagster_aws/emr/main.py.template
 dagster_aws/emr/pyspark_step_launcher.py
 dagster_aws/emr/types.py
 dagster_aws/emr/utils.py
 dagster_aws/redshift/__init__.py
 dagster_aws/redshift/resources.py
 dagster_aws/s3/__init__.py
 dagster_aws/s3/compute_log_manager.py
-dagster_aws/s3/file_cache.py
 dagster_aws/s3/file_manager.py
-dagster_aws/s3/intermediate_storage.py
-dagster_aws/s3/object_store.py
+dagster_aws/s3/io_manager.py
+dagster_aws/s3/ops.py
 dagster_aws/s3/resources.py
 dagster_aws/s3/s3_fake_resource.py
+dagster_aws/s3/sensor.py
 dagster_aws/s3/solids.py
-dagster_aws/s3/system_storage.py
 dagster_aws/s3/utils.py
+dagster_aws/secretsmanager/__init__.py
+dagster_aws/secretsmanager/resources.py
+dagster_aws/secretsmanager/secrets.py
 dagster_aws/utils/__init__.py
 dagster_aws/utils/mrjob/__init__.py
 dagster_aws/utils/mrjob/log4j.py
 dagster_aws/utils/mrjob/retry.py
-dagster_aws/utils/mrjob/utils.py
-dagster_aws_tests/__init__.py
-dagster_aws_tests/test_version.py
-dagster_aws_tests/cloudwatch_tests/__init__.py
-dagster_aws_tests/cloudwatch_tests/conftest.py
-dagster_aws_tests/cloudwatch_tests/test_loggers.py
-dagster_aws_tests/ecs_tests/__init__.py
-dagster_aws_tests/ecs_tests/test_ecs_client.py
-dagster_aws_tests/emr_tests/__init__.py
-dagster_aws_tests/emr_tests/conftest.py
-dagster_aws_tests/emr_tests/test_emr.py
-dagster_aws_tests/emr_tests/test_emr_step_main.py
-dagster_aws_tests/emr_tests/test_pyspark.py
-dagster_aws_tests/emr_tests/test_pyspark_step_launcher.py
-dagster_aws_tests/emr_tests/test_utils.py
-dagster_aws_tests/redshift_tests/__init__.py
-dagster_aws_tests/redshift_tests/conftest.py
-dagster_aws_tests/redshift_tests/test_resources.py
-dagster_aws_tests/s3_tests/__init__.py
-dagster_aws_tests/s3_tests/conftest.py
-dagster_aws_tests/s3_tests/test_compute_log_manager.py
-dagster_aws_tests/s3_tests/test_file_handle_to_s3.py
-dagster_aws_tests/s3_tests/test_intermediate_storage.py
-dagster_aws_tests/s3_tests/test_object_store.py
-dagster_aws_tests/s3_tests/test_s3_file_cache.py
-dagster_aws_tests/s3_tests/test_s3_file_manager.py
-dagster_aws_tests/utils_tests/__init__.py
-dagster_aws_tests/utils_tests/mrjob_tests/__init__.py
-dagster_aws_tests/utils_tests/mrjob_tests/test_log4j.py
-dagster_aws_tests/utils_tests/mrjob_tests/test_utils.py
+dagster_aws/utils/mrjob/utils.py
```

### Comparing `dagster-aws-0.9.9rc1/setup.py` & `dagster-aws-1.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,52 @@
+from typing import Dict
+
 from setuptools import find_packages, setup
 
 
-def get_version():
-    version = {}
-    with open("dagster_aws/version.py") as fp:
+def get_version() -> str:
+    version: Dict[str, str] = {}
+    with open("dagster_aws/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
 if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
     setup(
         name="dagster-aws",
-        version=get_version(),
+        version=ver,
         author="Elementl",
         author_email="hello@elementl.com",
         license="Apache-2.0",
         description="Package for AWS-specific Dagster framework solid and resource components.",
         url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-aws",
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
+        packages=find_packages(exclude=["dagster_aws_tests*"]),
         include_package_data=True,
-        install_requires=["boto3>=1.9", "dagster", "psycopg2-binary", "requests",],
-        extras_require={"pyspark": ["dagster-pyspark"]},
+        install_requires=[
+            "boto3",
+            "dagster==1.0.5",
+            "packaging",
+            "requests",
+        ],
+        extras_require={
+            "redshift": ["psycopg2-binary"],
+            "pyspark": ["dagster-pyspark"],
+            "test": [
+                "moto>=2.2.8",
+                "requests-mock",
+                "xmltodict==0.12.0",  # pinned until moto>=3.1.9 (https://github.com/spulec/moto/issues/5112)
+            ],
+        },
         zip_safe=False,
     )
```

