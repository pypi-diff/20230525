# Comparing `tmp/robocorp_browser-0.4.1.tar.gz` & `tmp/robocorp_browser-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_browser-0.4.1.tar", max compression
+gzip compressed data, was "robocorp_browser-0.4.2.tar", max compression
```

## Comparing `robocorp_browser-0.4.1.tar` & `robocorp_browser-0.4.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       94 2023-05-19 08:55:34.397861 robocorp_browser-0.4.1/README.md
--rw-r--r--   0        0        0      640 2023-05-19 08:55:34.401862 robocorp_browser-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     7225 2023-05-19 08:55:34.401862 robocorp_browser-0.4.1/src/robocorp/browser/__init__.py
--rw-r--r--   0        0        0     6898 2023-05-19 08:55:34.401862 robocorp_browser-0.4.1/src/robocorp/browser/_browser_context.py
--rw-r--r--   0        0        0        0 2023-05-19 08:55:34.401862 robocorp_browser-0.4.1/src/robocorp/browser/py.typed
--rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 robocorp_browser-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-05-25 10:54:53.683212 robocorp_browser-0.4.2/README.md
+-rw-r--r--   0        0        0      640 2023-05-25 10:54:53.683212 robocorp_browser-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     7225 2023-05-25 10:54:53.683212 robocorp_browser-0.4.2/src/robocorp/browser/__init__.py
+-rw-r--r--   0        0        0     6898 2023-05-25 10:54:53.683212 robocorp_browser-0.4.2/src/robocorp/browser/_browser_context.py
+-rw-r--r--   0        0        0        0 2023-05-25 10:54:53.683212 robocorp_browser-0.4.2/src/robocorp/browser/py.typed
+-rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 robocorp_browser-0.4.2/PKG-INFO
```

### Comparing `robocorp_browser-0.4.1/pyproject.toml` & `robocorp_browser-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "robocorp-browser"
-version = "0.4.1"
+version = "0.4.2"
 description = "Robocorp browser automation library"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 	"Kerkko P. <kerkko@robocorp.com>",
 	"Ossi R. <ossi@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robocorp", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 playwright = "^1.32.1"
-robocorp-tasks = "^0.2.1"
+robocorp-tasks = "^0.3.0"
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = {path = "../devutils/", develop = true}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `robocorp_browser-0.4.1/src/robocorp/browser/__init__.py` & `robocorp_browser-0.4.2/src/robocorp/browser/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Literal, Optional
 
 from playwright.sync_api import Browser, BrowserContext, Page, Playwright
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def configure(**kwargs) -> None:
     """
     May be called before any other method to configure the browser settings.
```

### Comparing `robocorp_browser-0.4.1/src/robocorp/browser/_browser_context.py` & `robocorp_browser-0.4.2/src/robocorp/browser/_browser_context.py`

 * *Files identical despite different names*

### Comparing `robocorp_browser-0.4.1/PKG-INFO` & `robocorp_browser-0.4.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: robocorp-browser
-Version: 0.4.1
+Version: 0.4.2
 Summary: Robocorp browser automation library
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: playwright (>=1.32.1,<2.0.0)
-Requires-Dist: robocorp-tasks (>=0.2.1,<0.3.0)
+Requires-Dist: robocorp-tasks (>=0.3.0,<0.4.0)
 Description-Content-Type: text/markdown
 
 # Robocorp browser library
 
 Provides a couple of helpers on top of Playwright python library.
```

