# Comparing `tmp/adafruit-circuitpython-ble-radio-0.5.7.tar.gz` & `tmp/adafruit-circuitpython-ble-radio-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ble-radio-0.5.7.tar", last modified: Fri Aug 26 02:28:53 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ble-radio-0.5.8.tar", last modified: Thu May 25 15:38:16 2023, max compression
```

## Comparing `adafruit-circuitpython-ble-radio-0.5.7.tar` & `adafruit-circuitpython-ble-radio-0.5.8.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:28:53.965732 adafruit-circuitpython-ble-radio-0.5.7/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:28:53.953732 adafruit-circuitpython-ble-radio-0.5.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:28:53.957732 adafruit-circuitpython-ble-radio-0.5.7/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:28:53.957732 adafruit-circuitpython-ble-radio-0.5.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:28:53.957732 adafruit-circuitpython-ble-radio-0.5.7/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3954 2022-08-26 02:28:53.965732 adafruit-circuitpython-ble-radio-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3197 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     7837 2022-08-26 02:28:41.000000 adafruit-circuitpython-ble-radio-0.5.7/adafruit_ble_radio.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:28:53.957732 adafruit-circuitpython-ble-radio-0.5.7/adafruit_circuitpython_ble_radio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3954 2022-08-26 02:28:53.000000 adafruit-circuitpython-ble-radio-0.5.7/adafruit_circuitpython_ble_radio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-08-26 02:28:53.000000 adafruit-circuitpython-ble-radio-0.5.7/adafruit_circuitpython_ble_radio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:28:53.000000 adafruit-circuitpython-ble-radio-0.5.7/adafruit_circuitpython_ble_radio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-08-26 02:28:53.000000 adafruit-circuitpython-ble-radio-0.5.7/adafruit_circuitpython_ble_radio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-26 02:28:53.000000 adafruit-circuitpython-ble-radio-0.5.7/adafruit_circuitpython_ble_radio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:28:53.961732 adafruit-circuitpython-ble-radio-0.5.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:28:53.961732 adafruit-circuitpython-ble-radio-0.5.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5659 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:28:53.961732 adafruit-circuitpython-ble-radio-0.5.7/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-08-26 02:28:41.000000 adafruit-circuitpython-ble-radio-0.5.7/examples/ble_radio_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-08-26 02:28:41.000000 adafruit-circuitpython-ble-radio-0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-08-26 02:28:27.000000 adafruit-circuitpython-ble-radio-0.5.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:28:53.965732 adafruit-circuitpython-ble-radio-0.5.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:28:53.965732 adafruit-circuitpython-ble-radio-0.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-26 02:28:41.000000 adafruit-circuitpython-ble-radio-0.5.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-08-26 02:28:41.000000 adafruit-circuitpython-ble-radio-0.5.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     6581 2022-08-26 02:28:41.000000 adafruit-circuitpython-ble-radio-0.5.7/tests/test_adafruit_radio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:38:16.541125 adafruit-circuitpython-ble-radio-0.5.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:38:16.533125 adafruit-circuitpython-ble-radio-0.5.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:38:16.533125 adafruit-circuitpython-ble-radio-0.5.8/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:38:16.537125 adafruit-circuitpython-ble-radio-0.5.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:38:16.537125 adafruit-circuitpython-ble-radio-0.5.8/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-05-25 15:38:16.541125 adafruit-circuitpython-ble-radio-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-25 15:38:07.000000 adafruit-circuitpython-ble-radio-0.5.8/adafruit_ble_radio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:38:16.537125 adafruit-circuitpython-ble-radio-0.5.8/adafruit_circuitpython_ble_radio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-05-25 15:38:16.000000 adafruit-circuitpython-ble-radio-0.5.8/adafruit_circuitpython_ble_radio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-25 15:38:16.000000 adafruit-circuitpython-ble-radio-0.5.8/adafruit_circuitpython_ble_radio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:38:16.000000 adafruit-circuitpython-ble-radio-0.5.8/adafruit_circuitpython_ble_radio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-25 15:38:16.000000 adafruit-circuitpython-ble-radio-0.5.8/adafruit_circuitpython_ble_radio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-25 15:38:16.000000 adafruit-circuitpython-ble-radio-0.5.8/adafruit_circuitpython_ble_radio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:38:16.537125 adafruit-circuitpython-ble-radio-0.5.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:38:16.537125 adafruit-circuitpython-ble-radio-0.5.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:38:16.541125 adafruit-circuitpython-ble-radio-0.5.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-25 15:38:07.000000 adafruit-circuitpython-ble-radio-0.5.8/examples/ble_radio_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-25 15:38:07.000000 adafruit-circuitpython-ble-radio-0.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-25 15:37:47.000000 adafruit-circuitpython-ble-radio-0.5.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:38:16.541125 adafruit-circuitpython-ble-radio-0.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:38:16.541125 adafruit-circuitpython-ble-radio-0.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:38:07.000000 adafruit-circuitpython-ble-radio-0.5.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-25 15:38:07.000000 adafruit-circuitpython-ble-radio-0.5.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-05-25 15:38:07.000000 adafruit-circuitpython-ble-radio-0.5.8/tests/test_adafruit_radio.py
```

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ble-radio-0.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/.gitignore` & `adafruit-circuitpython-ble-radio-0.5.8/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/.pre-commit-config.yaml` & `adafruit-circuitpython-ble-radio-0.5.8/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
+    rev: v1.1.2
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/.pylintrc` & `adafruit-circuitpython-ble-radio-0.5.8/.pylintrc`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
+# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
@@ -429,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ble-radio-0.5.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/LICENSE` & `adafruit-circuitpython-ble-radio-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ble-radio-0.5.8/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/LICENSES/MIT.txt` & `adafruit-circuitpython-ble-radio-0.5.8/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ble-radio-0.5.8/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/PKG-INFO` & `adafruit-circuitpython-ble-radio-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-radio
-Version: 0.5.7
+Version: 0.5.8
 Summary: Simple byte and string based inter-device communication via BLE.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BLE_Radio
 Keywords: adafruit,blinka,circuitpython,micropython,radio,ble
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/README.rst` & `adafruit-circuitpython-ble-radio-0.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/adafruit_ble_radio.py` & `adafruit-circuitpython-ble-radio-0.5.8/adafruit_ble_radio.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from adafruit_ble.advertising.standard import ManufacturerData
 from adafruit_ble.advertising.adafruit import (
     MANUFACTURING_DATA_ADT,
     ADAFRUIT_COMPANY_ID,
 )
 
 
