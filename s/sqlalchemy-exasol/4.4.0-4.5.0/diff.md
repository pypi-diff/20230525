# Comparing `tmp/sqlalchemy_exasol-4.4.0.tar.gz` & `tmp/sqlalchemy_exasol-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_exasol-4.4.0.tar", max compression
+gzip compressed data, was "sqlalchemy_exasol-4.5.0.tar", max compression
```

## Comparing `sqlalchemy_exasol-4.4.0.tar` & `sqlalchemy_exasol-4.5.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    14389 2023-05-16 06:24:15.278817 sqlalchemy_exasol-4.4.0/CHANGELOG.rst
--rw-r--r--   0        0        0     1395 2023-05-16 06:24:15.278817 sqlalchemy_exasol-4.4.0/LICENSE
--rw-r--r--   0        0        0     5119 2023-05-16 06:24:15.278817 sqlalchemy_exasol-4.4.0/README.rst
--rw-r--r--   0        0        0     3341 2023-05-16 06:24:15.334818 sqlalchemy_exasol-4.4.0/pyproject.toml
--rw-r--r--   0        0        0      413 2023-05-16 06:24:15.334818 sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/__init__.py
--rw-r--r--   0        0        0    33000 2023-05-16 06:24:15.334818 sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/base.py
--rw-r--r--   0        0        0      165 2023-05-16 06:24:15.334818 sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/constraints.py
--rw-r--r--   0        0        0    12880 2023-05-16 06:24:15.334818 sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/pyodbc.py
--rw-r--r--   0        0        0     7522 2023-05-16 06:24:15.334818 sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/requirements.py
--rw-r--r--   0        0        0     5130 2023-05-16 06:24:15.334818 sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/turbodbc.py
--rw-r--r--   0        0        0     1646 2023-05-16 06:24:15.334818 sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/util.py
--rw-r--r--   0        0        0      235 2023-05-16 06:24:15.334818 sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/version.py
--rw-r--r--   0        0        0     6371 1970-01-01 00:00:00.000000 sqlalchemy_exasol-4.4.0/setup.py
--rw-r--r--   0        0        0     7117 1970-01-01 00:00:00.000000 sqlalchemy_exasol-4.4.0/PKG-INFO
+-rw-r--r--   0        0        0    14999 2023-05-24 13:23:28.579247 sqlalchemy_exasol-4.5.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1395 2023-05-24 13:23:28.579247 sqlalchemy_exasol-4.5.0/LICENSE
+-rw-r--r--   0        0        0    10489 2023-05-24 13:23:28.579247 sqlalchemy_exasol-4.5.0/README.rst
+-rw-r--r--   0        0        0     3410 2023-05-24 13:23:28.635248 sqlalchemy_exasol-4.5.0/pyproject.toml
+-rw-r--r--   0        0        0      413 2023-05-24 13:23:28.635248 sqlalchemy_exasol-4.5.0/sqlalchemy_exasol/__init__.py
+-rw-r--r--   0        0        0    33919 2023-05-24 13:23:28.635248 sqlalchemy_exasol-4.5.0/sqlalchemy_exasol/base.py
+-rw-r--r--   0        0        0      165 2023-05-24 13:23:28.635248 sqlalchemy_exasol-4.5.0/sqlalchemy_exasol/constraints.py
+-rw-r--r--   0        0        0    11765 2023-05-24 13:23:28.635248 sqlalchemy_exasol-4.5.0/sqlalchemy_exasol/pyodbc.py
+-rw-r--r--   0        0        0     7522 2023-05-24 13:23:28.635248 sqlalchemy_exasol-4.5.0/sqlalchemy_exasol/requirements.py
+-rw-r--r--   0        0        0     4262 2023-05-24 13:23:28.635248 sqlalchemy_exasol-4.5.0/sqlalchemy_exasol/turbodbc.py
+-rw-r--r--   0        0        0     1646 2023-05-24 13:23:28.635248 sqlalchemy_exasol-4.5.0/sqlalchemy_exasol/util.py
+-rw-r--r--   0        0        0      235 2023-05-24 13:23:28.635248 sqlalchemy_exasol-4.5.0/sqlalchemy_exasol/version.py
+-rw-r--r--   0        0        0     4689 2023-05-24 13:23:28.635248 sqlalchemy_exasol-4.5.0/sqlalchemy_exasol/websocket.py
+-rw-r--r--   0        0        0    11962 1970-01-01 00:00:00.000000 sqlalchemy_exasol-4.5.0/setup.py
+-rw-r--r--   0        0        0    12487 1970-01-01 00:00:00.000000 sqlalchemy_exasol-4.5.0/PKG-INFO
```

### Comparing `sqlalchemy_exasol-4.4.0/CHANGELOG.rst` & `sqlalchemy_exasol-4.5.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 .. _changelog-unreleased:
 
 Unreleased
 ==========
 
