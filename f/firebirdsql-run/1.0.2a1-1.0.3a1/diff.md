# Comparing `tmp/firebirdsql_run-1.0.2a1.tar.gz` & `tmp/firebirdsql_run-1.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firebirdsql_run-1.0.2a1.tar", max compression
+gzip compressed data, was "firebirdsql_run-1.0.3a1.tar", max compression
```

## Comparing `firebirdsql_run-1.0.2a1.tar` & `firebirdsql_run-1.0.3a1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2023-05-05 09:18:10.769010 firebirdsql_run-1.0.2a1/LICENSE
--rw-r--r--   0        0        0     2067 2023-05-05 09:18:10.769010 firebirdsql_run-1.0.2a1/README.md
--rw-r--r--   0        0        0     2243 2023-05-05 09:18:25.929360 firebirdsql_run-1.0.2a1/pyproject.toml
--rw-r--r--   0        0        0     3134 2023-05-05 09:18:10.769010 firebirdsql_run-1.0.2a1/src/firebirdsql_run/__init__.py
--rw-r--r--   0        0        0     2794 1970-01-01 00:00:00.000000 firebirdsql_run-1.0.2a1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-25 16:26:17.636545 firebirdsql_run-1.0.3a1/LICENSE
+-rw-r--r--   0        0        0     2067 2023-05-25 16:26:17.636545 firebirdsql_run-1.0.3a1/README.md
+-rw-r--r--   0        0        0     2245 2023-05-25 16:26:40.428232 firebirdsql_run-1.0.3a1/pyproject.toml
+-rw-r--r--   0        0        0     3123 2023-05-25 16:26:17.636545 firebirdsql_run-1.0.3a1/src/firebirdsql_run/__init__.py
+-rw-r--r--   0        0        0     2794 1970-01-01 00:00:00.000000 firebirdsql_run-1.0.3a1/PKG-INFO
```

### Comparing `firebirdsql_run-1.0.2a1/LICENSE` & `firebirdsql_run-1.0.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `firebirdsql_run-1.0.2a1/README.md` & `firebirdsql_run-1.0.3a1/README.md`

 * *Files identical despite different names*

### Comparing `firebirdsql_run-1.0.2a1/pyproject.toml` & `firebirdsql_run-1.0.3a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "firebirdsql-run"
-version = "1.0.2-alpha.1"
+version = "1.0.3-alpha.1"
 description = "Firebirdsql wrapper inspired by subprocess.run"
 authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/firebirdsql-run"
 repository = "https://github.com/DeadNews/firebirdsql-run"
 keywords = ["firebird", "sql", "api"]
@@ -18,25 +18,25 @@
 python = "^3.10"
 firebirdsql = "^1.2.2"
 
 [tool.poetry.group.ci.dependencies]
 black = "^23.3.0"
 mypy = "^1.2.0"
 poethepoet = "^0.20.0"
-ruff = "^0.0.264"
+ruff = "^0.0.270"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 
 [tool.poe.tasks]
 ruff = "ruff check ."
 black = "black --check ."
 mypy = "mypy ."
-ci.sequence = ["ruff", "black", "mypy"]
+lint.sequence = ["ruff", "black", "mypy"]
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.black]
```

### Comparing `firebirdsql_run-1.0.2a1/src/firebirdsql_run/__init__.py` & `firebirdsql_run-1.0.3a1/src/firebirdsql_run/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
 """Firebirdsql wrapper inspired by subprocess.run."""
 from datetime import datetime
 from pathlib import Path
 from socket import getfqdn
-from typing import NamedTuple, Union
+from typing import NamedTuple
 
 from firebirdsql import Connection, connect
 
-FBTypes = Union[str, float, datetime, None]
+FBTypes = str | float | datetime | None
 Dataset = list[dict[str, FBTypes]]
 
 
 class CompletedTransaction(NamedTuple):
     """The return value from execute(), representing a transaction that has finished."""
 
     host: str
```

### Comparing `firebirdsql_run-1.0.2a1/PKG-INFO` & `firebirdsql_run-1.0.3a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebirdsql-run
-Version: 1.0.2a1
+Version: 1.0.3a1
 Summary: Firebirdsql wrapper inspired by subprocess.run
 Home-page: https://github.com/DeadNews/firebirdsql-run
 License: MIT
 Keywords: firebird,sql,api
 Author: DeadNews
 Author-email: aurczpbgr@mozmail.com
 Requires-Python: >=3.10,<4.0
```

