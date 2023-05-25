# Comparing `tmp/dissect.executable-1.3.dev1.tar.gz` & `tmp/dissect.executable-1.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.executable-1.3.dev1.tar", last modified: Mon May 15 12:47:39 2023, max compression
+gzip compressed data, was "dissect.executable-1.3.dev2.tar", last modified: Tue May 16 13:25:59 2023, max compression
```

## Comparing `dissect.executable-1.3.dev1.tar` & `dissect.executable-1.3.dev2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.952510 dissect.executable-1.3.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-15 12:47:39.952510 dissect.executable-1.3.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.944510 dissect.executable-1.3.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.948510 dissect.executable-1.3.dev1/dissect/executable/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/dissect/executable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.948510 dissect.executable-1.3.dev1/dissect/executable/elf/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/dissect/executable/elf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14842 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/dissect/executable/elf/c_elf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/dissect/executable/elf/elf.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/dissect/executable/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.948510 dissect.executable-1.3.dev1/dissect/executable/macho/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/dissect/executable/macho/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.948510 dissect.executable-1.3.dev1/dissect/executable/pe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/dissect/executable/pe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.948510 dissect.executable-1.3.dev1/dissect.executable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-15 12:47:39.000000 dissect.executable-1.3.dev1/dissect.executable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-15 12:47:39.000000 dissect.executable-1.3.dev1/dissect.executable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:47:39.000000 dissect.executable-1.3.dev1/dissect.executable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:47:39.000000 dissect.executable-1.3.dev1/dissect.executable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:47:39.000000 dissect.executable-1.3.dev1/dissect.executable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-15 12:47:30.000000 dissect.executable-1.3.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:47:39.952510 dissect.executable-1.3.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.948510 dissect.executable-1.3.dev1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.948510 dissect.executable-1.3.dev1/tests/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)    16608 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/data/hello_world.out
--rwxr-xr-x   0 runner    (1001) docker     (123)    14416 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/data/hello_world.stripped.out
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.948510 dissect.executable-1.3.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/test_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/test_elf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/test_section.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/test_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/test_segment_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:59.267598 dissect.executable-1.3.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-16 13:25:59.267598 dissect.executable-1.3.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:59.247598 dissect.executable-1.3.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:59.259598 dissect.executable-1.3.dev2/dissect/executable/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/dissect/executable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:59.259598 dissect.executable-1.3.dev2/dissect/executable/elf/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/dissect/executable/elf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14842 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/dissect/executable/elf/c_elf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/dissect/executable/elf/elf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/dissect/executable/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:59.259598 dissect.executable-1.3.dev2/dissect/executable/macho/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/dissect/executable/macho/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:59.259598 dissect.executable-1.3.dev2/dissect/executable/pe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/dissect/executable/pe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:59.259598 dissect.executable-1.3.dev2/dissect.executable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-16 13:25:59.000000 dissect.executable-1.3.dev2/dissect.executable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-16 13:25:59.000000 dissect.executable-1.3.dev2/dissect.executable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:25:59.000000 dissect.executable-1.3.dev2/dissect.executable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:25:59.000000 dissect.executable-1.3.dev2/dissect.executable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:25:59.000000 dissect.executable-1.3.dev2/dissect.executable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-16 13:25:47.000000 dissect.executable-1.3.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:25:59.267598 dissect.executable-1.3.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:59.263598 dissect.executable-1.3.dev2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:59.263598 dissect.executable-1.3.dev2/tests/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16608 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/tests/data/hello_world.out
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14416 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/tests/data/hello_world.stripped.out
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:59.267598 dissect.executable-1.3.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/tests/test_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/tests/test_elf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/tests/test_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/tests/test_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/tests/test_segment_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:25:41.000000 dissect.executable-1.3.dev2/tox.ini
```

### Comparing `dissect.executable-1.3.dev1/LICENSE` & `dissect.executable-1.3.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.3.dev1/PKG-INFO` & `dissect.executable-1.3.dev2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.executable
-Version: 1.3.dev1
+Version: 1.3.dev2
 Summary: A Dissect module implementing a parsers for various executable formats such as PE, ELF and Macho-O
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.executable
 Project-URL: repository, https://github.com/fox-it/dissect.executable
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,20 @@
 License-File: COPYRIGHT
 
 # dissect.executable
 
 A Dissect module implementing parsers for various executable formats such as PE, ELF and Macho-O. For
 more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.executable/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.executable` is available on [PyPI](https://pypi.org/project/dissect.executable/).
 
 ```bash
 pip install dissect.executable
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

### Comparing `dissect.executable-1.3.dev1/README.md` & `dissect.executable-1.3.dev2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # dissect.executable
 
 A Dissect module implementing parsers for various executable formats such as PE, ELF and Macho-O. For
 more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.executable/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.executable` is available on [PyPI](https://pypi.org/project/dissect.executable/).
 
 ```bash
 pip install dissect.executable
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

### Comparing `dissect.executable-1.3.dev1/dissect/executable/elf/c_elf.py` & `dissect.executable-1.3.dev2/dissect/executable/elf/c_elf.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.3.dev1/dissect/executable/elf/elf.py` & `dissect.executable-1.3.dev2/dissect/executable/elf/elf.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.3.dev1/dissect.executable.egg-info/PKG-INFO` & `dissect.executable-1.3.dev2/dissect.executable.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.executable
-Version: 1.3.dev1
+Version: 1.3.dev2
 Summary: A Dissect module implementing a parsers for various executable formats such as PE, ELF and Macho-O
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.executable
 Project-URL: repository, https://github.com/fox-it/dissect.executable
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,20 @@
 License-File: COPYRIGHT
 
 # dissect.executable
 
 A Dissect module implementing parsers for various executable formats such as PE, ELF and Macho-O. For
 more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.executable/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.executable` is available on [PyPI](https://pypi.org/project/dissect.executable/).
 
 ```bash
 pip install dissect.executable
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

### Comparing `dissect.executable-1.3.dev1/dissect.executable.egg-info/SOURCES.txt` & `dissect.executable-1.3.dev2/dissect.executable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.3.dev1/pyproject.toml` & `dissect.executable-1.3.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.3.dev1/tests/data/hello_world.out` & `dissect.executable-1.3.dev2/tests/data/hello_world.out`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.3.dev1/tests/data/hello_world.stripped.out` & `dissect.executable-1.3.dev2/tests/data/hello_world.stripped.out`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.3.dev1/tests/docs/Makefile` & `dissect.executable-1.3.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.3.dev1/tests/docs/conf.py` & `dissect.executable-1.3.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.3.dev1/tests/test_dump.py` & `dissect.executable-1.3.dev2/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.3.dev1/tests/test_section.py` & `dissect.executable-1.3.dev2/tests/test_section.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.3.dev1/tests/test_segment.py` & `dissect.executable-1.3.dev2/tests/test_segment.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.3.dev1/tests/test_segment_table.py` & `dissect.executable-1.3.dev2/tests/test_segment_table.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.3.dev1/tox.ini` & `dissect.executable-1.3.dev2/tox.ini`

 * *Files identical despite different names*

