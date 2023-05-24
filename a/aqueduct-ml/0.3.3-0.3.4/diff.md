# Comparing `tmp/aqueduct-ml-0.3.3.tar.gz` & `tmp/aqueduct-ml-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduct-ml-0.3.3.tar", last modified: Wed May 17 17:21:29 2023, max compression
+gzip compressed data, was "aqueduct-ml-0.3.4.tar", last modified: Wed May 24 22:48:45 2023, max compression
```

## Comparing `aqueduct-ml-0.3.3.tar` & `aqueduct-ml-0.3.4.tar`

### file list

```diff
@@ -1,130 +1,131 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.644296 aqueduct-ml-0.3.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7719 2023-05-17 17:21:29.644296 aqueduct-ml-0.3.3/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.632296 aqueduct-ml-0.3.3/aqueduct_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.632296 aqueduct-ml-0.3.3/aqueduct_executor/migrators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.632296 aqueduct-ml-0.3.3/aqueduct_executor/migrators/artifact_migration_000016/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4538 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/artifact_migration_000016/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      441 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/artifact_migration_000016/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/artifact_migration_000016/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.632296 aqueduct-ml-0.3.3/aqueduct_executor/migrators/backfill_python_type_000022/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      445 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/backfill_python_type_000022/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      437 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.632296 aqueduct-ml-0.3.3/aqueduct_executor/migrators/parameter_val_type_inference_000019/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4168 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.632296 aqueduct-ml-0.3.3/aqueduct_executor/operators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.636296 aqueduct-ml-0.3.3/aqueduct_executor/operators/airflow/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/airflow/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3092 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/airflow/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/airflow/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1122 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/airflow/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.636296 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.636296 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2680 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/athena.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      134 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/azure_sql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3990 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/bigquery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      658 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2892 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1829 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/connector.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16224 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6057 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/extract.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1462 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/gcs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      725 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/maria_db.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3821 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/mongodb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      798 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/postgres.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      129 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/redshift.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4774 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/relational.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9602 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7001 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/s3_serialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1808 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/snowflake.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.636296 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/spark/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/spark/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5385 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/spark/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2833 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/spark/snowflake.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5478 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/spec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1722 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/sql_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2434 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2728 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.640296 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2349 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/conf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      254 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/conftest.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1909 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_bigquery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1169 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_mariadb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_postgres.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_redshift.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_snowflake.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1173 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_sql_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1150 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      925 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.640296 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17252 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2770 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/extract_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      801 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/get_extract_path.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3286 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/install_requirements.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1276 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1280 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/set_conda_version.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/spec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.640296 aqueduct-ml-0.3.3/aqueduct_executor/operators/param_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/param_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3211 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/param_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1097 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/param_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/param_executor/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.640296 aqueduct-ml-0.3.3/aqueduct_executor/operators/spark/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/spark/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2683 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/spark/execute_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1020 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/spark/execute_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5401 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/spark/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.640296 aqueduct-ml-0.3.3/aqueduct_executor/operators/system_metric_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/system_metric_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2264 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/system_metric_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1105 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/system_metric_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      837 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/system_metric_executor/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.640296 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2259 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/enums.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      465 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7531 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/execution.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/saved_object_delete.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.640296 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      914 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1354 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/gcs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      720 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/parse.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3780 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      288 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/storage.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/timer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9254 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.644296 aqueduct-ml-0.3.3/aqueduct_ml.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7719 2023-05-17 17:21:29.000000 aqueduct-ml-0.3.3/aqueduct_ml.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5737 2023-05-17 17:21:29.000000 aqueduct-ml-0.3.3/aqueduct_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-17 17:21:29.000000 aqueduct-ml-0.3.3/aqueduct_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      248 2023-05-17 17:21:29.000000 aqueduct-ml-0.3.3/aqueduct_ml.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-05-17 17:21:29.000000 aqueduct-ml-0.3.3/aqueduct_ml.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.644296 aqueduct-ml-0.3.3/bin/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    29290 2023-05-17 01:51:34.000000 aqueduct-ml-0.3.3/bin/aqueduct
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-05-17 01:51:34.000000 aqueduct-ml-0.3.3/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-17 17:21:29.644296 aqueduct-ml-0.3.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-17 01:51:34.000000 aqueduct-ml-0.3.3/version
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.337711 aqueduct-ml-0.3.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7719 2023-05-24 22:48:45.337711 aqueduct-ml-0.3.4/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.305711 aqueduct-ml-0.3.4/aqueduct_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.305711 aqueduct-ml-0.3.4/aqueduct_executor/migrators/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.309712 aqueduct-ml-0.3.4/aqueduct_executor/migrators/artifact_migration_000016/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4538 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/artifact_migration_000016/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      441 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/artifact_migration_000016/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/artifact_migration_000016/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.309712 aqueduct-ml-0.3.4/aqueduct_executor/migrators/backfill_python_type_000022/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      445 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/backfill_python_type_000022/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      437 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.313712 aqueduct-ml-0.3.4/aqueduct_executor/migrators/parameter_val_type_inference_000019/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4168 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.313712 aqueduct-ml-0.3.4/aqueduct_executor/operators/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.313712 aqueduct-ml-0.3.4/aqueduct_executor/operators/airflow/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/airflow/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3092 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/airflow/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/airflow/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1122 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/airflow/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.313712 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.321711 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2680 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/athena.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      134 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/azure_sql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3970 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/bigquery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      658 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2892 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1829 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/connector.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16614 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5201 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/extract.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1462 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/gcs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      725 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/load.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/maria_db.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3821 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/mongodb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      798 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1742 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/parameters.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/postgres.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      129 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/redshift.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4774 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/relational.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9602 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7001 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/s3_serialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1808 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/snowflake.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.321711 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/spark/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/spark/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5385 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/spark/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2833 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/spark/snowflake.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5478 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/spec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1722 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/sql_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2434 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2728 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.329712 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2349 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/conf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      254 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/conftest.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1909 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_bigquery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1169 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_mariadb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_postgres.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_redshift.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_snowflake.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1173 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_sql_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1150 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      925 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.329712 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17252 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2770 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/extract_function.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      801 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/get_extract_path.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3286 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/install_requirements.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1276 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1280 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/set_conda_version.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/spec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.333711 aqueduct-ml-0.3.4/aqueduct_executor/operators/param_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/param_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3211 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/param_executor/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1097 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/param_executor/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/param_executor/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.333711 aqueduct-ml-0.3.4/aqueduct_executor/operators/spark/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/spark/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2683 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/spark/execute_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1020 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/spark/execute_function.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5401 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/spark/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.333711 aqueduct-ml-0.3.4/aqueduct_executor/operators/system_metric_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/system_metric_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2264 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/system_metric_executor/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1105 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/system_metric_executor/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      837 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/system_metric_executor/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.337711 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2259 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/enums.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      465 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7531 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/execution.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/saved_object_delete.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.337711 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      914 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1354 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/gcs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      720 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/parse.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3780 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      288 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/storage.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/timer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9254 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.337711 aqueduct-ml-0.3.4/aqueduct_ml.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7719 2023-05-24 22:48:45.000000 aqueduct-ml-0.3.4/aqueduct_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5795 2023-05-24 22:48:45.000000 aqueduct-ml-0.3.4/aqueduct_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-24 22:48:45.000000 aqueduct-ml-0.3.4/aqueduct_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      248 2023-05-24 22:48:45.000000 aqueduct-ml-0.3.4/aqueduct_ml.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-05-24 22:48:45.000000 aqueduct-ml-0.3.4/aqueduct_ml.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:45.337711 aqueduct-ml-0.3.4/bin/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    29429 2023-05-24 22:27:12.000000 aqueduct-ml-0.3.4/bin/aqueduct
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-05-24 22:27:12.000000 aqueduct-ml-0.3.4/requirements.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-24 22:48:45.337711 aqueduct-ml-0.3.4/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-05-24 04:24:42.000000 aqueduct-ml-0.3.4/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-24 22:27:12.000000 aqueduct-ml-0.3.4/version
```

### Comparing `aqueduct-ml-0.3.3/PKG-INFO` & `aqueduct-ml-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-ml
-Version: 0.3.3
+Version: 0.3.4
 Summary: The control center for ML in the cloud
 Home-page: https://www.aqueducthq.com/
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/migrators/artifact_migration_000016/execute.py` & `aqueduct-ml-0.3.4/aqueduct_executor/migrators/artifact_migration_000016/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/migrators/backfill_python_type_000022/execute.py` & `aqueduct-ml-0.3.4/aqueduct_executor/migrators/backfill_python_type_000022/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py` & `aqueduct-ml-0.3.4/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py` & `aqueduct-ml-0.3.4/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py` & `aqueduct-ml-0.3.4/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py` & `aqueduct-ml-0.3.4/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/airflow/execute.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/airflow/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/airflow/spec.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/airflow/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/athena.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/athena.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/bigquery.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 from typing import Any, Dict, List, Optional
 
