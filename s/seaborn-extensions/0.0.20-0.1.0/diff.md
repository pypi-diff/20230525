# Comparing `tmp/seaborn_extensions-0.0.20.tar.gz` & `tmp/seaborn_extensions-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaborn_extensions-0.0.20.tar", last modified: Tue Jul 26 07:49:12 2022, max compression
+gzip compressed data, was "seaborn_extensions-0.1.0.tar", last modified: Thu May 25 09:09:30 2023, max compression
```

## Comparing `seaborn_extensions-0.0.20.tar` & `seaborn_extensions-0.1.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 afr       (1001) afr       (1001)        0 2022-07-26 07:49:12.713051 seaborn_extensions-0.0.20/
--rw-rw-r--   0 afr       (1001) afr       (1001)      292 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/.editorconfig
--rw-rw-r--   0 afr       (1001) afr       (1001)     1196 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/.gitignore
--rw-rw-r--   0 afr       (1001) afr       (1001)       42 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/.readthedocs.yml
--rw-rw-r--   0 afr       (1001) afr       (1001)      708 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/.travis.yml
--rw-rw-r--   0 afr       (1001) afr       (1001)      160 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/AUTHORS.rst
--rw-rw-r--   0 afr       (1001) afr       (1001)      375 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/CHANGELOG.rst
--rw-rw-r--   0 afr       (1001) afr       (1001)     3646 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/CONTRIBUTING.rst
--rw-rw-r--   0 afr       (1001) afr       (1001)     1556 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/LICENSE
--rw-rw-r--   0 afr       (1001) afr       (1001)      329 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/MANIFEST.in
--rw-rw-r--   0 afr       (1001) afr       (1001)     2241 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/Makefile
--rw-rw-r--   0 afr       (1001) afr       (1001)     2225 2022-07-26 07:49:12.713051 seaborn_extensions-0.0.20/PKG-INFO
--rw-rw-r--   0 afr       (1001) afr       (1001)     1201 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/README.rst
-drwxrwxr-x   0 afr       (1001) afr       (1001)        0 2022-07-26 07:49:12.709051 seaborn_extensions-0.0.20/docs/
--rw-rw-r--   0 afr       (1001) afr       (1001)      619 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/docs/Makefile
--rw-rw-r--   0 afr       (1001) afr       (1001)       28 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/docs/authors.rst
--rw-rw-r--   0 afr       (1001) afr       (1001)       30 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/docs/changelog.rst
--rw-rw-r--   0 afr       (1001) afr       (1001)     5077 2022-07-26 07:43:26.000000 seaborn_extensions-0.0.20/docs/conf.py
--rw-rw-r--   0 afr       (1001) afr       (1001)       33 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/docs/contributing.rst
--rw-rw-r--   0 afr       (1001) afr       (1001)      317 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/docs/index.rst
--rw-rw-r--   0 afr       (1001) afr       (1001)     1210 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/docs/installation.rst
--rw-rw-r--   0 afr       (1001) afr       (1001)      780 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/docs/make.bat
--rw-rw-r--   0 afr       (1001) afr       (1001)       27 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/docs/readme.rst
--rw-rw-r--   0 afr       (1001) afr       (1001)      145 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/docs/usage.rst
--rw-rw-r--   0 afr       (1001) afr       (1001)      127 2022-07-26 07:43:26.000000 seaborn_extensions-0.0.20/requirements.txt
--rw-rw-r--   0 afr       (1001) afr       (1001)       75 2022-07-26 07:43:26.000000 seaborn_extensions-0.0.20/requirements_dev.txt
-drwxrwxr-x   0 afr       (1001) afr       (1001)        0 2022-07-26 07:49:12.713051 seaborn_extensions-0.0.20/seaborn_extensions/
--rw-rw-r--   0 afr       (1001) afr       (1001)     1503 2022-07-26 07:47:41.000000 seaborn_extensions-0.0.20/seaborn_extensions/__init__.py
--rw-rw-r--   0 afr       (1001) afr       (1001)       23 2022-07-26 07:49:11.000000 seaborn_extensions-0.0.20/seaborn_extensions/_version.py
--rw-rw-r--   0 afr       (1001) afr       (1001)    14554 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/seaborn_extensions/annotated_clustermap.py
--rw-rw-r--   0 afr       (1001) afr       (1001)       60 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/seaborn_extensions/py.typed
--rw-rw-r--   0 afr       (1001) afr       (1001)     1656 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/seaborn_extensions/rankplot.py
--rw-rw-r--   0 afr       (1001) afr       (1001)    17793 2022-07-26 07:43:26.000000 seaborn_extensions-0.0.20/seaborn_extensions/swarmboxenplot.py
--rw-rw-r--   0 afr       (1001) afr       (1001)      519 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/seaborn_extensions/types.py
--rw-rw-r--   0 afr       (1001) afr       (1001)     8929 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/seaborn_extensions/utils.py
--rw-rw-r--   0 afr       (1001) afr       (1001)     4607 2022-07-14 11:49:57.000000 seaborn_extensions-0.0.20/seaborn_extensions/volcano.py
-drwxrwxr-x   0 afr       (1001) afr       (1001)        0 2022-07-26 07:49:12.713051 seaborn_extensions-0.0.20/seaborn_extensions.egg-info/
--rw-rw-r--   0 afr       (1001) afr       (1001)     2225 2022-07-26 07:49:12.000000 seaborn_extensions-0.0.20/seaborn_extensions.egg-info/PKG-INFO
--rw-rw-r--   0 afr       (1001) afr       (1001)      952 2022-07-26 07:49:12.000000 seaborn_extensions-0.0.20/seaborn_extensions.egg-info/SOURCES.txt
--rw-rw-r--   0 afr       (1001) afr       (1001)        1 2022-07-26 07:49:12.000000 seaborn_extensions-0.0.20/seaborn_extensions.egg-info/dependency_links.txt
--rw-rw-r--   0 afr       (1001) afr       (1001)        1 2022-07-26 07:49:12.000000 seaborn_extensions-0.0.20/seaborn_extensions.egg-info/not-zip-safe
--rw-rw-r--   0 afr       (1001) afr       (1001)      209 2022-07-26 07:49:12.000000 seaborn_extensions-0.0.20/seaborn_extensions.egg-info/requires.txt
--rw-rw-r--   0 afr       (1001) afr       (1001)       25 2022-07-26 07:49:12.000000 seaborn_extensions-0.0.20/seaborn_extensions.egg-info/top_level.txt
--rw-rw-r--   0 afr       (1001) afr       (1001)      460 2022-07-26 07:49:12.713051 seaborn_extensions-0.0.20/setup.cfg
--rw-rw-r--   0 afr       (1001) afr       (1001)     2221 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/setup.py
-drwxrwxr-x   0 afr       (1001) afr       (1001)        0 2022-07-26 07:49:12.713051 seaborn_extensions-0.0.20/tests/
--rw-rw-r--   0 afr       (1001) afr       (1001)       48 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/tests/__init__.py
--rw-rw-r--   0 afr       (1001) afr       (1001)     7992 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/tests/test_swarmboxenplot.py
--rw-rw-r--   0 afr       (1001) afr       (1001)      392 2022-06-28 09:44:31.000000 seaborn_extensions-0.0.20/tox.ini
+drwxrwxr-x   0 afr       (1001) afr       (1001)        0 2023-05-25 09:09:30.746896 seaborn_extensions-0.1.0/
+-rw-rw-r--   0 afr       (1001) afr       (1001)      292 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/.editorconfig
+-rw-rw-r--   0 afr       (1001) afr       (1001)     1196 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/.gitignore
+-rw-rw-r--   0 afr       (1001) afr       (1001)       42 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/.readthedocs.yml
+-rw-rw-r--   0 afr       (1001) afr       (1001)      708 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/.travis.yml
+-rw-rw-r--   0 afr       (1001) afr       (1001)      160 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/AUTHORS.rst
+-rw-rw-r--   0 afr       (1001) afr       (1001)      379 2023-05-25 08:41:50.000000 seaborn_extensions-0.1.0/CHANGELOG.rst
+-rw-rw-r--   0 afr       (1001) afr       (1001)     3646 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 afr       (1001) afr       (1001)     1556 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/LICENSE
+-rw-rw-r--   0 afr       (1001) afr       (1001)      329 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/MANIFEST.in
+-rw-rw-r--   0 afr       (1001) afr       (1001)     2458 2023-05-25 09:09:25.000000 seaborn_extensions-0.1.0/Makefile
+-rw-rw-r--   0 afr       (1001) afr       (1001)     2342 2023-05-25 09:09:30.746896 seaborn_extensions-0.1.0/PKG-INFO
+-rw-rw-r--   0 afr       (1001) afr       (1001)     1299 2023-05-25 09:01:34.000000 seaborn_extensions-0.1.0/README.rst
+drwxrwxr-x   0 afr       (1001) afr       (1001)        0 2023-05-25 09:09:30.746896 seaborn_extensions-0.1.0/docs/
+-rw-rw-r--   0 afr       (1001) afr       (1001)      619 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/docs/Makefile
+-rw-rw-r--   0 afr       (1001) afr       (1001)     1255 2023-05-25 08:38:01.000000 seaborn_extensions-0.1.0/docs/api.rst
+-rw-rw-r--   0 afr       (1001) afr       (1001)       28 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/docs/authors.rst
+-rw-rw-r--   0 afr       (1001) afr       (1001)       30 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/docs/changelog.rst
+-rw-rw-r--   0 afr       (1001) afr       (1001)     5077 2022-07-26 07:43:26.000000 seaborn_extensions-0.1.0/docs/conf.py
+-rw-rw-r--   0 afr       (1001) afr       (1001)       33 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/docs/contributing.rst
+-rw-rw-r--   0 afr       (1001) afr       (1001)      341 2023-05-25 08:45:13.000000 seaborn_extensions-0.1.0/docs/index.rst
+-rw-rw-r--   0 afr       (1001) afr       (1001)     1210 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/docs/installation.rst
+-rw-rw-r--   0 afr       (1001) afr       (1001)      780 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/docs/make.bat
+-rw-rw-r--   0 afr       (1001) afr       (1001)      997 2023-05-25 08:56:49.000000 seaborn_extensions-0.1.0/docs/usage.rst
+-rw-rw-r--   0 afr       (1001) afr       (1001)      131 2023-05-24 14:10:21.000000 seaborn_extensions-0.1.0/requirements.txt
+-rw-rw-r--   0 afr       (1001) afr       (1001)       75 2023-05-25 09:08:24.000000 seaborn_extensions-0.1.0/requirements_dev.txt
+drwxrwxr-x   0 afr       (1001) afr       (1001)        0 2023-05-25 09:09:30.746896 seaborn_extensions-0.1.0/seaborn_extensions/
+-rw-rw-r--   0 afr       (1001) afr       (1001)     1503 2022-07-26 07:47:41.000000 seaborn_extensions-0.1.0/seaborn_extensions/__init__.py
+-rw-rw-r--   0 afr       (1001) afr       (1001)       22 2023-05-25 09:09:30.000000 seaborn_extensions-0.1.0/seaborn_extensions/_version.py
+-rw-rw-r--   0 afr       (1001) afr       (1001)    14554 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/seaborn_extensions/annotated_clustermap.py
+-rw-rw-r--   0 afr       (1001) afr       (1001)       60 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/seaborn_extensions/py.typed
+-rw-rw-r--   0 afr       (1001) afr       (1001)     1656 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/seaborn_extensions/rankplot.py
+-rw-rw-r--   0 afr       (1001) afr       (1001)    19150 2023-05-25 08:57:18.000000 seaborn_extensions-0.1.0/seaborn_extensions/swarmboxenplot.py
+-rw-rw-r--   0 afr       (1001) afr       (1001)      519 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/seaborn_extensions/types.py
+-rw-rw-r--   0 afr       (1001) afr       (1001)     8929 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/seaborn_extensions/utils.py
+-rw-rw-r--   0 afr       (1001) afr       (1001)     4607 2022-07-14 11:49:57.000000 seaborn_extensions-0.1.0/seaborn_extensions/volcano.py
+drwxrwxr-x   0 afr       (1001) afr       (1001)        0 2023-05-25 09:09:30.746896 seaborn_extensions-0.1.0/seaborn_extensions.egg-info/
+-rw-rw-r--   0 afr       (1001) afr       (1001)     2342 2023-05-25 09:09:30.000000 seaborn_extensions-0.1.0/seaborn_extensions.egg-info/PKG-INFO
+-rw-rw-r--   0 afr       (1001) afr       (1001)      949 2023-05-25 09:09:30.000000 seaborn_extensions-0.1.0/seaborn_extensions.egg-info/SOURCES.txt
+-rw-rw-r--   0 afr       (1001) afr       (1001)        1 2023-05-25 09:09:30.000000 seaborn_extensions-0.1.0/seaborn_extensions.egg-info/dependency_links.txt
+-rw-rw-r--   0 afr       (1001) afr       (1001)        1 2023-05-25 09:09:30.000000 seaborn_extensions-0.1.0/seaborn_extensions.egg-info/not-zip-safe
+-rw-rw-r--   0 afr       (1001) afr       (1001)      214 2023-05-25 09:09:30.000000 seaborn_extensions-0.1.0/seaborn_extensions.egg-info/requires.txt
+-rw-rw-r--   0 afr       (1001) afr       (1001)       25 2023-05-25 09:09:30.000000 seaborn_extensions-0.1.0/seaborn_extensions.egg-info/top_level.txt
+-rw-rw-r--   0 afr       (1001) afr       (1001)      460 2023-05-25 09:09:30.746896 seaborn_extensions-0.1.0/setup.cfg
+-rw-rw-r--   0 afr       (1001) afr       (1001)     2221 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/setup.py
+drwxrwxr-x   0 afr       (1001) afr       (1001)        0 2023-05-25 09:09:30.746896 seaborn_extensions-0.1.0/tests/
+-rw-rw-r--   0 afr       (1001) afr       (1001)       48 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/tests/__init__.py
+-rw-rw-r--   0 afr       (1001) afr       (1001)     7992 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/tests/test_swarmboxenplot.py
+-rw-rw-r--   0 afr       (1001) afr       (1001)      392 2022-06-28 09:44:31.000000 seaborn_extensions-0.1.0/tox.ini
```

### Comparing `seaborn_extensions-0.0.20/.gitignore` & `seaborn_extensions-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `seaborn_extensions-0.0.20/.travis.yml` & `seaborn_extensions-0.1.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `seaborn_extensions-0.0.20/CONTRIBUTING.rst` & `seaborn_extensions-0.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `seaborn_extensions-0.0.20/LICENSE` & `seaborn_extensions-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seaborn_extensions-0.0.20/Makefile` & `seaborn_extensions-0.1.0/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 export PRINT_HELP_PYSCRIPT
 
 BROWSER := python -c "$$BROWSER_PYSCRIPT"
 
 help:
 	@python -c "$$PRINT_HELP_PYSCRIPT" < $(MAKEFILE_LIST)
 
-clean: clean-build clean-pyc clean-test ## remove all build, test, coverage and Python artifacts
+clean: clean-build clean-pyc clean-test clean-docs ## remove all build, test, coverage, Python artifacts, docs
 
 clean-build: ## remove build artifacts
 	rm -fr build/
 	rm -fr dist/
 	rm -fr .eggs/
 	find . -name '*.egg-info' -exec rm -fr {} +
 	find . -name '*.egg' -exec rm -f {} +
@@ -43,14 +43,18 @@
 
 clean-test: ## remove test and coverage artifacts
 	rm -fr .tox/
 	rm -f .coverage
 	rm -fr htmlcov/
 	rm -fr .pytest_cache
 
+clean-docs: ## remove build artifacts
+	rm -fr docs/_build
+	rm -fr ~/seaborn_extensions_docs/
+
 lint: ## check style with flake8
 	flake8 seaborn_extensions tests
 
 test: ## run tests quickly with the default Python
 	pytest
 
 test-all: ## run tests on every Python version with tox
@@ -58,21 +62,22 @@
 
 coverage: ## check code coverage quickly with the default Python
 	coverage run --source seaborn_extensions -m pytest
 	coverage report -m
 	coverage html
 	$(BROWSER) htmlcov/index.html
 
-docs: ## generate Sphinx HTML documentation, including API docs
+docs: clean-docs ## generate Sphinx HTML documentation, including API docs
 	rm -f docs/seaborn_extensions.rst
 	rm -f docs/modules.rst
 	sphinx-apidoc -o docs/ seaborn_extensions
 	$(MAKE) -C docs clean
 	$(MAKE) -C docs html
-	$(BROWSER) docs/_build/html/index.html
+	cp -r docs/_build/html ~/seaborn_extensions_docs  # to work with containerized browsers
+	$(BROWSER) ~/seaborn_extensions_docs/index.html
 
 servedocs: docs ## compile the docs watching for changes
 	watchmedo shell-command -p '*.rst' -c '$(MAKE) -C docs html' -R -D .
 
 release: dist ## package and upload a release
 	twine upload dist/*
```

