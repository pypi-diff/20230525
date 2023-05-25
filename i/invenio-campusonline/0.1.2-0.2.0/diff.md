# Comparing `tmp/invenio-campusonline-0.1.2.tar.gz` & `tmp/invenio-campusonline-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-campusonline-0.1.2.tar", last modified: Mon May  1 20:21:04 2023, max compression
+gzip compressed data, was "invenio-campusonline-0.2.0.tar", last modified: Thu May 25 09:37:34 2023, max compression
```

## Comparing `invenio-campusonline-0.1.2.tar` & `invenio-campusonline-0.2.0.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:04.249348 invenio-campusonline-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:04.241347 invenio-campusonline-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:04.245348 invenio-campusonline-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:04.245348 invenio-campusonline-0.1.2/.tx/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/.tx/config
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-01 20:21:04.249348 invenio-campusonline-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:04.245348 invenio-campusonline-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:04.245348 invenio-campusonline-0.1.2/invenio_campusonline/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/invenio_campusonline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/invenio_campusonline/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/invenio_campusonline/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/invenio_campusonline/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/invenio_campusonline/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/invenio_campusonline/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/invenio_campusonline/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/invenio_campusonline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:04.249348 invenio-campusonline-0.1.2/invenio_campusonline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-01 20:21:04.000000 invenio-campusonline-0.1.2/invenio_campusonline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-01 20:21:04.000000 invenio-campusonline-0.1.2/invenio_campusonline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:21:04.000000 invenio-campusonline-0.1.2/invenio_campusonline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-01 20:21:04.000000 invenio-campusonline-0.1.2/invenio_campusonline.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:21:04.000000 invenio-campusonline-0.1.2/invenio_campusonline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-01 20:21:04.000000 invenio-campusonline-0.1.2/invenio_campusonline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 20:21:04.000000 invenio-campusonline-0.1.2/invenio_campusonline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      438 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-01 20:21:04.249348 invenio-campusonline-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:04.249348 invenio-campusonline-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/tests/test_invenio_campusonline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:37:34.719298 invenio-campusonline-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:37:34.715298 invenio-campusonline-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:37:34.715298 invenio-campusonline-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/.ruff.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:37:34.715298 invenio-campusonline-0.2.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-25 09:37:34.719298 invenio-campusonline-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:37:34.715298 invenio-campusonline-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:37:34.719298 invenio-campusonline-0.2.0/invenio_campusonline/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/invenio_campusonline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/invenio_campusonline/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/invenio_campusonline/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/invenio_campusonline/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/invenio_campusonline/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/invenio_campusonline/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/invenio_campusonline/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/invenio_campusonline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:37:34.719298 invenio-campusonline-0.2.0/invenio_campusonline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-25 09:37:34.000000 invenio-campusonline-0.2.0/invenio_campusonline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-25 09:37:34.000000 invenio-campusonline-0.2.0/invenio_campusonline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:37:34.000000 invenio-campusonline-0.2.0/invenio_campusonline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-25 09:37:34.000000 invenio-campusonline-0.2.0/invenio_campusonline.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:37:34.000000 invenio-campusonline-0.2.0/invenio_campusonline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-25 09:37:34.000000 invenio-campusonline-0.2.0/invenio_campusonline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 09:37:34.000000 invenio-campusonline-0.2.0/invenio_campusonline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      446 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-25 09:37:34.719298 invenio-campusonline-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:37:34.719298 invenio-campusonline-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/tests/minimal_record.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/tests/test_invenio_campusonline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-25 09:37:25.000000 invenio-campusonline-0.2.0/tests/test_utils.py
```

### Comparing `invenio-campusonline-0.1.2/.editorconfig` & `invenio-campusonline-0.2.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.2/.github/workflows/tests.yml` & `invenio-campusonline-0.2.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.2/.tx/config` & `invenio-campusonline-0.2.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.2/CHANGES.rst` & `invenio-campusonline-0.2.0/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,20 @@
     invenio-campusonline is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.2.0 (release 2023-05-25)