-import pandas as pd
 from aqueduct_executor.operators.connectors.data import common, config, connector, extract, load
 from aqueduct_executor.operators.utils.enums import ArtifactType
 from aqueduct_executor.operators.utils.saved_object_delete import SavedObjectDelete
 from aqueduct_executor.operators.utils.utils import delete_object
 from google.cloud import bigquery
 from google.cloud.exceptions import NotFound
 from google.oauth2 import service_account
```

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/common.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/common.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/config.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/connector.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/connector.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/execute.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import platform
 import sys
 from typing import Any
 
 from aqueduct_executor.operators.connectors.data import common, config, connector, extract
-from aqueduct_executor.operators.connectors.data.load import RelationalParams
+from aqueduct_executor.operators.connectors.data.load import RelationalParams, S3Params
+from aqueduct_executor.operators.connectors.data.parameters import (
+    _replace_parameterized_user_strings,
+)
 from aqueduct_executor.operators.connectors.data.spec import (
     AQUEDUCT_DEMO_NAME,
     AuthenticateSpec,
     DiscoverSpec,
     ExtractSpec,
     LoadSpec,
     LoadTableSpec,
@@ -268,28 +271,35 @@
         storage=storage,
         input_paths=spec.input_content_paths,
         input_metadata_paths=spec.input_metadata_paths,
         **kwargs,
     )
     if len(inputs) == 0:
         raise Exception("Expected at least one input artifact!")
-    if len(inputs) > 2:
-        raise Exception("Unexpected number of inputs to save operator: %v.", len(inputs))
 
-    # Handle any parameterization of the save queries here. Currently, we only support
-    # the parameterization of the `table_name` for SQL connectors.
+    # Handle any parameterization of the save queries here.
     if len(inputs) > 1:
-        if not isinstance(spec.parameters, RelationalParams):
-            raise Exception("Only relational database resources support parameterized saves.")
-
-        assert (
-            len(spec.parameters.table) == 0
-        ), "A parameterized relational save spec should have an empty table name."
-        assert isinstance(inputs[0], str), "Relational saves can only have string parameters."
-        spec.parameters.table = inputs[0]
+        for idx, input in enumerate(inputs[:-1]):
+            if not isinstance(input, str):
+                raise Exception(
+                    "Unexpected input type %s to save at %s-th index." % (type(input), idx)
+                )
+
+        param_input_vals = [str(input) for input in inputs[:-1]]
+        if isinstance(spec.parameters, RelationalParams):
+            assert (
+                len(spec.parameters.table) == 0
+            ), "A parameterized relational save spec should have an empty table name."
+            spec.parameters.table = param_input_vals[0]
+        elif isinstance(spec.parameters, S3Params):
+            spec.parameters.filepath = _replace_parameterized_user_strings(
+                spec.parameters.filepath, param_input_vals
+            )
+        else:
+            raise Exception("Parameters are only supported for S3 and Relational Data Resources.")
 
     # Any parameters are expected to have been resolved by the time we get here.
     @exec_state.user_fn_redirected(failure_tip=TIP_LOAD)
     def _load() -> None:
         if is_spark:
             op.load_spark(spec.parameters, inputs[-1], input_types[-1])  # type: ignore
         else:
@@ -342,14 +352,15 @@
 
         from aqueduct_executor.operators.connectors.data.snowflake import (  # type: ignore
             SnowflakeConnector as OpConnector,
         )
     elif connector_name == common.Name.BIG_QUERY:
         try:
             from google.cloud import bigquery
+            import db_dtypes
         except:
             raise MissingConnectorDependencyException(
                 "Unable to initialize the BigQuery connector. Have you run `aqueduct install bigquery`?"
             )
 
         from aqueduct_executor.operators.connectors.data.bigquery import (  # type: ignore
             BigQueryConnector as OpConnector,
```

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/extract.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/extract.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,20 @@
 import json
