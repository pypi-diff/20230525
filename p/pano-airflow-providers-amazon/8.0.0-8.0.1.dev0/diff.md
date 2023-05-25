# Comparing `tmp/pano-airflow-providers-amazon-8.0.0.tar.gz` & `tmp/pano-airflow-providers-amazon-8.0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pano-airflow-providers-amazon-8.0.0.tar", last modified: Tue May  9 07:43:21 2023, max compression
+gzip compressed data, was "pano-airflow-providers-amazon-8.0.1.dev0.tar", last modified: Thu May 25 03:54:18 2023, max compression
```

## Comparing `pano-airflow-providers-amazon-8.0.0.tar` & `pano-airflow-providers-amazon-8.0.1.dev0.tar`

### file list

```diff
@@ -1,513 +1,512 @@
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.018329 pano-airflow-providers-amazon-8.0.0/
--rw-rw-r--   0 homer     (1000) homer     (1000)    13661 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/LICENSE
--rw-rw-r--   0 homer     (1000) homer     (1000)     1533 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/MANIFEST.in
--rw-rw-r--   0 homer     (1000) homer     (1000)      789 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/NOTICE
--rw-rw-r--   0 homer     (1000) homer     (1000)     1815 2023-05-09 07:43:21.018329 pano-airflow-providers-amazon-8.0.0/PKG-INFO
--rw-rw-r--   0 homer     (1000) homer     (1000)    29013 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/README.md
--rw-rw-r--   0 homer     (1000) homer     (1000)   625592 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/RELEASE_NOTES.rst
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.986329 pano-airflow-providers-amazon-8.0.0/airflow/
--rw-rw-r--   0 homer     (1000) homer     (1000)     2320 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/alembic.ini
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.982329 pano-airflow-providers-amazon-8.0.0/airflow/api_connexion/
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.986329 pano-airflow-providers-amazon-8.0.0/airflow/api_connexion/openapi/
--rw-rw-r--   0 homer     (1000) homer     (1000)   151926 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/api_connexion/openapi/v1.yaml
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.986329 pano-airflow-providers-amazon-8.0.0/airflow/config_templates/
--rw-rw-r--   0 homer     (1000) homer     (1000)      787 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/config_templates/__init__.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    13633 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/config_templates/airflow_local_settings.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    97490 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/config_templates/config.yml
--rw-rw-r--   0 homer     (1000) homer     (1000)     2579 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/config_templates/config.yml.schema.json
--rw-rw-r--   0 homer     (1000) homer     (1000)    60155 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/config_templates/default_airflow.cfg
--rw-rw-r--   0 homer     (1000) homer     (1000)     4345 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/config_templates/default_celery.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     2199 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/config_templates/default_test.cfg
--rw-rw-r--   0 homer     (1000) homer     (1000)     4771 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/config_templates/default_webserver_config.py
--rw-rw-r--   0 homer     (1000) homer     (1000)      735 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/customized_form_field_behaviours.schema.json
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.982329 pano-airflow-providers-amazon-8.0.0/airflow/example_dags/
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.986329 pano-airflow-providers-amazon-8.0.0/airflow/example_dags/sql/
--rw-rw-r--   0 homer     (1000) homer     (1000)      866 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/example_dags/sql/sample.sql
--rw-rw-r--   0 homer     (1000) homer     (1000)       52 2023-05-08 23:47:31.000000 pano-airflow-providers-amazon-8.0.0/airflow/git_version
--rw-rw-r--   0 homer     (1000) homer     (1000)     2760 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/provider_info.schema.json
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.982329 pano-airflow-providers-amazon-8.0.0/airflow/providers/
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.986329 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/
--rw-rw-r--   0 homer     (1000) homer     (1000)     1389 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/__init__.py
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.986329 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/
--rw-rw-r--   0 homer     (1000) homer     (1000)      785 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/__init__.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     1731 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/exceptions.py
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.990329 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/
--rw-rw-r--   0 homer     (1000) homer     (1000)      785 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/__init__.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     4856 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/appflow.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    12240 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/athena.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    45932 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/base_aws.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    20629 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/batch_client.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     9697 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/batch_waiters.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3376 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/cloud_formation.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    14133 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/datasync.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     7906 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/dms.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     2668 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/dynamodb.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     7641 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/ec2.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3702 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/ecr.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     9194 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/ecs.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    23957 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/eks.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    12114 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    20465 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/emr.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3518 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/glacier.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    14759 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/glue.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     7611 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/glue_catalog.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     8895 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/glue_crawler.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     1993 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/kinesis.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     8008 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/lambda_function.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     4823 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/logs.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     7219 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/quicksight.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    15272 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/rds.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    13287 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/redshift_cluster.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     7720 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/redshift_data.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     7072 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/redshift_sql.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    42450 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/s3.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    56676 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/sagemaker.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     2692 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/secrets_manager.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     4143 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/ses.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3461 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/sns.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3119 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/sqs.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     2449 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/ssm.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3072 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/step_function.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     1817 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/sts.py
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.990329 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/links/
--rw-rw-r--   0 homer     (1000) homer     (1000)      785 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/links/__init__.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     2940 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/links/base_aws.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     1767 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/links/batch.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     1416 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/links/emr.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     1228 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/links/glue.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     1607 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/links/logs.py
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.990329 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/log/
--rw-rw-r--   0 homer     (1000) homer     (1000)      785 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/log/__init__.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     5072 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     9775 2023-05-07 05:32:50.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/log/s3_task_handler.py
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.990329 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/
--rw-rw-r--   0 homer     (1000) homer     (1000)      785 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/__init__.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    19677 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/appflow.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     6141 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/athena.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    16588 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/batch.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3633 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/cloud_formation.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    18419 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/datasync.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    10715 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/dms.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     9589 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/ec2.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    29018 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/ecs.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    31753 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/eks.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    50180 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/emr.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3705 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/glacier.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     7471 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/glue.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3306 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/glue_crawler.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     7755 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/lambda_function.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3972 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/quicksight.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    29868 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/rds.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    29124 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/redshift_cluster.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     5559 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/redshift_data.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    29966 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/s3.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    49835 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/sagemaker.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     2959 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/sns.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3563 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/sqs.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     4469 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/step_function.py
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.990329 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/secrets/
--rw-rw-r--   0 homer     (1000) homer     (1000)      785 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/secrets/__init__.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    15533 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/secrets/secrets_manager.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     8503 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/secrets/systems_manager.py
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.990329 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/
--rw-rw-r--   0 homer     (1000) homer     (1000)      785 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/__init__.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3120 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/athena.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     7384 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/batch.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     4163 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/cloud_formation.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3998 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/dms.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3915 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/dynamodb.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     2674 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/ec2.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     7203 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/ecs.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     9786 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/eks.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    18505 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/emr.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     4129 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/glacier.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3332 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/glue.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3732 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     2963 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/glue_crawler.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3064 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/lambda_function.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3641 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/quicksight.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     6447 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/rds.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     2637 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/redshift_cluster.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    11650 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/s3.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    13057 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/sagemaker.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     9584 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/sqs.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3400 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/step_function.py
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.994329 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/
--rw-rw-r--   0 homer     (1000) homer     (1000)      785 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/__init__.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     2768 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/base.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     5843 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     4410 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     6435 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     7676 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     4701 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     9042 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     4172 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     4248 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     4158 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/local_to_s3.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     5863 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     8108 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     2966 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     8268 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3191 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     4620 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/s3_to_sql.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     5679 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3679 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     8475 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/sql_to_s3.py
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.994329 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/triggers/
--rw-rw-r--   0 homer     (1000) homer     (1000)      787 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/triggers/__init__.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     5579 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/triggers/redshift_cluster.py
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.994329 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/utils/
--rw-rw-r--   0 homer     (1000) homer     (1000)     2215 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/utils/__init__.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    20348 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/utils/connection_wrapper.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     2561 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/utils/eks_get_token.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     1853 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/utils/emailer.py
--rw-rw-r--   0 homer     (1000) homer     (1000)      972 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/utils/rds.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     1913 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/utils/redshift.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     1040 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/utils/sagemaker.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     1701 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/utils/tags.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3583 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/utils/waiter.py
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.994329 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/waiters/
--rw-rw-r--   0 homer     (1000) homer     (1000)      785 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/waiters/__init__.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     1853 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/waiters/base_waiter.py
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.994329 pano-airflow-providers-amazon-8.0.0/airflow/serialization/
--rw-rw-r--   0 homer     (1000) homer     (1000)    10401 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/serialization/schema.json
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.994329 pano-airflow-providers-amazon-8.0.0/airflow/utils/
--rw-rw-r--   0 homer     (1000) homer     (1000)     4406 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/utils/context.pyi
--rw-rw-r--   0 homer     (1000) homer     (1000)     1964 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/utils/python_virtualenv_script.jinja2
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.994329 pano-airflow-providers-amazon-8.0.0/airflow/www/
--rw-rw-r--   0 homer     (1000) homer     (1000)       87 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/.eslintignore
--rw-rw-r--   0 homer     (1000) homer     (1000)     1530 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/.eslintrc
--rw-rw-r--   0 homer     (1000) homer     (1000)       51 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/.prettierignore
--rw-rw-r--   0 homer     (1000) homer     (1000)      111 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/.prettierrc
--rw-rw-r--   0 homer     (1000) homer     (1000)       26 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/.stylelintignore
--rw-rw-r--   0 homer     (1000) homer     (1000)       76 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/.stylelintrc
--rw-rw-r--   0 homer     (1000) homer     (1000)      787 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/__init__.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     7834 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/alias-rest-types.js
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.994329 pano-airflow-providers-amazon-8.0.0/airflow/www/api/
--rw-rw-r--   0 homer     (1000) homer     (1000)      787 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/api/__init__.py
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.994329 pano-airflow-providers-amazon-8.0.0/airflow/www/api/experimental/
--rw-rw-r--   0 homer     (1000) homer     (1000)      787 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/api/experimental/__init__.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    14422 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/api/experimental/endpoints.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     6904 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/app.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     2724 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/auth.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     1075 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/babel.config.js
--rw-rw-r--   0 homer     (1000) homer     (1000)     1018 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/blueprints.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     5768 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/decorators.py
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.994329 pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/
--rw-rw-r--   0 homer     (1000) homer     (1000)      785 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/__init__.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    25545 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_appbuilder.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     2142 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_appbuilder_links.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     1819 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_cache.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     1242 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_dagbag.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     3423 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_jinja_globals.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     2137 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_manifest_files.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     1436 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_robots.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     2548 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_security.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     2620 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_session.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    11573 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_views.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     2374 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_wsgi_middlewares.py
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.994329 pano-airflow-providers-amazon-8.0.0/airflow/www/fab_security/
--rw-rw-r--   0 homer     (1000) homer     (1000)      785 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/fab_security/__init__.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    66648 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/fab_security/manager.py
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.998329 pano-airflow-providers-amazon-8.0.0/airflow/www/fab_security/sqla/
--rw-rw-r--   0 homer     (1000) homer     (1000)      785 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/fab_security/sqla/__init__.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    21377 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/fab_security/sqla/manager.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     8364 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/fab_security/sqla/models.py
--rw-rw-r--   0 homer     (1000) homer     (1000)    10112 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/fab_security/views.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     8906 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/forms.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     1359 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/gunicorn_config.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     1821 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/jest-setup.js
--rw-rw-r--   0 homer     (1000) homer     (1000)     1807 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/jest.config.js
--rw-rw-r--   0 homer     (1000) homer     (1000)     4649 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/package.json
--rw-rw-r--   0 homer     (1000) homer     (1000)    33584 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/security.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     1741 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/session.py
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.998329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/
--rw-rw-r--   0 homer     (1000) homer     (1000)   622963 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/airflow.gif
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.998329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/
--rw-rw-r--   0 homer     (1000) homer     (1000)   128047 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/bootstrap-theme.css
--rw-rw-r--   0 homer     (1000) homer     (1000)     1211 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/calendar.css
--rw-rw-r--   0 homer     (1000) homer     (1000)     1524 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/chart.css
--rw-rw-r--   0 homer     (1000) homer     (1000)     3047 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/dags.css
--rw-rw-r--   0 homer     (1000) homer     (1000)     1468 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/flash.css
--rw-rw-r--   0 homer     (1000) homer     (1000)     1325 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/gantt.css
--rw-rw-r--   0 homer     (1000) homer     (1000)     3321 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/graph.css
--rw-rw-r--   0 homer     (1000) homer     (1000)     1385 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/loading-dots.css
--rw-rw-r--   0 homer     (1000) homer     (1000)    10009 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/main.css
--rw-rw-r--   0 homer     (1000) homer     (1000)   112039 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/material-icons.css
--rw-rw-r--   0 homer     (1000) homer     (1000)     2416 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/switch.css
--rw-rw-r--   0 homer     (1000) homer     (1000)      834 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/declarations.d.ts
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.002329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/
--rw-rw-r--   0 homer     (1000) homer     (1000)     2847 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/App.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     2080 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/README.md
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.002329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/
--rw-rw-r--   0 homer     (1000) homer     (1000)     2480 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/index.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     2139 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useClearRun.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     3227 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useClearTask.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     2625 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useClearTaskDryRun.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     1295 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useDataset.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     6050 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useDatasetDependencies.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     2349 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useDatasetEvents.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     2336 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useDatasets.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     2012 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useExtraLinks.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     1933 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useGraphData.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     2061 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useGridData.test.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     3595 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useGridData.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     2007 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useMappedInstances.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     2150 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useMarkFailedRun.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     2887 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useMarkFailedTask.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     2151 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useMarkSuccessRun.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     2892 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useMarkSuccessTask.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     2241 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useMarkTaskDryRun.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     2131 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useQueueRun.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     2239 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useSetDagRunNote.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     4272 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useSetTaskInstanceNote.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     2361 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useTaskInstance.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     2560 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useTaskLog.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     1587 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useUpstreamDatasetEvents.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)    11437 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/calendar.js
--rw-rw-r--   0 homer     (1000) homer     (1000)    11005 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/callModal.js
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.002329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/
--rw-rw-r--   0 homer     (1000) homer     (1000)     1806 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/AutoRefresh.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     1482 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/Clipboard.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     2276 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/Clipboard.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     1504 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/InfoTooltip.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     1306 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/LinkButton.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     1156 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/LinkButton.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     1586 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/MultiSelect.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     3850 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/ReactMarkdown.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     1698 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/RunTypeIcon.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     1433 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/TabWithTooltip.tsx
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.002329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/Table/
--rw-rw-r--   0 homer     (1000) homer     (1000)     2885 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/Table/Cells.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     4564 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/Table/Cells.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     8115 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/Table/Table.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     7943 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/Table/index.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     2797 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/Time.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     1593 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/Time.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     5144 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/Tooltip.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)    11295 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/connection_form.js
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.002329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/context/
--rw-rw-r--   0 homer     (1000) homer     (1000)     3178 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/context/autorefresh.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     1537 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/context/containerRef.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     1900 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/context/timezone.tsx
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.006329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/
--rw-rw-r--   0 homer     (1000) homer     (1000)     4010 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/InstanceTooltip.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     2698 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/InstanceTooltip.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     6274 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/Main.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     4529 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/StatusBox.tsx
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.006329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/
--rw-rw-r--   0 homer     (1000) homer     (1000)     1309 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/BreadcrumbText.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     5128 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/Dag.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     2448 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/FilterTasks.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     4232 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/Header.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     3692 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/NotesAccordion.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     5053 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/NotesAccordion.tsx
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.006329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/dagRun/
--rw-rw-r--   0 homer     (1000) homer     (1000)     2330 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/dagRun/ClearRun.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     2044 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/dagRun/DatasetTriggerEvents.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     2665 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/dagRun/MarkRunAs.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     5846 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/dagRun/index.tsx
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.006329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/graph/
--rw-rw-r--   0 homer     (1000) homer     (1000)     1959 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/graph/Edge.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     3434 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/graph/Node.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     5400 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/graph/Node.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     6083 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/graph/index.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     6429 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/graph/utils.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     8575 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/index.tsx
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.006329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/
--rw-rw-r--   0 homer     (1000) homer     (1000)     1303 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/BackToTaskSummary.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     2206 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/DatasetUpdateEvents.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     6049 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/Details.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     1909 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/ExtraLinks.tsx
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.006329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/Logs/
--rw-rw-r--   0 homer     (1000) homer     (1000)     2509 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/Logs/LogBlock.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     2398 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/Logs/LogLink.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     2143 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/Logs/LogLink.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     7322 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/Logs/index.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     8906 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/Logs/index.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     5361 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/Logs/utils.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     3051 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/Logs/utils.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     3834 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/MappedInstances.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     3742 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/Nav.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     3428 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/index.tsx
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.006329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/taskActions/
--rw-rw-r--   0 homer     (1000) homer     (1000)     1611 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/taskActions/ActionButton.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     3364 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/taskActions/ActionModal.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     6071 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/taskActions/ClearInstance.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     7327 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/taskActions/MarkInstanceAs.tsx
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.010329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/
--rw-rw-r--   0 homer     (1000) homer     (1000)     1835 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/TaskName.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     1849 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/TaskName.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     2504 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/ToggleGroups.tsx
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.010329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/dagRuns/
--rw-rw-r--   0 homer     (1000) homer     (1000)     5371 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/dagRuns/Bar.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     1765 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/dagRuns/Tooltip.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     5545 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/dagRuns/index.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     4512 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/dagRuns/index.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     7478 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/index.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     4792 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/index.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     3904 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/renderTaskRows.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     6030 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/renderTaskRows.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     1664 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/index.tsx
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.010329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/nav/
--rw-rw-r--   0 homer     (1000) homer     (1000)     3849 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/nav/FilterBar.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     2368 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/nav/LegendRow.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     2202 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/nav/LegendRow.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     5120 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/useFilters.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     4991 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/useFilters.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     2489 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/useSelection.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     2277 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/useSelection.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     1425 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/useToggleGroups.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     3795 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag.js
--rw-rw-r--   0 homer     (1000) homer     (1000)     1120 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag_code.js
--rw-rw-r--   0 homer     (1000) homer     (1000)     7219 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag_dependencies.js
--rw-rw-r--   0 homer     (1000) homer     (1000)    17313 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dags.js
--rw-rw-r--   0 homer     (1000) homer     (1000)     2934 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasetUtils.js
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.010329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/
--rw-rw-r--   0 homer     (1000) homer     (1000)     2459 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/DatasetEvents.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     1968 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/Details.tsx
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.010329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/Graph/
--rw-rw-r--   0 homer     (1000) homer     (1000)     2375 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/Graph/DagNode.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     1893 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/Graph/Edge.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     2125 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/Graph/Legend.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     2798 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/Graph/Node.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     4120 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/Graph/index.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     3698 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/List.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     6729 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/List.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     2983 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/index.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     4450 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datetime_utils.js
--rw-rw-r--   0 homer     (1000) homer     (1000)     1161 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/duration_chart.js
--rw-rw-r--   0 homer     (1000) homer     (1000)    11488 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/gantt.js
--rw-rw-r--   0 homer     (1000) homer     (1000)    24373 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/graph.js
--rw-rw-r--   0 homer     (1000) homer     (1000)     1124 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/index.d.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     7829 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/main.js
--rw-rw-r--   0 homer     (1000) homer     (1000)     1817 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/task.js
--rw-rw-r--   0 homer     (1000) homer     (1000)     6696 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/task_instances.js
--rw-rw-r--   0 homer     (1000) homer     (1000)     1123 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/theme.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     6826 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/ti_log.js
--rw-rw-r--   0 homer     (1000) homer     (1000)     7621 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/trigger.js
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.010329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/types/
--rw-rw-r--   0 homer     (1000) homer     (1000)   163643 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/types/api-generated.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     3203 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/types/index.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     4832 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/types/react-table-config.d.ts
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.010329 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/utils/
--rw-rw-r--   0 homer     (1000) homer     (1000)     1193 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/utils/URLSearchParamWrapper.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     5778 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/utils/graph.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     4231 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/utils/index.test.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     4616 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/utils/index.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     2420 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/utils/testUtils.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     2267 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/utils/useErrorToast.test.tsx
--rw-rw-r--   0 homer     (1000) homer     (1000)     1843 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/utils/useErrorToast.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)     1657 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/utils/useOffsetTop.ts
--rw-rw-r--   0 homer     (1000) homer     (1000)      988 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/variable_edit.js
--rw-rw-r--   0 homer     (1000) homer     (1000)    16671 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/loading.gif
--rw-rw-r--   0 homer     (1000) homer     (1000)     3184 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/pin.svg
--rw-rw-r--   0 homer     (1000) homer     (1000)     7501 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/pin_100.png
--rw-rw-r--   0 homer     (1000) homer     (1000)     1547 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/pin_25.png
--rw-rw-r--   0 homer     (1000) homer     (1000)     1201 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/pin_32.png
--rw-rw-r--   0 homer     (1000) homer     (1000)     2306 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/pin_35.png
--rw-rw-r--   0 homer     (1000) homer     (1000)     2685 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/pin_40.png
--rw-rw-r--   0 homer     (1000) homer     (1000)    24922 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/pin_large.png
--rw-rw-r--   0 homer     (1000) homer     (1000)       26 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/robots.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)      160 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/sort_asc.png
--rw-rw-r--   0 homer     (1000) homer     (1000)      201 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/sort_both.png
--rw-rw-r--   0 homer     (1000) homer     (1000)      158 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/static/sort_desc.png
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.982329 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.014329 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/
--rw-rw-r--   0 homer     (1000) homer     (1000)     1147 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/_messages.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     2004 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/calendar.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     2582 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/chart.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1740 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/config.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1593 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/confirm.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1913 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/conn_create.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1924 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/conn_edit.html
--rw-rw-r--   0 homer     (1000) homer     (1000)    26111 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/dag.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     4917 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/dag_audit_log.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1560 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/dag_code.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     2795 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/dag_dependencies.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     4043 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/dag_details.html
--rw-rw-r--   0 homer     (1000) homer     (1000)    23601 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/dags.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     2447 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/dataset_next_run_modal.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1881 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/datasets.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     2901 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/duration_chart.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1327 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/error.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     3187 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/gantt.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     5804 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/graph.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1975 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/grid.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     5117 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/main.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     3177 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/model_list.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1582 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/no_roles_permissions.html
--rw-rw-r--   0 homer     (1000) homer     (1000)      950 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/noaccess.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1495 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/plugin.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1512 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/providers.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1187 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/redoc.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     2502 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/task.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     2433 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/task_instance.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1044 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/ti_code.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     3118 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/ti_log.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     2326 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/traceback.html
--rw-rw-r--   0 homer     (1000) homer     (1000)    12933 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/trigger.html
--rw-rw-r--   0 homer     (1000) homer     (1000)      999 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/variable_edit.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1671 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/variable_list.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1013 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/variable_show.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     2301 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/variable_show_widget.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1231 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/xcom.html
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.014329 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/analytics/
--rw-rw-r--   0 homer     (1000) homer     (1000)     1076 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/analytics/google_analytics.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1807 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/analytics/metarouter.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1810 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/analytics/segment.html
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.014329 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/appbuilder/
--rw-rw-r--   0 homer     (1000) homer     (1000)     4446 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/appbuilder/custom_icons.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1806 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/appbuilder/dag_docs.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     3218 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/appbuilder/flash.html
--rw-rw-r--   0 homer     (1000) homer     (1000)      809 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/appbuilder/index.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1060 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/appbuilder/loading_dots.html
--rw-rw-r--   0 homer     (1000) homer     (1000)    10092 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/appbuilder/navbar.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     1661 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/appbuilder/navbar_menu.html
--rw-rw-r--   0 homer     (1000) homer     (1000)     3486 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/appbuilder/navbar_right.html
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.014329 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/swagger-ui/
--rw-rw-r--   0 homer     (1000) homer     (1000)     2601 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/templates/swagger-ui/index.j2
--rw-rw-r--   0 homer     (1000) homer     (1000)     1431 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/tsconfig.json
--rw-rw-r--   0 homer     (1000) homer     (1000)    31762 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/utils.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     2650 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/validators.py
--rw-rw-r--   0 homer     (1000) homer     (1000)   219115 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/views.py
--rw-rw-r--   0 homer     (1000) homer     (1000)     8881 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/webpack.config.js
--rw-rw-r--   0 homer     (1000) homer     (1000)     2770 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/airflow/www/widgets.py
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.018329 pano-airflow-providers-amazon-8.0.0/licenses/
--rw-rw-r--   0 homer     (1000) homer     (1000)     1131 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-bootstrap.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)      984 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-bootstrap3-typeahead.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)     1475 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-d3-shape.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)     1079 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-d3-tip.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)     1475 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-d3js.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)     1062 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-dagre-d3.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)     1076 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-datatables.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)     1081 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-elasticmock.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)     1096 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-eonasdan-bootstrap-datetimepicker.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)     1301 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-flask-kerberos.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)    11349 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-hue.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)    11357 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-jqclock.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)     1605 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-jquery.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)     1077 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-moment-strftime.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)     1075 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-moment.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)     1096 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-normalize.txt
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.018329 pano-airflow-providers-amazon-8.0.0/pano_airflow_providers_amazon.egg-info/
--rw-rw-r--   0 homer     (1000) homer     (1000)     1815 2023-05-09 07:43:20.000000 pano-airflow-providers-amazon-8.0.0/pano_airflow_providers_amazon.egg-info/PKG-INFO
--rw-rw-r--   0 homer     (1000) homer     (1000)    19855 2023-05-09 07:43:20.000000 pano-airflow-providers-amazon-8.0.0/pano_airflow_providers_amazon.egg-info/SOURCES.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)        1 2023-05-09 07:43:20.000000 pano-airflow-providers-amazon-8.0.0/pano_airflow_providers_amazon.egg-info/dependency_links.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)      103 2023-05-09 07:43:20.000000 pano-airflow-providers-amazon-8.0.0/pano_airflow_providers_amazon.egg-info/entry_points.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)        1 2023-05-09 07:43:20.000000 pano-airflow-providers-amazon-8.0.0/pano_airflow_providers_amazon.egg-info/not-zip-safe
--rw-rw-r--   0 homer     (1000) homer     (1000)      774 2023-05-09 07:43:20.000000 pano-airflow-providers-amazon-8.0.0/pano_airflow_providers_amazon.egg-info/requires.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)        8 2023-05-09 07:43:20.000000 pano-airflow-providers-amazon-8.0.0/pano_airflow_providers_amazon.egg-info/top_level.txt
--rw-rw-r--   0 homer     (1000) homer     (1000)     5246 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/pyproject.toml
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:20.982329 pano-airflow-providers-amazon-8.0.0/scripts/
-drwxrwxr-x   0 homer     (1000) homer     (1000)        0 2023-05-09 07:43:21.018329 pano-airflow-providers-amazon-8.0.0/scripts/systemd/
--rw-rw-r--   0 homer     (1000) homer     (1000)      678 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/scripts/systemd/README
--rw-rw-r--   0 homer     (1000) homer     (1000)      968 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/scripts/systemd/airflow
--rw-rw-r--   0 homer     (1000) homer     (1000)     1195 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/scripts/systemd/airflow-flower.service
--rw-rw-r--   0 homer     (1000) homer     (1000)     1200 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/scripts/systemd/airflow-kerberos.service
--rw-rw-r--   0 homer     (1000) homer     (1000)     1190 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/scripts/systemd/airflow-scheduler.service
--rw-rw-r--   0 homer     (1000) homer     (1000)     1243 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/scripts/systemd/airflow-webserver.service
--rw-rw-r--   0 homer     (1000) homer     (1000)     1203 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/scripts/systemd/airflow-worker.service
--rw-rw-r--   0 homer     (1000) homer     (1000)      824 2023-05-06 23:14:41.000000 pano-airflow-providers-amazon-8.0.0/scripts/systemd/airflow.conf
--rw-rw-r--   0 homer     (1000) homer     (1000)     2068 2023-05-09 07:43:21.018329 pano-airflow-providers-amazon-8.0.0/setup.cfg
--rw-rw-r--   0 homer     (1000) homer     (1000)     2362 2023-05-09 07:41:16.000000 pano-airflow-providers-amazon-8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.350612 pano-airflow-providers-amazon-8.0.1.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    30738 2023-05-25 03:54:18.350612 pano-airflow-providers-amazon-8.0.1.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    29013 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   625592 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/RELEASE_NOTES.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.306611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.302611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/api_connexion/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.306611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/api_connexion/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)   151926 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/api_connexion/openapi/v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.310611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/config_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/config_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13633 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/config_templates/airflow_local_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97490 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/config_templates/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/config_templates/config.yml.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60155 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/config_templates/default_airflow.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/config_templates/default_celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/config_templates/default_test.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/config_templates/default_webserver_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/customized_form_field_behaviours.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.302611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/example_dags/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.310611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/example_dags/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/example_dags/sql/sample.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/provider_info.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.302611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.310611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.310611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.314611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/appflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45932 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/base_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20629 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/batch_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/batch_waiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/cloud_formation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/datasync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/dms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/ecr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23957 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/eks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12114 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20465 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/emr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/glacier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/glue_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/glue_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/quicksight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15272 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/rds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/redshift_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/redshift_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/redshift_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42450 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56676 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/ses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/ssm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/step_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/sts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.314611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/links/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/links/base_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/links/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/links/emr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/links/glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/links/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.314611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/log/s3_task_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.314611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19677 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/appflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16588 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/cloud_formation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18419 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/datasync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/dms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29018 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31753 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/eks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50180 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/emr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/glacier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/glue_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/quicksight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29868 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/rds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29124 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/redshift_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/redshift_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29966 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49835 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/step_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.318611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15533 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/secrets/secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/secrets/systems_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.318611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/cloud_formation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/dms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/eks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/emr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/glacier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/glue_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/quicksight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/rds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/redshift_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13057 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/step_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.318611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/local_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/s3_to_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/sql_to_s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.322611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/triggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/triggers/redshift_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.322611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/utils/connection_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/utils/eks_get_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/utils/emailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/utils/rds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/utils/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/utils/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/utils/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/utils/waiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.322611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/waiters/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/waiters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/waiters/base_waiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.322611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/serialization/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.322611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/utils/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/utils/python_virtualenv_script.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.322611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/.eslintignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/.eslintrc
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/.stylelintignore
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/.stylelintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/alias-rest-types.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.322611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.326612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/api/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/api/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14422 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/api/experimental/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/babel.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.326612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25545 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_appbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_appbuilder_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_dagbag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_jinja_globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_manifest_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_robots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_wsgi_middlewares.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.326612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/fab_security/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/fab_security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66648 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/fab_security/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.326612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/fab_security/sqla/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/fab_security/sqla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/fab_security/sqla/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/fab_security/sqla/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/fab_security/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/gunicorn_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/jest-setup.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/jest.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33584 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.326612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   622963 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/airflow.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.330612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   128047 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/bootstrap-theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/calendar.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/chart.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/dags.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/flash.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/gantt.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/graph.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/loading-dots.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)   112039 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/material-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/switch.css
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/declarations.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.330612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/App.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.334612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useClearRun.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useClearTask.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useClearTaskDryRun.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useDataset.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useDatasetDependencies.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useDatasetEvents.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useDatasets.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useExtraLinks.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useGraphData.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useGridData.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useGridData.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useMappedInstances.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useMarkFailedRun.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useMarkFailedTask.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useMarkSuccessRun.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useMarkSuccessTask.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useMarkTaskDryRun.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useQueueRun.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useSetDagRunNote.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useSetTaskInstanceNote.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useTaskInstance.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useTaskLog.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useUpstreamDatasetEvents.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/calendar.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11005 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/callModal.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.334612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/AutoRefresh.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/Clipboard.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/Clipboard.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/InfoTooltip.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/LinkButton.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/LinkButton.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/MultiSelect.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/ReactMarkdown.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/RunTypeIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/TabWithTooltip.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.334612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/Table/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/Table/Cells.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/Table/Cells.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/Table/Table.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/Table/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/Time.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/Time.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/Tooltip.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)    11295 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/connection_form.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.334612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/context/
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/context/autorefresh.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/context/containerRef.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/context/timezone.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.334612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/InstanceTooltip.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/InstanceTooltip.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/Main.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/StatusBox.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.338612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/BreadcrumbText.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/Dag.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/FilterTasks.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/Header.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/NotesAccordion.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/NotesAccordion.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.338612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/dagRun/
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/dagRun/ClearRun.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/dagRun/DatasetTriggerEvents.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/dagRun/MarkRunAs.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/dagRun/index.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.338612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/graph/Edge.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/graph/Node.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/graph/Node.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/graph/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/graph/utils.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/index.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.338612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/BackToTaskSummary.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/DatasetUpdateEvents.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/Details.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/ExtraLinks.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.338612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/Logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/Logs/LogBlock.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/Logs/LogLink.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/Logs/LogLink.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/Logs/index.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/Logs/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/Logs/utils.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/Logs/utils.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/MappedInstances.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/Nav.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/index.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.338612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/taskActions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/taskActions/ActionButton.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/taskActions/ActionModal.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/taskActions/ClearInstance.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/taskActions/MarkInstanceAs.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.338612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/TaskName.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/TaskName.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/ToggleGroups.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.338612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/dagRuns/
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/dagRuns/Bar.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/dagRuns/Tooltip.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/dagRuns/index.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/dagRuns/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/index.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/renderTaskRows.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/renderTaskRows.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/index.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.342612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/nav/
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/nav/FilterBar.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/nav/LegendRow.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/nav/LegendRow.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/useFilters.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/useFilters.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/useSelection.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/useSelection.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/useToggleGroups.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag_code.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag_dependencies.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dags.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasetUtils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.342612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/DatasetEvents.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/Details.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.342612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/Graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/Graph/DagNode.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/Graph/Edge.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/Graph/Legend.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/Graph/Node.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/Graph/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/List.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/List.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datetime_utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/duration_chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/gantt.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24373 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/graph.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/task.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/task_instances.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/theme.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/ti_log.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/trigger.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.342612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/types/
+-rw-r--r--   0 runner    (1001) docker     (123)   163643 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/types/api-generated.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/types/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/types/react-table-config.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.342612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/utils/URLSearchParamWrapper.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/utils/graph.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/utils/index.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/utils/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/utils/testUtils.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/utils/useErrorToast.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/utils/useErrorToast.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/utils/useOffsetTop.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/variable_edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16671 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/pin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/pin_100.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/pin_25.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/pin_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/pin_35.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/pin_40.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24922 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/pin_large.png
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/sort_asc.png
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/sort_both.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/sort_desc.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.306611 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.346612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/_messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/chart.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/confirm.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/conn_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/conn_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    26111 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/dag.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/dag_audit_log.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/dag_code.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/dag_dependencies.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/dag_details.html
+-rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/dags.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/dataset_next_run_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/datasets.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/duration_chart.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/gantt.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/graph.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/grid.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/model_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/no_roles_permissions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/noaccess.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/plugin.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/providers.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/redoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/task.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/task_instance.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/ti_code.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/ti_log.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/traceback.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/trigger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/variable_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/variable_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/variable_show.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/variable_show_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/xcom.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.346612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/analytics/google_analytics.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/analytics/metarouter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/analytics/segment.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.346612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/appbuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/appbuilder/custom_icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/appbuilder/dag_docs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/appbuilder/flash.html
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/appbuilder/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/appbuilder/loading_dots.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/appbuilder/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/appbuilder/navbar_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/appbuilder/navbar_right.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.346612 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/swagger-ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/swagger-ui/index.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31762 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)   219115 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.346612 pano-airflow-providers-amazon-8.0.1.dev0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-bootstrap.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-bootstrap3-typeahead.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-d3-shape.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-d3-tip.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-d3js.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-dagre-d3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-datatables.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-elasticmock.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-eonasdan-bootstrap-datetimepicker.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-flask-kerberos.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-hue.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-jqclock.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-jquery.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-moment-strftime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-moment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-normalize.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.350612 pano-airflow-providers-amazon-8.0.1.dev0/pano_airflow_providers_amazon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30738 2023-05-25 03:54:18.000000 pano-airflow-providers-amazon-8.0.1.dev0/pano_airflow_providers_amazon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-05-25 03:54:18.000000 pano-airflow-providers-amazon-8.0.1.dev0/pano_airflow_providers_amazon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 03:54:18.000000 pano-airflow-providers-amazon-8.0.1.dev0/pano_airflow_providers_amazon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-25 03:54:18.000000 pano-airflow-providers-amazon-8.0.1.dev0/pano_airflow_providers_amazon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 03:54:18.000000 pano-airflow-providers-amazon-8.0.1.dev0/pano_airflow_providers_amazon.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-25 03:54:18.000000 pano-airflow-providers-amazon-8.0.1.dev0/pano_airflow_providers_amazon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 03:54:18.000000 pano-airflow-providers-amazon-8.0.1.dev0/pano_airflow_providers_amazon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.306611 pano-airflow-providers-amazon-8.0.1.dev0/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:54:18.350612 pano-airflow-providers-amazon-8.0.1.dev0/scripts/systemd/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/scripts/systemd/README
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/scripts/systemd/airflow
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/scripts/systemd/airflow-flower.service
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/scripts/systemd/airflow-kerberos.service
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/scripts/systemd/airflow-scheduler.service
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/scripts/systemd/airflow-webserver.service
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/scripts/systemd/airflow-worker.service
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/scripts/systemd/airflow.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-25 03:54:18.350612 pano-airflow-providers-amazon-8.0.1.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-25 03:54:07.000000 pano-airflow-providers-amazon-8.0.1.dev0/setup.py
```

### Comparing `pano-airflow-providers-amazon-8.0.0/LICENSE` & `pano-airflow-providers-amazon-8.0.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/MANIFEST.in` & `pano-airflow-providers-amazon-8.0.1.dev0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/NOTICE` & `pano-airflow-providers-amazon-8.0.1.dev0/NOTICE`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/README.md` & `pano-airflow-providers-amazon-8.0.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/RELEASE_NOTES.rst` & `pano-airflow-providers-amazon-8.0.1.dev0/RELEASE_NOTES.rst`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/alembic.ini` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/alembic.ini`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/api_connexion/openapi/v1.yaml` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/api_connexion/openapi/v1.yaml`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/config_templates/__init__.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/config_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/config_templates/airflow_local_settings.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/config_templates/airflow_local_settings.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/config_templates/config.yml` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/config_templates/config.yml`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/config_templates/config.yml.schema.json` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/config_templates/config.yml.schema.json`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/config_templates/default_airflow.cfg` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/config_templates/default_airflow.cfg`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/config_templates/default_celery.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/config_templates/default_celery.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/config_templates/default_test.cfg` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/config_templates/default_test.cfg`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/config_templates/default_webserver_config.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/config_templates/default_webserver_config.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/customized_form_field_behaviours.schema.json` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/customized_form_field_behaviours.schema.json`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/example_dags/sql/sample.sql` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/example_dags/sql/sample.sql`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/provider_info.schema.json` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/provider_info.schema.json`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/__init__.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,13 +26,13 @@
 
 import packaging.version
 
 import airflow
 
 __all__ = ["version"]
 
