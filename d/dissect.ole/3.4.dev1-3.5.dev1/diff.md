# Comparing `tmp/dissect.ole-3.4.dev1.tar.gz` & `tmp/dissect.ole-3.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.ole-3.4.dev1.tar", last modified: Thu Mar 16 13:04:20 2023, max compression
+gzip compressed data, was "dissect.ole-3.5.dev1.tar", last modified: Tue May 16 13:26:30 2023, max compression
```

## Comparing `dissect.ole-3.4.dev1.tar` & `dissect.ole-3.5.dev1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:20.916067 dissect.ole-3.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-16 13:04:05.000000 dissect.ole-3.4.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-16 13:04:05.000000 dissect.ole-3.4.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-16 13:04:05.000000 dissect.ole-3.4.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-03-16 13:04:20.916067 dissect.ole-3.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-16 13:04:05.000000 dissect.ole-3.4.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:20.912067 dissect.ole-3.4.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:20.916067 dissect.ole-3.4.dev1/dissect/ole/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-16 13:04:05.000000 dissect.ole-3.4.dev1/dissect/ole/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-03-16 13:04:05.000000 dissect.ole-3.4.dev1/dissect/ole/c_ole.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-16 13:04:05.000000 dissect.ole-3.4.dev1/dissect/ole/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-03-16 13:04:05.000000 dissect.ole-3.4.dev1/dissect/ole/ole.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:20.916067 dissect.ole-3.4.dev1/dissect.ole.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-03-16 13:04:20.000000 dissect.ole-3.4.dev1/dissect.ole.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-16 13:04:20.000000 dissect.ole-3.4.dev1/dissect.ole.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:04:20.000000 dissect.ole-3.4.dev1/dissect.ole.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-16 13:04:20.000000 dissect.ole-3.4.dev1/dissect.ole.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 13:04:20.000000 dissect.ole-3.4.dev1/dissect.ole.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-16 13:04:09.000000 dissect.ole-3.4.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 13:04:20.916067 dissect.ole-3.4.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-16 13:04:05.000000 dissect.ole-3.4.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:30.698049 dissect.ole-3.5.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 13:26:16.000000 dissect.ole-3.5.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:26:16.000000 dissect.ole-3.5.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:26:16.000000 dissect.ole-3.5.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-16 13:26:30.698049 dissect.ole-3.5.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-16 13:26:16.000000 dissect.ole-3.5.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:30.698049 dissect.ole-3.5.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:30.698049 dissect.ole-3.5.dev1/dissect/ole/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 13:26:16.000000 dissect.ole-3.5.dev1/dissect/ole/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-16 13:26:16.000000 dissect.ole-3.5.dev1/dissect/ole/c_ole.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 13:26:16.000000 dissect.ole-3.5.dev1/dissect/ole/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-05-16 13:26:16.000000 dissect.ole-3.5.dev1/dissect/ole/ole.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:30.698049 dissect.ole-3.5.dev1/dissect.ole.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-16 13:26:30.000000 dissect.ole-3.5.dev1/dissect.ole.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-16 13:26:30.000000 dissect.ole-3.5.dev1/dissect.ole.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:26:30.000000 dissect.ole-3.5.dev1/dissect.ole.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:26:30.000000 dissect.ole-3.5.dev1/dissect.ole.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:26:30.000000 dissect.ole-3.5.dev1/dissect.ole.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-16 13:26:20.000000 dissect.ole-3.5.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:26:30.698049 dissect.ole-3.5.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-16 13:26:16.000000 dissect.ole-3.5.dev1/tox.ini
```

### Comparing `dissect.ole-3.4.dev1/LICENSE` & `dissect.ole-3.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.4.dev1/PKG-INFO` & `dissect.ole-3.5.dev1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ole
-Version: 3.4.dev1
+Version: 3.5.dev1
 Summary: A Dissect module implementing a parser for the Object Linking & Embedding (OLE) format, commonly used by document editors on Windows operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ole
 Project-URL: repository, https://github.com/fox-it/dissect.ole
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,20 @@
 
 # dissect.ole
 
 A Dissect module implementing a parser for the Object Linking & Embedding (OLE) format, commonly used by document
 editors on Windows operating systems. For more information, please see [the
 documentation](https://docs.dissect.tools/en/latest/projects/dissect.ole/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.ole` is available on [PyPI](https://pypi.org/project/dissect.ole/).
 
 ```bash
 pip install dissect.ole
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

### Comparing `dissect.ole-3.4.dev1/README.md` & `dissect.ole-3.5.dev1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # dissect.ole
 
 A Dissect module implementing a parser for the Object Linking & Embedding (OLE) format, commonly used by document
 editors on Windows operating systems. For more information, please see [the
 documentation](https://docs.dissect.tools/en/latest/projects/dissect.ole/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.ole` is available on [PyPI](https://pypi.org/project/dissect.ole/).
 
 ```bash
 pip install dissect.ole
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

### Comparing `dissect.ole-3.4.dev1/dissect/ole/c_ole.py` & `dissect.ole-3.5.dev1/dissect/ole/c_ole.py`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.4.dev1/dissect/ole/ole.py` & `dissect.ole-3.5.dev1/dissect/ole/ole.py`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.4.dev1/dissect.ole.egg-info/PKG-INFO` & `dissect.ole-3.5.dev1/dissect.ole.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ole
-Version: 3.4.dev1
+Version: 3.5.dev1
 Summary: A Dissect module implementing a parser for the Object Linking & Embedding (OLE) format, commonly used by document editors on Windows operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ole
 Project-URL: repository, https://github.com/fox-it/dissect.ole
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,20 @@
 
 # dissect.ole
 
 A Dissect module implementing a parser for the Object Linking & Embedding (OLE) format, commonly used by document
 editors on Windows operating systems. For more information, please see [the
 documentation](https://docs.dissect.tools/en/latest/projects/dissect.ole/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.ole` is available on [PyPI](https://pypi.org/project/dissect.ole/).
 
 ```bash
 pip install dissect.ole
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

### Comparing `dissect.ole-3.4.dev1/pyproject.toml` & `dissect.ole-3.5.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.4.dev1/tox.ini` & `dissect.ole-3.5.dev1/tox.ini`

 * *Files identical despite different names*

