# Comparing `tmp/prd-0.2.0.tar.gz` & `tmp/prd-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prd-0.2.0.tar", last modified: Wed Aug 17 00:20:58 2022, max compression
+gzip compressed data, was "prd-0.3.0.tar", last modified: Thu May 25 21:53:20 2023, max compression
```

## Comparing `prd-0.2.0.tar` & `prd-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-08-17 00:20:58.480778 prd-0.2.0/
--rw-rw-rw-   0        0        0     1091 2022-07-03 01:09:48.000000 prd-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     6876 2022-08-17 00:20:58.480778 prd-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     6330 2022-08-16 23:43:54.000000 prd-0.2.0/README.rst
--rw-rw-rw-   0        0        0      971 2022-08-16 23:40:16.000000 prd-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-17 00:20:58.481321 prd-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-17 00:20:58.468044 prd-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2022-08-17 00:20:58.469884 prd-0.2.0/src/prd/
--rw-rw-rw-   0        0        0       71 2022-07-03 01:11:20.000000 prd-0.2.0/src/prd/__init__.py
--rw-rw-rw-   0        0        0     2432 2022-08-16 23:38:12.000000 prd-0.2.0/src/prd/prd.py
-drwxrwxrwx   0        0        0        0 2022-08-17 00:20:58.480080 prd-0.2.0/src/prd.egg-info/
--rw-rw-rw-   0        0        0     6876 2022-08-17 00:20:58.000000 prd-0.2.0/src/prd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2022-08-17 00:20:58.000000 prd-0.2.0/src/prd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-17 00:20:58.000000 prd-0.2.0/src/prd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      181 2022-08-17 00:20:58.000000 prd-0.2.0/src/prd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2022-08-17 00:20:58.000000 prd-0.2.0/src/prd.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 21:53:20.241287 prd-0.3.0/
+-rw-rw-rw-   0        0        0     1091 2022-07-03 01:09:48.000000 prd-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     7211 2023-05-25 21:53:20.241287 prd-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6665 2023-05-05 03:57:32.000000 prd-0.3.0/README.rst
+-rw-rw-rw-   0        0        0      972 2023-05-05 03:58:14.000000 prd-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 21:53:20.241287 prd-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 21:53:20.225782 prd-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 21:53:20.230784 prd-0.3.0/src/prd/
+-rw-rw-rw-   0        0        0       71 2022-07-03 01:11:20.000000 prd-0.3.0/src/prd/__init__.py
+-rw-rw-rw-   0        0        0     2432 2022-08-16 23:38:12.000000 prd-0.3.0/src/prd/prd.py
+drwxrwxrwx   0        0        0        0 2023-05-25 21:53:20.240287 prd-0.3.0/src/prd.egg-info/
+-rw-rw-rw-   0        0        0     7211 2023-05-25 21:53:20.000000 prd-0.3.0/src/prd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-05-25 21:53:20.000000 prd-0.3.0/src/prd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 21:53:20.000000 prd-0.3.0/src/prd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      182 2023-05-25 21:53:20.000000 prd-0.3.0/src/prd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-25 21:53:20.000000 prd-0.3.0/src/prd.egg-info/top_level.txt
```

### Comparing `prd-0.2.0/LICENSE` & `prd-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prd-0.2.0/PKG-INFO` & `prd-0.3.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: prd
-Version: 0.2.0
-Summary: Idiomatic implementation of a Python function that calculates the product of the items from an iterable.
-Author: Andrei Lapets
-Author-email: a@lapets.io
-License: MIT
-Project-URL: Repository, https://github.com/lapets/prd
-Project-URL: Documentation, https://prd.readthedocs.io
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: coveralls
-Provides-Extra: publish
-License-File: LICENSE
-
 ===
 prd
 ===
 
 Idiomatic implementation of a Python function that calculates the product of the items from an iterable.
 
 |pypi| |readthedocs| |actions| |coveralls|
