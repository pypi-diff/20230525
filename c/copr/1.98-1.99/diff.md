# Comparing `tmp/copr-1.98.tar.gz` & `tmp/copr-1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/copr-1.98.tar", last modified: Thu Oct  3 07:52:16 2019, max compression
+gzip compressed data, was "dist/copr-1.99.tar", last modified: Wed Dec  4 13:31:22 2019, max compression
```

## Comparing `copr-1.98.tar` & `copr-1.99.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-10-03 07:52:16.000000 copr-1.98/
--rw-rw-r--   0 twine    (17125) twine    (17125)    18092 2019-07-17 08:59:09.000000 copr-1.98/LICENSE
--rw-rw-r--   0 twine    (17125) twine    (17125)      252 2019-07-24 12:55:25.000000 copr-1.98/MANIFEST.in
--rw-rw-r--   0 twine    (17125) twine    (17125)      989 2019-10-03 07:52:16.000000 copr-1.98/PKG-INFO
-drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-10-03 07:52:16.000000 copr-1.98/copr/
--rw-rw-r--   0 twine    (17125) twine    (17125)     1411 2019-07-17 08:59:09.000000 copr-1.98/copr/README.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)      210 2019-07-17 08:59:09.000000 copr-1.98/copr/__init__.py
-drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-10-03 07:52:16.000000 copr-1.98/copr/client/
--rw-rw-r--   0 twine    (17125) twine    (17125)      179 2019-07-17 08:59:09.000000 copr-1.98/copr/client/__init__.py
--rw-rw-r--   0 twine    (17125) twine    (17125)    67334 2019-07-17 08:59:09.000000 copr-1.98/copr/client/client.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     7108 2019-07-17 08:59:09.000000 copr-1.98/copr/client/parsers.py
--rw-rw-r--   0 twine    (17125) twine    (17125)    11754 2019-07-17 08:59:09.000000 copr-1.98/copr/client/responses.py
-drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-10-03 07:52:16.000000 copr-1.98/copr/client_v2/
--rw-rw-r--   0 twine    (17125) twine    (17125)       16 2019-07-17 08:59:09.000000 copr-1.98/copr/client_v2/__init__.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     7658 2019-07-17 08:59:09.000000 copr-1.98/copr/client_v2/client.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     1157 2019-07-17 08:59:09.000000 copr-1.98/copr/client_v2/common.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     2874 2019-09-26 07:28:10.000000 copr-1.98/copr/client_v2/entities.py
--rw-rw-r--   0 twine    (17125) twine    (17125)    18933 2019-07-17 08:59:09.000000 copr-1.98/copr/client_v2/handlers.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     6133 2019-07-17 08:59:09.000000 copr-1.98/copr/client_v2/net_client.py
--rw-rw-r--   0 twine    (17125) twine    (17125)    20675 2019-09-26 07:28:10.000000 copr-1.98/copr/client_v2/resources.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     2830 2019-07-17 08:59:09.000000 copr-1.98/copr/client_v2/schemas.py
--rw-rw-r--   0 twine    (17125) twine    (17125)      543 2019-07-17 08:59:09.000000 copr-1.98/copr/client_v2/tools.py
--rw-rw-r--   0 twine    (17125) twine    (17125)      926 2019-07-17 08:59:09.000000 copr-1.98/copr/exceptions.py
-drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-10-03 07:52:16.000000 copr-1.98/copr/test/
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-07-17 08:59:09.000000 copr-1.98/copr/test/__init__.py
-drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-10-03 07:52:16.000000 copr-1.98/copr/test/client_v2/
--rw-rw-r--   0 twine    (17125) twine    (17125)     2703 2019-07-17 08:59:09.000000 copr-1.98/copr/test/client_v2/test_client.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     1043 2019-09-26 07:28:10.000000 copr-1.98/copr/test/client_v2/test_entities.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     7473 2019-09-26 07:28:10.000000 copr-1.98/copr/test/client_v2/test_handlers.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     1806 2019-07-17 08:59:09.000000 copr-1.98/copr/test/client_v2/test_net_client.py
-drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-10-03 07:52:16.000000 copr-1.98/copr/test/client_v3/
--rw-rw-r--   0 twine    (17125) twine    (17125)      537 2019-07-17 08:59:09.000000 copr-1.98/copr/test/client_v3/test_builds.py
--rw-rw-r--   0 twine    (17125) twine    (17125)      397 2019-07-17 08:59:09.000000 copr-1.98/copr/test/client_v3/test_general.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     2320 2019-07-17 08:59:09.000000 copr-1.98/copr/test/client_v3/test_helpers.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     1367 2019-07-17 08:59:09.000000 copr-1.98/copr/test/client_v3/test_requests.py
-drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-10-03 07:52:16.000000 copr-1.98/copr/test/resources/
--rw-rw-r--   0 twine    (17125) twine    (17125)      666 2019-07-17 08:59:09.000000 copr-1.98/copr/test/resources/build_details.200.json
--rw-rw-r--   0 twine    (17125) twine    (17125)      140 2019-07-17 08:59:09.000000 copr-1.98/copr/test/resources/copr_cli.conf
--rw-rw-r--   0 twine    (17125) twine    (17125)      344 2019-07-17 08:59:09.000000 copr-1.98/copr/test/resources/projects_list.200.json
--rw-rw-r--   0 twine    (17125) twine    (17125)     2374 2019-07-17 08:59:09.000000 copr-1.98/copr/test/test_client.py
--rw-rw-r--   0 twine    (17125) twine    (17125)      375 2019-07-17 08:59:09.000000 copr-1.98/copr/test/test_resources.py
--rw-rw-r--   0 twine    (17125) twine    (17125)      464 2019-07-17 08:59:09.000000 copr-1.98/copr/util.py
-drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-10-03 07:52:16.000000 copr-1.98/copr/v3/
--rw-rw-r--   0 twine    (17125) twine    (17125)     1000 2019-07-17 08:59:09.000000 copr-1.98/copr/v3/__init__.py
--rw-rw-r--   0 twine    (17125) twine    (17125)      916 2019-07-17 08:59:09.000000 copr-1.98/copr/v3/client.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     1011 2019-07-17 08:59:09.000000 copr-1.98/copr/v3/exceptions.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     4309 2019-07-17 08:59:09.000000 copr-1.98/copr/v3/helpers.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     1156 2019-07-17 08:59:09.000000 copr-1.98/copr/v3/pagination.py
-drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-10-03 07:52:16.000000 copr-1.98/copr/v3/proxies/
--rw-rw-r--   0 twine    (17125) twine    (17125)     1284 2019-07-17 08:59:09.000000 copr-1.98/copr/v3/proxies/__init__.py
--rw-rw-r--   0 twine    (17125) twine    (17125)    10186 2019-07-17 08:59:09.000000 copr-1.98/copr/v3/proxies/build.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     1728 2019-07-17 08:59:09.000000 copr-1.98/copr/v3/proxies/build_chroot.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     1748 2019-07-17 08:59:09.000000 copr-1.98/copr/v3/proxies/module.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     5619 2019-07-17 08:59:09.000000 copr-1.98/copr/v3/proxies/package.py
--rw-rw-r--   0 twine    (17125) twine    (17125)    11206 2019-09-26 07:28:10.000000 copr-1.98/copr/v3/proxies/project.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     3032 2019-07-17 08:59:09.000000 copr-1.98/copr/v3/proxies/project_chroot.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     3543 2019-07-17 08:59:09.000000 copr-1.98/copr/v3/requests.py
-drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-10-03 07:52:16.000000 copr-1.98/copr.egg-info/
--rw-rw-r--   0 twine    (17125) twine    (17125)      989 2019-10-03 07:52:16.000000 copr-1.98/copr.egg-info/PKG-INFO
--rw-rw-r--   0 twine    (17125) twine    (17125)     2408 2019-10-03 07:52:16.000000 copr-1.98/copr.egg-info/SOURCES.txt
--rw-rw-r--   0 twine    (17125) twine    (17125)        1 2019-10-03 07:52:16.000000 copr-1.98/copr.egg-info/dependency_links.txt
--rw-rw-r--   0 twine    (17125) twine    (17125)        1 2019-07-30 08:22:08.000000 copr-1.98/copr.egg-info/not-zip-safe
--rw-rw-r--   0 twine    (17125) twine    (17125)       49 2019-10-03 07:52:16.000000 copr-1.98/copr.egg-info/requires.txt
--rw-rw-r--   0 twine    (17125) twine    (17125)        5 2019-10-03 07:52:16.000000 copr-1.98/copr.egg-info/top_level.txt
-drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-10-03 07:52:16.000000 copr-1.98/docs/
--rw-rw-r--   0 twine    (17125) twine    (17125)      690 2019-07-17 08:59:09.000000 copr-1.98/docs/ClientV1.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)     1106 2019-07-17 08:59:09.000000 copr-1.98/docs/ClientV2.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)     1417 2019-07-17 08:59:09.000000 copr-1.98/docs/ClientV3.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)     5584 2019-07-17 08:59:09.000000 copr-1.98/docs/Makefile
--rw-rw-r--   0 twine    (17125) twine    (17125)      318 2019-07-17 08:59:09.000000 copr-1.98/docs/README.txt
-drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-10-03 07:52:16.000000 copr-1.98/docs/client_v1/
--rw-rw-r--   0 twine    (17125) twine    (17125)      355 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v1/CoprClient.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)     2809 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v1/Examples.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)      585 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v1/Responses.rst
-drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-10-03 07:52:16.000000 copr-1.98/docs/client_v2/
--rw-rw-r--   0 twine    (17125) twine    (17125)      231 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v2/entities.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)       51 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v2/errors.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)      335 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v2/general.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)      473 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v2/handlers.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)      368 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v2/initialization.rst
-drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-10-03 07:52:16.000000 copr-1.98/docs/client_v2/resource_info/
--rw-rw-r--   0 twine    (17125) twine    (17125)     3541 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v2/resource_info/build.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)     3607 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v2/resource_info/build_task.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)     2127 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v2/resource_info/mock_chroot.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)     4377 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v2/resource_info/project.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)     2847 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v2/resource_info/project_chroot.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)     1166 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v2/resources.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)     1958 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v2/resources_usage.rst
-drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-10-03 07:52:16.000000 copr-1.98/docs/client_v3/
--rw-rw-r--   0 twine    (17125) twine    (17125)     1040 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v3/build_options.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)     1760 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v3/client_initialization.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)     6030 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v3/data_structures.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)     2322 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v3/error_handling.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)     9285 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v3/migration.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)     2625 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v3/package_source_types.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)     3331 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v3/pagination.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)     1454 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v3/proxies.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)      757 2019-07-17 08:59:09.000000 copr-1.98/docs/client_v3/working_with_proxies_directly.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)     8357 2019-07-17 08:59:09.000000 copr-1.98/docs/conf.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     1244 2019-07-17 08:59:09.000000 copr-1.98/docs/index.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)      380 2019-07-17 08:59:09.000000 copr-1.98/docs/installation.rst
--rw-rw-r--   0 twine    (17125) twine    (17125)    35710 2019-10-03 07:51:43.000000 copr-1.98/python-copr.spec
--rw-rw-r--   0 twine    (17125) twine    (17125)      126 2019-07-17 08:59:09.000000 copr-1.98/requirements.txt
--rwxrwxr-x   0 twine    (17125) twine    (17125)      146 2019-09-26 07:28:10.000000 copr-1.98/run_tests.sh
--rw-rw-r--   0 twine    (17125) twine    (17125)       38 2019-10-03 07:52:16.000000 copr-1.98/setup.cfg
--rw-rw-r--   0 twine    (17125) twine    (17125)     1453 2019-10-03 07:51:43.000000 copr-1.98/setup.py
+drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-12-04 13:31:22.000000 copr-1.99/
+-rw-rw-r--   0 twine    (17125) twine    (17125)    18092 2019-07-17 08:59:09.000000 copr-1.99/LICENSE
+-rw-rw-r--   0 twine    (17125) twine    (17125)      252 2019-07-24 12:55:25.000000 copr-1.99/MANIFEST.in
+-rw-rw-r--   0 twine    (17125) twine    (17125)      989 2019-12-04 13:31:22.000000 copr-1.99/PKG-INFO
+drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-12-04 13:31:22.000000 copr-1.99/copr/
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1411 2019-07-17 08:59:09.000000 copr-1.99/copr/README.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)      210 2019-07-17 08:59:09.000000 copr-1.99/copr/__init__.py
+drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-12-04 13:31:22.000000 copr-1.99/copr/client/
+-rw-rw-r--   0 twine    (17125) twine    (17125)      179 2019-07-17 08:59:09.000000 copr-1.99/copr/client/__init__.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)    67334 2019-07-17 08:59:09.000000 copr-1.99/copr/client/client.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     7108 2019-07-17 08:59:09.000000 copr-1.99/copr/client/parsers.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)    11754 2019-07-17 08:59:09.000000 copr-1.99/copr/client/responses.py
+drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-12-04 13:31:22.000000 copr-1.99/copr/client_v2/
+-rw-rw-r--   0 twine    (17125) twine    (17125)       16 2019-07-17 08:59:09.000000 copr-1.99/copr/client_v2/__init__.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     7658 2019-07-17 08:59:09.000000 copr-1.99/copr/client_v2/client.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1157 2019-07-17 08:59:09.000000 copr-1.99/copr/client_v2/common.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     2874 2019-09-26 07:28:10.000000 copr-1.99/copr/client_v2/entities.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)    18933 2019-07-17 08:59:09.000000 copr-1.99/copr/client_v2/handlers.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     6133 2019-07-17 08:59:09.000000 copr-1.99/copr/client_v2/net_client.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)    20675 2019-09-26 07:28:10.000000 copr-1.99/copr/client_v2/resources.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     2830 2019-07-17 08:59:09.000000 copr-1.99/copr/client_v2/schemas.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)      543 2019-07-17 08:59:09.000000 copr-1.99/copr/client_v2/tools.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)      926 2019-07-17 08:59:09.000000 copr-1.99/copr/exceptions.py
+drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-12-04 13:31:22.000000 copr-1.99/copr/test/
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-07-17 08:59:09.000000 copr-1.99/copr/test/__init__.py
+drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-12-04 13:31:22.000000 copr-1.99/copr/test/client_v2/
+-rw-rw-r--   0 twine    (17125) twine    (17125)     2703 2019-07-17 08:59:09.000000 copr-1.99/copr/test/client_v2/test_client.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1043 2019-09-26 07:28:10.000000 copr-1.99/copr/test/client_v2/test_entities.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     7473 2019-09-26 07:28:10.000000 copr-1.99/copr/test/client_v2/test_handlers.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1806 2019-07-17 08:59:09.000000 copr-1.99/copr/test/client_v2/test_net_client.py
+drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-12-04 13:31:22.000000 copr-1.99/copr/test/client_v3/
+-rw-rw-r--   0 twine    (17125) twine    (17125)      537 2019-07-17 08:59:09.000000 copr-1.99/copr/test/client_v3/test_builds.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)      397 2019-07-17 08:59:09.000000 copr-1.99/copr/test/client_v3/test_general.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     2320 2019-07-17 08:59:09.000000 copr-1.99/copr/test/client_v3/test_helpers.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1367 2019-07-17 08:59:09.000000 copr-1.99/copr/test/client_v3/test_requests.py
+drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-12-04 13:31:22.000000 copr-1.99/copr/test/resources/
+-rw-rw-r--   0 twine    (17125) twine    (17125)      423 2019-12-04 13:30:26.000000 copr-1.99/copr/test/resources/build_config.200.json
+-rw-rw-r--   0 twine    (17125) twine    (17125)      666 2019-07-17 08:59:09.000000 copr-1.99/copr/test/resources/build_details.200.json
+-rw-rw-r--   0 twine    (17125) twine    (17125)      140 2019-07-17 08:59:09.000000 copr-1.99/copr/test/resources/copr_cli.conf
+-rw-rw-r--   0 twine    (17125) twine    (17125)      344 2019-07-17 08:59:09.000000 copr-1.99/copr/test/resources/projects_list.200.json
+-rw-rw-r--   0 twine    (17125) twine    (17125)     3043 2019-12-04 13:30:26.000000 copr-1.99/copr/test/test_client.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)      375 2019-07-17 08:59:09.000000 copr-1.99/copr/test/test_resources.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)      464 2019-07-17 08:59:09.000000 copr-1.99/copr/util.py
+drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-12-04 13:31:22.000000 copr-1.99/copr/v3/
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1000 2019-07-17 08:59:09.000000 copr-1.99/copr/v3/__init__.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)      916 2019-07-17 08:59:09.000000 copr-1.99/copr/v3/client.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1011 2019-07-17 08:59:09.000000 copr-1.99/copr/v3/exceptions.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     4309 2019-07-17 08:59:09.000000 copr-1.99/copr/v3/helpers.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1156 2019-07-17 08:59:09.000000 copr-1.99/copr/v3/pagination.py
+drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-12-04 13:31:22.000000 copr-1.99/copr/v3/proxies/
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1284 2019-07-17 08:59:09.000000 copr-1.99/copr/v3/proxies/__init__.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)    10186 2019-07-17 08:59:09.000000 copr-1.99/copr/v3/proxies/build.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1728 2019-07-17 08:59:09.000000 copr-1.99/copr/v3/proxies/build_chroot.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1748 2019-07-17 08:59:09.000000 copr-1.99/copr/v3/proxies/module.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     5619 2019-07-17 08:59:09.000000 copr-1.99/copr/v3/proxies/package.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)    11689 2019-12-04 13:30:26.000000 copr-1.99/copr/v3/proxies/project.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     3032 2019-07-17 08:59:09.000000 copr-1.99/copr/v3/proxies/project_chroot.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     3543 2019-07-17 08:59:09.000000 copr-1.99/copr/v3/requests.py
+drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-12-04 13:31:22.000000 copr-1.99/copr.egg-info/
+-rw-rw-r--   0 twine    (17125) twine    (17125)      989 2019-12-04 13:31:22.000000 copr-1.99/copr.egg-info/PKG-INFO
+-rw-rw-r--   0 twine    (17125) twine    (17125)     2450 2019-12-04 13:31:22.000000 copr-1.99/copr.egg-info/SOURCES.txt
+-rw-rw-r--   0 twine    (17125) twine    (17125)        1 2019-12-04 13:31:22.000000 copr-1.99/copr.egg-info/dependency_links.txt
+-rw-rw-r--   0 twine    (17125) twine    (17125)        1 2019-07-30 08:22:08.000000 copr-1.99/copr.egg-info/not-zip-safe
+-rw-rw-r--   0 twine    (17125) twine    (17125)       49 2019-12-04 13:31:22.000000 copr-1.99/copr.egg-info/requires.txt
+-rw-rw-r--   0 twine    (17125) twine    (17125)        5 2019-12-04 13:31:22.000000 copr-1.99/copr.egg-info/top_level.txt
+drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-12-04 13:31:22.000000 copr-1.99/docs/
+-rw-rw-r--   0 twine    (17125) twine    (17125)      690 2019-07-17 08:59:09.000000 copr-1.99/docs/ClientV1.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1106 2019-07-17 08:59:09.000000 copr-1.99/docs/ClientV2.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1417 2019-07-17 08:59:09.000000 copr-1.99/docs/ClientV3.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)     5584 2019-07-17 08:59:09.000000 copr-1.99/docs/Makefile
+-rw-rw-r--   0 twine    (17125) twine    (17125)      318 2019-07-17 08:59:09.000000 copr-1.99/docs/README.txt
+drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-12-04 13:31:22.000000 copr-1.99/docs/client_v1/
+-rw-rw-r--   0 twine    (17125) twine    (17125)      355 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v1/CoprClient.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)     2809 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v1/Examples.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)      585 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v1/Responses.rst
+drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-12-04 13:31:22.000000 copr-1.99/docs/client_v2/
+-rw-rw-r--   0 twine    (17125) twine    (17125)      231 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v2/entities.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)       51 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v2/errors.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)      335 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v2/general.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)      473 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v2/handlers.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)      368 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v2/initialization.rst
+drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-12-04 13:31:22.000000 copr-1.99/docs/client_v2/resource_info/
+-rw-rw-r--   0 twine    (17125) twine    (17125)     3541 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v2/resource_info/build.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)     3607 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v2/resource_info/build_task.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)     2127 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v2/resource_info/mock_chroot.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)     4377 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v2/resource_info/project.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)     2847 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v2/resource_info/project_chroot.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1166 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v2/resources.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1958 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v2/resources_usage.rst
+drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2019-12-04 13:31:22.000000 copr-1.99/docs/client_v3/
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1040 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v3/build_options.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1760 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v3/client_initialization.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)     6030 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v3/data_structures.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)     2322 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v3/error_handling.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)     9285 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v3/migration.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)     2625 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v3/package_source_types.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)     3331 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v3/pagination.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1454 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v3/proxies.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)      757 2019-07-17 08:59:09.000000 copr-1.99/docs/client_v3/working_with_proxies_directly.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)     8357 2019-07-17 08:59:09.000000 copr-1.99/docs/conf.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1244 2019-07-17 08:59:09.000000 copr-1.99/docs/index.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)      380 2019-07-17 08:59:09.000000 copr-1.99/docs/installation.rst
+-rw-rw-r--   0 twine    (17125) twine    (17125)    35845 2019-12-04 13:30:26.000000 copr-1.99/python-copr.spec
+-rw-rw-r--   0 twine    (17125) twine    (17125)      126 2019-07-17 08:59:09.000000 copr-1.99/requirements.txt
+-rwxrwxr-x   0 twine    (17125) twine    (17125)      146 2019-09-26 07:28:10.000000 copr-1.99/run_tests.sh
+-rw-rw-r--   0 twine    (17125) twine    (17125)       38 2019-12-04 13:31:22.000000 copr-1.99/setup.cfg
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1453 2019-12-04 13:30:26.000000 copr-1.99/setup.py
```

### Comparing `copr-1.98/LICENSE` & `copr-1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `copr-1.98/PKG-INFO` & `copr-1.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: copr
-Version: 1.98
+Version: 1.99
 Summary: Python client for copr service.
 Home-page: https://pagure.io/copr/copr
 Author: Valentin Gologuzov
 Author-email: vgologuz@redhat.com
 License: GPLv2+
 Description: Copr is designed to be a lightweight buildsystem that allows contributors
         to create packages, put them in repositories, and make it easy for users
```

