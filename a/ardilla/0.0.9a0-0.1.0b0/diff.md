# Comparing `tmp/ardilla-0.0.9a0.tar.gz` & `tmp/ardilla-0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ardilla-0.0.9a0.tar", last modified: Sun May 14 03:47:37 2023, max compression
+gzip compressed data, was "ardilla-0.1.0b0.tar", last modified: Wed May 24 16:47:54 2023, max compression
```

## Comparing `ardilla-0.0.9a0.tar` & `ardilla-0.1.0b0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 03:47:37.170175 ardilla-0.0.9a0/
--rw-rw-rw-   0        0        0     1084 2023-05-08 03:28:44.000000 ardilla-0.0.9a0/LICENCE
--rw-rw-rw-   0        0        0     4317 2023-05-14 03:47:37.168179 ardilla-0.0.9a0/PKG-INFO
--rw-rw-rw-   0        0        0     3488 2023-05-14 03:10:46.000000 ardilla-0.0.9a0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 03:47:37.064632 ardilla-0.0.9a0/ardilla/
--rw-rw-rw-   0        0        0      136 2023-05-13 16:32:48.000000 ardilla-0.0.9a0/ardilla/__init__.py
--rw-rw-rw-   0        0        0     3223 2023-05-14 02:51:15.000000 ardilla-0.0.9a0/ardilla/abc.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:47:37.151177 ardilla-0.0.9a0/ardilla/asyncio/
--rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.0.9a0/ardilla/asyncio/__init__.py
--rw-rw-rw-   0        0        0      468 2023-05-13 04:14:11.000000 ardilla-0.0.9a0/ardilla/asyncio/abc.py
--rw-rw-rw-   0        0        0     4960 2023-05-14 03:45:11.000000 ardilla-0.0.9a0/ardilla/asyncio/crud.py
--rw-rw-rw-   0        0        0     1292 2023-05-13 16:09:59.000000 ardilla-0.0.9a0/ardilla/asyncio/engine.py
--rw-rw-rw-   0        0        0     4754 2023-05-14 03:42:44.000000 ardilla-0.0.9a0/ardilla/crud.py
--rw-rw-rw-   0        0        0     1661 2023-05-13 16:03:58.000000 ardilla-0.0.9a0/ardilla/engine.py
--rw-rw-rw-   0        0        0      294 2023-05-13 22:19:12.000000 ardilla-0.0.9a0/ardilla/errors.py
--rw-rw-rw-   0        0        0      217 2023-05-13 16:26:28.000000 ardilla-0.0.9a0/ardilla/logging.py
--rw-rw-rw-   0        0        0     1686 2023-05-13 22:01:58.000000 ardilla-0.0.9a0/ardilla/models.py
--rw-rw-rw-   0        0        0     3106 2023-05-14 03:42:51.000000 ardilla-0.0.9a0/ardilla/queries.py
--rw-rw-rw-   0        0        0     2153 2023-05-13 22:00:57.000000 ardilla-0.0.9a0/ardilla/schemas.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:47:37.134195 ardilla-0.0.9a0/ardilla.egg-info/
--rw-rw-rw-   0        0        0     4317 2023-05-14 03:47:36.000000 ardilla-0.0.9a0/ardilla.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      509 2023-05-14 03:47:36.000000 ardilla-0.0.9a0/ardilla.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 03:47:36.000000 ardilla-0.0.9a0/ardilla.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2023-05-14 03:47:36.000000 ardilla-0.0.9a0/ardilla.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-14 03:47:36.000000 ardilla-0.0.9a0/ardilla.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1047 2023-05-14 03:46:32.000000 ardilla-0.0.9a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 03:47:37.170175 ardilla-0.0.9a0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 03:47:37.164178 ardilla-0.0.9a0/tests/
--rw-rw-rw-   0        0        0     5748 2023-05-14 02:49:39.000000 ardilla-0.0.9a0/tests/test_async.py
--rw-rw-rw-   0        0        0      567 2023-05-12 03:32:46.000000 ardilla-0.0.9a0/tests/test_models.py
--rw-rw-rw-   0        0        0     5491 2023-05-14 02:45:01.000000 ardilla-0.0.9a0/tests/test_sync.py
+drwxrwxrwx   0        0        0        0 2023-05-24 16:47:54.008825 ardilla-0.1.0b0/
+-rw-rw-rw-   0        0        0     1084 2023-05-21 21:48:03.000000 ardilla-0.1.0b0/LICENCE
+-rw-rw-rw-   0        0        0     4977 2023-05-24 16:47:54.005833 ardilla-0.1.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0     4097 2023-05-21 21:45:45.000000 ardilla-0.1.0b0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 16:47:53.915642 ardilla-0.1.0b0/ardilla/
+-rw-rw-rw-   0        0        0      145 2023-05-22 03:22:06.000000 ardilla-0.1.0b0/ardilla/__init__.py
+-rw-rw-rw-   0        0        0     3537 2023-05-23 20:17:34.000000 ardilla-0.1.0b0/ardilla/abc.py
+drwxrwxrwx   0        0        0        0 2023-05-24 16:47:53.990647 ardilla-0.1.0b0/ardilla/asyncio/
+-rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.1.0b0/ardilla/asyncio/__init__.py
+-rw-rw-rw-   0        0        0      468 2023-05-13 04:14:11.000000 ardilla-0.1.0b0/ardilla/asyncio/abc.py
+-rw-rw-rw-   0        0        0     4708 2023-05-22 17:26:54.000000 ardilla-0.1.0b0/ardilla/asyncio/crud.py
+-rw-rw-rw-   0        0        0     1674 2023-05-22 17:25:44.000000 ardilla-0.1.0b0/ardilla/asyncio/engine.py
+-rw-rw-rw-   0        0        0     4435 2023-05-22 17:23:08.000000 ardilla-0.1.0b0/ardilla/crud.py
+-rw-rw-rw-   0        0        0     3211 2023-05-24 16:39:49.000000 ardilla-0.1.0b0/ardilla/engine.py
+-rw-rw-rw-   0        0        0      316 2023-05-18 15:14:26.000000 ardilla-0.1.0b0/ardilla/errors.py
+-rw-rw-rw-   0        0        0     2420 2023-05-24 16:44:41.000000 ardilla-0.1.0b0/ardilla/fields.py
+-rw-rw-rw-   0        0        0      222 2023-05-22 17:13:39.000000 ardilla-0.1.0b0/ardilla/logging.py
+-rw-rw-rw-   0        0        0     2802 2023-05-24 16:05:39.000000 ardilla-0.1.0b0/ardilla/models.py
+-rw-rw-rw-   0        0        0     1082 2023-05-18 22:33:35.000000 ardilla-0.1.0b0/ardilla/ordering.py
+-rw-rw-rw-   0        0        0     6456 2023-05-24 16:04:50.000000 ardilla-0.1.0b0/ardilla/queries.py
+-rw-rw-rw-   0        0        0     4858 2023-05-22 17:12:54.000000 ardilla-0.1.0b0/ardilla/schemas.py
+drwxrwxrwx   0        0        0        0 2023-05-24 16:47:53.974640 ardilla-0.1.0b0/ardilla.egg-info/
+-rw-rw-rw-   0        0        0     4977 2023-05-24 16:47:53.000000 ardilla-0.1.0b0/ardilla.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-05-24 16:47:53.000000 ardilla-0.1.0b0/ardilla.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 16:47:53.000000 ardilla-0.1.0b0/ardilla.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-05-24 16:47:53.000000 ardilla-0.1.0b0/ardilla.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-24 16:47:53.000000 ardilla-0.1.0b0/ardilla.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1124 2023-05-24 16:46:07.000000 ardilla-0.1.0b0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 16:47:54.008825 ardilla-0.1.0b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 16:47:54.001830 ardilla-0.1.0b0/tests/
+-rw-rw-rw-   0        0        0     8304 2023-05-22 16:57:24.000000 ardilla-0.1.0b0/tests/test_async.py
+-rw-rw-rw-   0        0        0     1909 2023-05-18 02:32:05.000000 ardilla-0.1.0b0/tests/test_models.py
+-rw-rw-rw-   0        0        0     8383 2023-05-22 16:34:39.000000 ardilla-0.1.0b0/tests/test_sync.py
```

### Comparing `ardilla-0.0.9a0/LICENCE` & `ardilla-0.1.0b0/LICENCE`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.9a0/PKG-INFO` & `ardilla-0.1.0b0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,28 @@
-Metadata-Version: 2.1
-Name: ardilla
-Version: 0.0.9a0
-Summary: Ardilla ORM. Easy to use, fast to implement, with sync and async flavors
-Author-email: ChrisDewa <chrisdewa@duck.com>
-Project-URL: Homepage, https://github.com/chrisdewa/ardilla
-Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: async
-Provides-Extra: examples
-Provides-Extra: dev
-License-File: LICENCE
-
 # ardilla
 
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) 
+[![Downloads](https://static.pepy.tech/badge/ardilla/month)](https://pepy.tech/project/ardilla) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) 
 
 <div style="text-align:center">
   <img 
     src="https://images-ext-2.discordapp.net/external/sxevZWKA4UIZWNyt352zkHLGWrUMw_PV_jGWLXGPh_I/https/repository-images.githubusercontent.com/638528340/a0238c4e-addf-4130-a0fe-9a458be6cdc9?width=200&height=150"
   >  
 </div>
 
 Ardilla (pronounced *ahr-dee-yah*) means "**SQ**uirre**L**" in spanish.
 
-A very simple library to quickly add SQLite to your program.
-It leverages pydantic for data validation and modeling.
-It comes in sync (sqlite3) and async (aiosqlite) flavors.
+This library aims to be a simple way to add an SQLite database and 
+basic C.R.U.D. methods to python applications.
+It uses pydantic for data validation and supports a sync engine as well
+as an async (aiosqlite) version.
 
 ## Who and what is this for:
 
-For developers seeking a simple and straightforward way to incorporate a SQLite database into their applications, our library is an excellent option. It offers a user-friendly solution that is both fast and easy to use.
-
-While this library may not be suitable for those who require more complex querying and intricate relationships, it excels in its simplicity and ease of implementation.
+This library is well suited for developers seeking to incorporate SQLite into their python applications to use simple C.R.U.D. methods.
+It excels in its simplicity and ease of implementation while it may not be suitable for those who require more complex querying, intricate relationships or top performance.
 
 For developers who desire more advanced features, there are other libraries available, such as [tortoise-orm](https://github.com/tortoise/tortoise-orm), [sqlalchemy](https://github.com/sqlalchemy/sqlalchemy), [pony](https://github.com/ponyorm/pony) or [peewee](https://github.com/coleifer/peewee).
 
 
 ## install
 Install lastest release from PyPi
 ```bash
