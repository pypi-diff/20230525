# Comparing `tmp/oarepo-model-builder-files-4.0.0.tar.gz` & `tmp/oarepo-model-builder-files-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-files-4.0.0.tar", last modified: Sat May 20 14:03:16 2023, max compression
+gzip compressed data, was "oarepo-model-builder-files-4.0.1.tar", last modified: Thu May 25 12:36:42 2023, max compression
```

## Comparing `oarepo-model-builder-files-4.0.0.tar` & `oarepo-model-builder-files-4.0.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.595688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.595688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.595688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/invenio_files_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/invenio_files_record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/invenio_files_record_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/invenio_files_record_service_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.595688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_permissions.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_service_config.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio_parent/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio_parent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio_parent/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_schema.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/parent_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/invenio_files_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/invenio_files_conftest_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/invenio_files_test_file_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest_files.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/templates/invenio_files_test_file_resources.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builtin_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builtin_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builtin_models/invenio_files.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/datatypes/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/datatypes/components/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/datatypes/components/parent_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/datatypes/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/profiles/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.595688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-20 14:03:16.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-20 14:03:16.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 14:03:16.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-20 14:03:16.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-20 14:03:16.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-20 14:03:16.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-20 14:03:16.603688 oarepo-model-builder-files-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:36:42.194247 oarepo-model-builder-files-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-25 12:36:42.194247 oarepo-model-builder-files-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:36:42.182247 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:36:42.186247 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:36:42.186247 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio/invenio_files_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio/invenio_files_record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio/invenio_files_record_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio/invenio_files_record_service_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:36:42.186247 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_permissions.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_service_config.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:36:42.190247 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio_parent/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio_parent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:36:42.190247 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio_parent/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_schema.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/parent_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:36:42.190247 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/tests/invenio_files_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/tests/invenio_files_conftest_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/tests/invenio_files_test_file_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:36:42.190247 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest_files.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/tests/templates/invenio_files_test_file_resources.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:36:42.190247 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builtin_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builtin_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builtin_models/invenio_files.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:36:42.190247 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:36:42.194247 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/datatypes/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/datatypes/components/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/datatypes/components/parent_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/datatypes/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:36:42.194247 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/profiles/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:36:42.186247 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-25 12:36:42.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-25 12:36:42.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:36:42.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-25 12:36:42.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 12:36:42.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 12:36:42.000000 oarepo-model-builder-files-4.0.1/oarepo_model_builder_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-25 12:36:42.194247 oarepo-model-builder-files-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 12:31:34.000000 oarepo-model-builder-files-4.0.1/setup.py
```

### Comparing `oarepo-model-builder-files-4.0.0/PKG-INFO` & `oarepo-model-builder-files-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-files
-Version: 4.0.0
+Version: 4.0.1
 Description-Content-Type: text/markdown
 
 # OARepo model builder files
 
 Plugin adding support for working with files based on the invenio model. <br>
 Files are represented as another ("file") record connected with the original parent one.
 The plugin generates the file record and modifies the parent record to create connection with new file one.
```

### Comparing `oarepo-model-builder-files-4.0.0/README.md` & `oarepo-model-builder-files-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/__init__.py` & `oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_permissions.py.jinja2` & `oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_permissions.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_schema.py.jinja2` & `oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_schema.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest_files.py.jinja2` & `oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest_files.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/templates/invenio_files_test_file_resources.py.jinja2` & `oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builders/tests/templates/invenio_files_test_file_resources.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builtin_models/invenio_files.json` & `oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/builtin_models/invenio_files.json`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/datatypes/components/file.py` & `oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/datatypes/components/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,15 @@
         pid = set_default(datatype, "pid", {})
         pid.setdefault(
             "type",
             process_pid_type(parent_record_datatype.definition["pid"]["type"] + "File"),
         )
 
         set_default(datatype, "search-options", {}).setdefault("skip", True)
+        set_default(datatype, "facets", {}).setdefault("skip", True)
         set_default(datatype, "json-schema-settings", {}).setdefault("skip", True)
         set_default(datatype, "mapping-settings", {}).setdefault("skip", True)
         set_default(datatype, "record-dumper", {}).setdefault("skip", True)
 
 
 class FileMetadataComponent(DataTypeComponent):
     eligible_datatypes = [ModelDataType]
```

### Comparing `oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/datatypes/components/parent_record.py` & `oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/datatypes/components/parent_record.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/profiles/file.py` & `oarepo-model-builder-files-4.0.1/oarepo_model_builder_files/profiles/file.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.0/oarepo_model_builder_files.egg-info/PKG-INFO` & `oarepo-model-builder-files-4.0.1/oarepo_model_builder_files.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-files
-Version: 4.0.0
+Version: 4.0.1
 Description-Content-Type: text/markdown
 
 # OARepo model builder files
 
 Plugin adding support for working with files based on the invenio model. <br>
 Files are represented as another ("file") record connected with the original parent one.
 The plugin generates the file record and modifies the parent record to create connection with new file one.
```

### Comparing `oarepo-model-builder-files-4.0.0/oarepo_model_builder_files.egg-info/SOURCES.txt` & `oarepo-model-builder-files-4.0.1/oarepo_model_builder_files.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.0/oarepo_model_builder_files.egg-info/entry_points.txt` & `oarepo-model-builder-files-4.0.1/oarepo_model_builder_files.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.0/setup.cfg` & `oarepo-model-builder-files-4.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-files
-version = 4.0.0
+version = 4.0.1
 description = 
 authors = Ronald Krist <krist@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