### Comparing `copr-1.98/copr/README.rst` & `copr-1.99/copr/README.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/client/client.py` & `copr-1.99/copr/client/client.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/client/parsers.py` & `copr-1.99/copr/client/parsers.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/client/responses.py` & `copr-1.99/copr/client/responses.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/client_v2/client.py` & `copr-1.99/copr/client_v2/client.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/client_v2/common.py` & `copr-1.99/copr/client_v2/common.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/client_v2/entities.py` & `copr-1.99/copr/client_v2/entities.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/client_v2/handlers.py` & `copr-1.99/copr/client_v2/handlers.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/client_v2/net_client.py` & `copr-1.99/copr/client_v2/net_client.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/client_v2/resources.py` & `copr-1.99/copr/client_v2/resources.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/client_v2/schemas.py` & `copr-1.99/copr/client_v2/schemas.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/client_v2/tools.py` & `copr-1.99/copr/client_v2/tools.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/exceptions.py` & `copr-1.99/copr/exceptions.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/test/client_v2/test_client.py` & `copr-1.99/copr/test/client_v2/test_client.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/test/client_v2/test_entities.py` & `copr-1.99/copr/test/client_v2/test_entities.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/test/client_v2/test_handlers.py` & `copr-1.99/copr/test/client_v2/test_handlers.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/test/client_v2/test_net_client.py` & `copr-1.99/copr/test/client_v2/test_net_client.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/test/client_v3/test_builds.py` & `copr-1.99/copr/test/client_v3/test_builds.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/test/client_v3/test_helpers.py` & `copr-1.99/copr/test/client_v3/test_helpers.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/test/client_v3/test_requests.py` & `copr-1.99/copr/test/client_v3/test_requests.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/test/resources/build_details.200.json` & `copr-1.99/copr/test/resources/build_details.200.json`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/test/test_client.py` & `copr-1.99/copr/test/test_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,7 +72,22 @@
 
     test_resp = mock_client.get_build_details(27382)
 
     assert test_resp.status == "succeeded"
     assert test_resp.project == "atomic-next"
     assert test_resp.built_pkgs == [u'golang-github-stretchr-objx-devel 0']
     assert test_resp.submitted_on == 1408031345
