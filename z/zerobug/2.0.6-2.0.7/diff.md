# Comparing `tmp/zerobug-2.0.6.tar.gz` & `tmp/zerobug-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zerobug-2.0.6.tar", last modified: Tue May  9 17:26:34 2023, max compression
+gzip compressed data, was "dist/zerobug-2.0.7.tar", last modified: Thu May 25 08:52:48 2023, max compression
```

## Comparing `zerobug-2.0.6.tar` & `zerobug-2.0.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:26:34.000000 zerobug-2.0.6/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/__main__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    23850 2023-05-09 16:09:43.000000 zerobug-2.0.6/zerobug/z0testrc
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug/dummy/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      121 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/dummy/dummylib.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)       47 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/dummy/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug/scripts/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     4102 2023-05-09 17:24:33.000000 zerobug-2.0.6/zerobug/scripts/setup.info
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6806 2023-05-09 16:09:43.000000 zerobug-2.0.6/zerobug/scripts/main.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/scripts/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug/_travis/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1852 2023-04-14 14:02:41.000000 zerobug-2.0.6/zerobug/_travis/travis_after_tests_success
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    18626 2023-05-09 16:09:43.000000 zerobug-2.0.6/zerobug/_travis/travis_run_pypi_tests
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug/_travis/cfg/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      668 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2005 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_pr.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      534 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_70.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      593 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1126 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/coveragerc
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      744 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      716 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      122 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_shellcheck.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      703 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1022 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      690 2023-01-30 07:04:22.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8__init__AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      132 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_shellcheck_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      629 2023-01-30 06:58:04.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8__init__.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      152 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_shellcheck_MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2575 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2823 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      533 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_61.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      704 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8__init__NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2526 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_beta.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      814 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8_MINIMAL.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    24221 2023-05-09 16:09:43.000000 zerobug-2.0.6/zerobug/_travis/travis_install_env
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1361 2023-01-27 07:10:19.000000 zerobug-2.0.6/zerobug/_travis/build_cmd
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       24 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    63945 2023-05-09 16:09:43.000000 zerobug-2.0.6/zerobug/z0testlib.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      574 2023-05-09 16:09:43.000000 zerobug-2.0.6/zerobug/zerobug.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      157 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        8 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-09 06:43:26.000000 zerobug-2.0.6/zerobug.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       91 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1946 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       70 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2870 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-09 17:26:34.000000 zerobug-2.0.6/setup.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     4102 2023-05-09 16:09:43.000000 zerobug-2.0.6/setup.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2870 2023-05-09 17:26:34.000000 zerobug-2.0.6/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    15748 2023-05-09 17:26:33.000000 zerobug-2.0.6/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:52:48.000000 zerobug-2.0.7/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/__main__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    23977 2023-05-20 08:38:13.000000 zerobug-2.0.7/zerobug/z0testrc
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug/dummy/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      121 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/dummy/dummylib.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)       47 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/dummy/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4138 2023-05-21 12:33:18.000000 zerobug-2.0.7/zerobug/scripts/setup.info
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6806 2023-05-20 08:38:13.000000 zerobug-2.0.7/zerobug/scripts/main.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/scripts/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug/_travis/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1852 2023-04-14 14:02:41.000000 zerobug-2.0.7/zerobug/_travis/travis_after_tests_success
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    17892 2023-05-20 08:38:13.000000 zerobug-2.0.7/zerobug/_travis/travis_run_pypi_tests
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug/_travis/cfg/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      668 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2005 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_pr.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      534 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_70.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      593 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1126 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/coveragerc
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      744 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      716 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      122 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_shellcheck.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      703 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1022 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      690 2023-01-30 07:04:22.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8__init__AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      132 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_shellcheck_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      629 2023-01-30 06:58:04.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8__init__.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      152 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_shellcheck_MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2575 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2823 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      533 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_61.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      704 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8__init__NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2526 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_beta.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      814 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8_MINIMAL.cfg
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    24224 2023-05-20 08:38:13.000000 zerobug-2.0.7/zerobug/_travis/travis_install_env
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1361 2023-01-27 07:10:19.000000 zerobug-2.0.7/zerobug/_travis/build_cmd
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       24 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    60073 2023-05-20 08:38:13.000000 zerobug-2.0.7/zerobug/z0testlib.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      574 2023-05-20 08:38:13.000000 zerobug-2.0.7/zerobug/zerobug.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      157 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        8 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-09 06:43:26.000000 zerobug-2.0.7/zerobug.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       91 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1946 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       70 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    15053 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-25 08:52:48.000000 zerobug-2.0.7/setup.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2877 2023-05-22 09:12:28.000000 zerobug-2.0.7/setup.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    15053 2023-05-25 08:52:48.000000 zerobug-2.0.7/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    10937 2023-05-25 08:52:42.000000 zerobug-2.0.7/README.rst
```

### Comparing `zerobug-2.0.6/zerobug/z0testrc` & `zerobug-2.0.7/zerobug/z0testrc`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 # WLOGCMD:        oveerride opt_echo; may be None, 'echo', 'echo-1' or 'echo-0'
 #
 # This free software is released under GNU Affero GPL3
 # author: Antonio M. Vigliotti - antoniomaria.vigliotti@gmail.com
 # (C) 2015-2023 by SHS-AV s.r.l. - http://www.shs-av.com - info@shs-av.com
 #
 
-__version__=2.0.6
+__version__=2.0.7
 
 export opt_dry_run
 export ctr
 export opt_verbose
 export max_test
 export min_test
 export opt_noctr
@@ -85,42 +85,43 @@
     if [[ -t 0 || -p /dev/stdin ]]; then
       export LECHO=echo
       local Z0=0
     else
       export LECHO=
       local Z0=1
     fi
-    OPTOPTS=(h        B         C         e        f        k       J         l      N       n           O         q        R   r        s        V           v           z        Z        0         1         2       3)
-    OPTDEST=(opt_help opt_debug run4cover opt_echo opt_fail opt_new opt_tjLib logfn  opt_new opt_dry_run opt_oeLib opt_echo nrt min_test min_test opt_version opt_verbose max_test opt_zLib opt_noctr run4cover opt_py2 opt_py3)
-    OPTACTI=(1        1         0         1        1        0       1         "="    1       1           1         0        1   "=>"     "=>"     "*>"        1           "=>"     1        1         1         1       1)
-    OPTDEFL=(0        0         -1        -1       0        -1      0         ""     -1      0           0         -1       0   ""       ""       ""          0           ""       0        $Z0       -1        0       0)
-    OPTMETA=("help"   "debug"   ""        "echo"   ""       "keep"  ""        "file" "new"   "count"     ""        "quiet"  ""  "number" "number" "version"   "verbose"   "number" ""       "no"      ""        ""      "")
-    OPTHELP=("show this help message and exit"\
-     "run tests in debug mode"\
-     "run tests w/o coverage"\
-     "enable echoing even if not interactive tty"\
-     "stop on first failure"\
-     "keep current logfile"\
-     "load travisrc library"\
-     "set logfile name"\
-     "create new logfile"\
-     "count and display # unit tests"\
-     "load odoorc library"\
-     "run tests without output (quiet mode)"\
-     "ignored"\
-     "restart count next to number"\
-     "see -r (deprecated)"\
-     "show version and exit"\
-      "verbose mode"\
-     "display total # tests when execute them"\
-     "load zar library"\
-     "no count # unit tests"\
-     "run tests for coverage (obsolete)"\
-     "python2"\
-     "python3")
+    OPTOPTS=(h        B         C         e        f        J         k       l      N       n           O         p         q        R   r        s        V           v           z        Z        0         1         2       3)
+    OPTDEST=(opt_help opt_debug run4cover opt_echo opt_fail opt_tjLib opt_new logfn  opt_new opt_dry_run opt_oeLib opt_patrn opt_echo nrt min_test min_test opt_version opt_verbose max_test opt_zLib opt_noctr run4cover opt_py2 opt_py3)
+    OPTACTI=(1        1         0         1        1        1         0       "="    1       1           1         "="       0        1   "=>"     "=>"     "*>"        1           "=>"     1        1         1         1       1)
+    OPTDEFL=(0        0         -1        -1       0        0         -1      ""     -1      0           0         ""        -1       0   ""       ""       ""          0           ""       0        $Z0       -1        0       0)
+    OPTMETA=("help"   "debug"   ""        "echo"   ""       ""        "keep"  "file" "new"   "count"     ""        "pattern" "quiet"  ""  "number" "number" "version"   "verbose"   "number" ""       "no"      ""        ""      "")
+    OPTHELP=("show this help message and exit"
+     "run tests in debug mode"
+     "run tests w/o coverage"
+     "enable echoing even if not interactive tty"
+     "stop on first failure"
+     "load travisrc library"
+      "keep current logfile"
+     "set logfile name"
+     "create new logfile"
+     "count and display # unit tests"
+     "load odoorc library"
+     "pattern to apply for test files (comma separated)"
+     "run tests without output (quiet mode)"
+     "ignored"
+     "restart count next to number"
+     "see -r (deprecated)"
+     "show version and exit"
+      "verbose mode"
+     "display total # tests when execute them"
+     "load zar library"
+     "no count # unit tests (deprecated)"
+     "run tests for coverage (obsolete)"
+     "python2 (deprecated)"
+     "python3 (deprecated)")
     OPTARGS=()
     parseoptargs "$@"
     if [ "$opt_version" ]; then
       echo "$__version__"
       exit 0
     elif [ $opt_help -gt 0 ]; then
       print_help "Regression test on $module_id"\
@@ -533,15 +534,15 @@
           s=$?
         elif [ "$basetn" != "$THIS" ]; then
           dbgmsg "\$ elif [ \"\$basetn\" != \"\$THIS\" ]; then"
           [[ "$dirtn" == "." ]] && testname=$TESTDIR/$basetn
           if [ "${basetn: -3}" == ".py" ]; then
             if [ ${run4cover:-0} -ne 0 ]; then
               dbgmsg "\$ coverage run -a --rcfile=$COVERAGE_PROCESS_START $testname $opt4childs"
-              echo "coverage run -a --rcfile=$COVERAGE_PROCESS_START $testname $opt4childs"     #debug
+              # echo "coverage run -a --rcfile=$COVERAGE_PROCESS_START $testname $opt4childs"     #debug
               coverage run -a --rcfile=$COVERAGE_PROCESS_START $testname $opt4childs
             else
               dbgmsg "\$ python $testname $opt4childs"
               python $testname $opt4childs
             fi
             s=$?
           else
```

