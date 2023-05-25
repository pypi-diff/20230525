# Comparing `tmp/camminapy-0.8.9.tar.gz` & `tmp/camminapy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camminapy-0.8.9.tar", max compression
+gzip compressed data, was "camminapy-0.9.0.tar", max compression
```

## Comparing `camminapy-0.8.9.tar` & `camminapy-0.9.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-05-25 08:57:11.658456 camminapy-0.8.9/LICENSE
--rw-r--r--   0        0        0      177 2023-05-25 09:38:05.904312 camminapy-0.8.9/README.rst
--rw-r--r--   0        0        0      232 2023-05-25 09:36:38.187302 camminapy-0.8.9/camminapy/__init__.py
--rw-r--r--   0        0        0      343 2023-05-25 09:40:51.581748 camminapy-0.8.9/camminapy/data/__init__.py
--rw-r--r--   0        0        0     3390 2023-05-25 10:23:04.781864 camminapy-0.8.9/camminapy/data/resample.py
--rw-r--r--   0        0        0       63 2023-05-25 09:24:37.675451 camminapy-0.8.9/camminapy/plot/__init__.py
--rw-r--r--   0        0        0     2583 2023-05-25 09:25:59.612697 camminapy-0.8.9/camminapy/plot/footer.py
--rw-r--r--   0        0        0        0 2023-05-25 08:57:11.673431 camminapy-0.8.9/camminapy/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-05-25 08:57:11.672848 camminapy-0.8.9/camminapy/utils/config.py
--rw-r--r--   0        0        0      721 2023-05-25 08:57:11.674539 camminapy-0.8.9/camminapy/utils/logger.py
--rw-r--r--   0        0        0     1031 2023-05-25 10:23:16.719298 camminapy-0.8.9/pyproject.toml
--rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 camminapy-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-25 08:57:11.658456 camminapy-0.9.0/LICENSE
+-rw-r--r--   0        0        0      177 2023-05-25 09:38:05.904312 camminapy-0.9.0/README.rst
+-rw-r--r--   0        0        0      232 2023-05-25 09:36:38.187302 camminapy-0.9.0/camminapy/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-25 09:40:51.581748 camminapy-0.9.0/camminapy/data/__init__.py
+-rw-r--r--   0        0        0     3390 2023-05-25 10:23:04.781864 camminapy-0.9.0/camminapy/data/resample.py
+-rw-r--r--   0        0        0      163 2023-05-25 11:46:26.866899 camminapy-0.9.0/camminapy/plot/__init__.py
+-rw-r--r--   0        0        0     1085 2023-05-25 11:44:40.466282 camminapy-0.9.0/camminapy/plot/altair_config.py
+-rw-r--r--   0        0        0     6221 2023-05-25 11:45:21.605193 camminapy-0.9.0/camminapy/plot/altair_theme.py
+-rw-r--r--   0        0        0     2622 2023-05-25 11:06:20.283403 camminapy-0.9.0/camminapy/plot/footer.py
+-rw-r--r--   0        0        0        0 2023-05-25 08:57:11.673431 camminapy-0.9.0/camminapy/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-25 08:57:11.672848 camminapy-0.9.0/camminapy/utils/config.py
+-rw-r--r--   0        0        0      721 2023-05-25 08:57:11.674539 camminapy-0.9.0/camminapy/utils/logger.py
+-rw-r--r--   0        0        0     1084 2023-05-25 12:55:26.042757 camminapy-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 camminapy-0.9.0/PKG-INFO
```

### Comparing `camminapy-0.8.9/LICENSE` & `camminapy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.9/camminapy/data/resample.py` & `camminapy-0.9.0/camminapy/data/resample.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.9/camminapy/plot/footer.py` & `camminapy-0.9.0/camminapy/plot/footer.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 from typing import Any
 
 import altair as alt
 from git import Repo  # type: ignore
 
 
 class Footer:
-    """Add .properties(title=Footer().create()) to your plot to create a footer.
+    """Add .properties(title=Footer(repo).create()) to your plot to create a footer.
 
     IMPORTANT: As of now, this kills the original title.
 
     Workaround:
     Add .properties(title={"text": "ACTUAL PLOT TITLE", **Footer().subtitle()})
     Then it is not a footer but a subtitle.
     """
 
-    def __init__(self, repo: str):
-        self.path = repo  # TODO: Get this automatically as pwd.
-        self.repo = Repo(repo)
+    def __init__(self, path: str | None = None):
+        if path is None:
+            path = os.getcwd()
+        self.path = path
+        self.repo = Repo(self.path)
 
     def get_username(self) -> str:
         """Returns the username."""
         return pwd.getpwuid(os.getuid())[0]
 
     def get_path(self) -> str:
         """Returns the path to the repo."""
```

### Comparing `camminapy-0.8.9/camminapy/utils/config.py` & `camminapy-0.9.0/camminapy/utils/config.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.9/camminapy/utils/logger.py` & `camminapy-0.9.0/camminapy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `camminapy-0.8.9/pyproject.toml` & `camminapy-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [tool.poetry]
 name = "camminapy"
-version = "0.8.9"
+version = "0.9.0"
 description = "Personal helper functions and code snippets."
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 readme = "README.rst"
 repository = "https://github.com/thomascamminady/camminapy"
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 altair = "^5.0.0"
 gitpython = "^3.1.31"
 polars = "^0.17.15"
 pyarrow = "^12.0.0"
+rich = "^13.3.5"
+toolz = "^0.12.0"
+pdoc3 = "^0.10.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.0.1"
 ruff = "^0.0.253"
 black = "^23.1.0"
 pyclean = "^2.2.0"
 pre-commit = "^3.1.1"
```

