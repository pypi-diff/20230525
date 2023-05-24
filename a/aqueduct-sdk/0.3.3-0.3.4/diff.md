# Comparing `tmp/aqueduct-sdk-0.3.3.tar.gz` & `tmp/aqueduct-sdk-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduct-sdk-0.3.3.tar", last modified: Wed May 17 16:03:38 2023, max compression
+gzip compressed data, was "aqueduct-sdk-0.3.4.tar", last modified: Wed May 24 22:48:10 2023, max compression
```

## Comparing `aqueduct-sdk-0.3.3.tar` & `aqueduct-sdk-0.3.4.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.508865 aqueduct-sdk-0.3.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7716 2023-05-17 16:03:38.508865 aqueduct-sdk-0.3.3/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.500865 aqueduct-sdk-0.3.3/aqueduct/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1530 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.500865 aqueduct-sdk-0.3.3/aqueduct/artifacts/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/_create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1815 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/base_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4188 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/bool_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3729 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4688 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/generic_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11713 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/numeric_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6599 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/preview.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4124 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/system_metric.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24895 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/table_artifact.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.500865 aqueduct-sdk-0.3.3/aqueduct/backend/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/backend/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24525 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/backend/api_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6091 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/backend/response_helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35831 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.500865 aqueduct-sdk-0.3.3/aqueduct/constants/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/constants/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6626 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/constants/enums.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/constants/exports.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/constants/metrics.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    52868 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/decorator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3930 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/error.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5525 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/flow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7295 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/flow_run.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8260 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/github.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.500865 aqueduct-sdk-0.3.3/aqueduct/globals/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      200 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/globals/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/globals/api_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      477 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/globals/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      192 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/globals/dag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8506 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/llm_wrapper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/logger.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.500865 aqueduct-sdk-0.3.3/aqueduct/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      574 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19371 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/dag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/dag_rules.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      554 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/execution_state.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3061 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7786 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/operators.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12714 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/response_models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      176 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.504865 aqueduct-sdk-0.3.3/aqueduct/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      285 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      474 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/airflow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      624 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/aws.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      464 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/aws_lambda.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13077 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/connect_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      486 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/databricks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7518 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/dynamic_k8s.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1789 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/ecr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4878 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/google_sheets.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      458 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/k8s.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8993 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/mongodb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2596 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/parameters.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9035 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5519 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/salesforce.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3528 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/save.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      466 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/spark.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13374 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/sql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      738 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/validation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3846 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/schedule.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.504865 aqueduct-sdk-0.3.3/aqueduct/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      451 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/connect_config_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19133 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/dag_delta_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4058 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/dag_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3040 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/decorator_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3811 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/decorators_with_without_parentheses_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      218 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/enum_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1094 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/flow_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1398 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/helpers_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4498 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/metric_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      488 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/naming_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15641 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/serialization_test.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.504865 aqueduct-sdk-0.3.3/aqueduct/tests/test_files/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/test_files/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.504865 aqueduct-sdk-0.3.3/aqueduct/tests/test_files/python_function/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/test_files/python_function/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/test_files/python_function/python_function.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.504865 aqueduct-sdk-0.3.3/aqueduct/tests/test_files/python_function/test_dependency_folder/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/test_files/python_function/test_dependency_folder/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/test_files/python_function/test_dependency_folder/helper_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6071 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/type_annotations.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.508865 aqueduct-sdk-0.3.3/aqueduct/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10726 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/dag_deltas.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1271 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/describe.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/format.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11492 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/function_packaging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1446 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/integration_validation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1706 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/local_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1234 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/naming.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16574 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/serialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2148 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/type_inference.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8505 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.508865 aqueduct-sdk-0.3.3/aqueduct_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7716 2023-05-17 16:03:38.000000 aqueduct-sdk-0.3.3/aqueduct_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3124 2023-05-17 16:03:38.000000 aqueduct-sdk-0.3.3/aqueduct_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-17 16:03:38.000000 aqueduct-sdk-0.3.3/aqueduct_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-05-17 16:03:38.000000 aqueduct-sdk-0.3.3/aqueduct_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-17 16:03:38.000000 aqueduct-sdk-0.3.3/aqueduct_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.508865 aqueduct-sdk-0.3.3/requirements/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/requirements/python-3-10.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/requirements/python-3-7.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/requirements/python-3-8.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/requirements/python-3-9.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-17 16:03:38.508865 aqueduct-sdk-0.3.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1197 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-17 01:51:34.000000 aqueduct-sdk-0.3.3/version
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.921607 aqueduct-sdk-0.3.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7716 2023-05-24 22:48:10.921607 aqueduct-sdk-0.3.4/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.905607 aqueduct-sdk-0.3.4/aqueduct/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1530 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.909607 aqueduct-sdk-0.3.4/aqueduct/artifacts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/_create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1815 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/base_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4188 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/bool_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3729 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4688 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/generic_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11713 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/numeric_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6599 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/preview.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4124 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/system_metric.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24895 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/artifacts/table_artifact.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.909607 aqueduct-sdk-0.3.4/aqueduct/backend/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/backend/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24525 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/backend/api_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6091 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/backend/response_helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    39473 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.909607 aqueduct-sdk-0.3.4/aqueduct/constants/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/constants/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6626 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/constants/enums.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/constants/exports.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/constants/metrics.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    52868 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/decorator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3930 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/error.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5525 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/flow.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7295 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/flow_run.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8260 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/github.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.909607 aqueduct-sdk-0.3.4/aqueduct/globals/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      200 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/globals/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/globals/api_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      477 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/globals/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      192 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/globals/dag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8506 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/llm_wrapper.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/logger.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.913607 aqueduct-sdk-0.3.4/aqueduct/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      574 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/models/artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/models/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21114 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/models/dag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/models/dag_rules.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      554 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/models/execution_state.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3061 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/models/integration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7786 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/models/operators.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13906 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/models/response_models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      176 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/models/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.913607 aqueduct-sdk-0.3.4/aqueduct/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      285 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      474 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/airflow.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      624 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/aws.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      464 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/aws_lambda.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13077 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/connect_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      486 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/databricks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7518 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/dynamic_k8s.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1789 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/ecr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4878 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/google_sheets.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      458 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/k8s.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8993 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/mongodb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4866 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/parameters.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9364 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5519 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/salesforce.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3528 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/save.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      466 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/spark.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13323 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/sql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      738 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/resources/validation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3846 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/schedule.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.917607 aqueduct-sdk-0.3.4/aqueduct/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      451 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/connect_config_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19133 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/dag_delta_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4058 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/tests/dag_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3040 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/decorator_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3811 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/decorators_with_without_parentheses_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      218 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/enum_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      909 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/flow_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1398 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/helpers_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4498 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/tests/metric_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      488 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/naming_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15641 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/serialization_test.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.917607 aqueduct-sdk-0.3.4/aqueduct/tests/test_files/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/tests/test_files/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.917607 aqueduct-sdk-0.3.4/aqueduct/tests/test_files/python_function/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/tests/test_files/python_function/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/tests/test_files/python_function/python_function.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.917607 aqueduct-sdk-0.3.4/aqueduct/tests/test_files/python_function/test_dependency_folder/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/tests/test_files/python_function/test_dependency_folder/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/tests/test_files/python_function/test_dependency_folder/helper_function.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6071 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/tests/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/type_annotations.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.921607 aqueduct-sdk-0.3.4/aqueduct/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10726 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/utils/dag_deltas.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1271 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.4/aqueduct/utils/describe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/utils/format.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11492 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/utils/function_packaging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1446 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/utils/integration_validation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1706 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/utils/local_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1234 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/utils/naming.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16574 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/utils/serialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2148 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/utils/type_inference.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8220 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/aqueduct/utils/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.921607 aqueduct-sdk-0.3.4/aqueduct_sdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7716 2023-05-24 22:48:10.000000 aqueduct-sdk-0.3.4/aqueduct_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3124 2023-05-24 22:48:10.000000 aqueduct-sdk-0.3.4/aqueduct_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-24 22:48:10.000000 aqueduct-sdk-0.3.4/aqueduct_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-05-24 22:48:10.000000 aqueduct-sdk-0.3.4/aqueduct_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-24 22:48:10.000000 aqueduct-sdk-0.3.4/aqueduct_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 22:48:10.921607 aqueduct-sdk-0.3.4/requirements/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/requirements/python-3-10.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/requirements/python-3-7.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/requirements/python-3-8.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/requirements/python-3-9.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-24 22:48:10.921607 aqueduct-sdk-0.3.4/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1197 2023-05-24 04:24:42.000000 aqueduct-sdk-0.3.4/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-24 22:27:12.000000 aqueduct-sdk-0.3.4/version
```

### Comparing `aqueduct-sdk-0.3.3/PKG-INFO` & `aqueduct-sdk-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-sdk
-Version: 0.3.3
+Version: 0.3.4
 Summary: Python SDK for Aqueduct
 Home-page: https://github.com/aqueducthq/aqueduct
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `aqueduct-sdk-0.3.3/aqueduct/__init__.py` & `aqueduct-sdk-0.3.4/aqueduct/__init__.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/artifacts/_create.py` & `aqueduct-sdk-0.3.4/aqueduct/artifacts/_create.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/artifacts/base_artifact.py` & `aqueduct-sdk-0.3.4/aqueduct/artifacts/base_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/artifacts/bool_artifact.py` & `aqueduct-sdk-0.3.4/aqueduct/artifacts/bool_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/artifacts/create.py` & `aqueduct-sdk-0.3.4/aqueduct/artifacts/create.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/artifacts/generic_artifact.py` & `aqueduct-sdk-0.3.4/aqueduct/artifacts/generic_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/artifacts/numeric_artifact.py` & `aqueduct-sdk-0.3.4/aqueduct/artifacts/numeric_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/artifacts/preview.py` & `aqueduct-sdk-0.3.4/aqueduct/artifacts/preview.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/artifacts/system_metric.py` & `aqueduct-sdk-0.3.4/aqueduct/artifacts/system_metric.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/artifacts/table_artifact.py` & `aqueduct-sdk-0.3.4/aqueduct/artifacts/table_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/backend/api_client.py` & `aqueduct-sdk-0.3.4/aqueduct/backend/api_client.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/backend/response_helpers.py` & `aqueduct-sdk-0.3.4/aqueduct/backend/response_helpers.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/client.py` & `aqueduct-sdk-0.3.4/aqueduct/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import os
 import platform
+import re
 import uuid
 import warnings
 from collections import defaultdict
-from typing import Any, DefaultDict, Dict, List, Optional, Union
+from typing import Any, DefaultDict, Dict, List, Optional, Tuple, Union
 
 import __main__ as main
 import yaml
 from aqueduct.artifacts.base_artifact import BaseArtifact
 from aqueduct.artifacts.bool_artifact import BoolArtifact
 from aqueduct.artifacts.create import create_param_artifact
 from aqueduct.artifacts.numeric_artifact import NumericArtifact
@@ -25,15 +26,15 @@
     InvalidUserArgumentException,
 )
 from aqueduct.flow import Flow
 from aqueduct.github import Github
 from aqueduct.logger import logger
 from aqueduct.models.dag import Metadata, RetentionPolicy
 from aqueduct.models.integration import BaseResource, ResourceInfo
-from aqueduct.models.operators import ParamSpec
+from aqueduct.models.operators import ParamSpec, S3LoadParams
 from aqueduct.models.response_models import SavedObjectUpdate
 from aqueduct.resources.airflow import AirflowResource
 from aqueduct.resources.aws import AWSResource
 from aqueduct.resources.aws_lambda import LambdaResource
 from aqueduct.resources.connect_config import (
     BaseConnectionConfig,
     ResourceConfig,
@@ -42,14 +43,15 @@
 )
 from aqueduct.resources.databricks import DatabricksResource
 from aqueduct.resources.dynamic_k8s import DynamicK8sResource
 from aqueduct.resources.ecr import ECRResource
 from aqueduct.resources.google_sheets import GoogleSheetsResource
 from aqueduct.resources.k8s import K8sResource
 from aqueduct.resources.mongodb import MongoDBResource
+from aqueduct.resources.parameters import USER_TAG_PATTERN
 from aqueduct.resources.s3 import S3Resource
 from aqueduct.resources.salesforce import SalesforceResource
 from aqueduct.resources.spark import SparkResource
 from aqueduct.resources.sql import RelationalDBResource
 from aqueduct.utils.dag_deltas import (
     SubgraphDAGDelta,
     apply_deltas_to_dag,
@@ -487,40 +489,55 @@
         return [
             workflow_resp.to_readable_dict()
             for workflow_resp in globals.__GLOBAL_API_CLIENT__.list_workflows()
         ]
 
     def flow(
         self,
+        flow_identifier: Optional[Union[str, uuid.UUID]] = None,
         flow_id: Optional[Union[str, uuid.UUID]] = None,
         flow_name: Optional[str] = None,
     ) -> Flow:
         """Fetches a flow corresponding to the given flow id.
 
         Args:
+            flow_identifier:
+                Used to identify the flow to fetch from the system.
+                Use either the flow name or id as identifier to fetch
+                from the system.
             flow_id:
                 Used to identify the flow to fetch from the system.
                 Between `flow_id` and `flow_name`, at least one must be provided.
                 If both are specified, they must correspond to the same flow.
             flow_name:
                 Used to identify the flow to fetch from the system.
 
+            flow_identifier takes precedence over flow_id or flow_name arguments
+
         Raises:
             InvalidUserArgumentException:
                 If the provided flow id or name does not correspond to a flow the client knows about.
         """
-        flows = [(flow.id, flow.name) for flow in globals.__GLOBAL_API_CLIENT__.list_workflows()]
-        flow_id = find_flow_with_user_supplied_id_and_name(
-            flows,
-            flow_id,
-            flow_name,
-        )
+        # TODO(ENG-3013): Completely remove these optional parameters.
+        if flow_id or flow_name:
+            warnings.warn(
+                "flow_id and flow_name arguments will be deprecated. Please use flow_identifier.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+            if not flow_identifier:
+                if flow_id:
+                    flow_identifier = flow_id
+                elif flow_name:
+                    flow_identifier = flow_name
 
+        flows = [(flow.id, flow.name) for flow in globals.__GLOBAL_API_CLIENT__.list_workflows()]
+        flow_id_key = find_flow_with_user_supplied_id_and_name(flows, flow_identifier)
         return Flow(
-            flow_id,
+            flow_id_key,
             self._in_notebook_or_console_context,
         )
 
     def publish_flow(
         self,
         name: str,
         description: str = "",
@@ -770,43 +787,59 @@
         return Flow(
             str(flow_id),
             self._in_notebook_or_console_context,
         )
 
     def trigger(
         self,
+        flow_identifier: Optional[Union[str, uuid.UUID]] = None,
+        parameters: Optional[Dict[str, Any]] = None,
         flow_id: Optional[Union[str, uuid.UUID]] = None,
         flow_name: Optional[str] = None,
-        parameters: Optional[Dict[str, Any]] = None,
     ) -> None:
         """Immediately triggers another run of the provided flow.
 
         Args:
-            flow_id:
-                The id of the flow to delete.
-                Between `flow_id` and `flow_name`, at least one must be provided.
-                If both are specified, they must correspond to the same flow.
-            flow_name:
-                The name of the flow to delete.
+            flow_identifier:
+                The uuid or name of the flow to delete.
             parameters:
                 A map containing custom values to use for the designated parameters. The mapping
                 is expected to be from parameter name to the custom value. These custom values
                 are not persisted to the workflow. To actually change the default parameter values
                 edit the workflow itself through `client.publish_flow()`.
+            flow_id:
+                Used to identify the flow to fetch from the system.
+                Between `flow_id` and `flow_name`, at least one must be provided.
+                If both are specified, they must correspond to the same flow.
+            flow_name:
+                Used to identify the flow to fetch from the system.
 
+            flow_identifier takes precedence over flow_id or flow_name arguments
         Raises:
             InvalidRequestError:
                 An error occurred when attempting to fetch the workflow to
                 delete. The provided `flow_id` may be malformed.
             InternalServerError:
                 An unexpected error occurred within the Aqueduct cluster.
         """
+        # TODO(ENG-3013): Completely remove these optional parameters.
+        if flow_id or flow_name:
+            warnings.warn(
+                "flow_id and flow_name arguments will be deprecated. Please use flow_identifier.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+            if not flow_identifier:
+                if flow_id:
+                    flow_identifier = flow_id
+                elif flow_name:
+                    flow_identifier = flow_name
         param_specs: Dict[str, ParamSpec] = {}
         if parameters is not None:
-            flow = self.flow(flow_id)
+            flow = self.flow(flow_identifier)
             latest_run = flow.latest()
 
             # NOTE: this is a defense check against triggering runs that haven't run yet.
             # We may want to revisit this in the future if more nuanced constraints are necessary.
             if not latest_run:
                 raise InvalidUserActionException(
                     "Cannot trigger a workflow that hasn't already run at least once."
@@ -814,65 +847,100 @@
             validate_overwriting_parameters(latest_run._dag, parameters)
 
             for name, new_val in parameters.items():
                 artifact_type = infer_artifact_type(new_val)
                 param_specs[name] = construct_param_spec(new_val, artifact_type)
 
         flows = [(flow.id, flow.name) for flow in globals.__GLOBAL_API_CLIENT__.list_workflows()]
-        flow_id = find_flow_with_user_supplied_id_and_name(
-            flows,
-            flow_id,
-            flow_name,
-        )
-        globals.__GLOBAL_API_CLIENT__.refresh_workflow(flow_id, param_specs)
+        flow_id_key = find_flow_with_user_supplied_id_and_name(flows, flow_identifier)
+        globals.__GLOBAL_API_CLIENT__.refresh_workflow(flow_id_key, param_specs)
 
     def delete_flow(
         self,
+        flow_identifier: Optional[Union[str, uuid.UUID]] = None,
         flow_id: Optional[Union[str, uuid.UUID]] = None,
         flow_name: Optional[str] = None,
         saved_objects_to_delete: Optional[
             DefaultDict[Union[str, BaseResource], List[SavedObjectUpdate]]
         ] = None,
         force: bool = False,
     ) -> None:
         """Deletes a flow object.
 
         Args:
+            flow_identifier:
+                The id of the flow to delete. Must be name or uuid
             flow_id:
-                The id of the flow to delete.
+                Used to identify the flow to fetch from the system.
                 Between `flow_id` and `flow_name`, at least one must be provided.
                 If both are specified, they must correspond to the same flow.
             flow_name:
-                The name of the flow to delete.
+                Used to identify the flow to fetch from the system.
+
+            flow_identifier takes precedence over flow_id or flow_name arguments
+
             saved_objects_to_delete:
                 The tables or storage paths to delete grouped by integration name.
             force:
                 Force the deletion even though some workflow-written objects in the writes_to_delete argument had UpdateMode=append
 
         Raises:
             InvalidRequestError:
                 An error occurred when attempting to fetch the workflow to
                 delete. The provided `flow_id` may be malformed.
             InternalServerError:
                 An unexpected error occurred within the Aqueduct cluster.
         """
+        # TODO(ENG-3013): Completely remove these optional parameters.
+        if flow_id or flow_name:
+            warnings.warn(
+                "flow_id and flow_name arguments will be deprecated. Please use flow_identifier.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+            if not flow_identifier:
+                if flow_id:
+                    flow_identifier = flow_id
+                elif flow_name:
+                    flow_identifier = flow_name
+
         if saved_objects_to_delete is None:
             saved_objects_to_delete = defaultdict()
 
+        # TODO(ENG-3015): Until parameterized S3 filepath deletion is fixed, we prevent users from
+        #  deleting those objects.
+        s3_parameterized_filepaths: List[Tuple[str, str]] = []
+        for saved_obj_list in saved_objects_to_delete.values():
+            for saved_obj_to_delete in saved_obj_list:
+                if isinstance(saved_obj_to_delete.spec.parameters, S3LoadParams):
+                    filepath = saved_obj_to_delete.spec.parameters.filepath
+                    if len(re.findall(USER_TAG_PATTERN, filepath)) > 0:
+                        s3_parameterized_filepaths.append(
+                            (saved_obj_to_delete.integration_name, filepath)
+                        )
+
+        if len(s3_parameterized_filepaths) > 0:
+            raise InvalidUserArgumentException(
+                "Deleting objects at parameterized filepaths in S3 is currently unsupported. The following resource-filepath "
+                "combinations in `saved_objects_to_delete` are parameterized: \n"
+                + ", ".join(
+                    [
+                        f"{integration_name}: {filepath}"
+                        for integration_name, filepath in s3_parameterized_filepaths
+                    ]
+                )
+            )
+
         flows = [(flow.id, flow.name) for flow in globals.__GLOBAL_API_CLIENT__.list_workflows()]
-        flow_id = find_flow_with_user_supplied_id_and_name(
-            flows,
-            flow_id,
-            flow_name,
-        )
+        flow_id_key = find_flow_with_user_supplied_id_and_name(flows, flow_identifier)
 
         # TODO(ENG-410): This method gives no indication as to whether the flow
         #  was successfully deleted.
         resp = globals.__GLOBAL_API_CLIENT__.delete_workflow(
-            flow_id, saved_objects_to_delete, force
+            flow_id_key, saved_objects_to_delete, force
         )
 
         failures = []
         for integration in resp.saved_object_deletion_results:
             for obj in resp.saved_object_deletion_results[integration]:
                 if obj.exec_state.status == ExecutionStatus.FAILED:
                     trace = ""
```

