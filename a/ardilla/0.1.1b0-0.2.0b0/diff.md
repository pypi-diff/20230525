# Comparing `tmp/ardilla-0.1.1b0.tar.gz` & `tmp/ardilla-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ardilla-0.1.1b0.tar", last modified: Thu May 25 05:24:03 2023, max compression
+gzip compressed data, was "ardilla-0.2.0b0.tar", last modified: Thu May 25 18:23:30 2023, max compression
```

## Comparing `ardilla-0.1.1b0.tar` & `ardilla-0.2.0b0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 05:24:03.792829 ardilla-0.1.1b0/
--rw-rw-rw-   0        0        0     1084 2023-05-21 21:48:03.000000 ardilla-0.1.1b0/LICENCE
--rw-rw-rw-   0        0        0     4999 2023-05-25 05:24:03.790829 ardilla-0.1.1b0/PKG-INFO
--rw-rw-rw-   0        0        0     4097 2023-05-25 02:59:53.000000 ardilla-0.1.1b0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 05:24:03.701814 ardilla-0.1.1b0/ardilla/
--rw-rw-rw-   0        0        0      145 2023-05-22 03:22:06.000000 ardilla-0.1.1b0/ardilla/__init__.py
--rw-rw-rw-   0        0        0     3537 2023-05-23 20:17:34.000000 ardilla-0.1.1b0/ardilla/abc.py
-drwxrwxrwx   0        0        0        0 2023-05-25 05:24:03.775817 ardilla-0.1.1b0/ardilla/asyncio/
--rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.1.1b0/ardilla/asyncio/__init__.py
--rw-rw-rw-   0        0        0      468 2023-05-13 04:14:11.000000 ardilla-0.1.1b0/ardilla/asyncio/abc.py
--rw-rw-rw-   0        0        0     4708 2023-05-22 17:26:54.000000 ardilla-0.1.1b0/ardilla/asyncio/crud.py
--rw-rw-rw-   0        0        0     1674 2023-05-22 17:25:44.000000 ardilla-0.1.1b0/ardilla/asyncio/engine.py
--rw-rw-rw-   0        0        0     4435 2023-05-22 17:23:08.000000 ardilla-0.1.1b0/ardilla/crud.py
--rw-rw-rw-   0        0        0     3211 2023-05-24 16:39:49.000000 ardilla-0.1.1b0/ardilla/engine.py
--rw-rw-rw-   0        0        0      316 2023-05-18 15:14:26.000000 ardilla-0.1.1b0/ardilla/errors.py
--rw-rw-rw-   0        0        0     2455 2023-05-25 03:48:27.000000 ardilla-0.1.1b0/ardilla/fields.py
--rw-rw-rw-   0        0        0      222 2023-05-22 17:13:39.000000 ardilla-0.1.1b0/ardilla/logging.py
--rw-rw-rw-   0        0        0     2802 2023-05-24 16:05:39.000000 ardilla-0.1.1b0/ardilla/models.py
--rw-rw-rw-   0        0        0     1082 2023-05-18 22:33:35.000000 ardilla-0.1.1b0/ardilla/ordering.py
--rw-rw-rw-   0        0        0     6456 2023-05-24 16:04:50.000000 ardilla-0.1.1b0/ardilla/queries.py
--rw-rw-rw-   0        0        0     5128 2023-05-25 03:52:26.000000 ardilla-0.1.1b0/ardilla/schemas.py
-drwxrwxrwx   0        0        0        0 2023-05-25 05:24:03.760809 ardilla-0.1.1b0/ardilla.egg-info/
--rw-rw-rw-   0        0        0     4999 2023-05-25 05:24:03.000000 ardilla-0.1.1b0/ardilla.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-05-25 05:24:03.000000 ardilla-0.1.1b0/ardilla.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 05:24:03.000000 ardilla-0.1.1b0/ardilla.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      179 2023-05-25 05:24:03.000000 ardilla-0.1.1b0/ardilla.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 05:24:03.000000 ardilla-0.1.1b0/ardilla.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1181 2023-05-25 05:17:58.000000 ardilla-0.1.1b0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 05:24:03.793340 ardilla-0.1.1b0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 05:24:03.787830 ardilla-0.1.1b0/tests/
--rw-rw-rw-   0        0        0     8304 2023-05-22 16:57:24.000000 ardilla-0.1.1b0/tests/test_async.py
--rw-rw-rw-   0        0        0     1909 2023-05-18 02:32:05.000000 ardilla-0.1.1b0/tests/test_models.py
--rw-rw-rw-   0        0        0     8383 2023-05-22 16:34:39.000000 ardilla-0.1.1b0/tests/test_sync.py
+drwxrwxrwx   0        0        0        0 2023-05-25 18:23:30.856564 ardilla-0.2.0b0/
+-rw-rw-rw-   0        0        0     1084 2023-05-21 21:48:03.000000 ardilla-0.2.0b0/LICENCE
+-rw-rw-rw-   0        0        0     5298 2023-05-25 18:23:30.853564 ardilla-0.2.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0     4396 2023-05-25 05:34:17.000000 ardilla-0.2.0b0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 18:23:30.755033 ardilla-0.2.0b0/ardilla/
+-rw-rw-rw-   0        0        0      145 2023-05-22 03:22:06.000000 ardilla-0.2.0b0/ardilla/__init__.py
+-rw-rw-rw-   0        0        0     3537 2023-05-23 20:17:34.000000 ardilla-0.2.0b0/ardilla/abc.py
+drwxrwxrwx   0        0        0        0 2023-05-25 18:23:30.836562 ardilla-0.2.0b0/ardilla/asyncio/
+-rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.2.0b0/ardilla/asyncio/__init__.py
+-rw-rw-rw-   0        0        0      468 2023-05-13 04:14:11.000000 ardilla-0.2.0b0/ardilla/asyncio/abc.py
+-rw-rw-rw-   0        0        0     8082 2023-05-25 17:33:42.000000 ardilla-0.2.0b0/ardilla/asyncio/crud.py
+-rw-rw-rw-   0        0        0     2398 2023-05-25 18:19:51.000000 ardilla-0.2.0b0/ardilla/asyncio/engine.py
+-rw-rw-rw-   0        0        0     7762 2023-05-25 17:31:21.000000 ardilla-0.2.0b0/ardilla/crud.py
+-rw-rw-rw-   0        0        0     4983 2023-05-25 18:16:14.000000 ardilla-0.2.0b0/ardilla/engine.py
+-rw-rw-rw-   0        0        0      316 2023-05-18 15:14:26.000000 ardilla-0.2.0b0/ardilla/errors.py
+-rw-rw-rw-   0        0        0     2586 2023-05-25 17:47:32.000000 ardilla-0.2.0b0/ardilla/fields.py
+-rw-rw-rw-   0        0        0      222 2023-05-22 17:13:39.000000 ardilla-0.2.0b0/ardilla/logging.py
+-rw-rw-rw-   0        0        0     2885 2023-05-25 17:39:33.000000 ardilla-0.2.0b0/ardilla/models.py
+-rw-rw-rw-   0        0        0     1082 2023-05-18 22:33:35.000000 ardilla-0.2.0b0/ardilla/ordering.py
+-rw-rw-rw-   0        0        0     6456 2023-05-24 16:04:50.000000 ardilla-0.2.0b0/ardilla/queries.py
+-rw-rw-rw-   0        0        0     5181 2023-05-25 17:28:48.000000 ardilla-0.2.0b0/ardilla/schemas.py
+drwxrwxrwx   0        0        0        0 2023-05-25 18:23:30.819551 ardilla-0.2.0b0/ardilla.egg-info/
+-rw-rw-rw-   0        0        0     5298 2023-05-25 18:23:30.000000 ardilla-0.2.0b0/ardilla.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-05-25 18:23:30.000000 ardilla-0.2.0b0/ardilla.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 18:23:30.000000 ardilla-0.2.0b0/ardilla.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      208 2023-05-25 18:23:30.000000 ardilla-0.2.0b0/ardilla.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 18:23:30.000000 ardilla-0.2.0b0/ardilla.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1215 2023-05-25 18:22:15.000000 ardilla-0.2.0b0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 18:23:30.856564 ardilla-0.2.0b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 18:23:30.848563 ardilla-0.2.0b0/tests/
+-rw-rw-rw-   0        0        0     8304 2023-05-22 16:57:24.000000 ardilla-0.2.0b0/tests/test_async.py
+-rw-rw-rw-   0        0        0     1909 2023-05-18 02:32:05.000000 ardilla-0.2.0b0/tests/test_models.py
+-rw-rw-rw-   0        0        0     8383 2023-05-22 16:34:39.000000 ardilla-0.2.0b0/tests/test_sync.py
```

### Comparing `ardilla-0.1.1b0/LICENCE` & `ardilla-0.2.0b0/LICENCE`

 * *Files identical despite different names*

### Comparing `ardilla-0.1.1b0/PKG-INFO` & `ardilla-0.2.0b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ardilla
-Version: 0.1.1b0
+Version: 0.2.0b0
 Summary: Ardilla ORM. Easy to use, fast to implement, with sync and async flavors
 Author-email: ChrisDewa <chrisdewa@duck.com>
 Project-URL: Homepage, https://github.com/chrisdewa/ardilla
 Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
