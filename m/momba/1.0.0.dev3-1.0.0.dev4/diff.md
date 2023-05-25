# Comparing `tmp/momba-1.0.0.dev3.tar.gz` & `tmp/momba-1.0.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momba-1.0.0.dev3.tar", max compression
+gzip compressed data, was "momba-1.0.0.dev4.tar", max compression
```

## Comparing `momba-1.0.0.dev3.tar` & `momba-1.0.0.dev4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1160 2021-02-26 13:00:38.147882 momba-1.0.0.dev3/LICENSE
--rw-r--r--   0        0        0     4030 2021-02-26 13:00:38.147882 momba-1.0.0.dev3/README.md
--rw-r--r--   0        0        0      345 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/__init__.py
--rw-r--r--   0        0        0       91 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/analysis/__init__.py
--rw-r--r--   0        0        0     2145 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/analysis/checkers.py
--rw-r--r--   0        0        0      462 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/engine/__init__.py
--rw-r--r--   0        0        0      404 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/engine/_engine.py
--rw-r--r--   0        0        0     9822 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/engine/explore.py
--rw-r--r--   0        0        0     1025 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/engine/time.py
--rw-r--r--   0        0        0    29508 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/engine/translator.py
--rw-r--r--   0        0        0     1931 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/engine/values.py
--rw-r--r--   0        0        0      409 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/jani/__init__.py
--rw-r--r--   0        0        0    24005 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/jani/dump_model.py
--rw-r--r--   0        0        0      742 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/jani/jsonutils.py
--rw-r--r--   0        0        0    32204 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/jani/load_model.py
--rw-r--r--   0        0        0      346 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/kit/__init__.py
--rw-r--r--   0        0        0    13585 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/kit/dbm.py
--rw-r--r--   0        0        0      391 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/kit/intervals.py
--rw-r--r--   0        0        0      253 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/metadata.py
--rw-r--r--   0        0        0     1812 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/model/__init__.py
--rw-r--r--   0        0        0     3703 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/model/actions.py
--rw-r--r--   0        0        0    17482 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/model/automata.py
--rw-r--r--   0        0        0    19872 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/model/context.py
--rw-r--r--   0        0        0     4039 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/model/distributions.py
--rw-r--r--   0        0        0      781 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/model/errors.py
--rw-r--r--   0        0        0    29427 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/model/expressions.py
--rw-r--r--   0        0        0     1704 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/model/functions.py
--rw-r--r--   0        0        0     3977 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/model/networks.py
--rw-r--r--   0        0        0     9447 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/model/operators.py
--rw-r--r--   0        0        0    13360 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/model/properties.py
--rw-r--r--   0        0        0     5617 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/model/types.py
--rw-r--r--   0        0        0     1216 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/moml/__init__.py
--rw-r--r--   0        0        0     1458 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/moml/__main__.py
--rw-r--r--   0        0        0     5199 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/moml/lexer.py
--rw-r--r--   0        0        0    31226 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/moml/parser.py
--rw-r--r--   0        0        0        0 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/py.typed
--rw-r--r--   0        0        0      135 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/tools/__init__.py
--rw-r--r--   0        0        0      805 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/tools/errors.py
--rw-r--r--   0        0        0     4079 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/tools/modest.py
--rw-r--r--   0        0        0     3744 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/tools/storm.py
--rw-r--r--   0        0        0      275 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/utils/__init__.py
--rw-r--r--   0        0        0      323 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/utils/cache.py
--rw-r--r--   0        0        0     1936 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/utils/checks.py
--rw-r--r--   0        0        0      550 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/utils/clstools.py
--rw-r--r--   0        0        0     2169 2021-02-26 13:00:38.155882 momba-1.0.0.dev3/momba/utils/distribution.py
--rw-r--r--   0        0        0     1255 2021-02-26 13:00:38.159882 momba-1.0.0.dev3/pyproject.toml
--rw-r--r--   0        0        0     5146 2021-02-26 13:00:50.248990 momba-1.0.0.dev3/setup.py
--rw-r--r--   0        0        0     4918 2021-02-26 13:00:50.249872 momba-1.0.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0     1160 2021-02-26 15:00:23.494209 momba-1.0.0.dev4/LICENSE
+-rw-r--r--   0        0        0     4027 2021-02-26 15:00:23.494209 momba-1.0.0.dev4/README.md
+-rw-r--r--   0        0        0      345 2021-02-26 15:00:23.498209 momba-1.0.0.dev4/momba/__init__.py
+-rw-r--r--   0        0        0       91 2021-02-26 15:00:23.498209 momba-1.0.0.dev4/momba/analysis/__init__.py
+-rw-r--r--   0        0        0     2145 2021-02-26 15:00:23.498209 momba-1.0.0.dev4/momba/analysis/checkers.py
+-rw-r--r--   0        0        0      462 2021-02-26 15:00:23.498209 momba-1.0.0.dev4/momba/engine/__init__.py
+-rw-r--r--   0        0        0      404 2021-02-26 15:00:23.498209 momba-1.0.0.dev4/momba/engine/_engine.py
+-rw-r--r--   0        0        0     9822 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/engine/explore.py
+-rw-r--r--   0        0        0     1025 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/engine/time.py
+-rw-r--r--   0        0        0    29508 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/engine/translator.py
+-rw-r--r--   0        0        0     1931 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/engine/values.py
+-rw-r--r--   0        0        0      409 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/jani/__init__.py
+-rw-r--r--   0        0        0    24005 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/jani/dump_model.py
+-rw-r--r--   0        0        0      742 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/jani/jsonutils.py
+-rw-r--r--   0        0        0    32204 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/jani/load_model.py
+-rw-r--r--   0        0        0      346 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/kit/__init__.py
+-rw-r--r--   0        0        0    13585 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/kit/dbm.py
+-rw-r--r--   0        0        0      391 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/kit/intervals.py
+-rw-r--r--   0        0        0      253 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/metadata.py
+-rw-r--r--   0        0        0     1812 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/model/__init__.py
+-rw-r--r--   0        0        0     3703 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/model/actions.py
+-rw-r--r--   0        0        0    17482 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/model/automata.py
+-rw-r--r--   0        0        0    19872 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/model/context.py
+-rw-r--r--   0        0        0     4039 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/model/distributions.py
+-rw-r--r--   0        0        0      781 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/model/errors.py
+-rw-r--r--   0        0        0    29427 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/model/expressions.py
+-rw-r--r--   0        0        0     1704 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/model/functions.py
+-rw-r--r--   0        0        0     3977 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/model/networks.py
+-rw-r--r--   0        0        0     9447 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/model/operators.py
+-rw-r--r--   0        0        0    13360 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/model/properties.py
+-rw-r--r--   0        0        0     5617 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/model/types.py
+-rw-r--r--   0        0        0     1216 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/moml/__init__.py
+-rw-r--r--   0        0        0     1458 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/moml/__main__.py
+-rw-r--r--   0        0        0     5199 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/moml/lexer.py
+-rw-r--r--   0        0        0    31226 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/moml/parser.py
+-rw-r--r--   0        0        0        0 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/py.typed
+-rw-r--r--   0        0        0      135 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/tools/__init__.py
+-rw-r--r--   0        0        0      805 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/tools/errors.py
+-rw-r--r--   0        0        0     4079 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/tools/modest.py
+-rw-r--r--   0        0        0     3744 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/tools/storm.py
+-rw-r--r--   0        0        0      275 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/utils/__init__.py
+-rw-r--r--   0        0        0      323 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/utils/cache.py
+-rw-r--r--   0        0        0     1936 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/utils/checks.py
+-rw-r--r--   0        0        0      550 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/utils/clstools.py
+-rw-r--r--   0        0        0     2169 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/momba/utils/distribution.py
+-rw-r--r--   0        0        0     1265 2021-02-26 15:00:23.502209 momba-1.0.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0     5189 2021-02-26 15:00:33.581960 momba-1.0.0.dev4/setup.py
+-rw-r--r--   0        0        0     4980 2021-02-26 15:00:33.582960 momba-1.0.0.dev4/PKG-INFO
```

### Comparing `momba-1.0.0.dev3/LICENSE` & `momba-1.0.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/README.md` & `momba-1.0.0.dev4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <p align="center">
   <img src="https://raw.githubusercontent.com/koehlma/momba/master/docs/_static/images/logo_with_text.svg" alt="Momba Logo" width="200px">
 </p>
 
 <p align="center">
   <a href="https://pypi.python.org/pypi/momba"><img alt="PyPi Package" src="https://img.shields.io/pypi/v/momba.svg?label=latest%20version"></a>