+
+
+@mock.patch('requests.request')
+def test_get_build_config(mock_request):
+    mock_client = CoprClient.create_from_file_config(config_location)
+    mock_request.return_value = make_mock_response("build_config.200.json")
+    test_resp = mock_client.get_build_config("project", "chroot")
+    assert 'additional_packages' in test_resp.data
+    expected_args = ["additional_packages", "additional_repos", "chroot",
+                     "enable_net", "repos", "use_bootstrap_container",
+                     "with_opts", "without_opts"]
+    for arg in expected_args:
+        assert arg in test_resp.data
+        test_resp.data.pop(arg)
+    assert not test_resp.data.keys()
```

### Comparing `copr-1.98/copr/v3/__init__.py` & `copr-1.99/copr/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/v3/client.py` & `copr-1.99/copr/v3/client.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/v3/exceptions.py` & `copr-1.99/copr/v3/exceptions.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/v3/helpers.py` & `copr-1.99/copr/v3/helpers.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/v3/pagination.py` & `copr-1.99/copr/v3/pagination.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/v3/proxies/__init__.py` & `copr-1.99/copr/v3/proxies/__init__.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/v3/proxies/build.py` & `copr-1.99/copr/v3/proxies/build.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/v3/proxies/build_chroot.py` & `copr-1.99/copr/v3/proxies/build_chroot.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/v3/proxies/module.py` & `copr-1.99/copr/v3/proxies/module.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/v3/proxies/package.py` & `copr-1.99/copr/v3/proxies/package.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/v3/proxies/project.py` & `copr-1.99/copr/v3/proxies/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         request = Request(endpoint, api_base_url=self.api_base_url, params=params)
         response = request.send()
         return munchify(response)
 
     def add(self, ownername, projectname, chroots, description=None, instructions=None, homepage=None,
             contact=None, additional_repos=None, unlisted_on_hp=False, enable_net=True, persistent=False,
             auto_prune=True, use_bootstrap_container=False, devel_mode=False,
-            delete_after_days=None, multilib=False):
+            delete_after_days=None, multilib=False, module_hotfixes=False):
         """
         Create a project
 
         :param str ownername:
         :param str projectname:
         :param list chroots:
         :param str description:
@@ -75,14 +75,16 @@
         :param bool unlisted_on_hp: project will not be shown on Copr homepage
         :param bool enable_net: if builder can access net for builds in this project
         :param bool persistent: if builds and the project are undeletable
         :param bool auto_prune: if backend auto-deletion script should be run for the project
         :param bool use_bootstrap_container: if mock bootstrap container is used to initialize the buildroot
         :param bool devel_mode: if createrepo should run automatically
         :param int delete_after_days: delete the project after the specfied period of time
+        :param bool module_hotfixes: make packages from this project available
+                                     on along with packages from the active module streams.
         :return: Munch
         """
         endpoint = "/project/add/{ownername}"
         params = {
             "ownername": ownername,
         }
         data = {
@@ -97,24 +99,25 @@
             "enable_net": enable_net,
             "persistent": persistent,
             "auto_prune": auto_prune,
             "use_bootstrap_container": use_bootstrap_container,
             "devel_mode": devel_mode,
             "delete_after_days": delete_after_days,
             "multilib": multilib,
+            "module_hotfixes": module_hotfixes,
         }
         request = Request(endpoint, api_base_url=self.api_base_url, method=POST,
                           params=params, data=data, auth=self.auth)
         response = request.send()
         return munchify(response)
 
     def edit(self, ownername, projectname, chroots=None, description=None, instructions=None, homepage=None,
              contact=None, additional_repos=None, unlisted_on_hp=None, enable_net=None,
              auto_prune=None, use_bootstrap_container=None, devel_mode=None,
-             delete_after_days=None, multilib=None):
+             delete_after_days=None, multilib=None, module_hotfixes=None):
         """
         Edit a project
 
         :param str ownername:
         :param str projectname:
         :param list chroots:
         :param str description:
@@ -124,14 +127,16 @@
         :param list repos:
         :param bool unlisted_on_hp: project will not be shown on Copr homepage
         :param bool enable_net: if builder can access net for builds in this project
         :param bool auto_prune: if backend auto-deletion script should be run for the project
         :param bool use_bootstrap_container: if mock bootstrap container is used to initialize the buildroot
         :param bool devel_mode: if createrepo should run automatically
         :param int delete_after_days: delete the project after the specfied period of time
+        :param bool module_hotfixes: make packages from this project available
+                                     on along with packages from the active module streams.
         :return: Munch
         """
         endpoint = "/project/edit/{ownername}/{projectname}"
         params = {
             "ownername": ownername,
             "projectname": projectname,
         }