### Comparing `aqueduct-sdk-0.3.3/aqueduct/constants/enums.py` & `aqueduct-sdk-0.3.4/aqueduct/constants/enums.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/decorator.py` & `aqueduct-sdk-0.3.4/aqueduct/decorator.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/error.py` & `aqueduct-sdk-0.3.4/aqueduct/error.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/flow.py` & `aqueduct-sdk-0.3.4/aqueduct/flow.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/flow_run.py` & `aqueduct-sdk-0.3.4/aqueduct/flow_run.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/github.py` & `aqueduct-sdk-0.3.4/aqueduct/github.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/llm_wrapper.py` & `aqueduct-sdk-0.3.4/aqueduct/llm_wrapper.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/models/artifact.py` & `aqueduct-sdk-0.3.4/aqueduct/models/artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/models/config.py` & `aqueduct-sdk-0.3.4/aqueduct/models/config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/models/dag.py` & `aqueduct-sdk-0.3.4/aqueduct/models/dag.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 import uuid
+from collections import OrderedDict
 from typing import Any, Callable, Dict, List, Optional, Set
 
 from aqueduct.constants.enums import (
     ArtifactType,
     OperatorType,
     RuntimeType,
     SparkRuntimeType,
@@ -43,15 +44,21 @@
     name: Optional[str]
     description: Optional[str]
     schedule: Optional[Schedule]
     retention_policy: Optional[RetentionPolicy]
 
 
 class DAG(BaseModel):
-    operators: Dict[str, Operator] = {}
+    # We use an OrderedDict here to preserve insertion order of operators. This is helpful
+    # any case where we have multiple choices, but can resolve the ambiguity by picking the
+    # latest added, for example. This is relevant for parameter string interpolation.
+    #
+    # Although as of Python3.7, a regular python dict also preserves insertion order, we use an
+    # OrderedDict as future-proofing against any expansion of Aqueduct to Python<=3.7.
+    operators: Dict[str, Operator] = OrderedDict()
     artifacts: Dict[str, ArtifactMetadata] = {}
 
     # The field must be set when publishing the workflow.
     metadata: Metadata
 
     # Represents the default engine the DAG will be executed on. Can be overwritten
     # by individual operators.
@@ -340,15 +347,14 @@
     def must_get_artifacts(self, artifact_ids: List[uuid.UUID]) -> List[ArtifactMetadata]:
         return [self.must_get_artifact(artifact_id) for artifact_id in artifact_ids]
 
     def get_artifact_by_name(self, name: str) -> Optional[ArtifactMetadata]:
         for artifact in self.list_artifacts():
             if artifact.name == name:
                 return artifact
-
         return None
 
     def list_artifacts(
         self,
         on_op_ids: Optional[List[uuid.UUID]] = None,
         filter_to: Optional[List[ArtifactType]] = None,
     ) -> List[ArtifactMetadata]:
@@ -392,18 +398,44 @@
                     filter_to=[OperatorType.CHECK],
                     on_artifact_id=artf,
                 )
             )
         return check_operators
 
     def get_param_op_by_name(self, name: str) -> Optional[Operator]:
