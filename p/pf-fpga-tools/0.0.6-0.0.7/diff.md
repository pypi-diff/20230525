# Comparing `tmp/pf_fpga_tools-0.0.6.tar.gz` & `tmp/pf_fpga_tools-0.0.7.tar.gz`

## Comparing `pf_fpga_tools-0.0.6.tar` & `pf_fpga_tools-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/.flake8
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/__about__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/__init__.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/exceptions.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/utils.py
--rwxr-xr-x   0        0        0      916 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfBuildCore/__main__.py
--rw-r--r--   0        0        0    14626 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfBuildCore/pfBuildCore.py
--rwxr-xr-x   0        0        0      940 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfCloneCoreTemplate/__main__.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfCloneCoreTemplate/pfCloneCoreTemplate.py
--rwxr-xr-x   0        0        0      925 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfConvertImage/__main__.py
--rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfConvertImage/pfConvertImage.py
--rwxr-xr-x   0        0        0      922 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfInstallCore/__main__.py
--rw-r--r--   0        0        0     7369 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfInstallCore/pfInstallCore.py
--rwxr-xr-x   0        0        0      922 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfQuartusEdit/__main__.py
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfQuartusEdit/pfQuartusEdit.py
--rwxr-xr-x   0        0        0      937 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfReverseBitstream/__main__.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfReverseBitstream/pfReverseBitstream.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/LICENSE
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/README.md
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/.flake8
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/pfFPGATools/__about__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/pfFPGATools/__init__.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/pfFPGATools/exceptions.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/pfFPGATools/utils.py
+-rwxr-xr-x   0        0        0      916 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/pfFPGATools/pfBuildCore/__main__.py
+-rw-r--r--   0        0        0    14626 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/pfFPGATools/pfBuildCore/pfBuildCore.py
+-rwxr-xr-x   0        0        0      940 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/pfFPGATools/pfCloneCoreTemplate/__main__.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/pfFPGATools/pfCloneCoreTemplate/pfCloneCoreTemplate.py
+-rwxr-xr-x   0        0        0      925 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/pfFPGATools/pfConvertImage/__main__.py
+-rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/pfFPGATools/pfConvertImage/pfConvertImage.py
+-rwxr-xr-x   0        0        0      922 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/pfFPGATools/pfInstallCore/__main__.py
+-rw-r--r--   0        0        0     7369 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/pfFPGATools/pfInstallCore/pfInstallCore.py
+-rwxr-xr-x   0        0        0      922 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/pfFPGATools/pfQuartusEdit/__main__.py
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/pfFPGATools/pfQuartusEdit/pfQuartusEdit.py
+-rwxr-xr-x   0        0        0      937 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/pfFPGATools/pfReverseBitstream/__main__.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/pfFPGATools/pfReverseBitstream/pfReverseBitstream.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/README.md
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.7/PKG-INFO
```

### Comparing `pf_fpga_tools-0.0.6/pfFPGATools/utils.py` & `pf_fpga_tools-0.0.7/pfFPGATools/utils.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.6/pfFPGATools/pfBuildCore/__main__.py` & `pf_fpga_tools-0.0.7/pfFPGATools/pfBuildCore/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.6/pfFPGATools/pfBuildCore/pfBuildCore.py` & `pf_fpga_tools-0.0.7/pfFPGATools/pfBuildCore/pfBuildCore.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.6/pfFPGATools/pfCloneCoreTemplate/__main__.py` & `pf_fpga_tools-0.0.7/pfFPGATools/pfCloneCoreTemplate/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.6/pfFPGATools/pfCloneCoreTemplate/pfCloneCoreTemplate.py` & `pf_fpga_tools-0.0.7/pfFPGATools/pfCloneCoreTemplate/pfCloneCoreTemplate.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.6/pfFPGATools/pfConvertImage/__main__.py` & `pf_fpga_tools-0.0.7/pfFPGATools/pfConvertImage/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.6/pfFPGATools/pfConvertImage/pfConvertImage.py` & `pf_fpga_tools-0.0.7/pfFPGATools/pfConvertImage/pfConvertImage.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.6/pfFPGATools/pfInstallCore/__main__.py` & `pf_fpga_tools-0.0.7/pfFPGATools/pfInstallCore/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.6/pfFPGATools/pfInstallCore/pfInstallCore.py` & `pf_fpga_tools-0.0.7/pfFPGATools/pfInstallCore/pfInstallCore.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.6/pfFPGATools/pfQuartusEdit/__main__.py` & `pf_fpga_tools-0.0.7/pfFPGATools/pfQuartusEdit/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.6/pfFPGATools/pfQuartusEdit/pfQuartusEdit.py` & `pf_fpga_tools-0.0.7/pfFPGATools/pfQuartusEdit/pfQuartusEdit.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.6/pfFPGATools/pfReverseBitstream/__main__.py` & `pf_fpga_tools-0.0.7/pfFPGATools/pfReverseBitstream/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.6/pfFPGATools/pfReverseBitstream/pfReverseBitstream.py` & `pf_fpga_tools-0.0.7/pfFPGATools/pfReverseBitstream/pfReverseBitstream.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.6/LICENSE` & `pf_fpga_tools-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.6/README.md` & `pf_fpga_tools-0.0.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # pfFPGATools
 
