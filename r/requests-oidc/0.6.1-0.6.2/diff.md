# Comparing `tmp/requests_oidc-0.6.1.tar.gz` & `tmp/requests_oidc-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests_oidc-0.6.1.tar", max compression
+gzip compressed data, was "requests_oidc-0.6.2.tar", max compression
```

## Comparing `requests_oidc-0.6.1.tar` & `requests_oidc-0.6.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1054 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/LICENSE
--rw-r--r--   0        0        0     3500 2023-05-12 18:03:15.200671 requests_oidc-0.6.1/README.rst
--rw-r--r--   0        0        0      890 2023-05-18 19:44:22.977415 requests_oidc-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      443 2023-05-12 18:04:27.323513 requests_oidc-0.6.1/src/requests_oidc/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/__main__.py
--rw-r--r--   0        0        0     3292 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/cli.py
--rw-r--r--   0        0        0       41 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/flows/__init__.py
--rw-r--r--   0        0        0     3285 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/flows/auth_code.py
--rw-r--r--   0        0        0     1174 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/flows/client_credentials.py
--rw-r--r--   0        0        0     4021 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/flows/device_code.py
--rw-r--r--   0        0        0     1192 2023-05-12 14:40:01.115653 requests_oidc-0.6.1/src/requests_oidc/flows/token.py
--rw-r--r--   0        0        0      582 2023-05-18 19:43:58.577780 requests_oidc-0.6.1/src/requests_oidc/flows/utils.py
--rw-r--r--   0        0        0     1372 2023-05-18 19:43:58.581780 requests_oidc-0.6.1/src/requests_oidc/plugins.py
--rw-r--r--   0        0        0      170 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/types.py
--rw-r--r--   0        0        0      104 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/utils/__init__.py
--rw-r--r--   0        0        0      930 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/utils/catcher.py
--rw-r--r--   0        0        0      637 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/utils/discovery.py
--rw-r--r--   0        0        0      220 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/utils/scope.py
--rw-r--r--   0        0        0     4520 1970-01-01 00:00:00.000000 requests_oidc-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-05-12 13:41:52.727655 requests_oidc-0.6.2/LICENSE
+-rw-r--r--   0        0        0     3500 2023-05-12 18:03:15.200671 requests_oidc-0.6.2/README.rst
+-rw-r--r--   0        0        0      895 2023-05-25 21:01:07.732221 requests_oidc-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      443 2023-05-12 18:04:27.323513 requests_oidc-0.6.2/src/requests_oidc/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 13:41:52.727655 requests_oidc-0.6.2/src/requests_oidc/__main__.py
+-rw-r--r--   0        0        0     3292 2023-05-12 13:41:52.727655 requests_oidc-0.6.2/src/requests_oidc/cli.py
+-rw-r--r--   0        0        0       41 2023-05-12 13:41:52.727655 requests_oidc-0.6.2/src/requests_oidc/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-12 13:41:52.727655 requests_oidc-0.6.2/src/requests_oidc/flows/__init__.py
+-rw-r--r--   0        0        0     3285 2023-05-12 13:41:52.727655 requests_oidc-0.6.2/src/requests_oidc/flows/auth_code.py
+-rw-r--r--   0        0        0     1174 2023-05-12 13:41:52.727655 requests_oidc-0.6.2/src/requests_oidc/flows/client_credentials.py
+-rw-r--r--   0        0        0     4021 2023-05-12 13:41:52.727655 requests_oidc-0.6.2/src/requests_oidc/flows/device_code.py
+-rw-r--r--   0        0        0     1192 2023-05-12 14:40:01.115653 requests_oidc-0.6.2/src/requests_oidc/flows/token.py
+-rw-r--r--   0        0        0      582 2023-05-18 19:43:58.577780 requests_oidc-0.6.2/src/requests_oidc/flows/utils.py
+-rw-r--r--   0        0        0     1382 2023-05-25 20:59:30.669787 requests_oidc-0.6.2/src/requests_oidc/plugins.py
+-rw-r--r--   0        0        0      170 2023-05-12 13:41:52.727655 requests_oidc-0.6.2/src/requests_oidc/types.py
+-rw-r--r--   0        0        0      104 2023-05-12 13:41:52.727655 requests_oidc-0.6.2/src/requests_oidc/utils/__init__.py
+-rw-r--r--   0        0        0      930 2023-05-12 13:41:52.727655 requests_oidc-0.6.2/src/requests_oidc/utils/catcher.py
+-rw-r--r--   0        0        0      637 2023-05-12 13:41:52.727655 requests_oidc-0.6.2/src/requests_oidc/utils/discovery.py
+-rw-r--r--   0        0        0      220 2023-05-12 13:41:52.727655 requests_oidc-0.6.2/src/requests_oidc/utils/scope.py
+-rw-r--r--   0        0        0     4525 1970-01-01 00:00:00.000000 requests_oidc-0.6.2/PKG-INFO
```

### Comparing `requests_oidc-0.6.1/LICENSE` & `requests_oidc-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.6.1/README.rst` & `requests_oidc-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.6.1/pyproject.toml` & `requests_oidc-0.6.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "requests-oidc"
-version = "0.6.1"
+version = "0.6.2"
 description = ""
 authors = ["Tristan Sweeney <tsweeney@dustidentity.com>"]
 readme = "README.rst"
 packages = [{include = "requests_oidc", from = "src"}]
 repository = "https://github.com/tsweeney-dust/requests-oidc"
 documentation = "https://requests-oidc.readthedocs.io/en/latest/"
 license = "MIT"