@@ -55,109 +37,137 @@
 .. |mul| replace:: ``__mul__``
 .. _mul: https://docs.python.org/3/reference/datamodel.html#object.__mul__
 
 A built-in product function that would complement the |sum|_ function was `rejected <https://bugs.python.org/issue1093>`__, and the built-in |math_sum|_ function does not accept iterables that contain values of non-numeric types. This library exports an idiomatic implementation (using |functools_reduce|_) of a product function that can operate on iterables that contain objects of any type for which the multiplication operation is defined (*e.g.*, via a definition of the |mul|_ method). 
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/prd>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/prd>`__:
+
+.. code-block:: bash
 
     python -m pip install prd
 
-The library can be imported in the usual ways::
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import prd
     from prd import prd
 
 Examples
 ^^^^^^^^
 
 .. |operator_mul| replace:: ``operator.mul``
 .. _operator_mul: https://docs.python.org/3/library/operator.html#operator.mul
 
-This library exports an idiomatic implementation of a product function (an analog of -- and complement to -- the built-in |sum|_ function). This function applies the built-in multiplication operator |operator_mul|_ to all of the items from the supplied iterable::
+This library exports an idiomatic implementation of a product function (an analog of -- and complement to -- the built-in |sum|_ function). This function applies the built-in multiplication operator |operator_mul|_ to all of the items from the supplied iterable:
+
+.. code-block:: python
 
     >>> prd([1, 2, 3, 4])
     24
     >>> prd([2])
     2
     >>> prd([1.2, 3.4, 5.6])
     22.848
     >>> prd([])
     1
 
-The function is compatible with objects for which the built-in multiplication operator is defined::
+The function is compatible with objects for which the built-in multiplication operator is defined:
+
+.. code-block:: python
 
     >>> class var(str):
     ...     def __mul__(self, other):
     ...         return self + ' * ' + other
     ...     def __rmul__(self, other):
     ...         return other + ' * ' + self
     >>> prd([var('b'), var('c'), var('d')], var('a'))
     'a * b * c * d'
 
-The ``start`` parameter and the elements found in the iterable can be of different types. It is only required that the output of the multiplication operation can by multiplied with the next element from the iterable::
+The ``start`` parameter and the elements found in the iterable can be of different types. It is only required that the output of the multiplication operation can by multiplied with the next element from the iterable:
+
+.. code-block:: python
 
     >>> prd([], 'a')
     'a'
     >>> prd([1, 2, 3], 'a')
     'aaaaaa'
     >>> prd(['a', 3], 2)
     'aaaaaa'
 
 Development
 -----------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs,lint]
 
 Documentation
 ^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs]
     cd docs
     sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/prd/prd.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/prd
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/prd>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/prd>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/prd>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
 
     python -m pip install .[publish]
 
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
 
     git tag ?.?.?
     git push origin ?.?.?
 
-Remove any old build/distribution files. Then, package the source into a distribution archive::
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
 
     rm -rf build dist src/*.egg-info
     python -m build --sdist --wheel .
 
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
 
     python -m twine upload dist/*
```

### Comparing `prd-0.2.0/README.rst` & `prd-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: prd
+Version: 0.3.0
+Summary: Idiomatic implementation of a Python function that calculates the product of the items from an iterable.
+Author: Andrei Lapets
+Author-email: a@lapets.io
+License: MIT
+Project-URL: Repository, https://github.com/lapets/prd
+Project-URL: Documentation, https://prd.readthedocs.io
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: coveralls
+Provides-Extra: publish
+License-File: LICENSE
+
 ===
 prd
 ===
 
 Idiomatic implementation of a Python function that calculates the product of the items from an iterable.
 
 |pypi| |readthedocs| |actions| |coveralls|