+
+- utils: implement get_embargo_range
+- setup: migrate to ruff
+
+
 Version v0.1.2 (release 2023-05-01)
 
 - cli: move to secho way from logger
 
 
 Version v0.1.1 (release 2023-01-11)
```

### Comparing `invenio-campusonline-0.1.2/CONTRIBUTING.rst` & `invenio-campusonline-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.2/LICENSE` & `invenio-campusonline-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.2/MANIFEST.in` & `invenio-campusonline-0.2.0/MANIFEST.in`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021 Graz University of Technology.
+# Copyright (C) 2021-2023 Graz University of Technology.
 #
 # invenio-campusonline is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
-# TODO: Generate this manifest file by running the following commands:
-# (please sort the lines in this file after running below commands)
-#
-#  git init
-#  git add -A
-#  pip install -e .[all]
-#  check-manifest -u
-
 include .dockerignore
 include .editorconfig
 include .tx/config
 prune docs/_build
 recursive-include .github/workflows *.yml
 recursive-include invenio_campusonline/translations *.po *.pot *.mo
 
 # added by check-manifest
 include *.md
 include *.rst
 include *.sh
 include *.txt
+include *.toml
 include babel.ini
 include pytest.ini
 recursive-include docs *.bat
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs *.txt
 recursive-include docs Makefile
 recursive-include tests *.py
+recursive-include tests *.xml
 include .git-blame-ignore-revs
```

### Comparing `invenio-campusonline-0.1.2/PKG-INFO` & `invenio-campusonline-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: invenio-campusonline
-Version: 0.1.2
-Summary: "This module is used to import/export from/to the CampusOnline System."
+Version: 0.2.0
+Summary: "The module is used to import/export from/to the CampusOnline System."
 Home-page: https://github.com/tu-graz-library/invenio-campusonline
 Author: Graz University of Technology
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio TODO
 Platform: any
 Classifier: Programming Language :: Python :: 3.9
@@ -53,14 +53,20 @@
     invenio-campusonline is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.2.0 (release 2023-05-25)
+
+- utils: implement get_embargo_range
+- setup: migrate to ruff
+
+
 Version v0.1.2 (release 2023-05-01)
 
 - cli: move to secho way from logger
 
 
 Version v0.1.1 (release 2023-01-11)
```

### Comparing `invenio-campusonline-0.1.2/README.rst` & `invenio-campusonline-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.2/babel.ini` & `invenio-campusonline-0.2.0/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.2/docs/Makefile` & `invenio-campusonline-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.2/docs/conf.py` & `invenio-campusonline-0.2.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,18 @@
     "sphinx.ext.autodoc",
     "sphinx.ext.coverage",
     "sphinx.ext.doctest",
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
 ]
 
+nitpick_ignore = [
+    ("py:class", "flask.app.Flask"),
+]
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 # source_suffix = ['.rst', '.md']
 source_suffix = ".rst"
```

### Comparing `invenio-campusonline-0.1.2/docs/index.rst` & `invenio-campusonline-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.2/docs/make.bat` & `invenio-campusonline-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.2/invenio_campusonline/__init__.py` & `invenio-campusonline-0.2.0/invenio_campusonline/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021-2022 Graz University of Technology.
+# Copyright (C) 2021-2023 Graz University of Technology.
 #
 # invenio-campusonline is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
-"""This module is used to import/export from/to the CampusOnline System."""
+"""The module is used to import/export from/to the CampusOnline System."""
 
 from .api import fetch_all_ids, import_from_campusonline
 from .ext import InvenioCampusonline
 from .types import ThesesFilter, ThesesState
 
