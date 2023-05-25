# Comparing `tmp/cloud2-0.0.4.tar.gz` & `tmp/cloud2-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud2-0.0.4.tar", last modified: Thu May 25 12:21:52 2023, max compression
+gzip compressed data, was "cloud2-0.0.5.tar", last modified: Thu May 25 12:24:03 2023, max compression
```

## Comparing `cloud2-0.0.4.tar` & `cloud2-0.0.5.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.183840 cloud2-0.0.4/
--rw-r--r--   0 ab         (501) staff       (20)       17 2023-05-23 16:51:20.000000 cloud2-0.0.4/MANIFEST.in
--rw-r--r--   0 ab         (501) staff       (20)     2221 2023-05-25 12:21:52.183952 cloud2-0.0.4/PKG-INFO
--rw-r--r--   0 ab         (501) staff       (20)      176 2023-05-25 12:21:52.184294 cloud2-0.0.4/setup.cfg
--rw-r--r--   0 ab         (501) staff       (20)     1129 2023-05-25 12:21:19.000000 cloud2-0.0.4/setup.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.168568 cloud2-0.0.4/src/
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.169108 cloud2-0.0.4/src/aws_services/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/aws_services/__init__.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.170137 cloud2-0.0.4/src/aws_services/api_gateway/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/aws_services/api_gateway/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1267 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/api_gateway/api_gateway_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     7883 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/api_gateway/api_gateway_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.171294 cloud2-0.0.4/src/aws_services/dat_lambda/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/dat_lambda/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)      574 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/dat_lambda/lambda_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     3854 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/dat_lambda/lambda_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.172348 cloud2-0.0.4/src/aws_services/dynamodb/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/aws_services/dynamodb/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1311 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/aws_services/dynamodb/dynamodb_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     6770 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/aws_services/dynamodb/dynamodb_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.173222 cloud2-0.0.4/src/aws_services/emr/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/aws_services/emr/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1537 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/emr/emr_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10580 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/emr/emr_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.173930 cloud2-0.0.4/src/aws_services/fargate/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/aws_services/fargate/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1459 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/fargate/fargate_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10989 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/fargate/fargate_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.174839 cloud2-0.0.4/src/aws_services/glue/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/aws_services/glue/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2141 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/glue/glue_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    15754 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/glue/glue_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.175580 cloud2-0.0.4/src/aws_services/kinesis_firehose/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/aws_services/kinesis_firehose/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)      964 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/kinesis_firehose/firehose_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     5882 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/kinesis_firehose/kinesis_firehose_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.176298 cloud2-0.0.4/src/aws_services/kinesis_stream/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/kinesis_stream/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1085 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/kinesis_stream/kinesis_stream_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     5542 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/kinesis_stream/kinesis_stream_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.176986 cloud2-0.0.4/src/aws_services/rds/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/aws_services/rds/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2663 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/rds/rds_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    13762 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/rds/rds_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.177812 cloud2-0.0.4/src/aws_services/redshift/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/redshift/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2922 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/redshift/redshift_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    13529 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/aws_services/redshift/redshift_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.178528 cloud2-0.0.4/src/aws_services/s3/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/s3/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2146 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/s3/s3_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    11711 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/s3/s3_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.179097 cloud2-0.0.4/src/aws_services/ses/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/aws_services/ses/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1808 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/aws_services/ses/ses_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10018 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/aws_services/ses/ses_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.179893 cloud2-0.0.4/src/aws_services/sns/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/aws_services/sns/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1907 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/aws_services/sns/sns_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    11294 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/aws_services/sns/sns_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.180549 cloud2-0.0.4/src/aws_services/sqs/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/sqs/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2360 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/aws_services/sqs/sqs_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10990 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/aws_services/sqs/sqs_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.181644 cloud2-0.0.4/src/cloud2.egg-info/
--rw-r--r--   0 ab         (501) staff       (20)     2221 2023-05-25 12:21:52.000000 cloud2-0.0.4/src/cloud2.egg-info/PKG-INFO
--rw-r--r--   0 ab         (501) staff       (20)     2326 2023-05-25 12:21:52.000000 cloud2-0.0.4/src/cloud2.egg-info/SOURCES.txt
--rw-r--r--   0 ab         (501) staff       (20)        1 2023-05-25 12:21:52.000000 cloud2-0.0.4/src/cloud2.egg-info/dependency_links.txt
--rw-r--r--   0 ab         (501) staff       (20)       74 2023-05-25 12:21:52.000000 cloud2-0.0.4/src/cloud2.egg-info/entry_points.txt
--rw-r--r--   0 ab         (501) staff       (20)      114 2023-05-25 12:21:52.000000 cloud2-0.0.4/src/cloud2.egg-info/requires.txt
--rw-r--r--   0 ab         (501) staff       (20)       25 2023-05-25 12:21:52.000000 cloud2-0.0.4/src/cloud2.egg-info/top_level.txt
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.181791 cloud2-0.0.4/src/common/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/common/__init__.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.182072 cloud2-0.0.4/src/common/constants/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/common/constants/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2428 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/common/constants/application_constants.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.182628 cloud2-0.0.4/src/common/service/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/common/service/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     6395 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/common/service/dat_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:21:52.183597 cloud2-0.0.4/src/common/utils/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/common/utils/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)    10345 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/common/utils/helper.py
--rw-r--r--   0 ab         (501) staff       (20)      188 2023-05-11 06:33:05.000000 cloud2-0.0.4/src/common/utils/initialize_logger.py
--rw-r--r--   0 ab         (501) staff       (20)     1624 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/common/utils/instance_initializer.py
--rw-r--r--   0 ab         (501) staff       (20)     3206 2023-05-23 16:51:20.000000 cloud2-0.0.4/src/main.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.574879 cloud2-0.0.5/
+-rw-r--r--   0 ab         (501) staff       (20)       17 2023-05-23 16:51:20.000000 cloud2-0.0.5/MANIFEST.in
+-rw-r--r--   0 ab         (501) staff       (20)     2240 2023-05-25 12:24:03.575000 cloud2-0.0.5/PKG-INFO
+-rw-r--r--   0 ab         (501) staff       (20)      176 2023-05-25 12:24:03.575375 cloud2-0.0.5/setup.cfg
+-rw-r--r--   0 ab         (501) staff       (20)     1140 2023-05-25 12:23:42.000000 cloud2-0.0.5/setup.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.560108 cloud2-0.0.5/src/
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.560497 cloud2-0.0.5/src/aws_services/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/aws_services/__init__.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.561317 cloud2-0.0.5/src/aws_services/api_gateway/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/aws_services/api_gateway/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1267 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/api_gateway/api_gateway_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     7883 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/api_gateway/api_gateway_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.562428 cloud2-0.0.5/src/aws_services/dat_lambda/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/dat_lambda/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)      574 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/dat_lambda/lambda_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     3854 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/dat_lambda/lambda_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.563514 cloud2-0.0.5/src/aws_services/dynamodb/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/aws_services/dynamodb/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1311 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/aws_services/dynamodb/dynamodb_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     6770 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/aws_services/dynamodb/dynamodb_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.564398 cloud2-0.0.5/src/aws_services/emr/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/aws_services/emr/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1537 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/emr/emr_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10580 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/emr/emr_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.565152 cloud2-0.0.5/src/aws_services/fargate/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/aws_services/fargate/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1459 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/fargate/fargate_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10989 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/fargate/fargate_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.565819 cloud2-0.0.5/src/aws_services/glue/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/aws_services/glue/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2141 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/glue/glue_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    15754 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/glue/glue_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.566483 cloud2-0.0.5/src/aws_services/kinesis_firehose/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/aws_services/kinesis_firehose/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)      964 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/kinesis_firehose/firehose_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     5882 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/kinesis_firehose/kinesis_firehose_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.567034 cloud2-0.0.5/src/aws_services/kinesis_stream/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/kinesis_stream/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1085 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/kinesis_stream/kinesis_stream_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     5542 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/kinesis_stream/kinesis_stream_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.567720 cloud2-0.0.5/src/aws_services/rds/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/aws_services/rds/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2663 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/rds/rds_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    13762 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/rds/rds_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.568480 cloud2-0.0.5/src/aws_services/redshift/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/redshift/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2922 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/redshift/redshift_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    13529 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/aws_services/redshift/redshift_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.569208 cloud2-0.0.5/src/aws_services/s3/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/s3/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2146 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/s3/s3_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    11711 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/s3/s3_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.569917 cloud2-0.0.5/src/aws_services/ses/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/aws_services/ses/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1808 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/aws_services/ses/ses_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10018 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/aws_services/ses/ses_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.570702 cloud2-0.0.5/src/aws_services/sns/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/aws_services/sns/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1907 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/aws_services/sns/sns_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    11294 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/aws_services/sns/sns_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.571342 cloud2-0.0.5/src/aws_services/sqs/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/sqs/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2360 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/aws_services/sqs/sqs_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10990 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/aws_services/sqs/sqs_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.572584 cloud2-0.0.5/src/cloud2.egg-info/
+-rw-r--r--   0 ab         (501) staff       (20)     2240 2023-05-25 12:24:03.000000 cloud2-0.0.5/src/cloud2.egg-info/PKG-INFO
+-rw-r--r--   0 ab         (501) staff       (20)     2326 2023-05-25 12:24:03.000000 cloud2-0.0.5/src/cloud2.egg-info/SOURCES.txt
+-rw-r--r--   0 ab         (501) staff       (20)        1 2023-05-25 12:24:03.000000 cloud2-0.0.5/src/cloud2.egg-info/dependency_links.txt
+-rw-r--r--   0 ab         (501) staff       (20)       74 2023-05-25 12:24:03.000000 cloud2-0.0.5/src/cloud2.egg-info/entry_points.txt
+-rw-r--r--   0 ab         (501) staff       (20)      114 2023-05-25 12:24:03.000000 cloud2-0.0.5/src/cloud2.egg-info/requires.txt
+-rw-r--r--   0 ab         (501) staff       (20)       25 2023-05-25 12:24:03.000000 cloud2-0.0.5/src/cloud2.egg-info/top_level.txt
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.572744 cloud2-0.0.5/src/common/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/common/__init__.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.572990 cloud2-0.0.5/src/common/constants/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/common/constants/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2428 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/common/constants/application_constants.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.573505 cloud2-0.0.5/src/common/service/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/common/service/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     6395 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/common/service/dat_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 12:24:03.574518 cloud2-0.0.5/src/common/utils/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/common/utils/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)    10345 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/common/utils/helper.py
+-rw-r--r--   0 ab         (501) staff       (20)      188 2023-05-11 06:33:05.000000 cloud2-0.0.5/src/common/utils/initialize_logger.py
+-rw-r--r--   0 ab         (501) staff       (20)     1624 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/common/utils/instance_initializer.py
+-rw-r--r--   0 ab         (501) staff       (20)     3206 2023-05-23 16:51:20.000000 cloud2-0.0.5/src/main.py
```

### Comparing `cloud2-0.0.4/PKG-INFO` & `cloud2-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cloud2
-Version: 0.0.4
+Version: 0.0.5
 Summary: AWS Cloud Audit Tool
 Home-page: UNKNOWN
 Author: Vishal, Koushik, Sudharshan, Vikneshwar, Bhanuja, Ajay
