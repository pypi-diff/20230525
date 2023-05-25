# Comparing `tmp/sans-1.1.3.tar.gz` & `tmp/sans-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sans-1.1.3.tar", last modified: Thu May 18 18:24:00 2023, max compression
+gzip compressed data, was "sans-1.1.4.tar", last modified: Thu May 25 07:09:21 2023, max compression
```

## Comparing `sans-1.1.3.tar` & `sans-1.1.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:24:00.851521 sans-1.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:24:00.843521 sans-1.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:24:00.847521 sans-1.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-18 18:23:49.000000 sans-1.1.3/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-18 18:23:49.000000 sans-1.1.3/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-18 18:23:49.000000 sans-1.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-18 18:23:49.000000 sans-1.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-18 18:23:49.000000 sans-1.1.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-18 18:23:49.000000 sans-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-18 18:24:00.851521 sans-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-18 18:23:49.000000 sans-1.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:24:00.847521 sans-1.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-18 18:23:49.000000 sans-1.1.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-18 18:23:49.000000 sans-1.1.3/docs/auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-18 18:23:49.000000 sans-1.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 18:23:49.000000 sans-1.1.3/docs/errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-18 18:23:49.000000 sans-1.1.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-18 18:23:49.000000 sans-1.1.3/docs/limiter.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-18 18:23:49.000000 sans-1.1.3/docs/lock.rst
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-18 18:23:49.000000 sans-1.1.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-18 18:23:49.000000 sans-1.1.3/docs/response.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-18 18:23:49.000000 sans-1.1.3/docs/url.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 18:23:49.000000 sans-1.1.3/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-18 18:23:49.000000 sans-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-18 18:23:49.000000 sans-1.1.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:24:00.847521 sans-1.1.3/sans/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-18 18:23:49.000000 sans-1.1.3/sans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-18 18:23:49.000000 sans-1.1.3/sans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-18 18:23:49.000000 sans-1.1.3/sans/_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-18 18:23:49.000000 sans-1.1.3/sans/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-18 18:23:49.000000 sans-1.1.3/sans/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29341 2023-05-18 18:23:49.000000 sans-1.1.3/sans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-18 18:23:49.000000 sans-1.1.3/sans/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-18 18:23:49.000000 sans-1.1.3/sans/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-18 18:23:49.000000 sans-1.1.3/sans/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-05-18 18:23:49.000000 sans-1.1.3/sans/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:23:49.000000 sans-1.1.3/sans/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-18 18:23:49.000000 sans-1.1.3/sans/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-18 18:23:49.000000 sans-1.1.3/sans/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-18 18:23:49.000000 sans-1.1.3/sans/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:24:00.851521 sans-1.1.3/sans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-18 18:24:00.000000 sans-1.1.3/sans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-18 18:24:00.000000 sans-1.1.3/sans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:24:00.000000 sans-1.1.3/sans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-18 18:24:00.000000 sans-1.1.3/sans.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-18 18:24:00.000000 sans-1.1.3/sans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-18 18:24:00.000000 sans-1.1.3/sans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 18:24:00.851521 sans-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-18 18:23:49.000000 sans-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:21.472500 sans-1.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:21.464500 sans-1.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:21.468500 sans-1.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-25 07:09:08.000000 sans-1.1.4/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-25 07:09:08.000000 sans-1.1.4/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-25 07:09:08.000000 sans-1.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-25 07:09:08.000000 sans-1.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-25 07:09:08.000000 sans-1.1.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-25 07:09:08.000000 sans-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-25 07:09:21.472500 sans-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-25 07:09:08.000000 sans-1.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:21.468500 sans-1.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-25 07:09:08.000000 sans-1.1.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-25 07:09:08.000000 sans-1.1.4/docs/auth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-25 07:09:08.000000 sans-1.1.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 07:09:08.000000 sans-1.1.4/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-25 07:09:08.000000 sans-1.1.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-25 07:09:08.000000 sans-1.1.4/docs/limiter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-25 07:09:08.000000 sans-1.1.4/docs/lock.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-25 07:09:08.000000 sans-1.1.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-25 07:09:08.000000 sans-1.1.4/docs/response.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-25 07:09:08.000000 sans-1.1.4/docs/url.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-25 07:09:08.000000 sans-1.1.4/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-25 07:09:08.000000 sans-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-25 07:09:08.000000 sans-1.1.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:21.468500 sans-1.1.4/sans/
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-25 07:09:08.000000 sans-1.1.4/sans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-25 07:09:08.000000 sans-1.1.4/sans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-25 07:09:08.000000 sans-1.1.4/sans/_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-25 07:09:08.000000 sans-1.1.4/sans/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-25 07:09:08.000000 sans-1.1.4/sans/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29341 2023-05-25 07:09:08.000000 sans-1.1.4/sans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-25 07:09:08.000000 sans-1.1.4/sans/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-25 07:09:08.000000 sans-1.1.4/sans/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-25 07:09:08.000000 sans-1.1.4/sans/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-05-25 07:09:08.000000 sans-1.1.4/sans/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:08.000000 sans-1.1.4/sans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-25 07:09:08.000000 sans-1.1.4/sans/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-25 07:09:08.000000 sans-1.1.4/sans/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-25 07:09:08.000000 sans-1.1.4/sans/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:21.472500 sans-1.1.4/sans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-25 07:09:21.000000 sans-1.1.4/sans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-25 07:09:21.000000 sans-1.1.4/sans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:09:21.000000 sans-1.1.4/sans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 07:09:21.000000 sans-1.1.4/sans.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-25 07:09:21.000000 sans-1.1.4/sans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-25 07:09:21.000000 sans-1.1.4/sans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:09:21.472500 sans-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-25 07:09:08.000000 sans-1.1.4/setup.py
```

### Comparing `sans-1.1.3/.github/workflows/codeql-analysis.yml` & `sans-1.1.4/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `sans-1.1.3/.github/workflows/pythonpublish.yml` & `sans-1.1.4/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `sans-1.1.3/.gitignore` & `sans-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `sans-1.1.3/.pre-commit-config.yaml` & `sans-1.1.4/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -6,24 +6,24 @@
     hooks:
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
     -   id: check-yaml
     -   id: check-toml
     -   id: check-added-large-files
 -   repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.267
+    rev: v0.0.269
     hooks:
     -   id: ruff
         args: [ --fix, --exit-non-zero-on-fix ]
 -   repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
     -   id: black
 -   repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.308
+    rev: v1.1.309
     hooks:
     -   id: pyright
         additional_dependencies:
             # required dependencies
         -   httpx ~= 0.23
         -   importlib_metadata >= 1.4.0; python_version < "3.8"
```