@@ -70,43 +49,54 @@
 engine = Engine('db.sqlite3')
 
 class User(Model):
     id: int = Field(primary=True, autoincrement=True) 
     name: str
     age: int
 
-user_crud = engine.crud(User)
+crud = engine.crud(User)
 
 def main():
-    engine.setup() # creates tables 
     # get or none
-    user = user_crud.get_or_none(id=1)
+    user = crud.get_or_none(id=1) # user with id of 1
     # get or create
-    user2, was_created = user_crud.get_or_create(id=2, name='chris', age=35)
+    user2, was_created = crud.get_or_create(id=2, name='chris', age=35)
+    # get many
+    users = crud.get_many(name='chris') # all users named chris
     # save one
     user3 = User(id=3, name='moni', age=35)
-    user_crud.save_one(user3)
+    user.age += 1 # it's her birthday
+    crud.save_one(user3)
     # save many
-    user_crud.save_many(user, user2, user3)
-    # get many
-    users = user_crud.get_many(age=35)
+    crud.save_many(user, user2, user3)
 ```
 
 ## Supported CRUD methods:
 - `crud.insert` Inserts a record, rises errors if there's a conflict
 - `crud.insert_or_ignore` Inserts a record or silently ignores if it already exists
 - `crud.save_one` upserts an object
 - `crud.save_many` upserts many objects
 - `crud.get_all` equivalent to `SELECT * FROM tablename`
 - `crud.get_many` returns all the objects that meet criteria
 - `crud.get_or_create` returns an tuple of the object and a bool, True if the object was newly created
 - `crud.get_or_none` Returns the first object meeting criteria if any
 - `crud.delete_one` Deletes an object
 - `crud.delete_many` Deletes many objects
 
+
+## Examples:
+
+- A simple [FastAPI](https://github.com/chrisdewa/ardilla/blob/master/examples/fastapi_app.py) application
+- A reputation based discord [bot](https://github.com/chrisdewa/ardilla/blob/master/examples/rep_discord_bot.py)
+- [basic usage](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage.py)
+- [basic usage with foreign keys](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage_fk.py)
+
 ## To-dos
 
 - [x] Add testing
 - [x] Add a schema generator 
+- [X] Add filtering
+- [X] Add limiting
 - [ ] Docstring everything using Google format
+- [ ] Start a changelog when out of alpha
 - [ ] Add proper documentation
-  - propper as in a site with how to use
+  - propper as in a site with how to use
```

