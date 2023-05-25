# Comparing `tmp/CosmoTech_Acceleration_Library-0.2.8.tar.gz` & `tmp/CosmoTech_Acceleration_Library-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CosmoTech_Acceleration_Library-0.2.8.tar", last modified: Fri Feb 17 14:07:50 2023, max compression
+gzip compressed data, was "CosmoTech_Acceleration_Library-0.2.9.tar", last modified: Mon Apr 24 08:45:06 2023, max compression
```

## Comparing `CosmoTech_Acceleration_Library-0.2.8.tar` & `CosmoTech_Acceleration_Library-0.2.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:50.747234 CosmoTech_Acceleration_Library-0.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:50.739234 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:50.743234 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Accelerators/
--rw-r--r--   0 runner    (1001) docker     (116)      147 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Accelerators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10972 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Accelerators/adx_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (116)     2540 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Accelerators/cosmo_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1875 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Accelerators/csm_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:50.743234 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Accelerators/scenario_download/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Accelerators/scenario_download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1199 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Accelerators/scenario_download/azure_function_main.py
--rw-r--r--   0 runner    (1001) docker     (116)    11257 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Accelerators/scenario_download/scenario_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:50.743234 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Accelerators/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Accelerators/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      525 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Accelerators/utils/multi_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:50.743234 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Core/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:50.743234 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Core/DataInterface/
--rw-r--r--   0 runner    (1001) docker     (116)       73 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Core/DataInterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:50.743234 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Core/DataStorage/
--rw-r--r--   0 runner    (1001) docker     (116)       73 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Core/DataStorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:50.743234 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/
--rw-r--r--   0 runner    (1001) docker     (116)       74 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:50.743234 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/
--rw-r--r--   0 runner    (1001) docker     (116)       74 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:50.747234 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/common/
--rw-r--r--   0 runner    (1001) docker     (116)       74 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5102 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/common/graph_handler.py
--rw-r--r--   0 runner    (1001) docker     (116)      589 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/common/redis_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:50.747234 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/common/writer/
--rw-r--r--   0 runner    (1001) docker     (116)     2853 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/common/writer/CsvWriter.py
--rw-r--r--   0 runner    (1001) docker     (116)       74 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/common/writer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:50.747234 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/decorators/
--rw-r--r--   0 runner    (1001) docker     (116)       74 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1850 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/decorators/model_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:50.747234 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/io/
--rw-r--r--   0 runner    (1001) docker     (116)       74 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4339 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/io/model_exporter.py
--rw-r--r--   0 runner    (1001) docker     (116)     2200 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/io/model_importer.py
--rw-r--r--   0 runner    (1001) docker     (116)     5688 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/io/model_metadata.py
--rw-r--r--   0 runner    (1001) docker     (116)     4747 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/io/model_reader.py
--rw-r--r--   0 runner    (1001) docker     (116)     1343 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/io/model_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:50.747234 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/utils/
--rw-r--r--   0 runner    (1001) docker     (116)       74 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6606 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/utils/model_util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:50.747234 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (116)       74 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4581 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/model_util_test.py
--rw-r--r--   0 runner    (1001) docker     (116)       97 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 14:07:50.743234 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2218 2023-02-17 14:07:50.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2372 2023-02-17 14:07:50.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-17 14:07:50.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      306 2023-02-17 14:07:50.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       31 2023-02-17 14:07:50.000000 CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1195 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     2218 2023-02-17 14:07:50.747234 CosmoTech_Acceleration_Library-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1857 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-02-17 14:07:50.747234 CosmoTech_Acceleration_Library-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      857 2023-02-17 14:07:40.000000 CosmoTech_Acceleration_Library-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.179604 CosmoTech_Acceleration_Library-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/adx_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/cosmo_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/csm_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/scenario_download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/scenario_download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/scenario_download/azure_function_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/scenario_download/scenario_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/utils/multi_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Core/DataInterface/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Core/DataInterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Core/DataStorage/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Core/DataStorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/graph_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/redis_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/writer/CsvWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/writer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/decorators/model_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.179604 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/model_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/model_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/model_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/model_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/model_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.179604 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/utils/model_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.179604 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/model_util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-24 08:45:06.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-24 08:45:06.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:45:06.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-24 08:45:06.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-24 08:45:06.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-24 08:45:06.179604 CosmoTech_Acceleration_Library-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 08:45:06.179604 CosmoTech_Acceleration_Library-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/setup.py
```

### Comparing `CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Accelerators/adx_wrapper.py` & `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/adx_wrapper.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Accelerators/cosmo_api.py` & `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/cosmo_api.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Accelerators/csm_engine.py` & `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/csm_engine.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Accelerators/scenario_download/azure_function_main.py` & `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/scenario_download/azure_function_main.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Accelerators/scenario_download/scenario_downloader.py` & `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/scenario_download/scenario_downloader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Accelerators/utils/multi_environment.py` & `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/utils/multi_environment.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/common/graph_handler.py` & `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/graph_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 class GraphHandler(RedisHandler):
     """
     Class that handle Graph Redis information
     """
 
