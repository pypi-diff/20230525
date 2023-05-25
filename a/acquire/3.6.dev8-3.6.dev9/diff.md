# Comparing `tmp/acquire-3.6.dev8.tar.gz` & `tmp/acquire-3.6.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acquire-3.6.dev8.tar", last modified: Mon May 15 12:44:54 2023, max compression
+gzip compressed data, was "acquire-3.6.dev9.tar", last modified: Tue May 16 13:24:44 2023, max compression
```

## Comparing `acquire-3.6.dev8.tar` & `acquire-3.6.dev9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.021101 acquire-3.6.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-15 12:44:40.000000 acquire-3.6.dev8/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:44:40.000000 acquire-3.6.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:44:40.000000 acquire-3.6.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-15 12:44:54.021101 acquire-3.6.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-15 12:44:40.000000 acquire-3.6.dev8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.017101 acquire-3.6.dev8/acquire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    75961 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/acquire.py
--rw-r--r--   0 runner    (1001) docker     (123)    21084 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.017101 acquire-3.6.dev8/acquire/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/dynamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.017101 acquire-3.6.dev8/acquire/dynamic/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/dynamic/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/dynamic/windows/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/dynamic/windows/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/dynamic/windows/handles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/dynamic/windows/named_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/dynamic/windows/ntdll.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/dynamic/windows/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/esxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.017101 acquire-3.6.dev8/acquire/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/outputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/outputs/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/outputs/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.017101 acquire-3.6.dev8/acquire/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/tools/decrypter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.021101 acquire-3.6.dev8/acquire/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/uploaders/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/uploaders/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/uploaders/plugin_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-15 12:44:40.000000 acquire-3.6.dev8/acquire/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-15 12:44:53.000000 acquire-3.6.dev8/acquire/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.017101 acquire-3.6.dev8/acquire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-15 12:44:53.000000 acquire-3.6.dev8/acquire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-15 12:44:54.000000 acquire-3.6.dev8/acquire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:44:53.000000 acquire-3.6.dev8/acquire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-15 12:44:53.000000 acquire-3.6.dev8/acquire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-15 12:44:53.000000 acquire-3.6.dev8/acquire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:44:53.000000 acquire-3.6.dev8/acquire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-15 12:44:44.000000 acquire-3.6.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:44:54.021101 acquire-3.6.dev8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.021101 acquire-3.6.dev8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:44:54.021101 acquire-3.6.dev8/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/test_acquire_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/test_esxi_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/test_file_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/test_minio_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-15 12:44:40.000000 acquire-3.6.dev8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:44.807918 acquire-3.6.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-16 13:24:30.000000 acquire-3.6.dev9/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:24:30.000000 acquire-3.6.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:24:30.000000 acquire-3.6.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-16 13:24:44.807918 acquire-3.6.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-16 13:24:30.000000 acquire-3.6.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:44.795918 acquire-3.6.dev9/acquire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75961 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/acquire.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21084 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:44.795918 acquire-3.6.dev9/acquire/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/dynamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:44.799918 acquire-3.6.dev9/acquire/dynamic/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/dynamic/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/dynamic/windows/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/dynamic/windows/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/dynamic/windows/handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/dynamic/windows/named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/dynamic/windows/ntdll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/dynamic/windows/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/esxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:44.799918 acquire-3.6.dev9/acquire/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/outputs/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/outputs/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:44.799918 acquire-3.6.dev9/acquire/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/tools/decrypter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:44.803918 acquire-3.6.dev9/acquire/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/uploaders/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/uploaders/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/uploaders/plugin_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-16 13:24:30.000000 acquire-3.6.dev9/acquire/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-16 13:24:44.000000 acquire-3.6.dev9/acquire/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:44.795918 acquire-3.6.dev9/acquire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-16 13:24:44.000000 acquire-3.6.dev9/acquire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-16 13:24:44.000000 acquire-3.6.dev9/acquire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:24:44.000000 acquire-3.6.dev9/acquire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 13:24:44.000000 acquire-3.6.dev9/acquire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-16 13:24:44.000000 acquire-3.6.dev9/acquire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:24:44.000000 acquire-3.6.dev9/acquire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-16 13:24:35.000000 acquire-3.6.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:24:44.807918 acquire-3.6.dev9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:44.807918 acquire-3.6.dev9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:30.000000 acquire-3.6.dev9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-16 13:24:30.000000 acquire-3.6.dev9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:44.807918 acquire-3.6.dev9/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:24:30.000000 acquire-3.6.dev9/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:24:30.000000 acquire-3.6.dev9/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:24:30.000000 acquire-3.6.dev9/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-16 13:24:30.000000 acquire-3.6.dev9/tests/test_acquire_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-05-16 13:24:30.000000 acquire-3.6.dev9/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-16 13:24:30.000000 acquire-3.6.dev9/tests/test_esxi_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-16 13:24:30.000000 acquire-3.6.dev9/tests/test_file_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-16 13:24:30.000000 acquire-3.6.dev9/tests/test_minio_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-16 13:24:30.000000 acquire-3.6.dev9/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-05-16 13:24:30.000000 acquire-3.6.dev9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-16 13:24:30.000000 acquire-3.6.dev9/tox.ini
```

### Comparing `acquire-3.6.dev8/LICENSE` & `acquire-3.6.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/PKG-INFO` & `acquire-3.6.dev9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.6.dev8
+Version: 3.6.dev9
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Programming Language :: Python :: 3
@@ -32,14 +32,20 @@
 ```
 
 The tool requires administrative access to read raw disk data instead of using the operating system for file access.
 However, there are some options available to use the operating system as a fallback option. (e.g `--fallback` or `--force-fallback`)
 
 For more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/acquire/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `acquire` is available on [PyPI](https://pypi.org/project/acquire/).
 
 ```bash
 pip install acquire
 ```
@@ -59,20 +65,20 @@
 using the default installed Python version, run:
 
 ```bash
 tox
 ```
 
 For a more elaborate explanation on how to build and test the project, please see [the
-documentation](https://docs.dissect.tools/en/latest/contributing/developing.html#building-testing).
+documentation](https://docs.dissect.tools/en/latest/contributing/tooling.html).
 
 ## Contributing
 
 The Dissect project encourages any contribution to the codebase. To make your contribution fit into the project, please
-refer to [the style guide](https://docs.dissect.tools/en/latest/contributing/style-guide.html).
+refer to [the development guide](https://docs.dissect.tools/en/latest/contributing/developing.html).
 
 ## Copyright and license
 
 Dissect is released as open source by Fox-IT (<https://www.fox-it.com>) part of NCC Group Plc
 (<https://www.nccgroup.com>).
 
 Developed by the Dissect Team (<dissect@fox-it.com>) and made available at <https://github.com/fox-it/acquire>.
```

