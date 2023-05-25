# Comparing `tmp/mysql_context_manager-0.1.6.tar.gz` & `tmp/mysql_context_manager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql_context_manager-0.1.6.tar", max compression
+gzip compressed data, was "mysql_context_manager-0.2.0.tar", max compression
```

## Comparing `mysql_context_manager-0.1.6.tar` & `mysql_context_manager-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1065 2022-12-13 11:48:18.319462 mysql_context_manager-0.1.6/LICENSE
--rw-r--r--   0        0        0     2983 2022-12-13 11:48:18.319462 mysql_context_manager-0.1.6/README.md
--rw-r--r--   0        0        0      904 2022-12-13 11:48:18.323462 mysql_context_manager-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3338 2022-12-13 11:48:18.323462 mysql_context_manager-0.1.6/src/mysql_context_manager/__init__.py
--rw-r--r--   0        0        0     3887 1970-01-01 00:00:00.000000 mysql_context_manager-0.1.6/setup.py
--rw-r--r--   0        0        0     3806 1970-01-01 00:00:00.000000 mysql_context_manager-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-25 07:04:25.797912 mysql_context_manager-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2983 2023-05-25 07:04:25.797912 mysql_context_manager-0.2.0/README.md
+-rw-r--r--   0        0        0     1413 2023-05-25 07:04:25.797912 mysql_context_manager-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3727 2023-05-25 07:04:25.797912 mysql_context_manager-0.2.0/src/mysql_context_manager/__init__.py
+-rw-r--r--   0        0        0     3798 1970-01-01 00:00:00.000000 mysql_context_manager-0.2.0/PKG-INFO
```

### Comparing `mysql_context_manager-0.1.6/LICENSE` & `mysql_context_manager-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql_context_manager-0.1.6/README.md` & `mysql_context_manager-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mysql_context_manager-0.1.6/src/mysql_context_manager/__init__.py` & `mysql_context_manager-0.2.0/src/mysql_context_manager/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # pylint: disable=C0114,C0115,R0913
 from __future__ import annotations
 
-__version__ = "0.1.6"
+__version__ = "0.2.0"
 
+import contextlib
 import json
 from json import JSONDecodeError
 from typing import Any
 
 import databases
 
 
@@ -28,15 +29,15 @@
             schema (str | None, optional): Schema, if required. Defaults to None.
             port (int, optional): Port. Defaults to 3306.
         """
         credentials = username if password is None else f"{username}:{password}"
         if schema is None:
             schema = ""
         self.connection_string = f"mysql://{credentials}@{hostname}:{port}/{schema}"
-        self.connection = None
+        self.connection: databases.Database | None = None
         self.engine = None
 
     async def __aenter__(self):
         await self.connect()
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
@@ -49,48 +50,56 @@
         """If connection is established, disconnects"""
         if self.connection is not None:
             await self.connection.disconnect()
 
     async def connect(self) -> None:
         """Establishes the connection to the database"""
         self.connection = databases.Database(self.connection_string)
-
-        await self.connection.connect()
+        if self.connection is not None:
+            await self.connection.connect()
 
     async def query(self, sql_query: str, **kwargs) -> list[dict[str, Any]]:
         """Queries the database
 
         Args:
             sql_query (str): SQL query, with placeholders as :placeholder
 
         Returns:
             list[dict[str, Any]]: List of rows represented in dictioary format
 
+        Raises:
+            ConnectionError: in case of method call before running connect()
+
         Examples:
-            >>> query = "select username, element from users where team_name = :team_name limit 2;"
+            >>> query = "select name, elem from users where team = :team limit 2;"
             >>> async with MysqlConnector(hostname="localhost") as conn:
-            >>>    print(await conn.query(query, team_name="Team Avatar"))
-            [{"username": "Katara", "element": "water"}, {"username": "Toph", "element": "earth"}]
+            >>>    print(await conn.query(query, team="Team Avatar"))
+            [{"name": "Katara", "elem": "water"}, {"name": "Toph", "elem": "earth"}]
 
         """
-        result = await self.connection.fetch_all(query=sql_query, values=kwargs)
-        result = [dict(i) for i in result]
+        if self.connection is None:
+            raise ConnectionError("No active connection")
+        records = await self.connection.fetch_all(query=sql_query, values=kwargs)
+        result = [dict(i) for i in records]
         for res in result:
             for key, val in res.items():
-                try:
+                with contextlib.suppress(JSONDecodeError, TypeError):
                     res[key] = json.loads(val)
-                except (JSONDecodeError, TypeError):
-                    pass
         return result
 
     async def execute(self, sql_query: str, **kwargs) -> None:
         """Executes and commits an SQL query to the database
 
         Args:
             sql_query (str): SQL query, with placeholders as :placeholder
 
