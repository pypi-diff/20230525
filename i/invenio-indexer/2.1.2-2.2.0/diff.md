# Comparing `tmp/invenio-indexer-2.1.2.tar.gz` & `tmp/invenio-indexer-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-indexer-2.1.2.tar", last modified: Fri May  5 12:53:07 2023, max compression
+gzip compressed data, was "invenio-indexer-2.2.0.tar", last modified: Thu May 25 08:20:35 2023, max compression
```

## Comparing `invenio-indexer-2.1.2.tar` & `invenio-indexer-2.2.0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.302495 invenio-indexer-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.290495 invenio-indexer-2.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.294495 invenio-indexer-2.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (122)      539 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3204 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3735 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)      731 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5828 2023-05-05 12:53:07.302495 invenio-indexer-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.294495 invenio-indexer-2.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7445 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      554 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10286 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      300 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6999 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/invenio_indexer/
--rw-r--r--   0 runner    (1001) docker     (122)     6480 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17246 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4293 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/proxies.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2744 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/tasks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/invenio_indexer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5828 2023-05-05 12:53:06.000000 invenio-indexer-2.1.2/invenio_indexer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1800 2023-05-05 12:53:07.000000 invenio-indexer-2.1.2/invenio_indexer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 12:53:06.000000 invenio-indexer-2.1.2/invenio_indexer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-05 12:53:06.000000 invenio-indexer-2.1.2/invenio_indexer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 12:53:06.000000 invenio-indexer-2.1.2/invenio_indexer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      411 2023-05-05 12:53:06.000000 invenio-indexer-2.1.2/invenio_indexer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-05 12:53:06.000000 invenio-indexer-2.1.2/invenio_indexer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (122)      756 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-05-05 12:53:07.302495 invenio-indexer-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      360 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3049 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (122)      258 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/tests/data/os-v1/
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/tests/data/os-v1/records/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/tests/data/os-v1/records/authorities/
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/os-v1/records/authorities/authority-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/tests/data/os-v1/records/bibliographic/
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/os-v1/records/bibliographic/bibliographic-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/os-v1/records/default-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/tests/data/os-v2/
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/tests/data/os-v2/records/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/tests/data/os-v2/records/authorities/
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/os-v2/records/authorities/authority-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.302495 invenio-indexer-2.1.2/tests/data/os-v2/records/bibliographic/
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/os-v2/records/bibliographic/bibliographic-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/os-v2/records/default-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.302495 invenio-indexer-2.1.2/tests/data/v7/
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.302495 invenio-indexer-2.1.2/tests/data/v7/records/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.302495 invenio-indexer-2.1.2/tests/data/v7/records/authorities/
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/v7/records/authorities/authority-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.302495 invenio-indexer-2.1.2/tests/data/v7/records/bibliographic/
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/v7/records/bibliographic/bibliographic-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/v7/records/default-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.302495 invenio-indexer-2.1.2/tests/demo/
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/demo/json_resolver.py
--rw-r--r--   0 runner    (1001) docker     (122)    14030 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3284 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     6002 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/test_invenio_indexer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1188 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1372 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.997163 invenio-indexer-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.989163 invenio-indexer-2.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.993163 invenio-indexer-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      539 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3318 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3735 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      731 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5982 2023-05-25 08:20:34.997163 invenio-indexer-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.993163 invenio-indexer-2.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7445 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      554 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10286 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      300 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6999 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.993163 invenio-indexer-2.2.0/invenio_indexer/
+-rw-r--r--   0 runner    (1001) docker     (122)     6480 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/invenio_indexer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17246 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/invenio_indexer/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4902 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/invenio_indexer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/invenio_indexer/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/invenio_indexer/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/invenio_indexer/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/invenio_indexer/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2744 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/invenio_indexer/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/invenio_indexer/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/invenio_indexer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.997163 invenio-indexer-2.2.0/invenio_indexer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5982 2023-05-25 08:20:34.000000 invenio-indexer-2.2.0/invenio_indexer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1800 2023-05-25 08:20:34.000000 invenio-indexer-2.2.0/invenio_indexer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 08:20:34.000000 invenio-indexer-2.2.0/invenio_indexer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-25 08:20:34.000000 invenio-indexer-2.2.0/invenio_indexer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 08:20:34.000000 invenio-indexer-2.2.0/invenio_indexer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-05-25 08:20:34.000000 invenio-indexer-2.2.0/invenio_indexer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-25 08:20:34.000000 invenio-indexer-2.2.0/invenio_indexer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (122)      756 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-05-25 08:20:34.997163 invenio-indexer-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.997163 invenio-indexer-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3049 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.997163 invenio-indexer-2.2.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.997163 invenio-indexer-2.2.0/tests/data/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/data/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.997163 invenio-indexer-2.2.0/tests/data/os-v1/records/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.997163 invenio-indexer-2.2.0/tests/data/os-v1/records/authorities/
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/data/os-v1/records/authorities/authority-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.997163 invenio-indexer-2.2.0/tests/data/os-v1/records/bibliographic/
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/data/os-v1/records/bibliographic/bibliographic-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/data/os-v1/records/default-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.997163 invenio-indexer-2.2.0/tests/data/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/data/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.997163 invenio-indexer-2.2.0/tests/data/os-v2/records/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.997163 invenio-indexer-2.2.0/tests/data/os-v2/records/authorities/
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/data/os-v2/records/authorities/authority-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.997163 invenio-indexer-2.2.0/tests/data/os-v2/records/bibliographic/
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/data/os-v2/records/bibliographic/bibliographic-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/data/os-v2/records/default-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.997163 invenio-indexer-2.2.0/tests/data/v7/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/data/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.997163 invenio-indexer-2.2.0/tests/data/v7/records/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.997163 invenio-indexer-2.2.0/tests/data/v7/records/authorities/
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/data/v7/records/authorities/authority-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.997163 invenio-indexer-2.2.0/tests/data/v7/records/bibliographic/
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/data/v7/records/bibliographic/bibliographic-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/data/v7/records/default-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:20:34.997163 invenio-indexer-2.2.0/tests/demo/
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/demo/json_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14030 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6307 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6002 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/test_invenio_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1188 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1372 2023-05-25 08:20:27.000000 invenio-indexer-2.2.0/tests/test_utils.py
```

### Comparing `invenio-indexer-2.1.2/.editorconfig` & `invenio-indexer-2.2.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/.github/workflows/pypi-publish.yml` & `invenio-indexer-2.2.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/.github/workflows/tests.yml` & `invenio-indexer-2.2.0/.github/workflows/tests.yml`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   Tests:
     runs-on: ubuntu-20.04
     strategy:
       matrix:
         python-version: [3.7, 3.8, 3.9]
         requirements-level: [pypi]
         cache-service: [redis]
-        mq-service: [rabbitmq, redis]
+        mq-service: [rabbitmq]
         search-service: [opensearch2,elasticsearch7]
 
         include:
           - search-service: opensearch2
             SEARCH_EXTRAS: "opensearch2"
 
           - search-service: elasticsearch7
```