+.. _changelog-4.5.0:
+
+4.5.0 — 2023-05-24
+==================
+* Added Beta version of websocket based dialect
+
+     **🚨 Attention:**
+
+        This feature is currently in Beta, therefore it should not be used in production.
+        We also recommend to have a look into the known issues, before you start using it.
+
+        If you encounter any problem, please `create an issue <https://github.com/exasol/sqlalchemy-exasol/issues/new?assignees=&labels=bug&projects=&template=bug.md&title=%F0%9F%90%9E+%3CInsert+Title%3E>`_.
+        With your feedback, we will be able stabilize this feature more quickly.
+
+
 .. _changelog-4.4.0:
 
 4.4.0 — 2023-05-16
 ==================
 
  **🚨 Attention:**
```

### Comparing `sqlalchemy_exasol-4.4.0/LICENSE` & `sqlalchemy_exasol-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_exasol-4.4.0/pyproject.toml` & `sqlalchemy_exasol-4.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "poetry>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sqlalchemy_exasol"
-version = "4.4.0"
+version = "4.5.0"
 description = "EXASOL dialect for SQLAlchemy"
 readme = "README.rst"
 authors = [
     "Exasol AG <opensource@exasol.com>",
     "Blue Yonder GmbH",
 ]
 license = "BSD"
@@ -88,14 +88,15 @@
 
 [tool.poetry.extras]
 turbodbc = ["turbodbc"]
 
 [tool.poetry.plugins."sqlalchemy.dialects"]
 "exa.pyodbc" = "sqlalchemy_exasol.pyodbc:EXADialect_pyodbc"
 "exa.turbodbc" = "sqlalchemy_exasol.turbodbc:EXADialect_turbodbc"