-  <a href="https://github.com/koehlma/momba/actions"><img alt="Tests" src="https://img.shields.io/github/workflow/status/koehlma/momba/Run%20Tests?label=tests"></a>
+  <a href="https://github.com/koehlma/momba/actions"><img alt="Tests" src="https://img.shields.io/github/workflow/status/koehlma/momba/Pipeline?label=tests"></a>
   <a href="https://koehlma.github.io/momba/"><img alt="Docs" src="https://img.shields.io/static/v1?label=docs&message=master&color=blue"></a>
   <a href="https://github.com/psf/black"><img alt="Code Style: Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
   <a href="https://gitter.im/koehlma/momba?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge"><img alt="Gitter" src="https://badges.gitter.im/koehlma/momba.svg"></a>
   <a href="https://doi.org/10.5281/zenodo.4519376"><img alt="DOI" src="https://zenodo.org/badge/DOI/10.5281/zenodo.4519376.svg"></a>
 </p>
 
 *Momba* is a Python framework for dealing with quantitative models centered around the [JANI-model](http://www.jani-spec.org/) interchange format.
```

### Comparing `momba-1.0.0.dev3/momba/analysis/checkers.py` & `momba-1.0.0.dev4/momba/analysis/checkers.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/engine/explore.py` & `momba-1.0.0.dev4/momba/engine/explore.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/engine/time.py` & `momba-1.0.0.dev4/momba/engine/time.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/engine/translator.py` & `momba-1.0.0.dev4/momba/engine/translator.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/engine/values.py` & `momba-1.0.0.dev4/momba/engine/values.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/jani/dump_model.py` & `momba-1.0.0.dev4/momba/jani/dump_model.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/jani/jsonutils.py` & `momba-1.0.0.dev4/momba/jani/jsonutils.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/jani/load_model.py` & `momba-1.0.0.dev4/momba/jani/load_model.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/kit/dbm.py` & `momba-1.0.0.dev4/momba/kit/dbm.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/model/__init__.py` & `momba-1.0.0.dev4/momba/model/__init__.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/model/actions.py` & `momba-1.0.0.dev4/momba/model/actions.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/model/automata.py` & `momba-1.0.0.dev4/momba/model/automata.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/model/context.py` & `momba-1.0.0.dev4/momba/model/context.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/model/distributions.py` & `momba-1.0.0.dev4/momba/model/distributions.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/model/errors.py` & `momba-1.0.0.dev4/momba/model/errors.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/model/expressions.py` & `momba-1.0.0.dev4/momba/model/expressions.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/model/functions.py` & `momba-1.0.0.dev4/momba/model/functions.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/model/networks.py` & `momba-1.0.0.dev4/momba/model/networks.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/model/operators.py` & `momba-1.0.0.dev4/momba/model/operators.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/model/properties.py` & `momba-1.0.0.dev4/momba/model/properties.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/model/types.py` & `momba-1.0.0.dev4/momba/model/types.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/moml/__init__.py` & `momba-1.0.0.dev4/momba/moml/__init__.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/moml/__main__.py` & `momba-1.0.0.dev4/momba/moml/__main__.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/moml/lexer.py` & `momba-1.0.0.dev4/momba/moml/lexer.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/moml/parser.py` & `momba-1.0.0.dev4/momba/moml/parser.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/tools/errors.py` & `momba-1.0.0.dev4/momba/tools/errors.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/tools/modest.py` & `momba-1.0.0.dev4/momba/tools/modest.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/tools/storm.py` & `momba-1.0.0.dev4/momba/tools/storm.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/utils/checks.py` & `momba-1.0.0.dev4/momba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/utils/clstools.py` & `momba-1.0.0.dev4/momba/utils/clstools.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/momba/utils/distribution.py` & `momba-1.0.0.dev4/momba/utils/distribution.py`

 * *Files identical despite different names*

### Comparing `momba-1.0.0.dev3/pyproject.toml` & `momba-1.0.0.dev4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "momba"
-version = "1.0.0-dev3"
+version = "1.0.0.dev4"
 description = "A Python library for quantitative models."
 authors = [
     "Maximilian Köhl <koehl@cs.uni-saarland.de>"
 ]
 license = "MIT"
 readme = "README.md"
 repository = "https://dgit.cs.uni-saarland.de/koehlma/momba.git"
@@ -13,30 +13,31 @@
     "License :: OSI Approved :: MIT License",
     "Development Status :: 2 - Pre-Alpha",
     "Operating System :: OS Independent"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-click = {version = "^7.0", optional = true}
+click = { version = "^7.0", optional = true }
+momba_engine = { version = "*", optional = true }
 mxu = "^0.0.6"
 immutables = "^0.14"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 pytest-cov = "^2.8.1"
 black = { version = "^20.8b1", allow-prereleases = true }
 flake8 = "^3.7.9"
 flake8-bugbear = "^20.1.2"
 pep8-naming = "^0.9.1"
 mypy = "^0.800"
 sphinx = "^3.4.3"
 sphinx-autobuild = "^2020.9.1"
 jupyter_sphinx = "^0.3.2"
-maturin = { git = "https://github.com/koehlma/maturin.git" }
+maturin = "^0.9.4"
 furo = "^2021.2.21b25"
 myst-parser = "^0.13.3"
 
 [tool.poetry.scripts]
 momba-moml = "momba.moml.__main__:main"
 
 [tool.poetry.extras]
```

### Comparing `momba-1.0.0.dev3/setup.py` & `momba-1.0.0.dev4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,24 +15,26 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['immutables>=0.14,<0.15', 'mxu>=0.0.6,<0.0.7']
 
 extras_require = \
-{'all': ['click>=7.0,<8.0'], 'cli': ['click>=7.0,<8.0']}
+{'all': ['click>=7.0,<8.0', 'momba_engine'],
+ 'cli': ['click>=7.0,<8.0'],
+ 'engine': ['momba_engine']}
 
 entry_points = \
 {'console_scripts': ['momba-moml = momba.moml.__main__:main']}
 
 setup_kwargs = {
     'name': 'momba',
-    'version': '1.0.0.dev3',
+    'version': '1.0.0.dev4',
     'description': 'A Python library for quantitative models.',
-    'long_description': '<p align="center">\n  <img src="https://raw.githubusercontent.com/koehlma/momba/master/docs/_static/images/logo_with_text.svg" alt="Momba Logo" width="200px">\n</p>\n\n<p align="center">\n  <a href="https://pypi.python.org/pypi/momba"><img alt="PyPi Package" src="https://img.shields.io/pypi/v/momba.svg?label=latest%20version"></a>\n  <a href="https://github.com/koehlma/momba/actions"><img alt="Tests" src="https://img.shields.io/github/workflow/status/koehlma/momba/Run%20Tests?label=tests"></a>\n  <a href="https://koehlma.github.io/momba/"><img alt="Docs" src="https://img.shields.io/static/v1?label=docs&message=master&color=blue"></a>\n  <a href="https://github.com/psf/black"><img alt="Code Style: Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>\n  <a href="https://gitter.im/koehlma/momba?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge"><img alt="Gitter" src="https://badges.gitter.im/koehlma/momba.svg"></a>\n  <a href="https://doi.org/10.5281/zenodo.4519376"><img alt="DOI" src="https://zenodo.org/badge/DOI/10.5281/zenodo.4519376.svg"></a>\n</p>\n\n*Momba* is a Python framework for dealing with quantitative models centered around the [JANI-model](http://www.jani-spec.org/) interchange format.\nMomba strives to deliver an integrated and intuitive experience to aid the process of model construction, validation, and analysis.\nIt provides convenience functions for the modular construction of models effectively turning Python into a syntax-aware macro language for quantitative models.\nMomba\'s built-in exploration engine allows gaining confidence in a model, for instance, by rapidly prototyping a tool for interactive model exploration and visualization, or by connecting it to a testing framework.\nFinally, thanks to the JANI-model interchange format, several state-of-the-art model checkers and other tools are readily available for model analysis.\n\nPlease cite Momba as follows:\n\nMaximilian A. Köhl, Michaela Klauck, and Holger Hermanns: *Momba: JANI Meets Python*. In: Jan Friso Groote and Kim G. Larsen (eds.) 27th International Conference on Tools and Algorithms for the Construction and Analysis of Systems, TACAS 2021.\n\n\n## Features\n\n* first-class **import and export** of **JANI models**\n* **syntax-aware macros** for the modular construction of models with Python code\n* **built-in exploration engine** for PTAs, MDPs and other model types\n* interfaces to state-of-the-art model checkers, e.g., [The Modest Toolset](http://www.modestchecker.net/) and [Storm](https://www.stormchecker.org/)\n* pythonic and **statically typed** APIs to thinker with formal models\n\n\n## Getting Started\n\nMomba is available from the [Python Package Index](https://pypi.org/):\n```sh\npip install momba[all]\n```\nInstalling Momba with the `all` feature flag will install all optional dependencies unleashing the full power and all features of Momba.\nCheck out the [examples](https://koehlma.github.io/momba/examples) or read the [user guide](https://koehlma.github.io/momba/guide) to learn more.\n\n\n## Rust Crates\n\nThe exploration engine of Momba is written in [Rust](https://rust-lang.org) levering [PyO3](https://pyo3.rs/) for Python bindings.\nIn case you are a Rust developer you might find some of the crates in [engine/crates](engine/crates) useful.\nIn particular, the crate [momba-explore](https://crates.io/crates/momba-explore) allows developing model analysis tools with JANI support in Rust based on Momba\'s explicit state space exploration engine.\nThe Rust command line tool [`momba-sidekick`](https://crates.io/crates/momba-sidekick) directly exposes some of this functionality.\n\n\n## Acknowledgements\n\nThis project is partially supported by the ERC Advanced Investigators Grant 695614 ([POWVER](https://powver.org)), by the German Research Foundation (DFG) under grant No. 389792660, as part of [TRR 248](https://perspicuous-computing.science), and by the Key-Area Research and Development Program Grant 2018B010107004 of Guangdong Province.\n\nThanks to Sarah Sterz for the awesome Momba logo.\n',
+    'long_description': '<p align="center">\n  <img src="https://raw.githubusercontent.com/koehlma/momba/master/docs/_static/images/logo_with_text.svg" alt="Momba Logo" width="200px">\n</p>\n\n<p align="center">\n  <a href="https://pypi.python.org/pypi/momba"><img alt="PyPi Package" src="https://img.shields.io/pypi/v/momba.svg?label=latest%20version"></a>\n  <a href="https://github.com/koehlma/momba/actions"><img alt="Tests" src="https://img.shields.io/github/workflow/status/koehlma/momba/Pipeline?label=tests"></a>\n  <a href="https://koehlma.github.io/momba/"><img alt="Docs" src="https://img.shields.io/static/v1?label=docs&message=master&color=blue"></a>\n  <a href="https://github.com/psf/black"><img alt="Code Style: Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>\n  <a href="https://gitter.im/koehlma/momba?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge"><img alt="Gitter" src="https://badges.gitter.im/koehlma/momba.svg"></a>\n  <a href="https://doi.org/10.5281/zenodo.4519376"><img alt="DOI" src="https://zenodo.org/badge/DOI/10.5281/zenodo.4519376.svg"></a>\n</p>\n\n*Momba* is a Python framework for dealing with quantitative models centered around the [JANI-model](http://www.jani-spec.org/) interchange format.\nMomba strives to deliver an integrated and intuitive experience to aid the process of model construction, validation, and analysis.\nIt provides convenience functions for the modular construction of models effectively turning Python into a syntax-aware macro language for quantitative models.\nMomba\'s built-in exploration engine allows gaining confidence in a model, for instance, by rapidly prototyping a tool for interactive model exploration and visualization, or by connecting it to a testing framework.\nFinally, thanks to the JANI-model interchange format, several state-of-the-art model checkers and other tools are readily available for model analysis.\n\nPlease cite Momba as follows:\n\nMaximilian A. Köhl, Michaela Klauck, and Holger Hermanns: *Momba: JANI Meets Python*. In: Jan Friso Groote and Kim G. Larsen (eds.) 27th International Conference on Tools and Algorithms for the Construction and Analysis of Systems, TACAS 2021.\n\n\n## Features\n\n* first-class **import and export** of **JANI models**\n* **syntax-aware macros** for the modular construction of models with Python code\n* **built-in exploration engine** for PTAs, MDPs and other model types\n* interfaces to state-of-the-art model checkers, e.g., [The Modest Toolset](http://www.modestchecker.net/) and [Storm](https://www.stormchecker.org/)\n* pythonic and **statically typed** APIs to thinker with formal models\n\n\n## Getting Started\n\nMomba is available from the [Python Package Index](https://pypi.org/):\n```sh\npip install momba[all]\n```\nInstalling Momba with the `all` feature flag will install all optional dependencies unleashing the full power and all features of Momba.\nCheck out the [examples](https://koehlma.github.io/momba/examples) or read the [user guide](https://koehlma.github.io/momba/guide) to learn more.\n\n\n## Rust Crates\n\nThe exploration engine of Momba is written in [Rust](https://rust-lang.org) levering [PyO3](https://pyo3.rs/) for Python bindings.\nIn case you are a Rust developer you might find some of the crates in [engine/crates](engine/crates) useful.\nIn particular, the crate [momba-explore](https://crates.io/crates/momba-explore) allows developing model analysis tools with JANI support in Rust based on Momba\'s explicit state space exploration engine.\nThe Rust command line tool [`momba-sidekick`](https://crates.io/crates/momba-sidekick) directly exposes some of this functionality.\n\n\n## Acknowledgements\n\nThis project is partially supported by the ERC Advanced Investigators Grant 695614 ([POWVER](https://powver.org)), by the German Research Foundation (DFG) under grant No. 389792660, as part of [TRR 248](https://perspicuous-computing.science), and by the Key-Area Research and Development Program Grant 2018B010107004 of Guangdong Province.\n\nThanks to Sarah Sterz for the awesome Momba logo.\n',
     'author': 'Maximilian Köhl',
     'author_email': 'koehl@cs.uni-saarland.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://depend.cs.uni-saarland.de/~koehl/momba/',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['momba',
 'momba.analysis', 'momba.engine', 'momba.jani', 'momba.kit', 'momba.model',
 'momba.moml', 'momba.tools', 'momba.utils'] package_data = \ {'': ['*']}
 install_requires = \ ['immutables>=0.14,<0.15', 'mxu>=0.0.6,<0.0.7']
-extras_require = \ {'all': ['click>=7.0,<8.0'], 'cli': ['click>=7.0,<8.0']}
-entry_points = \ {'console_scripts': ['momba-moml = momba.moml.__main__:main']}
-setup_kwargs = { 'name': 'momba', 'version': '1.0.0.dev3', 'description': 'A
-Python library for quantitative models.', 'long_description': '
+extras_require = \ {'all': ['click>=7.0,<8.0', 'momba_engine'], 'cli':
+['click>=7.0,<8.0'], 'engine': ['momba_engine']} entry_points = \
+{'console_scripts': ['momba-moml = momba.moml.__main__:main']} setup_kwargs =
+{ 'name': 'momba', 'version': '1.0.0.dev4', 'description': 'A Python library
+for quantitative models.', 'long_description': '
                                \n [Momba Logo]\n
 \n\n
 \n [PyPi_Package]\n [Tests]\n [Docs]\n [Code_Style:_Black]\n [Gitter]\n [DOI]\n
 \n\n*Momba* is a Python framework for dealing with quantitative models centered
 around the [JANI-model](http://www.jani-spec.org/) interchange format.\nMomba
 strives to deliver an integrated and intuitive experience to aid the process of
 model construction, validation, and analysis.\nIt provides convenience
```

### Comparing `momba-1.0.0.dev3/PKG-INFO` & `momba-1.0.0.dev4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momba
-Version: 1.0.0.dev3
+Version: 1.0.0.dev4
 Summary: A Python library for quantitative models.
 Home-page: https://depend.cs.uni-saarland.de/~koehl/momba/
 License: MIT
 Author: Maximilian Köhl
 Author-email: koehl@cs.uni-saarland.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,25 +14,26 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: all
 Provides-Extra: cli
 Provides-Extra: engine
 Requires-Dist: click (>=7.0,<8.0); extra == "cli" or extra == "all"
 Requires-Dist: immutables (>=0.14,<0.15)
+Requires-Dist: momba_engine; extra == "engine" or extra == "all"
 Requires-Dist: mxu (>=0.0.6,<0.0.7)
 Project-URL: Repository, https://dgit.cs.uni-saarland.de/koehlma/momba.git
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/koehlma/momba/master/docs/_static/images/logo_with_text.svg" alt="Momba Logo" width="200px">
 </p>
 
 <p align="center">
   <a href="https://pypi.python.org/pypi/momba"><img alt="PyPi Package" src="https://img.shields.io/pypi/v/momba.svg?label=latest%20version"></a>
-  <a href="https://github.com/koehlma/momba/actions"><img alt="Tests" src="https://img.shields.io/github/workflow/status/koehlma/momba/Run%20Tests?label=tests"></a>
+  <a href="https://github.com/koehlma/momba/actions"><img alt="Tests" src="https://img.shields.io/github/workflow/status/koehlma/momba/Pipeline?label=tests"></a>
   <a href="https://koehlma.github.io/momba/"><img alt="Docs" src="https://img.shields.io/static/v1?label=docs&message=master&color=blue"></a>
   <a href="https://github.com/psf/black"><img alt="Code Style: Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
   <a href="https://gitter.im/koehlma/momba?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge"><img alt="Gitter" src="https://badges.gitter.im/koehlma/momba.svg"></a>
   <a href="https://doi.org/10.5281/zenodo.4519376"><img alt="DOI" src="https://zenodo.org/badge/DOI/10.5281/zenodo.4519376.svg"></a>
 </p>
 
 *Momba* is a Python framework for dealing with quantitative models centered around the [JANI-model](http://www.jani-spec.org/) interchange format.
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: momba Version: 1.0.0.dev3 Summary: A Python library
+Metadata-Version: 2.1 Name: momba Version: 1.0.0.dev4 Summary: A Python library
 for quantitative models. Home-page: https://depend.cs.uni-saarland.de/~koehl/
 momba/ License: MIT Author: Maximilian KÃ¶hl Author-email: koehl@cs.uni-
 saarland.de Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 2 -
 Pre-Alpha Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Provides-Extra: all Provides-Extra: cli Provides-
 Extra: engine Requires-Dist: click (>=7.0,<8.0); extra == "cli" or extra ==
-"all" Requires-Dist: immutables (>=0.14,<0.15) Requires-Dist: mxu
-(>=0.0.6,<0.0.7) Project-URL: Repository, https://dgit.cs.uni-saarland.de/
-koehlma/momba.git Description-Content-Type: text/markdown
+"all" Requires-Dist: immutables (>=0.14,<0.15) Requires-Dist: momba_engine;
+extra == "engine" or extra == "all" Requires-Dist: mxu (>=0.0.6,<0.0.7)
+Project-URL: Repository, https://dgit.cs.uni-saarland.de/koehlma/momba.git
+Description-Content-Type: text/markdown
                                  [Momba Logo]
        [PyPi_Package] [Tests] [Docs] [Code_Style:_Black] [Gitter] [DOI]
 *Momba* is a Python framework for dealing with quantitative models centered
 around the [JANI-model](http://www.jani-spec.org/) interchange format. Momba
 strives to deliver an integrated and intuitive experience to aid the process of
 model construction, validation, and analysis. It provides convenience functions
 for the modular construction of models effectively turning Python into a
```