+        """Use this in the case where multiple parameters with the same name are not allowed.
+
+        This uniqueness is guaranteed after sanitizing the names with `validate_and_resolve_artifact_names()`,
+        typically for preview or publish.
+        """
+        found_op: Optional[Operator] = None
         for op in self.operators.values():
             if op.name == name and get_operator_type(op) == OperatorType.PARAM:
-                return op
-        return None
+                if found_op is not None:
+                    raise InternalAqueductError(
+                        "Unexpectedly found multiple parameters with the same name: %s" % name
+                    )
+                found_op = op
+
+        return found_op
+
+    def get_param_ops_by_name(self, name: str) -> List[Operator]:
+        """Use this in the case where multiple parameters with the same name are allowed.
+
+        This typically happens when the DAG is not ready to preview/publish, but we need to fetch
+        parameters by name, for situations like string interpolation with "{param_name}".
+
+        The returned operators are ordered in descending insertion order, with the latest-added
+        operator first.
+        """
+        found_ops: List[Operator] = []
+        for op in reversed(list(self.operators.values())):
+            if op.name == name and get_operator_type(op) == OperatorType.PARAM:
+                found_ops.append(op)
+        return found_ops
 
     ######################## DAG WRITES #############################
 
     def add_operator(self, op: Operator) -> None:
         self.add_operators([op])
 
     def add_operators(self, ops: List[Operator]) -> None:
