# Comparing `tmp/datacrunch-1.2.0.tar.gz` & `tmp/datacrunch-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datacrunch-1.2.0.tar", last modified: Mon Apr 24 15:02:00 2023, max compression
+gzip compressed data, was "datacrunch-1.3.0.tar", last modified: Thu May 25 13:47:42 2023, max compression
```

## Comparing `datacrunch-1.2.0.tar` & `datacrunch-1.3.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 15:01:48.000000 datacrunch-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-24 15:02:00.991226 datacrunch-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-24 15:01:48.000000 datacrunch-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.987226 datacrunch-1.2.0/datacrunch/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.987226 datacrunch-1.2.0/datacrunch/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/authentication/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.987226 datacrunch-1.2.0/datacrunch/balance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/balance/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/datacrunch.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.987226 datacrunch-1.2.0/datacrunch/http_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/http_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/http_client/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.987226 datacrunch-1.2.0/datacrunch/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/images/images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.987226 datacrunch-1.2.0/datacrunch/instance_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/instance_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/instance_types/instance_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.987226 datacrunch-1.2.0/datacrunch/instances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/instances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/instances/instances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.987226 datacrunch-1.2.0/datacrunch/ssh_keys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/ssh_keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/ssh_keys/ssh_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/datacrunch/startup_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/startup_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/startup_scripts/startup_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/datacrunch/volume_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/volume_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/volume_types/volume_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/datacrunch/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/volumes/volumes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.987226 datacrunch-1.2.0/datacrunch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-24 15:02:00.000000 datacrunch-1.2.0/datacrunch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-24 15:02:00.000000 datacrunch-1.2.0/datacrunch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:02:00.000000 datacrunch-1.2.0/datacrunch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-24 15:02:00.000000 datacrunch-1.2.0/datacrunch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 15:02:00.000000 datacrunch-1.2.0/datacrunch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 15:02:00.991226 datacrunch-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-24 15:01:48.000000 datacrunch-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/authentication/test_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/balance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/balance/test_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/http_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/http_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/http_client/test_http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/images/test_images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/instance_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/instance_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/instance_types/test_instance_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/instances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/instances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/instances/test_instances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/ssh_keys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/ssh_keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/ssh_keys/test_ssh_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/startup_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/startup_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/startup_scripts/test_startup_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/test_datacrunch.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/test_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/volume_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/volume_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/volume_types/test_volume_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15235 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/volumes/test_volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.132008 datacrunch-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-25 13:47:28.000000 datacrunch-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-05-25 13:47:42.132008 datacrunch-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-25 13:47:28.000000 datacrunch-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.124008 datacrunch-1.3.0/datacrunch/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.124008 datacrunch-1.3.0/datacrunch/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/authentication/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.124008 datacrunch-1.3.0/datacrunch/balance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/balance/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/datacrunch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.124008 datacrunch-1.3.0/datacrunch/http_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/http_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/http_client/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/datacrunch/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/images/images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/datacrunch/instance_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/instance_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/instance_types/instance_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/datacrunch/instances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/instances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/instances/instances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/datacrunch/ssh_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/ssh_keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/ssh_keys/ssh_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/datacrunch/startup_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/startup_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/startup_scripts/startup_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/datacrunch/volume_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/volume_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/volume_types/volume_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/datacrunch/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/volumes/volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.124008 datacrunch-1.3.0/datacrunch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-05-25 13:47:42.000000 datacrunch-1.3.0/datacrunch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-25 13:47:42.000000 datacrunch-1.3.0/datacrunch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:47:42.000000 datacrunch-1.3.0/datacrunch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 13:47:42.000000 datacrunch-1.3.0/datacrunch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 13:47:42.000000 datacrunch-1.3.0/datacrunch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:47:42.132008 datacrunch-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-25 13:47:28.000000 datacrunch-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/tests/unit_tests/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/authentication/test_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/tests/unit_tests/balance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/balance/test_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/tests/unit_tests/http_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/http_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/http_client/test_http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/tests/unit_tests/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/images/test_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.132008 datacrunch-1.3.0/tests/unit_tests/instance_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/instance_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/instance_types/test_instance_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.132008 datacrunch-1.3.0/tests/unit_tests/instances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/instances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/instances/test_instances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.132008 datacrunch-1.3.0/tests/unit_tests/ssh_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/ssh_keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/ssh_keys/test_ssh_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.132008 datacrunch-1.3.0/tests/unit_tests/startup_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/startup_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/startup_scripts/test_startup_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/test_datacrunch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/test_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.132008 datacrunch-1.3.0/tests/unit_tests/volume_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/volume_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/volume_types/test_volume_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.132008 datacrunch-1.3.0/tests/unit_tests/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20505 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/volumes/test_volumes.py
```

### Comparing `datacrunch-1.2.0/LICENSE` & `datacrunch-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/PKG-INFO` & `datacrunch-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacrunch
-Version: 1.2.0
+Version: 1.3.0
 Summary: Official Python SDK for DataCrunch Public API
 Home-page: https://github.com/DataCrunch-io
 Author: DataCrunch Oy
 Author-email: info@datacrunch.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datacrunch Version: 1.2.0 Summary: Official Python