-Maintainer-email: vishalrv1904@gmail.com
+Author-email: vishalrv1904@gmail.com , bhanuja497@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # **CLOUD AUDIT TOOL** #
```

### Comparing `cloud2-0.0.4/setup.py` & `cloud2-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 import os
 
 with open("README_PIP.md", "r") as fh:
     long_description = fh.read()
 with open("requirements.txt","r") as req:
     required_packages = req.read().splitlines()
 
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 __author__='Vishal, Koushik, Sudharshan, Vikneshwar, Bhanuja, Ajay'
-__maintainer_email__ = 'vishalrv1904@gmail.com'
+__author_email__ = 'vishalrv1904@gmail.com , bhanuja497@gmail.com'
 
 setuptools.setup(
     name="cloud2",                
     version=__version__,                        
     author=__author__,  
-    maintainer_email=__maintainer_email__,
+    author_email=__author_email__,
     license= 'MIT',              
     description="AWS Cloud Audit Tool",
     long_description=long_description,     
     long_description_content_type="text/markdown",
     packages=find_packages('src'),
     package_dir={'': 'src'},
     package_data={
```

### Comparing `cloud2-0.0.4/src/aws_services/api_gateway/api_gateway_constants.py` & `cloud2-0.0.5/src/aws_services/api_gateway/api_gateway_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/api_gateway/api_gateway_service.py` & `cloud2-0.0.5/src/aws_services/api_gateway/api_gateway_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/dat_lambda/lambda_constants.py` & `cloud2-0.0.5/src/aws_services/dat_lambda/lambda_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/dat_lambda/lambda_service.py` & `cloud2-0.0.5/src/aws_services/dat_lambda/lambda_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/dynamodb/dynamodb_constants.py` & `cloud2-0.0.5/src/aws_services/dynamodb/dynamodb_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/dynamodb/dynamodb_service.py` & `cloud2-0.0.5/src/aws_services/dynamodb/dynamodb_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/emr/emr_constants.py` & `cloud2-0.0.5/src/aws_services/emr/emr_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/emr/emr_service.py` & `cloud2-0.0.5/src/aws_services/emr/emr_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/fargate/fargate_constants.py` & `cloud2-0.0.5/src/aws_services/fargate/fargate_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/fargate/fargate_service.py` & `cloud2-0.0.5/src/aws_services/fargate/fargate_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/glue/glue_constants.py` & `cloud2-0.0.5/src/aws_services/glue/glue_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/glue/glue_service.py` & `cloud2-0.0.5/src/aws_services/glue/glue_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/kinesis_firehose/firehose_constants.py` & `cloud2-0.0.5/src/aws_services/kinesis_firehose/firehose_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/kinesis_firehose/kinesis_firehose_service.py` & `cloud2-0.0.5/src/aws_services/kinesis_firehose/kinesis_firehose_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/kinesis_stream/kinesis_stream_constants.py` & `cloud2-0.0.5/src/aws_services/kinesis_stream/kinesis_stream_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/kinesis_stream/kinesis_stream_service.py` & `cloud2-0.0.5/src/aws_services/kinesis_stream/kinesis_stream_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/rds/rds_constants.py` & `cloud2-0.0.5/src/aws_services/rds/rds_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/rds/rds_service.py` & `cloud2-0.0.5/src/aws_services/rds/rds_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/redshift/redshift_constants.py` & `cloud2-0.0.5/src/aws_services/redshift/redshift_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/redshift/redshift_service.py` & `cloud2-0.0.5/src/aws_services/redshift/redshift_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/s3/s3_constants.py` & `cloud2-0.0.5/src/aws_services/s3/s3_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/s3/s3_service.py` & `cloud2-0.0.5/src/aws_services/s3/s3_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/ses/ses_constants.py` & `cloud2-0.0.5/src/aws_services/ses/ses_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/ses/ses_service.py` & `cloud2-0.0.5/src/aws_services/ses/ses_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/sns/sns_constants.py` & `cloud2-0.0.5/src/aws_services/sns/sns_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/sns/sns_service.py` & `cloud2-0.0.5/src/aws_services/sns/sns_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/sqs/sqs_constants.py` & `cloud2-0.0.5/src/aws_services/sqs/sqs_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/aws_services/sqs/sqs_service.py` & `cloud2-0.0.5/src/aws_services/sqs/sqs_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/cloud2.egg-info/PKG-INFO` & `cloud2-0.0.5/src/cloud2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cloud2
-Version: 0.0.4
+Version: 0.0.5
 Summary: AWS Cloud Audit Tool
 Home-page: UNKNOWN
 Author: Vishal, Koushik, Sudharshan, Vikneshwar, Bhanuja, Ajay
-Maintainer-email: vishalrv1904@gmail.com
+Author-email: vishalrv1904@gmail.com , bhanuja497@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # **CLOUD AUDIT TOOL** #
```

### Comparing `cloud2-0.0.4/src/cloud2.egg-info/SOURCES.txt` & `cloud2-0.0.5/src/cloud2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/common/constants/application_constants.py` & `cloud2-0.0.5/src/common/constants/application_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/common/service/dat_service.py` & `cloud2-0.0.5/src/common/service/dat_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/common/utils/helper.py` & `cloud2-0.0.5/src/common/utils/helper.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/common/utils/instance_initializer.py` & `cloud2-0.0.5/src/common/utils/instance_initializer.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.0.4/src/main.py` & `cloud2-0.0.5/src/main.py`

 * *Files identical despite different names*

