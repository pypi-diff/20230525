# Comparing `tmp/astro-sdk-python-1.7.0a1.tar.gz` & `tmp/astro-sdk-python-1.7.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-sdk-python-1.7.0a1.tar", last modified: Fri May  5 14:23:20 2023, max compression
+gzip compressed data, was "astro-sdk-python-1.7.0a2.tar", last modified: Fri May  5 23:38:53 2023, max compression
```

## Comparing `astro-sdk-python-1.7.0a1.tar` & `astro-sdk-python-1.7.0a2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-lrwxr-xr-x   0        0        0        0 2023-05-05 14:23:07.796431 astro-sdk-python-1.7.0a1/LICENSE -> ../LICENSE
--rw-r--r--   0        0        0     8344 2023-05-05 14:23:07.796431 astro-sdk-python-1.7.0a1/README.md
--rw-r--r--   0        0        0     5401 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/pyproject.toml
--rw-r--r--   0        0        0      687 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/airflow/__init__.py
--rw-r--r--   0        0        0     1605 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/airflow/datasets.py
--rw-r--r--   0        0        0     2256 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/constants.py
--rw-r--r--   0        0        0        0 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/custom_backend/__init__.py
--rw-r--r--   0        0        0     2187 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/custom_backend/astro_custom_backend.py
--rw-r--r--   0        0        0     3915 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/custom_backend/serializer.py
--rw-r--r--   0        0        0     1876 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/aws/__init__.py
--rw-r--r--   0        0        0    18189 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/aws/redshift.py
--rw-r--r--   0        0        0    37369 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/base.py
--rw-r--r--   0        0        0        0 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/__init__.py
--rw-r--r--   0        0        0     7247 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/api_utils.py
--rw-r--r--   0        0        0    18097 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/delta.py
--rw-r--r--   0        0        0        0 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/__init__.py
--rw-r--r--   0        0        0      720 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2
--rw-r--r--   0        0        0      647 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2
--rw-r--r--   0        0        0      913 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2
--rw-r--r--   0        0        0      512 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2
--rw-r--r--   0        0        0     6368 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/load_file_job.py
--rw-r--r--   0        0        0      880 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/load_file_python_code_generator.py
--rw-r--r--   0        0        0     2687 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_options.py
--rw-r--r--   0        0        0     6181 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/duckdb.py
--rw-r--r--   0        0        0        0 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/google/__init__.py
--rw-r--r--   0        0        0    26823 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/google/bigquery.py
--rw-r--r--   0        0        0    17049 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/mssql.py
--rw-r--r--   0        0        0     9267 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/mysql.py
--rw-r--r--   0        0        0    10678 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/postgres.py
--rw-r--r--   0        0        0    42201 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/snowflake.py
--rw-r--r--   0        0        0     6508 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/sqlite.py
--rw-r--r--   0        0        0        0 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/dataframes/__init__.py
--rw-r--r--   0        0        0     4116 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/dataframes/load_options.py
--rw-r--r--   0        0        0     2356 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/dataframes/pandas.py
--rw-r--r--   0        0        0     1267 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/exceptions.py
--rw-r--r--   0        0        0     1096 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/files/__init__.py
--rw-r--r--   0        0        0    10151 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/files/base.py
--rw-r--r--   0        0        0     1535 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/files/locations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/amazon/__init__.py
--rw-r--r--   0        0        0     3605 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/amazon/s3.py
--rw-r--r--   0        0        0        0 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/azure/__init__.py
--rw-r--r--   0        0        0     5867 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/azure/wasb.py
--rw-r--r--   0        0        0     6601 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/base.py
--rw-r--r--   0        0        0     2374 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/ftp.py
--rw-r--r--   0        0        0        0 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/google/__init__.py
--rw-r--r--   0        0        0     4420 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/google/gcs.py
--rw-r--r--   0        0        0     5006 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/google/gdrive.py
--rw-r--r--   0        0        0     1303 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/http.py
--rw-r--r--   0        0        0     1531 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/local.py
--rw-r--r--   0        0        0     3267 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/sftp.py
--rw-r--r--   0        0        0        0 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/operators/__init__.py
--rw-r--r--   0        0        0     1595 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/operators/files.py
--rw-r--r--   0        0        0     2576 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/types/__init__.py
--rw-r--r--   0        0        0     1504 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/types/base.py
--rw-r--r--   0        0        0     1900 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/types/csv.py
--rw-r--r--   0        0        0     2197 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/types/json.py
--rw-r--r--   0        0        0     3652 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/types/ndjson.py
--rw-r--r--   0        0        0     2848 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/types/parquet.py
--rw-r--r--   0        0        0      700 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/lineage/__init__.py
--rw-r--r--   0        0        0     4264 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/lineage/facets.py
--rw-r--r--   0        0        0     3910 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/options.py
--rw-r--r--   0        0        0     1117 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/query_modifier.py
--rw-r--r--   0        0        0     4168 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/settings.py
--rw-r--r--   0        0        0     3194 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/__init__.py
--rw-r--r--   0        0        0     7857 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/append.py
--rw-r--r--   0        0        0    18419 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/base_decorator.py
--rw-r--r--   0        0        0      334 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/base_operator.py
--rw-r--r--   0        0        0    12688 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/cleanup.py
--rw-r--r--   0        0        0     7870 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/data_validations/check_column.py
--rw-r--r--   0        0        0     3696 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/data_validations/check_table.py
--rw-r--r--   0        0        0    15362 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/dataframe.py
--rw-r--r--   0        0        0     1435 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/drop.py
--rw-r--r--   0        0        0     2693 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/export_file.py
--rw-r--r--   0        0        0     2715 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/export_table_to_file.py
--rw-r--r--   0        0        0     7035 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/export_to_file.py
--rw-r--r--   0        0        0    17519 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/load_file.py
--rw-r--r--   0        0        0     8824 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/merge.py
--rw-r--r--   0        0        0     9898 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/raw_sql.py
--rw-r--r--   0        0        0     7393 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/transform.py
--rw-r--r--   0        0        0      880 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/upstream_task_mixin.py
--rw-r--r--   0        0        0      160 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/table.py
--rw-r--r--   0        0        0     8747 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/table.py
--rw-r--r--   0        0        0        0 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/utils/compat/__init__.py
--rw-r--r--   0        0        0      359 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/utils/compat/functools.py
--rw-r--r--   0        0        0      843 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/utils/compat/typing.py
--rw-r--r--   0        0        0     2022 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/utils/dataframe.py
--rw-r--r--   0        0        0     1581 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/utils/load.py
--rw-r--r--   0        0        0     2790 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/utils/path.py
--rw-r--r--   0        0        0     4025 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/utils/table.py
--rw-r--r--   0        0        0    13466 1970-01-01 00:00:00.000000 astro-sdk-python-1.7.0a1/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2023-05-05 23:38:37.411658 astro-sdk-python-1.7.0a2/LICENSE -> ../LICENSE
+-rw-r--r--   0        0        0     8344 2023-05-05 23:38:37.411658 astro-sdk-python-1.7.0a2/README.md
+-rw-r--r--   0        0        0     5401 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/pyproject.toml
+-rw-r--r--   0        0        0      687 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/src/astro/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/src/astro/airflow/__init__.py
+-rw-r--r--   0        0        0     1605 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/src/astro/airflow/datasets.py
+-rw-r--r--   0        0        0     2256 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/src/astro/constants.py
+-rw-r--r--   0        0        0        0 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/src/astro/custom_backend/__init__.py
+-rw-r--r--   0        0        0     2187 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/src/astro/custom_backend/astro_custom_backend.py
+-rw-r--r--   0        0        0     3915 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/src/astro/custom_backend/serializer.py
+-rw-r--r--   0        0        0     1876 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/src/astro/databases/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 23:38:37.423658 astro-sdk-python-1.7.0a2/src/astro/databases/aws/__init__.py
+-rw-r--r--   0        0        0    18189 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/aws/redshift.py
+-rw-r--r--   0        0        0    37548 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/base.py
+-rw-r--r--   0        0        0        0 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/__init__.py
+-rw-r--r--   0        0        0     7247 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/api_utils.py
+-rw-r--r--   0        0        0    18134 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/delta.py
+-rw-r--r--   0        0        0        0 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/__init__.py
+-rw-r--r--   0        0        0      720 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2
+-rw-r--r--   0        0        0      647 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2
+-rw-r--r--   0        0        0      913 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2
+-rw-r--r--   0        0        0      512 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2
+-rw-r--r--   0        0        0     6368 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/load_file_job.py
+-rw-r--r--   0        0        0      880 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/load_file_python_code_generator.py
+-rw-r--r--   0        0        0     2687 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_options.py
+-rw-r--r--   0        0        0     6181 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/duckdb.py
+-rw-r--r--   0        0        0        0 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/google/__init__.py
+-rw-r--r--   0        0        0    26823 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/google/bigquery.py
+-rw-r--r--   0        0        0    17049 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/mssql.py
+-rw-r--r--   0        0        0     9267 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/mysql.py
+-rw-r--r--   0        0        0    10682 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/postgres.py
+-rw-r--r--   0        0        0    42201 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/snowflake.py
+-rw-r--r--   0        0        0     6508 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/databases/sqlite.py
+-rw-r--r--   0        0        0        0 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/dataframes/__init__.py
+-rw-r--r--   0        0        0     4116 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/dataframes/load_options.py
+-rw-r--r--   0        0        0     2356 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/dataframes/pandas.py
+-rw-r--r--   0        0        0     1267 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/exceptions.py
+-rw-r--r--   0        0        0     1096 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/__init__.py
+-rw-r--r--   0        0        0    10151 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/base.py
+-rw-r--r--   0        0        0     1535 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/amazon/__init__.py
+-rw-r--r--   0        0        0     3605 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/amazon/s3.py
+-rw-r--r--   0        0        0        0 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/azure/__init__.py
+-rw-r--r--   0        0        0     5867 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/azure/wasb.py
+-rw-r--r--   0        0        0     6601 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/base.py
+-rw-r--r--   0        0        0     2374 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/ftp.py
+-rw-r--r--   0        0        0        0 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/google/__init__.py
+-rw-r--r--   0        0        0     4420 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/google/gcs.py
+-rw-r--r--   0        0        0     5006 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/google/gdrive.py
+-rw-r--r--   0        0        0     1303 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/http.py
+-rw-r--r--   0        0        0     1531 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/local.py
+-rw-r--r--   0        0        0     3267 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/locations/sftp.py
+-rw-r--r--   0        0        0        0 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/operators/__init__.py
+-rw-r--r--   0        0        0     1595 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/operators/files.py
+-rw-r--r--   0        0        0     2576 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/types/__init__.py
+-rw-r--r--   0        0        0     1504 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/types/base.py
+-rw-r--r--   0        0        0     1900 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/types/csv.py
+-rw-r--r--   0        0        0     2197 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/types/json.py
+-rw-r--r--   0        0        0     3652 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/types/ndjson.py
+-rw-r--r--   0        0        0     2848 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/files/types/parquet.py
+-rw-r--r--   0        0        0      700 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/lineage/__init__.py
+-rw-r--r--   0        0        0     4264 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/lineage/facets.py
+-rw-r--r--   0        0        0     3910 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/options.py
+-rw-r--r--   0        0        0     1117 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/query_modifier.py
+-rw-r--r--   0        0        0     4152 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/settings.py
+-rw-r--r--   0        0        0     3194 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/__init__.py
+-rw-r--r--   0        0        0     7857 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/append.py
+-rw-r--r--   0        0        0    18419 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/base_decorator.py
+-rw-r--r--   0        0        0      334 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/base_operator.py
+-rw-r--r--   0        0        0    12688 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/cleanup.py
+-rw-r--r--   0        0        0     7870 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/data_validations/check_column.py
+-rw-r--r--   0        0        0     3696 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/data_validations/check_table.py
+-rw-r--r--   0        0        0    15362 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/dataframe.py
+-rw-r--r--   0        0        0     1435 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/drop.py
+-rw-r--r--   0        0        0     2693 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/export_file.py
+-rw-r--r--   0        0        0     2715 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/export_table_to_file.py
+-rw-r--r--   0        0        0     7035 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/export_to_file.py
+-rw-r--r--   0        0        0    17526 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/load_file.py
+-rw-r--r--   0        0        0     8824 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/merge.py
+-rw-r--r--   0        0        0     9898 2023-05-05 23:38:37.427658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/raw_sql.py
+-rw-r--r--   0        0        0     8055 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/transform.py
+-rw-r--r--   0        0        0      880 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/sql/operators/upstream_task_mixin.py
+-rw-r--r--   0        0        0      160 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/sql/table.py
+-rw-r--r--   0        0        0     8747 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/table.py
+-rw-r--r--   0        0        0        0 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/utils/compat/__init__.py
+-rw-r--r--   0        0        0      359 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/utils/compat/functools.py
+-rw-r--r--   0        0        0      843 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/utils/compat/typing.py
+-rw-r--r--   0        0        0     2022 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/utils/dataframe.py
+-rw-r--r--   0        0        0     1581 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/utils/load.py
+-rw-r--r--   0        0        0     2790 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/utils/path.py
+-rw-r--r--   0        0        0     4025 2023-05-05 23:38:37.431658 astro-sdk-python-1.7.0a2/src/astro/utils/table.py
+-rw-r--r--   0        0        0    13466 1970-01-01 00:00:00.000000 astro-sdk-python-1.7.0a2/PKG-INFO
```

### Comparing `astro-sdk-python-1.7.0a1/README.md` & `astro-sdk-python-1.7.0a2/README.md`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/pyproject.toml` & `astro-sdk-python-1.7.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/__init__.py` & `astro-sdk-python-1.7.0a2/src/astro/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A decorator that allows users to run SQL queries natively in Airflow."""
 
-__version__ = "1.7.0a1"
+__version__ = "1.7.0a2"
 
 
 # This is needed to allow Airflow to pick up specific metadata fields it needs
 # for certain features. We recognize it's a bit unclean to define these in
 # multiple places, but at this point it's the only workaround if you'd like
 # your custom conn type to show up in the Airflow UI.
 def get_provider_info() -> dict:
```