@@ -145,14 +150,15 @@
             "unlisted_on_hp": unlisted_on_hp,
             "enable_net": enable_net,
             "auto_prune": auto_prune,
             "use_bootstrap_container": use_bootstrap_container,
             "devel_mode": devel_mode,
             "delete_after_days": delete_after_days,
             "multilib": multilib,
+            "module_hotfixes": module_hotfixes,
         }
         request = Request(endpoint, api_base_url=self.api_base_url, method=POST,
                           params=params, data=data, auth=self.auth)
         response = request.send()
         return munchify(response)
 
     def delete(self, ownername, projectname):
```

### Comparing `copr-1.98/copr/v3/proxies/project_chroot.py` & `copr-1.99/copr/v3/proxies/project_chroot.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr/v3/requests.py` & `copr-1.99/copr/v3/requests.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/copr.egg-info/PKG-INFO` & `copr-1.99/copr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: copr
-Version: 1.98
+Version: 1.99
 Summary: Python client for copr service.
 Home-page: https://pagure.io/copr/copr
 Author: Valentin Gologuzov
 Author-email: vgologuz@redhat.com
 License: GPLv2+
 Description: Copr is designed to be a lightweight buildsystem that allows contributors
         to create packages, put them in repositories, and make it easy for users
```

### Comparing `copr-1.98/copr.egg-info/SOURCES.txt` & `copr-1.99/copr.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 copr/test/client_v2/test_entities.py
 copr/test/client_v2/test_handlers.py
 copr/test/client_v2/test_net_client.py
 copr/test/client_v3/test_builds.py
 copr/test/client_v3/test_general.py
 copr/test/client_v3/test_helpers.py
 copr/test/client_v3/test_requests.py
