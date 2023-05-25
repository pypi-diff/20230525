# Comparing `tmp/dissect.clfs-1.5.dev1.tar.gz` & `tmp/dissect.clfs-1.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.clfs-1.5.dev1.tar", last modified: Mon May 15 12:47:17 2023, max compression
+gzip compressed data, was "dissect.clfs-1.5.dev2.tar", last modified: Tue May 16 13:25:30 2023, max compression
```

## Comparing `dissect.clfs-1.5.dev1.tar` & `dissect.clfs-1.5.dev2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:17.511274 dissect.clfs-1.5.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-15 12:47:17.511274 dissect.clfs-1.5.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:17.491273 dissect.clfs-1.5.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:17.503274 dissect.clfs-1.5.dev1/dissect/clfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:01.000000 dissect.clfs-1.5.dev1/dissect/clfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14324 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/dissect/clfs/blf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/dissect/clfs/c_clfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/dissect/clfs/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/dissect/clfs/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:17.499274 dissect.clfs-1.5.dev1/dissect.clfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-15 12:47:17.000000 dissect.clfs-1.5.dev1/dissect.clfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-15 12:47:17.000000 dissect.clfs-1.5.dev1/dissect.clfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:47:17.000000 dissect.clfs-1.5.dev1/dissect.clfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-15 12:47:17.000000 dissect.clfs-1.5.dev1/dissect.clfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:47:17.000000 dissect.clfs-1.5.dev1/dissect.clfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 12:47:07.000000 dissect.clfs-1.5.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:47:17.511274 dissect.clfs-1.5.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:17.503274 dissect.clfs-1.5.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:01.000000 dissect.clfs-1.5.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:17.507274 dissect.clfs-1.5.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    65536 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TM.blf
--rw-r--r--   0 runner    (1001) docker     (123)   524288 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TMContainer00000000000000000001.regtrans-ms
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/data/bad_control_record.blf
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/data/control_record.blf
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/data/invalid_control_record.blf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:17.511274 dissect.clfs-1.5.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/test_control_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/test_record_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/test_validate_blf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:30.681578 dissect.clfs-1.5.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-16 13:25:30.681578 dissect.clfs-1.5.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:30.673578 dissect.clfs-1.5.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:30.677578 dissect.clfs-1.5.dev2/dissect/clfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/dissect/clfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14324 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/dissect/clfs/blf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/dissect/clfs/c_clfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/dissect/clfs/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/dissect/clfs/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:30.673578 dissect.clfs-1.5.dev2/dissect.clfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-16 13:25:30.000000 dissect.clfs-1.5.dev2/dissect.clfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-16 13:25:30.000000 dissect.clfs-1.5.dev2/dissect.clfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:25:30.000000 dissect.clfs-1.5.dev2/dissect.clfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-16 13:25:30.000000 dissect.clfs-1.5.dev2/dissect.clfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:25:30.000000 dissect.clfs-1.5.dev2/dissect.clfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 13:25:20.000000 dissect.clfs-1.5.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:25:30.681578 dissect.clfs-1.5.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:30.677578 dissect.clfs-1.5.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:30.677578 dissect.clfs-1.5.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    65536 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TM.blf
+-rw-r--r--   0 runner    (1001) docker     (123)   524288 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TMContainer00000000000000000001.regtrans-ms
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/tests/data/bad_control_record.blf
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/tests/data/control_record.blf
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/tests/data/invalid_control_record.blf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:30.677578 dissect.clfs-1.5.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/tests/test_control_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/tests/test_record_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/tests/test_validate_blf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:25:16.000000 dissect.clfs-1.5.dev2/tox.ini
```

### Comparing `dissect.clfs-1.5.dev1/LICENSE` & `dissect.clfs-1.5.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.5.dev1/PKG-INFO` & `dissect.clfs-1.5.dev2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.clfs
-Version: 1.5.dev1
+Version: 1.5.dev2
 Summary: A Dissect module implementing a parser for the CLFS (Common Log File System) file system of Windows
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.clfs
 Project-URL: repository, https://github.com/fox-it/dissect.clfs
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,20 @@
 
 # dissect.clfs
 
 A Dissect module implementing a parser for the CLFS (Common Log File System) file system of Windows.
 Currently only supports the persistent variant. For more information,
 please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.clfs/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.clfs` is available on [PyPI](https://pypi.org/project/dissect.clfs/).
 
 ```bash
 pip install dissect.clfs
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