### Comparing `astro-sdk-python-1.7.0a1/src/astro/airflow/datasets.py` & `astro-sdk-python-1.7.0a2/src/astro/airflow/datasets.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/constants.py` & `astro-sdk-python-1.7.0a2/src/astro/constants.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/custom_backend/astro_custom_backend.py` & `astro-sdk-python-1.7.0a2/src/astro/custom_backend/astro_custom_backend.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/custom_backend/serializer.py` & `astro-sdk-python-1.7.0a2/src/astro/custom_backend/serializer.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/databases/__init__.py` & `astro-sdk-python-1.7.0a2/src/astro/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/databases/aws/redshift.py` & `astro-sdk-python-1.7.0a2/src/astro/databases/aws/redshift.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/databases/base.py` & `astro-sdk-python-1.7.0a2/src/astro/databases/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 from astro.exceptions import DatabaseCustomError, NonExistentTableException
 from astro.files import File, resolve_file_path_pattern
 from astro.files.types import create_file_type
 from astro.files.types.base import FileType as FileTypeConstants
 from astro.options import LoadOptions
 from astro.query_modifier import QueryModifier
 from astro.settings import (
+    ASSUME_SCHEMA_EXISTS,
     LOAD_FILE_ENABLE_NATIVE_FALLBACK,
     LOAD_TABLE_AUTODETECT_ROWS_COUNT,
-    LOAD_TABLE_SCHEMA_EXISTS,
     SCHEMA,
 )
 from astro.table import BaseTable, Metadata
 from astro.utils.compat.functools import cached_property
 
 
 class BaseDatabase(ABC):
