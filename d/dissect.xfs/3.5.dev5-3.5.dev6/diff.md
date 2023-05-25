# Comparing `tmp/dissect.xfs-3.5.dev5.tar.gz` & `tmp/dissect.xfs-3.5.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.xfs-3.5.dev5.tar", last modified: Mon May 15 12:48:48 2023, max compression
+gzip compressed data, was "dissect.xfs-3.5.dev6.tar", last modified: Tue May 16 13:27:08 2023, max compression
```

## Comparing `dissect.xfs-3.5.dev5.tar` & `dissect.xfs-3.5.dev6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:48.197005 dissect.xfs-3.5.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-15 12:48:48.193005 dissect.xfs-3.5.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:48.181005 dissect.xfs-3.5.dev5/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:48.189005 dissect.xfs-3.5.dev5/dissect/xfs/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/dissect/xfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41820 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/dissect/xfs/c_xfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/dissect/xfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22085 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/dissect/xfs/xfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:48.185005 dissect.xfs-3.5.dev5/dissect.xfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-15 12:48:48.000000 dissect.xfs-3.5.dev5/dissect.xfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-15 12:48:48.000000 dissect.xfs-3.5.dev5/dissect.xfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:48:48.000000 dissect.xfs-3.5.dev5/dissect.xfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:48:48.000000 dissect.xfs-3.5.dev5/dissect.xfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:48:48.000000 dissect.xfs-3.5.dev5/dissect.xfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-15 12:48:38.000000 dissect.xfs-3.5.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:48:48.197005 dissect.xfs-3.5.dev5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:48.189005 dissect.xfs-3.5.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:48.193005 dissect.xfs-3.5.dev5/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    41799 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/data/xfs.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    42673 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/data/xfs_bigtime.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    45520 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/data/xfs_sparse.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    42284 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/data/xfs_symlink_test1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    42015 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/data/xfs_symlink_test2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    41936 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/data/xfs_symlink_test3.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:48.193005 dissect.xfs-3.5.dev5/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/test_xfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:08.735108 dissect.xfs-3.5.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-16 13:27:08.735108 dissect.xfs-3.5.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:08.731108 dissect.xfs-3.5.dev6/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:08.735108 dissect.xfs-3.5.dev6/dissect/xfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/dissect/xfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41820 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/dissect/xfs/c_xfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/dissect/xfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22085 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/dissect/xfs/xfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:08.731108 dissect.xfs-3.5.dev6/dissect.xfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-16 13:27:08.000000 dissect.xfs-3.5.dev6/dissect.xfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-16 13:27:08.000000 dissect.xfs-3.5.dev6/dissect.xfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:27:08.000000 dissect.xfs-3.5.dev6/dissect.xfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:27:08.000000 dissect.xfs-3.5.dev6/dissect.xfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:27:08.000000 dissect.xfs-3.5.dev6/dissect.xfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 13:26:59.000000 dissect.xfs-3.5.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:27:08.735108 dissect.xfs-3.5.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:08.735108 dissect.xfs-3.5.dev6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:08.735108 dissect.xfs-3.5.dev6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    41799 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/tests/data/xfs.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    42673 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/tests/data/xfs_bigtime.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    45520 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/tests/data/xfs_sparse.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    42284 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/tests/data/xfs_symlink_test1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    42015 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/tests/data/xfs_symlink_test2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    41936 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/tests/data/xfs_symlink_test3.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:08.735108 dissect.xfs-3.5.dev6/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/tests/test_xfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:26:55.000000 dissect.xfs-3.5.dev6/tox.ini
```

### Comparing `dissect.xfs-3.5.dev5/LICENSE` & `dissect.xfs-3.5.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev5/PKG-INFO` & `dissect.xfs-3.5.dev6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.xfs
-Version: 3.5.dev5
+Version: 3.5.dev6
 Summary: A Dissect module implementing a parser for the XFS file system, commonly used by RedHat Linux distributions
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.xfs
 Project-URL: repository, https://github.com/fox-it/dissect.xfs
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,20 @@
 License-File: COPYRIGHT
 
 # dissect.xfs
 
 A Dissect module implementing a parser for the XFS file system, commonly used by RedHat Linux distributions. For more
 information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.xfs/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.xfs` is available on [PyPI](https://pypi.org/project/dissect.xfs/).
 
 ```bash
 pip install dissect.xfs
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