+"exa.websocket" = "sqlalchemy_exasol.websocket:EXADialect_websocket"
 
 
 [tool.pytest.ini_options]
 addopts = "--tb native -v -r fxX"
 filterwarnings = [
     "error::DeprecationWarning",
     "ignore::DeprecationWarning:sqlalchemy.testing.plugin.*",
@@ -107,15 +108,15 @@
 include = "\\.pyi?$"
 
 [tool.isort]
 profile = "black"
 force_grid_wrap = 2
 
 [tool.pylint.master]
-fail-under = 5.5
+fail-under = 6.4
 
 [tool.pylint.format]
 max-line-length = 88
 max-module-lines = 800
 
 [tool.mypy]
 files = [
```

### Comparing `sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/base.py` & `sqlalchemy_exasol-4.5.0/sqlalchemy_exasol/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -784,21 +784,44 @@
     statement_compiler = EXACompiler
     ddl_compiler = EXADDLCompiler
     type_compiler = EXATypeCompiler
     preparer = EXAIdentifierPreparer
     ischema_names = ischema_names
     colspecs = colspecs
     isolation_level = None
+    server_version_info = None
 
     def __init__(self, isolation_level=None, native_datetime=False, **kwargs):
         default.DefaultDialect.__init__(self, **kwargs)
         self.isolation_level = isolation_level
 
     _isolation_lookup = {"SERIALIZABLE": 0}
 
+    def _get_server_version_info(self, connection):
+        if self.server_version_info is None:
+            query = (
+                "select PARAM_VALUE from SYS.EXA_METADATA"
+                " where PARAM_NAME = 'databaseProductVersion'"
+            )
+            result = connection.execute(query).fetchone()[0].split(".")
+            major, minor, patch = 0, 0, 0
+            major = int(result[0])
+            minor = int(result[1])
+            try:
+                # last version position can something like: '12-S' or 'RC2'
+                # might fail with ValueError
+                patch = int(result[2].split("-")[0])
+            except ValueError:
+                # ignore if there is some funky string in the patch field
+                pass
+            self.server_version_info = (major, minor, patch)
+
+        # return cached info
+        return self.server_version_info
+
     def _get_default_schema_name(self, connection):
         """
         Default schema is derived from current connections url
         or 'SYS'. Tables in 'SYS' are not reflectable!
         """
         schema = None
         schema = self._get_schema_from_url(connection, schema)
```

### Comparing `sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/pyodbc.py` & `sqlalchemy_exasol-4.5.0/sqlalchemy_exasol/pyodbc.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,52 +23,27 @@
 
 logger = logging.getLogger("sqlalchemy_exasol")
 
 
 class EXADialect_pyodbc(EXADialect, PyODBCConnector):
     supports_statement_cache = False
     execution_ctx_cls = EXAExecutionContext
-
     driver_version = None
-    server_version_info = None
 
     def __init__(self, **kw):
         super().__init__(**kw)
 
     def get_driver_version(self, connection):
         # LooseVersion will also work with interim versions like '4.2.7dev1' or '5.0.rc4'
         if self.driver_version is None:
             self.driver_version = version.parse(
                 connection.connection.getinfo(self.dbapi.SQL_DRIVER_VER) or "2.0.0"
             )
         return self.driver_version
 
-    def _get_server_version_info(self, connection):
-        if self.server_version_info is None:
-            # need to check if current version of EXAODBC returns proper server version
-            if self.get_driver_version(connection) >= version.parse("4.2.1"):
-                # v4.2.1 and above should deliver usable SQL_DBMS_VER
-                result = connection.connection.getinfo(self.dbapi.SQL_DBMS_VER).split(
-                    "."
-                )
-            else:
-                # Older versions do not include patchlevels, so we need to get info through SQL call
-                query = "select PARAM_VALUE from SYS.EXA_METADATA where PARAM_NAME = 'databaseProductVersion'"
-                result = connection.execute(query).fetchone()[0].split(".")
-
-            # last version position can something like: '12-S' for an EXASolo
-            self.server_version_info = (
-                int(result[0]),
-                int(result[1]),
-                int(result[2].split("-")[0]),
-            )
-
-        # return cached info
-        return self.server_version_info
-
     if sys.platform == "darwin":
 
         def connect(self, *cargs, **cparams):
             # Get connection
             conn = super().connect(*cargs, **cparams)
 
             # Set up encodings
```

### Comparing `sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/requirements.py` & `sqlalchemy_exasol-4.5.0/sqlalchemy_exasol/requirements.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/turbodbc.py` & `sqlalchemy_exasol-4.5.0/sqlalchemy_exasol/turbodbc.py`

 * *Files 14% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 
         return to_integer
 
 
 class EXADialect_turbodbc(EXADialect):
     driver = "turbodbc"
     driver_version = None
-    server_version_info = None
     supports_statement_cache = False
     supports_native_decimal = False
     supports_sane_multi_rowcount = False
 
     colspecs = {sqltypes.Numeric: _ExaDecimal, sqltypes.Integer: _ExaInteger}
 
     @classmethod
@@ -80,33 +79,14 @@
     def create_connect_args(self, url):
         options = self._get_options_with_defaults(url)
         self._translate_none(options)
         self._interpret_destination(options)
 
         return [[options.pop("dsn", None)], options]
 
-    def _get_server_version_info(self, connection):
-        if self.server_version_info is None:
-            query = "select PARAM_VALUE from SYS.EXA_METADATA where PARAM_NAME = 'databaseProductVersion'"
-            result = connection.execute(query).fetchone()[0].split(".")
-            major, minor, patch = 0, 0, 0
-            major = int(result[0])
-            minor = int(result[1])
-            try:
-                # last version position can something like: '12-S' or 'RC2'
-                # might fail with ValueError
-                patch = int(result[2].split("-")[0])
-            except ValueError:
-                # ignore if there is some funky string in the patch field
-                pass
-            self.server_version_info = (major, minor, patch)
-
-        # return cached info
-        return self.server_version_info
-
     @staticmethod
     def _get_options_with_defaults(url):
         user_options = url.translate_connect_args(
             username="uid", password="pwd", database="exaschema", host="destination"
         )
         user_options.update(url.query)
```

### Comparing `sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/util.py` & `sqlalchemy_exasol-4.5.0/sqlalchemy_exasol/util.py`

 * *Files identical despite different names*

