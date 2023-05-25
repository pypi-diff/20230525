# Comparing `tmp/firebirdsql_run-1.0.3.tar.gz` & `tmp/firebirdsql_run-1.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firebirdsql_run-1.0.3.tar", max compression
+gzip compressed data, was "firebirdsql_run-1.0.3a1.tar", max compression
```

## Comparing `firebirdsql_run-1.0.3.tar` & `firebirdsql_run-1.0.3a1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2023-05-25 16:36:46.867562 firebirdsql_run-1.0.3/LICENSE
--rw-r--r--   0        0        0     2150 2023-05-25 16:36:46.867562 firebirdsql_run-1.0.3/README.md
--rw-r--r--   0        0        0     2237 2023-05-25 16:37:00.291753 firebirdsql_run-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3171 2023-05-25 16:36:46.867562 firebirdsql_run-1.0.3/src/firebirdsql_run/__init__.py
--rw-r--r--   0        0        0     2875 1970-01-01 00:00:00.000000 firebirdsql_run-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-25 16:26:17.636545 firebirdsql_run-1.0.3a1/LICENSE
+-rw-r--r--   0        0        0     2067 2023-05-25 16:26:17.636545 firebirdsql_run-1.0.3a1/README.md
+-rw-r--r--   0        0        0     2245 2023-05-25 16:26:40.428232 firebirdsql_run-1.0.3a1/pyproject.toml
+-rw-r--r--   0        0        0     3123 2023-05-25 16:26:17.636545 firebirdsql_run-1.0.3a1/src/firebirdsql_run/__init__.py
+-rw-r--r--   0        0        0     2794 1970-01-01 00:00:00.000000 firebirdsql_run-1.0.3a1/PKG-INFO
```

### Comparing `firebirdsql_run-1.0.3/LICENSE` & `firebirdsql_run-1.0.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `firebirdsql_run-1.0.3/README.md` & `firebirdsql_run-1.0.3a1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # firebirdsql-run
 
 > [Firebirdsql](https://github.com/nakagami/pyfirebirdsql/) wrapper inspired by [subprocess.run](https://docs.python.org/3/library/subprocess.html#subprocess.run)
 
 [![PyPI version](https://img.shields.io/pypi/v/firebirdsql-run)](https://pypi.org/project/firebirdsql-run)
-[![Main](https://github.com/DeadNews/firebirdsql-run/actions/workflows/main.yml/badge.svg)](https://github.com/DeadNews/firebirdsql-run/actions/workflows/main.yml)
+[![CI/CD](https://github.com/DeadNews/firebirdsql-run/actions/workflows/python-app.yml/badge.svg)](https://github.com/DeadNews/firebirdsql-run/actions/workflows/python-app.yml)
 [![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/firebirdsql-run/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/firebirdsql-run/main)
 [![codecov](https://codecov.io/gh/DeadNews/firebirdsql-run/branch/main/graph/badge.svg?token=OCZDZIYPMC)](https://codecov.io/gh/DeadNews/firebirdsql-run)
 
 ## Installation
 
 ```sh
 pip install firebirdsql-run
@@ -24,23 +24,24 @@
 
 ```py
 result = execute(
     query="SELECT * FROM TABLE",
     host="localhost",
     db="fdb",
     user="sysdba",
+    passwd=getenv("FB_PASSWORD"),
 )
 
 if result.returncode != 0:
     log.error(result)
 else:
     log.info(result)
 ```
 
-### Info result example
+- `Info`
 
 ```py
 CompletedTransaction(
     host="localhost",
     db="fdb",
     user="sysdba",
     returncode=0,
@@ -50,15 +51,15 @@
     data=[
         {"maker": "B", "model": 1121, "type": "PC"},
         {"maker": "A", "model": 1232, "type": "PC"},
     ],
 )
 ```
 
-### Error result example
+- `Error`
 
 ```py
 CompletedTransaction(
     host="localhost",
     db="fdb",
     user="sysdba",
     returncode=1,
@@ -68,24 +69,21 @@
     data=[],
 )
 ```
 
 ### Reuse connection
 
 ```py
-conn = connection(host="localhost", db="fdb", user="sysdba")
+conn = connection(
+    host="localhost",
+    db="fdb",
+    user="sysdba",
+    passwd=getenv("FB_PASSWORD"),
+)
 
 execute(use_conn=conn, query="SELECT * FROM TABLE")
 ...
 callproc(use_conn=conn, procname="PROCNAME", params=(...))
 ...
 
 conn.close()
 ```