```

### Comparing `aqueduct-sdk-0.3.3/aqueduct/models/dag_rules.py` & `aqueduct-sdk-0.3.4/aqueduct/models/dag_rules.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/models/execution_state.py` & `aqueduct-sdk-0.3.4/aqueduct/models/execution_state.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/models/integration.py` & `aqueduct-sdk-0.3.4/aqueduct/models/integration.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/models/operators.py` & `aqueduct-sdk-0.3.4/aqueduct/models/operators.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/models/response_models.py` & `aqueduct-sdk-0.3.4/aqueduct/models/response_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,40 @@
 from aqueduct.constants.enums import (
     ArtifactType,
     ExecutionStatus,
     K8sClusterStatusType,
     SerializationType,
 )
 from aqueduct.models.artifact import ArtifactMetadata
-from aqueduct.models.dag import Metadata, RetentionPolicy, Schedule
+from aqueduct.models.dag import EngineConfig, Metadata, RetentionPolicy, Schedule
 from aqueduct.models.execution_state import ExecutionState
 from aqueduct.models.operators import LoadSpec, Operator, OperatorSpec
 from aqueduct.models.utils import human_readable_timestamp
 from pydantic import BaseModel
 
 
 class ArtifactResult(BaseModel):
     serialization_type: SerializationType
     artifact_type: ArtifactType
     content: bytes
 
 
 # V2 Responses