-import re
 import uuid
 from typing import Any, Dict, List, Optional, Union
 
-from aqueduct.resources.parameters import BUILT_IN_EXPANSIONS, TAG_PATTERN
 from aqueduct_executor.operators.connectors.data import common, models
+from aqueduct_executor.operators.connectors.data.parameters import (
+    PREV_TABLE_TAG,
+    _replace_builtin_tags,
+    _replace_param_sql_placeholders,
+)
 from aqueduct_executor.operators.utils.enums import ArtifactType
 from pydantic import parse_obj_as
 
-# The TAG for 'previous table' when the user specifies a chained query.
-PREV_TABLE_TAG = "$"
-
-
-def _replace_builtin_tags(query: str) -> str:
-    """Expands any builtin tags found in the raw query, eg. {{ today }}."""
-    matches = re.findall(TAG_PATTERN, query)
-    for match in matches:
-        tag_name = match.strip(" {}")
-        if tag_name in BUILT_IN_EXPANSIONS:
-            expansion_func = BUILT_IN_EXPANSIONS[tag_name]
-            query = query.replace(match, expansion_func())
-    return query
-
-
-def _replace_param_placeholders(query: str, parameter_vals: List[str]) -> str:
-    """Replaces any user-defined placeholders in the query with the corresponding parameter value.
-
-    Assumes that we've already validated that every parameter value has a corresponding placeholder in the query.
-    """
-    for i in range(len(parameter_vals)):
-        query = query.replace("$" + str(i + 1), parameter_vals[i])
-    return query
-
 
 class RelationalParams(models.BaseParams):
     # The query cannot be used until `apply_placeholders()` is called on it. This flushes out
     # any user-defined tags like `{{today}}`.
     query_is_usable: Optional[bool] = False
 
     # Exactly one of 'query' and 'queries' will be set.