@@ -37,109 +55,137 @@
 .. |mul| replace:: ``__mul__``
 .. _mul: https://docs.python.org/3/reference/datamodel.html#object.__mul__
 
 A built-in product function that would complement the |sum|_ function was `rejected <https://bugs.python.org/issue1093>`__, and the built-in |math_sum|_ function does not accept iterables that contain values of non-numeric types. This library exports an idiomatic implementation (using |functools_reduce|_) of a product function that can operate on iterables that contain objects of any type for which the multiplication operation is defined (*e.g.*, via a definition of the |mul|_ method). 
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/prd>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/prd>`__:
+
+.. code-block:: bash
 
     python -m pip install prd
 
-The library can be imported in the usual ways::
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import prd
     from prd import prd
 
 Examples
 ^^^^^^^^
 
 .. |operator_mul| replace:: ``operator.mul``
 .. _operator_mul: https://docs.python.org/3/library/operator.html#operator.mul
 
-This library exports an idiomatic implementation of a product function (an analog of -- and complement to -- the built-in |sum|_ function). This function applies the built-in multiplication operator |operator_mul|_ to all of the items from the supplied iterable::
+This library exports an idiomatic implementation of a product function (an analog of -- and complement to -- the built-in |sum|_ function). This function applies the built-in multiplication operator |operator_mul|_ to all of the items from the supplied iterable:
+
+.. code-block:: python
 
     >>> prd([1, 2, 3, 4])
     24
     >>> prd([2])
     2
     >>> prd([1.2, 3.4, 5.6])
     22.848
     >>> prd([])
     1
 
-The function is compatible with objects for which the built-in multiplication operator is defined::
+The function is compatible with objects for which the built-in multiplication operator is defined:
+
+.. code-block:: python
 
     >>> class var(str):
     ...     def __mul__(self, other):
     ...         return self + ' * ' + other
     ...     def __rmul__(self, other):
     ...         return other + ' * ' + self
     >>> prd([var('b'), var('c'), var('d')], var('a'))
     'a * b * c * d'
 
-The ``start`` parameter and the elements found in the iterable can be of different types. It is only required that the output of the multiplication operation can by multiplied with the next element from the iterable::
+The ``start`` parameter and the elements found in the iterable can be of different types. It is only required that the output of the multiplication operation can by multiplied with the next element from the iterable:
+
+.. code-block:: python
 
     >>> prd([], 'a')
     'a'
     >>> prd([1, 2, 3], 'a')
     'aaaaaa'
     >>> prd(['a', 3], 2)
     'aaaaaa'
 
 Development
 -----------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs,lint]
 
 Documentation
 ^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs]
     cd docs
     sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/prd/prd.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/prd
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/prd>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/prd>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/prd>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
 
     python -m pip install .[publish]
 
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
 
     git tag ?.?.?
     git push origin ?.?.?
 
-Remove any old build/distribution files. Then, package the source into a distribution archive::
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
 
     rm -rf build dist src/*.egg-info
     python -m build --sdist --wheel .
 
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
 
     python -m twine upload dist/*
```

