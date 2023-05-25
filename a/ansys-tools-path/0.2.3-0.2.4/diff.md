# Comparing `tmp/ansys-tools-path-0.2.3.tar.gz` & `tmp/ansys_tools_path-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-tools-path-0.2.3.tar", last modified: Fri May 12 17:12:54 2023, max compression
+gzip compressed data, was "ansys_tools_path-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys-tools-path-0.2.3.tar` & `ansys_tools_path-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1089 2023-05-12 17:12:39.846011 ansys-tools-path-0.2.3/LICENSE
--rw-r--r--   0        0        0     4701 2023-05-12 17:12:39.846011 ansys-tools-path-0.2.3/README.rst
--rw-r--r--   0        0        0     1849 2023-05-12 17:12:39.850011 ansys-tools-path-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      919 2023-05-12 17:12:39.850011 ansys-tools-path-0.2.3/src/ansys/tools/path/__init__.py
--rw-r--r--   0        0        0      648 2023-05-12 17:12:39.850011 ansys-tools-path-0.2.3/src/ansys/tools/path/misc.py
--rw-r--r--   0        0        0    26017 2023-05-12 17:12:39.850011 ansys-tools-path-0.2.3/src/ansys/tools/path/path.py
--rw-r--r--   0        0        0     6192 1970-01-01 00:00:00.000000 ansys-tools-path-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-25 07:10:14.342738 ansys_tools_path-0.2.4/LICENSE
+-rw-r--r--   0        0        0     4691 2023-05-25 07:10:14.342738 ansys_tools_path-0.2.4/README.rst
+-rw-r--r--   0        0        0     1843 2023-05-25 07:10:14.342738 ansys_tools_path-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      919 2023-05-25 07:10:14.342738 ansys_tools_path-0.2.4/src/ansys/tools/path/__init__.py
+-rw-r--r--   0        0        0      648 2023-05-25 07:10:14.342738 ansys_tools_path-0.2.4/src/ansys/tools/path/misc.py
+-rw-r--r--   0        0        0    26062 2023-05-25 07:10:14.342738 ansys_tools_path-0.2.4/src/ansys/tools/path/path.py
+-rw-r--r--   0        0        0     6176 1970-01-01 00:00:00.000000 ansys_tools_path-0.2.4/PKG-INFO
```

### Comparing `ansys-tools-path-0.2.3/LICENSE` & `ansys_tools_path-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-tools-path-0.2.3/README.rst` & `ansys_tools_path-0.2.4/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -11,20 +11,20 @@
    :target: https://pypi.org/project/ansys-tools-path/
    :alt: Python
 
 .. |pypi| image:: https://img.shields.io/pypi/v/ansys-tools-path.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/ansys-tools-path
    :alt: PyPI
 
-.. |codecov| image:: https://codecov.io/gh/pyansys/ansys-tools-path/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/pyansys/ansys-tools-path
+.. |codecov| image:: https://codecov.io/gh/ansys/ansys-tools-path/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/ansys/ansys-tools-path
    :alt: Codecov
 
-.. |GH-CI| image:: https://github.com/pyansys/ansys-tools-path/actions/workflows/ci_cd.yml/badge.svg
-   :target: https://github.com/pyansys/ansys-tools-path/actions/workflows/ci_cd.yml
+.. |GH-CI| image:: https://github.com/ansys/ansys-tools-path/actions/workflows/ci_cd.yml/badge.svg
+   :target: https://github.com/ansys/ansys-tools-path/actions/workflows/ci_cd.yml
    :alt: GH-CI
 
 .. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
@@ -70,15 +70,15 @@
 Before contributing to the project, please refer to the `PyAnsys Developer's guide`_.
 You need to follow these steps:
 
 #. Start by cloning this repository:
 
    .. code:: bash
 
-      git clone https://github.com/pyansys/ansys-tools-path
+      git clone https://github.com/ansys/ansys-tools-path
 
 #. Create a fresh-clean Python environment and activate it:
 
    .. code:: bash
 
       # Create a virtual environment
       python -m venv .venv
```

### Comparing `ansys-tools-path-0.2.3/pyproject.toml` & `ansys_tools_path-0.2.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-tools-path"
-version = "0.2.3"
+version = "0.2.4"
 description = "Library to locate Ansys products in a local machine."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -36,32 +36,32 @@
 [project.optional-dependencies]
 test = [
     "pytest==7.3.1",
     "pytest-cov==4.0.0",
 ]
 
 doc = [
-    "Sphinx==7.0.0",
+    "Sphinx==6.2.1",
     "numpydoc==1.5.0",
-    "ansys-sphinx-theme==0.9.8",
+    "ansys-sphinx-theme==0.9.9",
     "sphinx-copybutton==0.5.2",
 ]
 
 build = [
     "build==0.10.0",
     "twine==4.0.2",
 ]
 
 [tool.flit.module]
 name = "ansys.tools.path"
 
 [project.urls]
