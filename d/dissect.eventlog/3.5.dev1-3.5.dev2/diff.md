# Comparing `tmp/dissect.eventlog-3.5.dev1.tar.gz` & `tmp/dissect.eventlog-3.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.eventlog-3.5.dev1.tar", last modified: Mon May 15 12:47:40 2023, max compression
+gzip compressed data, was "dissect.eventlog-3.5.dev2.tar", last modified: Tue May 16 13:25:50 2023, max compression
```

## Comparing `dissect.eventlog-3.5.dev1.tar` & `dissect.eventlog-3.5.dev2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:40.834092 dissect.eventlog-3.5.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-15 12:47:40.830093 dissect.eventlog-3.5.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:40.822092 dissect.eventlog-3.5.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:40.830093 dissect.eventlog-3.5.dev1/dissect/eventlog/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/dissect/eventlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22978 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/dissect/eventlog/bxml.py
--rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/dissect/eventlog/evt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/dissect/eventlog/evtx.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/dissect/eventlog/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/dissect/eventlog/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/dissect/eventlog/wevt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/dissect/eventlog/wevt_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/dissect/eventlog/wevtutil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:40.826092 dissect.eventlog-3.5.dev1/dissect.eventlog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-15 12:47:40.000000 dissect.eventlog-3.5.dev1/dissect.eventlog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-15 12:47:40.000000 dissect.eventlog-3.5.dev1/dissect.eventlog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:47:40.000000 dissect.eventlog-3.5.dev1/dissect.eventlog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:47:40.000000 dissect.eventlog-3.5.dev1/dissect.eventlog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:47:40.000000 dissect.eventlog-3.5.dev1/dissect.eventlog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:40.830093 dissect.eventlog-3.5.dev1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/examples/parse_wevt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/examples/pool_evtx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/examples/pool_wevtutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/examples/scrape_evt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/examples/scrape_evtx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/examples/splunkify_evtx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/examples/splunkify_wevtutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-15 12:47:29.000000 dissect.eventlog-3.5.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:47:40.834092 dissect.eventlog-3.5.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:40.830093 dissect.eventlog-3.5.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/tests/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:40.830093 dissect.eventlog-3.5.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    65536 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/tests/data/TestLog-dirty.evt
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/tests/data/TestLog.evt
--rw-r--r--   0 runner    (1001) docker     (123)    69632 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/tests/data/TestLogX.evtx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:40.830093 dissect.eventlog-3.5.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/tests/test_binxml.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/tests/test_crim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/tests/test_evt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/tests/test_evtx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/tests/test_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/tests/test_wevt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/tests/test_wevt_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/tests/test_wevtobj.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:47:24.000000 dissect.eventlog-3.5.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:50.722114 dissect.eventlog-3.5.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-16 13:25:50.722114 dissect.eventlog-3.5.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:50.698113 dissect.eventlog-3.5.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:50.710113 dissect.eventlog-3.5.dev2/dissect/eventlog/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/dissect/eventlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22978 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/dissect/eventlog/bxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/dissect/eventlog/evt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/dissect/eventlog/evtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/dissect/eventlog/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/dissect/eventlog/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/dissect/eventlog/wevt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/dissect/eventlog/wevt_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/dissect/eventlog/wevtutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:50.706113 dissect.eventlog-3.5.dev2/dissect.eventlog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-16 13:25:50.000000 dissect.eventlog-3.5.dev2/dissect.eventlog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-16 13:25:50.000000 dissect.eventlog-3.5.dev2/dissect.eventlog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:25:50.000000 dissect.eventlog-3.5.dev2/dissect.eventlog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:25:50.000000 dissect.eventlog-3.5.dev2/dissect.eventlog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:25:50.000000 dissect.eventlog-3.5.dev2/dissect.eventlog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:50.714114 dissect.eventlog-3.5.dev2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/examples/parse_wevt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/examples/pool_evtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/examples/pool_wevtutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/examples/scrape_evt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/examples/scrape_evtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/examples/splunkify_evtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/examples/splunkify_wevtutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-16 13:25:39.000000 dissect.eventlog-3.5.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:25:50.722114 dissect.eventlog-3.5.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:50.718114 dissect.eventlog-3.5.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/tests/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:50.722114 dissect.eventlog-3.5.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    65536 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/tests/data/TestLog-dirty.evt
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/tests/data/TestLog.evt
+-rw-r--r--   0 runner    (1001) docker     (123)    69632 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/tests/data/TestLogX.evtx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:50.722114 dissect.eventlog-3.5.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/tests/test_binxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/tests/test_crim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/tests/test_evt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/tests/test_evtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/tests/test_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/tests/test_wevt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/tests/test_wevt_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/tests/test_wevtobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:25:34.000000 dissect.eventlog-3.5.dev2/tox.ini
```

### Comparing `dissect.eventlog-3.5.dev1/LICENSE` & `dissect.eventlog-3.5.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/PKG-INFO` & `dissect.eventlog-3.5.dev2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.eventlog
-Version: 3.5.dev1
+Version: 3.5.dev2
 Summary: A Dissect module implementing parsers for the Windows EVT, EVTX and WEVT log file formats
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.eventlog
 Project-URL: repository, https://github.com/fox-it/dissect.eventlog
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,20 @@
 License-File: COPYRIGHT
 
 # dissect.eventlog
 
 A Dissect module implementing parsers for the Windows EVT, EVTX and WEVT log file formats. For more information, please
 see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.eventlog/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.eventlog` is available on [PyPI](https://pypi.org/project/dissect.eventlog/).
 
 ```bash
 pip install dissect.eventlog
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
 
 Developed by the Dissect Team (<dissect@fox-it.com>) and made available at <https://github.com/fox-it/dissect>.