### Comparing `sans-1.1.3/LICENSE` & `sans-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sans-1.1.3/PKG-INFO` & `sans-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sans
-Version: 1.1.3
+Version: 1.1.4
 Summary: Synchronous / Asynchronous HTTPX extension for NationStates
 Author: Zephyrkul
 License: MIT License
         
         Copyright (c) 2018 - 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,15 +55,15 @@
 sans
 ====
 
 |pypi| |Code style: black| |Build Status| |Documentation Status|
 
 **S**\ ynchronous / **A**\ synchronous **N**\ ation\ **S**\ tates
 
-An extension for `HTTPX <https://www.python-httpx.org/>`_ for the `NationStates API <https://www.nationstates.net/pages/api.html>`_
+A `fully typed <https://docs.python.org/3/library/typing.html>`_ extension for `HTTPX <https://www.python-httpx.org/>`_ for the `NationStates API <https://www.nationstates.net/pages/api.html>`_.
 
 Installing
 ----------
 
 .. code::
 
    python3 -m pip install -U sans
@@ -89,15 +89,15 @@
       sans.set_agent("Darcania")
       request = sans.Nation(
          "darcania",
          "fullname population flag census",
          mode="score",
          scale="65 66",
       )
-      root = sans.get(request)
+      root = sans.get(request).xml
       sans.indent(root)
       print(ET.tostring(root, encoding="unicode"))
 
       with sans.stream("GET", sans.RegionsDump()) as response:
          for region in response.iter_xml():
             sans.indent(region)
             print(ET.tostring(region, encoding="unicode"))