+Metadata-Version: 2.1 Name: datacrunch Version: 1.3.0 Summary: Official Python
 SDK for DataCrunch Public API Home-page: https://github.com/DataCrunch-io
 Author: DataCrunch Oy Author-email: info@datacrunch.io Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Development Status :: 5 - Production/
```

### Comparing `datacrunch-1.2.0/README.md` & `datacrunch-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/datacrunch/authentication/authentication.py` & `datacrunch-1.3.0/datacrunch/authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/datacrunch/balance/balance.py` & `datacrunch-1.3.0/datacrunch/balance/balance.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/datacrunch/constants.py` & `datacrunch-1.3.0/datacrunch/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 class VolumeActions:
     ATTACH = 'attach'
     DETACH = 'detach'
     RENAME = 'rename'
     INCREASE_SIZE = 'increase-size'
     DELETE = 'delete'
+    CLONE = 'clone'
 
     def __init__(self):
         return
 
 
 class InstanceStatus:
     RUNNING = 'running'
@@ -36,14 +37,15 @@
 class VolumeStatus:
     ORDERED = "ordered"
     CREATING = "creating"
     ATTACHED = "attached"
     DETACHED = "detached"
     DELETING = "deleting"
     DELETED = "deleted"
+    CLONING = 'cloning'
 
     def __init__(self):
         return
 
 
 class VolumeTypes:
     NVMe = "NVMe"