-__version__ = "0.5.7"
+__version__ = "0.5.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE_Radio.git"
 
 
 #: Maximum length of a message (in bytes).
 MAX_LENGTH = 248
 
 #: Amount of time to advertise a message (in seconds).
@@ -142,15 +142,15 @@
         # Ensure length of message.
         if len(message) > MAX_LENGTH:
             raise ValueError("Message too long (max length = {})".format(MAX_LENGTH))
         advertisement = _RadioAdvertisement()
         # Concatenate the bytes that make up the advertised message.
         advertisement.msg = struct.pack("<BB", self._channel, self.uid) + message
 
-        self.uid = (self.uid + 1) % 255
+        self.uid = (self.uid + 1) % 256
         # Advertise (block) for AD_DURATION period of time.
         self.ble.start_advertising(advertisement)
         time.sleep(AD_DURATION)
         self.ble.stop_advertising()
 
     def receive(self, timeout: float = 1.0) -> str:
         """
```

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/adafruit_circuitpython_ble_radio.egg-info/PKG-INFO` & `adafruit-circuitpython-ble-radio-0.5.8/adafruit_circuitpython_ble_radio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-radio
-Version: 0.5.7
+Version: 0.5.8
 Summary: Simple byte and string based inter-device communication via BLE.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BLE_Radio
 Keywords: adafruit,blinka,circuitpython,micropython,radio,ble
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/adafruit_circuitpython_ble_radio.egg-info/SOURCES.txt` & `adafruit-circuitpython-ble-radio-0.5.8/adafruit_circuitpython_ble_radio.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 adafruit_ble_radio.py
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_ble_radio.egg-info/PKG-INFO
 adafruit_circuitpython_ble_radio.egg-info/SOURCES.txt
 adafruit_circuitpython_ble_radio.egg-info/dependency_links.txt
 adafruit_circuitpython_ble_radio.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/docs/_static/favicon.ico` & `adafruit-circuitpython-ble-radio-0.5.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/docs/conf.py` & `adafruit-circuitpython-ble-radio-0.5.8/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
```

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/docs/index.rst` & `adafruit-circuitpython-ble-radio-0.5.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/examples/ble_radio_simpletest.py` & `adafruit-circuitpython-ble-radio-0.5.8/examples/ble_radio_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/pyproject.toml` & `adafruit-circuitpython-ble-radio-0.5.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ble-radio"
 description = "Simple byte and string based inter-device communication via BLE."
-version = "0.5.7"
+version = "0.5.8"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BLE_Radio"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/tests/conftest.py` & `adafruit-circuitpython-ble-radio-0.5.8/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,19 @@
 import sys
 from unittest.mock import MagicMock
 
 # Add fully qualified namespace paths to things that are imported, but which
 # should be mocked away. For instance, modules which are available in
 # CircuitPython but not standard Python.
 MOCK_MODULES = [
-    "adafruit_ble.BLERadio",
-    "adafruit_ble.advertising.adafruit.AdafruitRadio",
+    "adafruit_ble",
+    "adafruit_ble.advertising",
+    "adafruit_ble.advertising.standard",
+    "adafruit_ble.advertising.adafruit",
+    "_bleio",
 ]
 
 
 def mock_imported_modules():
     """
     Mocks away the modules named in MOCK_MODULES, so the module under test
     can be imported with modules which may not be available.