### Comparing `ardilla-0.0.9a0/README.md` & `ardilla-0.1.0b0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,50 @@
+Metadata-Version: 2.1
+Name: ardilla
+Version: 0.1.0b0
+Summary: Ardilla ORM. Easy to use, fast to implement, with sync and async flavors
+Author-email: ChrisDewa <chrisdewa@duck.com>
+Project-URL: Homepage, https://github.com/chrisdewa/ardilla
+Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: async
+Provides-Extra: examples
+Provides-Extra: dev
+License-File: LICENCE
+
 # ardilla
 
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) 
+[![Downloads](https://static.pepy.tech/badge/ardilla/month)](https://pepy.tech/project/ardilla) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) 
 
 <div style="text-align:center">
   <img 
     src="https://images-ext-2.discordapp.net/external/sxevZWKA4UIZWNyt352zkHLGWrUMw_PV_jGWLXGPh_I/https/repository-images.githubusercontent.com/638528340/a0238c4e-addf-4130-a0fe-9a458be6cdc9?width=200&height=150"
   >  
 </div>
 
 Ardilla (pronounced *ahr-dee-yah*) means "**SQ**uirre**L**" in spanish.
 
-A very simple library to quickly add SQLite to your program.
-It leverages pydantic for data validation and modeling.
-It comes in sync (sqlite3) and async (aiosqlite) flavors.
+This library aims to be a simple way to add an SQLite database and 
+basic C.R.U.D. methods to python applications.
+It uses pydantic for data validation and supports a sync engine as well
+as an async (aiosqlite) version.
 
 ## Who and what is this for:
 
-For developers seeking a simple and straightforward way to incorporate a SQLite database into their applications, our library is an excellent option. It offers a user-friendly solution that is both fast and easy to use.
-
-While this library may not be suitable for those who require more complex querying and intricate relationships, it excels in its simplicity and ease of implementation.
+This library is well suited for developers seeking to incorporate SQLite into their python applications to use simple C.R.U.D. methods.
+It excels in its simplicity and ease of implementation while it may not be suitable for those who require more complex querying, intricate relationships or top performance.
 
 For developers who desire more advanced features, there are other libraries available, such as [tortoise-orm](https://github.com/tortoise/tortoise-orm), [sqlalchemy](https://github.com/sqlalchemy/sqlalchemy), [pony](https://github.com/ponyorm/pony) or [peewee](https://github.com/coleifer/peewee).
 
 
 ## install
 Install lastest release from PyPi
 ```bash
@@ -49,43 +71,54 @@
 engine = Engine('db.sqlite3')
 
 class User(Model):
     id: int = Field(primary=True, autoincrement=True) 
     name: str
     age: int
 
-user_crud = engine.crud(User)
+crud = engine.crud(User)
 
 def main():
-    engine.setup() # creates tables 
     # get or none
-    user = user_crud.get_or_none(id=1)
+    user = crud.get_or_none(id=1) # user with id of 1
     # get or create
-    user2, was_created = user_crud.get_or_create(id=2, name='chris', age=35)
+    user2, was_created = crud.get_or_create(id=2, name='chris', age=35)
+    # get many
+    users = crud.get_many(name='chris') # all users named chris
     # save one
     user3 = User(id=3, name='moni', age=35)
-    user_crud.save_one(user3)
+    user.age += 1 # it's her birthday
+    crud.save_one(user3)
     # save many
-    user_crud.save_many(user, user2, user3)
-    # get many
-    users = user_crud.get_many(age=35)
+    crud.save_many(user, user2, user3)
 ```
 
 ## Supported CRUD methods:
 - `crud.insert` Inserts a record, rises errors if there's a conflict
 - `crud.insert_or_ignore` Inserts a record or silently ignores if it already exists
 - `crud.save_one` upserts an object
 - `crud.save_many` upserts many objects
 - `crud.get_all` equivalent to `SELECT * FROM tablename`
 - `crud.get_many` returns all the objects that meet criteria
 - `crud.get_or_create` returns an tuple of the object and a bool, True if the object was newly created
 - `crud.get_or_none` Returns the first object meeting criteria if any
 - `crud.delete_one` Deletes an object
 - `crud.delete_many` Deletes many objects
 
+
+## Examples:
+
+- A simple [FastAPI](https://github.com/chrisdewa/ardilla/blob/master/examples/fastapi_app.py) application
+- A reputation based discord [bot](https://github.com/chrisdewa/ardilla/blob/master/examples/rep_discord_bot.py)
+- [basic usage](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage.py)
+- [basic usage with foreign keys](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage_fk.py)
+
 ## To-dos
 
 - [x] Add testing
 - [x] Add a schema generator 
+- [X] Add filtering
+- [X] Add limiting
 - [ ] Docstring everything using Google format
+- [ ] Start a changelog when out of alpha
 - [ ] Add proper documentation
   - propper as in a site with how to use
```

### Comparing `ardilla-0.0.9a0/ardilla/abc.py` & `ardilla-0.1.0b0/ardilla/abc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,87 @@
 import sqlite3
-from typing import Generic, Self, Literal, TypeVar, Type
+from typing import Literal, TypeVar, Protocol, Optional
 from abc import abstractmethod, ABC
 from sqlite3 import Row
 
 from .errors import MissingEngine
 from .models import M, Model as BaseModel
 
 E = TypeVar("E")  # Engine Type
 
 
+class ContextCursorProtocol(Protocol):
+    def __init__(self, con: sqlite3.Connection):
+        ...
+
+    def __enter__(self) -> sqlite3.Cursor:
+        ...
+
+    def __exit__(self, *_) -> None:
+        ...
+
+
 class AbstractEngine(ABC):
     """This just provides autocompletition across the library"""
+
     schemas: set[str]
+
     @abstractmethod
     def __enter__(self) -> sqlite3.Connection:
         ...
-    abstractmethod
-    def cursor(self, con: sqlite3.Connection) -> sqlite3.Cursor:
+
+    @abstractmethod
+    def __exit__(self, *_) -> None:
+        ...
+
+    @abstractmethod
+    def cursor(self, con: sqlite3.Connection) -> ContextCursorProtocol:
         ...
 
 
 class CrudABC(ABC):
+    __slots__ = (
+        "engine",
+        "tablename",
+        "Model",
+        "columns",
+    )
+
     engine: AbstractEngine
-    def __init__(self, Model: type[M], engine: E | None = None) -> None:
+
+    def __init__(self, Model: type[M], engine: Optional[AbstractEngine] = None) -> None:
         if engine:
             self.engine = engine
 
         self.Model = Model
         if Model.__schema__:
             self.engine.schemas.add(Model.__schema__)
         self.tablename = Model.__tablename__
         self.columns = tuple(Model.__fields__)
 
-    def __new__(cls, Model: type[M], engine: E | None = None) -> Self:
+    def __new__(cls, Model: type[M], engine: Optional[AbstractEngine] = None):
         if not issubclass(Model, BaseModel):
             raise TypeError("Model param has to be a subclass of model")
 
         cls_engine = getattr(cls, "engine", None)
 
         if engine is None and cls_engine is None:
-            # if not isinstance(engine, Engine) and not isinstance(cls_engine, Engine):
             raise MissingEngine(
                 "Missing engine. Set the engine at instance level (Crud(Model, engine))"
                 "or at class level (Crud.engine = engine)"
             )
         return super().__new__(cls)
 
-    def _row2obj(self, row: Row, rowid: int = None) -> M:
+    def _row2obj(self, row: Row, rowid: Optional[int] = None) -> BaseModel:
         """
         Args:
             row: the sqlite row
             rowid: the rowid of the row.
                 If passed it means it comes from an insert function
-                
+
         """
         [*keys] = self.Model.__fields__
         if rowid is None:
             rowid, *vals = row
         else:
             vals = list(row)
         data = {k: v for k, v in zip(keys, vals)}
@@ -80,27 +105,23 @@
 
     # Read
     @abstractmethod
     def get_all(self) -> list[M]:
         pass
 
     @abstractmethod
-    def get_many(self, **kws) -> list[M]:
+    def get_many(self, order_by: Optional[dict[str, str]] = None, limit: Optional[int] = None, **kws) -> list[M]:
         pass
 
     @abstractmethod
     def get_or_create(self, **kws) -> tuple[M, bool]:
         pass
 
     @abstractmethod
-    def get_or_none(self, **kws) -> M | None:
-        pass
-
-    @abstractmethod
-    def _get_or_none_any(self, many: bool, **kws) -> list[M] | M | None:
+    def get_or_none(self, **kws) -> Optional[M]:
         pass
 
     # Update
     @abstractmethod
     def save_one(self, obj: M) -> Literal[True]:
         pass
```

### Comparing `ardilla-0.0.9a0/ardilla/asyncio/crud.py` & `ardilla-0.1.0b0/ardilla/asyncio/crud.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,39 @@
-from typing import Literal, Generic, Self
+from typing import Literal, Generic, Optional, Union
 
 import aiosqlite
 from aiosqlite import Row
 
-from ..errors import BadQueryError, QueryExecutionError
+from ..errors import QueryExecutionError
 from ..models import M
 from ..abc import CrudABC
-from ..logging import log, log_query
+from ..logging import log
 from .. import queries
 
 from .abc import AbstractAsyncEngine
 
+
 class AsyncCrud(CrudABC, Generic[M]):
     """Abstracts CRUD actions for model associated tables"""
 
     engine: AbstractAsyncEngine
 
-    async def _get_or_none_any(self, many: bool, **kws) -> list[M] | M | None:
-        """
-        private helper to the get_or_none queries.
-        if param "many" is true it will return a list of matches else will return only one record
-        """
-        q, vals = queries.for_get_or_none_any(self.tablename, many, kws)
-        log_query(q, vals)
+    async def get_or_none(self, **kws) -> Optional[M]:
+        """Gets an object from a database or None if not found"""
+        q, vals = queries.for_get_or_none(self.tablename, kws)
         async with self.engine as con:
             async with con.execute(q, vals) as cur:
-                if many:
-                    rows: list[Row] = await cur.fetchall()
-                    return [self._row2obj(row) for row in rows]
-
-                else:
-                    row: Row | None = await cur.fetchone()
-                    if row:
-                        return self._row2obj(row)
-        return
-
-    async def get_or_none(self, **kws) -> M | None:
-        """Gets an object from a database or None if not found"""
-        return await self._get_or_none_any(many=False, **kws)
+                row: Union[Row, None] = await cur.fetchone()
+                if row:
+                    return self._row2obj(row)
+        return None
 
     async def _do_insert(self, ignore: bool = False, returning: bool = True, /, **kws):
         q, vals = queries.for_do_insert(self.tablename, ignore, returning, kws)
-        log_query(q, vals)
+
         async with self.engine as con:
             con = await self.engine.connect()
             cur = None
             try:
                 cur = await con.execute(q, vals)
             except aiosqlite.IntegrityError as e:
                 raise QueryExecutionError(str(e))
@@ -65,69 +53,81 @@
         Returns:
             Model | None: Returns a model only if newly created
         Rises:
             ardilla.error.QueryExecutionError: if there's a conflict when inserting the record
         """
         return await self._do_insert(False, True, **kws)
 
-    async def insert_or_ignore(self, **kws) -> M | None:
+    async def insert_or_ignore(self, **kws) -> Optional[M]:
         """inserts a the object of a row or ignores it if it already exists"""
         return await self._do_insert(True, True, **kws)
 
     async def get_or_create(self, **kws) -> tuple[M, bool]:
         """Returns object and bool indicated if it was created or not"""
         created = False
         result = await self.get_or_none(**kws)
         if not result:
             result = await self.insert_or_ignore(**kws)
             created = True
         return result, created
 
     async def get_all(self) -> list[M]:
         """Gets all objects from the database"""
+        q = f"SELECT rowid, * FROM {self.tablename};"
+        log.debug(f"Querying: {q}")
+
         async with self.engine as con:
-            async with con.execute(f"SELECT rowid, * FROM {self.tablename};") as cur:
+            async with con.execute(q) as cur:
                 return [self._row2obj(row) for row in await cur.fetchall()]
 
-    async def get_many(self, **kws) -> list[M]:
+    async def get_many(
+        self,
+        order_by: Optional[dict[str, str]] = None,
+        limit: Optional[int] = None,
+        **kws,
+    ) -> list[M]:
         """Returns a list of objects that have the given conditions"""
-        return await self._get_or_none_any(many=True, **kws)
+        q, vals = queries.for_get_many(self.Model, order_by=order_by, limit=limit, kws=kws)
+        async with self.engine as con:
+            async with con.execute(q, vals) as cur:
+                rows: list[Row] = await cur.fetchall()
+                return [self._row2obj(row) for row in rows]
 
     async def save_one(self, obj: M) -> Literal[True]:
         """Saves one object to the database"""
         q, vals = queries.for_save_one(obj)
-        log_query(q, vals)
+
         async with self.engine as con:
             await con.execute(q, vals)
             await con.commit()
         return True
 
     async def save_many(self, *objs: M) -> Literal[True]:
         """Saves all the given objects to the database"""
         q, vals = queries.for_save_many(objs)
-        log_query(q, vals)
+
         async with self.engine as con:
             await con.executemany(q, vals)
             await con.commit()
 
         return True
 
     async def delete_one(self, obj: M) -> Literal[True]:
         """
         Deletes the object from the database (won't delete the actual object)
         queries only by the Model id fields (fields suffixed with 'id')
         """
         q, vals = queries.for_delete_one(obj)
-        log_query(q, vals)
+
         async with self.engine as con:
             await con.execute(q, vals)
             await con.commit()
         return True
 
     async def delete_many(self, *objs: M) -> Literal[True]:
         q, vals = queries.for_delete_many(objs)
-        
+
         async with self.engine as con:
             await con.execute(q, vals)
             await con.commit()
 
-        return 
+
```

### Comparing `ardilla-0.0.9a0/ardilla/asyncio/engine.py` & `ardilla-0.1.0b0/ardilla/asyncio/engine.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,31 +3,37 @@
 
 from .crud import AsyncCrud
 from ..models import M
 from ..engine import Engine
 
 from .abc import AbstractAsyncEngine
 
-
 class AsyncEngine(Engine, AbstractAsyncEngine):
+    def __init__(self, path: str, enable_foreing_keys: bool = False, single_connection: bool = False):
+        if single_connection is True:
+            raise NotImplementedError('The async engine does not support single connection for now')
+        super().__init__(path, enable_foreing_keys, single_connection)
+    
     async def connect(self) -> aiosqlite.Connection:
         con = await aiosqlite.connect(self.path)
         con.row_factory = aiosqlite.Row
         return con
 
     async def __aenter__(self) -> aiosqlite.Connection:
-        self.con = await self.connect()
-        return self.con
+        self.acon = await self.connect()
+        if self.enable_foreing_keys:
+            await self.acon.execute('PRAGMA foreign_keys = ON;')
+            
+        return self.acon
 
     async def __aexit__(self, *_):
-        await self.con.close()
+        await self.acon.close()
 
     async def setup(self):
         async with self as con:
-            await con.execute("PRAGMA foreign_keys = ON;")
             for table in self.schemas:
                 await con.execute(table)
                 self.tables_created.add(table)
             await con.commit()
     
     def crud(self, Model: type[M]) -> AsyncCrud[M]:
         """This function runs synchronously"""
```

### Comparing `ardilla-0.0.9a0/ardilla/crud.py` & `ardilla-0.1.0b0/ardilla/crud.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,124 +1,126 @@
 import sqlite3
 from sqlite3 import Row
-from typing import Literal, Generic, Self
+from typing import Literal, Generic, Optional, Union
 
 from .abc import CrudABC, AbstractEngine
-from .models import M, Model as BaseModel
-from .errors import BadQueryError, QueryExecutionError
+from .models import M
+from .errors import QueryExecutionError
+from .logging import log
 from . import queries
 
+
 class Crud(CrudABC, Generic[M]):
     """Abstracts CRUD actions for model associated tables"""
 
     engine: AbstractEngine
 
-    def _get_or_none_any(self, many: bool, **kws) -> list[M] | M | None:
-        """
-        private helper to the get_or_none queries.
-        if param "many" is true it will return a list of matches else will return only one record
-        """
-        q, vals = queries.for_get_or_none_any(self.tablename, many, kws)
-        with self.engine as con:
-            with self.engine.cursor(con) as cur:
-                cur: sqlite3.Cursor
-                cur.execute(q, vals)
-                if many:
-                    rows: list[Row] = cur.fetchall()
-                    return [self._row2obj(row) for row in rows]
-                else:
-                    row: Row | None = cur.fetchone()
-                    if row:
-                        return self._row2obj(row)
-
     def _do_insert(
-        self, ignore: bool = False, returning: bool = True, /, **kws
-    ) -> M | None:
+        self,
+        ignore: bool = False,
+        returning: bool = True,
+        /,
+        **kws,
+    ) -> Optional[M]:
         q, vals = queries.for_do_insert(self.tablename, ignore, returning, kws)
 
         with self.engine as con:
             with self.engine.cursor(con) as cur:
-                cur: sqlite3.Cursor
                 try:
                     cur.execute(q, vals)
                 except sqlite3.IntegrityError as e:
                     raise QueryExecutionError(str(e))
 
                 row = cur.fetchone()
                 con.commit()
                 if returning and row:
                     return self._row2obj(row, cur.lastrowid)
 
-    def get_or_none(self, **kws) -> M | None:
+        return None
+
+    def get_or_none(self, **kws) -> Optional[M]:
         """Gets an object from a database or None if not found"""
-        return self._get_or_none_any(many=False, **kws)
+        q, vals = queries.for_get_or_none(self.tablename, kws)
+        with self.engine as con:
+            ctxcur = self.engine.cursor(con)
+            with ctxcur as cur:
+                cur.execute(q, vals)
+                row: Union[Row, None] = cur.fetchone()
+                if row:
+                    return self._row2obj(row)
+        return None
 
-    def insert(self, **kws):
+    def insert(self, **kws) -> M:
         """
         Inserts a record into the database.
         Returns:
-            Model | None: Returns a model only if newly created
+            Model: Creates a new entry in the database and returns the object
         Rises:
             ardilla.error.QueryExecutionError: if there's a conflict when inserting the record
         """
         return self._do_insert(False, True, **kws)
 
-    def insert_or_ignore(self, **kws) -> M | None:
+    def insert_or_ignore(self, **kws) -> Optional[M]:
         """inserts a the object of a row or ignores it if it already exists"""
         return self._do_insert(True, True, **kws)
 
     def get_or_create(self, **kws) -> tuple[M, bool]:
         """Returns object and bool indicated if it was created or not"""
         created = False
         result = self.get_or_none(**kws)
         if not result:
             result = self.insert_or_ignore(**kws)
             created = True
         return result, created
 
     def get_all(self) -> list[M]:
         """Gets all objects from the database"""
-        q = f"SELECT rowid, * FROM {self.tablename};"
-        with self.engine as con:
-            with self.engine.cursor(con) as cur:
-                cur: sqlite3.Cursor
-                cur.execute(q)
-                results: list[Row] = cur.fetchall()
-                return [self._row2obj(res) for res in results]
-            
+        return self.get_many()
 
-    def get_many(self, **kws) -> list[M]:
+    def get_many(
+        self,
+        order_by: Optional[dict[str, str]] = None,
+        limit: Optional[int] = None,
+        **kws,
+    ) -> list[M]:
         """Returns a list of objects that have the given conditions"""
-        return self._get_or_none_any(many=True, **kws)
+        q, vals = queries.for_get_many(self.Model, order_by=order_by, limit=limit, kws=kws)
+        with self.engine as con:
+            ctxcur = self.engine.cursor(con)
+            with ctxcur as cur:
+                cur.execute(q, vals)
+                rows: list[Row] = cur.fetchall()
+                return [self._row2obj(row) for row in rows]
 
     def save_one(self, obj: M) -> Literal[True]:
         """Saves one object to the database"""
         q, vals = queries.for_save_one(obj)
+
         with self.engine as con:
             con.execute(q, vals)
             con.commit()
         return True
 
-    def save_many(self, *objs: M) -> Literal[True]:
+    def save_many(self, *objs: tuple[M]) -> Literal[True]:
         """Saves all the given objects to the database"""
         q, vals = queries.for_save_many(objs)
         with self.engine as con:
             con.executemany(q, vals)
             con.commit()
 
         return True
 
     def delete_one(self, obj: M) -> Literal[True]:
         """
         Deletes the object from the database (won't delete the actual object)
-        If the object has a PK field or the rowid setup, those will be 
-        used to locate the obj and delete it. 
+        If the object has a PK field or the rowid setup, those will be
+        used to locate the obj and delete it.
         If not, this function will delete any object like this one.
         """
-        
+
         q, vals = queries.for_delete_one(obj)
         with self.engine as con:
             con.execute(q, vals)
             con.commit()
 
         return True
```

### Comparing `ardilla-0.0.9a0/ardilla.egg-info/PKG-INFO` & `ardilla-0.1.0b0/ardilla.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 Metadata-Version: 2.1
 Name: ardilla
-Version: 0.0.9a0
+Version: 0.1.0b0
 Summary: Ardilla ORM. Easy to use, fast to implement, with sync and async flavors
 Author-email: ChrisDewa <chrisdewa@duck.com>
 Project-URL: Homepage, https://github.com/chrisdewa/ardilla
 Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.10
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: async
 Provides-Extra: examples
 Provides-Extra: dev
 License-File: LICENCE
 
 # ardilla
 
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) 
+[![Downloads](https://static.pepy.tech/badge/ardilla/month)](https://pepy.tech/project/ardilla) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) 
 
 <div style="text-align:center">
   <img 
     src="https://images-ext-2.discordapp.net/external/sxevZWKA4UIZWNyt352zkHLGWrUMw_PV_jGWLXGPh_I/https/repository-images.githubusercontent.com/638528340/a0238c4e-addf-4130-a0fe-9a458be6cdc9?width=200&height=150"
   >  
 </div>
 
 Ardilla (pronounced *ahr-dee-yah*) means "**SQ**uirre**L**" in spanish.
 
-A very simple library to quickly add SQLite to your program.
-It leverages pydantic for data validation and modeling.
-It comes in sync (sqlite3) and async (aiosqlite) flavors.
+This library aims to be a simple way to add an SQLite database and 
+basic C.R.U.D. methods to python applications.
+It uses pydantic for data validation and supports a sync engine as well
+as an async (aiosqlite) version.
 
 ## Who and what is this for:
 
-For developers seeking a simple and straightforward way to incorporate a SQLite database into their applications, our library is an excellent option. It offers a user-friendly solution that is both fast and easy to use.
-
-While this library may not be suitable for those who require more complex querying and intricate relationships, it excels in its simplicity and ease of implementation.
+This library is well suited for developers seeking to incorporate SQLite into their python applications to use simple C.R.U.D. methods.
+It excels in its simplicity and ease of implementation while it may not be suitable for those who require more complex querying, intricate relationships or top performance.
 
 For developers who desire more advanced features, there are other libraries available, such as [tortoise-orm](https://github.com/tortoise/tortoise-orm), [sqlalchemy](https://github.com/sqlalchemy/sqlalchemy), [pony](https://github.com/ponyorm/pony) or [peewee](https://github.com/coleifer/peewee).
 
 
 ## install
 Install lastest release from PyPi
 ```bash
@@ -70,43 +71,54 @@
 engine = Engine('db.sqlite3')
 
 class User(Model):
     id: int = Field(primary=True, autoincrement=True) 
     name: str
     age: int
 
-user_crud = engine.crud(User)
+crud = engine.crud(User)
 
 def main():
-    engine.setup() # creates tables 
     # get or none
-    user = user_crud.get_or_none(id=1)
+    user = crud.get_or_none(id=1) # user with id of 1
     # get or create
-    user2, was_created = user_crud.get_or_create(id=2, name='chris', age=35)
+    user2, was_created = crud.get_or_create(id=2, name='chris', age=35)
+    # get many
+    users = crud.get_many(name='chris') # all users named chris
     # save one
     user3 = User(id=3, name='moni', age=35)
-    user_crud.save_one(user3)
+    user.age += 1 # it's her birthday
+    crud.save_one(user3)
     # save many
-    user_crud.save_many(user, user2, user3)
-    # get many
-    users = user_crud.get_many(age=35)
+    crud.save_many(user, user2, user3)
 ```
 
 ## Supported CRUD methods:
 - `crud.insert` Inserts a record, rises errors if there's a conflict
 - `crud.insert_or_ignore` Inserts a record or silently ignores if it already exists
 - `crud.save_one` upserts an object
 - `crud.save_many` upserts many objects
 - `crud.get_all` equivalent to `SELECT * FROM tablename`
 - `crud.get_many` returns all the objects that meet criteria
 - `crud.get_or_create` returns an tuple of the object and a bool, True if the object was newly created
 - `crud.get_or_none` Returns the first object meeting criteria if any
 - `crud.delete_one` Deletes an object
 - `crud.delete_many` Deletes many objects
 
+
+## Examples:
+
+- A simple [FastAPI](https://github.com/chrisdewa/ardilla/blob/master/examples/fastapi_app.py) application
+- A reputation based discord [bot](https://github.com/chrisdewa/ardilla/blob/master/examples/rep_discord_bot.py)
+- [basic usage](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage.py)
+- [basic usage with foreign keys](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage_fk.py)
+
 ## To-dos
 
 - [x] Add testing
 - [x] Add a schema generator 
+- [X] Add filtering
+- [X] Add limiting
 - [ ] Docstring everything using Google format
+- [ ] Start a changelog when out of alpha
 - [ ] Add proper documentation
   - propper as in a site with how to use
```

### Comparing `ardilla-0.0.9a0/pyproject.toml` & `ardilla-0.1.0b0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ardilla"
-version = "0.0.9-alpha"
+version = "0.1.0-beta"
 authors = [
   { name="ChrisDewa", email="chrisdewa@duck.com" },
 ]
 description = "Ardilla ORM. Easy to use, fast to implement, with sync and async flavors"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 classifiers = [
   "Intended Audience :: Developers",
   "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
-  "Development Status :: 3 - Alpha",
+  "Development Status :: 4 - Beta",
 ]
 dependencies = [
   "pydantic==1.10.7",
 ]
 
 [project.optional-dependencies]
 async = ["aiosqlite==0.19.0",]
 examples = ["fastapi-0.95.1", "uvicorn-0.22.0"]
 dev = [
-  "pytest==7.3.1", 
-  "pytest-asyncio==0.21.0", 
-  "black==23.3.0"
+  "pytest==7.3.1", # testing
+  "pytest-asyncio==0.21.0", # testing async
+  "black==23.3.0" # formating
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/chrisdewa/ardilla"
 "Bug Tracker" = "https://github.com/chrisdewa/ardilla/issues"
```

### Comparing `ardilla-0.0.9a0/tests/test_sync.py` & `ardilla-0.1.0b0/tests/test_sync.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,39 @@
+import random
 import sqlite3
 from contextlib import contextmanager
 from pathlib import Path
 
-import pytest
 
 from ardilla import Engine, Model, Crud
 from ardilla.errors import QueryExecutionError
 from pydantic import Field
 
+from ardilla.fields import ForeignField
+
 
 path = Path(__file__).parent
-db = path / "testdb.sqlite"
+db = path / "testdb_sync.sqlite"
 
 
 class User(Model):
     id: int = Field(primary=True, autoincrement=True)
     name: str
     age: int
 
 
 @contextmanager
 def cleanup():
     try:
         db.unlink(missing_ok=True)
-        engine = Engine(db)
+        engine = Engine(db, single_connection=True)
         crud = engine.crud(User)
-        engine.setup()
         yield crud
     finally:
+        engine.close()
         db.unlink(missing_ok=True)
 
 
 @contextmanager
 def query():
     try:
         con = sqlite3.connect(db)
@@ -57,15 +59,16 @@
 """
 
 
 def test_insert():
     with cleanup() as crud:
         u = crud.insert(id=1, name="chris", age=35)
         assert u is not None, "User wasn't created as expected"
-
+        assert u.__rowid__ is not None, "Created user did not have __rowid__ set"
+        assert u.__rowid__ == 1, "Created User did not have correct __rowid__ "
         try:
             crud.insert(id=1, name="chris", age=35)
         except QueryExecutionError:
             pass
         else:
             raise Exception("QueryExcecutionError should have been rised")
 
@@ -86,14 +89,27 @@
         with query() as cur:
             cur.execute("SELECT * FROM user;")
             res = cur.fetchall()
 
         assert len(res) == 1, "Incorrect number of users in the database"
 
 
+def test_save_one_rowid():
+    with cleanup() as crud:
+        chris = crud.insert(id=1, name="chris", age=35)
+        chris.name = 'chris_is_alt'
+        crud.save_one(chris)
+        
+
+        with query() as cur:
+            cur.execute("SELECT * FROM user;")
+            res = cur.fetchall()
+
+        assert len(res) == 1, "Incorrect number of users in the database"
+
 def test_save_many():
     with cleanup() as crud:
         chris = User(id=1, name="chris", age=35)
         moni = User(id=2, name="moni", age=36)
         elena = User(id=3, name="elena", age=5)
         crud.save_many(chris, moni, elena)
 
@@ -125,14 +141,34 @@
         crud.save_many(u1, u2, u3, u4, u5)
 
         users = crud.get_many(name="chris")
 
         assert len(users) == 3, "Incorrect number of users returned"
         assert all(u.__rowid__ for u in users), 'User objects did not get their rowid populated'
 
+def test_get_many_with_limit():
+    users = [User(id=n, name='chris', age=random.randint(1, 27)) for n in range(50)]
+    with cleanup() as crud:
+        crud.save_many(*users)
+        users = crud.get_many(limit=5)
+        assert len(users) == 5
+
+def test_get_many_with_ordering():
+    with cleanup() as crud:
+        crud.insert(id=1, name='chris', age=3)
+        crud.insert(id=2, name='chris', age=2)
+        crud.insert(id=3, name='chris', age=5)
+        crud.insert(id=4, name='chris', age=1)
+        crud.insert(id=5, name='chris', age=4)
+        
+        users = crud.get_many(order_by={'age': 'desc'})
+        
+        sorted_users = sorted(users, key=lambda u: u.age, reverse=True)
+        assert users == sorted_users
+
 
 def test_get_or_create():
     with cleanup() as crud:
         elena = User(id=1, name="elena", age=5)
         crud.save_one(elena)
 
         u, c = crud.get_or_create(name="fran", age=1)
@@ -160,14 +196,40 @@
         moni = User(id=2, name="moni", age=36)
         elena = User(id=3, name="elena", age=5)
         crud.save_many(chris, moni, elena)
         crud.delete_one(moni)
         users = crud.get_all()
         assert len(users) == 2, "Delete one didn't delete the correct amount of users"
 
+class Foo(Model):
+    a: str
+    b: int
+
+def test_delete_one_without_ids():
+    db.unlink(missing_ok=True)
+    engine = Engine(db)
+    crud = engine.crud(Foo)
+    try:
+        for i, l in enumerate('abcdef',1):
+            crud.insert(a=l, b=i)
+            
+        to_del = [
+            Foo(a='b', b=2),
+            Foo(a='c', b=3),
+            Foo(a='d', b=4),
+        ]
+        for obj in to_del:
+            crud.delete_one(obj)
+        
+        foos = crud.get_all()
+        assert len(foos) == 3, 'Mismatch beween expected and found after delete_many'
+        
+    finally:
+        db.unlink(missing_ok=True)
+    
 
 def test_delete_many_by_id():
     with cleanup() as crud:
         users = [
             User(id=n, name='chris', age=n)
             for n in range(10)
         ]
@@ -191,7 +253,37 @@
         crud.delete_many(*users[:-1])
         
         users = crud.get_all()
         
         
         assert len(users) == 1, "Delete many didn't delete the correct amount of users"
 
+
+def test_foreign_keys():
+    db = path / 'sync_test.sqlite'
+    db.unlink(missing_ok=True)
+    engine = Engine(db, enable_foreing_keys=True)
+    
+    class Guild(Model):
+        id: int = Field(pk=True, auto=True)
+        name: str
+        
+    class User(Model):
+        id: int = Field(pk=True, auto=True)
+        name: str
+        guild_id: int = ForeignField(references=Guild, on_delete=ForeignField.CASCADE)
+    
+    gcrud = engine.crud(Guild)
+    ucrud = engine.crud(User)
+    
+    ga = gcrud.insert(name='guild a')
+    gb = gcrud.insert(name='guild b')
+    for guild in [ga, gb]:
+        for n in range(5):
+            ucrud.insert(name=f'user {n}', guild_id=guild.id)
+    
+    users = ucrud.get_all()
+    assert len(users) == 10
+    gcrud.delete_one(ga)
+    users = ucrud.get_all()
+    assert len(users) == 5 
+    db.unlink(missing_ok=True)
```