-version = "8.0.0"
+version = "8.0.1.dev0"
 
 if packaging.version.parse(airflow.version.version) < packaging.version.parse("2.4.0"):
     raise RuntimeError(
         f"The package `apache-airflow-providers-amazon:{version}` requires Apache Airflow 2.4.0+"
     )
```

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/__init__.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/exceptions.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/exceptions.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/__init__.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/appflow.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/appflow.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/athena.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/athena.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/base_aws.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/base_aws.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/batch_client.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/batch_client.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/batch_waiters.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/batch_waiters.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/cloud_formation.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/datasync.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/datasync.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/dms.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/dms.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/dynamodb.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/dynamodb.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/ec2.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/ec2.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/ecr.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/ecr.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/ecs.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/ecs.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/eks.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/eks.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/emr.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/emr.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/glacier.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/glacier.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/glue.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/glue.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/glue_catalog.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/glue_catalog.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/glue_crawler.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/kinesis.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/kinesis.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/lambda_function.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/lambda_function.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/logs.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/logs.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/quicksight.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/quicksight.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/rds.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/rds.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/redshift_cluster.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/redshift_data.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/redshift_data.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/redshift_sql.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/redshift_sql.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/s3.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/s3.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/sagemaker.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/sagemaker.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/secrets_manager.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/ses.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/ses.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/sns.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/sns.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/sqs.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/sqs.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/ssm.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/ssm.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/step_function.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/step_function.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/hooks/sts.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/hooks/sts.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/links/__init__.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/links/__init__.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/links/base_aws.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/links/base_aws.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/links/batch.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/links/batch.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/links/emr.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/links/emr.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/links/glue.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/links/glue.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/links/logs.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/links/logs.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/log/__init__.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/log/s3_task_handler.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/log/s3_task_handler.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/__init__.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/appflow.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/appflow.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/athena.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/athena.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/batch.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/batch.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/cloud_formation.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/datasync.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/datasync.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/dms.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/dms.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/ec2.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/ec2.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/ecs.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/ecs.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/eks.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/eks.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/emr.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/emr.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/glacier.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/glacier.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/glue.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/glue.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/glue_crawler.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/lambda_function.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/lambda_function.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/quicksight.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/quicksight.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/rds.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/rds.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/redshift_cluster.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/redshift_data.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/redshift_data.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/s3.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/s3.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/sagemaker.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/sagemaker.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/sns.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/sns.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/sqs.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/sqs.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/operators/step_function.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/operators/step_function.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/secrets/__init__.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/secrets/secrets_manager.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/secrets/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/secrets/systems_manager.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/secrets/systems_manager.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/__init__.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/athena.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/athena.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/batch.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/batch.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/cloud_formation.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/dms.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/dms.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/dynamodb.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/dynamodb.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/ec2.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/ec2.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/ecs.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/ecs.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/eks.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/eks.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/emr.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/emr.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/glacier.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/glacier.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/glue.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/glue.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/glue_crawler.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/lambda_function.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/lambda_function.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/quicksight.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/quicksight.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/rds.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/rds.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/redshift_cluster.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/s3.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/s3.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/sagemaker.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/sagemaker.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/sqs.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/sqs.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/sensors/step_function.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/sensors/step_function.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/__init__.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/base.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/base.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/exasol_to_s3.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/exasol_to_s3.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/ftp_to_s3.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/ftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/gcs_to_s3.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/gcs_to_s3.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/google_api_to_s3.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/google_api_to_s3.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/local_to_s3.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/local_to_s3.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/mongo_to_s3.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/mongo_to_s3.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/redshift_to_s3.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/redshift_to_s3.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/s3_to_ftp.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/s3_to_ftp.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/s3_to_redshift.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/s3_to_redshift.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/s3_to_sftp.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/s3_to_sftp.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/s3_to_sql.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/s3_to_sql.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/sftp_to_s3.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/sftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/transfers/sql_to_s3.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/transfers/sql_to_s3.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/triggers/__init__.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/triggers/redshift_cluster.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/triggers/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/utils/__init__.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/utils/connection_wrapper.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/utils/connection_wrapper.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/utils/eks_get_token.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/utils/eks_get_token.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/utils/emailer.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/utils/emailer.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/utils/rds.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/utils/rds.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/utils/redshift.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/utils/redshift.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/utils/sagemaker.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/utils/sagemaker.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/utils/tags.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/utils/tags.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/utils/waiter.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/utils/waiter.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/waiters/__init__.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/waiters/__init__.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/providers/amazon/aws/waiters/base_waiter.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/providers/amazon/aws/waiters/base_waiter.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/serialization/schema.json` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/serialization/schema.json`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/utils/context.pyi` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/utils/context.pyi`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/utils/python_virtualenv_script.jinja2` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/utils/python_virtualenv_script.jinja2`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/.eslintrc` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/.eslintrc`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/__init__.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/__init__.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/alias-rest-types.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/alias-rest-types.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/api/__init__.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/api/experimental/__init__.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/api/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/api/experimental/endpoints.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/api/experimental/endpoints.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/app.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/app.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/auth.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/auth.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/babel.config.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/babel.config.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/blueprints.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/blueprints.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/decorators.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/decorators.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/__init__.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_appbuilder.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_appbuilder.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_appbuilder_links.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_appbuilder_links.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_cache.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_cache.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_dagbag.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_dagbag.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_jinja_globals.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_jinja_globals.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_manifest_files.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_manifest_files.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_robots.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_robots.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_security.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_security.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_session.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_session.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_views.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_views.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/extensions/init_wsgi_middlewares.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/extensions/init_wsgi_middlewares.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/fab_security/__init__.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/fab_security/__init__.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/fab_security/manager.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/fab_security/manager.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/fab_security/sqla/__init__.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/fab_security/sqla/__init__.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/fab_security/sqla/manager.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/fab_security/sqla/manager.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/fab_security/sqla/models.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/fab_security/sqla/models.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/fab_security/views.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/fab_security/views.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/forms.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/forms.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/gunicorn_config.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/jest-setup.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/jest-setup.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/jest.config.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/jest.config.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/package.json` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/package.json`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/security.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/security.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/session.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/session.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/airflow.gif` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/airflow.gif`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/bootstrap-theme.css` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/calendar.css` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/calendar.css`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/chart.css` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/chart.css`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/dags.css` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/dags.css`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/flash.css` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/flash.css`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/gantt.css` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/gantt.css`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/graph.css` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/graph.css`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/loading-dots.css` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/loading-dots.css`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/main.css` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/main.css`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/material-icons.css` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/material-icons.css`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/css/switch.css` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/css/switch.css`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/declarations.d.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/declarations.d.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/App.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/App.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/README.md` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/README.md`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/index.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/index.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useClearRun.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useClearRun.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useClearTask.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useClearTask.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useClearTaskDryRun.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useClearTaskDryRun.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useDataset.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useDataset.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useDatasetDependencies.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useDatasetDependencies.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useDatasetEvents.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useDatasetEvents.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useDatasets.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useDatasets.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useExtraLinks.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useExtraLinks.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useGraphData.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useGraphData.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useGridData.test.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useGridData.test.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useGridData.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useGridData.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useMappedInstances.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useMappedInstances.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useMarkFailedRun.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useMarkFailedRun.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useMarkFailedTask.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useMarkFailedTask.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useMarkSuccessRun.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useMarkSuccessRun.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useMarkSuccessTask.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useMarkSuccessTask.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useMarkTaskDryRun.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useMarkTaskDryRun.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useQueueRun.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useQueueRun.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useSetDagRunNote.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useSetDagRunNote.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useSetTaskInstanceNote.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useSetTaskInstanceNote.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useTaskInstance.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useTaskInstance.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useTaskLog.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useTaskLog.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/api/useUpstreamDatasetEvents.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/api/useUpstreamDatasetEvents.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/calendar.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/calendar.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/callModal.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/callModal.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/AutoRefresh.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/AutoRefresh.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/Clipboard.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/Clipboard.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/Clipboard.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/Clipboard.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/InfoTooltip.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/InfoTooltip.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/LinkButton.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/LinkButton.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/LinkButton.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/LinkButton.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/MultiSelect.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/MultiSelect.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/ReactMarkdown.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/ReactMarkdown.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/RunTypeIcon.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/RunTypeIcon.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/TabWithTooltip.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/TabWithTooltip.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/Table/Cells.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/Table/Cells.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/Table/Cells.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/Table/Cells.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/Table/Table.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/Table/Table.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/Table/index.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/Table/index.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/Time.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/Time.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/Time.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/Time.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/components/Tooltip.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/components/Tooltip.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/connection_form.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/connection_form.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/context/autorefresh.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/context/autorefresh.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/context/containerRef.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/context/containerRef.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/context/timezone.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/context/timezone.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/InstanceTooltip.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/InstanceTooltip.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/InstanceTooltip.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/InstanceTooltip.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/Main.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/Main.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/StatusBox.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/StatusBox.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/BreadcrumbText.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/BreadcrumbText.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/Dag.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/Dag.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/FilterTasks.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/FilterTasks.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/Header.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/Header.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/NotesAccordion.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/NotesAccordion.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/NotesAccordion.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/NotesAccordion.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/dagRun/ClearRun.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/dagRun/ClearRun.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/dagRun/DatasetTriggerEvents.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/dagRun/DatasetTriggerEvents.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/dagRun/MarkRunAs.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/dagRun/MarkRunAs.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/dagRun/index.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/dagRun/index.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/graph/Edge.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/graph/Edge.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/graph/Node.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/graph/Node.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/graph/Node.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/graph/Node.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/graph/index.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/graph/index.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/graph/utils.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/graph/utils.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/index.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/index.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/BackToTaskSummary.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/BackToTaskSummary.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/DatasetUpdateEvents.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/DatasetUpdateEvents.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/Details.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/Details.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/ExtraLinks.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/ExtraLinks.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/Logs/LogBlock.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/Logs/LogBlock.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/Logs/LogLink.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/Logs/LogLink.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/Logs/LogLink.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/Logs/LogLink.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/Logs/index.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/Logs/index.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/Logs/index.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/Logs/index.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/Logs/utils.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/Logs/utils.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/Logs/utils.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/Logs/utils.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/MappedInstances.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/MappedInstances.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/Nav.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/Nav.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/index.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/index.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/taskActions/ActionButton.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/taskActions/ActionButton.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/taskActions/ActionModal.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/taskActions/ActionModal.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/taskActions/ClearInstance.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/taskActions/ClearInstance.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/details/taskInstance/taskActions/MarkInstanceAs.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/details/taskInstance/taskActions/MarkInstanceAs.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/TaskName.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/TaskName.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/TaskName.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/TaskName.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/ToggleGroups.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/ToggleGroups.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/dagRuns/Bar.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/dagRuns/Bar.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/dagRuns/Tooltip.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/dagRuns/Tooltip.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/dagRuns/index.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/dagRuns/index.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/dagRuns/index.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/dagRuns/index.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/index.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/index.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/index.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/index.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/renderTaskRows.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/renderTaskRows.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/grid/renderTaskRows.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/grid/renderTaskRows.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/index.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/index.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/nav/FilterBar.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/nav/FilterBar.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/nav/LegendRow.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/nav/LegendRow.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/nav/LegendRow.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/nav/LegendRow.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/useFilters.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/useFilters.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/useFilters.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/useFilters.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/useSelection.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/useSelection.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/useSelection.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/useSelection.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag/useToggleGroups.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag/useToggleGroups.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag_code.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag_code.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dag_dependencies.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dag_dependencies.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/dags.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/dags.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasetUtils.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasetUtils.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/DatasetEvents.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/DatasetEvents.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/Details.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/Details.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/Graph/DagNode.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/Graph/DagNode.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/Graph/Edge.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/Graph/Edge.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/Graph/Legend.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/Graph/Legend.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/Graph/Node.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/Graph/Node.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/Graph/index.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/Graph/index.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/List.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/List.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/List.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/List.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datasets/index.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datasets/index.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/datetime_utils.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/datetime_utils.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/duration_chart.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/duration_chart.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/gantt.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/gantt.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/graph.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/graph.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/index.d.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/index.d.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/main.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/main.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/task.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/task.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/task_instances.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/task_instances.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/theme.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/theme.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/ti_log.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/ti_log.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/trigger.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/trigger.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/types/api-generated.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/types/api-generated.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/types/index.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/types/index.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/types/react-table-config.d.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/types/react-table-config.d.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/utils/URLSearchParamWrapper.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/utils/URLSearchParamWrapper.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/utils/graph.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/utils/graph.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/utils/index.test.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/utils/index.test.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/utils/index.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/utils/index.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/utils/testUtils.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/utils/testUtils.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/utils/useErrorToast.test.tsx` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/utils/useErrorToast.test.tsx`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/utils/useErrorToast.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/utils/useErrorToast.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/utils/useOffsetTop.ts` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/utils/useOffsetTop.ts`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/js/variable_edit.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/js/variable_edit.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/loading.gif` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/loading.gif`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/pin.svg` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/pin.svg`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/pin_100.png` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/pin_100.png`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/pin_25.png` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/pin_25.png`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/pin_32.png` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/pin_32.png`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/pin_35.png` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/pin_35.png`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/pin_40.png` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/pin_40.png`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/static/pin_large.png` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/static/pin_large.png`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/_messages.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/_messages.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/calendar.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/calendar.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/chart.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/chart.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/config.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/config.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/confirm.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/confirm.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/conn_create.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/conn_create.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/conn_edit.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/conn_edit.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/dag.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/dag.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/dag_audit_log.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/dag_audit_log.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/dag_code.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/dag_code.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/dag_dependencies.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/dag_dependencies.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/dag_details.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/dag_details.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/dags.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/dags.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/dataset_next_run_modal.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/dataset_next_run_modal.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/datasets.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/datasets.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/duration_chart.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/duration_chart.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/error.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/error.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/gantt.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/gantt.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/graph.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/graph.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/grid.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/grid.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/main.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/main.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/model_list.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/model_list.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/no_roles_permissions.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/no_roles_permissions.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/noaccess.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/noaccess.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/plugin.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/plugin.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/providers.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/providers.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/redoc.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/redoc.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/task.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/task.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/task_instance.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/task_instance.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/ti_code.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/ti_code.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/ti_log.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/ti_log.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/traceback.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/traceback.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/trigger.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/trigger.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/variable_edit.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/variable_edit.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/variable_list.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/variable_list.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/variable_show.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/variable_show.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/variable_show_widget.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/variable_show_widget.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/airflow/xcom.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/airflow/xcom.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/analytics/google_analytics.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/analytics/google_analytics.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/analytics/metarouter.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/analytics/metarouter.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/analytics/segment.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/analytics/segment.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/appbuilder/custom_icons.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/appbuilder/custom_icons.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/appbuilder/dag_docs.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/appbuilder/dag_docs.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/appbuilder/flash.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/appbuilder/flash.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/appbuilder/index.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/appbuilder/index.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/appbuilder/loading_dots.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/appbuilder/loading_dots.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/appbuilder/navbar.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/appbuilder/navbar.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/appbuilder/navbar_menu.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/appbuilder/navbar_menu.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/appbuilder/navbar_right.html` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/appbuilder/navbar_right.html`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/templates/swagger-ui/index.j2` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/templates/swagger-ui/index.j2`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/tsconfig.json` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/tsconfig.json`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/utils.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/utils.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/validators.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/validators.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/views.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/views.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/webpack.config.js` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/webpack.config.js`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/airflow/www/widgets.py` & `pano-airflow-providers-amazon-8.0.1.dev0/airflow/www/widgets.py`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-bootstrap.txt` & `pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-bootstrap.txt`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-bootstrap3-typeahead.txt` & `pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-bootstrap3-typeahead.txt`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-d3-shape.txt` & `pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-d3-shape.txt`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-d3-tip.txt` & `pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-d3-tip.txt`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-d3js.txt` & `pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-d3js.txt`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-dagre-d3.txt` & `pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-dagre-d3.txt`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-datatables.txt` & `pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-datatables.txt`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-elasticmock.txt` & `pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-elasticmock.txt`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-eonasdan-bootstrap-datetimepicker.txt` & `pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-eonasdan-bootstrap-datetimepicker.txt`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-flask-kerberos.txt` & `pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-flask-kerberos.txt`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-hue.txt` & `pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-hue.txt`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-jqclock.txt` & `pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-jqclock.txt`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-jquery.txt` & `pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-jquery.txt`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-moment-strftime.txt` & `pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-moment-strftime.txt`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-moment.txt` & `pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-moment.txt`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/licenses/LICENSE-normalize.txt` & `pano-airflow-providers-amazon-8.0.1.dev0/licenses/LICENSE-normalize.txt`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/pano_airflow_providers_amazon.egg-info/SOURCES.txt` & `pano-airflow-providers-amazon-8.0.1.dev0/pano_airflow_providers_amazon.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 README.md
 RELEASE_NOTES.rst
 pyproject.toml
 setup.cfg
 setup.py
 airflow/alembic.ini
 airflow/customized_form_field_behaviours.schema.json
-airflow/git_version
 airflow/provider_info.schema.json
 airflow/api_connexion/openapi/v1.yaml
 airflow/config_templates/__init__.py
 airflow/config_templates/airflow_local_settings.py
 airflow/config_templates/config.yml
 airflow/config_templates/config.yml.schema.json
 airflow/config_templates/default_airflow.cfg
```