```

### Comparing `adafruit-circuitpython-ble-radio-0.5.7/tests/test_adafruit_radio.py` & `adafruit-circuitpython-ble-radio-0.5.8/tests/test_adafruit_radio.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,23 @@
 found in the testconf.py file. See comments therein for explanation of how it
 works.
 """
 import struct
 import time
 from unittest import mock
 import pytest
+from adafruit_ble.advertising import Advertisement
 import adafruit_ble_radio
 
 
+# pylint: disable=redefined-outer-name
+
+
 @pytest.fixture
-def radio():
+def radio_obj():
     """
     A fixture to recreate a new Radio instance for each test that needs it.
     """
     return adafruit_ble_radio.Radio()
 
 
 def test_radio_init_default():
@@ -100,17 +104,15 @@
     broadcast for AD_DURATION period of time.
     """
     radio_obj.uid = 255  # set up for cycle back to 0.
     msg = b"Hello"
     with mock.patch("adafruit_ble_radio.time.sleep") as mock_sleep:
         radio_obj.send_bytes(msg)
         mock_sleep.assert_called_once_with(adafruit_ble_radio.AD_DURATION)
-    spy_advertisement = (
-        adafruit_ble_radio._RadioAdvertisement()  # pylint: disable=protected-access
-    )  # pylint: disable=protected-access
+    spy_advertisement = Advertisement
     chan = struct.pack("<B", radio_obj._channel)  # pylint: disable=protected-access
     uid = struct.pack("<B", 255)
     assert spy_advertisement.msg == chan + uid + msg
     radio_obj.ble.start_advertising.assert_called_once_with(spy_advertisement)
     radio_obj.ble.stop_advertising.assert_called_once_with()
     assert radio_obj.uid == 0
 
@@ -118,15 +120,15 @@
 def test_radio_receive_no_message(radio_obj):
     """
     If no message is received from the receive_bytes method, then None is
     returned.
     """
     radio_obj.receive_full = mock.MagicMock(return_value=None)
     assert radio_obj.receive() is None
-    radio_obj.receive_full.assert_called_once_with()
+    radio_obj.receive_full.assert_called_once_with(timeout=1.0)
 
 
 def test_radio_receive(radio_obj):
     """
     If bytes are received from the receive_bytes method, these are decoded
     using utf-8 and returned as a string with null characters stripped from the
     end.
```

