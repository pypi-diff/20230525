# Comparing `tmp/cloud2-0.2.0.tar.gz` & `tmp/cloud2-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud2-0.2.0.tar", last modified: Thu May 25 16:11:33 2023, max compression
+gzip compressed data, was "cloud2-0.2.1.tar", last modified: Thu May 25 16:14:21 2023, max compression
```

## Comparing `cloud2-0.2.0.tar` & `cloud2-0.2.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.145727 cloud2-0.2.0/
--rw-r--r--   0 ab         (501) staff       (20)       17 2023-05-23 16:51:20.000000 cloud2-0.2.0/MANIFEST.in
--rw-r--r--   0 ab         (501) staff       (20)     2221 2023-05-25 16:11:33.145844 cloud2-0.2.0/PKG-INFO
--rw-r--r--   0 ab         (501) staff       (20)      176 2023-05-25 16:11:33.146167 cloud2-0.2.0/setup.cfg
--rw-r--r--   0 ab         (501) staff       (20)     1103 2023-05-25 16:11:28.000000 cloud2-0.2.0/setup.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.131010 cloud2-0.2.0/src/
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.131480 cloud2-0.2.0/src/aws_services/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/aws_services/__init__.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.132252 cloud2-0.2.0/src/aws_services/api_gateway/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/aws_services/api_gateway/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1267 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/api_gateway/api_gateway_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     7883 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/api_gateway/api_gateway_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.133271 cloud2-0.2.0/src/aws_services/dat_lambda/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/dat_lambda/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)      574 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/dat_lambda/lambda_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     3854 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/dat_lambda/lambda_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.134138 cloud2-0.2.0/src/aws_services/dynamodb/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/aws_services/dynamodb/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1311 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/aws_services/dynamodb/dynamodb_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     6770 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/aws_services/dynamodb/dynamodb_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.134928 cloud2-0.2.0/src/aws_services/emr/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/aws_services/emr/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1537 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/emr/emr_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10580 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/emr/emr_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.135572 cloud2-0.2.0/src/aws_services/fargate/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/aws_services/fargate/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1459 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/fargate/fargate_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10989 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/fargate/fargate_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.136189 cloud2-0.2.0/src/aws_services/glue/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/aws_services/glue/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2141 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/glue/glue_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    15754 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/glue/glue_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.136965 cloud2-0.2.0/src/aws_services/kinesis_firehose/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/aws_services/kinesis_firehose/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)      964 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/kinesis_firehose/firehose_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     5882 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/kinesis_firehose/kinesis_firehose_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.138497 cloud2-0.2.0/src/aws_services/kinesis_stream/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/kinesis_stream/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1085 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/kinesis_stream/kinesis_stream_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     5542 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/kinesis_stream/kinesis_stream_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.139066 cloud2-0.2.0/src/aws_services/rds/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/aws_services/rds/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2663 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/rds/rds_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    13762 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/rds/rds_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.139716 cloud2-0.2.0/src/aws_services/redshift/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/redshift/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2922 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/redshift/redshift_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    13529 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/aws_services/redshift/redshift_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.140458 cloud2-0.2.0/src/aws_services/s3/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/s3/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2146 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/s3/s3_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    11711 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/s3/s3_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.141064 cloud2-0.2.0/src/aws_services/ses/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/aws_services/ses/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1808 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/aws_services/ses/ses_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10018 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/aws_services/ses/ses_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.141671 cloud2-0.2.0/src/aws_services/sns/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/aws_services/sns/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1907 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/aws_services/sns/sns_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    11294 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/aws_services/sns/sns_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.142600 cloud2-0.2.0/src/aws_services/sqs/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/sqs/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2360 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/aws_services/sqs/sqs_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10990 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/aws_services/sqs/sqs_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.143722 cloud2-0.2.0/src/cloud2.egg-info/
--rw-r--r--   0 ab         (501) staff       (20)     2221 2023-05-25 16:11:33.000000 cloud2-0.2.0/src/cloud2.egg-info/PKG-INFO
--rw-r--r--   0 ab         (501) staff       (20)     2326 2023-05-25 16:11:33.000000 cloud2-0.2.0/src/cloud2.egg-info/SOURCES.txt
--rw-r--r--   0 ab         (501) staff       (20)        1 2023-05-25 16:11:33.000000 cloud2-0.2.0/src/cloud2.egg-info/dependency_links.txt
--rw-r--r--   0 ab         (501) staff       (20)       74 2023-05-25 16:11:33.000000 cloud2-0.2.0/src/cloud2.egg-info/entry_points.txt
--rw-r--r--   0 ab         (501) staff       (20)      114 2023-05-25 16:11:33.000000 cloud2-0.2.0/src/cloud2.egg-info/requires.txt
--rw-r--r--   0 ab         (501) staff       (20)       25 2023-05-25 16:11:33.000000 cloud2-0.2.0/src/cloud2.egg-info/top_level.txt
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.143867 cloud2-0.2.0/src/common/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/common/__init__.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.144121 cloud2-0.2.0/src/common/constants/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/common/constants/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2428 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/common/constants/application_constants.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.144625 cloud2-0.2.0/src/common/service/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/common/service/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     6395 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/common/service/dat_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:11:33.145481 cloud2-0.2.0/src/common/utils/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/common/utils/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)    10345 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/common/utils/helper.py
--rw-r--r--   0 ab         (501) staff       (20)      188 2023-05-11 06:33:05.000000 cloud2-0.2.0/src/common/utils/initialize_logger.py
--rw-r--r--   0 ab         (501) staff       (20)     1624 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/common/utils/instance_initializer.py
--rw-r--r--   0 ab         (501) staff       (20)     3206 2023-05-23 16:51:20.000000 cloud2-0.2.0/src/main.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.302962 cloud2-0.2.1/
+-rw-r--r--   0 ab         (501) staff       (20)       17 2023-05-23 16:51:20.000000 cloud2-0.2.1/MANIFEST.in
+-rw-r--r--   0 ab         (501) staff       (20)     2228 2023-05-25 16:14:21.303060 cloud2-0.2.1/PKG-INFO
+-rw-r--r--   0 ab         (501) staff       (20)      176 2023-05-25 16:14:21.303329 cloud2-0.2.1/setup.cfg
+-rw-r--r--   0 ab         (501) staff       (20)     1110 2023-05-25 16:14:06.000000 cloud2-0.2.1/setup.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.288177 cloud2-0.2.1/src/
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.288629 cloud2-0.2.1/src/aws_services/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/aws_services/__init__.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.289318 cloud2-0.2.1/src/aws_services/api_gateway/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/aws_services/api_gateway/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1267 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/api_gateway/api_gateway_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     7883 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/api_gateway/api_gateway_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.290527 cloud2-0.2.1/src/aws_services/dat_lambda/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/dat_lambda/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)      574 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/dat_lambda/lambda_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     3854 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/dat_lambda/lambda_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.291578 cloud2-0.2.1/src/aws_services/dynamodb/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/aws_services/dynamodb/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1311 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/aws_services/dynamodb/dynamodb_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     6770 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/aws_services/dynamodb/dynamodb_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.292497 cloud2-0.2.1/src/aws_services/emr/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/aws_services/emr/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1537 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/emr/emr_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10580 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/emr/emr_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.293256 cloud2-0.2.1/src/aws_services/fargate/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/aws_services/fargate/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1459 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/fargate/fargate_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10989 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/fargate/fargate_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.293949 cloud2-0.2.1/src/aws_services/glue/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/aws_services/glue/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2141 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/glue/glue_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    15754 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/glue/glue_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.294611 cloud2-0.2.1/src/aws_services/kinesis_firehose/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/aws_services/kinesis_firehose/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)      964 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/kinesis_firehose/firehose_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     5882 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/kinesis_firehose/kinesis_firehose_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.295262 cloud2-0.2.1/src/aws_services/kinesis_stream/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/kinesis_stream/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1085 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/kinesis_stream/kinesis_stream_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     5542 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/kinesis_stream/kinesis_stream_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.295825 cloud2-0.2.1/src/aws_services/rds/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/aws_services/rds/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2663 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/rds/rds_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    13762 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/rds/rds_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.296441 cloud2-0.2.1/src/aws_services/redshift/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/redshift/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2922 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/redshift/redshift_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    13529 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/aws_services/redshift/redshift_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.297137 cloud2-0.2.1/src/aws_services/s3/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/s3/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2146 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/s3/s3_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    11711 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/s3/s3_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.298050 cloud2-0.2.1/src/aws_services/ses/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/aws_services/ses/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1808 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/aws_services/ses/ses_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10018 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/aws_services/ses/ses_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.298761 cloud2-0.2.1/src/aws_services/sns/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/aws_services/sns/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1907 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/aws_services/sns/sns_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    11294 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/aws_services/sns/sns_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.299477 cloud2-0.2.1/src/aws_services/sqs/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/sqs/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2360 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/aws_services/sqs/sqs_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10990 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/aws_services/sqs/sqs_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.300742 cloud2-0.2.1/src/cloud2.egg-info/
+-rw-r--r--   0 ab         (501) staff       (20)     2228 2023-05-25 16:14:21.000000 cloud2-0.2.1/src/cloud2.egg-info/PKG-INFO
+-rw-r--r--   0 ab         (501) staff       (20)     2326 2023-05-25 16:14:21.000000 cloud2-0.2.1/src/cloud2.egg-info/SOURCES.txt
+-rw-r--r--   0 ab         (501) staff       (20)        1 2023-05-25 16:14:21.000000 cloud2-0.2.1/src/cloud2.egg-info/dependency_links.txt
+-rw-r--r--   0 ab         (501) staff       (20)       74 2023-05-25 16:14:21.000000 cloud2-0.2.1/src/cloud2.egg-info/entry_points.txt
+-rw-r--r--   0 ab         (501) staff       (20)      114 2023-05-25 16:14:21.000000 cloud2-0.2.1/src/cloud2.egg-info/requires.txt
+-rw-r--r--   0 ab         (501) staff       (20)       25 2023-05-25 16:14:21.000000 cloud2-0.2.1/src/cloud2.egg-info/top_level.txt
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.300920 cloud2-0.2.1/src/common/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/common/__init__.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.301204 cloud2-0.2.1/src/common/constants/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/common/constants/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2428 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/common/constants/application_constants.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.301690 cloud2-0.2.1/src/common/service/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/common/service/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     6395 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/common/service/dat_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-25 16:14:21.302680 cloud2-0.2.1/src/common/utils/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/common/utils/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)    10345 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/common/utils/helper.py
+-rw-r--r--   0 ab         (501) staff       (20)      188 2023-05-11 06:33:05.000000 cloud2-0.2.1/src/common/utils/initialize_logger.py
+-rw-r--r--   0 ab         (501) staff       (20)     1624 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/common/utils/instance_initializer.py
+-rw-r--r--   0 ab         (501) staff       (20)     3206 2023-05-23 16:51:20.000000 cloud2-0.2.1/src/main.py
```

### Comparing `cloud2-0.2.0/PKG-INFO` & `cloud2-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cloud2
-Version: 0.2.0
+Version: 0.2.1
 Summary: AWS Cloud Audit Tool
 Home-page: UNKNOWN
 Author: Vishal, Koushik, Sudharshan, Vikneshwar, Bhanuja, Ajay