### Comparing `seaborn_extensions-0.0.20/PKG-INFO` & `seaborn_extensions-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: seaborn_extensions
-Version: 0.0.20
+Version: 0.1.0
 Summary: Extensions of seaborn plots for biology
 Home-page: https://github.com/afrendeiro/seaborn_extensions
 Author: Andre Rendeiro
 Author-email: afrendeiro@gmail.com
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/afrendeiro/seaborn_extensions/issues
 Project-URL: Documentation, https://seaborn-extensions.readthedocs.io
 Project-URL: Source Code, https://github.com/afrendeiro/seaborn_extensions
 Keywords: seaborn_extensions
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -26,17 +27,14 @@
 seaborn_extensions
 ==================
 
 
 .. image:: https://img.shields.io/pypi/v/seaborn_extensions.svg
         :target: https://pypi.python.org/pypi/seaborn_extensions
 
-.. image:: https://img.shields.io/travis/afrendeiro/seaborn_extensions.svg
-        :target: https://travis-ci.com/afrendeiro/seaborn_extensions
-
 .. image:: https://readthedocs.org/projects/seaborn-extensions/badge/?version=latest
         :target: https://seaborn-extensions.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 
 My collection of general ploting functions that I build on top of seaborn.
 
@@ -46,15 +44,28 @@
 
 
 Features
 --------
 
 * swarmboxenplot: Overlayed swarm- and boxen-plots with significance bars between groups.
 * clustermap: The great clustermap but with easy annotation of rows and columns for numeric and categorical factors.