### Comparing `zerobug-2.0.6/zerobug/scripts/setup.info` & `zerobug-2.0.7/zerobug/scripts/setup.info`

 * *Files 3% similar despite different names*

```diff
@@ -15,25 +15,26 @@
         ],
     )
 else:
     install_requires = (
         [
             'future',
             'coverage',
-            'pylint-odoo<=5.0.0',
+            # 'pylint-odoo<=5.0.0',
+            'pylint-odoo==3.5.0',
             'python-magic',
             'python-plus',
             'os0',
             'z0lib',
         ],
     )
 
 setup(
     name='zerobug',
-    version='2.0.6',
+    version='2.0.7',
     description='Zeroincombenze continuous testing framework'
     ' and tools for python and bash programs',
     long_description="""
 This library can run unit test of target package software.
 Supported languages are python (through z0testlib.py) and bash (through z0testrc)
 
 zerobug supports test automation, aggregation of tests into collections
```

### Comparing `zerobug-2.0.6/zerobug/scripts/main.py` & `zerobug-2.0.7/zerobug/scripts/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
```

### Comparing `zerobug-2.0.6/zerobug/_travis/travis_after_tests_success` & `zerobug-2.0.7/zerobug/_travis/travis_after_tests_success`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/travis_run_pypi_tests` & `zerobug-2.0.7/zerobug/_travis/travis_run_pypi_tests`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.6
+__version__=2.0.7
 
 
 travis_test_bash() {
     echo "======== Testing test_bash   ========"
     local s sts
     sts=0
     if [ ${opt_dry_run:-0} -eq 0 ]; then
@@ -215,29 +215,16 @@
     local x opts OPTS
     local s sts
     sts=0
     if [ ${opt_dry_run:-0} -eq 0 ]; then
         [[ $TRAVIS_PDB == "true" ]] && opts="${opts}B"
         [[ $TRAVIS_DEBUG_MODE =~ [89] ]] && opts="${opts}n"
         OPTS=$(inherits_travis_opts "$opts" "T")
+        [[ -n $TRAVIS_TEST_PATTERN ]] && OPTS="$OPTS -p $TRAVIS_TEST_PATTERN"
         coverage_set
-#        if [[ -f ./tests/all_tests.py ]]; then
-#            if [[ ${opt_dprj:-0} -gt 0 ]]; then
-#                run_traced "cd $PRJPATH; DEV_ENVIRONMENT=$PRJNAME coverage run -a --rcfile $COVERAGE_PROCESS_START ./tests/all_tests.py $OPTS"
-#            else
-#                run_traced "cd $PRJPATH/tests; DEV_ENVIRONMENT=$PRJNAME coverage run -a --rcfile $COVERAGE_PROCESS_START all_tests.py $OPTS"
-#            fi
-#            s=$?; [ ${s-1} -eq 0 -o $sts -ne 0 ] || sts=$s
-#        elif [[ -f ./tests/all_tests && ${opt_pyth:-0} -eq 0 ]]; then
-#            if [ ${opt_dprj:-0} -gt 0 ]; then
-#                run_traced "$PRJPATH/tests/all_tests $OPTS"
-#            else
-#                run_traced "cd $PRJPATH/tests; ./all_tests $OPTS"
-#            fi
-#            s=$?; [ ${s-1} -eq 0 -o $sts -ne 0 ] || sts=$s
         if [[ -f ./tests/test_$PRJNAME.py ]]; then
             if [ ${opt_dprj:-0} -gt 0 ]; then
                 run_traced "cd $PRJPATH; DEV_ENVIRONMENT=$PRJNAME coverage run -a --rcfile $COVERAGE_PROCESS_START ./tests/test_$PRJNAME.py $OPTS"
             else
                 run_traced "cd $PRJPATH/tests; DEV_ENVIRONMENT=$PRJNAME coverage run -a --rcfile $COVERAGE_PROCESS_START test_$PRJNAME.py $OPTS"
             fi
             s=$?; [ ${s-1} -eq 0 -o $sts -ne 0 ] || sts=$s
@@ -252,17 +239,14 @@
         $(ls ./pytest* &> /dev/null) && cd ..
         if $(ls ./tests/pytest* &> /dev/null); then
             run_traced "coverage run -m pytest -v ./tests/pytest*"
             s=$?; [ ${s-1} -eq 0 -o $sts -ne 0 ] || sts=$s
         fi
         if [[ ! -f $COVERAGE_DATA_FILE ]]; then
             echo "Result coverage file not found!"
-#        elif [ ${opt_dprj:-0} -eq 0 ]; then
-#            run_traced "mv .coverage .."
-#            run_traced "cd .."
         fi
     fi
     return $sts
 }
 
 do_test () {
     if [[ $PRJNAME == "Odoo" ]]; then
@@ -341,48 +325,48 @@
         [ -n "$PYTHONPATH" ] && export PYTHONPATH=$PYTHONPATH:$pth
         [ -z "$PYTHONPATH" ] && export PYTHONPATH=$pth
       fi
     done
 }
 
 