+class GetDagResponse(BaseModel):
+    id: uuid.UUID
+    workflow_id: uuid.UUID
+    created_at: str
+    engine_config: EngineConfig
+
+
+class GetNodeResultContentResponse(BaseModel):
+    is_downsampled: bool
+    content: str
+
+
 class GetDagResultResponse(BaseModel):
     """Represents the result of a single workflow run.
 
     Attributes:
         id:
             The id of the workflow run. This is the same id users can use to fetch
             FlowRuns.
@@ -135,14 +147,50 @@
     name: str
     description: str
     type: ArtifactType
     input: uuid.UUID
     outputs: List[uuid.UUID]
 
 
+class GetOperatorWithArtifactNodeResponse(BaseModel):
+    """Represents a single merged node (metric or check) in a workflow run.
+
+    Attributes:
+        id:
+            The id of the operator node.
+        artifact_id:
+            The id of the artifact node.
+        dag_id:
+            This id can be used to find the corresponding workflow dag version.
+        name:
+            The name of the operator.
+        description:
+            The description of the operator.
+        type:
+            The artifact type.
+        spec:
+            The operator spec.
+        inputs:
+            The id(s) of the input artifact(s) of the operator.
+        outputs:
+            The id(s) of the operator(s) that take this artifact as input.
+
+    """
+
+    id: uuid.UUID
+    dag_id: uuid.UUID
+    artifact_id: uuid.UUID
+    name: str
+    description: str
+    spec: OperatorSpec
+    type: ArtifactType
+    inputs: List[uuid.UUID]
+    outputs: List[uuid.UUID]
+
+
 # V1 Responses
 class PreviewResponse(BaseModel):
     """This is the response object returned by api_client.preview().
 
     Attributes:
         status:
             The execution state of preview.