-__version__ = "0.1.2"
+__version__ = "0.2.0"
 
 __all__ = (
     "__version__",
     "InvenioCampusonline",
     "import_from_campusonline",
     "fetch_all_ids",
     "ThesesFilter",
```

### Comparing `invenio-campusonline-0.1.2/invenio_campusonline/api.py` & `invenio-campusonline-0.2.0/invenio_campusonline/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 # Copyright (C) 2022 Graz University of Technology.
 #
 # invenio-campusonline is free software; you can redistribute it
 # and/or modify it under the terms of the MIT License; see LICENSE
 # file for more details.
 
 """API functions of the campusonline connector."""
-from typing import Callable
+from collections.abc import Callable
 from xml.etree.ElementTree import fromstring
 
+from invenio_records_resources.services.records.results import RecordItem
 from requests import post
 
 from .types import (
     URL,
     CampusOnlineConfigs,
     CampusOnlineID,
     CampusOnlineToken,
@@ -25,28 +26,33 @@
     create_request_header,
     download_file,
     get_metadata,
 )
 
 
 def import_from_campusonline(
-    import_func: Callable, cms_id: CampusOnlineID, configs: CampusOnlineConfigs
-):
+    import_func: Callable,
+    cms_id: CampusOnlineID,
+    configs: CampusOnlineConfigs,
+) -> RecordItem:
     """Import record from campusonline."""
     return import_func(cms_id, configs, get_metadata, download_file)
 
 
 def fetch_all_ids(
-    endpoint: URL, token: CampusOnlineToken, theses_filters: ThesesFilter = None
+    endpoint: URL,
+    token: CampusOnlineToken,
+    theses_filters: ThesesFilter = None,
 ) -> list[tuple[CampusOnlineID, ThesesState]]:
     """Fetch to import ids."""
     ids = []
     for theses_filter, state in theses_filters:
         body = create_request_body_ids(token, theses_filter)
 
         headers = create_request_header("getAllThesesMetadataRequest")
-        response = post(endpoint, data=body, headers=headers)
+        response = post(endpoint, data=body, headers=headers, timeout=10)
 
         root = fromstring(response.text)
         xpath = "{http://www.campusonline.at/thesisservice/basetypes}ID"
         ids += [(CampusOnlineID(node.text), state) for node in root.iter(xpath)]
+
     return ids
```

### Comparing `invenio-campusonline-0.1.2/invenio_campusonline/cli.py` & `invenio-campusonline-0.2.0/invenio_campusonline/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,46 +14,61 @@
 from flask.cli import with_appcontext
 
 from .api import fetch_all_ids, import_from_campusonline
 from .types import CampusOnlineConfigs, Color
 
 
 @group()
-def campusonline():
+def campusonline() -> None:
     """Campusonline CLI."""
 
 
 @campusonline.command()
 @with_appcontext
 @option("--endpoint", type=URL)
 @option("--campusonline-id", type=STRING)
 @option("--token", type=STRING)
 @option("--user-email", type=STRING, default="cms@tugraz.at")
-@option("--no-color", is_flag=True)
-def import_thesis(endpoint, campusonline_id, token, user_email, no_color=False):
+@option("--no-color", is_flag=True, default=False)
+def import_thesis(
+    endpoint: str,
+    campusonline_id: str,
+    token: str,
+    user_email: str,
+    no_color: bool,  # noqa: FBT001
+) -> None:
     """Import metadata and file (aka one thesis) from campusonline."""
     import_func = current_app.config["CAMPUSONLINE_IMPORT_FUNC"]
     theses_filters = current_app.config["CAMPUSONLINE_THESES_FILTERS"]
     recipients = current_app.config["CAMPUSONLINE_ERROR_MAIL_RECIPIENTS"]
     sender = current_app.config["CAMPUSONLINE_ERROR_MAIL_SENDER"]
 
     configs = CampusOnlineConfigs(
-        endpoint, token, user_email, theses_filters, recipients, sender
+        endpoint,
+        token,
+        user_email,
+        theses_filters,
+        recipients,
+        sender,
     )
     record = import_from_campusonline(import_func, campusonline_id, configs)
 
     color = Color.success if not no_color else Color.neutral
     secho(f"record.id: {record.id}", fg=color)
 
 
 @campusonline.command()
 @with_appcontext
 @option("--endpoint", type=URL)
 @option("--token", type=STRING)
 @option("--no-color", is_flag=True)