@@ -113,15 +92,15 @@
 
         queries = self.queries or []
         if self.query:
             queries = [self.query]
 
         # Expand the placeholders first, before collapsing the query chain, since $ is broader than $1, $2, etc.
         for i, q in enumerate(queries):
-            q = _replace_param_placeholders(q, parameter_vals)
+            q = _replace_param_sql_placeholders(q, parameter_vals)
             queries[i] = _replace_builtin_tags(q)
         print(f"Expanded queries are `{queries}`.")
 
         print(f"Compiling queries {queries} .")
         query = self._compile_chain(queries)
         print(f"Compiled query is {query} .")
 
@@ -152,15 +131,15 @@
 
 class MongoDBParams(models.BaseParams):
     collection: str
     query_serialized: str
     query: Optional[MongoDBFindParams] = None
 
     def compile(self, parameters: List[str]) -> None:
-        expanded = _replace_param_placeholders(self.query_serialized, parameters)
+        expanded = _replace_param_sql_placeholders(self.query_serialized, parameters)
         self.query = parse_obj_as(MongoDBFindParams, json.loads(expanded))
 
     def usable(self) -> bool:
         return bool(self.query) and bool(self.collection)
 
 
 Params = Union[RelationalParams, S3Params, MongoDBParams]
```

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/gcs.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/gcs.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/load.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/load.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/main.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/models.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/models.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/mongodb.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/mongodb.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/mysql.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/mysql.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/postgres.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/postgres.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/relational.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/relational.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/s3.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/s3_serialization.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/s3_serialization.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/snowflake.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/spark/s3.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/spark/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/spark/snowflake.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/spark/snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/spec.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/sql_server.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/sql_server.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/sqlite.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/sqlite.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/utils.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/data/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/conf.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/conf.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_bigquery.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_mariadb.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_mysql.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_postgres.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_redshift.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_redshift.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_snowflake.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_sql_server.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_sql_server.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_sqlite.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/utils.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/connectors/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/execute.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/extract_function.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/extract_function.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/get_extract_path.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/get_extract_path.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/install_requirements.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/install_requirements.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/main.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/set_conda_version.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/set_conda_version.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/spec.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/function_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/param_executor/execute.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/param_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/param_executor/main.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/param_executor/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/param_executor/spec.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/param_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/spark/execute_data.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/spark/execute_data.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/spark/execute_function.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/spark/execute_function.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/spark/utils.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/spark/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/system_metric_executor/execute.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/system_metric_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/system_metric_executor/main.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/system_metric_executor/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/system_metric_executor/spec.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/system_metric_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/enums.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/enums.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/execution.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/execution.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/config.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/file.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/file.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/gcs.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/parse.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/parse.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/s3.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/storage/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/timer.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/timer.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/utils.py` & `aqueduct-ml-0.3.4/aqueduct_executor/operators/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.3/aqueduct_ml.egg-info/PKG-INFO` & `aqueduct-ml-0.3.4/aqueduct_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-ml
-Version: 0.3.3
+Version: 0.3.4
 Summary: The control center for ML in the cloud
 Home-page: https://www.aqueducthq.com/
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `aqueduct-ml-0.3.3/aqueduct_ml.egg-info/SOURCES.txt` & `aqueduct-ml-0.3.4/aqueduct_ml.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 aqueduct_executor/operators/connectors/data/gcs.py
 aqueduct_executor/operators/connectors/data/load.py
 aqueduct_executor/operators/connectors/data/main.py
 aqueduct_executor/operators/connectors/data/maria_db.py
 aqueduct_executor/operators/connectors/data/models.py
 aqueduct_executor/operators/connectors/data/mongodb.py
 aqueduct_executor/operators/connectors/data/mysql.py
