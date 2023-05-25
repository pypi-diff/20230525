# Comparing `tmp/ign-gpao-utils-0.0.1.tar.gz` & `tmp/ign-gpao-utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ign-gpao-utils-0.0.1.tar", last modified: Tue May 23 14:52:01 2023, max compression
+gzip compressed data, was "ign-gpao-utils-0.0.2.tar", last modified: Thu May 25 15:31:26 2023, max compression
```

## Comparing `ign-gpao-utils-0.0.1.tar` & `ign-gpao-utils-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:52:01.835411 ign-gpao-utils-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-23 14:52:01.835411 ign-gpao-utils-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-23 14:51:57.000000 ign-gpao-utils-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:52:01.835411 ign-gpao-utils-0.0.1/gpao_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:57.000000 ign-gpao-utils-0.0.1/gpao_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-23 14:51:57.000000 ign-gpao-utils-0.0.1/gpao_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-23 14:51:57.000000 ign-gpao-utils-0.0.1/gpao_utils/utils_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:52:01.835411 ign-gpao-utils-0.0.1/ign_gpao_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-23 14:52:01.000000 ign-gpao-utils-0.0.1/ign_gpao_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-23 14:52:01.000000 ign-gpao-utils-0.0.1/ign_gpao_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:52:01.000000 ign-gpao-utils-0.0.1/ign_gpao_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 14:52:01.000000 ign-gpao-utils-0.0.1/ign_gpao_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:52:01.835411 ign-gpao-utils-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-23 14:51:57.000000 ign-gpao-utils-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:52:01.835411 ign-gpao-utils-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-23 14:51:57.000000 ign-gpao-utils-0.0.1/test/test_utils_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:26.540844 ign-gpao-utils-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-25 15:31:26.540844 ign-gpao-utils-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 15:31:22.000000 ign-gpao-utils-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:26.540844 ign-gpao-utils-0.0.2/gpao_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:22.000000 ign-gpao-utils-0.0.2/gpao_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-25 15:31:22.000000 ign-gpao-utils-0.0.2/gpao_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 15:31:22.000000 ign-gpao-utils-0.0.2/gpao_utils/interface_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-25 15:31:22.000000 ign-gpao-utils-0.0.2/gpao_utils/utils_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:26.540844 ign-gpao-utils-0.0.2/ign_gpao_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-25 15:31:26.000000 ign-gpao-utils-0.0.2/ign_gpao_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-25 15:31:26.000000 ign-gpao-utils-0.0.2/ign_gpao_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:31:26.000000 ign-gpao-utils-0.0.2/ign_gpao_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 15:31:26.000000 ign-gpao-utils-0.0.2/ign_gpao_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:31:26.540844 ign-gpao-utils-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-25 15:31:22.000000 ign-gpao-utils-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:26.540844 ign-gpao-utils-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-25 15:31:22.000000 ign-gpao-utils-0.0.2/test/test_utils_store.py
```

### Comparing `ign-gpao-utils-0.0.1/setup.py` & `ign-gpao-utils-0.0.2/setup.py`

 * *Files identical despite different names*