-OPTOPTS=(h        c        j        K         n            p        q           r     T        t         V           v)
-OPTDEST=(opt_help opt_conf opt_dprj opt_check opt_dry_run  opt_pyth opt_verbose opt_r opt_regr test_mode opt_version opt_verbose)
-OPTACTI=("+"      "="      1        1         1            1        0           1     1        1         "*>"        "+")
-OPTDEFL=(0        ""       0        0         0            0        0           0     0        0         ""          -1)
-OPTMETA=("help"   "file"   "dprj"   "check"   "do nothing" ""       "quiet"     "rxt" "test"   "test"    "version"   "verbose")
-OPTHELP=("this help"\
- "configuration file (def .travis.conf)"\
- "execute tests in project dir rather in test dir"\
- "do bash, flake8 and pylint checks"\
- "do nothing (dry-run)"\
- "prefer python test over bash test when avaiable"\
- "silent mode"\
- "run rescricted mode (w/o parsing travis.yml file)"\
- "do regression tests"\
- "test mode (implies dry-run)"\
- "show version"\
- "verbose mode")
+OPTOPTS=(h        c        j        K         n            p         q           r     T        t         V           v)
+OPTDEST=(opt_help opt_conf opt_dprj opt_check opt_dry_run  opt_patrn opt_verbose opt_r opt_regr test_mode opt_version opt_verbose)
+OPTACTI=("+"      "="      1        1         1            "="       0           1     1        1         "*>"        "+")
+OPTDEFL=(0        ""       0        0         0            ""        0           0     0        0         ""          -1)
+OPTMETA=("help"   "file"   "dprj"   "check"   "do nothing" "pattern" "quiet"     "rxt" "test"   "test"    "version"   "verbose")
+OPTHELP=("this help"
+ "configuration file (def .travis.conf)"
+ "deprecated: execute tests in project dir rather in test dir"
+ "do bash, flake8 and pylint checks - BASH_CHECK='1' LINT_CHECK='1'"
+ "do nothing (dry-run) - MQT_DRY_RUN"
+ "pattern to apply for test files (comma separated) - TRAVIS_TEST_PATTERN"
+ "silent mode"
+ "DEPRECATED: run rescricted mode (w/o parsing travis.yml file)"
+ "do regression tests - TESTS='1'"
+ "test mode (implies dry-run)"
+ "show version"
+ "verbose mode - MQT_VERBOSE_MODE")
 OPTARGS=(pkg PRJNAME)
 
 parseoptargs "$@"
 if [[ "$opt_version" ]]; then
     echo "$__version__"
     exit 0
 fi
 if [[ $opt_help -gt 0 ]]; then
     print_help "Run test in travis environment" \
                "(C) 2015-2023 by zeroincombenze(R)\nhttp://wiki.zeroincombenze.org/en/Linux/dev\nAuthor: antoniomaria.vigliotti@gmail.com"
     exit 0
 fi
 
-[ "${MQT_DRY_RUN:-0}" == "1" ] && opt_dry_run=1
-[ "${MQT_VERBOSE_MODE:-0}" == "1" ] && opt_verbose=1
-[ "${MQT_VERBOSE_MODE:-1}" == "0" ] && opt_verbose=0
-[ ${TRAVIS_DEBUG_MODE:-0} -ne 0 ] && opt_verbose=1
+[[ ${MQT_DRY_RUN:-0} == "1" ]] && opt_dry_run=1
+[[ ${MQT_VERBOSE_MODE:-1} == "0" ]] && opt_verbose=0
+[[ ${TRAVIS_DEBUG_MODE:-0} -ne 0 ]] && opt_verbose=1
+[[ -n $opt_patrn ]] && TRAVIS_TEST_PATTERN="$opt_patrn"
 
 opts_travis
 conf_default
 [[ $opt_verbose -gt 2 ]] && set -x
 init_travis
 prepare_env_travis
