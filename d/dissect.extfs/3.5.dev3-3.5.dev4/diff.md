# Comparing `tmp/dissect.extfs-3.5.dev3.tar.gz` & `tmp/dissect.extfs-3.5.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.extfs-3.5.dev3.tar", last modified: Mon May 15 12:47:58 2023, max compression
+gzip compressed data, was "dissect.extfs-3.5.dev4.tar", last modified: Tue May 16 13:25:57 2023, max compression
```

## Comparing `dissect.extfs-3.5.dev3.tar` & `dissect.extfs-3.5.dev4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:58.950386 dissect.extfs-3.5.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-15 12:47:58.950386 dissect.extfs-3.5.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:58.946386 dissect.extfs-3.5.dev3/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:58.950386 dissect.extfs-3.5.dev3/dissect/extfs/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/dissect/extfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23393 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/dissect/extfs/c_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/dissect/extfs/c_jdb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/dissect/extfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/dissect/extfs/extfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/dissect/extfs/journal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:58.946386 dissect.extfs-3.5.dev3/dissect.extfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-15 12:47:58.000000 dissect.extfs-3.5.dev3/dissect.extfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-15 12:47:58.000000 dissect.extfs-3.5.dev3/dissect.extfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:47:58.000000 dissect.extfs-3.5.dev3/dissect.extfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:47:58.000000 dissect.extfs-3.5.dev3/dissect.extfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:47:58.000000 dissect.extfs-3.5.dev3/dissect.extfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-15 12:47:42.000000 dissect.extfs-3.5.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:47:58.954386 dissect.extfs-3.5.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:58.950386 dissect.extfs-3.5.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:33.000000 dissect.extfs-3.5.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:58.950386 dissect.extfs-3.5.dev3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/data/ext4.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/data/ext4_sparse.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/data/ext4_symlink_test1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/data/ext4_symlink_test2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/data/ext4_symlink_test3.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:58.950386 dissect.extfs-3.5.dev3/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/test_ext4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:57.427714 dissect.extfs-3.5.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-16 13:25:57.427714 dissect.extfs-3.5.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:57.411713 dissect.extfs-3.5.dev4/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:57.423714 dissect.extfs-3.5.dev4/dissect/extfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/dissect/extfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23393 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/dissect/extfs/c_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/dissect/extfs/c_jdb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/dissect/extfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/dissect/extfs/extfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/dissect/extfs/journal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:57.419714 dissect.extfs-3.5.dev4/dissect.extfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-16 13:25:57.000000 dissect.extfs-3.5.dev4/dissect.extfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-16 13:25:57.000000 dissect.extfs-3.5.dev4/dissect.extfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:25:57.000000 dissect.extfs-3.5.dev4/dissect.extfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:25:57.000000 dissect.extfs-3.5.dev4/dissect.extfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:25:57.000000 dissect.extfs-3.5.dev4/dissect.extfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-16 13:25:48.000000 dissect.extfs-3.5.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:25:57.427714 dissect.extfs-3.5.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:57.423714 dissect.extfs-3.5.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:57.427714 dissect.extfs-3.5.dev4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/data/ext4.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/data/ext4_sparse.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/data/ext4_symlink_test1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/data/ext4_symlink_test2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/data/ext4_symlink_test3.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:57.427714 dissect.extfs-3.5.dev4/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tests/test_ext4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:25:44.000000 dissect.extfs-3.5.dev4/tox.ini
```

### Comparing `dissect.extfs-3.5.dev3/LICENSE` & `dissect.extfs-3.5.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev3/PKG-INFO` & `dissect.extfs-3.5.dev4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.extfs
-Version: 3.5.dev3
+Version: 3.5.dev4
 Summary: A Dissect module implementing a parser for the ExtFS file system, the native filesystem for Linux operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.extfs
 Project-URL: repository, https://github.com/fox-it/dissect.extfs
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,20 @@
 License-File: COPYRIGHT
 
 # dissect.extfs
 
 A Dissect module implementing a parser for the ExtFS file system, the native filesystem for Linux operating systems. For
 more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.extfs/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.extfs` is available on [PyPI](https://pypi.org/project/dissect.extfs/).
 
 ```bash
 pip install dissect.extfs
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

### Comparing `dissect.extfs-3.5.dev3/README.md` & `dissect.extfs-3.5.dev4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # dissect.extfs
 
 A Dissect module implementing a parser for the ExtFS file system, the native filesystem for Linux operating systems. For
 more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.extfs/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.extfs` is available on [PyPI](https://pypi.org/project/dissect.extfs/).
 
 ```bash
 pip install dissect.extfs
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

### Comparing `dissect.extfs-3.5.dev3/dissect/extfs/c_ext.py` & `dissect.extfs-3.5.dev4/dissect/extfs/c_ext.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev3/dissect/extfs/c_jdb2.py` & `dissect.extfs-3.5.dev4/dissect/extfs/c_jdb2.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev3/dissect/extfs/extfs.py` & `dissect.extfs-3.5.dev4/dissect/extfs/extfs.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev3/dissect/extfs/journal.py` & `dissect.extfs-3.5.dev4/dissect/extfs/journal.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev3/dissect.extfs.egg-info/PKG-INFO` & `dissect.extfs-3.5.dev4/dissect.extfs.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.extfs
-Version: 3.5.dev3
+Version: 3.5.dev4
 Summary: A Dissect module implementing a parser for the ExtFS file system, the native filesystem for Linux operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.extfs
 Project-URL: repository, https://github.com/fox-it/dissect.extfs
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,20 @@
 License-File: COPYRIGHT
 
 # dissect.extfs
 
 A Dissect module implementing a parser for the ExtFS file system, the native filesystem for Linux operating systems. For
 more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.extfs/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.extfs` is available on [PyPI](https://pypi.org/project/dissect.extfs/).
 
 ```bash
 pip install dissect.extfs
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

### Comparing `dissect.extfs-3.5.dev3/dissect.extfs.egg-info/SOURCES.txt` & `dissect.extfs-3.5.dev4/dissect.extfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev3/pyproject.toml` & `dissect.extfs-3.5.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev3/tests/conftest.py` & `dissect.extfs-3.5.dev4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev3/tests/data/ext4.bin.gz` & `dissect.extfs-3.5.dev4/tests/data/ext4.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev3/tests/data/ext4_sparse.bin.gz` & `dissect.extfs-3.5.dev4/tests/data/ext4_sparse.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev3/tests/data/ext4_symlink_test1.bin.gz` & `dissect.extfs-3.5.dev4/tests/data/ext4_symlink_test1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev3/tests/data/ext4_symlink_test2.bin.gz` & `dissect.extfs-3.5.dev4/tests/data/ext4_symlink_test2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev3/tests/data/ext4_symlink_test3.bin.gz` & `dissect.extfs-3.5.dev4/tests/data/ext4_symlink_test3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev3/tests/docs/Makefile` & `dissect.extfs-3.5.dev4/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev3/tests/docs/conf.py` & `dissect.extfs-3.5.dev4/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev3/tests/test_ext4.py` & `dissect.extfs-3.5.dev4/tests/test_ext4.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev3/tox.ini` & `dissect.extfs-3.5.dev4/tox.ini`

 * *Files identical despite different names*