-def fetch_ids(endpoint, token, no_color):
+def fetch_ids(
+    endpoint: str,
+    token: str,
+    no_color: bool,  # noqa: FBT001
+) -> None:
     """Fetch all to import ids."""
     theses_filters = current_app.config["CAMPUSONLINE_THESES_FILTERS"]
     ids = fetch_all_ids(endpoint, token, theses_filters)
 
     color = Color.success if not no_color else Color.neutral
     secho(f"ids: {ids}", fg=color)
```

### Comparing `invenio-campusonline-0.1.2/invenio_campusonline/config.py` & `invenio-campusonline-0.2.0/invenio_campusonline/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021-2022 Graz University of Technology.
+# Copyright (C) 2021-2023 Graz University of Technology.
 #
 # invenio-campusonline is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
-"""This is the configuration file."""
+"""The configuration file."""
 
 CAMPUSONLINE_ENDPOINT = ""
 """This is the endpoint to fetch the records."""
 
 CAMPUSONLINE_TOKEN = ""
 """This is the token to get the records from the campusonline endpoint."""
```

### Comparing `invenio-campusonline-0.1.2/invenio_campusonline/tasks.py` & `invenio-campusonline-0.2.0/invenio_campusonline/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022 Graz University of Technology.
+# Copyright (C) 2022-2023 Graz University of Technology.
 #
 # invenio-campusonline is free software; you can redistribute it
 # and/or modify it under the terms of the MIT License; see LICENSE
 # file for more details.
 
 
 """Celery tasks for `invenio-campusonline`."""
-from typing import Callable
+from collections.abc import Callable
 
 from celery import shared_task
 from flask import current_app
 from flask_mail import Message
 
 from .api import fetch_all_ids, import_from_campusonline
 from .types import CampusOnlineConfigs
 
 
 def config_variables() -> tuple[Callable, CampusOnlineConfigs]:
-    """Configuration variables."""
+    """Configure variables."""
     import_func = current_app.config["CAMPUSONLINE_IMPORT_FUNC"]
     endpoint = current_app.config["CAMPUSONLINE_ENDPOINT"]
     token = current_app.config["CAMPUSONLINE_TOKEN"]
     user_email = current_app.config["CAMPUSONLINE_USER_EMAIL"]
     theses_filters = current_app.config["CAMPUSONLINE_THESES_FILTERS"]
     recipients = current_app.config["CAMPUSONLINE_ERROR_MAIL_RECIPIENTS"]
     sender = current_app.config["CAMPUSONLINE_ERROR_MAIL_SENDER"]
 
     return import_func, CampusOnlineConfigs(
-        endpoint, token, user_email, theses_filters, recipients, sender
+        endpoint,
+        token,
+        user_email,
+        theses_filters,
+        recipients,
+        sender,
     )
 
 
 @shared_task(ignore_result=True)
 def import_theses_from_campusonline() -> None:
     """Import theses from campusonline."""
     import_func, configs = config_variables()
     ids = fetch_all_ids(configs.endpoint, configs.token, configs.theses_filters)
 