-Source = "https://github.com/pyansys/ansys-tools-path"
-Tracker = "https://github.com/pyansys/ansys-tools-path/issues"
-Homepage = "https://github.com/pyansys/ansys-tools-path"
+Source = "https://github.com/ansys/ansys-tools-path"
+Tracker = "https://github.com/ansys/ansys-tools-path/issues"
+Homepage = "https://github.com/ansys/ansys-tools-path"
 Documentation = "https://path.tools.docs.pyansys.com"
 
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
```

### Comparing `ansys-tools-path-0.2.3/src/ansys/tools/path/__init__.py` & `ansys_tools_path-0.2.4/src/ansys/tools/path/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-tools-path-0.2.3/src/ansys/tools/path/misc.py` & `ansys_tools_path-0.2.4/src/ansys/tools/path/misc.py`

 * *Files identical despite different names*

### Comparing `ansys-tools-path-0.2.3/src/ansys/tools/path/path.py` & `ansys_tools_path-0.2.4/src/ansys/tools/path/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -647,15 +647,17 @@
     """Used by tests. We can consider supporting it on the library"""
     if os.path.isfile(CONFIG_FILE):
         os.remove(CONFIG_FILE)
 
 
 def _read_config_file(product_name: str) -> dict:
     """Read config file for a given product, migrating if needed"""
-    _migrate_config_file(product_name)
+
+    if not os.path.isfile(CONFIG_FILE):
+        _migrate_config_file(product_name)
     if os.path.isfile(CONFIG_FILE):
         with open(CONFIG_FILE, "r") as f:
             return json.load(f)
     else:
         return {}
```

### Comparing `ansys-tools-path-0.2.3/PKG-INFO` & `ansys_tools_path-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-tools-path
-Version: 0.2.3
+Version: 0.2.4
 Summary: Library to locate Ansys products in a local machine.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
@@ -14,24 +14,24 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: importlib-metadata >=4.0
 Requires-Dist: appdirs>=1.4.0
 Requires-Dist: build==0.10.0 ; extra == "build"
 Requires-Dist: twine==4.0.2 ; extra == "build"
-Requires-Dist: Sphinx==7.0.0 ; extra == "doc"
+Requires-Dist: Sphinx==6.2.1 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
-Requires-Dist: ansys-sphinx-theme==0.9.8 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: pytest==7.3.1 ; extra == "test"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "test"
 Project-URL: Documentation, https://path.tools.docs.pyansys.com
-Project-URL: Homepage, https://github.com/pyansys/ansys-tools-path
-Project-URL: Source, https://github.com/pyansys/ansys-tools-path
-Project-URL: Tracker, https://github.com/pyansys/ansys-tools-path/issues
+Project-URL: Homepage, https://github.com/ansys/ansys-tools-path
+Project-URL: Source, https://github.com/ansys/ansys-tools-path
+Project-URL: Tracker, https://github.com/ansys/ansys-tools-path/issues
 Provides-Extra: build
 Provides-Extra: doc
 Provides-Extra: test
 
 ansys-tools-path
 ================
 
@@ -45,20 +45,20 @@
    :target: https://pypi.org/project/ansys-tools-path/
    :alt: Python
 
 .. |pypi| image:: https://img.shields.io/pypi/v/ansys-tools-path.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/ansys-tools-path
    :alt: PyPI
 
-.. |codecov| image:: https://codecov.io/gh/pyansys/ansys-tools-path/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/pyansys/ansys-tools-path
+.. |codecov| image:: https://codecov.io/gh/ansys/ansys-tools-path/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/ansys/ansys-tools-path
    :alt: Codecov
 
-.. |GH-CI| image:: https://github.com/pyansys/ansys-tools-path/actions/workflows/ci_cd.yml/badge.svg
-   :target: https://github.com/pyansys/ansys-tools-path/actions/workflows/ci_cd.yml
+.. |GH-CI| image:: https://github.com/ansys/ansys-tools-path/actions/workflows/ci_cd.yml/badge.svg
+   :target: https://github.com/ansys/ansys-tools-path/actions/workflows/ci_cd.yml
    :alt: GH-CI
 
 .. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
@@ -104,15 +104,15 @@
 Before contributing to the project, please refer to the `PyAnsys Developer's guide`_.
 You need to follow these steps:
 
 #. Start by cloning this repository:
 
    .. code:: bash
 
-      git clone https://github.com/pyansys/ansys-tools-path
+      git clone https://github.com/ansys/ansys-tools-path
 
 #. Create a fresh-clean Python environment and activate it:
 
    .. code:: bash
 
       # Create a virtual environment
       python -m venv .venv
```