-
-## Env variables
-
-```ini
-FIREBIRD_KEY=
-```
-
-The `FIREBIRD_KEY` environment variable can be overridden with the optional function argument `passwd`.
```

### Comparing `firebirdsql_run-1.0.3/pyproject.toml` & `firebirdsql_run-1.0.3a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "firebirdsql-run"
-version = "1.0.3"
+version = "1.0.3-alpha.1"
 description = "Firebirdsql wrapper inspired by subprocess.run"
 authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/firebirdsql-run"
 repository = "https://github.com/DeadNews/firebirdsql-run"
 keywords = ["firebird", "sql", "api"]
```

### Comparing `firebirdsql_run-1.0.3/src/firebirdsql_run/__init__.py` & `firebirdsql_run-1.0.3a1/src/firebirdsql_run/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 """Firebirdsql wrapper inspired by subprocess.run."""
 from datetime import datetime
-from os import getenv
 from pathlib import Path
 from socket import getfqdn
 from typing import NamedTuple
 
 from firebirdsql import Connection, connect
 
 FBTypes = str | float | datetime | None
@@ -38,15 +37,15 @@
 ) -> Connection:
     """Create a connection to the database."""
     return connect(
         host=getfqdn(host),
         database=f"{db}",
         port=port,
         user=user,
-        password=passwd or getenv("FIREBIRD_KEY"),
+        password=passwd,
     )
 
 
 def execute(
     query: str,
     params: tuple = (),
     db: Path | str = "",
```

### Comparing `firebirdsql_run-1.0.3/PKG-INFO` & `firebirdsql_run-1.0.3a1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebirdsql-run
-Version: 1.0.3
+Version: 1.0.3a1
 Summary: Firebirdsql wrapper inspired by subprocess.run
 Home-page: https://github.com/DeadNews/firebirdsql-run
 License: MIT
 Keywords: firebird,sql,api
 Author: DeadNews
 Author-email: aurczpbgr@mozmail.com
 Requires-Python: >=3.10,<4.0
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 
 # firebirdsql-run
 
 > [Firebirdsql](https://github.com/nakagami/pyfirebirdsql/) wrapper inspired by [subprocess.run](https://docs.python.org/3/library/subprocess.html#subprocess.run)
 
 [![PyPI version](https://img.shields.io/pypi/v/firebirdsql-run)](https://pypi.org/project/firebirdsql-run)
-[![Main](https://github.com/DeadNews/firebirdsql-run/actions/workflows/main.yml/badge.svg)](https://github.com/DeadNews/firebirdsql-run/actions/workflows/main.yml)
+[![CI/CD](https://github.com/DeadNews/firebirdsql-run/actions/workflows/python-app.yml/badge.svg)](https://github.com/DeadNews/firebirdsql-run/actions/workflows/python-app.yml)
 [![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/firebirdsql-run/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/firebirdsql-run/main)
 [![codecov](https://codecov.io/gh/DeadNews/firebirdsql-run/branch/main/graph/badge.svg?token=OCZDZIYPMC)](https://codecov.io/gh/DeadNews/firebirdsql-run)
 
 ## Installation
 
 ```sh
 pip install firebirdsql-run
@@ -44,23 +44,24 @@
 
 ```py
 result = execute(
     query="SELECT * FROM TABLE",
     host="localhost",
     db="fdb",
     user="sysdba",
+    passwd=getenv("FB_PASSWORD"),
 )
 
 if result.returncode != 0:
     log.error(result)
 else:
     log.info(result)
 ```
 
-### Info result example
+- `Info`
 
 ```py
 CompletedTransaction(
     host="localhost",
     db="fdb",
     user="sysdba",
     returncode=0,
@@ -70,15 +71,15 @@
     data=[
         {"maker": "B", "model": 1121, "type": "PC"},
         {"maker": "A", "model": 1232, "type": "PC"},
     ],
 )
 ```
 
-### Error result example
+- `Error`
 
 ```py
 CompletedTransaction(
     host="localhost",
     db="fdb",
     user="sysdba",
     returncode=1,
@@ -88,25 +89,22 @@
     data=[],
 )
 ```
 
 ### Reuse connection
 
 ```py
-conn = connection(host="localhost", db="fdb", user="sysdba")
+conn = connection(
+    host="localhost",
+    db="fdb",
+    user="sysdba",
+    passwd=getenv("FB_PASSWORD"),
+)
 
 execute(use_conn=conn, query="SELECT * FROM TABLE")
 ...
 callproc(use_conn=conn, procname="PROCNAME", params=(...))
 ...
 
 conn.close()
 ```
 
-## Env variables
-
-```ini
-FIREBIRD_KEY=
-```
-
-The `FIREBIRD_KEY` environment variable can be overridden with the optional function argument `passwd`.
-
```

