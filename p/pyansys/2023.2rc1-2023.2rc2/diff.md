# Comparing `tmp/pyansys-2023.2rc1.tar.gz` & `tmp/pyansys-2023.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyansys-2023.2rc1.tar", last modified: Wed Apr  5 09:48:40 2023, max compression
+gzip compressed data, was "pyansys-2023.2rc2.tar", last modified: Thu Apr 13 16:33:40 2023, max compression
```

## Comparing `pyansys-2023.2rc1.tar` & `pyansys-2023.2rc2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1089 2023-04-05 09:48:23.184417 pyansys-2023.2rc1/LICENSE
--rw-r--r--   0        0        0     8725 2023-04-05 09:48:23.184417 pyansys-2023.2rc1/README.rst
--rw-r--r--   0        0        0     2379 2023-04-05 09:48:23.200417 pyansys-2023.2rc1/pyproject.toml
--rw-r--r--   0        0        0      287 2023-04-05 09:48:23.200417 pyansys-2023.2rc1/src/pyansys/__init__.py
--rw-r--r--   0        0        0    11100 1970-01-01 00:00:00.000000 pyansys-2023.2rc1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-13 16:33:18.343608 pyansys-2023.2rc2/LICENSE
+-rw-r--r--   0        0        0     8723 2023-04-13 16:33:18.343608 pyansys-2023.2rc2/README.rst
+-rw-r--r--   0        0        0     2370 2023-04-13 16:33:18.359616 pyansys-2023.2rc2/pyproject.toml
+-rw-r--r--   0        0        0      287 2023-04-13 16:33:18.359616 pyansys-2023.2rc2/src/pyansys/__init__.py
+-rw-r--r--   0        0        0    11092 1970-01-01 00:00:00.000000 pyansys-2023.2rc2/PKG-INFO
```

### Comparing `pyansys-2023.2rc1/LICENSE` & `pyansys-2023.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyansys-2023.2rc1/README.rst` & `pyansys-2023.2rc2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 - `PyAnsys Math <https://math.docs.pyansys.com/>`_: Pythonic interface to PyAnsys Math libraries.
 - `PyDPF-Core <https://dpf.docs.pyansys.com/>`_: Pythonic interface to Ansys DPF (Data Processing Framework) for building more advanced and customized workflows.
 - `PyDPF-Post <https://post.docs.pyansys.com/>`_: Pythonic interface to DPF's postprocessing toolbox for manipulating and transforming simulation data.
 - `PyDPF Composites <https://composites.dpf.docs.pyansys.com/>`_: Pythonic interface for DPF's postprocessing of layered and short-fiber composite models.
 - `PyFluent <https://fluent.docs.pyansys.com/>`_: Pythonic interface to Ansys Fluent.
 - `PyFluent-Parametric <https://parametric.fluent.docs.pyansys.com/>`_: Pythonic interface to Ansys Fluent parametric workflows.
 - `PyFluent-Visualization <https://visualization.fluent.docs.pyansys.com/>`_: Pythonic interface to visualize Ansys Fluent simulations.
-- `PyMAPDL <https://mapdl.docs.pyansys.com/>`_: Pythonic interface to Ansys MAPDL (Mechanical APLD).
+- `PyMAPDL <https://mapdl.docs.pyansys.com/>`_: Pythonic interface to Ansys MAPDL (Mechanical APDL).
 - `PyMAPDL Reader <https://reader.docs.pyansys.com/>`_: Pythonic interface to read legacy MAPDL result files (MAPDL 14.5 and later).
 - `PyMotorCAD <https://motorcad.docs.pyansys.com/>`_: Pythonic interface to Ansys Motor-CAD.
 - `PyOptislang <https://optislang.docs.pyansys.com/>`_: Pythonic interface to Ansys Optislang.
 - `PyPIM <https://pypim.docs.pyansys.com/>`_: Pythonic interface to communicate with the Ansys PIM (Product Instance Management) API.
 - `PyPrimeMesh <https://prime.docs.pyansys.com>`_: Pythonic interface to Ansys Prime Server, which delivers core Ansys meshing technology.
 - `PySeascape <https://seascape.docs.pyansys.com/>`_: Pythonic interface to communicate with Ansys RedHawkSC and TotemSC.
 - `PySystemCoupling <https://systemcoupling.docs.pyansys.com/>`_: Pythonic interface to communicate with Ansys System Coupling.
@@ -126,23 +126,23 @@
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 
 If you lack an internet connection on your installation machine, the recommended way of installing
 the ``pyansys`` metapackage is downloading the wheelhouse archive from the
 `Releases Page <https://github.com/pyansys/pyansys/releases>`_ for your corresponding machine architecture.
 
 Each wheelhouse archive contains all the Python wheels necessary to install the ``pyansys`` metapackage from
-scratch on Windows, Linux, and MacOS from Python 3.7 to 3.10. You can install this on an isolated system with
+scratch on Windows, Linux, and MacOS from Python 3.8 to 3.11. You can install this on an isolated system with
 a fresh Python installation or on a virtual environment.
 
