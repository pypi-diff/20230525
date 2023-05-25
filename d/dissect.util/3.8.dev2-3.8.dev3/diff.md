# Comparing `tmp/dissect.util-3.8.dev2.tar.gz` & `tmp/dissect.util-3.8.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.util-3.8.dev2.tar", last modified: Mon May 15 12:47:09 2023, max compression
+gzip compressed data, was "dissect.util-3.8.dev3.tar", last modified: Tue May 16 13:25:32 2023, max compression
```

## Comparing `dissect.util-3.8.dev2.tar` & `dissect.util-3.8.dev3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:09.768098 dissect.util-3.8.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-15 12:47:09.768098 dissect.util-3.8.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:09.760099 dissect.util-3.8.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:09.764099 dissect.util-3.8.dev2/dissect/util/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/dissect/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:09.764099 dissect.util-3.8.dev2/dissect/util/compression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/dissect/util/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/dissect/util/compression/lz4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/dissect/util/compression/lznt1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/dissect/util/compression/lzo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/dissect/util/compression/lzxpress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/dissect/util/compression/lzxpress_huffman.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/dissect/util/compression/sevenbit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/dissect/util/cpio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:09.764099 dissect.util-3.8.dev2/dissect/util/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/dissect/util/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/dissect/util/encoding/surrogateescape.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/dissect/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/dissect/util/plist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/dissect/util/sid.py
--rw-r--r--   0 runner    (1001) docker     (123)    18781 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/dissect/util/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:09.764099 dissect.util-3.8.dev2/dissect/util/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/dissect/util/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/dissect/util/tools/dump_nskeyedarchiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/dissect/util/ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/dissect/util/xmemoryview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:09.764099 dissect.util-3.8.dev2/dissect.util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-15 12:47:09.000000 dissect.util-3.8.dev2/dissect.util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-15 12:47:09.000000 dissect.util-3.8.dev2/dissect.util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:47:09.000000 dissect.util-3.8.dev2/dissect.util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-15 12:47:09.000000 dissect.util-3.8.dev2/dissect.util.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:47:09.000000 dissect.util-3.8.dev2/dissect.util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-15 12:47:00.000000 dissect.util-3.8.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:47:09.768098 dissect.util-3.8.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:09.768098 dissect.util-3.8.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:09.768098 dissect.util-3.8.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/tests/data/bin.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/tests/data/crc.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/tests/data/hpbin.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/tests/data/hpodc.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/tests/data/newc.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/tests/data/odc.cpio.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:09.768098 dissect.util-3.8.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/tests/test_cpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/tests/test_plist.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/tests/test_sid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/tests/test_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/tests/test_xmemoryview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:46:55.000000 dissect.util-3.8.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.017402 dissect.util-3.8.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-16 13:25:32.017402 dissect.util-3.8.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.009402 dissect.util-3.8.dev3/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.013402 dissect.util-3.8.dev3/dissect/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.013402 dissect.util-3.8.dev3/dissect/util/compression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/compression/lz4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/compression/lznt1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/compression/lzo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/compression/lzxpress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/compression/lzxpress_huffman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/compression/sevenbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/cpio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.013402 dissect.util-3.8.dev3/dissect/util/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/encoding/surrogateescape.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/plist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/sid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18781 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.013402 dissect.util-3.8.dev3/dissect/util/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/tools/dump_nskeyedarchiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/xmemoryview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.009402 dissect.util-3.8.dev3/dissect.util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-16 13:25:31.000000 dissect.util-3.8.dev3/dissect.util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-16 13:25:32.000000 dissect.util-3.8.dev3/dissect.util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:25:31.000000 dissect.util-3.8.dev3/dissect.util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 13:25:31.000000 dissect.util-3.8.dev3/dissect.util.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:25:31.000000 dissect.util-3.8.dev3/dissect.util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-16 13:25:18.000000 dissect.util-3.8.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:25:32.017402 dissect.util-3.8.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.017402 dissect.util-3.8.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.017402 dissect.util-3.8.dev3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/data/bin.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/data/crc.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/data/hpbin.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/data/hpodc.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/data/newc.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/data/odc.cpio.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.017402 dissect.util-3.8.dev3/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/test_cpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/test_plist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/test_sid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/test_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/test_xmemoryview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tox.ini
```

### Comparing `dissect.util-3.8.dev2/LICENSE` & `dissect.util-3.8.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/PKG-INFO` & `dissect.util-3.8.dev3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.util
-Version: 3.8.dev2
+Version: 3.8.dev3
 Summary: A Dissect module implementing various utility functions for the other Dissect modules
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.util
 Project-URL: repository, https://github.com/fox-it/dissect.util
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,20 @@
 License-File: COPYRIGHT
 
 # dissect.util
 
 A Dissect module implementing various utility functions for the other Dissect modules. For more information, please see
 [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.util/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.util` is available on [PyPI](https://pypi.org/project/dissect.util/).
 
 ```bash
 pip install dissect.util
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

### Comparing `dissect.util-3.8.dev2/README.md` & `dissect.util-3.8.dev3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # dissect.util
 
 A Dissect module implementing various utility functions for the other Dissect modules. For more information, please see
 [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.util/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.util` is available on [PyPI](https://pypi.org/project/dissect.util/).
 
 ```bash
 pip install dissect.util
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

### Comparing `dissect.util-3.8.dev2/dissect/util/compression/lz4.py` & `dissect.util-3.8.dev3/dissect/util/compression/lz4.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/dissect/util/compression/lznt1.py` & `dissect.util-3.8.dev3/dissect/util/compression/lznt1.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/dissect/util/compression/lzo.py` & `dissect.util-3.8.dev3/dissect/util/compression/lzo.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/dissect/util/compression/lzxpress.py` & `dissect.util-3.8.dev3/dissect/util/compression/lzxpress.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/dissect/util/compression/lzxpress_huffman.py` & `dissect.util-3.8.dev3/dissect/util/compression/lzxpress_huffman.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/dissect/util/compression/sevenbit.py` & `dissect.util-3.8.dev3/dissect/util/compression/sevenbit.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/dissect/util/cpio.py` & `dissect.util-3.8.dev3/dissect/util/cpio.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/dissect/util/plist.py` & `dissect.util-3.8.dev3/dissect/util/plist.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/dissect/util/sid.py` & `dissect.util-3.8.dev3/dissect/util/sid.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/dissect/util/stream.py` & `dissect.util-3.8.dev3/dissect/util/stream.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/dissect/util/tools/dump_nskeyedarchiver.py` & `dissect.util-3.8.dev3/dissect/util/tools/dump_nskeyedarchiver.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/dissect/util/ts.py` & `dissect.util-3.8.dev3/dissect/util/ts.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/dissect/util/xmemoryview.py` & `dissect.util-3.8.dev3/dissect/util/xmemoryview.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/dissect.util.egg-info/PKG-INFO` & `dissect.util-3.8.dev3/dissect.util.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.util
-Version: 3.8.dev2
+Version: 3.8.dev3
 Summary: A Dissect module implementing various utility functions for the other Dissect modules
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.util
 Project-URL: repository, https://github.com/fox-it/dissect.util
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,20 @@
 License-File: COPYRIGHT
 
 # dissect.util
 
 A Dissect module implementing various utility functions for the other Dissect modules. For more information, please see
 [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.util/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.util` is available on [PyPI](https://pypi.org/project/dissect.util/).
 
 ```bash
 pip install dissect.util
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

### Comparing `dissect.util-3.8.dev2/dissect.util.egg-info/SOURCES.txt` & `dissect.util-3.8.dev3/dissect.util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/pyproject.toml` & `dissect.util-3.8.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/tests/data/bin.cpio.gz` & `dissect.util-3.8.dev3/tests/data/bin.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/tests/data/crc.cpio.gz` & `dissect.util-3.8.dev3/tests/data/crc.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/tests/data/hpbin.cpio.gz` & `dissect.util-3.8.dev3/tests/data/hpbin.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/tests/data/hpodc.cpio.gz` & `dissect.util-3.8.dev3/tests/data/hpodc.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/tests/data/newc.cpio.gz` & `dissect.util-3.8.dev3/tests/data/newc.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/tests/data/odc.cpio.gz` & `dissect.util-3.8.dev3/tests/data/odc.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/tests/docs/Makefile` & `dissect.util-3.8.dev3/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/tests/docs/conf.py` & `dissect.util-3.8.dev3/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/tests/test_compression.py` & `dissect.util-3.8.dev3/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/tests/test_cpio.py` & `dissect.util-3.8.dev3/tests/test_cpio.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/tests/test_plist.py` & `dissect.util-3.8.dev3/tests/test_plist.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/tests/test_sid.py` & `dissect.util-3.8.dev3/tests/test_sid.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/tests/test_stream.py` & `dissect.util-3.8.dev3/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/tests/test_ts.py` & `dissect.util-3.8.dev3/tests/test_ts.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/tests/test_xmemoryview.py` & `dissect.util-3.8.dev3/tests/test_xmemoryview.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev2/tox.ini` & `dissect.util-3.8.dev3/tox.ini`

 * *Files identical despite different names*