-[![GPL-v3.0](https://img.shields.io/github/license/DidierMalenfant/pfFPGATools)](https://spdx.org/licenses/GPL-3.0-or-later.html) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pfFPGATools.svg)](https://python.org) [![PyPI - Version](https://img.shields.io/pypi/v/pfFPGATools.svg)](https://pypi.org/project/pfFPGATools)
+[![GPL-v3.0](https://img.shields.io/github/license/DidierMalenfant/pfFPGATools)](https://spdx.org/licenses/GPL-3.0-or-later.html) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pf-fpga-tools.svg)](https://python.org) [![PyPI - Version](https://img.shields.io/pypi/v/pf-fpga-tools.svg)](https://pypi.org/project/pf-fpga-tools)
 
 A set of tools for building and installing [**openFPGA**](https://www.analogue.co/developer) cores for the [**Analog Pocket**](https://www.analogue.co/pocket).
 
 Copyright (c) 2023-present Didier Malenfant.
 
-openFPGA is a registered trademark of [**Analogue**](https://analogue.co).
-
 -----
 
 ### Installation
 
 **pfFPGATools** requires at least [Python](https://python.org) 3.10. Make sure you have a [supported version](http://didier.malenfant.net/blog/nerdy/2022/08/17/installing-python.html) of **Python** before proceeding.
 
 You can then install **pfFPGATools** by typing the following in a terminal window:
@@ -47,10 +45,17 @@
 
 - `pfCloneCoreTemplate` - Clone the core dev template from Github.
 
 - `pfQuartusEdit` - Edit Quartus project files.
 
 You can use the `--help` argument to get some usage info for each command.
 
+### Trademarks
+
+**openFPGA** and the **openFPGA** logo are trademarks of [**Analogue**](https://www.analogue.co/) Enterprises Ltd.
+**Quartus** is a registered trademark of [**Intel**](https://intel.com/).
+
+This project is not affiliated, associated with, sponsored or supported by neither **Analogue** nor **Intel**.
+
 ### License
 
 **pfFPGATools** is distributed under the terms of the [GPLv3.0](https://spdx.org/licenses/GPL-3.0-or-later.html) or later license.
```

### Comparing `pf_fpga_tools-0.0.6/pyproject.toml` & `pf_fpga_tools-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.6/PKG-INFO` & `pf_fpga_tools-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pf-fpga-tools
-Version: 0.0.6
+Version: 0.0.7
 Summary: A collection of tools for openFPGA projects
 Project-URL: Homepage, https://didier.malenfant.net/ProjectFreedom/
 Project-URL: Documentation, https://github.com/DidierMalenfant/pfFPGATools#readme
 Project-URL: Bug Tracker, https://github.com/DidierMalenfant/pfFPGATools/issues
 Project-URL: Source Code, https://github.com/DidierMalenfant/pfFPGATools
 Author-email: Didier Malenfant <coding@malenfant.net>
 License-Expression: GPL-3.0-or-later
@@ -18,22 +18,20 @@
 Requires-Python: >=3.10
 Requires-Dist: pillow
 Requires-Dist: tomli>=1.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # pfFPGATools
 
-[![GPL-v3.0](https://img.shields.io/github/license/DidierMalenfant/pfFPGATools)](https://spdx.org/licenses/GPL-3.0-or-later.html) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pfFPGATools.svg)](https://python.org) [![PyPI - Version](https://img.shields.io/pypi/v/pfFPGATools.svg)](https://pypi.org/project/pfFPGATools)
+[![GPL-v3.0](https://img.shields.io/github/license/DidierMalenfant/pfFPGATools)](https://spdx.org/licenses/GPL-3.0-or-later.html) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pf-fpga-tools.svg)](https://python.org) [![PyPI - Version](https://img.shields.io/pypi/v/pf-fpga-tools.svg)](https://pypi.org/project/pf-fpga-tools)
 
 A set of tools for building and installing [**openFPGA**](https://www.analogue.co/developer) cores for the [**Analog Pocket**](https://www.analogue.co/pocket).
 
 Copyright (c) 2023-present Didier Malenfant.
 
-openFPGA is a registered trademark of [**Analogue**](https://analogue.co).
-
 -----
 
 ### Installation
 
 **pfFPGATools** requires at least [Python](https://python.org) 3.10. Make sure you have a [supported version](http://didier.malenfant.net/blog/nerdy/2022/08/17/installing-python.html) of **Python** before proceeding.
 
 You can then install **pfFPGATools** by typing the following in a terminal window:
@@ -69,10 +67,17 @@
 
 - `pfCloneCoreTemplate` - Clone the core dev template from Github.
 
 - `pfQuartusEdit` - Edit Quartus project files.
 
 You can use the `--help` argument to get some usage info for each command.
 
+### Trademarks
+
+**openFPGA** and the **openFPGA** logo are trademarks of [**Analogue**](https://www.analogue.co/) Enterprises Ltd.
+**Quartus** is a registered trademark of [**Intel**](https://intel.com/).
+
+This project is not affiliated, associated with, sponsored or supported by neither **Analogue** nor **Intel**.
+
 ### License
 
 **pfFPGATools** is distributed under the terms of the [GPLv3.0](https://spdx.org/licenses/GPL-3.0-or-later.html) or later license.
```