### Comparing `prd-0.2.0/pyproject.toml` & `prd-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "prd"
-version = "0.2.0"
+version = "0.3.0"
 description = """\
     Idiomatic implementation of a Python function that calculates the product \
     of the items from an iterable.\
     """
 license = {text = "MIT"}
 authors = [
     {name = "Andrei Lapets"},
@@ -20,29 +20,29 @@
 [project.optional-dependencies]
 docs = [
     "toml~=0.10.2",
     "sphinx~=4.2.0",
     "sphinx-rtd-theme~=1.0.0"
 ]
 test = [
-    "pytest~=7.0",
-    "pytest-cov~=3.0"
+    "pytest~=7.2",
+    "pytest-cov~=4.0"
 ]
 lint = [
-    "pylint~=2.14.0"
+    "pylint~=2.17.0"
 ]
 coveralls = [
     "coveralls~=3.3.1"
 ]
 publish = [
-    "build~=0.8",
+    "build~=0.10",
     "twine~=4.0"
 ]
 
 [build-system]
 requires = [
-    "setuptools~=62.0"
+    "setuptools~=67.6"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --ignore=docs --cov=prd --cov-report term-missing"
```

### Comparing `prd-0.2.0/src/prd/prd.py` & `prd-0.3.0/src/prd/prd.py`

 * *Files identical despite different names*

### Comparing `prd-0.2.0/src/prd.egg-info/PKG-INFO` & `prd-0.3.0/src/prd.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prd
-Version: 0.2.0
+Version: 0.3.0
 Summary: Idiomatic implementation of a Python function that calculates the product of the items from an iterable.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/lapets/prd
 Project-URL: Documentation, https://prd.readthedocs.io
 Requires-Python: >=3.7
@@ -55,109 +55,137 @@
 .. |mul| replace:: ``__mul__``
 .. _mul: https://docs.python.org/3/reference/datamodel.html#object.__mul__
 
 A built-in product function that would complement the |sum|_ function was `rejected <https://bugs.python.org/issue1093>`__, and the built-in |math_sum|_ function does not accept iterables that contain values of non-numeric types. This library exports an idiomatic implementation (using |functools_reduce|_) of a product function that can operate on iterables that contain objects of any type for which the multiplication operation is defined (*e.g.*, via a definition of the |mul|_ method). 
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/prd>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/prd>`__:
+
+.. code-block:: bash
 
     python -m pip install prd
 
-The library can be imported in the usual ways::
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import prd
     from prd import prd
 
 Examples
 ^^^^^^^^
 
 .. |operator_mul| replace:: ``operator.mul``
 .. _operator_mul: https://docs.python.org/3/library/operator.html#operator.mul
 
-This library exports an idiomatic implementation of a product function (an analog of -- and complement to -- the built-in |sum|_ function). This function applies the built-in multiplication operator |operator_mul|_ to all of the items from the supplied iterable::
+This library exports an idiomatic implementation of a product function (an analog of -- and complement to -- the built-in |sum|_ function). This function applies the built-in multiplication operator |operator_mul|_ to all of the items from the supplied iterable:
+
+.. code-block:: python
 
     >>> prd([1, 2, 3, 4])
     24
     >>> prd([2])
     2
     >>> prd([1.2, 3.4, 5.6])
     22.848
     >>> prd([])
     1
 
-The function is compatible with objects for which the built-in multiplication operator is defined::
+The function is compatible with objects for which the built-in multiplication operator is defined:
+
+.. code-block:: python
 
     >>> class var(str):
     ...     def __mul__(self, other):
     ...         return self + ' * ' + other
     ...     def __rmul__(self, other):
     ...         return other + ' * ' + self
     >>> prd([var('b'), var('c'), var('d')], var('a'))
     'a * b * c * d'
 
-The ``start`` parameter and the elements found in the iterable can be of different types. It is only required that the output of the multiplication operation can by multiplied with the next element from the iterable::
+The ``start`` parameter and the elements found in the iterable can be of different types. It is only required that the output of the multiplication operation can by multiplied with the next element from the iterable:
+
+.. code-block:: python
 
     >>> prd([], 'a')
     'a'
     >>> prd([1, 2, 3], 'a')
     'aaaaaa'
     >>> prd(['a', 3], 2)
     'aaaaaa'
 
 Development
 -----------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs,lint]
 
 Documentation
 ^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs]
     cd docs
     sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/prd/prd.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/prd
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/prd>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/prd>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/prd>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
 
     python -m pip install .[publish]
 
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
 
     git tag ?.?.?
     git push origin ?.?.?
 
-Remove any old build/distribution files. Then, package the source into a distribution archive::
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
 
     rm -rf build dist src/*.egg-info
     python -m build --sdist --wheel .
 
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
 
     python -m twine upload dist/*
```