@@ -15,17 +15,17 @@
 [tool.poetry.scripts]
 requests-oidc-cli = "requests_oidc.cli:app"
 
 [tool.poetry.dependencies]
 python = ">=3.7, <4"
 requests = "^2.28.1"
 requests-oauthlib = "^1.3.1"
-appdirs = "^1.4.4"
 qrcode = "^7.4.2"
 typer = "^0.9.0"
+platformdirs = "^3.5.1"
 
 
 [tool.poetry.group.dev.dependencies]
 sphinx = ">=5.0.0"
 sphinx-toolbox = "^3.2.0"
 sphinx-copybutton = "^0.5.1"
 types-requests = "^2.28.11.15"
```

### Comparing `requests_oidc-0.6.1/src/requests_oidc/cli.py` & `requests_oidc-0.6.2/src/requests_oidc/cli.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.6.1/src/requests_oidc/flows/auth_code.py` & `requests_oidc-0.6.2/src/requests_oidc/flows/auth_code.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.6.1/src/requests_oidc/flows/client_credentials.py` & `requests_oidc-0.6.2/src/requests_oidc/flows/client_credentials.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.6.1/src/requests_oidc/flows/device_code.py` & `requests_oidc-0.6.2/src/requests_oidc/flows/device_code.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.6.1/src/requests_oidc/flows/token.py` & `requests_oidc-0.6.2/src/requests_oidc/flows/token.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.6.1/src/requests_oidc/flows/utils.py` & `requests_oidc-0.6.2/src/requests_oidc/flows/utils.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.6.1/src/requests_oidc/plugins.py` & `requests_oidc-0.6.2/src/requests_oidc/plugins.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 import json
-import appdirs
+import platformdirs
 from typing import Optional
 
 
 class PathPlugin:
     """Plugin to load / store files to an OS path location"""
 
     def __init__(self, path: Path, *, noload: bool = False, nostore: bool = False) -> None:
@@ -37,11 +37,11 @@
         self,
         appname: str,
         appauthor: str,
         version: Optional[str] = None,
         filename: str = "token.json",
         *, noload: bool = False, nostore: bool = False
     ) -> None:
-        dirs = appdirs.AppDirs(appname=appname, appauthor=appauthor, version=version)
-        dir = Path(dirs.user_cache_dir)
+        dirs = platformdirs.PlatformDirs(appname=appname, appauthor=appauthor, version=version)
+        dir = dirs.user_cache_path
         dir.mkdir(parents=True, exist_ok=True)
         super().__init__(dir / filename, noload=noload, nostore=nostore)
```

### Comparing `requests_oidc-0.6.1/src/requests_oidc/utils/catcher.py` & `requests_oidc-0.6.2/src/requests_oidc/utils/catcher.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.6.1/src/requests_oidc/utils/discovery.py` & `requests_oidc-0.6.2/src/requests_oidc/utils/discovery.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.6.1/PKG-INFO` & `requests_oidc-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: requests-oidc
-Version: 0.6.1
+Version: 0.6.2
 Summary: 
 Home-page: https://github.com/tsweeney-dust/requests-oidc
 License: MIT
 Author: Tristan Sweeney
 Author-email: tsweeney@dustidentity.com
 Requires-Python: >=3.7,<4
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: appdirs (>=1.4.4,<2.0.0)
+Requires-Dist: platformdirs (>=3.5.1,<4.0.0)
 Requires-Dist: qrcode (>=7.4.2,<8.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: requests-oauthlib (>=1.3.1,<2.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://requests-oidc.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/tsweeney-dust/requests-oidc
 Description-Content-Type: text/x-rst
```