+        Raises:
+            ConnectionError: in case of method call before running connect()
+
         Examples:
-            >>> query = "update users set username = :username where user_id = :user_id;"
+            >>> query = "update users set name = :name where user_id = :user_id;"
             >>> async with MysqlConnector(hostname="localhost") as conn:
-            >>>    await conn.query(query, username="Truth", user_id=42)
+            >>>    await conn.query(query, name="Truth", user_id=42)
         """
+        if self.connection is None:
+            raise ConnectionError("No active connection")
         await self.connection.execute(query=sql_query, values=kwargs)
```

### Comparing `mysql_context_manager-0.1.6/setup.py` & `mysql_context_manager-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,101 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: mysql-context-manager
+Version: 0.2.0
+Summary: Work with MySQL databases asynchronously, and in context.
+Home-page: https://pypi.org/project/mysql-context-manager/
+License: MIT
+Author: IdoKendo
+Author-email: ryuusuke@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyMySQL (>=1.0,<2.0)
+Requires-Dist: aiomysql (>=0.1.1,<0.2.0)
+Requires-Dist: databases (>=0.7,<0.8)
+Project-URL: Repository, https://github.com/IdoKendo/mysql-context-manager
+Description-Content-Type: text/markdown
+
+# MySQL Context Manager
+
+ > Work with MySQL based databases asynchronously, using a context manager.
+
+[![PyPI version][pypi-image]][pypi-url]
+[![PyPI downloads][downloads-image]][downloads-url]
+[![Build status][build-image]][build-url]
+[![Code coverage][coverage-image]][coverage-url]
+[![Codacy Badge][codacy-iamge]][codacy-url]
+[![Support Python versions][versions-image]][versions-url]
+[![Code style: Black][black-image]][black-url]
+
+## Getting started
+
+You can [get `mysql-context-manager` from PyPI](https://pypi.org/project/mysql-context-manager/),
+which means you can install it with pip easily:
+
+```bash
+python -m pip install mysql-context-manager
+```
+
+## Example
+
+```py
+from mysql_context_manager import MysqlConnector
+
+async with MysqlConnector(hostname="localhost") as conn:
+    results = await conn.query("select username from users where is_bender = 1 order by username asc;")
+assert results[0]["username"] == "Aang"
+assert results[1]["username"] == "Katara"
+assert results[2]["username"] == "Toph"
+```
+
+## Example using SQLAlchemy
+
+```py
+from mysql_context_manager import MysqlConnector
+import sqlalchemy
+from sqlalchemy.dialects import mysql
+
+metadata = sqlalchemy.MetaData()
+
+users = sqlalchemy.Table(
+    "users",
+    metadata,
+    sqlalchemy.Column("user_id", mysql.INTEGER(), autoincrement=True, nullable=False),
+    sqlalchemy.Column("username", mysql.VARCHAR(length=128), nullable=False),
+    sqlalchemy.Column("is_bender", mysql.SMALLINT(), autoincrement=False, nullable=True),
+    sqlalchemy.PrimaryKeyConstraint("user_id"),
+    mysql_default_charset="utf8mb4",
+    mysql_engine="InnoDB",
+)
+
+async with MysqlConnector(hostname="localhost") as conn:
+    results = await conn.query(users.select().where(users.c.username == "Aang"))
+assert results[0]["username"] == "Aang"
+assert results[0]["is_bender"] == 1
+```
+
+## Changelog
+
+Refer to the [CHANGELOG.rst](CHANGELOG.rst) file.
+
+<!-- Badges -->
+
+[pypi-image]: https://img.shields.io/pypi/v/mysql-context-manager
+[pypi-url]: https://pypi.org/project/mysql-context-manager/
+[downloads-image]: https://img.shields.io/pypi/dm/mysql-context-manager.svg
+[downloads-url]: https://pypistats.org/packages/mysql-context-manager
+[build-image]: https://github.com/idokendo/mysql-context-manager/actions/workflows/build.yaml/badge.svg
+[build-url]: https://github.com/idokendo/mysql-context-manager/actions/workflows/build.yaml
+[coverage-image]: https://codecov.io/gh/idokendo/mysql-context-manager/branch/main/graph/badge.svg
+[coverage-url]: https://codecov.io/gh/idokendo/mysql-context-manager
+[versions-image]: https://img.shields.io/pypi/pyversions/mysql-context-manager
+[versions-url]: https://pypi.org/project/mysql-context-manager/
+[codacy-iamge]: https://app.codacy.com/project/badge/Grade/59b037e21c4e4c6ea5a51f4a693dc267
+[codacy-url]: https://www.codacy.com/gh/IdoKendo/mysql-context-manager/dashboard
+[black-image]: https://img.shields.io/badge/code%20style-Black-000000.svg
+[black-url]: https://github.com/psf/black
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['mysql_context_manager']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyMySQL>=1.0.2,<2.0.0', 'aiomysql>=0.1.1,<0.2.0', 'databases>=0.6.2,<0.7.0']
-
-setup_kwargs = {
-    'name': 'mysql-context-manager',
-    'version': '0.1.6',
-    'description': 'Work with MySQL databases asynchronously, and in context.',
-    'long_description': '# MySQL Context Manager\n\n > Work with MySQL based databases asynchronously, using a context manager.\n\n[![PyPI version][pypi-image]][pypi-url]\n[![PyPI downloads][downloads-image]][downloads-url]\n[![Build status][build-image]][build-url]\n[![Code coverage][coverage-image]][coverage-url]\n[![Codacy Badge][codacy-iamge]][codacy-url]\n[![Support Python versions][versions-image]][versions-url]\n[![Code style: Black][black-image]][black-url]\n\n## Getting started\n\nYou can [get `mysql-context-manager` from PyPI](https://pypi.org/project/mysql-context-manager/),\nwhich means you can install it with pip easily:\n\n```bash\npython -m pip install mysql-context-manager\n```\n\n## Example\n\n```py\nfrom mysql_context_manager import MysqlConnector\n\nasync with MysqlConnector(hostname="localhost") as conn:\n    results = await conn.query("select username from users where is_bender = 1 order by username asc;")\nassert results[0]["username"] == "Aang"\nassert results[1]["username"] == "Katara"\nassert results[2]["username"] == "Toph"\n```\n\n## Example using SQLAlchemy\n\n```py\nfrom mysql_context_manager import MysqlConnector\nimport sqlalchemy\nfrom sqlalchemy.dialects import mysql\n\nmetadata = sqlalchemy.MetaData()\n\nusers = sqlalchemy.Table(\n    "users",\n    metadata,\n    sqlalchemy.Column("user_id", mysql.INTEGER(), autoincrement=True, nullable=False),\n    sqlalchemy.Column("username", mysql.VARCHAR(length=128), nullable=False),\n    sqlalchemy.Column("is_bender", mysql.SMALLINT(), autoincrement=False, nullable=True),\n    sqlalchemy.PrimaryKeyConstraint("user_id"),\n    mysql_default_charset="utf8mb4",\n    mysql_engine="InnoDB",\n)\n\nasync with MysqlConnector(hostname="localhost") as conn:\n    results = await conn.query(users.select().where(users.c.username == "Aang"))\nassert results[0]["username"] == "Aang"\nassert results[0]["is_bender"] == 1\n```\n\n## Changelog\n\nRefer to the [CHANGELOG.rst](CHANGELOG.rst) file.\n\n<!-- Badges -->\n\n[pypi-image]: https://img.shields.io/pypi/v/mysql-context-manager\n[pypi-url]: https://pypi.org/project/mysql-context-manager/\n[downloads-image]: https://img.shields.io/pypi/dm/mysql-context-manager.svg\n[downloads-url]: https://pypistats.org/packages/mysql-context-manager\n[build-image]: https://github.com/idokendo/mysql-context-manager/actions/workflows/build.yaml/badge.svg\n[build-url]: https://github.com/idokendo/mysql-context-manager/actions/workflows/build.yaml\n[coverage-image]: https://codecov.io/gh/idokendo/mysql-context-manager/branch/main/graph/badge.svg\n[coverage-url]: https://codecov.io/gh/idokendo/mysql-context-manager\n[versions-image]: https://img.shields.io/pypi/pyversions/mysql-context-manager\n[versions-url]: https://pypi.org/project/mysql-context-manager/\n[codacy-iamge]: https://app.codacy.com/project/badge/Grade/59b037e21c4e4c6ea5a51f4a693dc267\n[codacy-url]: https://www.codacy.com/gh/IdoKendo/mysql-context-manager/dashboard\n[black-image]: https://img.shields.io/badge/code%20style-Black-000000.svg\n[black-url]: https://github.com/psf/black\n',
-    'author': 'IdoKendo',
-    'author_email': 'ryuusuke@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://pypi.org/project/mysql-context-manager/',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