@@ -19,15 +19,16 @@
 Provides-Extra: examples
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENCE
 
 # ardilla
 
-[![Downloads](https://static.pepy.tech/badge/ardilla/month)](https://pepy.tech/project/ardilla) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) 
+[![Downloads](https://static.pepy.tech/badge/ardilla/month)](https://pepy.tech/project/ardilla) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) [![Documentation Status](https://readthedocs.org/projects/ardilla/badge/?version=latest)](https://ardilla.readthedocs.io/en/latest/?badge=latest)
+
 
 <div style="text-align:center">
   <img 
     src="https://images-ext-2.discordapp.net/external/sxevZWKA4UIZWNyt352zkHLGWrUMw_PV_jGWLXGPh_I/https/repository-images.githubusercontent.com/638528340/a0238c4e-addf-4130-a0fe-9a458be6cdc9?width=200&height=150"
   >  
 </div>
 
@@ -42,14 +43,20 @@
 
 This library is well suited for developers seeking to incorporate SQLite into their python applications to use simple C.R.U.D. methods.
 It excels in its simplicity and ease of implementation while it may not be suitable for those who require more complex querying, intricate relationships or top performance.
 
 For developers who desire more advanced features, there are other libraries available, such as [tortoise-orm](https://github.com/tortoise/tortoise-orm), [sqlalchemy](https://github.com/sqlalchemy/sqlalchemy), [pony](https://github.com/ponyorm/pony) or [peewee](https://github.com/coleifer/peewee).
 
 
+## Links
+
+Find Ardilla's source code [here](https://github.com/chrisdewa/ardilla)
+
+Documentation can be accessed [here](http://ardilla.rtfd.io/)
+
 ## install
 Install lastest release from PyPi
 ```bash
 pip install -U ardilla
 pip install -U ardilla[async]
 pip install -U ardilla[dev]
 ```
```

### Comparing `ardilla-0.1.1b0/README.md` & `ardilla-0.2.0b0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # ardilla
 
-[![Downloads](https://static.pepy.tech/badge/ardilla/month)](https://pepy.tech/project/ardilla) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) 
+[![Downloads](https://static.pepy.tech/badge/ardilla/month)](https://pepy.tech/project/ardilla) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) [![Documentation Status](https://readthedocs.org/projects/ardilla/badge/?version=latest)](https://ardilla.readthedocs.io/en/latest/?badge=latest)
+
 
 <div style="text-align:center">
   <img 
     src="https://images-ext-2.discordapp.net/external/sxevZWKA4UIZWNyt352zkHLGWrUMw_PV_jGWLXGPh_I/https/repository-images.githubusercontent.com/638528340/a0238c4e-addf-4130-a0fe-9a458be6cdc9?width=200&height=150"
   >  
 </div>
 
@@ -19,14 +20,20 @@
 
 This library is well suited for developers seeking to incorporate SQLite into their python applications to use simple C.R.U.D. methods.
 It excels in its simplicity and ease of implementation while it may not be suitable for those who require more complex querying, intricate relationships or top performance.
 
 For developers who desire more advanced features, there are other libraries available, such as [tortoise-orm](https://github.com/tortoise/tortoise-orm), [sqlalchemy](https://github.com/sqlalchemy/sqlalchemy), [pony](https://github.com/ponyorm/pony) or [peewee](https://github.com/coleifer/peewee).
 
 
+## Links
+
+Find Ardilla's source code [here](https://github.com/chrisdewa/ardilla)
+
+Documentation can be accessed [here](http://ardilla.rtfd.io/)
+
 ## install
 Install lastest release from PyPi
 ```bash
 pip install -U ardilla
 pip install -U ardilla[async]
 pip install -U ardilla[dev]
 ```
```

### Comparing `ardilla-0.1.1b0/ardilla/abc.py` & `ardilla-0.2.0b0/ardilla/abc.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.1.1b0/ardilla/asyncio/engine.py` & `ardilla-0.2.0b0/ardilla/asyncio/engine.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,43 +4,65 @@
 from .crud import AsyncCrud
 from ..models import M
 from ..engine import Engine
 
 from .abc import AbstractAsyncEngine
 
 class AsyncEngine(Engine, AbstractAsyncEngine):
+    """Async Engine that uses `aiosqlite.Connection` and `aiosqlite.Cursor`
+    Inhetits attributes from `Engine`
+    """
     def __init__(self, path: str, enable_foreing_keys: bool = False, single_connection: bool = False):
         if single_connection is True:
             raise NotImplementedError('The async engine does not support single connection for now')
         super().__init__(path, enable_foreing_keys, single_connection)
     
     async def connect(self) -> aiosqlite.Connection:
+        """
+        Stablishes a connection to the database
+        Returns:
+            The connection
+        """
         con = await aiosqlite.connect(self.path)
         con.row_factory = aiosqlite.Row
         return con
 
     async def __aenter__(self) -> aiosqlite.Connection:
+        """Stablishes the connection and if specified enables foreign keys pragma
+
+        Returns:
+            The connection
+        """
         self.acon = await self.connect()
         if self.enable_foreing_keys:
             await self.acon.execute('PRAGMA foreign_keys = ON;')
             
         return self.acon
 
     async def __aexit__(self, *_):
+        """Closes the connection"""
         await self.acon.close()
 
     async def setup(self):
+        """Creates the tables setup by the engine
+        """
         async with self as con:
             for table in self.schemas:
                 await con.execute(table)
                 self.tables_created.add(table)
             await con.commit()
     
     def crud(self, Model: type[M]) -> AsyncCrud[M]:
-        """This function runs synchronously"""
+        """
+        This function runs synchronously and works exactly like `Engine.crud` but
+        returns an instance of `ardilla.asyncio.crud.AsyncCrud` instead of `ardilla.crud.Crud`
+        
+        Returns:
+            The async Crud for the given model
+        """
         crud = self._cruds.setdefault(Model, AsyncCrud(Model, self))
         if Model.__schema__ not in self.tables_created:
             with self as con:
                 con.execute(Model.__schema__)
                 con.commit()
             self.tables_created.add(Model.__schema__)
         return crud
```

### Comparing `ardilla-0.1.1b0/ardilla/fields.py` & `ardilla-0.2.0b0/ardilla/fields.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
+from typing import Any
 from pydantic import Field
 from ardilla import Model
 
 class _ForeignFieldMaker():
     """
     Helper class to generate foreing key field constrains.
     
     Intead of instantiating this class the developer should use 
     the already instantiated `ardilla.fields.ForeignKey`
     instead of directly instantiating this class.
     
-    Class Attributes
-        NO_ACTION - The database won't take action. This most likely will result in errors
-        RESTRICT - The app will not be able to delete the foreing row unless there's no related child elements left
-        SET_NULL - The app will set the child to Null if the parent is deleted
-        SET_DEFAULT - Returns the value of this field to the default of the child when the parent is deleted or updated
-        CASCADE - If the parent gets deleted or updated the child follows
-            
+    Attributes:
+        NO_ACTION (str): (class attribute) The database won't take action. This most likely will result in errors
+        RESTRICT (str): (class attribute) The app will not be able to delete the foreing row unless there's no related child elements left
+        SET_NULL (str): (class attribute) The app will set the child to Null if the parent is deleted
+        SET_DEFAULT (str): (class attribute) Returns the value of this field to the default of the child when the parent is deleted or updated
+        CASCADE (str): (class attribute) If the parent gets deleted or updated the child follows  
         
     """
     NO_ACTION = 'NO ACTION'
     RESTRICT = 'RESTRICT'
     SET_NULL = 'SET NULL'
     SET_DEFAULT = 'SET DEFAULT'
     CASCADE = 'CASCADE'
@@ -27,28 +27,28 @@
     def __call__(
         self,
         *,
         references: type[Model],
         on_delete: str = NO_ACTION, 
         on_update: str = NO_ACTION,
         **kws,
-    ):
+    ) -> Any:
         """
         Args:
             references (type[Model]):
                 The model this foreign key points to
-            on_delete (str) defaults to 'NO ACTION':
+            on_delete (str): defaults to 'NO ACTION'
                 what happens when the referenced row gets deleted
-            on_update (str) defaults to 'NO ACTION':
+            on_update (str): defaults to 'NO ACTION'
                 what happens when the referenced row gets updated
         Returns:
             A `pydantic.Field` with extra metadata for the schema creation
-        raises:
-            KeyError if the referenced value is not a type of model
-            ValueError if the referenced model does not have a primary key or has not yet been instantiated
+        Raises:
+            KeyError: if the referenced value is not a type of model
+            ValueError: if the referenced model does not have a primary key or has not yet been instantiated
         """
         if not issubclass(references, Model):
             raise TypeError('The referenced type must be a subclass of ardilla.Model')
         fk = getattr(references, '__pk__', None)
         tablename = getattr(references, '__tablename__')
         
         if not fk:
```

### Comparing `ardilla-0.1.1b0/ardilla/models.py` & `ardilla-0.2.0b0/ardilla/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,29 +10,31 @@
 
 
 class Model(BaseModel):
     """
     The base model representing SQLite tables
     Inherits directly from pydantic.BaseModel
     
-    Additional Attributes:
-        __rowid__ (int | None): when an object is returned by a query it will 
+    Attributes:
+        __rowid__ (int | None): (class attribute) when an object is returned by a query it will 
             contain the rowid field that can be used for update and deletion.
-        __pk__ (str | None): Holds the primary key column name of the table
-        __tablename__ (str): the name of the table in the database
-        __schema__(str): the schema for the table.
+        __pk__ (str | None): (class attribute) Holds the primary key column name of the table
+        __tablename__ (str): (class attribute) the name of the table in the database
+        __schema__(str): the (class attribute) schema for the table.
         
-    Usage Example:
+    Example:
+        ```py
         from ardilla import Model, Field
         # Field is actually pydantic.Field but it's imported here for the convenience of the developer
         
         class User(Model):
             __tablename__ = 'users' # by default the tablename is just the model's name in lowercase
             id: int = Field(primary=True) # sets this field as the primary key
             name: str
+        ```
     """
     __rowid__: Optional[int] = PrivateAttr(default=None)
     __pk__: Optional[str]  # tells the model which key to idenfity as primary
     __tablename__: str  # will default to the lowercase name of the subclass
     __schema__: str  # best effort will be made if it's missing
     # there's no support for constrains or foreign fields yet but you can
     # define your own schema to support them
```

### Comparing `ardilla-0.1.1b0/ardilla/ordering.py` & `ardilla-0.2.0b0/ardilla/ordering.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.1.1b0/ardilla/queries.py` & `ardilla-0.2.0b0/ardilla/queries.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.1.1b0/ardilla/schemas.py` & `ardilla-0.2.0b0/ardilla/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 """
 variables and functions here are used to generate and work with the Model's schemas
 """
 import re
-from typing import Optional
+from typing import Optional, Union
 from datetime import datetime, date, time
 from pydantic import BaseModel, Json
 from .errors import ModelIntegrityError
 
 
 SCHEMA_TEMPLATE: str = "CREATE TABLE IF NOT EXISTS {tablename} (\n{fields}\n);"
 
+SQLFieldType = Union[int,float,str,bool,datetime,bytes,date,time]
 
 FIELD_MAPPING: dict[type, str] = {
     int: "INTEGER",
     float: "REAL",
     str: "TEXT",
     bool: "INTEGER",
     datetime: "DATETIME",
     bytes: "BLOB",
     date: "DATE",
     time: "TIME",
-    Json: "TEXT",
 }
 
 AUTOFIELDS = {
     int: " AUTOINCREMENT",
     datetime: " DEFAULT CURRENT_TIMESTAMP",
     date: " DEFAULT CURRENT_DATE",
     time: " DEFAULT CURRENT_TIME"
 }
 
-
 def get_tablename(model: type[BaseModel]) -> str:
     """returns the tablename of a model either from the attribute __tablenam__
     or from the lowercase model's name
 
     Args:
         model (type[BaseModel]): the model
```

### Comparing `ardilla-0.1.1b0/ardilla.egg-info/PKG-INFO` & `ardilla-0.2.0b0/ardilla.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ardilla
-Version: 0.1.1b0
+Version: 0.2.0b0
 Summary: Ardilla ORM. Easy to use, fast to implement, with sync and async flavors
 Author-email: ChrisDewa <chrisdewa@duck.com>
 Project-URL: Homepage, https://github.com/chrisdewa/ardilla
 Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
@@ -19,15 +19,16 @@
 Provides-Extra: examples
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENCE
 
 # ardilla
 
-[![Downloads](https://static.pepy.tech/badge/ardilla/month)](https://pepy.tech/project/ardilla) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) 
+[![Downloads](https://static.pepy.tech/badge/ardilla/month)](https://pepy.tech/project/ardilla) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) [![Documentation Status](https://readthedocs.org/projects/ardilla/badge/?version=latest)](https://ardilla.readthedocs.io/en/latest/?badge=latest)
+
 
 <div style="text-align:center">
   <img 
     src="https://images-ext-2.discordapp.net/external/sxevZWKA4UIZWNyt352zkHLGWrUMw_PV_jGWLXGPh_I/https/repository-images.githubusercontent.com/638528340/a0238c4e-addf-4130-a0fe-9a458be6cdc9?width=200&height=150"
   >  
 </div>
 
@@ -42,14 +43,20 @@
 
 This library is well suited for developers seeking to incorporate SQLite into their python applications to use simple C.R.U.D. methods.
 It excels in its simplicity and ease of implementation while it may not be suitable for those who require more complex querying, intricate relationships or top performance.
 
 For developers who desire more advanced features, there are other libraries available, such as [tortoise-orm](https://github.com/tortoise/tortoise-orm), [sqlalchemy](https://github.com/sqlalchemy/sqlalchemy), [pony](https://github.com/ponyorm/pony) or [peewee](https://github.com/coleifer/peewee).
 
 
+## Links
+
+Find Ardilla's source code [here](https://github.com/chrisdewa/ardilla)
+
+Documentation can be accessed [here](http://ardilla.rtfd.io/)
+
 ## install
 Install lastest release from PyPi
 ```bash
 pip install -U ardilla
 pip install -U ardilla[async]
 pip install -U ardilla[dev]
 ```
```

### Comparing `ardilla-0.1.1b0/ardilla.egg-info/SOURCES.txt` & `ardilla-0.2.0b0/ardilla.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ardilla-0.1.1b0/pyproject.toml` & `ardilla-0.2.0b0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ardilla"
-version = "0.1.1-beta"
+version = "0.2.0-beta"
 authors = [
   { name="ChrisDewa", email="chrisdewa@duck.com" },
 ]
 description = "Ardilla ORM. Easy to use, fast to implement, with sync and async flavors"
 readme = "README.md"
 requires-python = ">=3.9"
 
@@ -34,12 +34,13 @@
   "pytest==7.3.1", # testing
   "pytest-asyncio==0.21.0", # testing async
   "black==23.3.0", # formating
 ]
 docs = [
   "mkdocs==1.4.3",
   "jinja2<3.1.0",
+  "mkdocstrings[python]==0.21.2"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/chrisdewa/ardilla"
 "Bug Tracker" = "https://github.com/chrisdewa/ardilla/issues"
```

### Comparing `ardilla-0.1.1b0/tests/test_async.py` & `ardilla-0.2.0b0/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.1.1b0/tests/test_models.py` & `ardilla-0.2.0b0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.1.1b0/tests/test_sync.py` & `ardilla-0.2.0b0/tests/test_sync.py`

 * *Files identical despite different names*