-For example, on Linux with Python 3.7, unzip the wheelhouse archive and install it with the following
+For example, on Linux with Python 3.8, unzip the wheelhouse archive and install it with the following
 commands:
 
 .. code:: bash
 
-    unzip pyansys-v2023.1.dev0-wheelhouse-Linux-3.7-core.zip wheelhouse
+    unzip pyansys-v2023.2rc2-wheelhouse-Linux-3.8-core.zip wheelhouse
     pip install pyansys -f wheelhouse --no-index --upgrade --ignore-installed
 
 If you're on Windows with Python 3.9, unzip to a wheelhouse directory and then install using
 the same ``pip`` command as in the previous example.
 
 Consider installing using a `virtual environment <https://docs.python.org/3/library/venv.html>`_.
```

### Comparing `pyansys-2023.2rc1/pyproject.toml` & `pyansys-2023.2rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "pyansys"
-version = "2023.2rc1"
+version = "2023.2rc2"
 description = "Pythonic interfaces to Ansys products"
 readme = "README.rst"
-requires-python = ">=3.7,<4"
+requires-python = ">=3.8,<4"
 license = {file = "LICENSE"}
 authors = [{name = "ANSYS, Inc.", email = "pyansys.support@ansys.com"}]
 maintainers = [{name = "PyAnsys developers", email = "pyansys.maintainers@ansys.com"}]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 dependencies = [
     "importlib-metadata>=4.0,<5; python_version<='3.8'",
     "ansys-mapdl-core==0.64.1",
     "ansys-dpf-core==0.8.0",
     "ansys-dpf-post==0.4.0",
     "ansys-dpf-gate==0.3.1",
     "ansys-dpf-composites==0.2b2",
     "ansys-fluent-core==0.12.5",
-    "pyaedt==0.6.61",
+    "pyaedt==0.6.70",
     "ansys-platform-instancemanagement==1.0.3",
     "ansys-grantami-bomanalytics==1.1.3",
     "ansys-openapi-common==1.2.1",
     "ansys-seascape==0.2.0",
     "ansys-meshing-prime==0.3.0",
     "pytwin==0.3.0",
     "ansys-systemcoupling-core==0.1.3",
     "ansys-motorcad-core==0.1.3",
-    "ansys-math-core==0.1.0",
+    "ansys-math-core==0.1.1",
     "ansys-optislang-core==0.2.0",
+    "ansys-mechanical-core==0.7.1",
 ]
 
 [project.optional-dependencies]
 mapdl-all = [
     "ansys-mapdl-reader==0.52.11",
 ]
 fluent-all = [
@@ -57,17 +57,17 @@
 all = [
     "ansys-mapdl-reader==0.52.11",
     "ansys-fluent-visualization==0.6.0",
     "ansys-fluent-parametric==0.6.1",
 ]
 doc = [
     "Sphinx==5.3.0",
-    "ansys-sphinx-theme==0.9.6",
+    "ansys-sphinx-theme==0.9.7",
     "sphinx-copybutton==0.5.1",
-    "sphinx-design==0.3.0",
+    "sphinx-design==0.4.1",
 ]
 
 [project.urls]
 Source = "https://github.com/pyansys/pyansys"
 Documentation = "https://docs.pyansys.com"
 
 [tool.flit.module]
```

### Comparing `pyansys-2023.2rc1/PKG-INFO` & `pyansys-2023.2rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 Metadata-Version: 2.1
 Name: pyansys
-Version: 2023.2rc1
+Version: 2023.2rc2
 Summary: Pythonic interfaces to Ansys products
 Author-email: "ANSYS, Inc." <pyansys.support@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
-Requires-Python: >=3.7,<4
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: importlib-metadata>=4.0,<5; python_version<='3.8'
 Requires-Dist: ansys-mapdl-core==0.64.1
 Requires-Dist: ansys-dpf-core==0.8.0
 Requires-Dist: ansys-dpf-post==0.4.0
 Requires-Dist: ansys-dpf-gate==0.3.1
 Requires-Dist: ansys-dpf-composites==0.2b2
 Requires-Dist: ansys-fluent-core==0.12.5
-Requires-Dist: pyaedt==0.6.61
+Requires-Dist: pyaedt==0.6.70
 Requires-Dist: ansys-platform-instancemanagement==1.0.3
 Requires-Dist: ansys-grantami-bomanalytics==1.1.3
 Requires-Dist: ansys-openapi-common==1.2.1
 Requires-Dist: ansys-seascape==0.2.0
 Requires-Dist: ansys-meshing-prime==0.3.0
 Requires-Dist: pytwin==0.3.0
 Requires-Dist: ansys-systemcoupling-core==0.1.3
 Requires-Dist: ansys-motorcad-core==0.1.3
-Requires-Dist: ansys-math-core==0.1.0
+Requires-Dist: ansys-math-core==0.1.1
 Requires-Dist: ansys-optislang-core==0.2.0
+Requires-Dist: ansys-mechanical-core==0.7.1
 Requires-Dist: ansys-mapdl-reader==0.52.11 ; extra == "all"
 Requires-Dist: ansys-fluent-visualization==0.6.0 ; extra == "all"
 Requires-Dist: ansys-fluent-parametric==0.6.1 ; extra == "all"
 Requires-Dist: Sphinx==5.3.0 ; extra == "doc"
-Requires-Dist: ansys-sphinx-theme==0.9.6 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.9.7 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.1 ; extra == "doc"
-Requires-Dist: sphinx-design==0.3.0 ; extra == "doc"
+Requires-Dist: sphinx-design==0.4.1 ; extra == "doc"
 Requires-Dist: ansys-fluent-visualization==0.6.0 ; extra == "fluent-all"
 Requires-Dist: ansys-fluent-parametric==0.6.1 ; extra == "fluent-all"
 Requires-Dist: ansys-mapdl-reader==0.52.11 ; extra == "mapdl-all"
 Project-URL: Documentation, https://docs.pyansys.com
 Project-URL: Source, https://github.com/pyansys/pyansys
 Provides-Extra: all
 Provides-Extra: doc
@@ -93,15 +93,15 @@
 - `PyAnsys Math <https://math.docs.pyansys.com/>`_: Pythonic interface to PyAnsys Math libraries.
 - `PyDPF-Core <https://dpf.docs.pyansys.com/>`_: Pythonic interface to Ansys DPF (Data Processing Framework) for building more advanced and customized workflows.
 - `PyDPF-Post <https://post.docs.pyansys.com/>`_: Pythonic interface to DPF's postprocessing toolbox for manipulating and transforming simulation data.
 - `PyDPF Composites <https://composites.dpf.docs.pyansys.com/>`_: Pythonic interface for DPF's postprocessing of layered and short-fiber composite models.
 - `PyFluent <https://fluent.docs.pyansys.com/>`_: Pythonic interface to Ansys Fluent.
 - `PyFluent-Parametric <https://parametric.fluent.docs.pyansys.com/>`_: Pythonic interface to Ansys Fluent parametric workflows.
 - `PyFluent-Visualization <https://visualization.fluent.docs.pyansys.com/>`_: Pythonic interface to visualize Ansys Fluent simulations.
-- `PyMAPDL <https://mapdl.docs.pyansys.com/>`_: Pythonic interface to Ansys MAPDL (Mechanical APLD).
+- `PyMAPDL <https://mapdl.docs.pyansys.com/>`_: Pythonic interface to Ansys MAPDL (Mechanical APDL).
 - `PyMAPDL Reader <https://reader.docs.pyansys.com/>`_: Pythonic interface to read legacy MAPDL result files (MAPDL 14.5 and later).
 - `PyMotorCAD <https://motorcad.docs.pyansys.com/>`_: Pythonic interface to Ansys Motor-CAD.
 - `PyOptislang <https://optislang.docs.pyansys.com/>`_: Pythonic interface to Ansys Optislang.
 - `PyPIM <https://pypim.docs.pyansys.com/>`_: Pythonic interface to communicate with the Ansys PIM (Product Instance Management) API.
 - `PyPrimeMesh <https://prime.docs.pyansys.com>`_: Pythonic interface to Ansys Prime Server, which delivers core Ansys meshing technology.
 - `PySeascape <https://seascape.docs.pyansys.com/>`_: Pythonic interface to communicate with Ansys RedHawkSC and TotemSC.
 - `PySystemCoupling <https://systemcoupling.docs.pyansys.com/>`_: Pythonic interface to communicate with Ansys System Coupling.
@@ -179,23 +179,23 @@
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 
 If you lack an internet connection on your installation machine, the recommended way of installing
 the ``pyansys`` metapackage is downloading the wheelhouse archive from the
 `Releases Page <https://github.com/pyansys/pyansys/releases>`_ for your corresponding machine architecture.
 
 Each wheelhouse archive contains all the Python wheels necessary to install the ``pyansys`` metapackage from
-scratch on Windows, Linux, and MacOS from Python 3.7 to 3.10. You can install this on an isolated system with
+scratch on Windows, Linux, and MacOS from Python 3.8 to 3.11. You can install this on an isolated system with
 a fresh Python installation or on a virtual environment.
 
-For example, on Linux with Python 3.7, unzip the wheelhouse archive and install it with the following
+For example, on Linux with Python 3.8, unzip the wheelhouse archive and install it with the following
 commands:
 
 .. code:: bash
 
-    unzip pyansys-v2023.1.dev0-wheelhouse-Linux-3.7-core.zip wheelhouse
+    unzip pyansys-v2023.2rc2-wheelhouse-Linux-3.8-core.zip wheelhouse
     pip install pyansys -f wheelhouse --no-index --upgrade --ignore-installed
 
 If you're on Windows with Python 3.9, unzip to a wheelhouse directory and then install using
 the same ``pip`` command as in the previous example.
 
 Consider installing using a `virtual environment <https://docs.python.org/3/library/venv.html>`_.
```