+copr/test/resources/build_config.200.json
 copr/test/resources/build_details.200.json
 copr/test/resources/copr_cli.conf
 copr/test/resources/projects_list.200.json
 copr/v3/__init__.py
 copr/v3/client.py
 copr/v3/exceptions.py
 copr/v3/helpers.py
```

### Comparing `copr-1.98/docs/ClientV1.rst` & `copr-1.99/docs/ClientV1.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/ClientV2.rst` & `copr-1.99/docs/ClientV2.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/ClientV3.rst` & `copr-1.99/docs/ClientV3.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/Makefile` & `copr-1.99/docs/Makefile`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/client_v1/Examples.rst` & `copr-1.99/docs/client_v1/Examples.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/client_v1/Responses.rst` & `copr-1.99/docs/client_v1/Responses.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/client_v2/resource_info/build.rst` & `copr-1.99/docs/client_v2/resource_info/build.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/client_v2/resource_info/build_task.rst` & `copr-1.99/docs/client_v2/resource_info/build_task.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/client_v2/resource_info/mock_chroot.rst` & `copr-1.99/docs/client_v2/resource_info/mock_chroot.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/client_v2/resource_info/project.rst` & `copr-1.99/docs/client_v2/resource_info/project.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/client_v2/resource_info/project_chroot.rst` & `copr-1.99/docs/client_v2/resource_info/project_chroot.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/client_v2/resources.rst` & `copr-1.99/docs/client_v2/resources.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/client_v2/resources_usage.rst` & `copr-1.99/docs/client_v2/resources_usage.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/client_v3/build_options.rst` & `copr-1.99/docs/client_v3/build_options.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/client_v3/client_initialization.rst` & `copr-1.99/docs/client_v3/client_initialization.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/client_v3/data_structures.rst` & `copr-1.99/docs/client_v3/data_structures.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/client_v3/error_handling.rst` & `copr-1.99/docs/client_v3/error_handling.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/client_v3/migration.rst` & `copr-1.99/docs/client_v3/migration.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/client_v3/package_source_types.rst` & `copr-1.99/docs/client_v3/package_source_types.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/client_v3/pagination.rst` & `copr-1.99/docs/client_v3/pagination.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/client_v3/proxies.rst` & `copr-1.99/docs/client_v3/proxies.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/client_v3/working_with_proxies_directly.rst` & `copr-1.99/docs/client_v3/working_with_proxies_directly.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/conf.py` & `copr-1.99/docs/conf.py`

 * *Files identical despite different names*