-    for cms_id, state in ids:
+    for cms_id, _ in ids:
         try:
             import_from_campusonline(import_func, cms_id, configs)
         except RuntimeError:
             msg = Message(
                 "ERROR: importing from campusonline",
                 sender=configs.sender,
                 recipients=configs.recipients,
```

### Comparing `invenio-campusonline-0.1.2/invenio_campusonline/types.py` & `invenio-campusonline-0.2.0/invenio_campusonline/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022 Graz University of Technology.
+# Copyright (C) 2022-2023 Graz University of Technology.
 #
 # invenio-campusonline is free software; you can redistribute it
 # and/or modify it under the terms of the MIT License; see LICENSE
 # file for more details.
 
 
 """Types."""
 
 from dataclasses import astuple, dataclass
+from datetime import datetime
 from enum import Enum
 from xml.etree.ElementTree import Element
 
 URL = str
 """Type to indicate that an URL is necessary."""
 
 CampusOnlineToken = str
@@ -35,23 +36,40 @@
 """The email address.
 
 The address does not have to have a special format, but it has to be an email.
 """
 
 
 @dataclass(frozen=True)
+class Embargo:
+    """The class is for the embargo management."""
+
+    start: datetime = None
+    end: datetime = None
+
+    @property
+    def end_date(self) -> str:
+        """Calculate str date in format %Y-%m-%d."""
+        return self.end.strftime("%Y-%m-%d")
+
+    def __bool__(self) -> bool:
+        """Check if values are set, otherwise return is false."""
+        return bool(self.start and self.end)
+
+
+@dataclass(frozen=True)
 class Color:
-    """This class is for the output color management."""
+    """The class is for the output color management."""
 
     neutral = "black"
     error = "red"
     warning = "yellow"
     abort = "magenta"
     success = "green"
-    alternate = ["blue", "cyan"]
+    alternate = ("blue", "cyan")
 
 
 class ThesesState(Enum):
     """Theses State class."""
 
     LOCKED = 1
     OPEN = 2
@@ -60,16 +78,16 @@
 @dataclass
 class ThesesFilter:
     """Filter dataclass."""
 
     filter_: list[Element]
     state: ThesesState
 
-    def __iter__(self):
-        """This method makes the properties iterable."""
+    def __iter__(self):  # noqa: ANN204
+        """Make the class iteratable."""
         return iter(astuple(self))
 
 
 @dataclass
 class CampusOnlineConfigs:
     """Configs for campus online."""
```

### Comparing `invenio-campusonline-0.1.2/invenio_campusonline/utils.py` & `invenio-campusonline-0.2.0/invenio_campusonline/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022 Graz University of Technology.
+# Copyright (C) 2022-2023 Graz University of Technology.
 #
 # invenio-campusonline is free software; you can redistribute it
 # and/or modify it under the terms of the MIT License; see LICENSE
 # file for more details.
 
 """Command line interface to interact with the CampusOnline-Connector module."""
+from datetime import datetime
+from pathlib import Path
 from shutil import copyfileobj
 from xml.etree.ElementTree import Element, fromstring
 
 from requests import get, post
 
-from .types import URL, CampusOnlineID, CampusOnlineToken, FilePath
+from .types import URL, CampusOnlineID, CampusOnlineToken, Embargo, FilePath
 
 
 def create_request_body_metadata(
-    token: CampusOnlineToken, campusonline_id: CampusOnlineID
+    token: CampusOnlineToken,
+    campusonline_id: CampusOnlineID,
 ) -> str:
     """Build Request."""
     body = """
     <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
                       xmlns:bas="http://www.campusonline.at/thesisservice/basetypes">
       <soapenv:Header/>
       <soapenv:Body>
@@ -45,15 +48,16 @@
     </soapenv:Envelope>
     """
 
     return body.replace("TOKEN", token).replace("CAMPUSONLINE_ID", campusonline_id)
 
 
 def create_request_body_download(
-    token: CampusOnlineToken, campusonline_id: CampusOnlineID
+    token: CampusOnlineToken,
+    campusonline_id: CampusOnlineID,
 ) -> str:
     """Build Request."""
     body = """
     <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
                   xmlns:bas="http://www.campusonline.at/thesisservice/basetypes">
       <soapenv:Header/>
       <soapenv:Body>
@@ -66,15 +70,16 @@
     </soapenv:Envelope>
     """
 
     return body.replace("TOKEN", token).replace("CAMPUSONLINE_ID", campusonline_id)
 
 
 def create_request_body_ids(
-    token: CampusOnlineToken, theses_filter: list[Element]
+    token: CampusOnlineToken,
+    theses_filter: list[Element],
 ) -> str:
     """Build request."""
     body = """
     <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
                       xmlns:bas="http://www.campusonline.at/thesisservice/basetypes">
       <soapenv:Header/>
       <soapenv:Body>
@@ -87,59 +92,84 @@
     """
 
     return body.replace("TOKEN", token).replace("FILTER", "\n".join(theses_filter))
 
 
 def create_request_header(service: str) -> dict:
     """Create request header."""
-    header = {
+    return {
         "Content-Type": "application/xml",
         "SOAPAction": f"urn:service#{service}",
     }
-    return header
+
+
+def get_embargo_range(thesis: Element) -> Element:
+    """Extract the embargo range."""
+    ns = "http://www.campusonline.at/thesisservice/basetypes"
+    xpath_start = f".//{{{ns}}}attr[@key='SPVON']"
+    xpath_end = f".//{{{ns}}}attr[@key='SPBIS']"
+    start = thesis.find(xpath_start)
+    end = thesis.find(xpath_end)
+
+    if start is None or end is None:
+        return Embargo()
+
+    if start.text is None or end.text is None:
+        return Embargo()
+
+    in_format = "%Y-%m-%d %H:%M:%S"
+    start_embargo = datetime.strptime(start.text, in_format)
+    end_embargo = datetime.strptime(end.text, in_format)
+
+    return Embargo(start_embargo, end_embargo)
 
 
 def get_metadata(
-    endpoint: URL, token: CampusOnlineToken, campusonline_id: CampusOnlineID
+    endpoint: URL,
+    token: CampusOnlineToken,
+    campusonline_id: CampusOnlineID,
 ) -> Element:
     """Get Metadata."""
     body = create_request_body_metadata(token, campusonline_id)
     headers = create_request_header("getMetadataByThesisID")
-    response = post(endpoint, data=body, headers=headers)
+    response = post(endpoint, data=body, headers=headers, timeout=10)
 
     root = fromstring(response.text)
 
     xpath = "{http://www.campusonline.at/thesisservice/basetypes}thesis"
-    thesis = list(root.iter(xpath))[0]  # TODO: fix it
-    return thesis
+    return list(root.iter(xpath))[0]  # TODO: fix it
 
 
 def get_file_url(
-    endpoint: URL, token: CampusOnlineToken, campusonline_id: CampusOnlineID
+    endpoint: URL,
+    token: CampusOnlineToken,
+    campusonline_id: CampusOnlineID,
 ) -> str:
     """Get file URL."""
     body = create_request_body_download(token, campusonline_id)
     headers = create_request_header("getDocumentByThesisID")
-    response = post(endpoint, data=body, headers=headers)
+    response = post(endpoint, data=body, headers=headers, timeout=10)
 
     root = fromstring(response.text)
     xpath = "{http://www.campusonline.at/thesisservice/basetypes}docUrl"
     file_url = list(root.iter(xpath))[0]  # TODO: make it more nice
     return file_url.text
 
 
-def store_file_temporarily(file_url: URL, file_path: FilePath):
-    """This function stores files referenced by an url to the local file path."""
-    with get(file_url, stream=True) as response:
-        with open(file_path, "wb") as fp:
+def store_file_temporarily(file_url: URL, file_path: FilePath) -> None:
+    """Store the file referenced by url to the local file path."""
+    with get(file_url, stream=True, timeout=10) as response:  # noqa: SIM117
+        with Path(file_path).open("wb") as fp:
             copyfileobj(response.raw, fp)
 
 
 def download_file(
-    endpoint: URL, token: CampusOnlineToken, campusonline_id: CampusOnlineID
+    endpoint: URL,
+    token: CampusOnlineToken,
+    campusonline_id: CampusOnlineID,
 ) -> FilePath:
-    """This function downloads files from campus online."""
+    """Download files from campus online by campusonline_id."""
     file_url = get_file_url(endpoint, token, campusonline_id)
     file_url = f"{file_url}{token}"
-    file_path = f"/tmp/{campusonline_id}.pdf"
+    file_path = f"/tmp/{campusonline_id}.pdf"  # noqa: S108
     store_file_temporarily(file_url, file_path)
     return file_path
```

### Comparing `invenio-campusonline-0.1.2/invenio_campusonline.egg-info/PKG-INFO` & `invenio-campusonline-0.2.0/invenio_campusonline.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: invenio-campusonline
-Version: 0.1.2
-Summary: "This module is used to import/export from/to the CampusOnline System."
+Version: 0.2.0
+Summary: "The module is used to import/export from/to the CampusOnline System."
 Home-page: https://github.com/tu-graz-library/invenio-campusonline
 Author: Graz University of Technology
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio TODO
 Platform: any
 Classifier: Programming Language :: Python :: 3.9
@@ -53,14 +53,20 @@
     invenio-campusonline is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.2.0 (release 2023-05-25)
+
+- utils: implement get_embargo_range
+- setup: migrate to ruff
+
+
 Version v0.1.2 (release 2023-05-01)
 
 - cli: move to secho way from logger
 
 
 Version v0.1.1 (release 2023-01-11)
```

### Comparing `invenio-campusonline-0.1.2/invenio_campusonline.egg-info/SOURCES.txt` & `invenio-campusonline-0.2.0/invenio_campusonline.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .dockerignore
 .editorconfig
 .git-blame-ignore-revs
+.ruff.toml
 AUTHORS.rst
 CHANGES.rst
 CONTRIBUTING.rst
 INSTALL.rst
 LICENSE
 MANIFEST.in
 README.rst
@@ -42,9 +43,10 @@
 invenio_campusonline.egg-info/SOURCES.txt
 invenio_campusonline.egg-info/dependency_links.txt
 invenio_campusonline.egg-info/entry_points.txt
 invenio_campusonline.egg-info/not-zip-safe
 invenio_campusonline.egg-info/requires.txt
 invenio_campusonline.egg-info/top_level.txt
 tests/conftest.py
+tests/minimal_record.xml
 tests/test_invenio_campusonline.py
 tests/test_utils.py
```

### Comparing `invenio-campusonline-0.1.2/setup.cfg` & `invenio-campusonline-0.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = invenio-campusonline
 version = attr: invenio_campusonline.__version__
-description = "This module is used to import/export from/to the CampusOnline System."
+description = "The module is used to import/export from/to the CampusOnline System."
 long_description = file: README.rst, CHANGES.rst
 keywords = invenio TODO
 license = MIT
 author = Graz University of Technology
 author_email = info@tugraz.at
 platforms = any
 url = https://github.com/tu-graz-library/invenio-campusonline
@@ -19,24 +19,25 @@
 include_package_data = True
 packages = find:
 python_requires = >=3.7
 zip_safe = False
 install_requires = 
 	click>=8.0.0
 	click-params>=0.4.0
-	invenio-i18n>=1.2.0
 	invenio-celery>=1.2.5
 	invenio-mail>=1.0.2
 	requests>=2.0.0
 
 [options.extras_require]
 tests = 
 	pytest-black>=0.3.0
 	pytest-invenio>=1.4.0
+	invenio-records-resources>=1.0.0
 	invenio-search[opensearch2]>=2.1.0
+	ruff>=0.0.263
 	sphinx>=4.5
 
 [options.entry_points]
 flask.commands = 
 	campusonline = invenio_campusonline.cli:campusonline
 invenio_base.apps = 
 	invenio_campusonline = invenio_campusonline:InvenioCampusonline
@@ -58,14 +59,14 @@
 profile = black
 
 [check-manifest]
 ignore = 
 	*-requirements.txt
 
 [tool:pytest]
-addopts = --black --isort --pydocstyle --doctest-glob="*.rst" --doctest-modules --cov=invenio_campusonline --cov-report=term-missing
+addopts = --black --doctest-glob="*.rst" --doctest-modules --cov=invenio_campusonline --cov-report=term-missing
 testpaths = docs tests invenio_campusonline
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `invenio-campusonline-0.1.2/tests/test_invenio_campusonline.py` & `invenio-campusonline-0.2.0/tests/test_invenio_campusonline.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021 Graz University of Technology.
+# Copyright (C) 2021-2023 Graz University of Technology.
 #
 # invenio-campusonline is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Module tests."""
 
 from flask import Flask
 
-from invenio_campusonline import InvenioCampusonline
+from invenio_campusonline import InvenioCampusonline, __version__
 
 
-def test_version():
+def test_version() -> None:
     """Test version import."""
-    from invenio_campusonline import __version__
-
     assert __version__
 
 
-def test_init():
+def test_init() -> None:
     """Test extension initialization."""
     app = Flask("testapp")
     ext = InvenioCampusonline(app)
     assert "invenio-campusonline" in app.extensions
 
     app = Flask("testapp")
     ext = InvenioCampusonline()
```

### Comparing `invenio-campusonline-0.1.2/tests/test_utils.py` & `invenio-campusonline-0.2.0/tests/test_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022 Graz University of Technology.
+# Copyright (C) 2022-2023 Graz University of Technology.
 #
 # invenio-campusonline is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Module utils."""
 
+from xml.etree.ElementTree import Element
+
+from invenio_campusonline.types import Embargo
 from invenio_campusonline.utils import (
     create_request_body_download,
     create_request_body_ids,
     create_request_body_metadata,
     create_request_header,
+    get_embargo_range,
 )
 
 
-def test_create_request_body_metadata():
+def test_create_request_body_metadata() -> None:
     """Test the create_request_body_metadata function."""
     body = create_request_body_metadata("abcd", "efgh")
     expected = """
     <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
                       xmlns:bas="http://www.campusonline.at/thesisservice/basetypes">
       <soapenv:Header/>
       <soapenv:Body>
@@ -44,15 +48,15 @@
       </soapenv:Body>
     </soapenv:Envelope>
     """
 
     assert body == expected
 
 
-def test_create_request_body_download():
+def test_create_request_body_download() -> None:
     """Test the create_request_body_download function."""
     body = create_request_body_download("abcd", "efgh")
     expected = """
     <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
                   xmlns:bas="http://www.campusonline.at/thesisservice/basetypes">
       <soapenv:Header/>
       <soapenv:Body>
@@ -63,30 +67,31 @@
         </bas:getDocumentByThesisIDRequest>
       </soapenv:Body>
     </soapenv:Envelope>
     """
     assert body == expected
 
 
-def test_create_request_body_ids():
+def test_create_request_body_ids() -> None:
     """Test the create_request_body_ids function."""
     body = create_request_body_ids("abcd", [])
     expected = """
     <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
                       xmlns:bas="http://www.campusonline.at/thesisservice/basetypes">
       <soapenv:Header/>
       <soapenv:Body>
         <bas:getAllThesesMetadataRequest>
           <bas:token>abcd</bas:token>
           FILTER
         </bas:getAllThesesMetadataRequest>
       </soapenv:Body>
     </soapenv:Envelope>
     """.replace(
-        "FILTER", "\n".join([])
+        "FILTER",
+        "\n".join([]),
     )
     assert body == expected
 
     theses_filter = [
         """<bas:thesesType>DISS</bas:thesesType>""",
         """<bas:state name="IFG"/>""",
     ]
@@ -104,16 +109,31 @@
       </soapenv:Body>
     </soapenv:Envelope>
     """
 
     assert body == expected
 
 
-def test_create_request_header():
+def test_create_request_header() -> None:
     """Test the create_request_header function."""
     header = create_request_header("allThesesMetadataRequest")
     expected = {
         "Content-Type": "application/xml",
         "SOAPAction": "urn:service#allThesesMetadataRequest",
     }
 
     assert header == expected
+
+
+def test_get_embargo_range(minimal_record: Element) -> None:
+    """Test the get_embargo_range function."""
+    embargo = get_embargo_range(minimal_record)
+
+    assert embargo.end_date == "2025-03-03"
+    assert bool(Embargo()) is False
+
+    embargo = get_embargo_range(Element("root"))
+
+    assert bool(embargo) is False
+
+    if not bool(embargo := get_embargo_range(Element("root"))):
+        assert bool(embargo) is False
```