-Author-email: check-new@googlegroups.com
+Author-email: cloud-audit-tool@googlegroups.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # **CLOUD AUDIT TOOL** #
```

### Comparing `cloud2-0.2.0/setup.py` & `cloud2-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import os
 
 with open("README_PIP.md", "r") as fh:
     long_description = fh.read()
 with open("requirements.txt","r") as req:
     required_packages = req.read().splitlines()
 
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 __author__='Vishal, Koushik, Sudharshan, Vikneshwar, Bhanuja, Ajay'
-__author_email__ = 'check-new@googlegroups.com'
+__author_email__ = 'cloud-audit-tool@googlegroups.com'
 
 setuptools.setup(
     name="cloud2",                
     version=__version__,                        
     author=__author__,  
     author_email=__author_email__,
     license= 'MIT',
```

### Comparing `cloud2-0.2.0/src/aws_services/api_gateway/api_gateway_constants.py` & `cloud2-0.2.1/src/aws_services/api_gateway/api_gateway_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/api_gateway/api_gateway_service.py` & `cloud2-0.2.1/src/aws_services/api_gateway/api_gateway_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/dat_lambda/lambda_constants.py` & `cloud2-0.2.1/src/aws_services/dat_lambda/lambda_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/dat_lambda/lambda_service.py` & `cloud2-0.2.1/src/aws_services/dat_lambda/lambda_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/dynamodb/dynamodb_constants.py` & `cloud2-0.2.1/src/aws_services/dynamodb/dynamodb_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/dynamodb/dynamodb_service.py` & `cloud2-0.2.1/src/aws_services/dynamodb/dynamodb_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/emr/emr_constants.py` & `cloud2-0.2.1/src/aws_services/emr/emr_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/emr/emr_service.py` & `cloud2-0.2.1/src/aws_services/emr/emr_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/fargate/fargate_constants.py` & `cloud2-0.2.1/src/aws_services/fargate/fargate_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/fargate/fargate_service.py` & `cloud2-0.2.1/src/aws_services/fargate/fargate_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/glue/glue_constants.py` & `cloud2-0.2.1/src/aws_services/glue/glue_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/glue/glue_service.py` & `cloud2-0.2.1/src/aws_services/glue/glue_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/kinesis_firehose/firehose_constants.py` & `cloud2-0.2.1/src/aws_services/kinesis_firehose/firehose_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/kinesis_firehose/kinesis_firehose_service.py` & `cloud2-0.2.1/src/aws_services/kinesis_firehose/kinesis_firehose_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/kinesis_stream/kinesis_stream_constants.py` & `cloud2-0.2.1/src/aws_services/kinesis_stream/kinesis_stream_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/kinesis_stream/kinesis_stream_service.py` & `cloud2-0.2.1/src/aws_services/kinesis_stream/kinesis_stream_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/rds/rds_constants.py` & `cloud2-0.2.1/src/aws_services/rds/rds_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/rds/rds_service.py` & `cloud2-0.2.1/src/aws_services/rds/rds_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/redshift/redshift_constants.py` & `cloud2-0.2.1/src/aws_services/redshift/redshift_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/redshift/redshift_service.py` & `cloud2-0.2.1/src/aws_services/redshift/redshift_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/s3/s3_constants.py` & `cloud2-0.2.1/src/aws_services/s3/s3_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/s3/s3_service.py` & `cloud2-0.2.1/src/aws_services/s3/s3_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/ses/ses_constants.py` & `cloud2-0.2.1/src/aws_services/ses/ses_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/ses/ses_service.py` & `cloud2-0.2.1/src/aws_services/ses/ses_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/sns/sns_constants.py` & `cloud2-0.2.1/src/aws_services/sns/sns_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/sns/sns_service.py` & `cloud2-0.2.1/src/aws_services/sns/sns_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/sqs/sqs_constants.py` & `cloud2-0.2.1/src/aws_services/sqs/sqs_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/aws_services/sqs/sqs_service.py` & `cloud2-0.2.1/src/aws_services/sqs/sqs_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/cloud2.egg-info/PKG-INFO` & `cloud2-0.2.1/src/cloud2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cloud2
-Version: 0.2.0
+Version: 0.2.1
 Summary: AWS Cloud Audit Tool
 Home-page: UNKNOWN
 Author: Vishal, Koushik, Sudharshan, Vikneshwar, Bhanuja, Ajay
-Author-email: check-new@googlegroups.com
+Author-email: cloud-audit-tool@googlegroups.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # **CLOUD AUDIT TOOL** #
```

### Comparing `cloud2-0.2.0/src/cloud2.egg-info/SOURCES.txt` & `cloud2-0.2.1/src/cloud2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/common/constants/application_constants.py` & `cloud2-0.2.1/src/common/constants/application_constants.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/common/service/dat_service.py` & `cloud2-0.2.1/src/common/service/dat_service.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/common/utils/helper.py` & `cloud2-0.2.1/src/common/utils/helper.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/common/utils/instance_initializer.py` & `cloud2-0.2.1/src/common/utils/instance_initializer.py`

 * *Files identical despite different names*

### Comparing `cloud2-0.2.0/src/main.py` & `cloud2-0.2.1/src/main.py`

 * *Files identical despite different names*

