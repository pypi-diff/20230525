# Comparing `tmp/cloud2-0.1.7.tar.gz` & `tmp/cloud2-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud2-0.1.7.tar", last modified: Thu May 25 15:30:58 2023, max compression
+gzip compressed data, was "cloud2-0.1.8.tar", last modified: Thu May 25 15:34:59 2023, max compression
```

## Comparing `cloud2-0.1.7.tar` & `cloud2-0.1.8.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.653447 cloud2-0.1.7/
--rw-r--r--   0 ab         (501) staff       (20)       17 2023-05-23 16:51:20.000000 cloud2-0.1.7/MANIFEST.in
--rw-r--r--   0 ab         (501) staff       (20)     2228 2023-05-25 15:30:58.653545 cloud2-0.1.7/PKG-INFO
--rw-r--r--   0 ab         (501) staff       (20)      176 2023-05-25 15:30:58.653838 cloud2-0.1.7/setup.cfg
--rw-r--r--   0 ab         (501) staff       (20)     1161 2023-05-25 15:30:55.000000 cloud2-0.1.7/setup.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.637693 cloud2-0.1.7/src/
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.638073 cloud2-0.1.7/src/aws_services/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/aws_services/__init__.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.639022 cloud2-0.1.7/src/aws_services/api_gateway/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/aws_services/api_gateway/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1267 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/api_gateway/api_gateway_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     7883 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/api_gateway/api_gateway_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.640794 cloud2-0.1.7/src/aws_services/dat_lambda/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/dat_lambda/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)      574 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/dat_lambda/lambda_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     3854 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/dat_lambda/lambda_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.641810 cloud2-0.1.7/src/aws_services/dynamodb/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/aws_services/dynamodb/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1311 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/aws_services/dynamodb/dynamodb_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     6770 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/aws_services/dynamodb/dynamodb_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.642702 cloud2-0.1.7/src/aws_services/emr/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/aws_services/emr/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1537 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/emr/emr_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10580 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/emr/emr_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.643505 cloud2-0.1.7/src/aws_services/fargate/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/aws_services/fargate/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1459 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/fargate/fargate_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10989 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/fargate/fargate_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.644201 cloud2-0.1.7/src/aws_services/glue/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/aws_services/glue/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2141 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/glue/glue_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    15754 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/glue/glue_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.644869 cloud2-0.1.7/src/aws_services/kinesis_firehose/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/aws_services/kinesis_firehose/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)      964 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/kinesis_firehose/firehose_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     5882 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/kinesis_firehose/kinesis_firehose_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.645610 cloud2-0.1.7/src/aws_services/kinesis_stream/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/kinesis_stream/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1085 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/kinesis_stream/kinesis_stream_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     5542 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/kinesis_stream/kinesis_stream_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.646358 cloud2-0.1.7/src/aws_services/rds/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/aws_services/rds/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2663 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/rds/rds_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    13762 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/rds/rds_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.647126 cloud2-0.1.7/src/aws_services/redshift/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/redshift/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2922 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/redshift/redshift_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    13529 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/aws_services/redshift/redshift_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.647836 cloud2-0.1.7/src/aws_services/s3/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/s3/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2146 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/s3/s3_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    11711 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/s3/s3_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.648440 cloud2-0.1.7/src/aws_services/ses/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/aws_services/ses/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1808 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/aws_services/ses/ses_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10018 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/aws_services/ses/ses_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.649218 cloud2-0.1.7/src/aws_services/sns/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/aws_services/sns/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1907 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/aws_services/sns/sns_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    11294 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/aws_services/sns/sns_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.649853 cloud2-0.1.7/src/aws_services/sqs/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/sqs/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2360 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/aws_services/sqs/sqs_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10990 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/aws_services/sqs/sqs_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.650875 cloud2-0.1.7/src/cloud2.egg-info/
--rw-r--r--   0 ab         (501) staff       (20)     2228 2023-05-25 15:30:58.000000 cloud2-0.1.7/src/cloud2.egg-info/PKG-INFO
--rw-r--r--   0 ab         (501) staff       (20)     2326 2023-05-25 15:30:58.000000 cloud2-0.1.7/src/cloud2.egg-info/SOURCES.txt
--rw-r--r--   0 ab         (501) staff       (20)        1 2023-05-25 15:30:58.000000 cloud2-0.1.7/src/cloud2.egg-info/dependency_links.txt
--rw-r--r--   0 ab         (501) staff       (20)       74 2023-05-25 15:30:58.000000 cloud2-0.1.7/src/cloud2.egg-info/entry_points.txt
--rw-r--r--   0 ab         (501) staff       (20)      114 2023-05-25 15:30:58.000000 cloud2-0.1.7/src/cloud2.egg-info/requires.txt
--rw-r--r--   0 ab         (501) staff       (20)       25 2023-05-25 15:30:58.000000 cloud2-0.1.7/src/cloud2.egg-info/top_level.txt
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.651023 cloud2-0.1.7/src/common/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/common/__init__.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.651306 cloud2-0.1.7/src/common/constants/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/common/constants/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2428 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/common/constants/application_constants.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.651636 cloud2-0.1.7/src/common/service/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/common/service/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     6395 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/common/service/dat_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:30:58.652950 cloud2-0.1.7/src/common/utils/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/common/utils/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)    10345 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/common/utils/helper.py
--rw-r--r--   0 ab         (501) staff       (20)      188 2023-05-11 06:33:05.000000 cloud2-0.1.7/src/common/utils/initialize_logger.py
--rw-r--r--   0 ab         (501) staff       (20)     1624 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/common/utils/instance_initializer.py
--rw-r--r--   0 ab         (501) staff       (20)     3206 2023-05-23 16:51:20.000000 cloud2-0.1.7/src/main.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.595113 cloud2-0.1.8/
+-rw-r--r--   0 ab         (501) staff       (20)       17 2023-05-23 16:51:20.000000 cloud2-0.1.8/MANIFEST.in
+-rw-r--r--   0 ab         (501) staff       (20)     2226 2023-05-25 15:34:59.595201 cloud2-0.1.8/PKG-INFO
+-rw-r--r--   0 ab         (501) staff       (20)      176 2023-05-25 15:34:59.595540 cloud2-0.1.8/setup.cfg
+-rw-r--r--   0 ab         (501) staff       (20)     1159 2023-05-25 15:34:53.000000 cloud2-0.1.8/setup.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.585881 cloud2-0.1.8/src/
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.586067 cloud2-0.1.8/src/aws_services/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/aws_services/__init__.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.586511 cloud2-0.1.8/src/aws_services/api_gateway/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/aws_services/api_gateway/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1267 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/api_gateway/api_gateway_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     7883 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/api_gateway/api_gateway_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.587086 cloud2-0.1.8/src/aws_services/dat_lambda/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/dat_lambda/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)      574 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/dat_lambda/lambda_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     3854 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/dat_lambda/lambda_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.587541 cloud2-0.1.8/src/aws_services/dynamodb/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/aws_services/dynamodb/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1311 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/aws_services/dynamodb/dynamodb_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     6770 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/aws_services/dynamodb/dynamodb_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.588003 cloud2-0.1.8/src/aws_services/emr/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/aws_services/emr/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1537 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/emr/emr_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10580 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/emr/emr_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.588430 cloud2-0.1.8/src/aws_services/fargate/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/aws_services/fargate/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1459 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/fargate/fargate_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10989 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/fargate/fargate_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.588907 cloud2-0.1.8/src/aws_services/glue/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/aws_services/glue/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2141 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/glue/glue_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    15754 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/glue/glue_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.589340 cloud2-0.1.8/src/aws_services/kinesis_firehose/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/aws_services/kinesis_firehose/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)      964 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/kinesis_firehose/firehose_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     5882 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/kinesis_firehose/kinesis_firehose_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.589788 cloud2-0.1.8/src/aws_services/kinesis_stream/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/kinesis_stream/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1085 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/kinesis_stream/kinesis_stream_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     5542 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/kinesis_stream/kinesis_stream_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.590304 cloud2-0.1.8/src/aws_services/rds/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/aws_services/rds/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2663 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/rds/rds_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    13762 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/rds/rds_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.590719 cloud2-0.1.8/src/aws_services/redshift/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/redshift/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2922 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/redshift/redshift_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    13529 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/aws_services/redshift/redshift_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.591145 cloud2-0.1.8/src/aws_services/s3/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/s3/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2146 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/s3/s3_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    11711 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/s3/s3_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.591590 cloud2-0.1.8/src/aws_services/ses/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/aws_services/ses/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1808 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/aws_services/ses/ses_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10018 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/aws_services/ses/ses_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.592016 cloud2-0.1.8/src/aws_services/sns/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/aws_services/sns/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1907 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/aws_services/sns/sns_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    11294 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/aws_services/sns/sns_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.592437 cloud2-0.1.8/src/aws_services/sqs/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/sqs/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2360 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/aws_services/sqs/sqs_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10990 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/aws_services/sqs/sqs_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.593375 cloud2-0.1.8/src/cloud2.egg-info/
+-rw-r--r--   0 ab         (501) staff       (20)     2226 2023-05-25 15:34:59.000000 cloud2-0.1.8/src/cloud2.egg-info/PKG-INFO
+-rw-r--r--   0 ab         (501) staff       (20)     2326 2023-05-25 15:34:59.000000 cloud2-0.1.8/src/cloud2.egg-info/SOURCES.txt
+-rw-r--r--   0 ab         (501) staff       (20)        1 2023-05-25 15:34:59.000000 cloud2-0.1.8/src/cloud2.egg-info/dependency_links.txt
+-rw-r--r--   0 ab         (501) staff       (20)       74 2023-05-25 15:34:59.000000 cloud2-0.1.8/src/cloud2.egg-info/entry_points.txt
+-rw-r--r--   0 ab         (501) staff       (20)      114 2023-05-25 15:34:59.000000 cloud2-0.1.8/src/cloud2.egg-info/requires.txt
+-rw-r--r--   0 ab         (501) staff       (20)       25 2023-05-25 15:34:59.000000 cloud2-0.1.8/src/cloud2.egg-info/top_level.txt
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.593524 cloud2-0.1.8/src/common/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/common/__init__.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.593770 cloud2-0.1.8/src/common/constants/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/common/constants/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2428 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/common/constants/application_constants.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.594351 cloud2-0.1.8/src/common/service/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/common/service/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     6395 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/common/service/dat_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 15:34:59.594967 cloud2-0.1.8/src/common/utils/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/common/utils/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)    10345 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/common/utils/helper.py
+-rw-r--r--   0 ab         (501) staff       (20)      188 2023-05-11 06:33:05.000000 cloud2-0.1.8/src/common/utils/initialize_logger.py
+-rw-r--r--   0 ab         (501) staff       (20)     1624 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/common/utils/instance_initializer.py
+-rw-r--r--   0 ab         (501) staff       (20)     3206 2023-05-23 16:51:20.000000 cloud2-0.1.8/src/main.py
```

### Comparing `cloud2-0.1.7/PKG-INFO` & `cloud2-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cloud2
-Version: 0.1.7
+Version: 0.1.8
 Summary: AWS Cloud Audit Tool
 Home-page: UNKNOWN
