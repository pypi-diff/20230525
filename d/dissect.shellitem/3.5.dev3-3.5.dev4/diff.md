# Comparing `tmp/dissect.shellitem-3.5.dev3.tar.gz` & `tmp/dissect.shellitem-3.5.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.shellitem-3.5.dev3.tar", last modified: Mon May 15 12:48:25 2023, max compression
+gzip compressed data, was "dissect.shellitem-3.5.dev4.tar", last modified: Tue May 16 13:26:47 2023, max compression
```

## Comparing `dissect.shellitem-3.5.dev3.tar` & `dissect.shellitem-3.5.dev4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.588348 dissect.shellitem-3.5.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-15 12:48:25.588348 dissect.shellitem-3.5.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.576348 dissect.shellitem-3.5.dev3/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.580348 dissect.shellitem-3.5.dev3/dissect/shellitem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/dissect/shellitem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.580348 dissect.shellitem-3.5.dev3/dissect/shellitem/lnk/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/dissect/shellitem/lnk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39685 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/dissect/shellitem/lnk/c_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)    17611 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/dissect/shellitem/lnk/lnk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.584348 dissect.shellitem-3.5.dev3/dissect/shellitem/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/dissect/shellitem/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/dissect/shellitem/tools/lnk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.580348 dissect.shellitem-3.5.dev3/dissect.shellitem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-15 12:48:25.000000 dissect.shellitem-3.5.dev3/dissect.shellitem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-15 12:48:25.000000 dissect.shellitem-3.5.dev3/dissect.shellitem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:48:25.000000 dissect.shellitem-3.5.dev3/dissect.shellitem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-15 12:48:25.000000 dissect.shellitem-3.5.dev3/dissect.shellitem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:48:25.000000 dissect.shellitem-3.5.dev3/dissect.shellitem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:48:25.000000 dissect.shellitem-3.5.dev3/dissect.shellitem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-15 12:48:13.000000 dissect.shellitem-3.5.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:48:25.588348 dissect.shellitem-3.5.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.584348 dissect.shellitem-3.5.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.588348 dissect.shellitem-3.5.dev3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/data/downloads.win81.lnk
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/data/local.directory.seven.lnk
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/data/modified_remote.file.xp.lnk
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/data/remote.directory.xp.lnk
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/data/remote.file.xp.lnk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.588348 dissect.shellitem-3.5.dev3/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/test_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:47.374049 dissect.shellitem-3.5.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-16 13:26:47.374049 dissect.shellitem-3.5.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:47.358049 dissect.shellitem-3.5.dev4/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:47.366049 dissect.shellitem-3.5.dev4/dissect/shellitem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/dissect/shellitem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:47.366049 dissect.shellitem-3.5.dev4/dissect/shellitem/lnk/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/dissect/shellitem/lnk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39685 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/dissect/shellitem/lnk/c_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17611 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/dissect/shellitem/lnk/lnk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:47.370049 dissect.shellitem-3.5.dev4/dissect/shellitem/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/dissect/shellitem/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/dissect/shellitem/tools/lnk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:47.366049 dissect.shellitem-3.5.dev4/dissect.shellitem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-16 13:26:47.000000 dissect.shellitem-3.5.dev4/dissect.shellitem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-16 13:26:47.000000 dissect.shellitem-3.5.dev4/dissect.shellitem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:26:47.000000 dissect.shellitem-3.5.dev4/dissect.shellitem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 13:26:47.000000 dissect.shellitem-3.5.dev4/dissect.shellitem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:26:47.000000 dissect.shellitem-3.5.dev4/dissect.shellitem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:26:47.000000 dissect.shellitem-3.5.dev4/dissect.shellitem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-16 13:26:35.000000 dissect.shellitem-3.5.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:26:47.374049 dissect.shellitem-3.5.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:47.370049 dissect.shellitem-3.5.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:47.374049 dissect.shellitem-3.5.dev4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/tests/data/downloads.win81.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/tests/data/local.directory.seven.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/tests/data/modified_remote.file.xp.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/tests/data/remote.directory.xp.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/tests/data/remote.file.xp.lnk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:47.374049 dissect.shellitem-3.5.dev4/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/tests/test_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:26:27.000000 dissect.shellitem-3.5.dev4/tox.ini
```

### Comparing `dissect.shellitem-3.5.dev3/LICENSE` & `dissect.shellitem-3.5.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev3/PKG-INFO` & `dissect.shellitem-3.5.dev4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.shellitem
-Version: 3.5.dev3
+Version: 3.5.dev4
 Summary: A Dissect module implementing a parser for the Shellitem structures, commonly used by Microsoft Windows
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.shellitem
 Project-URL: repository, https://github.com/fox-it/dissect.shellitem
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,20 @@
 License-File: COPYRIGHT
 
 # dissect.shellitem
 
 A Dissect module implementing a parser for the Shellitem structures, commonly used by Microsoft Windows. For more
 information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.shellitem/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.shellitem` is available on [PyPI](https://pypi.org/project/dissect.shellitem/).
 
 ```bash
 pip install dissect.shellitem
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