### Comparing `dissect.xfs-3.5.dev5/README.md` & `dissect.xfs-3.5.dev6/dissect.xfs.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,33 @@
+Metadata-Version: 2.1
+Name: dissect.xfs
+Version: 3.5.dev6
+Summary: A Dissect module implementing a parser for the XFS file system, commonly used by RedHat Linux distributions
+Author-email: Dissect Team <dissect@fox-it.com>
+License: Affero General Public License v3
+Project-URL: homepage, https://dissect.tools
+Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.xfs
+Project-URL: repository, https://github.com/fox-it/dissect.xfs
+Classifier: Programming Language :: Python :: 3
+Requires-Python: ~=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: COPYRIGHT
+
 # dissect.xfs
 
 A Dissect module implementing a parser for the XFS file system, commonly used by RedHat Linux distributions. For more
 information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.xfs/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.xfs` is available on [PyPI](https://pypi.org/project/dissect.xfs/).
 
 ```bash
 pip install dissect.xfs
 ```
@@ -28,20 +49,20 @@
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

### Comparing `dissect.xfs-3.5.dev5/dissect/xfs/c_xfs.py` & `dissect.xfs-3.5.dev6/dissect/xfs/c_xfs.py`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev5/dissect/xfs/xfs.py` & `dissect.xfs-3.5.dev6/dissect/xfs/xfs.py`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev5/dissect.xfs.egg-info/PKG-INFO` & `dissect.xfs-3.5.dev6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,18 @@
-Metadata-Version: 2.1
-Name: dissect.xfs
-Version: 3.5.dev5
-Summary: A Dissect module implementing a parser for the XFS file system, commonly used by RedHat Linux distributions
-Author-email: Dissect Team <dissect@fox-it.com>
-License: Affero General Public License v3
-Project-URL: homepage, https://dissect.tools
-Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.xfs
-Project-URL: repository, https://github.com/fox-it/dissect.xfs
-Classifier: Programming Language :: Python :: 3
-Requires-Python: ~=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: COPYRIGHT
-
 # dissect.xfs
 
 A Dissect module implementing a parser for the XFS file system, commonly used by RedHat Linux distributions. For more
 information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.xfs/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.xfs` is available on [PyPI](https://pypi.org/project/dissect.xfs/).
 
 ```bash
 pip install dissect.xfs
 ```
@@ -43,20 +34,20 @@
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

### Comparing `dissect.xfs-3.5.dev5/dissect.xfs.egg-info/SOURCES.txt` & `dissect.xfs-3.5.dev6/dissect.xfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev5/pyproject.toml` & `dissect.xfs-3.5.dev6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev5/tests/data/xfs.bin.gz` & `dissect.xfs-3.5.dev6/tests/data/xfs.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev5/tests/data/xfs_bigtime.bin.gz` & `dissect.xfs-3.5.dev6/tests/data/xfs_bigtime.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev5/tests/data/xfs_sparse.bin.gz` & `dissect.xfs-3.5.dev6/tests/data/xfs_sparse.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev5/tests/data/xfs_symlink_test1.bin.gz` & `dissect.xfs-3.5.dev6/tests/data/xfs_symlink_test1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev5/tests/data/xfs_symlink_test2.bin.gz` & `dissect.xfs-3.5.dev6/tests/data/xfs_symlink_test2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev5/tests/data/xfs_symlink_test3.bin.gz` & `dissect.xfs-3.5.dev6/tests/data/xfs_symlink_test3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev5/tests/docs/Makefile` & `dissect.xfs-3.5.dev6/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev5/tests/docs/conf.py` & `dissect.xfs-3.5.dev6/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev5/tests/test_xfs.py` & `dissect.xfs-3.5.dev6/tests/test_xfs.py`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev5/tox.ini` & `dissect.xfs-3.5.dev6/tox.ini`

 * *Files identical despite different names*

