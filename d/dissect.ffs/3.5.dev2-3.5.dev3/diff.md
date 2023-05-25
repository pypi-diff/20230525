# Comparing `tmp/dissect.ffs-3.5.dev2.tar.gz` & `tmp/dissect.ffs-3.5.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.ffs-3.5.dev2.tar", last modified: Mon May 15 12:47:56 2023, max compression
+gzip compressed data, was "dissect.ffs-3.5.dev3.tar", last modified: Tue May 16 13:26:09 2023, max compression
```

## Comparing `dissect.ffs-3.5.dev2.tar` & `dissect.ffs-3.5.dev3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:56.674564 dissect.ffs-3.5.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-15 12:47:56.674564 dissect.ffs-3.5.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:56.666564 dissect.ffs-3.5.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:56.670564 dissect.ffs-3.5.dev2/dissect/ffs/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/dissect/ffs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24537 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/dissect/ffs/c_ffs.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/dissect/ffs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/dissect/ffs/ffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:56.670564 dissect.ffs-3.5.dev2/dissect.ffs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-15 12:47:56.000000 dissect.ffs-3.5.dev2/dissect.ffs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-15 12:47:56.000000 dissect.ffs-3.5.dev2/dissect.ffs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:47:56.000000 dissect.ffs-3.5.dev2/dissect.ffs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:47:56.000000 dissect.ffs-3.5.dev2/dissect.ffs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:47:56.000000 dissect.ffs-3.5.dev2/dissect.ffs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-15 12:47:46.000000 dissect.ffs-3.5.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:47:56.674564 dissect.ffs-3.5.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:56.670564 dissect.ffs-3.5.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:56.674564 dissect.ffs-3.5.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/data/ffs.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/data/ffs_symlink_test1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    16084 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/data/ffs_symlink_test2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/data/ffs_symlink_test3.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:56.674564 dissect.ffs-3.5.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/test_ffs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:09.096281 dissect.ffs-3.5.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-16 13:26:09.096281 dissect.ffs-3.5.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:09.088281 dissect.ffs-3.5.dev3/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:09.092281 dissect.ffs-3.5.dev3/dissect/ffs/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/dissect/ffs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24537 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/dissect/ffs/c_ffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/dissect/ffs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/dissect/ffs/ffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:09.092281 dissect.ffs-3.5.dev3/dissect.ffs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-16 13:26:09.000000 dissect.ffs-3.5.dev3/dissect.ffs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-16 13:26:09.000000 dissect.ffs-3.5.dev3/dissect.ffs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:26:09.000000 dissect.ffs-3.5.dev3/dissect.ffs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:26:09.000000 dissect.ffs-3.5.dev3/dissect.ffs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:26:09.000000 dissect.ffs-3.5.dev3/dissect.ffs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-16 13:25:59.000000 dissect.ffs-3.5.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:26:09.096281 dissect.ffs-3.5.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:09.096281 dissect.ffs-3.5.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:09.096281 dissect.ffs-3.5.dev3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/data/ffs.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/data/ffs_symlink_test1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    16084 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/data/ffs_symlink_test2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/data/ffs_symlink_test3.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:09.096281 dissect.ffs-3.5.dev3/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tests/test_ffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:25:55.000000 dissect.ffs-3.5.dev3/tox.ini
```

### Comparing `dissect.ffs-3.5.dev2/LICENSE` & `dissect.ffs-3.5.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev2/PKG-INFO` & `dissect.ffs-3.5.dev3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ffs
-Version: 3.5.dev2
+Version: 3.5.dev3
 Summary: A Dissect module implementing a parser for the FFS file system, commonly used by BSD operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ffs
 Project-URL: repository, https://github.com/fox-it/dissect.ffs
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,20 @@
 License-File: COPYRIGHT
 
 # dissect.ffs
 
 A Dissect module implementing a parser for the FFS file system, commonly used by BSD operating systems. For more
 information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.ffs/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.ffs` is available on [PyPI](https://pypi.org/project/dissect.ffs/).
 
 ```bash
 pip install dissect.ffs
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

### Comparing `dissect.ffs-3.5.dev2/README.md` & `dissect.ffs-3.5.dev3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # dissect.ffs
 
 A Dissect module implementing a parser for the FFS file system, commonly used by BSD operating systems. For more
 information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.ffs/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.ffs` is available on [PyPI](https://pypi.org/project/dissect.ffs/).
 
 ```bash
 pip install dissect.ffs
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

### Comparing `dissect.ffs-3.5.dev2/dissect/ffs/c_ffs.py` & `dissect.ffs-3.5.dev3/dissect/ffs/c_ffs.py`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev2/dissect/ffs/ffs.py` & `dissect.ffs-3.5.dev3/dissect/ffs/ffs.py`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev2/dissect.ffs.egg-info/PKG-INFO` & `dissect.ffs-3.5.dev3/dissect.ffs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ffs
-Version: 3.5.dev2
+Version: 3.5.dev3
 Summary: A Dissect module implementing a parser for the FFS file system, commonly used by BSD operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ffs
 Project-URL: repository, https://github.com/fox-it/dissect.ffs
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,20 @@
 License-File: COPYRIGHT
 
 # dissect.ffs
 
 A Dissect module implementing a parser for the FFS file system, commonly used by BSD operating systems. For more
 information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.ffs/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.ffs` is available on [PyPI](https://pypi.org/project/dissect.ffs/).
 
 ```bash
 pip install dissect.ffs
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

### Comparing `dissect.ffs-3.5.dev2/dissect.ffs.egg-info/SOURCES.txt` & `dissect.ffs-3.5.dev3/dissect.ffs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev2/pyproject.toml` & `dissect.ffs-3.5.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev2/tests/data/ffs.bin.gz` & `dissect.ffs-3.5.dev3/tests/data/ffs.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev2/tests/data/ffs_symlink_test1.bin.gz` & `dissect.ffs-3.5.dev3/tests/data/ffs_symlink_test1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev2/tests/data/ffs_symlink_test2.bin.gz` & `dissect.ffs-3.5.dev3/tests/data/ffs_symlink_test2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev2/tests/data/ffs_symlink_test3.bin.gz` & `dissect.ffs-3.5.dev3/tests/data/ffs_symlink_test3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev2/tests/docs/Makefile` & `dissect.ffs-3.5.dev3/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev2/tests/docs/conf.py` & `dissect.ffs-3.5.dev3/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev2/tests/test_ffs.py` & `dissect.ffs-3.5.dev3/tests/test_ffs.py`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev2/tox.ini` & `dissect.ffs-3.5.dev3/tox.ini`

 * *Files identical despite different names*