### Comparing `invenio-indexer-2.1.2/AUTHORS.rst` & `invenio-indexer-2.2.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/CHANGES.rst` & `invenio-indexer-2.2.0/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 2.2.0 (released 2023-05-25)
+
+- cli: add queue selection options
+- tests: remove redis as message backend
+
 Version 2.1.2 (released 2023-05-05)
 
 - Allow passing message queue producer publish arguments via the ``RecordIndexer``
   constructor and the ``INDEXER_MQ_PUBLISH_KWARGS`` config.
 
 Version 2.1.1 (released 2022-10-07)
```

### Comparing `invenio-indexer-2.1.2/CONTRIBUTING.rst` & `invenio-indexer-2.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/INSTALL.rst` & `invenio-indexer-2.2.0/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/LICENSE` & `invenio-indexer-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/MANIFEST.in` & `invenio-indexer-2.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/PKG-INFO` & `invenio-indexer-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-indexer
-Version: 2.1.2
+Version: 2.2.0
 Summary: "Record indexer for Invenio."
 Home-page: https://github.com/inveniosoftware/invenio-indexer
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -41,14 +41,19 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.2.0 (released 2023-05-25)
+        
+        - cli: add queue selection options
+        - tests: remove redis as message backend
+        
         Version 2.1.2 (released 2023-05-05)
         
         - Allow passing message queue producer publish arguments via the ``RecordIndexer``
           constructor and the ``INDEXER_MQ_PUBLISH_KWARGS`` config.
         
         Version 2.1.1 (released 2022-10-07)