```

### Comparing `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg` & `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_pr.cfg` & `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_pr.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_70.cfg` & `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_70.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg` & `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/cfg/coveragerc` & `zerobug-2.0.7/zerobug/_travis/cfg/coveragerc`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg` & `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg` & `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg` & `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg` & `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg` & `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg` & `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8.cfg` & `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8__init__.cfg` & `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8__init__.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint.cfg` & `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg` & `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_61.cfg` & `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_61.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg` & `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_beta.cfg` & `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_beta.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8_MINIMAL.cfg` & `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8_MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/_travis/travis_install_env` & `zerobug-2.0.7/zerobug/_travis/travis_install_env`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.6
+__version__=2.0.7
 
 
 run_traced() {
   [[ :$SHELLOPTS: =~ :xtrace: ]] && set +x
   [[ -z ${Z0_STACK:+_} ]] && export Z0_STACK=0
   ((Z0_STACK=Z0_STACK+2))
   local xcmd="$1" lm="                    "
@@ -540,15 +540,15 @@
       dependencies_dir=${HOME}/dependencies
       run_traced "$VEM amend -D -O $ODOO_BRANCH -o $ocb_dir"
     else
       ocb_dir=${ODOO_PATH}
       dependencies_dir="$TRAVIS_BUILD_DIR,${HOME}/dependencies"
       run_traced "$VEM amend -D -O $ODOO_BRANCH -o ${ODOO_PATH} -d $dependencies_dir"
     fi
-    run_traced "$VEM uninstall pyOpenSSL -y"  #debug
+    ## run_traced "$VEM uninstall pyOpenSSL -y"  #debug
     if [[ $ODOO_TEST_SELECT == "APPLICATIONS" ]]; then
       if [[ -f "${TRAVIS_BUILD_DIR}/addons/website/tests/test_crawl.py" ]]; then
         run_traced "sed -i \"s/self.url_open(url)/self.url_open(url, timeout=100)/g\" ${TRAVIS_BUILD_DIR}/addons/website/tests/test_crawl.py"
       elif [[ -f "${ODOO_PATH}/addons/website/tests/test_crawl.py" ]]; then
         run_traced "sed -i \"s/self.url_open(url)/self.url_open(url, timeout=100)/g\" ${ODOO_PATH}/addons/website/tests/test_crawl.py"
       fi
     elif [[ $ODOO_TEST_SELECT == "LOCALIZATION" ]]; then
```

### Comparing `zerobug-2.0.6/zerobug/_travis/build_cmd` & `zerobug-2.0.7/zerobug/_travis/build_cmd`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/zerobug/z0testlib.py` & `zerobug-2.0.7/zerobug/z0testlib.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from subprocess import PIPE, Popen
 
 import magic
 
 from os0 import os0
 from python_plus import _c
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 # return code
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 if os.name == "posix":
     RED = "\033[1;31m"
     GREEN = "\033[1;32m"
@@ -398,37 +398,23 @@
             if os.path.isdir('./tests'):
                 self.testdir = os.path.join(self.this_dir, 'tests')
             else:
                 self.testdir = self.this_dir
             self.rundir = self.this_dir
         # Testing package dir must be the 1.st one in sys.path
         this_pkg_dir = os.path.dirname(self.rundir)
-        # PYTHONPATH = os.environ.get('PYTHONPATH', '')
-        # if this_pkg_dir not in sys.path:
-        #     if PYTHONPATH:
-        #         p = ':%s:' % PYTHONPATH
-        #         if p.find(':%s:' % this_pkg_dir) < 0:
-        #             PYTHONPATH = '%s:%s' % (this_pkg_dir, PYTHONPATH)
-        #     else:
-        #         PYTHONPATH = this_pkg_dir
-        # if this == 'test_zerobug':
-        #     this_pkg_dir = '%s/%s' % (self.rundir, 'dummy')
-        #     PYTHONPATH = '%s:%s' % (this_pkg_dir, PYTHONPATH)
-        # os.putenv('PYTHONPATH', PYTHONPATH)
-        # self.PYTHONPATH = PYTHONPATH
         if this_pkg_dir in sys.path:
             ix = sys.path.index(this_pkg_dir)
             del sys.path[ix]
         sys.path.insert(0, this_pkg_dir)
 
         if not id:
             if this.startswith('test_'):
                 id = this[5:]
             elif (
-                # this.startswith('all_tests')
                 this.startswith('zerobug')
                 or this == '__main__'
             ):
                 id = os.path.basename(self.rundir)
             else:
                 id = this
             if id[-3:] >= '_00' and id[-3:] <= '_99':
@@ -483,15 +469,15 @@
             description="Regression test on " + self.module_id,
             epilog="© 2015-2023 by SHS-AV s.r.l."
             " - http://wiki.zeroincombenze.org/en/Zerobug",
         )
         parser.add_argument(
             "-B",
             "--debug",
-            help="trace msgs in zerobug.tracehis",
+            help="run tests in debug mode",
             action="store_true",
             dest="opt_debug",
             default=False,
         )
         parser.add_argument(
             "-C",
             "--no-coverage",
@@ -548,15 +534,15 @@
             action="store_true",
             dest="opt_oelib",
             default=False,
         )
         parser.add_argument(
             "-p",
             "--search-pattern",
-            help="test file pattern",
+            help="pattern to apply for test files (comma separated)",
             dest="opt_pattern",
             metavar="file_list",
             default='',
         )
         parser.add_argument(
             "-Q",
             "--count",
@@ -579,15 +565,15 @@
             help="inner mode w/o final messages",
             action="store_true",
             dest="no_run_on_top",
         )
         parser.add_argument(
             "-r",
             "--restart",
-            help="set to counted tests, 1st one next to this",
+            help="restart count next to number",
             dest="min_test",
             metavar="number",
         )
         parser.add_argument(
             "-s", "--start", help="deprecated", dest="min_test2", metavar="number"
         )
         parser.add_argument("-V", "--version", action="version", version=version)
@@ -637,23 +623,23 @@
             action="store_true",
             dest="run4cover",
             default=True,
         )
         parser.add_argument(
             "-2",
             "--python2",
-            help="use python2",
+            help="use python2 (deprecated)",
             action="store_true",
             dest="python2",
             default=False,
         )
         parser.add_argument(
             "-3",
             "--python3",
-            help="use python3",
+            help="use python3 (deprecated)",
             action="store_true",
             dest="python3",
             default=False,
         )
         return parser
 
     def set_tlog_file(self, ctx):
@@ -959,39 +945,24 @@
             ['sys.executable', '-m', 'doctest', file],
             stdout=FNULL,
             stderr=subprocess.STDOUT,
         )
         return self.test_result(ctx, msg, TEST_SUCCESS, res)
 
     def _exec_tests_4_count(self, test_list, ctx, TestCls=None):
-        # if ctx.get('_run_autotest', False):
-        #     self.dbgmsg(ctx, '>>> exec_tests_4_count(autotest)')
-        # else:
-        #     self.dbgmsg(ctx, '>>> exec_tests_4_count(%s)' % test_list)
         opt4childs = ['-n', '-R']
         ctx = self._ready_opts(ctx)
         ctx = self._save_options(ctx)
         testctr = 0
         if TestCls:
             T = TestCls(self)
             if hasattr(TestCls, 'setup'):
-                # getattr(T, 'setup')(ctx)
+                ctx['dry_run'] = True
                 T.setup(ctx)
         for testname in test_list:
-            # self.dbgmsg(
-            #     ctx,
-            #     '- min=%d, max=%d, ctr=%d, -0=%s, Cover=%s'
-            #     % (
-            #         ctx['min_test'],
-            #         ctx['max_test'],
-            #         ctx['ctr'],
-            #         ctx.get('opt_noctr', False),
-            #         ctx.get('run4cover', False),
-            #     ),
-            # )
             ctx['dry_run'] = True
             basetn = os.path.basename(testname)
             ctx['ctr'] = 0
             if testname.startswith('__test'):
                 ctx['ctr'] = int(testname[7:9])
             elif testname.startswith('__version'):
                 self.test_version(ctx, testname)
@@ -1016,80 +987,58 @@
                 p = Popen(test_w_args, stdin=PIPE, stdout=PIPE, stderr=PIPE)
                 res, err = p.communicate()
                 try:
                     ctx['ctr'] = int(res)
                 except BaseException:  # pragma: no cover
                     ctx['ctr'] = 0
                 self.ctr_list.append(ctx['ctr'])
-            # self.dbgmsg(ctx, '- testctr=%d+%d' % (testctr, ctx['ctr']))
             testctr += ctx['ctr']
         if TestCls and hasattr(TestCls, 'teardown'):
+            ctx['dry_run'] = True
             T.teardown(ctx)
         ctx = self._restore_options(ctx)
         ctx['ctr'] = testctr
         if ctx.get('max_test', 0) == 0:
             ctx['max_test'] = ctx.get('min_test', 0) + testctr
-        # self.dbgmsg(
-        #     ctx,
-        #     '- c=%d, min=%d, max=%d' % (ctx['ctr'], ctx['min_test'], ctx['max_test']),
-        # )
         ctx['_prior_msg'] = ''
         return TEST_SUCCESS
 
     def _exec_all_tests(self, test_list, ctx, TestCls=None):
-        # if ctx.get('_run_autotest', False):
-        #     self.dbgmsg(ctx, '>>> exec_all_tests(autotest)')
-        # else:
-        #     self.dbgmsg(ctx, '>>> exec_all_tests()')
         ctx = self._ready_opts(ctx)
         if (
             not ctx.get('_run_autotest', False)
             and ctx.get('run4cover', False)
             and not os.path.isfile(ctx['COVERAGE_PROCESS_START'])
         ):
             with open(ctx['COVERAGE_PROCESS_START'], 'w') as fd:
                 fd.write(DEFAULT_COVERARC)
         ix = 0
         sts = 0
         ctx['ctr'] = ctx['min_test']
-        # self.dbgmsg(ctx, '- c=%d, ctr_list=%s' % (ctx['ctr'], self.ctr_list))
+
         if TestCls:
             T = TestCls(self)
         if TestCls and hasattr(TestCls, 'setup'):
             T.setup(ctx)
         for testname in test_list:
-            # self.dbgmsg(
-            #     ctx,
-            #     '- min=%d, max=%d, ctr=%d, -0=%s, Cover=%s'
-            #     % (
-            #         ctx['min_test'],
-            #         ctx['max_test'],
-            #         ctx['ctr'],
-            #         ctx.get('opt_noctr', False),
-            #         ctx.get('run4cover', False),
-            #     ),
-            # )
             opt4childs = self._inherit_opts(ctx)
             basetn = os.path.basename(testname)
             if testname.startswith('__test'):
                 sts = self.test_result(ctx, testname, True, True)
             elif testname.startswith('__version'):
                 sts = self.test_version(ctx, testname)
             elif testname.startswith('__doctest'):
                 self.doctest(ctx, testname)
             elif TestCls and hasattr(TestCls, testname):
-                # if ctx.get('opt_debug', False):
-                #     self.dbgmsg(ctx, ">>> %s()" % testname)
                 sts = getattr(T, testname)(ctx)
             elif os.path.splitext(basetn)[0] != ctx['this']:
                 mime = magic.Magic(mime=True).from_file(os.path.realpath(testname))
                 if os.path.dirname(testname) == "":
                     testname = os.path.join(self.testdir, testname)
                 if mime == 'text/x-python':
-                    # self.dbgmsg(ctx, '- ctr=%d' % ctx['ctr'])
                     if os.environ.get('TRAVIS_PDB') == 'true':
                         if ctx.get('python3', False):
                             test_w_args = [
                                 'python3',
                                 '-m',
                                 'pdb',
                                 testname,
@@ -1120,21 +1069,19 @@
                     else:
                         if ctx.get('python3', False):
                             test_w_args = ['python3'] + [testname] + opt4childs
                         elif ctx.get('python2', False):
                             test_w_args = ['python2'] + [testname] + opt4childs
                         else:
                             test_w_args = [sys.executable] + [testname] + opt4childs
-                    # self.dbgmsg(ctx, ">>> subprocess.call(%s)" % test_w_args)
                     try:
                         sts = subprocess.call(test_w_args)
                     except OSError:
                         sts = 127
                 else:
-                    # self.dbgmsg(ctx, ">>> %s(%s)" % (testname, opt4childs))
                     test_w_args = [testname] + opt4childs
                     try:
                         sts = subprocess.call(test_w_args)
                     except OSError:
                         sts = 127
                 if not ctx.get('opt_noctr', False):
                     ctx['ctr'] += self.ctr_list[ix]
@@ -1150,21 +1097,14 @@
     def main_local(self, ctx, Test, UT1=None, UT=None):
         """Default main program for local tests"""
         # self.dbgmsg(ctx, '>>> main_local(%s)' % Test)
         test_list = sorted(
             [meth for meth in dir(Test)
              if meth.startswith("test_") and callable(getattr(Test, meth))]
         )
-        # test_num = 0
-        # test_list = []
-        # for _i in range(MAX_TEST_NUM):
-        #     tname = "test_{:02}".format(test_num)
-        #     if hasattr(Test, tname):
-        #         test_list.append(tname)
-        #     test_num += 1
         if not ctx.get('opt_noctr', False):
             self._exec_tests_4_count(test_list, ctx, Test)
         if ctx.get('dry_run', False):
             if not ctx.get('_run_autotest', False):
                 print(ctx['max_test'])
             sts = TEST_SUCCESS
         else:
@@ -1178,31 +1118,14 @@
         ctx: context
         Test: test class for internal tests;
               if supplied only internal tests are executed
         UT1: protected Unit Test list (w/o log)
         UT: Unit Test list (if None, search for files)
         """
         ctx = self._ready_opts(ctx)
-        # if (
-        #     ctx.get('opt_debug', False)
-        #     and ctx.get('run_on_top', False)
-        #     and not ctx.get('_run_autotest', False)
-        # ):
-        #     self.dbgmsg(ctx, "# Test tree of %s!" % self.module_id)
-        # self.dbgmsg(ctx, '>>> main()')
-        # self.dbgmsg(
-        #     ctx,
-        #     '- min=%s, max=%s, -0=%s, Cover=%s'
-        #     % (
-        #         ctx.get('min_test', None),
-        #         ctx.get('max_test', None),
-        #         ctx.get('opt_noctr', False),
-        #         ctx.get('run4cover', False),
-        #     ),
-        # )
         # Execute sanity check on test library (no if zerobug testing itself)
         if (
             ctx['this'] != 'test_zerobug'
             and ctx.get('run_on_top', False)
             and not ctx.get('_run_autotest', False)
         ):
             if ctx.get('run4cover', False) and not ctx.get('dry_run', False):
@@ -1221,33 +1144,29 @@
             test_list = UT
         elif not ctx.get('_run_autotest', False):
             # Discover test files
             test_list = []
             for pattern in (
                 ctx['opt_pattern'] and ctx['opt_pattern'].split(',') or self.pattern
             ):
-                # self.dbgmsg(ctx, '- Search for files %s' % pattern)
-                test_files = os.path.abspath(os.path.join(self.testdir, pattern))
-                for fn in sorted(glob.glob(test_files)):
+                t_list = glob.glob(os.path.abspath(os.path.join(self.testdir, pattern)))
+                if not pattern.endswith(".py") and not pattern.endswith(".sh"):
+                    t_list += glob.glob(os.path.abspath(os.path.join(self.testdir,
+                                                                     pattern + ".py")))
+                    t_list += glob.glob(os.path.abspath(os.path.join(self.testdir,
+                                                                     pattern + ".sh")))
+                for fn in sorted(t_list):
                     mime = magic.Magic(mime=True).from_file(os.path.realpath(fn))
                     if mime in ('text/x-python', 'text/x-shellscript'):
                         test_list.append(fn)
         if len(test_list) == 0 and Test is not None:
-            # self.dbgmsg(ctx, '- len(test_list) == 0 ')
             test_list = sorted(
                 [meth for meth in dir(Test)
                  if meth.startswith("test_") and callable(getattr(Test, meth))]
             )
-            # test_num = 0
-            # for _i in range(MAX_TEST_NUM):
-            #     tname = "test_{:02}".format(test_num)
-            #     if hasattr(Test, tname):
-            #         test_list.append(tname)
-            #     test_num += 1
-        # self.dbgmsg(ctx, '- test_list=%s' % test_list)
         if not ctx.get('opt_noctr', False):
             self._exec_tests_4_count(test_list, ctx, Test)
         if ctx.get('dry_run', False):
             if not ctx.get('_run_autotest', False):
                 print(ctx['ctr'])
             sts = TEST_SUCCESS
         else:
@@ -1265,24 +1184,15 @@
                             ['coverage', 'report', '--show-missing'],
                         )
                     except OSError:
                         print('Coverage not found!')
                         ctx['run4cover'] = False
         return sts
 
-    # def dbgmsg(self, ctx, msg, echo=None):
-    #     # if ctx.get('opt_debug', False):
-    #     #     fmode = 'w' if msg[0] == "!" else 'a'
-    #     #     with open(os.path.join(self.testdir, 'z0bug.tracehis'), fmode) as fd:
-    #     #         fd.write("%s> %s\n" % (os.path.basename(ctx['this_fqn']), msg))
-    #     if echo:
-    #         print('#DEBUG>>> %s' % msg)
-
     def msg_test(self, ctx, msg):
-        # ctx = self.ready_opts(ctx)
         if msg == ctx['_prior_msg']:
             # NEWLN = False
             prfx = "\x1b[A"
         else:
             # NEWLN = True
             prfx = ""
             ctx['_prior_msg'] = msg
@@ -1301,18 +1211,14 @@
                     txt = "{}Test {}/{}: {}".format(
                         prfx, ctx['ctr'], ctx['max_test'], msg
                     )
                 else:
                     txt = "{}Test {}: {}".format(prfx, ctx['ctr'], msg)
                 os0.wlog(txt)
 
-    # def test_result(self, ctx, msg, test_value, result_value):
-    #     print("Function test_result() deprecated! Please use assertEqual()")
-    #     return assertEqual(test_value, result_value, message=msg)
-
     def test_result(self, ctx, msg, test_value, result_val):
         ctx = self._ready_opts(ctx)
         ctx['ctr'] += 1
         if ctx.get('teststs', TEST_SUCCESS):  # pragma: no cover
             return TEST_FAILED
         self.msg_test(ctx, msg)
         if not ctx.get('dry_run', False):
```

### Comparing `zerobug-2.0.6/zerobug/zerobug.py` & `zerobug-2.0.7/zerobug/zerobug.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 """
     Zeroincombenze® unit test library for python programs Regression Test Suite
 """
 import sys
 from . import z0test
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 
 def version():
     return __version__
 
 
 def main(cli_args=None):
```

### Comparing `zerobug-2.0.6/zerobug.egg-info/SOURCES.txt` & `zerobug-2.0.7/zerobug.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.6/README.rst` & `zerobug-2.0.7/zerobug.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,522 +1,390 @@
-
-=============
-zerobug 2.0.6
-=============
-
-
-
-|Maturity| |Build Status| |Coverage Status| |license gpl|
-
-
-
-
-Overview
-========
-
-Zeroincombenze® continuous testing framework for python and bash programs
--------------------------------------------------------------------------
-
-This library can run unit test of target package software.
-Supported languages are *python* (through z0testlib.py) and *bash* (through z0testrc)
-
-*zerobug* supports test automation, aggregation of tests into collections
-and independence of the tests from the reporting framework.
-The *zerobug* module provides all code that make it easy to support testing
-both for python programs both for bash scripts.
-*zerobug* shows execution test with a message like "n/tot message"
-where *n* is current unit test and *tot* is the total unit test to execute,
-that is a sort of advancing test progress.
-
-You can use z0bug_odoo that is the odoo integration to test Odoo modules.
-
-*zerobug* is built on follow concepts:
-
-* test main - it is a main program to executes all test runners
-* test runner - it is a program to executes one or more test suites
-* test suite - it is a collection of test cases
-* test case - it is a smallest unit test
-
-The main file is the command **zerobug** of this package; it searches for test runner files
-named `[id_]test_` where 'id' is the shor name of testing package.
-
-Test suite is a collection of test case named `test_[0-9]+` inside the runner file,
-executed in sorted order.
-
-Every suit can contains one or more test case, the smallest unit test;
-every unit test terminates with success or with failure.
-
-Because **zerobug** can show total number of unit test to execute, it runs tests
-in 2 passes. In the first pass it counts the number of test, in second pass executes really
-it. This behavior can be overridden by -0 switch.
-
-
-
-
-
-
-
-|
-
-Features
---------
-
-* Test execution log
-* Autodiscovery test modules and functions
-* Python 2.7+ and 3.5+
-* coverage integration
-* travis integration
-
-
-|
-
-Usage
-=====
-
-::
-
-    usage: zerobug [-h] [-B] [-C] [-e] [-J] [-k] [-l file] [-N] [-n] [-O]
-                   [-p file_list] [-q] [-r number] [-s number] [-V] [-v] [-x] [-X]
-                   [-z number] [-0] [-1] [-3]
-
-    Regression test on z0bug_odoo
-
-    optional arguments:
-      -h, --help            show this help message and exit
-      -B, --debug           trace msgs in zerobug.tracehis
-      -C, --no-coverage     run tests without coverage
-      -e, --echo            enable echoing even if not interactive tty
-      -J                    load travisrc
-      -k, --keep            keep current logfile
-      -l file, --logname file
-                            set logfile name
-      -N, --new             create new logfile
-      -n, --dry-run         count and display # unit tests
-      -O                    load odoorc
-      -p file_list, --search-pattern file_list
-                            test file pattern
-      -q, --quiet           run tests without output (quiet mode)
-      -r number, --restart number
-                            set to counted tests, 1st one next to this
-      -s number, --start number
-                            deprecated
-      -V, --version         show program's version number and exit
-      -v, --verbose         verbose mode
-      -x, --qsanity         like -X but run silently
-      -X, --esanity         execute test library sanity check and exit
-      -z number, --end number
-                            display total # tests when execute them
-      -0, --no-count        no count # unit tests
-      -1, --coverage        run tests for coverage (obsolete)
-      -3, --python3         use python3
-
-
-Code example
-~~~~~~~~~~~~
-
-*zerobug* makes avaiable following functions to test:
-
-|
-
-`Z0BUG.setup(ctx)` (python)
-
-`Z0BUG_setup` (bash)
-
-Setup for test. It is called before all tests.
-
-|
-
-`Z0BUG.teardown(ctx)` (python)
-
-`Z0BUG_teardown` (bash)
-
-Setup for test. It is called after all tests.
-
-|
-
-`Z0BUG.build_os_tree(ctx, list_of_paths)` (python)
-
-`Z0BUG_build_os_tree list_of_paths` (bash)
-
-Build a full os tree from supplied list.
-If python, list of paths is a list of strings.
-If bash, list is one string of paths separated by spaces.
-Function reads list of paths and then create all directories.
-If directory is an absolute path, it is created with the supplied path.
-If directory is a relative path, the directory is created under "tests/res" directory.
-
-Warning!
-To check is made is parent dir does not exit. Please, supply path from parent
-to children, if you want to build a nested tree.
-
-::
-
-    # (python)
-    from zerobug import Z0BUG
-    class RegressionTest():
-
-        def __init__(self, Z0BUG):
-            self.Z0BUG = Z0BUG
-
-        def test_01(self, ctx):
-            os_tree = ['10.0',
-                       '10.0/addons',
-                       '10.0/odoo',]
-            root = self.Z0BUG.build_os_tree(ctx, os_tree)
-
-::
-
-    # (bash)
-    Z0BUG_setup() {
-        Z0BUG_build_os_tree "10.0 10.0/addons 10.0/odoo"
-    }
-
-|
-
-`Z0BUG.remove_os_tree(ctx, list_of_paths)` (python)
-
-`Z0BUG_remove_os_tree list_of_paths` (bash)
-
-Remove a full os tree created by `build_os_tree`
-If python, list of paths is a list of strings.
-If bash, list is a string of paths separated by spaces.
-Function reads list of paths and remove all directories.
-If directory is an absolute path, the supplied path is dropped.
-If directory is a relative path, the directory is dropped from tests/res directory.
-
-Warning!
-This function remove directory and all sub-directories without any control.
-
-::
-
-    # (python)
-    from zerobug import Z0BUG
-    class RegressionTest():
-
-        def __init__(self, Z0BUG):
-            self.Z0BUG = Z0BUG
-
-        def test_01(self, ctx):
-            os_tree = ['10.0',
-                       '10.0/addons',
-                       '10.0/odoo',]
-            root = self.Z0BUG.remove_os_tree(ctx, os_tree)
-
-|
-
-`Z0BUG.build_odoo_env(ctx, version)` (python)
-
-Like build_os_tree but create a specific odoo os tree.
-
-::
-
-    # (python)
-    from zerobug import Z0BUG
-    from zerobug import Z0testOdoo
-    class RegressionTest():
-
-        def __init__(self, Z0BUG):
-            self.Z0BUG = Z0BUG
-
-        def test_01(self, ctx):
-            root = Z0testOdoo.build_odoo_env(ctx, '10.0')
-
-|
-
-`Z0BUG.git_clone(remote, reponame, branch, odoo_path, force=None)` (python)
-
-Execute git clone of `remote:reponame:branch` into local directory `odoo_path`.
-In local travis emulation, if repository uses local repository, if exists.
-Return odoo root directory
-
-::
-
-    # (python)
-    from zerobug import Z0BUG
-    from zerobug import Z0testOdoo
-
-    from zerobug import Z0BUG
-    class RegressionTest():
-
-        def __init__(self, Z0BUG):
-            self.Z0BUG = Z0BUG
-
-        def test_01(self, ctx):
-            remote = 'OCA'
-            reponame = 'OCB'
-            branch = '10.0'
-            odoo_path = '/opt/odoo/10.0'
-            Z0testOdoo.git_clone(remote, reponame, branch, odoo_path)
-
-
-
-
-Unit test can run in package directory or in ./tests directory of package.
-
-Every test can inquire internal context.
-
-::
-
-    this_fqn      parent caller full qualified name (i.e. /opt/odoo/z0bug.pyc)
-    this          parent name, w/o extension (i.e. z0bug)
-    ctr           test counter [both bash and python tests]
-    dry_run       dry-run (do nothing) [opt_dry_run in bash test]          "-n"
-    esanity       True if required sanity check with echo                  "-X"
-    max_test      # of tests to execute [both bash and python tests]       "-z"
-    min_test      # of test executed before this one                       "-r"
-    on_error      behavior after error, 'continue' or 'raise' (default)
-    opt_echo      True if echo test result onto std output                 "-e"
-    opt_new       new log file [both bash and python tests]                "-N"
-    opt_noctr     do not count # tests [both bash and python tests]        "-0"
-    opt_verbose   show messages during execution                           "-v"
-    logfn         real trace log file name from switch                     "-l"
-    qsanity       True if required sanity check w/o echo                   "-x"
-    run4cover     Run tests for coverage (use coverage run rather python)  "-C"
-    python3       Execute test in python3                                  "-3"
-    run_daemon    True if execution w/o tty as stdio
-    run_on_top    Top test (not parent)
-    run_tty       Opposite of run_daemon
-    tlog          default tracelog file name
-    _run_autotest True if running auto-test
-    _parser       cmd line parser
-    _opt_obj      parser obj, to acquire optional switches
-    WLOGCMD       override opt_echo; may be None, 'echo', 'echo-1', 'echo-0'
-    Z0            this library object
-
-Environment read:
-
-DEV_ENVIRONMENT Name of package; if set test is under travis emulator control
-
-COVERAGE_PROCESS_START
-                Name of coverage conf file; if set test is running for coverage
-
-
-
-|
-|
-
-Getting started
-===============
-
-
-|
-
-Installation
-------------
-
-Installation
-------------
-
-Zeroincombenze tools require:
-
-* Linux Centos 7/8 or Debian 9/10 or Ubuntu 18/20
-* python 2.7, some tools require python 3.6+
-* bash 5.0+
-
-Stable version via Python Package
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-    pip install zerobug
-
-|
-
-Current version via Git
-~~~~~~~~~~~~~~~~~~~~~~~
-
-::
-
-    cd $HOME
-    git clone https://github.com/zeroincombenze/tools.git
-    cd ./tools
-    ./install_tools.sh -p
-    source /opt/odoo/devel/activate_tools
-
-
-Upgrade
--------
-
-Upgrade
--------
-
-Stable version via Python Package
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-    pip install zerobug -U
-
-|
-
-Current stable version
-~~~~~~~~~~~~~~~~~~~~~~
-
-::
-
-    cd $HOME
-    ./install_tools.sh -U
-    source /opt/odoo/devel/activate_tools
-
-Current development version
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-::
-
-    cd $HOME
-    ./install_tools.sh -Ud
-    source /opt/odoo/devel/activate_tools
-
-
-History
--------
-
-2.0.6 (2023-05-08)
-~~~~~~~~~~~~~~~~~~
-
-* [IMP] Now all_tests is ignored
-* [IMP] Build Odoo environment for Odoo 16.0
-
-2.0.5 (2023-03-24)
-~~~~~~~~~~~~~~~~~~
-
-* [FIX] travis_install_env: ensure list_requirements is executable
-* [IMP] flake8 configuration
-* [IMP] coveralls and codecov are not more dependencies
-* [IMP] Test for Odoo 16.0
-
-2.0.4 (2022-12-08)
-~~~~~~~~~~~~~~~~~~
-
-* [FIX] run_pypi_test: best recognition of python version
-* [FIX] build_cmd: best recognition of python version
-* [FIX] travis_install_env: ensure coverage version
-* [IMP] odoo environment to test more precise
-
-2.0.3 (2022-11-08)
-~~~~~~~~~~~~~~~~~~
-
-* [IMP] npm management
-
-2.0.2.1 (2022-10-31)
-~~~~~~~~~~~~~~~~~~~~
-
-* [FIX] Odoo 11.0+
-* [FIX] Ensure coverage 5.0+
-
-2.0.2 (2022-10-20)
-~~~~~~~~~~~~~~~~~~
-
-* [IMP] Stable version
-
-2.0.1.1 (2022-10-12)
-~~~~~~~~~~~~~~~~~~~~
-
-* [IMP] minor improvements
-
-2.0.1 (2022-10-12)
-~~~~~~~~~~~~~~~~~~
-
-* [IMP] stable version
-
-2.0.0.2 (2022-10-05)
-~~~~~~~~~~~~~~~~~~~~
-
-* [IMP] travis_install_env: python2 tests
-
-2.0.0.1 (2022-09-06)
-~~~~~~~~~~~~~~~~~~~~
-
-* [FIX] travis_install_env: minor fixes
-* [IMP] z0testlib: show coverage result
-
-
-2.0.0 (2022-08-10)
-~~~~~~~~~~~~~~~~~~
-
-* [REF] Partial refactoring for shell scripts
-
-
-
-|
-|
-
-Credits
-=======
-
-Copyright
----------
-
-SHS-AV s.r.l. <https://www.shs-av.com/>
-
-
-Contributors
-------------
-
-* Antonio Maria Vigliotti <antoniomaria.vigliotti@gmail.com>
-Contributors
-------------
-
-
-
-|
-
-This module is part of tools project.
-
-Last Update / Ultimo aggiornamento: 2023-05-09
-
-.. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
-    :target: https://odoo-community.org/page/development-status
-    :alt: 
-.. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
-    :target: https://travis-ci.com/zeroincombenze/tools
-    :alt: github.com
-.. |license gpl| image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
-    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
-    :alt: License: AGPL-3
-.. |license opl| image:: https://img.shields.io/badge/licence-OPL-7379c3.svg
-    :target: https://www.odoo.com/documentation/user/9.0/legal/licenses/licenses.html
-    :alt: License: OPL
-.. |Coverage Status| image:: https://coveralls.io/repos/github/zeroincombenze/tools/badge.svg?branch=master
-    :target: https://coveralls.io/github/zeroincombenze/tools?branch=2.0
-    :alt: Coverage
-.. |Codecov Status| image:: https://codecov.io/gh/zeroincombenze/tools/branch/2.0/graph/badge.svg
-    :target: https://codecov.io/gh/zeroincombenze/tools/branch/2.0
-    :alt: Codecov
-.. |Tech Doc| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-2.svg
-    :target: https://wiki.zeroincombenze.org/en/Odoo/2.0/dev
-    :alt: Technical Documentation
-.. |Help| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-2.svg
-    :target: https://wiki.zeroincombenze.org/it/Odoo/2.0/man
-    :alt: Technical Documentation
-.. |Try Me| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-2.svg
-    :target: https://erp2.zeroincombenze.it
-    :alt: Try Me
-.. |OCA Codecov| image:: https://codecov.io/gh/OCA/tools/branch/2.0/graph/badge.svg
-    :target: https://codecov.io/gh/OCA/tools/branch/2.0
-    :alt: Codecov
-.. |Odoo Italia Associazione| image:: https://www.odoo-italia.org/images/Immagini/Odoo%20Italia%20-%20126x56.png
-   :target: https://odoo-italia.org
-   :alt: Odoo Italia Associazione
-.. |Zeroincombenze| image:: https://avatars0.githubusercontent.com/u/6972555?s=460&v=4
-   :target: https://www.zeroincombenze.it/
-   :alt: Zeroincombenze
-.. |en| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/en_US.png
-   :target: https://www.facebook.com/Zeroincombenze-Software-gestionale-online-249494305219415/
-.. |it| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/it_IT.png
-   :target: https://www.facebook.com/Zeroincombenze-Software-gestionale-online-249494305219415/
-.. |check| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/check.png
-.. |no_check| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/no_check.png
-.. |menu| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/menu.png
-.. |right_do| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/right_do.png
-.. |exclamation| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/exclamation.png
-.. |warning| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/warning.png
-.. |same| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/same.png
-.. |late| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/late.png
-.. |halt| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/halt.png
-.. |info| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/info.png
-.. |xml_schema| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/certificates/iso/icons/xml-schema.png
-   :target: https://github.com/zeroincombenze/grymb/blob/master/certificates/iso/scope/xml-schema.md
-.. |DesktopTelematico| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/certificates/ade/icons/DesktopTelematico.png
-   :target: https://github.com/zeroincombenze/grymb/blob/master/certificates/ade/scope/Desktoptelematico.md
-.. |FatturaPA| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/certificates/ade/icons/fatturapa.png
-   :target: https://github.com/zeroincombenze/grymb/blob/master/certificates/ade/scope/fatturapa.md
-.. |chat_with_us| image:: https://www.shs-av.com/wp-content/chat_with_us.gif
-   :target: https://t.me/Assitenza_clienti_powERP
-
-
+Metadata-Version: 1.2
+Name: zerobug
+Version: 2.0.7
+Summary: Zeroincombenze continuous testing framework and tools for python and bash programs
+Home-page: https://github.com/zeroincombenze/tools
+Author: Antonio Maria Vigliotti
+Author-email: <info@shs-av.com>
+License: Affero GPL
+Project-URL: Source, https://github.com/zeroincombenze/tools/tree/master/zerobug
+Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io/en/latest/zerobug
+Project-URL: Changelog, https://github.com/zeroincombenze/tools/blob/master/zerobug/egg-info/CHANGELOG.rst
+Description: 
+        =============
+        zerobug 2.0.7
+        =============
+        
+        
+        
+        |Maturity| |Build Status| |Coverage Status| |license gpl|
+        
+        
+        
+        
+        Overview
+        ========
+        
+        
+        
+        
+        
+        
+        
+        
+        |
+        
+        Features
+        --------
+        
+        * Test execution log
+        * Autodiscovery test modules and functions
+        * Python 2.7+ and 3.5+
+        * coverage integration
+        * travis integration
+        
+        
+        |
+        
+        Usage
+        =====
+        
+        
+        
+        Code example
+        ------------
+        
+        *zerobug* makes avaiable following functions to test:
+        
+        |
+        
+        `Z0BUG.setup(ctx)` (python)
+        
+        `Z0BUG_setup` (bash)
+        
+        Setup for test. It is called before all tests.
+        
+        |
+        
+        `Z0BUG.teardown(ctx)` (python)
+        
+        `Z0BUG_teardown` (bash)
+        
+        Setup for test. It is called after all tests.
+        
+        |
+        
+        `Z0BUG.build_os_tree(ctx, list_of_paths)` (python)
+        
+        `Z0BUG_build_os_tree list_of_paths` (bash)
+        
+        Build a full os tree from supplied list.
+        If python, list of paths is a list of strings.
+        If bash, list is one string of paths separated by spaces.
+        Function reads list of paths and then create all directories.
+        If directory is an absolute path, it is created with the supplied path.
+        If directory is a relative path, the directory is created under "tests/res" directory.
+        
+        Warning!
+        To check is made is parent dir does not exit. Please, supply path from parent
+        to children, if you want to build a nested tree.
+        
+        ::
+        
+            # (python)
+            from zerobug import Z0BUG
+            class RegressionTest():
+        
+                def __init__(self, Z0BUG):
+                    self.Z0BUG = Z0BUG
+        
+                def test_01(self, ctx):
+                    os_tree = ['10.0',
+                               '10.0/addons',
+                               '10.0/odoo',]
+                    root = self.Z0BUG.build_os_tree(ctx, os_tree)
+        
+        ::
+        
+            # (bash)
+            Z0BUG_setup() {
+                Z0BUG_build_os_tree "10.0 10.0/addons 10.0/odoo"
+            }
+        
+        |
+        
+        `Z0BUG.remove_os_tree(ctx, list_of_paths)` (python)
+        
+        `Z0BUG_remove_os_tree list_of_paths` (bash)
+        
+        Remove a full os tree created by `build_os_tree`
+        If python, list of paths is a list of strings.
+        If bash, list is a string of paths separated by spaces.
+        Function reads list of paths and remove all directories.
+        If directory is an absolute path, the supplied path is dropped.
+        If directory is a relative path, the directory is dropped from tests/res directory.
+        
+        Warning!
+        This function remove directory and all sub-directories without any control.
+        
+        ::
+        
+            # (python)
+            from zerobug import Z0BUG
+            class RegressionTest():
+        
+                def __init__(self, Z0BUG):
+                    self.Z0BUG = Z0BUG
+        
+                def test_01(self, ctx):
+                    os_tree = ['10.0',
+                               '10.0/addons',
+                               '10.0/odoo',]
+                    root = self.Z0BUG.remove_os_tree(ctx, os_tree)
+        
+        |
+        
+        `Z0BUG.build_odoo_env(ctx, version)` (python)
+        
+        Like build_os_tree but create a specific odoo os tree.
+        
+        ::
+        
+            # (python)
+            from zerobug import Z0BUG
+            from zerobug import Z0testOdoo
+            class RegressionTest():
+        
+                def __init__(self, Z0BUG):
+                    self.Z0BUG = Z0BUG
+        
+                def test_01(self, ctx):
+                    root = Z0testOdoo.build_odoo_env(ctx, '10.0')
+        
+        |
+        
+        `Z0BUG.git_clone(remote, reponame, branch, odoo_path, force=None)` (python)
+        
+        Execute git clone of `remote:reponame:branch` into local directory `odoo_path`.
+        In local travis emulation, if repository uses local repository, if exists.
+        Return odoo root directory
+        
+        ::
+        
+            # (python)
+            from zerobug import Z0BUG
+            from zerobug import Z0testOdoo
+        
+            from zerobug import Z0BUG
+            class RegressionTest():
+        
+                def __init__(self, Z0BUG):
+                    self.Z0BUG = Z0BUG
+        
+                def test_01(self, ctx):
+                    remote = 'OCA'
+                    reponame = 'OCB'
+                    branch = '10.0'
+                    odoo_path = '/opt/odoo/10.0'
+                    Z0testOdoo.git_clone(remote, reponame, branch, odoo_path)
+        
+        
+        
+        
+        Unit test can run in package directory or in ./tests directory of package.
+        
+        Every test can inquire internal context.
+        
+        ::
+        
+            this_fqn      parent caller full qualified name (i.e. /opt/odoo/z0bug.pyc)
+            this          parent name, w/o extension (i.e. z0bug)
+            ctr           test counter [both bash and python tests]
+            dry_run       dry-run (do nothing) [opt_dry_run in bash test]          "-n"
+            esanity       True if required sanity check with echo                  "-X"
+            max_test      # of tests to execute [both bash and python tests]       "-z"
+            min_test      # of test executed before this one                       "-r"
+            on_error      behavior after error, 'continue' or 'raise' (default)
+            opt_echo      True if echo test result onto std output                 "-e"
+            opt_new       new log file [both bash and python tests]                "-N"
+            opt_noctr     do not count # tests [both bash and python tests]        "-0"
+            opt_verbose   show messages during execution                           "-v"
+            logfn         real trace log file name from switch                     "-l"
+            qsanity       True if required sanity check w/o echo                   "-x"
+            run4cover     Run tests for coverage (use coverage run rather python)  "-C"
+            python3       Execute test in python3                                  "-3"
+            run_daemon    True if execution w/o tty as stdio
+            run_on_top    Top test (not parent)
+            run_tty       Opposite of run_daemon
+            tlog          default tracelog file name
+            _run_autotest True if running auto-test
+            _parser       cmd line parser
+            _opt_obj      parser obj, to acquire optional switches
+            WLOGCMD       override opt_echo; may be None, 'echo', 'echo-1', 'echo-0'
+            Z0            this library object
+        
+        Environment read:
+        
+        DEV_ENVIRONMENT Name of package; if set test is under travis emulator control
+        
+        COVERAGE_PROCESS_START
+                        Name of coverage conf file; if set test is running for coverage
+        
+        
+        
+        |
+        |
+        
+        Getting started
+        ===============
+        
+        
+        Installation
+        ------------
+        
+        Zeroincombenze tools require:
+        
+        * Linux Centos 7/8 or Debian 9/10 or Ubuntu 18/20/22
+        * python 2.7+, some tools require python 3.6+
+        * bash 5.0+
+        
+        Stable version via Python Package
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        ::
+        
+            pip install zerobug
+        
+        |
+        
+        Current version via Git
+        ~~~~~~~~~~~~~~~~~~~~~~~
+        
+        ::
+        
+            cd $HOME
+            git clone https://github.com/zeroincombenze/tools.git
+            cd ./tools
+            ./install_tools.sh -p
+            source $HOME/devel/activate_tools
+        
+        
+        Upgrade
+        -------
+        
+        Stable version via Python Package
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        ::
+        
+            pip install zerobug -U
+        
+        |
+        
+        Current version via Git
+        ~~~~~~~~~~~~~~~~~~~~~~~
+        
+        ::
+        
+            cd $HOME
+            ./install_tools.sh -U
+            source $HOME/devel/activate_tools
+        
+        
+        |
+        |
+        
+        Credits
+        =======
+        
+        Copyright
+        ---------
+        
+        SHS-AV s.r.l. <https://www.shs-av.com/>
+        
+        
+        Contributors
+        ------------
+        
+        * Antonio Maria Vigliotti <antoniomaria.vigliotti@gmail.com>
+        
+        |
+        
+        This module is part of tools project.
+        
+        Last Update / Ultimo aggiornamento: 2023-05-21
+        
+        .. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
+            :target: https://odoo-community.org/page/development-status
+            :alt:
+        .. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
+            :target: https://travis-ci.com/zeroincombenze/tools
+            :alt: github.com
+        .. |license gpl| image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
+            :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
+            :alt: License: AGPL-3
+        .. |license opl| image:: https://img.shields.io/badge/licence-OPL-7379c3.svg
+            :target: https://www.odoo.com/documentation/user/9.0/legal/licenses/licenses.html
+            :alt: License: OPL
+        .. |Coverage Status| image:: https://coveralls.io/repos/github/zeroincombenze/tools/badge.svg?branch=master
+            :target: https://coveralls.io/github/zeroincombenze/tools?branch=2.0
+            :alt: Coverage
+        .. |Codecov Status| image:: https://codecov.io/gh/zeroincombenze/tools/branch/2.0/graph/badge.svg
+            :target: https://codecov.io/gh/zeroincombenze/tools/branch/2.0
+            :alt: Codecov
+        .. |Tech Doc| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-2.svg
+            :target: https://wiki.zeroincombenze.org/en/Odoo/2.0/dev
+            :alt: Technical Documentation
+        .. |Help| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-2.svg
+            :target: https://wiki.zeroincombenze.org/it/Odoo/2.0/man
+            :alt: Technical Documentation
+        .. |Try Me| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-2.svg
+            :target: https://erp2.zeroincombenze.it
+            :alt: Try Me
+        .. |OCA Codecov| image:: https://codecov.io/gh/OCA/tools/branch/2.0/graph/badge.svg
+            :target: https://codecov.io/gh/OCA/tools/branch/2.0
+            :alt: Codecov
+        .. |Odoo Italia Associazione| image:: https://www.odoo-italia.org/images/Immagini/Odoo%20Italia%20-%20126x56.png
+           :target: https://odoo-italia.org
+           :alt: Odoo Italia Associazione
+        .. |Zeroincombenze| image:: https://avatars0.githubusercontent.com/u/6972555?s=460&v=4
+           :target: https://www.zeroincombenze.it/
+           :alt: Zeroincombenze
+        .. |en| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/en_US.png
+           :target: https://www.facebook.com/Zeroincombenze-Software-gestionale-online-249494305219415/
+        .. |it| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/it_IT.png
+           :target: https://www.facebook.com/Zeroincombenze-Software-gestionale-online-249494305219415/
+        .. |check| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/check.png
+        .. |no_check| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/no_check.png
+        .. |menu| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/menu.png
+        .. |right_do| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/right_do.png
+        .. |exclamation| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/exclamation.png
+        .. |warning| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/warning.png
+        .. |same| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/same.png
+        .. |late| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/late.png
+        .. |halt| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/halt.png
+        .. |info| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/info.png
+        .. |xml_schema| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/certificates/iso/icons/xml-schema.png
+           :target: https://github.com/zeroincombenze/grymb/blob/master/certificates/iso/scope/xml-schema.md
+        .. |DesktopTelematico| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/certificates/ade/icons/DesktopTelematico.png
+           :target: https://github.com/zeroincombenze/grymb/blob/master/certificates/ade/scope/Desktoptelematico.md
+        .. |FatturaPA| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/certificates/ade/icons/fatturapa.png
+           :target: https://github.com/zeroincombenze/grymb/blob/master/certificates/ade/scope/fatturapa.md
+        .. |chat_with_us| image:: https://www.shs-av.com/wp-content/chat_with_us.gif
+           :target: https://t.me/Assitenza_clienti_powERP
+        
+        
+        
+Keywords: bash,optargs
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: System :: System Shells
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