```

### Comparing `aqueduct-sdk-0.3.3/aqueduct/resources/aws.py` & `aqueduct-sdk-0.3.4/aqueduct/resources/aws.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/resources/connect_config.py` & `aqueduct-sdk-0.3.4/aqueduct/resources/connect_config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/resources/dynamic_k8s.py` & `aqueduct-sdk-0.3.4/aqueduct/resources/dynamic_k8s.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/resources/ecr.py` & `aqueduct-sdk-0.3.4/aqueduct/resources/ecr.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/resources/google_sheets.py` & `aqueduct-sdk-0.3.4/aqueduct/resources/google_sheets.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/resources/mongodb.py` & `aqueduct-sdk-0.3.4/aqueduct/resources/mongodb.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/resources/s3.py` & `aqueduct-sdk-0.3.4/aqueduct/resources/s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from aqueduct.utils.utils import generate_uuid
 
 from aqueduct import globals
 
 from ..artifacts.create import to_artifact_class
 from ..error import InvalidUserArgumentException
 from ..utils.naming import default_artifact_name_from_op_name, sanitize_artifact_name
+from .parameters import _fetch_param_artifact_ids_embedded_in_string
 from .save import _save_artifact
 
 
 def _convert_to_s3_table_format(format: Optional[str]) -> Optional[S3TableFormat]:
     """A simple string -> enum conversion. Returns None if no format provided."""
     if format is None:
         return None
@@ -196,16 +197,22 @@
             and format is not None
         ):
             raise InvalidUserArgumentException(
                 "A `format` argument should only be supplied for saving table artifacts. This artifact type is %s."
                 % artifact.type()
             )
 
+        # Prepend any parameters embedded in the filepath.
+        param_artifact_ids_in_filepath = _fetch_param_artifact_ids_embedded_in_string(
+            self._dag, filepath
+        )
+        artifact_ids = param_artifact_ids_in_filepath + [artifact.id()]
+
         _save_artifact(
-            artifact.id(),
+            artifact_ids,
             self._dag,
             self._metadata,
             save_params=S3LoadParams(filepath=filepath, format=_convert_to_s3_table_format(format)),
         )
 
     def describe(self) -> None:
         """Prints out a human-readable description of the S3 integration."""
```

### Comparing `aqueduct-sdk-0.3.3/aqueduct/resources/salesforce.py` & `aqueduct-sdk-0.3.4/aqueduct/resources/salesforce.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/resources/save.py` & `aqueduct-sdk-0.3.4/aqueduct/resources/save.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/resources/sql.py` & `aqueduct-sdk-0.3.4/aqueduct/resources/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 from aqueduct.models.operators import (
     ExtractSpec,
     Operator,
     OperatorSpec,
     RelationalDBExtractParams,
     RelationalDBLoadParams,
 )