```

### Comparing `sans-1.1.3/README.rst` & `sans-1.1.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 sans
 ====
 
 |pypi| |Code style: black| |Build Status| |Documentation Status|
 
 **S**\ ynchronous / **A**\ synchronous **N**\ ation\ **S**\ tates
 
-An extension for `HTTPX <https://www.python-httpx.org/>`_ for the `NationStates API <https://www.nationstates.net/pages/api.html>`_
+A `fully typed <https://docs.python.org/3/library/typing.html>`_ extension for `HTTPX <https://www.python-httpx.org/>`_ for the `NationStates API <https://www.nationstates.net/pages/api.html>`_.
 
 Installing
 ----------
 
 .. code::
 
    python3 -m pip install -U sans
@@ -35,15 +35,15 @@
       sans.set_agent("Darcania")
       request = sans.Nation(
          "darcania",
          "fullname population flag census",
          mode="score",
          scale="65 66",
       )
-      root = sans.get(request)
+      root = sans.get(request).xml
       sans.indent(root)
       print(ET.tostring(root, encoding="unicode"))
 
       with sans.stream("GET", sans.RegionsDump()) as response:
          for region in response.iter_xml():
             sans.indent(region)
             print(ET.tostring(region, encoding="unicode"))
```

### Comparing `sans-1.1.3/docs/Makefile` & `sans-1.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sans-1.1.3/docs/conf.py` & `sans-1.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.3/docs/make.bat` & `sans-1.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sans-1.1.3/pyproject.toml` & `sans-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sans-1.1.3/sans/__init__.py` & `sans-1.1.4/sans/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,17 +16,23 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+from __future__ import annotations
+
 import sys as _sys
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing_extensions import Literal
 
-from ._state import set_agent as set_agent
+from . import _state
 from .auth import *
 from .client import *
 from .errors import *
 from .limiter import *
 from .lock import *
 from .response import *
 from .url import *
@@ -41,8 +47,41 @@
 
 _meta = _metadata(__name__)
 __title__ = _meta["Name"]
 __author__ = _meta["Author"]
 __license__ = _meta["License"]
 __version__ = _meta["Version"]
 
-del _sys, _metadata, _meta  # not for export
+
+del annotations, _sys, TYPE_CHECKING, _metadata, _meta  # not for export
+
+
+def set_agent(new_agent: str, *, _force: Literal[False] = False) -> str:
+    """
+    Sets sans' User-Agent header.
+
+    Parameters
+    ----------
+    agent: str
+        The User-Agent header to use.
+        Your nation name and a method of contact, like an email address, are recommended.
+        Some script info will be appended automatically.
+    _force: bool
+        Forcibly override the User-Agent header even after it's already been set.
+        Not recommended: https://www.nationstates.net/pages/api.html#terms
+
+    Returns
+    -------
+    The actual newly set agent, including attached additional script information.
+    """
+
+    if _state.agent and not _force:
+        raise RuntimeError("Agent cannot be re-set")
+    import sys
+
+    import httpx
+
+    _state.agent = (
+        f"{new_agent} Python/{sys.version_info[0]}.{sys.version_info[1]} "
+        f"httpx/{httpx.__version__} sans/{__version__}"
+    )
+    return _state.agent
```

### Comparing `sans-1.1.3/sans/__main__.py` & `sans-1.1.4/sans/__main__.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.3/sans/auth.py` & `sans-1.1.4/sans/auth.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from httpx import Request, Response
 
 from .limiter import RateLimiter
+from .url import API_URL
 
 try:
     # guard against reloading
     _PINS  # type: ignore  # noqa: B018
 except NameError:
     _PINS: dict[str, str] = {}
 
@@ -38,25 +39,28 @@
         if value:
             self._password = None  # no longer needed
         self._autologin = value
 
     def _request_hook(self, request: Request) -> Request:
         params = request.url.params
         nation = params.get("nation")
-        if not nation or not params.get("c"):
+        if not nation:
             return request