@@ -449,15 +449,15 @@
         normalize_config: dict | None = None,
         if_exists: LoadExistStrategy = "replace",
         chunk_size: int = DEFAULT_CHUNK_SIZE,
         use_native_support: bool = True,
         native_support_kwargs: dict | None = None,
         columns_names_capitalization: ColumnCapitalization = "original",
         enable_native_fallback: bool | None = LOAD_FILE_ENABLE_NATIVE_FALLBACK,
-        schema_exists: bool = LOAD_TABLE_SCHEMA_EXISTS,
+        assume_schema_exists: bool = ASSUME_SCHEMA_EXISTS,
         **kwargs,
     ):
         """
         Load content of multiple files in output_table.
         Multiple files are sourced from the file path, which can also be path pattern.
 
         :param input_file: File path and conn_id for object stores
@@ -466,26 +466,25 @@
         :param chunk_size: Specify the number of records in each batch to be written at a time
         :param use_native_support: Use native support for data transfer if available on the destination
         :param normalize_config: pandas json_normalize params config
         :param native_support_kwargs: kwargs to be used by method involved in native support flow
         :param columns_names_capitalization: determines whether to convert all columns to lowercase/uppercase
             in the resulting dataframe
         :param enable_native_fallback: Use enable_native_fallback=True to fall back to default transfer
-        :param schema_exists: Declare the table schema already exists and that load_file should not check if it exists
+        :param assume_schema_exists: If True, do not check if the output table schema it exists or attempt to create it
         """
         normalize_config = normalize_config or {}
         if self.check_for_minio_connection(input_file=input_file):
             logging.info(
                 "No native support available for the service provided via endpoint_url! Setting use_native_support"
                 " to False."
             )
             use_native_support = False
 