-from aqueduct.resources.parameters import _validate_builtin_expansions, _validate_parameters
+from aqueduct.resources.parameters import (
+    _validate_artifact_is_string,
+    _validate_builtin_expansions,
+    _validate_parameters,
+)
 from aqueduct.resources.save import _save_artifact
 from aqueduct.resources.validation import validate_is_connected
 from aqueduct.utils.dag_deltas import AddOperatorDelta, apply_deltas_to_dag
 from aqueduct.utils.naming import default_artifact_name_from_op_name, sanitize_artifact_name
 from aqueduct.utils.utils import generate_uuid
 
 from aqueduct import globals
@@ -262,38 +266,36 @@
             )
 
         if not isinstance(table_name, str) and not isinstance(table_name, BaseArtifact):
             raise InvalidUserArgumentException(
                 "`table_name` must either be a string or a string parameter artifact."
             )
 
+        # Non-tabular data cannot be saved into relational data stores.
+        if artifact.type() not in [ArtifactType.UNTYPED, ArtifactType.TABLE]:
+            raise InvalidUserActionException(
+                "Unable to save non-relational data into relational data store `%s`." % self.name()
+            )
+
+        # Resolve the table name if it is parameterized.
         table_name_str = table_name
         artifact_ids = [artifact.id()]
         if isinstance(table_name, BaseArtifact):
             table_name_artifact = table_name
-            if table_name_artifact.type() != ArtifactType.STRING:
-                raise InvalidUserArgumentException(
-                    "A parameter value for `table_name` must be of string type."
-                )
+            _validate_artifact_is_string(table_name_artifact)
 
             # This is unset in the LoadParams, since we're parameterizing it.
             table_name_str = ""
 
             # Assumption: All parameter artifacts are prepended to the operator's input list.
             artifact_ids = [table_name_artifact.id()] + artifact_ids
         else:
             if table_name_str == "":
                 raise InvalidUserArgumentException("Cannot save to an empty table name.")
 
-        # Non-tabular data cannot be saved into relational data stores.
-        if artifact.type() not in [ArtifactType.UNTYPED, ArtifactType.TABLE]:
-            raise InvalidUserActionException(
-                "Unable to save non-relational data into relational data store `%s`." % self.name()
-            )
-
         _save_artifact(
             artifact_ids,
             self._dag,
             self._metadata,
             save_params=RelationalDBLoadParams(table=table_name_str, update_mode=update_mode),
         )
```

### Comparing `aqueduct-sdk-0.3.3/aqueduct/resources/validation.py` & `aqueduct-sdk-0.3.4/aqueduct/resources/validation.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/schedule.py` & `aqueduct-sdk-0.3.4/aqueduct/schedule.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/tests/dag_delta_test.py` & `aqueduct-sdk-0.3.4/aqueduct/tests/dag_delta_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/tests/dag_test.py` & `aqueduct-sdk-0.3.4/aqueduct/tests/dag_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/tests/decorator_test.py` & `aqueduct-sdk-0.3.4/aqueduct/tests/decorator_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/tests/decorators_with_without_parentheses_test.py` & `aqueduct-sdk-0.3.4/aqueduct/tests/decorators_with_without_parentheses_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/tests/flow_test.py` & `aqueduct-sdk-0.3.4/aqueduct/tests/flow_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,30 +3,24 @@
 
 import pytest
 from aqueduct.error import InvalidUserArgumentException
 from aqueduct.utils.utils import find_flow_with_user_supplied_id_and_name
 
 
 def test_find_flow_with_user_supplied_id_and_name():
-    flow_1_id = "9740eb10-d77d-4393-a9bc-42862d7008e0"
-    flow_2_id = "6d9d7b93-028f-48b1-b723-ebd9e66ac867"
-    flow_3_id = "431841d6-aac5-450f-b395-66e110ba547b"
+    flow_1_id = uuid.UUID("9740eb10-d77d-4393-a9bc-42862d7008e0")
+    flow_2_id = uuid.UUID("6d9d7b93-028f-48b1-b723-ebd9e66ac867")
+    flow_3_id = uuid.UUID("431841d6-aac5-450f-b395-66e110ba547b")
 
     flows = [
-        (uuid.UUID(flow_1_id), "flow_1"),
-        (uuid.UUID(flow_2_id), "flow_2"),
-        (uuid.UUID(flow_3_id), "flow_3"),
+        (flow_1_id, "flow_1"),
+        (flow_2_id, "flow_2"),
     ]
 
-    flow_id = find_flow_with_user_supplied_id_and_name(flows, flow_id=flow_1_id)
-    assert flow_id == flow_1_id
+    flow_id = find_flow_with_user_supplied_id_and_name(flows, flow_identifier=flow_1_id)
+    assert flow_id == str(flow_1_id)
 
-    flow_id = find_flow_with_user_supplied_id_and_name(flows, flow_name="flow_1")
-    assert flow_id == flow_1_id
-
-    flow_id = find_flow_with_user_supplied_id_and_name(flows, flow_id=flow_1_id, flow_name="flow_1")
-    assert flow_id == flow_1_id
+    flow_id = find_flow_with_user_supplied_id_and_name(flows, flow_identifier="flow_2")
+    assert flow_id == str(flow_2_id)
 
     with pytest.raises(InvalidUserArgumentException):