```

### Comparing `datacrunch-1.2.0/datacrunch/datacrunch.py` & `datacrunch-1.3.0/datacrunch/datacrunch.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/datacrunch/exceptions.py` & `datacrunch-1.3.0/datacrunch/exceptions.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/datacrunch/helpers.py` & `datacrunch-1.3.0/datacrunch/helpers.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/datacrunch/http_client/http_client.py` & `datacrunch-1.3.0/datacrunch/http_client/http_client.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/datacrunch/images/images.py` & `datacrunch-1.3.0/datacrunch/images/images.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/datacrunch/instance_types/instance_types.py` & `datacrunch-1.3.0/datacrunch/instance_types/instance_types.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/datacrunch/instances/instances.py` & `datacrunch-1.3.0/datacrunch/instances/instances.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/datacrunch/ssh_keys/ssh_keys.py` & `datacrunch-1.3.0/datacrunch/ssh_keys/ssh_keys.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/datacrunch/startup_scripts/startup_scripts.py` & `datacrunch-1.3.0/datacrunch/startup_scripts/startup_scripts.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/datacrunch/volume_types/volume_types.py` & `datacrunch-1.3.0/datacrunch/volume_types/volume_types.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/datacrunch/volumes/volumes.py` & `datacrunch-1.3.0/datacrunch/volumes/volumes.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         :param location: datacenter location, defaults to "FIN1"
         :type location: str, optional
         :param instance_id: the instance id the volume is attached to, None if detached
         :type instance_id: str
         :param ssh_key_ids: list of ssh keys ids
         :type ssh_key_ids: List[str]
         """
-
         self._id = id
         self._status = status
         self._name = name
         self._size = size
         self._type = type
         self._is_os_volume = is_os_volume
         self._created_at = created_at
@@ -162,14 +161,15 @@
         """Returns a string of the json representation of the volume
 
         :return: json representation of the volume
         :rtype: str
         """
         return stringify_class_object_properties(self)
 
+
 class VolumesService:
     """A service for interacting with the volumes endpoint"""
 
     def __init__(self, http_client) -> None:
         self._http_client = http_client
 
     def get(self, status: str = None) -> List[Volume]:
@@ -189,15 +189,16 @@
             size=volume_dict['size'],
             type=volume_dict['type'],
             is_os_volume=volume_dict['is_os_volume'],
             created_at=volume_dict['created_at'],
             target=volume_dict['target'] if 'target' in volume_dict else None,
             location=volume_dict['location'],
             instance_id=volume_dict['instance_id'] if 'instance_id' in volume_dict else None,
-            ssh_key_ids=volume_dict['ssh_key_ids'] if 'ssh_key_ids' in volume_dict else [],
+            ssh_key_ids=volume_dict['ssh_key_ids'] if 'ssh_key_ids' in volume_dict else [
+            ],
         ), volumes_dict))
         return volumes
 
     def get_by_id(self, id: str) -> Volume:
         """Get a specific volume by its
 
         :param id: volume id
@@ -214,15 +215,16 @@
             size=volume_dict['size'],
             type=volume_dict['type'],
             is_os_volume=volume_dict['is_os_volume'],
             created_at=volume_dict['created_at'],
             target=volume_dict['target'] if 'target' in volume_dict else None,
             location=volume_dict['location'],
             instance_id=volume_dict['instance_id'] if 'instance_id' in volume_dict else None,
-            ssh_key_ids=volume_dict['ssh_key_ids'] if 'ssh_key_ids' in volume_dict else [],
+            ssh_key_ids=volume_dict['ssh_key_ids'] if 'ssh_key_ids' in volume_dict else [
+            ],
         )
         return volume
 
     def create(self,
                type: str,
                name: str,
                size: int,
@@ -284,14 +286,48 @@
             "id": id_list,
             "action": VolumeActions.DETACH,
         }
 
         self._http_client.put(VOLUMES_ENDPOINT, json=payload)
         return
 