```

### Comparing `invenio-indexer-2.1.2/README.rst` & `invenio-indexer-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/docs/Makefile` & `invenio-indexer-2.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/docs/api.rst` & `invenio-indexer-2.2.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/docs/conf.py` & `invenio-indexer-2.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/docs/index.rst` & `invenio-indexer-2.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/docs/make.bat` & `invenio-indexer-2.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/invenio_indexer/__init__.py` & `invenio-indexer-2.2.0/invenio_indexer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,10 +176,10 @@
 >>> res = before_record_index.dynamic_connect(
 ...     indexer_receiver, sender=app, index='authors-v1.0.0')
 """
 
 from .ext import InvenioIndexer
 from .proxies import current_record_to_index
 
-__version__ = "2.1.2"
+__version__ = "2.2.0"
 
 __all__ = ("__version__", "InvenioIndexer", "current_record_to_index")
```

### Comparing `invenio-indexer-2.1.2/invenio_indexer/api.py` & `invenio-indexer-2.2.0/invenio_indexer/api.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/invenio_indexer/cli.py` & `invenio-indexer-2.2.0/invenio_indexer/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from celery.messaging import establish_connection
 from flask import current_app
 from flask.cli import with_appcontext
 from invenio_pidstore.models import PersistentIdentifier, PIDStatus
 from invenio_search.cli import index
 
 from .api import RecordIndexer
+from .proxies import current_indexer_registry
 from .tasks import process_bulk_queue
 
 
 def abort_if_false(ctx, param, value):
     """Abort command is value is False."""
     if not value:
         ctx.abort()
@@ -106,27 +107,38 @@
         .values(PersistentIdentifier.object_uuid)
     )
     RecordIndexer().bulk_index(query)
     click.secho('Execute "run" command to process the queue!', fg="yellow")
 
 
 @index.group(chain=True)
-def queue():
+@click.option("-q", "--queue", "indexer_ids", multiple=True)
+@click.option("-a", "--all-queues", is_flag=True)
+def queue(indexer_ids=[], all_queues=False):
     """Manage indexing queue."""
 
 
 @resultcallback(queue)
 @with_appcontext
-def process_actions(actions):
+def process_actions(actions, indexer_ids=[], all_queues=False):
     """Process queue actions."""
-    queue = current_app.config["INDEXER_MQ_QUEUE"]
+    # Resolve indexer IDs
+    if all_queues:
+        indexers = current_indexer_registry.all().values()
+    else:
+        indexers = [current_indexer_registry.get(i) for i in indexer_ids]
+    # Get queues
+    queues = [i.mq_queue for i in indexers]
+    # Always add the default indexer queue (for backwards compatibility)
+    queues.append(current_app.config["INDEXER_MQ_QUEUE"])
     with establish_connection() as c:
-        q = queue(c)
-        for action in actions:
-            q = action(q)
+        for queue in queues:
+            bound_queue = queue(c)
+            for action in actions:
+                action(bound_queue)
 
 
 @queue.command("init")
 def init_queue():
     """Initialize indexing queue."""
 
     def action(queue):
```

### Comparing `invenio-indexer-2.1.2/invenio_indexer/config.py` & `invenio-indexer-2.2.0/invenio_indexer/config.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/invenio_indexer/ext.py` & `invenio-indexer-2.2.0/invenio_indexer/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/invenio_indexer/proxies.py` & `invenio-indexer-2.2.0/invenio_indexer/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/invenio_indexer/registry.py` & `invenio-indexer-2.2.0/invenio_indexer/registry.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/invenio_indexer/signals.py` & `invenio-indexer-2.2.0/invenio_indexer/signals.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/invenio_indexer/tasks.py` & `invenio-indexer-2.2.0/invenio_indexer/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/invenio_indexer/utils.py` & `invenio-indexer-2.2.0/invenio_indexer/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/invenio_indexer.egg-info/PKG-INFO` & `invenio-indexer-2.2.0/invenio_indexer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-indexer
-Version: 2.1.2
+Version: 2.2.0
 Summary: "Record indexer for Invenio."
 Home-page: https://github.com/inveniosoftware/invenio-indexer
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -41,14 +41,19 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.2.0 (released 2023-05-25)
+        
+        - cli: add queue selection options
+        - tests: remove redis as message backend
+        
         Version 2.1.2 (released 2023-05-05)
         
         - Allow passing message queue producer publish arguments via the ``RecordIndexer``
           constructor and the ``INDEXER_MQ_PUBLISH_KWARGS`` config.
         
         Version 2.1.1 (released 2022-10-07)
```

### Comparing `invenio-indexer-2.1.2/invenio_indexer.egg-info/SOURCES.txt` & `invenio-indexer-2.2.0/invenio_indexer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/run-tests.sh` & `invenio-indexer-2.2.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/setup.cfg` & `invenio-indexer-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/tests/conftest.py` & `invenio-indexer-2.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/tests/test_api.py` & `invenio-indexer-2.2.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/tests/test_invenio_indexer.py` & `invenio-indexer-2.2.0/tests/test_invenio_indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/tests/test_registry.py` & `invenio-indexer-2.2.0/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/tests/test_tasks.py` & `invenio-indexer-2.2.0/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.2/tests/test_utils.py` & `invenio-indexer-2.2.0/tests/test_utils.py`

 * *Files identical despite different names*