-    def __init__(self, host: str, port: int, name: str, password: str = None, source_url: str = "", graph_rotation: int = 1):
+    def __init__(self, host: str, port: int, name: str, password: str = None, source_url: str = "", graph_rotation: int = 3):
         super().__init__(host=host, port=port, name=name, password=password)
         logger.debug("GraphHandler init")
         self.graph = self.r.graph(name)
         self.m_metadata = ModelMetadata(host=host, port=port, name=name, password=password)
         current_metadata = self.m_metadata.get_metadata()
         if not current_metadata:
             logger.debug("Create metadata key")
@@ -29,15 +29,15 @@
 
 class VersionedGraphHandler(GraphHandler):
     """
     Class that handle Versioned Graph Redis information
     """
 
     def __init__(self, host: str, port: int, name: str, version: int, password: str = None, source_url: str = "",
-                 graph_rotation: int = 1):
+                 graph_rotation: int = 3):
         super().__init__(host=host, port=port, name=name, password=password, source_url=source_url,
                          graph_rotation=graph_rotation)
         logger.debug("VersionedGraphHandler init")
         self.version = None
         self.versioned_name = None
         self.fill_versioned_graph_data(name, version)
 
@@ -56,25 +56,24 @@
 
 class RotatedGraphHandler(VersionedGraphHandler):
     """
     Class that handle Rotated Graph Redis information
     """
 
     def __init__(self, host: str, port: int, name: str, password: str = None, version: int = -1, source_url: str = "",
-                 graph_rotation: int = 1):
+                 graph_rotation: int = 3):
         super().__init__(host=host, port=port, name=name, password=password, source_url=source_url, version=version,
                          graph_rotation=graph_rotation)
         logger.debug("RotatedGraphHandler init")
         self.graph_rotation = graph_rotation
         new_version = version
         if version == -1:
             logger.debug("Handle Rotation Graph")
             new_version = self.handle_graph_rotation(name, graph_rotation)
         self.fill_versioned_graph_data(name, new_version)
-        self.m_metadata.set_graph_rotation(graph_rotation=graph_rotation)
 
     def handle_graph_rotation(self, graph_name: str, graph_rotation: int) -> int:
         """
         Handle graph rotation (delete the oldest graph if the amount of graph is greater than graph rotation)
         :param graph_name: the graph name
         :param graph_rotation: the amount of graph to keep
         :return: the graph version to create
```

### Comparing `CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/common/redis_handler.py` & `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/redis_handler.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/common/writer/CsvWriter.py` & `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/writer/CsvWriter.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/decorators/model_decorators.py` & `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/decorators/model_decorators.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/io/model_exporter.py` & `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/model_exporter.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/io/model_importer.py` & `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/model_importer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/io/model_metadata.py` & `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/model_metadata.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/io/model_reader.py` & `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/model_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/io/model_writer.py` & `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/model_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/utils/model_util.py` & `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/utils/model_util.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/model_util_test.py` & `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/model_util_test.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library.egg-info/PKG-INFO` & `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CosmoTech-Acceleration-Library
-Version: 0.2.8
+Version: 0.2.9
 Summary: Acceleration libraries for CosmoTech cloud based solution development
 Home-page: https://github.com/Cosmo-Tech/CosmoTech-Acceleration-Library
 Author: afossart
 Author-email: alexis.fossart@cosmotech.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `CosmoTech_Acceleration_Library-0.2.8/CosmoTech_Acceleration_Library.egg-info/SOURCES.txt` & `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.8/LICENSE` & `CosmoTech_Acceleration_Library-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.8/PKG-INFO` & `CosmoTech_Acceleration_Library-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CosmoTech_Acceleration_Library
-Version: 0.2.8
+Version: 0.2.9
 Summary: Acceleration libraries for CosmoTech cloud based solution development
 Home-page: https://github.com/Cosmo-Tech/CosmoTech-Acceleration-Library
 Author: afossart
 Author-email: alexis.fossart@cosmotech.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `CosmoTech_Acceleration_Library-0.2.8/README.md` & `CosmoTech_Acceleration_Library-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.8/setup.py` & `CosmoTech_Acceleration_Library-0.2.9/setup.py`

 * *Files identical despite different names*