-        flow_id = find_flow_with_user_supplied_id_and_name(
-            flows, flow_id=flow_1_id, flow_name="flow_2"
-        )
+        find_flow_with_user_supplied_id_and_name(flows, flow_identifier=flow_3_id)
```

### Comparing `aqueduct-sdk-0.3.3/aqueduct/tests/helpers_test.py` & `aqueduct-sdk-0.3.4/aqueduct/tests/helpers_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/tests/metric_test.py` & `aqueduct-sdk-0.3.4/aqueduct/tests/metric_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/tests/serialization_test.py` & `aqueduct-sdk-0.3.4/aqueduct/tests/serialization_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/tests/utils.py` & `aqueduct-sdk-0.3.4/aqueduct/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/utils/dag_deltas.py` & `aqueduct-sdk-0.3.4/aqueduct/utils/dag_deltas.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/utils/describe.py` & `aqueduct-sdk-0.3.4/aqueduct/utils/describe.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/utils/function_packaging.py` & `aqueduct-sdk-0.3.4/aqueduct/utils/function_packaging.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/utils/integration_validation.py` & `aqueduct-sdk-0.3.4/aqueduct/utils/integration_validation.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/utils/local_data.py` & `aqueduct-sdk-0.3.4/aqueduct/utils/local_data.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/utils/naming.py` & `aqueduct-sdk-0.3.4/aqueduct/utils/naming.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/utils/serialization.py` & `aqueduct-sdk-0.3.4/aqueduct/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/utils/type_inference.py` & `aqueduct-sdk-0.3.4/aqueduct/utils/type_inference.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/aqueduct/utils/utils.py` & `aqueduct-sdk-0.3.4/aqueduct/utils/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -209,47 +209,35 @@
             ),
         )
     else:
         raise AqueductError("Unsupported engine configuration.")
 
 
 def find_flow_with_user_supplied_id_and_name(
-    flows: List[Tuple[uuid.UUID, str]],
-    flow_id: Optional[Union[str, uuid.UUID]] = None,
-    flow_name: Optional[str] = None,
+    flows: List[Tuple[uuid.UUID, str]], flow_identifier: Optional[Union[str, uuid.UUID]] = None
 ) -> str:
-    """Verifies that the user supplied flow id and name correspond
-    to an actual flow in `flows`. Only one of `flow_id` and `flow_name` is necessary,
-    but if both are provided, they must match to the same flow. It returns the
-    string version of the matching flow's id.
+    """Verifies that the user supplied flow_identifier correspond
+    to an actual flow in `flows`. Must be either uuid or name that
+    must match to the same flow. It returns the string version of
+    the matching flow's id.
     """
-    if not flow_id and not flow_name:
+    if not flow_identifier:
         raise InvalidUserArgumentException(
-            "Must supply at least one of the following:`flow_id` or `flow_name`"
+            "Must supply a valid flow identifier, either name or uuid"
         )
 
-    if flow_id:
-        flow_id_str = parse_user_supplied_id(flow_id)
-        if all(uuid.UUID(flow_id_str) != flow[0] for flow in flows):
-            raise InvalidUserArgumentException("Unable to find a flow with id %s" % flow_id)
+    flow_id_str = parse_user_supplied_id(flow_identifier)
 
-    if flow_name:
-        flow_id_str_from_name = None
+    if isinstance(flow_identifier, uuid.UUID) or is_string_valid_uuid(flow_identifier):
+        if all(uuid.UUID(flow_id_str) != flow[0] for flow in flows):
+            raise InvalidUserArgumentException("Unable to find a flow with id %s" % flow_identifier)
+    elif isinstance(flow_identifier, str):
+        if all(flow_id_str != flow[1] for flow in flows):
+            raise InvalidUserArgumentException("Unable to find a flow with name %s" % flow_id_str)
+        # You land here if found matching flow name, return corresponding uuid
+        # backend api's look for uuid instead of name
         for flow in flows:
-            if flow[1] == flow_name:
-                flow_id_str_from_name = str(flow[0])
+            if flow_id_str == flow[1]:
+                flow_id_str = str(flow[0])
                 break
 
-        if not flow_id_str_from_name:
-            raise InvalidUserArgumentException("Unable to find a flow with name %s" % flow_name)
-
-        if flow_id and flow_id_str != flow_id_str_from_name:
-            # User supplied both flow_id and flow_name, but they do not
-            # correspond to the same flow
-            raise InvalidUserArgumentException(
-                "The flow with id %s does not correspond to the flow with name %s"
-                % (flow_id, flow_name)
-            )
-
-        return flow_id_str_from_name
-
     return flow_id_str
```

### Comparing `aqueduct-sdk-0.3.3/aqueduct_sdk.egg-info/PKG-INFO` & `aqueduct-sdk-0.3.4/aqueduct_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-sdk
-Version: 0.3.3
+Version: 0.3.4
 Summary: Python SDK for Aqueduct
 Home-page: https://github.com/aqueducthq/aqueduct
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `aqueduct-sdk-0.3.3/aqueduct_sdk.egg-info/SOURCES.txt` & `aqueduct-sdk-0.3.4/aqueduct_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.3/setup.py` & `aqueduct-sdk-0.3.4/setup.py`

 * *Files identical despite different names*