### Comparing `dissect.clfs-1.5.dev1/README.md` & `dissect.clfs-1.5.dev2/dissect.clfs.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,34 @@
+Metadata-Version: 2.1
+Name: dissect.clfs
+Version: 1.5.dev2
+Summary: A Dissect module implementing a parser for the CLFS (Common Log File System) file system of Windows
+Author-email: Dissect Team <dissect@fox-it.com>
+License: Affero General Public License v3
+Project-URL: homepage, https://dissect.tools
+Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.clfs
+Project-URL: repository, https://github.com/fox-it/dissect.clfs
+Classifier: Programming Language :: Python :: 3
+Requires-Python: ~=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: COPYRIGHT
+
 # dissect.clfs
 
 A Dissect module implementing a parser for the CLFS (Common Log File System) file system of Windows.
 Currently only supports the persistent variant. For more information,
 please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.clfs/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.clfs` is available on [PyPI](https://pypi.org/project/dissect.clfs/).
 
 ```bash
 pip install dissect.clfs
 ```
@@ -29,20 +50,20 @@
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

### Comparing `dissect.clfs-1.5.dev1/dissect/clfs/blf.py` & `dissect.clfs-1.5.dev2/dissect/clfs/blf.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.5.dev1/dissect/clfs/c_clfs.py` & `dissect.clfs-1.5.dev2/dissect/clfs/c_clfs.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.5.dev1/dissect/clfs/container.py` & `dissect.clfs-1.5.dev2/dissect/clfs/container.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.5.dev1/dissect.clfs.egg-info/PKG-INFO` & `dissect.clfs-1.5.dev2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,19 @@
-Metadata-Version: 2.1
-Name: dissect.clfs
-Version: 1.5.dev1
-Summary: A Dissect module implementing a parser for the CLFS (Common Log File System) file system of Windows
-Author-email: Dissect Team <dissect@fox-it.com>
-License: Affero General Public License v3
-Project-URL: homepage, https://dissect.tools
-Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.clfs
-Project-URL: repository, https://github.com/fox-it/dissect.clfs
-Classifier: Programming Language :: Python :: 3
-Requires-Python: ~=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: COPYRIGHT
-
 # dissect.clfs
 
 A Dissect module implementing a parser for the CLFS (Common Log File System) file system of Windows.
 Currently only supports the persistent variant. For more information,
 please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.clfs/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.clfs` is available on [PyPI](https://pypi.org/project/dissect.clfs/).
 
 ```bash
 pip install dissect.clfs
 ```
@@ -44,20 +35,20 @@
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

### Comparing `dissect.clfs-1.5.dev1/dissect.clfs.egg-info/SOURCES.txt` & `dissect.clfs-1.5.dev2/dissect.clfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.5.dev1/pyproject.toml` & `dissect.clfs-1.5.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.5.dev1/tests/conftest.py` & `dissect.clfs-1.5.dev2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.5.dev1/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TM.blf` & `dissect.clfs-1.5.dev2/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TM.blf`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.5.dev1/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TMContainer00000000000000000001.regtrans-ms` & `dissect.clfs-1.5.dev2/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TMContainer00000000000000000001.regtrans-ms`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.5.dev1/tests/data/bad_control_record.blf` & `dissect.clfs-1.5.dev2/tests/data/bad_control_record.blf`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.5.dev1/tests/data/control_record.blf` & `dissect.clfs-1.5.dev2/tests/data/control_record.blf`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.5.dev1/tests/data/invalid_control_record.blf` & `dissect.clfs-1.5.dev2/tests/data/invalid_control_record.blf`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.5.dev1/tests/docs/Makefile` & `dissect.clfs-1.5.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.5.dev1/tests/docs/conf.py` & `dissect.clfs-1.5.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.5.dev1/tests/test_container.py` & `dissect.clfs-1.5.dev2/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.5.dev1/tests/test_control_record.py` & `dissect.clfs-1.5.dev2/tests/test_control_record.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.5.dev1/tests/test_record_header.py` & `dissect.clfs-1.5.dev2/tests/test_record_header.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.5.dev1/tox.ini` & `dissect.clfs-1.5.dev2/tox.ini`

 * *Files identical despite different names*