+* volcano_plot: A volcano plot with great defaults.
+* rankplot: A simple rank vs value plot, also known as a waterfall plot.
+
+
+Installation
+------------
+
+To install seaborn_extensions, simply use pip::
+
+        pip install seaborn_extensions
+
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
```

### Comparing `seaborn_extensions-0.0.20/README.rst` & `seaborn_extensions-0.1.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 seaborn_extensions
 ==================
 
 
 .. image:: https://img.shields.io/pypi/v/seaborn_extensions.svg
         :target: https://pypi.python.org/pypi/seaborn_extensions
 
-.. image:: https://img.shields.io/travis/afrendeiro/seaborn_extensions.svg
-        :target: https://travis-ci.com/afrendeiro/seaborn_extensions
-
 .. image:: https://readthedocs.org/projects/seaborn-extensions/badge/?version=latest
         :target: https://seaborn-extensions.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 
 My collection of general ploting functions that I build on top of seaborn.
 
@@ -21,14 +18,25 @@
 
 
 Features
 --------
 
 * swarmboxenplot: Overlayed swarm- and boxen-plots with significance bars between groups.
 * clustermap: The great clustermap but with easy annotation of rows and columns for numeric and categorical factors.
+* volcano_plot: A volcano plot with great defaults.
+* rankplot: A simple rank vs value plot, also known as a waterfall plot.
+
+
+Installation
+------------
+
+To install seaborn_extensions, simply use pip::
+
+        pip install seaborn_extensions
+
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
```

### Comparing `seaborn_extensions-0.0.20/docs/Makefile` & `seaborn_extensions-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `seaborn_extensions-0.0.20/docs/conf.py` & `seaborn_extensions-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `seaborn_extensions-0.0.20/docs/installation.rst` & `seaborn_extensions-0.1.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `seaborn_extensions-0.0.20/docs/make.bat` & `seaborn_extensions-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `seaborn_extensions-0.0.20/seaborn_extensions/__init__.py` & `seaborn_extensions-0.1.0/seaborn_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `seaborn_extensions-0.0.20/seaborn_extensions/annotated_clustermap.py` & `seaborn_extensions-0.1.0/seaborn_extensions/annotated_clustermap.py`

 * *Files identical despite different names*