+    def clone(self, id: str, name: str = None, type: str = None) -> Volume:
+        """Clone a volume or multiple volumes
+
+        :param id: volume id or list of volume ids
+        :type id: str or List[str]
+        :param name: new volume name
+        :type name: str
+        :param type: volume type
+        :type type: str, optional
+        :return: the new volume object, or a list of volume objects if cloned mutliple volumes
+        :rtype: Volume or List[Volume]
+        """
+        payload = {
+            "id": id,
+            "action": VolumeActions.CLONE,
+            "name": name,
+            "type": type
+        }
+
+        # clone volume(s)
+        volume_ids_array = self._http_client.put(
+            VOLUMES_ENDPOINT, json=payload).json()
+
+        # map the IDs into Volume objects
+        volumes_array = list(
+            map(lambda volume_id: self.get_by_id(volume_id), volume_ids_array))
+
+        # if the array has only one element, return that element
+        if len(volumes_array) == 1:
+            return volumes_array[0]
+
+        # otherwise return the volumes array
+        return volumes_array
+
     def rename(self, id_list: Union[List[str], str], name: str) -> None:
         """Rename multiple volumes or single volume
 
         :param id_list: list of volume ids, or a volume id
         :type id_list: Union[List[str], str]
         :param name: new name
         :type name: str
```

### Comparing `datacrunch-1.2.0/datacrunch.egg-info/PKG-INFO` & `datacrunch-1.3.0/datacrunch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacrunch
-Version: 1.2.0
+Version: 1.3.0
 Summary: Official Python SDK for DataCrunch Public API
 Home-page: https://github.com/DataCrunch-io
 Author: DataCrunch Oy
 Author-email: info@datacrunch.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datacrunch Version: 1.2.0 Summary: Official Python
+Metadata-Version: 2.1 Name: datacrunch Version: 1.3.0 Summary: Official Python
 SDK for DataCrunch Public API Home-page: https://github.com/DataCrunch-io
 Author: DataCrunch Oy Author-email: info@datacrunch.io Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Development Status :: 5 - Production/
```

### Comparing `datacrunch-1.2.0/datacrunch.egg-info/SOURCES.txt` & `datacrunch-1.3.0/datacrunch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/setup.py` & `datacrunch-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/tests/unit_tests/authentication/test_authentication.py` & `datacrunch-1.3.0/tests/unit_tests/authentication/test_authentication.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/tests/unit_tests/balance/test_balance.py` & `datacrunch-1.3.0/tests/unit_tests/balance/test_balance.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/tests/unit_tests/conftest.py` & `datacrunch-1.3.0/tests/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/tests/unit_tests/http_client/test_http_client.py` & `datacrunch-1.3.0/tests/unit_tests/http_client/test_http_client.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/tests/unit_tests/images/test_images.py` & `datacrunch-1.3.0/tests/unit_tests/images/test_images.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/tests/unit_tests/instance_types/test_instance_types.py` & `datacrunch-1.3.0/tests/unit_tests/instance_types/test_instance_types.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/tests/unit_tests/instances/test_instances.py` & `datacrunch-1.3.0/tests/unit_tests/instances/test_instances.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/tests/unit_tests/ssh_keys/test_ssh_keys.py` & `datacrunch-1.3.0/tests/unit_tests/ssh_keys/test_ssh_keys.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/tests/unit_tests/startup_scripts/test_startup_scripts.py` & `datacrunch-1.3.0/tests/unit_tests/startup_scripts/test_startup_scripts.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/tests/unit_tests/test_datacrunch.py` & `datacrunch-1.3.0/tests/unit_tests/test_datacrunch.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/tests/unit_tests/test_exceptions.py` & `datacrunch-1.3.0/tests/unit_tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/tests/unit_tests/volume_types/test_volume_types.py` & `datacrunch-1.3.0/tests/unit_tests/volume_types/test_volume_types.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.2.0/tests/unit_tests/volumes/test_volumes.py` & `datacrunch-1.3.0/tests/unit_tests/volumes/test_volumes.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
 HDD_VOL_ID = "ea4edc62-9838-4b7c-bd5b-862f2efec675"
 HDD_VOL_STATUS = VolumeStatus.DETACHED
 HDD_VOL_NAME = "Volume-iHdL4ysR"
 HDD_VOL_SIZE = 100
 HDD_VOL_CREATED_AT = "2021-06-02T12:56:49.582Z"
 
+RANDOM_VOL_ID = '07d864ee-ba86-451e-85b3-34ef551bd4a2'
+RANDOM_VOL2_ID = '72c5c082-7fe7-4d13-bd9e-f529c97d63b3'
+
 NVME_VOLUME = {
     "id": NVME_VOL_ID,
     "status": NVME_VOL_STATUS,
     "instance_id": INSTANCE_ID,
     "name": NVME_VOL_NAME,
     "size": NVME_VOL_SIZE,
     "type": NVME,
@@ -65,15 +68,31 @@
     def volumes_service(self, http_client):
         return VolumesService(http_client)
 
     @pytest.fixture
     def endpoint(self, http_client):
         return http_client._base_url + "/volumes"
 
-    def test_get_instances(self, volumes_service, endpoint):
+    def test_initialize_a_volume(self):
+        volume = Volume(RANDOM_VOL_ID, VolumeStatus.DETACHED, HDD_VOL_NAME, HDD_VOL_SIZE,
+                        HDD, False, HDD_VOL_CREATED_AT)
+
+        assert volume.id == RANDOM_VOL_ID
+        assert volume.status == VolumeStatus.DETACHED
+        assert volume.instance_id == None
+        assert volume.name == HDD_VOL_NAME
+        assert volume.size == HDD_VOL_SIZE
+        assert volume.type == HDD
+        assert volume.location == FIN1
+        assert volume.is_os_volume == False
+        assert volume.created_at == HDD_VOL_CREATED_AT
+        assert volume.target == None
+        assert volume.ssh_key_ids == []
+
+    def test_get_volumes(self, volumes_service, endpoint):
         # arrange - add response mock
         responses.add(
             responses.GET,
             endpoint,
             json=PAYLOAD,
             status=200
         )
@@ -215,15 +234,16 @@
             responses.GET,
             endpoint + "/" + NVME_VOL_ID,
             json=NVME_VOLUME,
             status=200
         )
 
         # act
-        volume = volumes_service.create(VolumeTypes.NVMe, NVME_VOL_NAME, NVME_VOL_SIZE)
+        volume = volumes_service.create(
+            VolumeTypes.NVMe, NVME_VOL_NAME, NVME_VOL_SIZE)
 
         # assert
         assert volume.id == NVME_VOL_ID
         assert type(volume.__str__()) == str
 
     def test_create_volume_failed(self, volumes_service, endpoint):
         # arrange - add response mock
@@ -232,15 +252,16 @@
             endpoint,
             json={"code": INVALID_REQUEST, "message": INVALID_REQUEST_MESSAGE},
             status=400
         )
 
         # act
         with pytest.raises(APIException) as excinfo:
-            volumes_service.create(VolumeTypes.NVMe, NVME_VOL_NAME, 100000000000000000000000)
+            volumes_service.create(
+                VolumeTypes.NVMe, NVME_VOL_NAME, 100000000000000000000000)
 
         # assert
         assert excinfo.value.code == INVALID_REQUEST
         assert excinfo.value.message == INVALID_REQUEST_MESSAGE
         assert responses.assert_call_count(endpoint, 1) is True
 
     def test_attach_volume_successful(self, volumes_service, endpoint):
@@ -477,7 +498,143 @@
         with pytest.raises(APIException) as excinfo:
             volumes_service.delete(NVME_VOL_ID)
 
         # assert
         assert excinfo.value.code == INVALID_REQUEST
         assert excinfo.value.message == INVALID_REQUEST_MESSAGE
         assert responses.assert_call_count(endpoint, 1) is True
+
+    def test_clone_volume_with_input_name_successful(self, volumes_service, endpoint):
+        # arrange
+        CLONED_VOLUME_NAME = "cloned-volume"
+
+        # mock response for cloning the volume
+        responses.add(
+            responses.PUT,
+            endpoint,
+            status=202,
+            json=[RANDOM_VOL_ID],
+            match=[
+                responses.json_params_matcher({
+                    "id": NVME_VOL_ID,
+                    "action": VolumeActions.CLONE,
+                    "name": CLONED_VOLUME_NAME,
+                    "type": None
+                })
+            ]
+        )
+
+        # mock object for the cloned volume
+        CLONED_VOL_GET_MOCK = NVME_VOLUME
+        CLONED_VOL_GET_MOCK['id'] = RANDOM_VOL_ID
+        CLONED_VOL_GET_MOCK['name'] = CLONED_VOLUME_NAME
+        CLONED_VOL_GET_MOCK['status'] = VolumeStatus.CLONING
+
+        # mock response for getting the cloned volume
+        responses.add(
+            responses.GET,
+            endpoint + "/" + RANDOM_VOL_ID,
+            status=200,
+            json=CLONED_VOL_GET_MOCK,
+        )
+
+        # act
+        cloned_volume = volumes_service.clone(NVME_VOL_ID, CLONED_VOLUME_NAME)
+
+        # assert
+        assert responses.assert_call_count(endpoint, 1) is True
+        assert cloned_volume.name == CLONED_VOLUME_NAME
+
+    def test_clone_volume_without_input_name_successful(self, volumes_service: VolumesService, endpoint):
+        # arrange
+        CLONED_VOLUME_NAME = "CLONE-" + NVME_VOL_NAME
+
+        # mock response for cloning the volume
+        responses.add(
+            responses.PUT,
+            endpoint,
+            status=202,
+            json=[RANDOM_VOL_ID],
+            match=[
+                responses.json_params_matcher({
+                    "id": NVME_VOL_ID,
+                    "action": VolumeActions.CLONE,
+                    "name": None,
+                    "type": None
+                })
+            ]
+        )
+
+        # mock object for the cloned volume
+        CLONED_VOL_GET_MOCK = NVME_VOLUME
+        CLONED_VOL_GET_MOCK['id'] = RANDOM_VOL_ID
+        CLONED_VOL_GET_MOCK['name'] = CLONED_VOLUME_NAME
+        CLONED_VOL_GET_MOCK['status'] = VolumeStatus.CLONING
+
+        # mock response for getting the cloned volume
+        responses.add(
+            responses.GET,
+            endpoint + "/" + RANDOM_VOL_ID,
+            status=200,
+            json=CLONED_VOL_GET_MOCK,
+        )
+
+        # act
+        cloned_volume = volumes_service.clone(NVME_VOL_ID)
+
+        # assert
+        assert responses.assert_call_count(endpoint, 1) is True
+        assert cloned_volume.name == CLONED_VOLUME_NAME
+
+    def test_clone_two_volumes_successful(self, volumes_service: VolumesService, endpoint):
+        # arrange
+        CLONED_VOL1_NAME = "CLONE-" + NVME_VOL_NAME
+        CLONED_VOL2_NAME = "CLONE-" + HDD_VOL_NAME
+
+        # mock response for cloning the volumes
+        responses.add(
+            responses.PUT,
+            endpoint,
+            status=202,
+            json=[RANDOM_VOL_ID, RANDOM_VOL2_ID],
+            match=[
+                responses.json_params_matcher({
+                    "id": [NVME_VOL_ID, HDD_VOL_ID],
+                    "action": VolumeActions.CLONE,
+                    "name": None,
+                    "type": None
+                })
+            ]
+        )
+
+        # mock object for the cloned volumes
+        CLONED_VOL1_GET_MOCK = NVME_VOLUME
+        CLONED_VOL1_GET_MOCK['id'] = RANDOM_VOL_ID
+        CLONED_VOL1_GET_MOCK['name'] = CLONED_VOL1_NAME
+        CLONED_VOL1_GET_MOCK['status'] = VolumeStatus.CLONING
+
+        CLONED_VOL2_GET_MOCK = HDD_VOLUME
+        CLONED_VOL2_GET_MOCK['id'] = RANDOM_VOL2_ID
+        CLONED_VOL2_GET_MOCK['name'] = CLONED_VOL2_NAME
+        CLONED_VOL2_GET_MOCK['status'] = VolumeStatus.CLONING
+
+        # mock response for getting the cloned volumes
+        responses.add(
+            responses.GET,
+            endpoint + "/" + RANDOM_VOL_ID,
+            status=200,
+            json=CLONED_VOL1_GET_MOCK,
+        )
+        responses.add(
+            responses.GET,
+            endpoint + "/" + RANDOM_VOL2_ID,
+            status=200,
+            json=CLONED_VOL2_GET_MOCK,
+        )
+
+        # act
+        cloned_volume = volumes_service.clone([NVME_VOL_ID, HDD_VOL_ID])
+
+        # assert
+        assert responses.assert_call_count(endpoint, 1) is True
+        assert cloned_volume[0].name == CLONED_VOL1_NAME
+        assert cloned_volume[1].name == CLONED_VOL2_NAME
```

