# Comparing `tmp/mlx.xunit2rst-1.5.1.tar.gz` & `tmp/mlx.xunit2rst-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mlx.xunit2rst-1.5.1.tar", last modified: Mon Apr  3 10:01:34 2023, max compression
+gzip compressed data, was "dist/mlx.xunit2rst-1.6.0.tar", last modified: Thu May 25 11:23:26 2023, max compression
```

## Comparing `mlx.xunit2rst-1.5.1.tar` & `mlx.xunit2rst-1.6.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:01:34.000000 mlx.xunit2rst-1.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:01:34.000000 mlx.xunit2rst-1.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:01:34.000000 mlx.xunit2rst-1.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-04-03 10:01:34.000000 mlx.xunit2rst-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:01:34.000000 mlx.xunit2rst-1.5.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:01:34.000000 mlx.xunit2rst-1.5.1/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/doc/source/example.rst
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/doc/source/extra_content.yml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/doc/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/doc/source/requirements.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:01:34.000000 mlx.xunit2rst-1.5.1/doc/source/robot/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/doc/source/robot/example.robot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:01:34.000000 mlx.xunit2rst-1.5.1/mlx/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/mlx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/mlx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/mlx/xunit2rst.mako
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/mlx/xunit2rst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:01:34.000000 mlx.xunit2rst-1.5.1/mlx.xunit2rst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-04-03 10:01:33.000000 mlx.xunit2rst-1.5.1/mlx.xunit2rst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-03 10:01:34.000000 mlx.xunit2rst-1.5.1/mlx.xunit2rst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 10:01:33.000000 mlx.xunit2rst-1.5.1/mlx.xunit2rst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-03 10:01:33.000000 mlx.xunit2rst-1.5.1/mlx.xunit2rst.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-03 10:01:33.000000 mlx.xunit2rst-1.5.1/mlx.xunit2rst.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 10:01:33.000000 mlx.xunit2rst-1.5.1/mlx.xunit2rst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-03 10:01:33.000000 mlx.xunit2rst-1.5.1/mlx.xunit2rst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-03 10:01:33.000000 mlx.xunit2rst-1.5.1/mlx.xunit2rst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-03 10:01:34.000000 mlx.xunit2rst-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:01:34.000000 mlx.xunit2rst-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/acceptance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/mako_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/prefix_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:01:34.000000 mlx.xunit2rst-1.5.1/tests/test_in/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/extra_content0.yml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/extra_content1.yml
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/itest_as_utest_report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/itest_lin_report.rst
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/itest_lin_report.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/itest_lin_report_failures.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/itest_lin_report_multisuite.xml
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/itest_report.rst
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/itest_report.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/itest_report_extra_content.rst
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/itest_report_extra_content.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/itest_report_log.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/itest_report_log_links.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/itest_report_log_links_multisuite.rst
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/itest_report_skipped.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/itest_report_skipped_failures_log.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/qtest_my_lib_report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/qtest_my_lib_report.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/rf6_multisuite_report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/rf6_multisuite_report.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/rf6_report.rst
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/rf6_report.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/utest_my_lib_no_prefix_report.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/utest_my_lib_report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/utest_my_lib_report.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/utest_my_lib_report_failures.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/utest_my_lib_report_skipped.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/utest_my_lib_report_skipped.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/utest_my_lib_suites_report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/utest_my_lib_suites_report_skipped.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tests/test_in/utest_override_prefix_report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-03 10:01:09.000000 mlx.xunit2rst-1.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/doc/source/example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/doc/source/extra_content.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/doc/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/doc/source/requirements.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/doc/source/robot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/doc/source/robot/example.robot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/mlx/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/mlx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/mlx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/mlx/xunit2rst.mako
+-rw-r--r--   0 runner    (1001) docker     (123)    12685 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/mlx/xunit2rst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/mlx.xunit2rst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/mlx.xunit2rst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/mlx.xunit2rst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/mlx.xunit2rst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/mlx.xunit2rst.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/mlx.xunit2rst.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/mlx.xunit2rst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/mlx.xunit2rst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/mlx.xunit2rst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/acceptance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/mako_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/prefix_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:23:26.000000 mlx.xunit2rst-1.6.0/tests/test_in/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/extra_content0.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/extra_content1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/itest_as_utest_report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/itest_lin_report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/itest_lin_report.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/itest_lin_report_failures.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/itest_lin_report_multisuite.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/itest_report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/itest_report.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/itest_report_extra_content.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/itest_report_extra_content.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/itest_report_log.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/itest_report_log_links.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/itest_report_log_links_multisuite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/itest_report_skipped.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/itest_report_skipped_failures_log.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/qtest_my_lib_report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/qtest_my_lib_report.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/rf6_multisuite_report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/rf6_multisuite_report.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/rf6_report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/rf6_report.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/utest_my_lib_no_prefix_report.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/utest_my_lib_report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/utest_my_lib_report.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/utest_my_lib_report_failures.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/utest_my_lib_report_skipped.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/utest_my_lib_report_skipped.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/utest_my_lib_suites_report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/utest_my_lib_suites_report_skipped.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tests/test_in/utest_override_prefix_report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-25 11:23:06.000000 mlx.xunit2rst-1.6.0/tox.ini
```

### Comparing `mlx.xunit2rst-1.5.1/.github/workflows/codeql-analysis.yml` & `mlx.xunit2rst-1.6.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/.github/workflows/python-package.yml` & `mlx.xunit2rst-1.6.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/.gitignore` & `mlx.xunit2rst-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/LICENSE` & `mlx.xunit2rst-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/PKG-INFO` & `mlx.xunit2rst-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx.xunit2rst
-Version: 1.5.1
+Version: 1.6.0
 Summary: Python script for converting xUnit/JUnit XML format to reStructuredText (.rst) with traceable items
 Home-page: https://github.com/melexis/xunit2rst
 Author: JasperCraeghs
 Author-email: jce@melexis.com
 License: Apache License Version 2.0
 Description: .. image:: https://img.shields.io/badge/License-Apache%202.0-blue.svg
             :target: https://opensource.org/licenses/Apache-2.0
