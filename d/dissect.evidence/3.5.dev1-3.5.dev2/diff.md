# Comparing `tmp/dissect.evidence-3.5.dev1.tar.gz` & `tmp/dissect.evidence-3.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.evidence-3.5.dev1.tar", last modified: Mon May 15 12:47:45 2023, max compression
+gzip compressed data, was "dissect.evidence-3.5.dev2.tar", last modified: Tue May 16 13:25:55 2023, max compression
```

## Comparing `dissect.evidence-3.5.dev1.tar` & `dissect.evidence-3.5.dev2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:45.019849 dissect.evidence-3.5.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-15 12:47:45.019849 dissect.evidence-3.5.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:44.999848 dissect.evidence-3.5.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:45.007849 dissect.evidence-3.5.dev1/dissect/evidence/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/dissect/evidence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/dissect/evidence/ad1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:45.011849 dissect.evidence-3.5.dev1/dissect/evidence/asdf/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/dissect/evidence/asdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23802 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/dissect/evidence/asdf/asdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/dissect/evidence/asdf/streams.py
--rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/dissect/evidence/ewf.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/dissect/evidence/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:45.011849 dissect.evidence-3.5.dev1/dissect/evidence/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/dissect/evidence/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:45.011849 dissect.evidence-3.5.dev1/dissect/evidence/tools/asdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/dissect/evidence/tools/asdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/dissect/evidence/tools/asdf/dd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/dissect/evidence/tools/asdf/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/dissect/evidence/tools/asdf/repair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/dissect/evidence/tools/asdf/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:45.007849 dissect.evidence-3.5.dev1/dissect.evidence.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-15 12:47:44.000000 dissect.evidence-3.5.dev1/dissect.evidence.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-15 12:47:44.000000 dissect.evidence-3.5.dev1/dissect.evidence.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:47:44.000000 dissect.evidence-3.5.dev1/dissect.evidence.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-15 12:47:44.000000 dissect.evidence-3.5.dev1/dissect.evidence.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:47:44.000000 dissect.evidence-3.5.dev1/dissect.evidence.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:47:44.000000 dissect.evidence-3.5.dev1/dissect.evidence.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-15 12:47:32.000000 dissect.evidence-3.5.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:47:45.019849 dissect.evidence-3.5.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:45.015849 dissect.evidence-3.5.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:45.015849 dissect.evidence-3.5.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/tests/data/ad1_long.ad1
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/tests/data/ad1_test.ad1
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/tests/data/ad1_test_compressed.ad1
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/tests/data/ewf.E01
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:45.019849 dissect.evidence-3.5.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/tests/test_ad1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/tests/test_asdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/tests/test_ewf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:47:25.000000 dissect.evidence-3.5.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:55.678813 dissect.evidence-3.5.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-16 13:25:55.678813 dissect.evidence-3.5.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:55.658812 dissect.evidence-3.5.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:55.666812 dissect.evidence-3.5.dev2/dissect/evidence/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/dissect/evidence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/dissect/evidence/ad1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:55.670812 dissect.evidence-3.5.dev2/dissect/evidence/asdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/dissect/evidence/asdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23802 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/dissect/evidence/asdf/asdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/dissect/evidence/asdf/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/dissect/evidence/ewf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/dissect/evidence/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:55.670812 dissect.evidence-3.5.dev2/dissect/evidence/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/dissect/evidence/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:55.670812 dissect.evidence-3.5.dev2/dissect/evidence/tools/asdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/dissect/evidence/tools/asdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/dissect/evidence/tools/asdf/dd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/dissect/evidence/tools/asdf/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/dissect/evidence/tools/asdf/repair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/dissect/evidence/tools/asdf/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:55.666812 dissect.evidence-3.5.dev2/dissect.evidence.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-16 13:25:55.000000 dissect.evidence-3.5.dev2/dissect.evidence.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-16 13:25:55.000000 dissect.evidence-3.5.dev2/dissect.evidence.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:25:55.000000 dissect.evidence-3.5.dev2/dissect.evidence.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-16 13:25:55.000000 dissect.evidence-3.5.dev2/dissect.evidence.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:25:55.000000 dissect.evidence-3.5.dev2/dissect.evidence.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:25:55.000000 dissect.evidence-3.5.dev2/dissect.evidence.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-16 13:25:45.000000 dissect.evidence-3.5.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:25:55.678813 dissect.evidence-3.5.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:55.674812 dissect.evidence-3.5.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:55.674812 dissect.evidence-3.5.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/tests/data/ad1_long.ad1
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/tests/data/ad1_test.ad1
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/tests/data/ad1_test_compressed.ad1
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/tests/data/ewf.E01
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:55.678813 dissect.evidence-3.5.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/tests/test_ad1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/tests/test_asdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/tests/test_ewf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:25:37.000000 dissect.evidence-3.5.dev2/tox.ini
```

### Comparing `dissect.evidence-3.5.dev1/LICENSE` & `dissect.evidence-3.5.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/PKG-INFO` & `dissect.evidence-3.5.dev2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.evidence
-Version: 3.5.dev1
+Version: 3.5.dev2
 Summary: A Dissect module implementing a parsers for various forensic evidence file containers, currently: AD1, ASDF and EWF
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.evidence
 Project-URL: repository, https://github.com/fox-it/dissect.evidence
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,20 @@
 License-File: COPYRIGHT
 
 # dissect.evidence
 
 A Dissect module implementing a parsers for various forensic evidence file containers, currently: AD1, ASDF and EWF. For
 more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.evidence/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.evidence` is available on [PyPI](https://pypi.org/project/dissect.evidence/).
 
 ```bash
 pip install dissect.evidence
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