-Author: Vishal <vishalrv1904@gmail.com>, Koushik, Sudharshan, Vikneshwar, Bhanuja <bhanuja497@gmail.com>, Ajay
+Author: Vishal vishalrv1904@gmail.com, Koushik, Sudharshan, Vikneshwar, Bhanuja <bhanuja497@gmail.com>, Ajay
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # **CLOUD AUDIT TOOL** #
```

### Comparing `cloud2-0.1.7/setup.py` & `cloud2-0.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import os
 
 with open("README_PIP.md", "r") as fh:
     long_description = fh.read()
 with open("requirements.txt","r") as req:
     required_packages = req.read().splitlines()
 
-__version__ = '0.1.7'
-__author__='Vishal <vishalrv1904@gmail.com>, Koushik, Sudharshan, Vikneshwar, Bhanuja <bhanuja497@gmail.com>, Ajay'
+__version__ = '0.1.8'
+__author__='Vishal vishalrv1904@gmail.com, Koushik, Sudharshan, Vikneshwar, Bhanuja <bhanuja497@gmail.com>, Ajay'
 __maintainer_email__ = 'vishalrv1904@gmail.com'
 
 setuptools.setup(
     name="cloud2",                
     version=__version__,                        
     author=__author__,  
     # maintainer_email=__maintainer_email__,
```

### Comparing `cloud2-0.1.7/src/aws_services/api_gateway/api_gateway_constants.py` & `cloud2-0.1.8/src/aws_services/api_gateway/api_gateway_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/api_gateway/api_gateway_service.py` & `cloud2-0.1.8/src/aws_services/api_gateway/api_gateway_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/dat_lambda/lambda_constants.py` & `cloud2-0.1.8/src/aws_services/dat_lambda/lambda_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/dat_lambda/lambda_service.py` & `cloud2-0.1.8/src/aws_services/dat_lambda/lambda_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/dynamodb/dynamodb_constants.py` & `cloud2-0.1.8/src/aws_services/dynamodb/dynamodb_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/dynamodb/dynamodb_service.py` & `cloud2-0.1.8/src/aws_services/dynamodb/dynamodb_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/emr/emr_constants.py` & `cloud2-0.1.8/src/aws_services/emr/emr_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/emr/emr_service.py` & `cloud2-0.1.8/src/aws_services/emr/emr_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/fargate/fargate_constants.py` & `cloud2-0.1.8/src/aws_services/fargate/fargate_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/fargate/fargate_service.py` & `cloud2-0.1.8/src/aws_services/fargate/fargate_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/glue/glue_constants.py` & `cloud2-0.1.8/src/aws_services/glue/glue_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/glue/glue_service.py` & `cloud2-0.1.8/src/aws_services/glue/glue_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/kinesis_firehose/firehose_constants.py` & `cloud2-0.1.8/src/aws_services/kinesis_firehose/firehose_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/kinesis_firehose/kinesis_firehose_service.py` & `cloud2-0.1.8/src/aws_services/kinesis_firehose/kinesis_firehose_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/kinesis_stream/kinesis_stream_constants.py` & `cloud2-0.1.8/src/aws_services/kinesis_stream/kinesis_stream_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/kinesis_stream/kinesis_stream_service.py` & `cloud2-0.1.8/src/aws_services/kinesis_stream/kinesis_stream_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/rds/rds_constants.py` & `cloud2-0.1.8/src/aws_services/rds/rds_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/rds/rds_service.py` & `cloud2-0.1.8/src/aws_services/rds/rds_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/redshift/redshift_constants.py` & `cloud2-0.1.8/src/aws_services/redshift/redshift_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/redshift/redshift_service.py` & `cloud2-0.1.8/src/aws_services/redshift/redshift_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/s3/s3_constants.py` & `cloud2-0.1.8/src/aws_services/s3/s3_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/s3/s3_service.py` & `cloud2-0.1.8/src/aws_services/s3/s3_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/ses/ses_constants.py` & `cloud2-0.1.8/src/aws_services/ses/ses_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/ses/ses_service.py` & `cloud2-0.1.8/src/aws_services/ses/ses_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/sns/sns_constants.py` & `cloud2-0.1.8/src/aws_services/sns/sns_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/sns/sns_service.py` & `cloud2-0.1.8/src/aws_services/sns/sns_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/sqs/sqs_constants.py` & `cloud2-0.1.8/src/aws_services/sqs/sqs_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/aws_services/sqs/sqs_service.py` & `cloud2-0.1.8/src/aws_services/sqs/sqs_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/cloud2.egg-info/PKG-INFO` & `cloud2-0.1.8/src/cloud2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cloud2
-Version: 0.1.7
+Version: 0.1.8
 Summary: AWS Cloud Audit Tool
 Home-page: UNKNOWN
-Author: Vishal <vishalrv1904@gmail.com>, Koushik, Sudharshan, Vikneshwar, Bhanuja <bhanuja497@gmail.com>, Ajay
+Author: Vishal vishalrv1904@gmail.com, Koushik, Sudharshan, Vikneshwar, Bhanuja <bhanuja497@gmail.com>, Ajay
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # **CLOUD AUDIT TOOL** #
```

### Comparing `cloud2-0.1.7/src/cloud2.egg-info/SOURCES.txt` & `cloud2-0.1.8/src/cloud2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/common/constants/application_constants.py` & `cloud2-0.1.8/src/common/constants/application_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/common/service/dat_service.py` & `cloud2-0.1.8/src/common/service/dat_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/common/utils/helper.py` & `cloud2-0.1.8/src/common/utils/helper.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/common/utils/instance_initializer.py` & `cloud2-0.1.8/src/common/utils/instance_initializer.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.1.7/src/main.py` & `cloud2-0.1.8/src/main.py`

 * *Files identical despite different names*