### Comparing `acquire-3.6.dev8/README.md` & `acquire-3.6.dev9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,20 @@
 ```
 
 The tool requires administrative access to read raw disk data instead of using the operating system for file access.
 However, there are some options available to use the operating system as a fallback option. (e.g `--fallback` or `--force-fallback`)
 
 For more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/acquire/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `acquire` is available on [PyPI](https://pypi.org/project/acquire/).
 
 ```bash
 pip install acquire
 ```
@@ -43,20 +49,20 @@
 using the default installed Python version, run:
 
 ```bash
 tox
 ```
 
 For a more elaborate explanation on how to build and test the project, please see [the
-documentation](https://docs.dissect.tools/en/latest/contributing/developing.html#building-testing).
+documentation](https://docs.dissect.tools/en/latest/contributing/tooling.html).
 
 ## Contributing
 
 The Dissect project encourages any contribution to the codebase. To make your contribution fit into the project, please
-refer to [the style guide](https://docs.dissect.tools/en/latest/contributing/style-guide.html).
+refer to [the development guide](https://docs.dissect.tools/en/latest/contributing/developing.html).
 
 ## Copyright and license
 
 Dissect is released as open source by Fox-IT (<https://www.fox-it.com>) part of NCC Group Plc
 (<https://www.nccgroup.com>).
 
 Developed by the Dissect Team (<dissect@fox-it.com>) and made available at <https://github.com/fox-it/acquire>.
```