```

### Comparing `mlx.xunit2rst-1.5.1/README.rst` & `mlx.xunit2rst-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/doc/Makefile` & `mlx.xunit2rst-1.6.0/doc/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 ECHO          := echo
 CP            := cp
 
 ROBOT_XUNIT   = $(ROBOTDIR)/report.xml
 ITEST_PLAN    = $(OUTDIR)/itest_plan.rst
 LOG_FILE      = log.html
 LAYER         ?= ""
+PREFIX        ?= ITEST_-  # becomes ITEST-
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS)
 
 clean:
 	$(RM) $(BUILDDIR)
@@ -34,11 +35,11 @@
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.
 html: Makefile
 	@$(RM) $(ROBOT_XUNIT)
 	@$(RM) $(ITEST_PLAN)
 	-@$(ROBOT) --xunit report.xml -d $(ROBOTDIR) $(ROBOTDIR)/example.robot
 	@$(XUNIT2RST) -v
-	@$(XUNIT2RST) -i $(ROBOT_XUNIT) -o $(OUTDIR)/itest_report.rst -p ITEST_- --trim-suffix -l ../$(LOG_FILE) --only $(LAYER) --links --failure-message
-	@$(ROBOT2RST) --robot $(ROBOTDIR)/example.robot --rst $(ITEST_PLAN) --tags ^RQT-$
+	@$(XUNIT2RST) -i $(ROBOT_XUNIT) -o $(OUTDIR)/itest_report.rst -p $(PREFIX) --trim-suffix -l ../$(LOG_FILE) --only $(LAYER) --links --failure-message
+	@$(ROBOT2RST) --robot $(ROBOTDIR)/example.robot --rst $(ITEST_PLAN) -p $(PREFIX) --trim-suffix --type $(PREFIX) --tags ^RQT-$
 	@$(ECHO) -n $(LOG_FILE) | xargs -d ' ' -n 1 -I {} $(CP) $(ROBOTDIR)/{} $(OUTDIR)
 	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS)
```

### Comparing `mlx.xunit2rst-1.5.1/doc/source/conf.py` & `mlx.xunit2rst-1.6.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/doc/source/robot/example.robot` & `mlx.xunit2rst-1.6.0/doc/source/robot/example.robot`

 * *Files 8% similar despite different names*

```diff
@@ -24,11 +24,15 @@
     Should Be Equal    ${sum}    ${256}
 
 A skipped test
     [Documentation]    Example of a test that is always skipped
     [Tags]             RQT-LOGGING
     Skip               This test case is always skipped.
 
+Comp1: testing 'Special" characters & prefix
+    [Documentation]     The item ID will contain COMP1-SPECIAL_CHARACTERS_AND_PREFIX.
+                        Log     Special characters in test case names are supported but not recommended.
+
 *** Keywords ***
 My Keyword
     [Arguments]    ${path}
     Directory Should Exist    ${path}