```

### Comparing `dissect.eventlog-3.5.dev1/README.md` & `dissect.eventlog-3.5.dev2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # dissect.eventlog
 
 A Dissect module implementing parsers for the Windows EVT, EVTX and WEVT log file formats. For more information, please
 see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.eventlog/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.eventlog` is available on [PyPI](https://pypi.org/project/dissect.eventlog/).
 
 ```bash
 pip install dissect.eventlog
 ```
@@ -28,20 +34,20 @@
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
 
 Developed by the Dissect Team (<dissect@fox-it.com>) and made available at <https://github.com/fox-it/dissect>.
```

### Comparing `dissect.eventlog-3.5.dev1/dissect/eventlog/bxml.py` & `dissect.eventlog-3.5.dev2/dissect/eventlog/bxml.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/dissect/eventlog/evt.py` & `dissect.eventlog-3.5.dev2/dissect/eventlog/evt.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/dissect/eventlog/evtx.py` & `dissect.eventlog-3.5.dev2/dissect/eventlog/evtx.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/dissect/eventlog/wevt.py` & `dissect.eventlog-3.5.dev2/dissect/eventlog/wevt.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/dissect/eventlog/wevt_object.py` & `dissect.eventlog-3.5.dev2/dissect/eventlog/wevt_object.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/dissect/eventlog/wevtutil.py` & `dissect.eventlog-3.5.dev2/dissect/eventlog/wevtutil.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/dissect.eventlog.egg-info/PKG-INFO` & `dissect.eventlog-3.5.dev2/dissect.eventlog.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.eventlog
-Version: 3.5.dev1
+Version: 3.5.dev2
 Summary: A Dissect module implementing parsers for the Windows EVT, EVTX and WEVT log file formats
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.eventlog
 Project-URL: repository, https://github.com/fox-it/dissect.eventlog
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,20 @@
 License-File: COPYRIGHT
 
 # dissect.eventlog
 
 A Dissect module implementing parsers for the Windows EVT, EVTX and WEVT log file formats. For more information, please
 see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.eventlog/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.eventlog` is available on [PyPI](https://pypi.org/project/dissect.eventlog/).
 
 ```bash
 pip install dissect.eventlog
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
 
 Developed by the Dissect Team (<dissect@fox-it.com>) and made available at <https://github.com/fox-it/dissect>.
```

### Comparing `dissect.eventlog-3.5.dev1/dissect.eventlog.egg-info/SOURCES.txt` & `dissect.eventlog-3.5.dev2/dissect.eventlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/examples/parse_wevt.py` & `dissect.eventlog-3.5.dev2/examples/parse_wevt.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/examples/pool_evtx.py` & `dissect.eventlog-3.5.dev2/examples/pool_evtx.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/examples/pool_wevtutil.py` & `dissect.eventlog-3.5.dev2/examples/pool_wevtutil.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/examples/scrape_evt.py` & `dissect.eventlog-3.5.dev2/examples/scrape_evt.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/examples/scrape_evtx.py` & `dissect.eventlog-3.5.dev2/examples/scrape_evtx.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/examples/splunkify_evtx.py` & `dissect.eventlog-3.5.dev2/examples/splunkify_evtx.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/examples/splunkify_wevtutil.py` & `dissect.eventlog-3.5.dev2/examples/splunkify_wevtutil.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/pyproject.toml` & `dissect.eventlog-3.5.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/tests/_utils.py` & `dissect.eventlog-3.5.dev2/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/tests/data/TestLog-dirty.evt` & `dissect.eventlog-3.5.dev2/tests/data/TestLog-dirty.evt`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/tests/data/TestLog.evt` & `dissect.eventlog-3.5.dev2/tests/data/TestLog.evt`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/tests/data/TestLogX.evtx` & `dissect.eventlog-3.5.dev2/tests/data/TestLogX.evtx`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/tests/docs/Makefile` & `dissect.eventlog-3.5.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/tests/docs/conf.py` & `dissect.eventlog-3.5.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/tests/test_binxml.py` & `dissect.eventlog-3.5.dev2/tests/test_binxml.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/tests/test_crim.py` & `dissect.eventlog-3.5.dev2/tests/test_crim.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/tests/test_evt.py` & `dissect.eventlog-3.5.dev2/tests/test_evt.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/tests/test_evtx.py` & `dissect.eventlog-3.5.dev2/tests/test_evtx.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/tests/test_maps.py` & `dissect.eventlog-3.5.dev2/tests/test_maps.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/tests/test_wevt.py` & `dissect.eventlog-3.5.dev2/tests/test_wevt.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/tests/test_wevt_type.py` & `dissect.eventlog-3.5.dev2/tests/test_wevt_type.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/tests/test_wevtobj.py` & `dissect.eventlog-3.5.dev2/tests/test_wevtobj.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.5.dev1/tox.ini` & `dissect.eventlog-3.5.dev2/tox.ini`

 * *Files identical despite different names*

