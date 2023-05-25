# Comparing `tmp/dissect.squashfs-1.2.dev1.tar.gz` & `tmp/dissect.squashfs-1.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.squashfs-1.2.dev1.tar", last modified: Mon May 15 12:48:29 2023, max compression
+gzip compressed data, was "dissect.squashfs-1.2.dev2.tar", last modified: Tue May 16 13:26:52 2023, max compression
```

## Comparing `dissect.squashfs-1.2.dev1.tar` & `dissect.squashfs-1.2.dev2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:29.469721 dissect.squashfs-1.2.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-15 12:48:29.469721 dissect.squashfs-1.2.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:29.457721 dissect.squashfs-1.2.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:29.461721 dissect.squashfs-1.2.dev1/dissect/squashfs/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/dissect/squashfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/dissect/squashfs/c_squashfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/dissect/squashfs/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/dissect/squashfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/dissect/squashfs/squashfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:29.461721 dissect.squashfs-1.2.dev1/dissect.squashfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-15 12:48:29.000000 dissect.squashfs-1.2.dev1/dissect.squashfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-15 12:48:29.000000 dissect.squashfs-1.2.dev1/dissect.squashfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:48:29.000000 dissect.squashfs-1.2.dev1/dissect.squashfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-15 12:48:29.000000 dissect.squashfs-1.2.dev1/dissect.squashfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:48:29.000000 dissect.squashfs-1.2.dev1/dissect.squashfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-15 12:48:19.000000 dissect.squashfs-1.2.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:48:29.469721 dissect.squashfs-1.2.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:29.465721 dissect.squashfs-1.2.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:29.465721 dissect.squashfs-1.2.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/data/gzip-opts.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/data/gzip.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/data/lz4.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/data/lzma.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)    28672 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/data/lzo.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/data/xz.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/data/zstd.sqfs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:29.469721 dissect.squashfs-1.2.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/test_squashfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:52.276617 dissect.squashfs-1.2.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-16 13:26:52.276617 dissect.squashfs-1.2.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:52.268617 dissect.squashfs-1.2.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:52.272617 dissect.squashfs-1.2.dev2/dissect/squashfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/dissect/squashfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/dissect/squashfs/c_squashfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/dissect/squashfs/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/dissect/squashfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/dissect/squashfs/squashfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:52.272617 dissect.squashfs-1.2.dev2/dissect.squashfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-16 13:26:52.000000 dissect.squashfs-1.2.dev2/dissect.squashfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-16 13:26:52.000000 dissect.squashfs-1.2.dev2/dissect.squashfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:26:52.000000 dissect.squashfs-1.2.dev2/dissect.squashfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 13:26:52.000000 dissect.squashfs-1.2.dev2/dissect.squashfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:26:52.000000 dissect.squashfs-1.2.dev2/dissect.squashfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-16 13:26:42.000000 dissect.squashfs-1.2.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:26:52.276617 dissect.squashfs-1.2.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:52.272617 dissect.squashfs-1.2.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:52.276617 dissect.squashfs-1.2.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/tests/data/gzip-opts.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/tests/data/gzip.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/tests/data/lz4.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/tests/data/lzma.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)    28672 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/tests/data/lzo.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/tests/data/xz.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/tests/data/zstd.sqfs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:52.276617 dissect.squashfs-1.2.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/tests/test_squashfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-16 13:26:34.000000 dissect.squashfs-1.2.dev2/tox.ini
```

### Comparing `dissect.squashfs-1.2.dev1/LICENSE` & `dissect.squashfs-1.2.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.2.dev1/PKG-INFO` & `dissect.squashfs-1.2.dev2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.squashfs
-Version: 1.2.dev1
+Version: 1.2.dev2
 Summary: A Dissect module implementing a parser for the SquashFS file system, commonly used in appliance or device firmware
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.squashfs
 Project-URL: repository, https://github.com/fox-it/dissect.squashfs
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,20 @@
 License-File: COPYRIGHT
 
 # dissect.squashfs
 
 A Dissect module implementing a parser for the SquashFS file system, commonly used in appliance or device firmware. For more
 information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.squashfs/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.squashfs` is available on [PyPI](https://pypi.org/project/dissect.squashfs/).
 
 ```bash
 pip install dissect.squashfs
 ```
@@ -44,20 +50,20 @@
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

### Comparing `dissect.squashfs-1.2.dev1/README.md` & `dissect.squashfs-1.2.dev2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # dissect.squashfs
 
 A Dissect module implementing a parser for the SquashFS file system, commonly used in appliance or device firmware. For more
 information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.squashfs/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.squashfs` is available on [PyPI](https://pypi.org/project/dissect.squashfs/).
 
 ```bash
 pip install dissect.squashfs
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

### Comparing `dissect.squashfs-1.2.dev1/dissect/squashfs/c_squashfs.py` & `dissect.squashfs-1.2.dev2/dissect/squashfs/c_squashfs.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.2.dev1/dissect/squashfs/compression.py` & `dissect.squashfs-1.2.dev2/dissect/squashfs/compression.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.2.dev1/dissect/squashfs/squashfs.py` & `dissect.squashfs-1.2.dev2/dissect/squashfs/squashfs.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.2.dev1/dissect.squashfs.egg-info/PKG-INFO` & `dissect.squashfs-1.2.dev2/dissect.squashfs.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.squashfs
-Version: 1.2.dev1
+Version: 1.2.dev2
 Summary: A Dissect module implementing a parser for the SquashFS file system, commonly used in appliance or device firmware
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.squashfs
 Project-URL: repository, https://github.com/fox-it/dissect.squashfs
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,20 @@
 License-File: COPYRIGHT
 
 # dissect.squashfs
 
 A Dissect module implementing a parser for the SquashFS file system, commonly used in appliance or device firmware. For more
 information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.squashfs/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.squashfs` is available on [PyPI](https://pypi.org/project/dissect.squashfs/).
 
 ```bash
 pip install dissect.squashfs
 ```
@@ -44,20 +50,20 @@
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

### Comparing `dissect.squashfs-1.2.dev1/dissect.squashfs.egg-info/SOURCES.txt` & `dissect.squashfs-1.2.dev2/dissect.squashfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.2.dev1/pyproject.toml` & `dissect.squashfs-1.2.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.2.dev1/tests/conftest.py` & `dissect.squashfs-1.2.dev2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.2.dev1/tests/data/gzip-opts.sqfs` & `dissect.squashfs-1.2.dev2/tests/data/gzip-opts.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.2.dev1/tests/data/gzip.sqfs` & `dissect.squashfs-1.2.dev2/tests/data/gzip.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.2.dev1/tests/data/lz4.sqfs` & `dissect.squashfs-1.2.dev2/tests/data/lz4.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.2.dev1/tests/data/lzma.sqfs` & `dissect.squashfs-1.2.dev2/tests/data/lzma.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.2.dev1/tests/data/lzo.sqfs` & `dissect.squashfs-1.2.dev2/tests/data/lzo.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.2.dev1/tests/data/xz.sqfs` & `dissect.squashfs-1.2.dev2/tests/data/xz.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.2.dev1/tests/data/zstd.sqfs` & `dissect.squashfs-1.2.dev2/tests/data/zstd.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.2.dev1/tests/docs/Makefile` & `dissect.squashfs-1.2.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.2.dev1/tests/docs/conf.py` & `dissect.squashfs-1.2.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.2.dev1/tests/test_squashfs.py` & `dissect.squashfs-1.2.dev2/tests/test_squashfs.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.2.dev1/tox.ini` & `dissect.squashfs-1.2.dev2/tox.ini`

 * *Files identical despite different names*