-        if not schema_exists:
-            self.create_schema_if_needed(output_table.metadata.schema)
+        self.create_schema_if_applicable(output_table.metadata.schema, assume_schema_exists)
 
         self.create_table_if_needed(
             file=input_file,
             table=output_table,
             columns_names_capitalization=columns_names_capitalization,
             if_exists=if_exists,
             normalize_config=normalize_config,
@@ -741,24 +740,27 @@
         df = self.export_table_to_pandas_dataframe(source_table)
         target_file.create_from_dataframe(df)
 
     # ---------------------------------------------------------
     # Schema Management
     # ---------------------------------------------------------
 
-    def create_schema_if_needed(self, schema: str | None) -> None:
+    def create_schema_if_applicable(
+        self, schema: str | None, assume_exists: bool = ASSUME_SCHEMA_EXISTS
+    ) -> None:
         """
         This function checks if the expected schema exists in the database. If the schema does not exist,
         it will attempt to create it.
 
         :param schema: DB Schema - a namespace that contains named objects like (tables, functions, etc)
+        :param assume_exists: If assume exists is True, does not check or attempt to create the schema
         """
         # We check if the schema exists first because snowflake will fail on a create schema query even if it
         # doesn't actually create a schema.
-        if schema and not self.schema_exists(schema):
+        if not assume_exists and schema and not self.schema_exists(schema):
             statement = self._create_schema_statement.format(schema)
             self.run_sql(statement)
 
     def schema_exists(self, schema: str) -> bool:
         """
         Checks if a schema exists in the database
```

### Comparing `astro-sdk-python-1.7.0a1/src/astro/databases/databricks/api_utils.py` & `astro-sdk-python-1.7.0a2/src/astro/databases/databricks/api_utils.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/databases/databricks/delta.py` & `astro-sdk-python-1.7.0a2/src/astro/databases/databricks/delta.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from astro.databases.base import BaseDatabase
 from astro.databases.databricks.load_file.load_file_job import load_file_to_delta
 from astro.databases.databricks.load_options import DeltaLoadOptions
 from astro.dataframes.pandas import PandasDataframe
 from astro.files import File
 from astro.options import LoadOptions
 from astro.query_modifier import QueryModifier
-from astro.settings import LOAD_TABLE_SCHEMA_EXISTS
+from astro.settings import ASSUME_SCHEMA_EXISTS
 from astro.table import BaseTable, Metadata
 
 
 class DeltaDatabase(BaseDatabase):
     LOAD_OPTIONS_CLASS_NAME = ("DeltaLoadOptions",)
     _create_table_statement: str = "CREATE TABLE IF NOT EXISTS {} USING DELTA AS {} "
 
@@ -91,15 +91,17 @@
         # TODO Do we need to implement this function? It seems like databricks will handle schemas for us
         raise NotImplementedError("Not implemented yet.")
 
     def schema_exists(self, schema: str) -> bool:
         # Schemas do not need to be created for delta, so we can assume this is true
         return True
 
-    def create_schema_if_needed(self, schema: str | None) -> None:  # skipcq: PYL-W0613
+    def create_schema_if_applicable(
+        self, schema: str | None, assume_exists: bool = ASSUME_SCHEMA_EXISTS
+    ) -> None:  # skipcq: PYL-W0613
         # Schemas do not need to be created for delta, so we don't need to do anything here
         return None
 
     def fetch_all_rows(self, table: BaseTable, row_limit: int = -1) -> list:
         """
         Fetches all rows for a table and returns as a list. This is needed because some
         databases have different cursors that require different methods to fetch rows
@@ -120,15 +122,15 @@
         normalize_config: dict | None = None,
         if_exists: LoadExistStrategy = "replace",
         chunk_size: int = DEFAULT_CHUNK_SIZE,
         use_native_support: bool = True,
         native_support_kwargs: dict | None = None,
         columns_names_capitalization: ColumnCapitalization = "original",
         enable_native_fallback: bool | None = None,
-        schema_exists: bool = LOAD_TABLE_SCHEMA_EXISTS,
+        assume_schema_exists: bool = ASSUME_SCHEMA_EXISTS,
         databricks_job_name: str = "",
         **kwargs,
     ):
         """
         Load content of multiple files in output_table.
         Multiple files are sourced from the file path, which can also be path pattern.
 
@@ -140,15 +142,15 @@
         :param chunk_size: Specify the number of records in each batch to be written at a time
         :param use_native_support: Use native support for data transfer if available on the destination
         :param normalize_config: pandas json_normalize params config
         :param native_support_kwargs: kwargs to be used by method involved in native support flow
         :param columns_names_capitalization: determines whether to convert all columns to lowercase/uppercase
             in the resulting dataframe
         :param enable_native_fallback: Use enable_native_fallback=True to fall back to default transfer
-        :param schema_exists: Declare the table schema already exists and that load_file should not check if it exists
+        :param assume_schema_exists: If True, skips check to see if output_table schema exists
         """
         load_file_to_delta(
             input_file=input_file,
             delta_table=output_table,
             databricks_job_name=databricks_job_name,
             delta_load_options=self.load_options,  # type: ignore
             if_exists=if_exists,
```

### Comparing `astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2` & `astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2` & `astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2` & `astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2` & `astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/load_file_job.py` & `astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/load_file_job.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/load_file_python_code_generator.py` & `astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_file/load_file_python_code_generator.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_options.py` & `astro-sdk-python-1.7.0a2/src/astro/databases/databricks/load_options.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/databases/duckdb.py` & `astro-sdk-python-1.7.0a2/src/astro/databases/duckdb.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/databases/google/bigquery.py` & `astro-sdk-python-1.7.0a2/src/astro/databases/google/bigquery.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/databases/mssql.py` & `astro-sdk-python-1.7.0a2/src/astro/databases/mssql.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/databases/mysql.py` & `astro-sdk-python-1.7.0a2/src/astro/databases/mysql.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/databases/postgres.py` & `astro-sdk-python-1.7.0a2/src/astro/databases/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         :param source_dataframe: Local or remote filepath
         :param target_table: Table in which the file will be loaded
         :param if_exists: Strategy to be used in case the target table already exists.
         :param chunk_size: Specify the number of rows in each batch to be written at a time.
         """
         self._assert_not_empty_df(source_dataframe)
 
-        self.create_schema_if_needed(target_table.metadata.schema)
+        self.create_schema_if_applicable(target_table.metadata.schema)
         if not self.table_exists(table=target_table) or if_exists == "replace":
             self.create_table(table=target_table, dataframe=source_dataframe)
 
         output_buffer = io.StringIO()
         source_dataframe.to_csv(output_buffer, sep=",", header=True, index=False)
         output_buffer.seek(0)
         table_name = self.get_table_qualified_name(target_table)
```

### Comparing `astro-sdk-python-1.7.0a1/src/astro/databases/snowflake.py` & `astro-sdk-python-1.7.0a2/src/astro/databases/snowflake.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/databases/sqlite.py` & `astro-sdk-python-1.7.0a2/src/astro/databases/sqlite.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/dataframes/load_options.py` & `astro-sdk-python-1.7.0a2/src/astro/dataframes/load_options.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/dataframes/pandas.py` & `astro-sdk-python-1.7.0a2/src/astro/dataframes/pandas.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/exceptions.py` & `astro-sdk-python-1.7.0a2/src/astro/exceptions.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/files/__init__.py` & `astro-sdk-python-1.7.0a2/src/astro/files/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/files/base.py` & `astro-sdk-python-1.7.0a2/src/astro/files/base.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/files/locations/__init__.py` & `astro-sdk-python-1.7.0a2/src/astro/files/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/files/locations/amazon/s3.py` & `astro-sdk-python-1.7.0a2/src/astro/files/locations/amazon/s3.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/files/locations/azure/wasb.py` & `astro-sdk-python-1.7.0a2/src/astro/files/locations/azure/wasb.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/files/locations/base.py` & `astro-sdk-python-1.7.0a2/src/astro/files/locations/base.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/files/locations/ftp.py` & `astro-sdk-python-1.7.0a2/src/astro/files/locations/ftp.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/files/locations/google/gcs.py` & `astro-sdk-python-1.7.0a2/src/astro/files/locations/google/gcs.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/files/locations/google/gdrive.py` & `astro-sdk-python-1.7.0a2/src/astro/files/locations/google/gdrive.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/files/locations/http.py` & `astro-sdk-python-1.7.0a2/src/astro/files/locations/http.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/files/locations/local.py` & `astro-sdk-python-1.7.0a2/src/astro/files/locations/local.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/files/locations/sftp.py` & `astro-sdk-python-1.7.0a2/src/astro/files/locations/sftp.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/files/operators/files.py` & `astro-sdk-python-1.7.0a2/src/astro/files/operators/files.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/files/types/__init__.py` & `astro-sdk-python-1.7.0a2/src/astro/files/types/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/files/types/base.py` & `astro-sdk-python-1.7.0a2/src/astro/files/types/base.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/files/types/csv.py` & `astro-sdk-python-1.7.0a2/src/astro/files/types/csv.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/files/types/json.py` & `astro-sdk-python-1.7.0a2/src/astro/files/types/json.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/files/types/ndjson.py` & `astro-sdk-python-1.7.0a2/src/astro/files/types/ndjson.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/files/types/parquet.py` & `astro-sdk-python-1.7.0a2/src/astro/files/types/parquet.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/lineage/__init__.py` & `astro-sdk-python-1.7.0a2/src/astro/lineage/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/lineage/facets.py` & `astro-sdk-python-1.7.0a2/src/astro/lineage/facets.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/options.py` & `astro-sdk-python-1.7.0a2/src/astro/options.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/query_modifier.py` & `astro-sdk-python-1.7.0a2/src/astro/query_modifier.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/settings.py` & `astro-sdk-python-1.7.0a2/src/astro/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,19 +71,19 @@
 #: Reduce responses sizes returned by aql.run_raw_sql to avoid trashing the Airflow DB if the BaseXCom is used.
 RAW_SQL_MAX_RESPONSE_SIZE = conf.getint(section=SECTION_KEY, key="run_raw_sql_response_size", fallback=-1)
 
 # Temp changes
 # Should Astro SDK automatically add inlets/outlets to take advantage of Airflow 2.4 Data-aware scheduling
 AUTO_ADD_INLETS_OUTLETS = conf.getboolean(SECTION_KEY, "auto_add_inlets_outlets", fallback=True)
 
-LOAD_TABLE_SCHEMA_EXISTS = False
+ASSUME_SCHEMA_EXISTS = False
 
 
 def reload():
     """
     Reload settings from environment variable during runtime.
     """
-    global LOAD_TABLE_SCHEMA_EXISTS  # skipcq: PYL-W0603
-    LOAD_TABLE_SCHEMA_EXISTS = conf.getboolean(SECTION_KEY, "load_table_schema_exists", fallback=False)
+    global ASSUME_SCHEMA_EXISTS  # skipcq: PYL-W0603
+    ASSUME_SCHEMA_EXISTS = conf.getboolean(SECTION_KEY, "assume_schema_exists", fallback=False)
 
 
 reload()
```

### Comparing `astro-sdk-python-1.7.0a1/src/astro/sql/__init__.py` & `astro-sdk-python-1.7.0a2/src/astro/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/sql/operators/append.py` & `astro-sdk-python-1.7.0a2/src/astro/sql/operators/append.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/sql/operators/base_decorator.py` & `astro-sdk-python-1.7.0a2/src/astro/sql/operators/base_decorator.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/sql/operators/cleanup.py` & `astro-sdk-python-1.7.0a2/src/astro/sql/operators/cleanup.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/sql/operators/data_validations/check_column.py` & `astro-sdk-python-1.7.0a2/src/astro/sql/operators/data_validations/check_column.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/sql/operators/data_validations/check_table.py` & `astro-sdk-python-1.7.0a2/src/astro/sql/operators/data_validations/check_table.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/sql/operators/dataframe.py` & `astro-sdk-python-1.7.0a2/src/astro/sql/operators/dataframe.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/sql/operators/drop.py` & `astro-sdk-python-1.7.0a2/src/astro/sql/operators/drop.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/sql/operators/export_file.py` & `astro-sdk-python-1.7.0a2/src/astro/sql/operators/export_file.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/sql/operators/export_table_to_file.py` & `astro-sdk-python-1.7.0a2/src/astro/sql/operators/export_table_to_file.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/sql/operators/export_to_file.py` & `astro-sdk-python-1.7.0a2/src/astro/sql/operators/export_to_file.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/sql/operators/load_file.py` & `astro-sdk-python-1.7.0a2/src/astro/sql/operators/load_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     :param chunk_size: Specify the number of records in each batch to be written at a time.
     :param if_exists: Overwrite file if exists. Default False.
     :param use_native_support: Use native support for data transfer if available on the destination.
     :param native_support_kwargs: kwargs to be used by method involved in native support flow
     :param columns_names_capitalization: determines whether to convert all columns to lowercase/uppercase
             in the resulting dataframe
     :param enable_native_fallback: Use enable_native_fallback=True to fall back to default transfer
-    :param schema_exists: Declare the table schema already exists and that load_file should not check if it exists
+    :param assume_schema_exists: If True, skips check to see if output_table schema exists
 
     :return: If ``output_table`` is passed this operator returns a Table object. If not
         passed, returns a dataframe.
     """
 
     template_fields = ("output_table", "input_file")
 
@@ -63,15 +63,15 @@
         if_exists: LoadExistStrategy = "replace",
         ndjson_normalize_sep: str = "_",
         use_native_support: bool = True,
         native_support_kwargs: dict | None = None,
         load_options: LoadOptions | list[LoadOptions] | None = None,
         columns_names_capitalization: ColumnCapitalization = "original",
         enable_native_fallback: bool | None = settings.LOAD_FILE_ENABLE_NATIVE_FALLBACK,
-        schema_exists: bool = settings.LOAD_TABLE_SCHEMA_EXISTS,
+        assume_schema_exists: bool = settings.ASSUME_SCHEMA_EXISTS,
         **kwargs,
     ) -> None:
         kwargs.setdefault("task_id", get_unique_task_id("load_file"))
         super().__init__(
             **kwargs_with_datasets(
                 kwargs=kwargs,
                 input_datasets=input_file,
@@ -110,15 +110,15 @@
         self.if_exists = if_exists
         self.ndjson_normalize_sep = ndjson_normalize_sep
         self.normalize_config: dict[str, str] = {}
         self.use_native_support = use_native_support
         self.native_support_kwargs: dict[str, Any] = native_support_kwargs or {}
         self.columns_names_capitalization = columns_names_capitalization
         self.enable_native_fallback = enable_native_fallback
-        self.schema_exists = schema_exists
+        self.assume_schema_exists = assume_schema_exists
         self.load_options_list = LoadOptionsList(load_options)
 
     def execute(self, context: Context) -> BaseTable | File:  # skipcq: PYL-W0613
         """
         Load an existing dataset from a supported file into a SQL table or a Dataframe.
         """
         if self.input_file.conn_id:
@@ -158,15 +158,15 @@
             output_table=self.output_table,
             if_exists=self.if_exists,
             chunk_size=self.chunk_size,
             use_native_support=self.use_native_support,
             native_support_kwargs=self.native_support_kwargs,
             columns_names_capitalization=self.columns_names_capitalization,
             enable_native_fallback=self.enable_native_fallback,
-            schema_exists=self.schema_exists,
+            assume_schema_exists=self.assume_schema_exists,
             databricks_job_name=f"Load data {self.dag_id}_{self.task_id}",
         )
         self.log.info("Completed loading the data into %s.", self.output_table)
         return self.output_table
 
     def load_data_to_dataframe(self, input_file: File) -> pd.DataFrame | None:
         """
```

### Comparing `astro-sdk-python-1.7.0a1/src/astro/sql/operators/merge.py` & `astro-sdk-python-1.7.0a2/src/astro/sql/operators/merge.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/sql/operators/raw_sql.py` & `astro-sdk-python-1.7.0a2/src/astro/sql/operators/raw_sql.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/sql/operators/transform.py` & `astro-sdk-python-1.7.0a2/src/astro/sql/operators/transform.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 except ImportError:
     from airflow.decorators import _TaskDecorator as TaskDecorator
 
 from airflow.decorators.base import get_unique_task_id, task_decorator_factory
 from airflow.models.xcom_arg import XComArg
 from sqlalchemy.sql.functions import Function
 
+from astro.settings import ASSUME_SCHEMA_EXISTS
 from astro.sql.operators.base_decorator import BaseSQLDecoratedOperator
 from astro.utils.compat.typing import Context
 
 
 class TransformOperator(BaseSQLDecoratedOperator):
     """
     Given a SQL statement and (optional) tables, execute the SQL statement and output
@@ -29,17 +30,19 @@
         handler: Function | None = None,
         database: str | None = None,
         schema: str | None = None,
         response_limit: int = -1,
         response_size: int = -1,
         sql: str = "",
         task_id: str = "",
+        assume_schema_exists: bool = ASSUME_SCHEMA_EXISTS,
         **kwargs: Any,
     ):
         task_id = task_id or get_unique_task_id("transform")
