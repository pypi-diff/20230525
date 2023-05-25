# Comparing `tmp/dissect-3.5.dev4.tar.gz` & `tmp/dissect-3.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect-3.5.dev4.tar", last modified: Fri Mar 24 14:56:11 2023, max compression
+gzip compressed data, was "dissect-3.6.dev1.tar", last modified: Tue May 16 13:25:36 2023, max compression
```

## Comparing `dissect-3.5.dev4.tar` & `dissect-3.6.dev1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:56:11.467474 dissect-3.5.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-24 14:55:57.000000 dissect-3.5.dev4/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-24 14:55:57.000000 dissect-3.5.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-24 14:55:57.000000 dissect-3.5.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-03-24 14:56:11.467474 dissect-3.5.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-03-24 14:55:57.000000 dissect-3.5.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:56:11.467474 dissect-3.5.dev4/dissect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-03-24 14:56:11.000000 dissect-3.5.dev4/dissect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-24 14:56:11.000000 dissect-3.5.dev4/dissect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 14:56:11.000000 dissect-3.5.dev4/dissect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-24 14:56:11.000000 dissect-3.5.dev4/dissect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 14:56:11.000000 dissect-3.5.dev4/dissect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-24 14:56:01.000000 dissect-3.5.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 14:56:11.467474 dissect-3.5.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-03-24 14:55:57.000000 dissect-3.5.dev4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:36.714911 dissect-3.6.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-16 13:25:21.000000 dissect-3.6.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:25:21.000000 dissect-3.6.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:25:21.000000 dissect-3.6.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-16 13:25:36.710911 dissect-3.6.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-16 13:25:21.000000 dissect-3.6.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:36.710911 dissect-3.6.dev1/dissect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-16 13:25:36.000000 dissect-3.6.dev1/dissect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-16 13:25:36.000000 dissect-3.6.dev1/dissect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:25:36.000000 dissect-3.6.dev1/dissect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 13:25:36.000000 dissect-3.6.dev1/dissect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:25:36.000000 dissect-3.6.dev1/dissect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-16 13:25:26.000000 dissect-3.6.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:25:36.714911 dissect-3.6.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-16 13:25:21.000000 dissect-3.6.dev1/tox.ini
```

### Comparing `dissect-3.5.dev4/LICENSE` & `dissect-3.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect-3.5.dev4/PKG-INFO` & `dissect-3.6.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect
-Version: 3.5.dev4
+Version: 3.6.dev1
 Summary: Dissect is a digital forensics & incident response framework and toolset that allows you to quickly access and analyse forensic artefacts from various disk and file formats, developed by Fox-IT (part of NCC Group)
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools
 Project-URL: repository, https://github.com/fox-it/dissect
 Classifier: Programming Language :: Python :: 3
@@ -79,14 +79,20 @@
 ### Related
 
 These projects are closely related to Dissect, but not installed by this meta package.
 
 - [acquire](https://github.com/fox-it/acquire)
 - [flow.record](https://github.com/fox-it/flow.record)
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect` is available on [PyPI](https://pypi.org/project/dissect/).
 
 ```bash
 pip install dissect
 ```
@@ -106,20 +112,20 @@
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

### Comparing `dissect-3.5.dev4/README.md` & `dissect-3.6.dev1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,20 @@
 ### Related
 
 These projects are closely related to Dissect, but not installed by this meta package.
 
 - [acquire](https://github.com/fox-it/acquire)
 - [flow.record](https://github.com/fox-it/flow.record)
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect` is available on [PyPI](https://pypi.org/project/dissect/).
 
 ```bash
 pip install dissect
 ```
@@ -91,20 +97,20 @@
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

### Comparing `dissect-3.5.dev4/dissect.egg-info/PKG-INFO` & `dissect-3.6.dev1/dissect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect
-Version: 3.5.dev4
+Version: 3.6.dev1
 Summary: Dissect is a digital forensics & incident response framework and toolset that allows you to quickly access and analyse forensic artefacts from various disk and file formats, developed by Fox-IT (part of NCC Group)
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools
 Project-URL: repository, https://github.com/fox-it/dissect
 Classifier: Programming Language :: Python :: 3
@@ -79,14 +79,20 @@
 ### Related
 
 These projects are closely related to Dissect, but not installed by this meta package.
 
 - [acquire](https://github.com/fox-it/acquire)
 - [flow.record](https://github.com/fox-it/flow.record)
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect` is available on [PyPI](https://pypi.org/project/dissect/).
 
 ```bash
 pip install dissect
 ```
@@ -106,20 +112,20 @@
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

### Comparing `dissect-3.5.dev4/pyproject.toml` & `dissect-3.6.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect-3.5.dev4/tox.ini` & `dissect-3.6.dev1/tox.ini`

 * *Files identical despite different names*