### Comparing `dissect.evidence-3.5.dev1/README.md` & `dissect.evidence-3.5.dev2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # dissect.evidence
 
 A Dissect module implementing a parsers for various forensic evidence file containers, currently: AD1, ASDF and EWF. For
 more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.evidence/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.evidence` is available on [PyPI](https://pypi.org/project/dissect.evidence/).
 
 ```bash
 pip install dissect.evidence
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

### Comparing `dissect.evidence-3.5.dev1/dissect/evidence/ad1.py` & `dissect.evidence-3.5.dev2/dissect/evidence/ad1.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/dissect/evidence/asdf/asdf.py` & `dissect.evidence-3.5.dev2/dissect/evidence/asdf/asdf.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/dissect/evidence/asdf/streams.py` & `dissect.evidence-3.5.dev2/dissect/evidence/asdf/streams.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/dissect/evidence/ewf.py` & `dissect.evidence-3.5.dev2/dissect/evidence/ewf.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/dissect/evidence/exceptions.py` & `dissect.evidence-3.5.dev2/dissect/evidence/exceptions.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/dissect/evidence/tools/asdf/dd.py` & `dissect.evidence-3.5.dev2/dissect/evidence/tools/asdf/dd.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/dissect/evidence/tools/asdf/meta.py` & `dissect.evidence-3.5.dev2/dissect/evidence/tools/asdf/meta.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/dissect/evidence/tools/asdf/repair.py` & `dissect.evidence-3.5.dev2/dissect/evidence/tools/asdf/repair.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/dissect/evidence/tools/asdf/verify.py` & `dissect.evidence-3.5.dev2/dissect/evidence/tools/asdf/verify.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/dissect.evidence.egg-info/PKG-INFO` & `dissect.evidence-3.5.dev2/dissect.evidence.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.evidence
-Version: 3.5.dev1
+Version: 3.5.dev2
 Summary: A Dissect module implementing a parsers for various forensic evidence file containers, currently: AD1, ASDF and EWF
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.evidence
 Project-URL: repository, https://github.com/fox-it/dissect.evidence
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,20 @@
 License-File: COPYRIGHT
 
 # dissect.evidence
 
 A Dissect module implementing a parsers for various forensic evidence file containers, currently: AD1, ASDF and EWF. For
 more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.evidence/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.evidence` is available on [PyPI](https://pypi.org/project/dissect.evidence/).
 
 ```bash
 pip install dissect.evidence
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

### Comparing `dissect.evidence-3.5.dev1/dissect.evidence.egg-info/SOURCES.txt` & `dissect.evidence-3.5.dev2/dissect.evidence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/pyproject.toml` & `dissect.evidence-3.5.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/tests/conftest.py` & `dissect.evidence-3.5.dev2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/tests/data/ad1_long.ad1` & `dissect.evidence-3.5.dev2/tests/data/ad1_long.ad1`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/tests/data/ad1_test.ad1` & `dissect.evidence-3.5.dev2/tests/data/ad1_test.ad1`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/tests/data/ad1_test_compressed.ad1` & `dissect.evidence-3.5.dev2/tests/data/ad1_test_compressed.ad1`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/tests/data/ewf.E01` & `dissect.evidence-3.5.dev2/tests/data/ewf.E01`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/tests/docs/Makefile` & `dissect.evidence-3.5.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/tests/docs/conf.py` & `dissect.evidence-3.5.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/tests/test_ad1.py` & `dissect.evidence-3.5.dev2/tests/test_ad1.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/tests/test_asdf.py` & `dissect.evidence-3.5.dev2/tests/test_asdf.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.5.dev1/tox.ini` & `dissect.evidence-3.5.dev2/tox.ini`

 * *Files identical despite different names*