+        self.assume_schema_exists = assume_schema_exists
         super().__init__(
             conn_id=conn_id,
             parameters=parameters,
             handler=handler,
             database=database,
             schema=schema,
             response_limit=response_limit,
@@ -47,15 +50,17 @@
             sql=sql,
             task_id=task_id,
             **kwargs,
         )
 
     def execute(self, context: Context):
         super().execute(context)
-        self.database_impl.create_schema_if_needed(self.output_table.metadata.schema)
+        self.database_impl.create_schema_if_applicable(
+            self.output_table.metadata.schema, self.assume_schema_exists
+        )
         self.database_impl.drop_table(self.output_table)
         self.database_impl.create_table_from_select_statement(
             statement=self.sql,
             target_table=self.output_table,
             parameters=self.parameters,
             query_modifier=self.query_modifier,
         )
@@ -69,14 +74,15 @@
 
 def transform(
     python_callable: Callable | None = None,
     conn_id: str = "",
     parameters: Mapping | Iterable | None = None,
     database: str | None = None,
     schema: str | None = None,
+    assume_schema_exists: bool = ASSUME_SCHEMA_EXISTS,
     **kwargs: Any,
 ) -> TaskDecorator:
     """
     Given a python function that returns a SQL statement and (optional) tables, execute the SQL statement and output
     the result into a SQL table.
 
     Use this function as a decorator like so:
@@ -107,27 +113,29 @@
         we can infer the connection ID from the first table passed into the python_callable function.
         (required if there are no table arguments)
     :param parameters: parameters to pass into the SQL query
     :param database: Database within the SQL instance you want to access. If left blank we will default to the
         table.metadata.database in the first Table passed to the function (required if there are no table arguments)
     :param schema: Schema within the SQL instance you want to access. If left blank we will default to the
         table.metadata.schema in the first Table passed to the function (required if there are no table arguments)
+    :param assume_schema_exists: If True, do not check if the output table schema exists or attempt to create it
     :param kwargs: Any keyword arguments supported by the BaseOperator is supported (e.g ``queue``, ``owner``)
     :return: Transform functions return a ``Table`` object that can be passed to future tasks.
         This table will be either an auto-generated temporary table,
         or will overwrite a table given in the `output_table` parameter.
     """
 
     kwargs.update(
         {
             "conn_id": conn_id,
             "parameters": parameters,
             "database": database,
             "schema": schema,
             "handler": None,
+            "assume_schema_exists": assume_schema_exists,
         }
     )
     return task_decorator_factory(
         python_callable=python_callable,
         multiple_outputs=False,
         decorated_operator_class=TransformOperator,
         **kwargs,
@@ -136,14 +144,15 @@
 
 def transform_file(
     file_path: str,
     conn_id: str = "",
     parameters: dict | None = None,
     database: str | None = None,
     schema: str | None = None,
+    assume_schema_exists: bool = ASSUME_SCHEMA_EXISTS,
     **kwargs: Any,
 ) -> XComArg:
     """
     This function returns a ``Table`` object that can be passed to future tasks from specified SQL file.
     Tables can be inserted via the parameters kwarg.
 
     :param file_path: File path for the SQL file you would like to parse. Can be an absolute path, or you can use a
@@ -152,14 +161,15 @@
         we can infer the connection ID from the first table passed into the python_callable function.
         (required if there are no table arguments)
     :param parameters: parameters to pass into the SQL query
     :param database: Database within the SQL instance you want to access. If left blank we will default to the
         table.metadata.database in the first Table passed to the function (required if there are no table arguments)
     :param schema: Schema within the SQL instance you want to access. If left blank we will default to the
         table.metadata.schema in the first Table passed to the function (required if there are no table arguments)
+    :param assume_schema_exists: If True, do not check if the output table schema exists or attempt to create it
     :param kwargs: Any keyword arguments supported by the BaseOperator is supported (e.g ``queue``, ``owner``)
     :return: Transform functions return a ``Table`` object that can be passed to future tasks.
         This table will be either an auto-generated temporary table,
         or will overwrite a table given in the `output_table` parameter.
     """
 
     kwargs.update(
@@ -171,10 +181,11 @@
     return TransformOperator(
         conn_id=conn_id,
         parameters=parameters,
         handler=None,
         database=database,
         schema=schema,
         sql=file_path,
+        assume_schema_exists=assume_schema_exists,
         python_callable=lambda: (file_path, parameters),
         **kwargs,
     ).output
```

### Comparing `astro-sdk-python-1.7.0a1/src/astro/sql/operators/upstream_task_mixin.py` & `astro-sdk-python-1.7.0a2/src/astro/sql/operators/upstream_task_mixin.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/table.py` & `astro-sdk-python-1.7.0a2/src/astro/table.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/utils/compat/typing.py` & `astro-sdk-python-1.7.0a2/src/astro/utils/compat/typing.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/utils/dataframe.py` & `astro-sdk-python-1.7.0a2/src/astro/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/utils/load.py` & `astro-sdk-python-1.7.0a2/src/astro/utils/load.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/utils/path.py` & `astro-sdk-python-1.7.0a2/src/astro/utils/path.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/src/astro/utils/table.py` & `astro-sdk-python-1.7.0a2/src/astro/utils/table.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.7.0a1/PKG-INFO` & `astro-sdk-python-1.7.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-sdk-python
-Version: 1.7.0a1
+Version: 1.7.0a2
 Summary: Astro SDK allows rapid and clean development of {Extract, Load, Transform} workflows using Python and SQL, powered by Apache Airflow.
 Keywords: airflow,provider,astronomer,sql,decorator,task flow,elt,etl,dag
 Author-email: Astronomer <humans@astronomer.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