+aqueduct_executor/operators/connectors/data/parameters.py
 aqueduct_executor/operators/connectors/data/postgres.py
 aqueduct_executor/operators/connectors/data/redshift.py
 aqueduct_executor/operators/connectors/data/relational.py
 aqueduct_executor/operators/connectors/data/s3.py
 aqueduct_executor/operators/connectors/data/s3_serialization.py
 aqueduct_executor/operators/connectors/data/snowflake.py
 aqueduct_executor/operators/connectors/data/spec.py
```

### Comparing `aqueduct-ml-0.3.3/bin/aqueduct` & `aqueduct-ml-0.3.4/bin/aqueduct`

 * *Files 1% similar despite different names*

```diff
@@ -23,25 +23,26 @@
 SCHEMA_VERSION = "26"
 CHUNK_SIZE = 4096
 
 # Connector Package Version Bounds
 PYMONGO_VERSION_BOUND = "<=4.3.3"
 PSYCOPG2_VERSION_BOUND = "<=2.9.5"
 BIGQUERY_VERSION_BOUND = "<=3.5.0"
+DB_DTYPES_VERSION_BOUND = "<=1.1.1"
 SNOWFLAKE_VERSION_BOUND = "<=1.4.4"
 PYARROW_VERSION_BOUND = "<=11.0.0"
 AWS_WRANGLER_VERSION_BOUND = "<=2.19.0"
 MYSQL_CLIENT_VERSION_BOUND = "<=2.1.1"
 PYODBC_VERSION_BOUND = "<=4.0.35"
 
 base_directory = os.path.join(os.environ["HOME"], ".aqueduct")
 server_directory = os.path.join(os.environ["HOME"], ".aqueduct", "server")
 ui_directory = os.path.join(os.environ["HOME"], ".aqueduct", "ui")
 
-package_version = "0.3.3"
+package_version = "0.3.4"
 aws_credentials_path = os.path.join(os.environ["HOME"], ".aws", "credentials")
 
 default_server_port = 8080
 
 s3_server_prefix = (
     "https://aqueduct-ai.s3.us-east-2.amazonaws.com/assets/%s/server" % package_version
 )
@@ -471,14 +472,15 @@
 
 def install_postgres():
     execute_command([sys.executable, "-m", "pip", "install", "psycopg2-binary%s" % PSYCOPG2_VERSION_BOUND])
 
 
 def install_bigquery():
     execute_command([sys.executable, "-m", "pip", "install", "google-cloud-bigquery%s" % BIGQUERY_VERSION_BOUND])
+    execute_command([sys.executable, "-m", "pip", "install", "db-dtypes%s" % DB_DTYPES_VERSION_BOUND])
 
 
 def install_snowflake():
     execute_command([sys.executable, "-m", "pip", "install", "snowflake-sqlalchemy%s" % SNOWFLAKE_VERSION_BOUND])
 
 
 def install_s3():
```

### Comparing `aqueduct-ml-0.3.3/setup.py` & `aqueduct-ml-0.3.4/setup.py`

 * *Files identical despite different names*