```

### Comparing `mlx.xunit2rst-1.5.1/mlx/xunit2rst.mako` & `mlx.xunit2rst-1.6.0/mlx/xunit2rst.mako`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 <%
+import re
 import textwrap
 import xml.etree.ElementTree as ET
 
 title = "{} Test Report for {}".format(info.type.capitalize(), report_name)
 
 
 def _convert_name(name):
-    """ Itemize given name and prepend prefix if needed """
-    name_without_suite = name.split('.')[-1]  # cut off suite name if prepended by a dot
-    converted_name = name_without_suite.upper().replace(' ', '_').replace('&', 'AND')
-    if not converted_name.startswith(prefix):
-        converted_name = prefix + converted_name
-    return converted_name
+    """ Itemize given test case name """
+    name = name.split('.')[-1]  # cut off suite name if prepended by a dot
+    name = name.upper()
+    name = re.sub('\s*:\s*', '-', name)
+    name = name.replace('&', 'AND')
+    name = re.sub('[^\w\s_-]', '', name)
+    name = re.sub('\s+', '_', name)
+    return name
 
 
 def generate_body(input_string, indent, error_type=None):
     ''' Transforms the input string to be part of an item's indented body with word wrapping.
 
     Args:
         input_string (str): Raw error message.
@@ -46,15 +49,18 @@
 Test Reports
 ============
 <%
 suite_names = set()
 test_idx = 0
 %>
 % for suite_idx, suite in enumerate(test_suites):
-<% print(suite_idx); extra_content_map = indexed_extra_content_map.get(suite_idx, {}) %>\
+<%
+extra_content_map = indexed_extra_content_map.get(suite_idx, {})
+extra_content_map = {_convert_name(key): value for key, value in extra_content_map.items()}
+%>\
     % if not itemize_suites:  # create traceable item per testcase element
         % for test in suite:
 <%
 if len(test):
     if test.findall('skipped'):
         test_result = 'Skip'
         relationship = 'skipped'
@@ -112,17 +118,20 @@
     :type: fails passes skipped
     :stats:
     :group: top
     :nocaptions:
 \
 <%def name="generate_item(element_name, relationship, failure_msg, tests, indexes, extra_content_map)">\
 <%
-test_name = _convert_name(element_name)
-key_name = element_name.lower().replace(' ', '_')
-extra_content = extra_content_map.get(key_name, "")
+test_name_no_prefix = _convert_name(element_name)
+extra_content = extra_content_map.get(test_name_no_prefix, "")
+if test_name_no_prefix.startswith(prefix):
+    test_name = test_name_no_prefix
+else:
+    test_name = prefix + test_name_no_prefix
 %>\
 .. item:: REPORT_${test_name} Test report for ${test_name}
     :${relationship}: ${test_name}
 % if add_links:
     :ext_robotframeworklog: ${log_file}:${"s1-" if indexes[0] else ""}s${indexes[0] if indexes[0] else 1}-t${indexes[1]}
 % endif
```

### Comparing `mlx.xunit2rst-1.5.1/mlx/xunit2rst.py` & `mlx.xunit2rst-1.6.0/mlx/xunit2rst.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     indexed_extra_content_map = {}
     for i, file in report_info_files.items():
         extra_content_map = {}
         yaml = YAML(typ='safe', pure=True)
         if not file.is_absolute():
             file = input_file.parent / file