-        auth = {}
-        if self._password:
-            auth["X-Password"] = self._password
-        elif self._autologin:
-            auth["X-Autologin"] = self._autologin
-        pin = _PINS.get(nation)
-        if pin:
-            auth["X-Pin"] = pin
-        request.method = "POST"
+        headers = request.headers
+        if self._autologin:
+            headers["X-Autologin"] = self._autologin
+            pin = _PINS.get(self._autologin)
+            if pin:
+                headers["X-Pin"] = pin
+        elif self._password:
+            headers["X-Password"] = self._password
+        request = Request("POST", API_URL, headers=headers, data=params)
         return super()._request_hook(request)
 
     def _response_hook(self, response: Response) -> None:
         autologin = response.headers.get("X-Autologin")
         if autologin:
             self.autologin = autologin
+            pin = response.headers.get("X-Pin")
+            if pin:
+                _PINS[autologin] = pin
         return super()._response_hook(response)
```

### Comparing `sans-1.1.3/sans/client.py` & `sans-1.1.4/sans/client.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.3/sans/client.pyi` & `sans-1.1.4/sans/client.pyi`

 * *Files identical despite different names*

### Comparing `sans-1.1.3/sans/decoder.py` & `sans-1.1.4/sans/decoder.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.3/sans/errors.py` & `sans-1.1.4/sans/errors.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.3/sans/limiter.py` & `sans-1.1.4/sans/limiter.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.3/sans/lock.py` & `sans-1.1.4/sans/lock.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.3/sans/response.py` & `sans-1.1.4/sans/response.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.3/sans/url.py` & `sans-1.1.4/sans/url.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,15 +40,18 @@
     for shard in shards:
         if isinstance(shard, Mapping):
             shard = dict(shard)
             q.append(shard.pop("q", None))
             query.update(shard)
         else:
             q.append(str(shard))
-    query.update(parameters, q=" ".join(map(str, filter(None, q))))
+    q_str = " ".join(map(str, filter(None, q)))
+    if q_str:
+        query["q"] = q_str
+    query.update(parameters)
     if query.get("a", "").lower() == "sendtg":
         raise RuntimeError("sans does not currently support the telegram API.")
     return API_URL.copy_with(params=query)
 
 
 def WA(
     wa: Literal[1, "1", 2, "2"], *shards: str | _Shard, **parameters: str
```

### Comparing `sans-1.1.3/sans/utils.py` & `sans-1.1.4/sans/utils.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.3/sans.egg-info/PKG-INFO` & `sans-1.1.4/sans.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sans
-Version: 1.1.3
+Version: 1.1.4
 Summary: Synchronous / Asynchronous HTTPX extension for NationStates
 Author: Zephyrkul
 License: MIT License
         
         Copyright (c) 2018 - 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,15 +55,15 @@
 sans
 ====
 
 |pypi| |Code style: black| |Build Status| |Documentation Status|
 
 **S**\ ynchronous / **A**\ synchronous **N**\ ation\ **S**\ tates
 
-An extension for `HTTPX <https://www.python-httpx.org/>`_ for the `NationStates API <https://www.nationstates.net/pages/api.html>`_
+A `fully typed <https://docs.python.org/3/library/typing.html>`_ extension for `HTTPX <https://www.python-httpx.org/>`_ for the `NationStates API <https://www.nationstates.net/pages/api.html>`_.
 
 Installing
 ----------
 
 .. code::
 
    python3 -m pip install -U sans
@@ -89,15 +89,15 @@
       sans.set_agent("Darcania")
       request = sans.Nation(
          "darcania",
          "fullname population flag census",
          mode="score",
          scale="65 66",
       )
-      root = sans.get(request)
+      root = sans.get(request).xml
       sans.indent(root)
       print(ET.tostring(root, encoding="unicode"))
 
       with sans.stream("GET", sans.RegionsDump()) as response:
          for region in response.iter_xml():
             sans.indent(region)
             print(ET.tostring(region, encoding="unicode"))
```

### Comparing `sans-1.1.3/sans.egg-info/SOURCES.txt` & `sans-1.1.4/sans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