### Comparing `pano-airflow-providers-amazon-8.0.0/pano_airflow_providers_amazon.egg-info/requires.txt` & `pano-airflow-providers-amazon-8.0.1.dev0/pano_airflow_providers_amazon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/pyproject.toml` & `pano-airflow-providers-amazon-8.0.1.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/scripts/systemd/README` & `pano-airflow-providers-amazon-8.0.1.dev0/scripts/systemd/README`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/scripts/systemd/airflow` & `pano-airflow-providers-amazon-8.0.1.dev0/scripts/systemd/airflow`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/scripts/systemd/airflow-flower.service` & `pano-airflow-providers-amazon-8.0.1.dev0/scripts/systemd/airflow-flower.service`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/scripts/systemd/airflow-kerberos.service` & `pano-airflow-providers-amazon-8.0.1.dev0/scripts/systemd/airflow-kerberos.service`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/scripts/systemd/airflow-scheduler.service` & `pano-airflow-providers-amazon-8.0.1.dev0/scripts/systemd/airflow-scheduler.service`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/scripts/systemd/airflow-webserver.service` & `pano-airflow-providers-amazon-8.0.1.dev0/scripts/systemd/airflow-webserver.service`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/scripts/systemd/airflow-worker.service` & `pano-airflow-providers-amazon-8.0.1.dev0/scripts/systemd/airflow-worker.service`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/scripts/systemd/airflow.conf` & `pano-airflow-providers-amazon-8.0.1.dev0/scripts/systemd/airflow.conf`

 * *Files identical despite different names*

### Comparing `pano-airflow-providers-amazon-8.0.0/setup.cfg` & `pano-airflow-providers-amazon-8.0.1.dev0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = pano-airflow-providers-amazon
 summary = Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 description = Provider package apache-airflow-providers-amazon for Apache Airflow
-long_description = file: README.rst
-long_description_content_type = text/x-rst
+long_description = file: README.md
+long_description_content_type = text/markdown
 author = Apache Software Foundation
 author_email = dev@airflow.apache.org
 url = https://airflow.apache.org/
 download_url = https://archive.apache.org/dist/airflow/providers
 license = Apache License 2.0
 license_files = 
 	LICENSE
@@ -23,15 +23,14 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.0.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `pano-airflow-providers-amazon-8.0.0/setup.py` & `pano-airflow-providers-amazon-8.0.1.dev0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-amazon package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "8.0.0"
+version = "8.0.1.dev0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-amazon setup."""
     setup(
         version=version,
         extras_require={
@@ -55,8 +55,8 @@
                 "airflow.providers.amazon_vendor.*",
             ],
         ),
     )
 
 
 if __name__ == "__main__":
-    do_setup()
+    do_setup()
```