### Comparing `seaborn_extensions-0.0.20/seaborn_extensions/rankplot.py` & `seaborn_extensions-0.1.0/seaborn_extensions/rankplot.py`

 * *Files identical despite different names*

### Comparing `seaborn_extensions-0.0.20/seaborn_extensions/swarmboxenplot.py` & `seaborn_extensions-0.1.0/seaborn_extensions/swarmboxenplot.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,32 +8,39 @@
 
 import numpy as np
 import pandas as pd
 import matplotlib
 import matplotlib.pyplot as plt
 import seaborn as sns
 import pingouin as pg
+from tqdm import tqdm as _tqdm
 
 from seaborn_extensions.types import DataFrame, Axis, Figure, Iterables
 from seaborn_extensions.utils import get_grid_dims, filter_kwargs_by_callable
 
 
 """
+import pandas as pd
+import pingouin as pg
+from seaborn_extensions import swarmboxenplot
 # Demo with various tests available in Pingouin:
 data = pd.DataFrame(
     {"cont": np.random.random(20), "cat": np.random.choice(["a", "b"], 20)}
 )
 data.loc[data["cat"] == "b", "cont"] *= 5
+fig, stats = swarmboxenplot(data=data, x='cat', y='cont')
+data['h'] = ['cl_1'] * 10 + ['cl_2'] * 10
+fig, stats = swarmboxenplot(data=data, x='cat', y='cont', hue='h')
+
+data['cont1'] = data['cont'] + np.random.random(20)
+data['cont2'] = data['cont'] + np.random.random(20)
+fig, stats = swarmboxenplot(data=data, x='cat', y=['cont1', 'cont2'], hue='h')
+
 x = 'cat'
 y = 'cont'
-
-fig, stats = swarmboxenplot(data=data, x='x', y='y', hue='h')
-
-fig, stats = swarmboxenplot(data=data, x=x, y=y)
-
 pg.ttest(*data.groupby(x)[y].apply(lambda x: list(x)))
 pg.mwu(*data.groupby(x)[y].apply(lambda x: list(x)))
 pg.kruskal(data=data, between=x, dv=y)
 pg.pairwise_ttests(data=data, between=x, dv=y, parametric=True)  # same as T-test
 pg.pairwise_ttests(data=data, between=x, dv=y, parametric=False)  # same as MWU
 
 c = data[x].astype(pd.CategoricalDtype())
@@ -43,30 +50,31 @@
 """
 
 
 def swarmboxenplot(
     data: DataFrame,
     x: str,
     y: tp.Union[str, Iterables],
-    hue: str = None,
+    hue: tp.Optional[str] = None,
     swarm: bool = True,
     boxen: bool = True,
     bar: bool = False,
     orient: str = "vertical",
     plot: bool = True,
     ax: tp.Union[Axis, tp.Sequence[Axis]] = None,
     test: tp.Union[bool, str] = "mann-whitney",
     to_test: str = "all",
     multiple_testing: tp.Union[bool, str] = "fdr_bh",
     test_upper_threshold: float = 0.05,
     test_lower_threshold: float = 0.01,
     plot_non_significant: bool = False,
-    plot_kws: tp.Dict[str, tp.Any] = None,
-    test_kws: tp.Dict[str, tp.Any] = None,
-    fig_kws: tp.Dict[str, tp.Any] = None,
+    plot_kws: tp.Optional[tp.Dict[str, tp.Any]] = None,
+    test_kws: tp.Optional[tp.Dict[str, tp.Any]] = None,
+    fig_kws: tp.Optional[tp.Dict[str, tp.Any]] = None,
+    tqdm: tp.Union[bool, tp.Dict[str, tp.Any]] = True,
 ) -> tp.Optional[tp.Union[Figure, DataFrame, tp.Tuple[Figure, DataFrame]]]:
     """
     A categorical plot that overlays individual observations
     as a swarm plot and summary statistics about them in a boxen plot.
 
     In addition, this plot will test differences between observation
     groups and add lines representing a significant difference between
@@ -122,14 +130,17 @@
     plot_non_significant: bool
         Whether to add a "n.s." sign to p-values above `test_upper_threshold`.
     plot_kws: dict
         Additional values to pass to seaborn.boxenplot or seaborn.swarmplot
     test_kws: dict
         Additional values to pass to pingouin.pairwise_tests.
         The default is: dict(parametric=False) to run a non-parametric test.
+    tqdm: bool, dict
+        Additional values to pass to pingouin.pairwise_tests.
+        The default is: dict(parametric=False) to run a non-parametric test.
 
     Returns
     -------
     tuple[Figure, pandas.DataFrame]:
         if `ax` is None and `test` is True.
 
         pandas.DataFrame: if `ax` is not None.
@@ -155,15 +166,26 @@
                 raise ValueError(
                     f"`{name}` variable must be categorical, string or object."
                 )
 
     if test_kws is None:
         test_kws = dict()
     if plot_kws is None:
-        plot_kws = dict()
+        plot_kws = dict(palette="tab10")
+    if isinstance(tqdm, bool):
+        tqdm_kws = dict(
+            disable=not tqdm, total=len(y) if not isinstance(y, str) else 1, desc="y"
+        )
+    else:
+        tqdm_kws = tqdm
+        tqdm_kws["disable"] = False
+        kw = dict(total=len(y) if not isinstance(y, str) else 1, desc="y")
+        for k, v in kw.items():
+            if k not in tqdm_kws:
+                tqdm_kws[k] = v
 
     data = data.sort_values([x] + ([hue] if hue is not None else []))
 
     if isinstance(y, (list, pd.Series, pd.Index)):
         if plot:
             # TODO: display only one legend for hue
             if ax is None:
@@ -179,15 +201,15 @@
             elif isinstance(ax, matplotlib.axes.Axes):
                 axes = np.asarray([ax])
         else:
             axes = [None] * len(y)
 
         _stats = list()
         idx = -1
-        for idx, _var in enumerate(y):
+        for idx, _var in _tqdm(enumerate(y), **tqdm_kws):
             _ax = axes[idx]
             s: DataFrame = swarmboxenplot(
                 data=data,
                 x=x,
                 y=_var,
                 hue=hue,
                 swarm=swarm,
@@ -262,15 +284,24 @@
             _add_transparency_to_plot(_ax, kind="bar" if bar else "boxen")
         if swarm:
             swarm_kws = filter_kwargs_by_callable(plot_kws, sns.swarmplot)
             if hue is not None and "dodge" not in swarm_kws:
                 swarm_kws["dodge"] = True
             with warnings.catch_warnings():
                 warnings.filterwarnings("ignore", category=UserWarning)
-                sns.swarmplot(data=data, x=x, y=y, hue=hue, ax=_ax, **swarm_kws)
+                sns.swarmplot(
+                    data=data,
+                    x=x,
+                    y=y,
+                    # use `hue` as `x` to have scatter colored accordingly
+                    hue=hue if hue is not None else x,
+                    legend="auto" if hue is not None else False,
+                    ax=_ax,
+                    **swarm_kws,
+                )
         if horizontal:
             _ax.set_yticklabels(_ax.get_yticklabels(), rotation=0, ha="right")
         else:
             _ax.set_xticklabels(_ax.get_xticklabels(), rotation=90, ha="right")
 
     if test is False:
         return fig if ax is None else None
@@ -439,15 +470,14 @@
     _ax.set_ylim(ylim)
     return (fig, stat) if ax is None else stat
 
 
 def _add_transparency_to_plot(
     ax: Axis, alpha: float = 0.25, kind: str = "boxen"
 ) -> None:
-
     objs = (
         (
             matplotlib.collections.PatchCollection,
             matplotlib.collections.PathCollection,
         )
         if kind == "boxen"
         else (matplotlib.patches.Rectangle)
```

### Comparing `seaborn_extensions-0.0.20/seaborn_extensions/types.py` & `seaborn_extensions-0.1.0/seaborn_extensions/types.py`

 * *Files identical despite different names*

### Comparing `seaborn_extensions-0.0.20/seaborn_extensions/utils.py` & `seaborn_extensions-0.1.0/seaborn_extensions/utils.py`

 * *Files identical despite different names*

### Comparing `seaborn_extensions-0.0.20/seaborn_extensions/volcano.py` & `seaborn_extensions-0.1.0/seaborn_extensions/volcano.py`

 * *Files identical despite different names*

### Comparing `seaborn_extensions-0.0.20/seaborn_extensions.egg-info/PKG-INFO` & `seaborn_extensions-0.1.0/seaborn_extensions.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: seaborn-extensions
-Version: 0.0.20
+Version: 0.1.0
 Summary: Extensions of seaborn plots for biology
 Home-page: https://github.com/afrendeiro/seaborn_extensions
 Author: Andre Rendeiro
 Author-email: afrendeiro@gmail.com
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/afrendeiro/seaborn_extensions/issues
 Project-URL: Documentation, https://seaborn-extensions.readthedocs.io
 Project-URL: Source Code, https://github.com/afrendeiro/seaborn_extensions
 Keywords: seaborn_extensions
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -26,17 +27,14 @@
 seaborn_extensions
 ==================
 
 
 .. image:: https://img.shields.io/pypi/v/seaborn_extensions.svg
         :target: https://pypi.python.org/pypi/seaborn_extensions
 
-.. image:: https://img.shields.io/travis/afrendeiro/seaborn_extensions.svg
-        :target: https://travis-ci.com/afrendeiro/seaborn_extensions
-
 .. image:: https://readthedocs.org/projects/seaborn-extensions/badge/?version=latest
         :target: https://seaborn-extensions.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 
 My collection of general ploting functions that I build on top of seaborn.
 
@@ -46,15 +44,28 @@
 
 
 Features
 --------
 
 * swarmboxenplot: Overlayed swarm- and boxen-plots with significance bars between groups.
 * clustermap: The great clustermap but with easy annotation of rows and columns for numeric and categorical factors.
+* volcano_plot: A volcano plot with great defaults.
+* rankplot: A simple rank vs value plot, also known as a waterfall plot.
+
+
+Installation
+------------
+
+To install seaborn_extensions, simply use pip::
+
+        pip install seaborn_extensions
+
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
```

### Comparing `seaborn_extensions-0.0.20/seaborn_extensions.egg-info/SOURCES.txt` & `seaborn_extensions-0.1.0/seaborn_extensions.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 README.rst
 requirements.txt
 requirements_dev.txt
 setup.cfg
 setup.py
 tox.ini
 docs/Makefile
+docs/api.rst
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
-docs/readme.rst
 docs/usage.rst
 seaborn_extensions/__init__.py
 seaborn_extensions/_version.py
 seaborn_extensions/annotated_clustermap.py
 seaborn_extensions/py.typed
 seaborn_extensions/rankplot.py
 seaborn_extensions/swarmboxenplot.py
```

### Comparing `seaborn_extensions-0.0.20/setup.py` & `seaborn_extensions-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `seaborn_extensions-0.0.20/tests/test_swarmboxenplot.py` & `seaborn_extensions-0.1.0/tests/test_swarmboxenplot.py`

 * *Files identical despite different names*

