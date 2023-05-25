# Comparing `tmp/dissect.fat-3.5.dev1.tar.gz` & `tmp/dissect.fat-3.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.fat-3.5.dev1.tar", last modified: Mon May 15 12:47:53 2023, max compression
+gzip compressed data, was "dissect.fat-3.5.dev2.tar", last modified: Tue May 16 13:26:04 2023, max compression
```

## Comparing `dissect.fat-3.5.dev1.tar` & `dissect.fat-3.5.dev2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:53.113127 dissect.fat-3.5.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-15 12:47:53.113127 dissect.fat-3.5.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:53.069126 dissect.fat-3.5.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:53.069126 dissect.fat-3.5.dev1/dissect/fat/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/dissect/fat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/dissect/fat/c_exfat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/dissect/fat/c_fat.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/dissect/fat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/dissect/fat/exfat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/dissect/fat/fat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:53.069126 dissect.fat-3.5.dev1/dissect.fat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-15 12:47:52.000000 dissect.fat-3.5.dev1/dissect.fat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-15 12:47:53.000000 dissect.fat-3.5.dev1/dissect.fat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:47:52.000000 dissect.fat-3.5.dev1/dissect.fat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:47:52.000000 dissect.fat-3.5.dev1/dissect.fat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:47:52.000000 dissect.fat-3.5.dev1/dissect.fat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-15 12:47:43.000000 dissect.fat-3.5.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:47:53.113127 dissect.fat-3.5.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:53.073126 dissect.fat-3.5.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:53.077127 dissect.fat-3.5.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/tests/data/exfat.bin
--rw-r--r--   0 runner    (1001) docker     (123)  1474560 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/tests/data/fat12.bin
--rw-r--r--   0 runner    (1001) docker     (123)  3072000 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/tests/data/fat16.bin
--rw-r--r--   0 runner    (1001) docker     (123) 34304000 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/tests/data/fat32.bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:53.113127 dissect.fat-3.5.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/tests/test_exfat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/tests/test_fat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:47:37.000000 dissect.fat-3.5.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:04.590538 dissect.fat-3.5.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-16 13:26:04.590538 dissect.fat-3.5.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:04.546538 dissect.fat-3.5.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:04.550538 dissect.fat-3.5.dev2/dissect/fat/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/dissect/fat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/dissect/fat/c_exfat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/dissect/fat/c_fat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/dissect/fat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/dissect/fat/exfat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/dissect/fat/fat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:04.546538 dissect.fat-3.5.dev2/dissect.fat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-16 13:26:04.000000 dissect.fat-3.5.dev2/dissect.fat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-16 13:26:04.000000 dissect.fat-3.5.dev2/dissect.fat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:26:04.000000 dissect.fat-3.5.dev2/dissect.fat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:26:04.000000 dissect.fat-3.5.dev2/dissect.fat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:26:04.000000 dissect.fat-3.5.dev2/dissect.fat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-16 13:25:54.000000 dissect.fat-3.5.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:26:04.590538 dissect.fat-3.5.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:04.550538 dissect.fat-3.5.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:04.554538 dissect.fat-3.5.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/data/exfat.bin
+-rw-r--r--   0 runner    (1001) docker     (123)  1474560 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/data/fat12.bin
+-rw-r--r--   0 runner    (1001) docker     (123)  3072000 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/data/fat16.bin
+-rw-r--r--   0 runner    (1001) docker     (123) 34304000 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/data/fat32.bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:04.590538 dissect.fat-3.5.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/test_exfat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tests/test_fat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:25:50.000000 dissect.fat-3.5.dev2/tox.ini
```

### Comparing `dissect.fat-3.5.dev1/LICENSE` & `dissect.fat-3.5.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev1/PKG-INFO` & `dissect.fat-3.5.dev2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.fat
-Version: 3.5.dev1
+Version: 3.5.dev2
 Summary: A Dissect module implementing parsers for the FAT and exFAT file systems, commonly used on flash memory based storage devices and UEFI partitions
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.fat
 Project-URL: repository, https://github.com/fox-it/dissect.fat
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,20 @@
 
 # dissect.fat
 
 A Dissect module implementing parsers for the FAT and exFAT file systems, commonly used on flash memory based storage
 devices and UEFI partitions. For more information, please see [the
 documentation](https://docs.dissect.tools/en/latest/projects/dissect.fat/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.fat` is available on [PyPI](https://pypi.org/project/dissect.fat/).
 
 ```bash
 pip install dissect.fat
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

### Comparing `dissect.fat-3.5.dev1/README.md` & `dissect.fat-3.5.dev2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # dissect.fat
 
 A Dissect module implementing parsers for the FAT and exFAT file systems, commonly used on flash memory based storage
 devices and UEFI partitions. For more information, please see [the
 documentation](https://docs.dissect.tools/en/latest/projects/dissect.fat/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.fat` is available on [PyPI](https://pypi.org/project/dissect.fat/).
 
 ```bash
 pip install dissect.fat
 ```
@@ -29,20 +35,20 @@
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

### Comparing `dissect.fat-3.5.dev1/dissect/fat/__init__.py` & `dissect.fat-3.5.dev2/dissect/fat/__init__.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev1/dissect/fat/c_exfat.py` & `dissect.fat-3.5.dev2/dissect/fat/c_exfat.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev1/dissect/fat/c_fat.py` & `dissect.fat-3.5.dev2/dissect/fat/c_fat.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev1/dissect/fat/exfat.py` & `dissect.fat-3.5.dev2/dissect/fat/exfat.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev1/dissect/fat/fat.py` & `dissect.fat-3.5.dev2/dissect/fat/fat.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev1/dissect.fat.egg-info/PKG-INFO` & `dissect.fat-3.5.dev2/dissect.fat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.fat
-Version: 3.5.dev1
+Version: 3.5.dev2
 Summary: A Dissect module implementing parsers for the FAT and exFAT file systems, commonly used on flash memory based storage devices and UEFI partitions
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.fat
 Project-URL: repository, https://github.com/fox-it/dissect.fat
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,20 @@
 
 # dissect.fat
 
 A Dissect module implementing parsers for the FAT and exFAT file systems, commonly used on flash memory based storage
 devices and UEFI partitions. For more information, please see [the
 documentation](https://docs.dissect.tools/en/latest/projects/dissect.fat/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.fat` is available on [PyPI](https://pypi.org/project/dissect.fat/).
 
 ```bash
 pip install dissect.fat
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

### Comparing `dissect.fat-3.5.dev1/dissect.fat.egg-info/SOURCES.txt` & `dissect.fat-3.5.dev2/dissect.fat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev1/pyproject.toml` & `dissect.fat-3.5.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev1/tests/conftest.py` & `dissect.fat-3.5.dev2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev1/tests/data/exfat.bin` & `dissect.fat-3.5.dev2/tests/data/exfat.bin`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev1/tests/data/fat12.bin` & `dissect.fat-3.5.dev2/tests/data/fat12.bin`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev1/tests/data/fat16.bin` & `dissect.fat-3.5.dev2/tests/data/fat16.bin`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev1/tests/data/fat32.bin` & `dissect.fat-3.5.dev2/tests/data/fat32.bin`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev1/tests/docs/Makefile` & `dissect.fat-3.5.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev1/tests/docs/conf.py` & `dissect.fat-3.5.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev1/tests/test_exfat.py` & `dissect.fat-3.5.dev2/tests/test_exfat.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev1/tests/test_fat.py` & `dissect.fat-3.5.dev2/tests/test_fat.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.5.dev1/tox.ini` & `dissect.fat-3.5.dev2/tox.ini`

 * *Files identical despite different names*