-        extra_content_map = {name.lower().replace(' ', '_'): content
+        extra_content_map = {name: content
                              for name, content in yaml.load(file).items()}
         indexed_extra_content_map[i] = extra_content_map
 
     render_template(
         rst_file,
         test_suites=test_suites,
         report_name=report_name,
```

### Comparing `mlx.xunit2rst-1.5.1/mlx.xunit2rst.egg-info/PKG-INFO` & `mlx.xunit2rst-1.6.0/mlx.xunit2rst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx.xunit2rst
-Version: 1.5.1
+Version: 1.6.0
 Summary: Python script for converting xUnit/JUnit XML format to reStructuredText (.rst) with traceable items
 Home-page: https://github.com/melexis/xunit2rst
 Author: JasperCraeghs
 Author-email: jce@melexis.com
 License: Apache License Version 2.0
 Description: .. image:: https://img.shields.io/badge/License-Apache%202.0-blue.svg
             :target: https://opensource.org/licenses/Apache-2.0
```

### Comparing `mlx.xunit2rst-1.5.1/mlx.xunit2rst.egg-info/SOURCES.txt` & `mlx.xunit2rst-1.6.0/mlx.xunit2rst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/setup.py` & `mlx.xunit2rst-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/acceptance_test.py` & `mlx.xunit2rst-1.6.0/tests/acceptance_test.py`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/mako_test.py` & `mlx.xunit2rst-1.6.0/tests/mako_test.py`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/prefix_test.py` & `mlx.xunit2rst-1.6.0/tests/prefix_test.py`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/itest_as_utest_report.rst` & `mlx.xunit2rst-1.6.0/tests/test_in/itest_as_utest_report.rst`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/itest_lin_report.rst` & `mlx.xunit2rst-1.6.0/tests/test_in/itest_lin_report.rst`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/itest_lin_report.xml` & `mlx.xunit2rst-1.6.0/tests/test_in/itest_lin_report.xml`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/itest_lin_report_failures.rst` & `mlx.xunit2rst-1.6.0/tests/test_in/itest_lin_report_failures.rst`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/itest_lin_report_multisuite.xml` & `mlx.xunit2rst-1.6.0/tests/test_in/itest_lin_report_multisuite.xml`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/itest_report.rst` & `mlx.xunit2rst-1.6.0/tests/test_in/itest_report.rst`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/itest_report.xml` & `mlx.xunit2rst-1.6.0/tests/test_in/itest_report.xml`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/itest_report_extra_content.rst` & `mlx.xunit2rst-1.6.0/tests/test_in/itest_report_extra_content.rst`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/itest_report_extra_content.xml` & `mlx.xunit2rst-1.6.0/tests/test_in/itest_report_extra_content.xml`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/itest_report_log.rst` & `mlx.xunit2rst-1.6.0/tests/test_in/itest_report_log.rst`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/itest_report_log_links.rst` & `mlx.xunit2rst-1.6.0/tests/test_in/itest_report_log_links.rst`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/itest_report_log_links_multisuite.rst` & `mlx.xunit2rst-1.6.0/tests/test_in/itest_report_log_links_multisuite.rst`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/itest_report_skipped.xml` & `mlx.xunit2rst-1.6.0/tests/test_in/itest_report_skipped.xml`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/itest_report_skipped_failures_log.rst` & `mlx.xunit2rst-1.6.0/tests/test_in/itest_report_skipped_failures_log.rst`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/qtest_my_lib_report.rst` & `mlx.xunit2rst-1.6.0/tests/test_in/qtest_my_lib_report.rst`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/qtest_my_lib_report.xml` & `mlx.xunit2rst-1.6.0/tests/test_in/qtest_my_lib_report.xml`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/rf6_multisuite_report.rst` & `mlx.xunit2rst-1.6.0/tests/test_in/rf6_multisuite_report.rst`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/rf6_multisuite_report.xml` & `mlx.xunit2rst-1.6.0/tests/test_in/rf6_multisuite_report.xml`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/rf6_report.rst` & `mlx.xunit2rst-1.6.0/tests/test_in/rf6_report.rst`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/rf6_report.xml` & `mlx.xunit2rst-1.6.0/tests/test_in/rf6_report.xml`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/utest_my_lib_no_prefix_report.xml` & `mlx.xunit2rst-1.6.0/tests/test_in/utest_my_lib_no_prefix_report.xml`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/utest_my_lib_report.rst` & `mlx.xunit2rst-1.6.0/tests/test_in/utest_my_lib_report.rst`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/utest_my_lib_report.xml` & `mlx.xunit2rst-1.6.0/tests/test_in/utest_my_lib_report.xml`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/utest_my_lib_report_failures.rst` & `mlx.xunit2rst-1.6.0/tests/test_in/utest_my_lib_report_failures.rst`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/utest_my_lib_report_skipped.rst` & `mlx.xunit2rst-1.6.0/tests/test_in/utest_my_lib_report_skipped.rst`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/utest_my_lib_report_skipped.xml` & `mlx.xunit2rst-1.6.0/tests/test_in/utest_my_lib_report_skipped.xml`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/utest_my_lib_suites_report.rst` & `mlx.xunit2rst-1.6.0/tests/test_in/utest_my_lib_suites_report.rst`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/utest_my_lib_suites_report_skipped.rst` & `mlx.xunit2rst-1.6.0/tests/test_in/utest_my_lib_suites_report_skipped.rst`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tests/test_in/utest_override_prefix_report.rst` & `mlx.xunit2rst-1.6.0/tests/test_in/utest_override_prefix_report.rst`

 * *Files identical despite different names*

### Comparing `mlx.xunit2rst-1.5.1/tox.ini` & `mlx.xunit2rst-1.6.0/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 [testenv:doc]
 deps=
     {[testenv]deps}
     sphinx_rtd_theme
     mlx.traceability >= 4.3.2
     mlx.warnings >= 1.2.0
-    mlx.robot2rst >= 2.0.2, <3
+    mlx.robot2rst >= 3.3.0, <4
     robotframework >= 5.0.1
     sphinx_selective_exclude >= 1.0.3
 allowlist_externals =
     bash
     make
     mlx-warnings >= 1.3.1
 commands=
```