### Comparing `acquire-3.6.dev8/acquire/acquire.py` & `acquire-3.6.dev9/acquire/acquire.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/acquire/collector.py` & `acquire-3.6.dev9/acquire/collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/acquire/crypt.py` & `acquire-3.6.dev9/acquire/crypt.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/acquire/dynamic/windows/collect.py` & `acquire-3.6.dev9/acquire/dynamic/windows/collect.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/acquire/dynamic/windows/handles.py` & `acquire-3.6.dev9/acquire/dynamic/windows/handles.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/acquire/dynamic/windows/named_objects.py` & `acquire-3.6.dev9/acquire/dynamic/windows/named_objects.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/acquire/dynamic/windows/ntdll.py` & `acquire-3.6.dev9/acquire/dynamic/windows/ntdll.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/acquire/dynamic/windows/types.py` & `acquire-3.6.dev9/acquire/dynamic/windows/types.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/acquire/esxi.py` & `acquire-3.6.dev9/acquire/esxi.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/acquire/hashes.py` & `acquire-3.6.dev9/acquire/hashes.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/acquire/log.py` & `acquire-3.6.dev9/acquire/log.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/acquire/outputs/base.py` & `acquire-3.6.dev9/acquire/outputs/base.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/acquire/outputs/dir.py` & `acquire-3.6.dev9/acquire/outputs/dir.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/acquire/outputs/tar.py` & `acquire-3.6.dev9/acquire/outputs/tar.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/acquire/tools/decrypter.py` & `acquire-3.6.dev9/acquire/tools/decrypter.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/acquire/uploaders/minio.py` & `acquire-3.6.dev9/acquire/uploaders/minio.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/acquire/uploaders/plugin.py` & `acquire-3.6.dev9/acquire/uploaders/plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/acquire/uploaders/plugin_registry.py` & `acquire-3.6.dev9/acquire/uploaders/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/acquire/utils.py` & `acquire-3.6.dev9/acquire/utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/acquire.egg-info/PKG-INFO` & `acquire-3.6.dev9/acquire.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.6.dev8
+Version: 3.6.dev9
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Programming Language :: Python :: 3
@@ -32,14 +32,20 @@
 ```
 
 The tool requires administrative access to read raw disk data instead of using the operating system for file access.
 However, there are some options available to use the operating system as a fallback option. (e.g `--fallback` or `--force-fallback`)
 
 For more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/acquire/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `acquire` is available on [PyPI](https://pypi.org/project/acquire/).
 
 ```bash
 pip install acquire
 ```
@@ -59,20 +65,20 @@
 using the default installed Python version, run:
 
 ```bash
 tox
 ```
 
 For a more elaborate explanation on how to build and test the project, please see [the
-documentation](https://docs.dissect.tools/en/latest/contributing/developing.html#building-testing).
+documentation](https://docs.dissect.tools/en/latest/contributing/tooling.html).
 
 ## Contributing
 
 The Dissect project encourages any contribution to the codebase. To make your contribution fit into the project, please
-refer to [the style guide](https://docs.dissect.tools/en/latest/contributing/style-guide.html).
+refer to [the development guide](https://docs.dissect.tools/en/latest/contributing/developing.html).
 
 ## Copyright and license
 
 Dissect is released as open source by Fox-IT (<https://www.fox-it.com>) part of NCC Group Plc
 (<https://www.nccgroup.com>).
 
 Developed by the Dissect Team (<dissect@fox-it.com>) and made available at <https://github.com/fox-it/acquire>.
```

### Comparing `acquire-3.6.dev8/acquire.egg-info/SOURCES.txt` & `acquire-3.6.dev9/acquire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/pyproject.toml` & `acquire-3.6.dev9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/tests/conftest.py` & `acquire-3.6.dev9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/tests/docs/Makefile` & `acquire-3.6.dev9/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/tests/docs/conf.py` & `acquire-3.6.dev9/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/tests/test_acquire_command.py` & `acquire-3.6.dev9/tests/test_acquire_command.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/tests/test_collector.py` & `acquire-3.6.dev9/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/tests/test_esxi_memory.py` & `acquire-3.6.dev9/tests/test_esxi_memory.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/tests/test_file_sorting.py` & `acquire-3.6.dev9/tests/test_file_sorting.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/tests/test_minio_uploader.py` & `acquire-3.6.dev9/tests/test_minio_uploader.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/tests/test_plugin.py` & `acquire-3.6.dev9/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/tests/test_utils.py` & `acquire-3.6.dev9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev8/tox.ini` & `acquire-3.6.dev9/tox.ini`

 * *Files identical despite different names*

