# Comparing `tmp/dissect.vmfs-3.5.dev1.tar.gz` & `tmp/dissect.vmfs-3.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.vmfs-3.5.dev1.tar", last modified: Mon May 15 12:48:39 2023, max compression
+gzip compressed data, was "dissect.vmfs-3.5.dev2.tar", last modified: Tue May 16 13:27:05 2023, max compression
```

## Comparing `dissect.vmfs-3.5.dev1.tar` & `dissect.vmfs-3.5.dev2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:39.453759 dissect.vmfs-3.5.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-15 12:48:39.453759 dissect.vmfs-3.5.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:39.445759 dissect.vmfs-3.5.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:39.449759 dissect.vmfs-3.5.dev1/dissect/vmfs/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/dissect/vmfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/dissect/vmfs/c_vmfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/dissect/vmfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/dissect/vmfs/lvm.py
--rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/dissect/vmfs/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    27978 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/dissect/vmfs/vmfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:39.445759 dissect.vmfs-3.5.dev1/dissect.vmfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-15 12:48:39.000000 dissect.vmfs-3.5.dev1/dissect.vmfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-15 12:48:39.000000 dissect.vmfs-3.5.dev1/dissect.vmfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:48:39.000000 dissect.vmfs-3.5.dev1/dissect.vmfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:48:39.000000 dissect.vmfs-3.5.dev1/dissect.vmfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:48:39.000000 dissect.vmfs-3.5.dev1/dissect.vmfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-15 12:48:29.000000 dissect.vmfs-3.5.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:48:39.453759 dissect.vmfs-3.5.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:39.449759 dissect.vmfs-3.5.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:39.449759 dissect.vmfs-3.5.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   531458 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/data/vmfs5.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1054739 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/data/vmfs6.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:39.453759 dissect.vmfs-3.5.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/test_address.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/test_lvm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/test_vmfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:05.833086 dissect.vmfs-3.5.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-16 13:27:05.833086 dissect.vmfs-3.5.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:05.825086 dissect.vmfs-3.5.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:05.829086 dissect.vmfs-3.5.dev2/dissect/vmfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/dissect/vmfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/dissect/vmfs/c_vmfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/dissect/vmfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/dissect/vmfs/lvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/dissect/vmfs/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27978 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/dissect/vmfs/vmfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:05.829086 dissect.vmfs-3.5.dev2/dissect.vmfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-16 13:27:05.000000 dissect.vmfs-3.5.dev2/dissect.vmfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-16 13:27:05.000000 dissect.vmfs-3.5.dev2/dissect.vmfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:27:05.000000 dissect.vmfs-3.5.dev2/dissect.vmfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:27:05.000000 dissect.vmfs-3.5.dev2/dissect.vmfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:27:05.000000 dissect.vmfs-3.5.dev2/dissect.vmfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 13:26:54.000000 dissect.vmfs-3.5.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:27:05.833086 dissect.vmfs-3.5.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:05.829086 dissect.vmfs-3.5.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:49.000000 dissect.vmfs-3.5.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:05.829086 dissect.vmfs-3.5.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   531458 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/tests/data/vmfs5.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1054739 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/tests/data/vmfs6.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:05.833086 dissect.vmfs-3.5.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/tests/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/tests/test_lvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/tests/test_vmfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:26:48.000000 dissect.vmfs-3.5.dev2/tox.ini
```

### Comparing `dissect.vmfs-3.5.dev1/LICENSE` & `dissect.vmfs-3.5.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.5.dev1/PKG-INFO` & `dissect.vmfs-3.5.dev2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.vmfs
-Version: 3.5.dev1
+Version: 3.5.dev2
 Summary: A Dissect module implementing a parser for the VMFS file system, used by VMware virtualization software
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.vmfs
 Project-URL: repository, https://github.com/fox-it/dissect.vmfs
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,20 @@
 License-File: COPYRIGHT
 
 # dissect.vmfs
 
 A Dissect module implementing a parser for the VMFS file system, used by VMware virtualization software. For more
 information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.vmfs/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.vmfs` is available on [PyPI](https://pypi.org/project/dissect.vmfs/).
 
 ```bash
 pip install dissect.vmfs
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

### Comparing `dissect.vmfs-3.5.dev1/README.md` & `dissect.vmfs-3.5.dev2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # dissect.vmfs
 
 A Dissect module implementing a parser for the VMFS file system, used by VMware virtualization software. For more
 information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.vmfs/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.vmfs` is available on [PyPI](https://pypi.org/project/dissect.vmfs/).
 
 ```bash
 pip install dissect.vmfs
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

### Comparing `dissect.vmfs-3.5.dev1/dissect/vmfs/c_vmfs.py` & `dissect.vmfs-3.5.dev2/dissect/vmfs/c_vmfs.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.5.dev1/dissect/vmfs/lvm.py` & `dissect.vmfs-3.5.dev2/dissect/vmfs/lvm.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.5.dev1/dissect/vmfs/resource.py` & `dissect.vmfs-3.5.dev2/dissect/vmfs/resource.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.5.dev1/dissect/vmfs/vmfs.py` & `dissect.vmfs-3.5.dev2/dissect/vmfs/vmfs.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.5.dev1/dissect.vmfs.egg-info/PKG-INFO` & `dissect.vmfs-3.5.dev2/dissect.vmfs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.vmfs
-Version: 3.5.dev1
+Version: 3.5.dev2
 Summary: A Dissect module implementing a parser for the VMFS file system, used by VMware virtualization software
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.vmfs
 Project-URL: repository, https://github.com/fox-it/dissect.vmfs
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,20 @@
 License-File: COPYRIGHT
 
 # dissect.vmfs
 
 A Dissect module implementing a parser for the VMFS file system, used by VMware virtualization software. For more
 information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.vmfs/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.vmfs` is available on [PyPI](https://pypi.org/project/dissect.vmfs/).
 
 ```bash
 pip install dissect.vmfs
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

### Comparing `dissect.vmfs-3.5.dev1/dissect.vmfs.egg-info/SOURCES.txt` & `dissect.vmfs-3.5.dev2/dissect.vmfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.5.dev1/pyproject.toml` & `dissect.vmfs-3.5.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.5.dev1/tests/data/vmfs5.bin.gz` & `dissect.vmfs-3.5.dev2/tests/data/vmfs5.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.5.dev1/tests/data/vmfs6.bin.gz` & `dissect.vmfs-3.5.dev2/tests/data/vmfs6.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.5.dev1/tests/docs/Makefile` & `dissect.vmfs-3.5.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.5.dev1/tests/docs/conf.py` & `dissect.vmfs-3.5.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.5.dev1/tests/test_address.py` & `dissect.vmfs-3.5.dev2/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.5.dev1/tests/test_lvm.py` & `dissect.vmfs-3.5.dev2/tests/test_lvm.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.5.dev1/tests/test_vmfs.py` & `dissect.vmfs-3.5.dev2/tests/test_vmfs.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.5.dev1/tox.ini` & `dissect.vmfs-3.5.dev2/tox.ini`

 * *Files identical despite different names*