### Comparing `copr-1.98/docs/index.rst` & `copr-1.99/docs/index.rst`

 * *Files identical despite different names*

### Comparing `copr-1.98/python-copr.spec` & `copr-1.99/python-copr.spec`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 %endif
 
 %if 0%{?fedora} < 28 || 0%{?rhel} && 0%{?rhel} <= 7
 %global with_python2 1
 %endif
 
 Name:       python-copr
-Version:    1.98
+Version:    1.99
 Release:    1%{?dist}
 Summary:    Python interface for Copr
 
 License:    GPLv2+
 URL:        https://pagure.io/copr/copr
 
 # Source is created by:
@@ -232,14 +232,18 @@
 # with python2
 
 %files -n python-copr-doc
 %license LICENSE
 %doc %{_pkgdocdir}
 
 %changelog
+* Wed Dec 04 2019 Pavel Raiskup <praiskup@redhat.com> 1.99-1
+- add api support for module_hotfixes
+- nicer mock-config command output
+
 * Thu Oct 03 2019 Pavel Raiskup <praiskup@redhat.com> 1.98-1
 - enable dynamic buildrequires on F31+
 - drop comments after %%endif
 
 * Thu Sep 26 2019 Pavel Raiskup <praiskup@redhat.com> 1.97-1
 - python: fix API for marshmallow 3+ (#934)
 - frontend, cli, python: support multilib projects (#1)
```

### Comparing `copr-1.98/setup.py` & `copr-1.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 __author__ = "Valentin Gologuzov"
 __author_email__ = "vgologuz@redhat.com"
 __url__ = "https://pagure.io/copr/copr"
 
 
 setup(
     name='copr',
-    version="1.98",
+    version="1.99",
     description=__description__,
     long_description=long_description,
     author=__author__,
     author_email=__author_email__,
     url=__url__,
     license='GPLv2+',
     classifiers=[
```