### Comparing `dissect.shellitem-3.5.dev3/README.md` & `dissect.shellitem-3.5.dev4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # dissect.shellitem
 
 A Dissect module implementing a parser for the Shellitem structures, commonly used by Microsoft Windows. For more
 information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.shellitem/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.shellitem` is available on [PyPI](https://pypi.org/project/dissect.shellitem/).
 
 ```bash
 pip install dissect.shellitem
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

### Comparing `dissect.shellitem-3.5.dev3/dissect/shellitem/lnk/c_lnk.py` & `dissect.shellitem-3.5.dev4/dissect/shellitem/lnk/c_lnk.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev3/dissect/shellitem/lnk/lnk.py` & `dissect.shellitem-3.5.dev4/dissect/shellitem/lnk/lnk.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev3/dissect/shellitem/tools/lnk.py` & `dissect.shellitem-3.5.dev4/dissect/shellitem/tools/lnk.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev3/dissect.shellitem.egg-info/PKG-INFO` & `dissect.shellitem-3.5.dev4/dissect.shellitem.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.shellitem
-Version: 3.5.dev3
+Version: 3.5.dev4
 Summary: A Dissect module implementing a parser for the Shellitem structures, commonly used by Microsoft Windows
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.shellitem
 Project-URL: repository, https://github.com/fox-it/dissect.shellitem
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,20 @@
 License-File: COPYRIGHT
 
 # dissect.shellitem
 
 A Dissect module implementing a parser for the Shellitem structures, commonly used by Microsoft Windows. For more
 information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.shellitem/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.shellitem` is available on [PyPI](https://pypi.org/project/dissect.shellitem/).
 
 ```bash
 pip install dissect.shellitem
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

### Comparing `dissect.shellitem-3.5.dev3/dissect.shellitem.egg-info/SOURCES.txt` & `dissect.shellitem-3.5.dev4/dissect.shellitem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev3/pyproject.toml` & `dissect.shellitem-3.5.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev3/tests/conftest.py` & `dissect.shellitem-3.5.dev4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev3/tests/data/downloads.win81.lnk` & `dissect.shellitem-3.5.dev4/tests/data/downloads.win81.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev3/tests/data/local.directory.seven.lnk` & `dissect.shellitem-3.5.dev4/tests/data/local.directory.seven.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev3/tests/data/modified_remote.file.xp.lnk` & `dissect.shellitem-3.5.dev4/tests/data/modified_remote.file.xp.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev3/tests/data/remote.directory.xp.lnk` & `dissect.shellitem-3.5.dev4/tests/data/remote.directory.xp.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev3/tests/data/remote.file.xp.lnk` & `dissect.shellitem-3.5.dev4/tests/data/remote.file.xp.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev3/tests/docs/Makefile` & `dissect.shellitem-3.5.dev4/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev3/tests/docs/conf.py` & `dissect.shellitem-3.5.dev4/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev3/tests/test_lnk.py` & `dissect.shellitem-3.5.dev4/tests/test_lnk.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev3/tox.ini` & `dissect.shellitem-3.5.dev4/tox.ini`

 * *Files identical despite different names*

