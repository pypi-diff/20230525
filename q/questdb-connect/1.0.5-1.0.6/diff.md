# Comparing `tmp/questdb-connect-1.0.5.tar.gz` & `tmp/questdb-connect-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-1.0.5.tar", last modified: Mon May 22 16:23:21 2023, max compression
+gzip compressed data, was "questdb-connect-1.0.6.tar", last modified: Mon May 22 17:23:20 2023, max compression
```

## Comparing `questdb-connect-1.0.5.tar` & `questdb-connect-1.0.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 16:23:21.919663 questdb-connect-1.0.5/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-1.0.5/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4493 2023-05-22 16:23:21.919508 questdb-connect-1.0.5/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3789 2023-05-22 13:37:39.000000 questdb-connect-1.0.5/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2577 2023-05-22 16:22:57.000000 questdb-connect-1.0.5/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 16:23:21.919702 questdb-connect-1.0.5/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 16:23:21.912363 questdb-connect-1.0.5/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 16:23:21.915288 questdb-connect-1.0.5/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-1.0.5/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-1.0.5/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-1.0.5/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-1.0.5/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-1.0.5/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-1.0.5/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 16:23:21.916450 questdb-connect-1.0.5/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1937 2023-05-22 14:22:42.000000 questdb-connect-1.0.5/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11809 2023-05-22 16:22:29.000000 questdb-connect-1.0.5/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-1.0.5/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)     5780 2023-05-22 09:34:56.000000 questdb-connect-1.0.5/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 16:23:21.917531 questdb-connect-1.0.5/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4493 2023-05-22 16:23:21.000000 questdb-connect-1.0.5/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      788 2023-05-22 16:23:21.000000 questdb-connect-1.0.5/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-22 16:23:21.000000 questdb-connect-1.0.5/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      160 2023-05-22 16:23:21.000000 questdb-connect-1.0.5/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-22 16:23:21.000000 questdb-connect-1.0.5/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 16:23:21.000000 questdb-connect-1.0.5/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 16:23:21.917644 questdb-connect-1.0.5/src/superset_ext/
--rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.5/src/superset_ext/__init__.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 16:23:21.918215 questdb-connect-1.0.5/src/superset_ext/db_engine_specs/
--rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.5/src/superset_ext/db_engine_specs/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    12383 2023-05-22 16:22:29.000000 questdb-connect-1.0.5/src/superset_ext/db_engine_specs/questdb.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 16:23:21.919104 questdb-connect-1.0.5/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-1.0.5/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2844 2023-05-22 13:02:28.000000 questdb-connect-1.0.5/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-1.0.5/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.838662 questdb-connect-1.0.6/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-1.0.6/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4493 2023-05-22 17:23:20.838526 questdb-connect-1.0.6/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3789 2023-05-22 13:37:39.000000 questdb-connect-1.0.6/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2640 2023-05-22 17:22:05.000000 questdb-connect-1.0.6/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 17:23:20.838703 questdb-connect-1.0.6/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.830250 questdb-connect-1.0.6/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.832518 questdb-connect-1.0.6/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-1.0.6/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-22 17:17:06.000000 questdb-connect-1.0.6/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-22 17:17:06.000000 questdb-connect-1.0.6/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-22 17:17:06.000000 questdb-connect-1.0.6/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-22 17:17:06.000000 questdb-connect-1.0.6/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-1.0.6/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.835646 questdb-connect-1.0.6/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1937 2023-05-22 14:22:42.000000 questdb-connect-1.0.6/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11788 2023-05-22 17:17:06.000000 questdb-connect-1.0.6/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-1.0.6/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5780 2023-05-22 09:34:56.000000 questdb-connect-1.0.6/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.836689 questdb-connect-1.0.6/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4493 2023-05-22 17:23:20.000000 questdb-connect-1.0.6/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      788 2023-05-22 17:23:20.000000 questdb-connect-1.0.6/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-22 17:23:20.000000 questdb-connect-1.0.6/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      160 2023-05-22 17:23:20.000000 questdb-connect-1.0.6/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      159 2023-05-22 17:23:20.000000 questdb-connect-1.0.6/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 17:23:20.000000 questdb-connect-1.0.6/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.836808 questdb-connect-1.0.6/src/superset_ext/
+-rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.6/src/superset_ext/__init__.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.837388 questdb-connect-1.0.6/src/superset_ext/db_engine_specs/
+-rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.6/src/superset_ext/db_engine_specs/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    12227 2023-05-22 17:20:15.000000 questdb-connect-1.0.6/src/superset_ext/db_engine_specs/questdb.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.838137 questdb-connect-1.0.6/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-22 17:17:07.000000 questdb-connect-1.0.6/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2846 2023-05-22 17:17:07.000000 questdb-connect-1.0.6/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-1.0.6/tests/test_types.py
```

### Comparing `questdb-connect-1.0.5/LICENSE` & `questdb-connect-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.5/PKG-INFO` & `questdb-connect-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 1.0.5
+Version: 1.0.6
 Summary: SqlAlchemy/Superset library.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-1.0.5/README.md` & `questdb-connect-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.5/pyproject.toml` & `questdb-connect-1.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = 'questdb-connect'
-version = '1.0.5'
+version = '1.0.6'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset library."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
@@ -52,14 +52,17 @@
 test = [
     'psycopg2-binary~=2.9.6',
     'SQLAlchemy<=1.4.47',
     'apache-superset>=2.1.0',
     'sqlparse==0.4.3',
     'ruff~=0.0.269',
     'pytest~=7.3.0',
+    'black~=23.3.0',
+    'isort~=5.12.0',
+    'bandit~=1.7.5',
 ]
 
 [tool.ruff]
 # https://github.com/charliermarsh/ruff#configuration
 select = ["PL", "RUF", "TCH", "TID", "PT", "C4", "B", "S", "I"]
 line-length = 120
 exclude = [
```

### Comparing `questdb-connect-1.0.5/src/examples/__init__.py` & `questdb-connect-1.0.6/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.5/src/examples/hello_world.py` & `questdb-connect-1.0.6/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.5/src/examples/psycopg2_connect.py` & `questdb-connect-1.0.6/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.5/src/examples/server_utilisation.py` & `questdb-connect-1.0.6/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.5/src/examples/sqlalchemy_orm.py` & `questdb-connect-1.0.6/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.5/src/examples/sqlalchemy_raw.py` & `questdb-connect-1.0.6/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.5/src/questdb_connect/__init__.py` & `questdb-connect-1.0.6/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.5/src/questdb_connect/dialect.py` & `questdb-connect-1.0.6/src/questdb_connect/dialect.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,20 +25,15 @@
 
 import sqlalchemy
 from sqlalchemy import Column, MetaData, text
 from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
 from sqlalchemy.engine.reflection import Inspector, cache
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql.base import SchemaEventTarget
-from sqlalchemy.sql.compiler import (
-    DDLCompiler,
-    GenericTypeCompiler,
-    IdentifierPreparer,
-    SQLCompiler,
-)
+from sqlalchemy.sql.compiler import DDLCompiler, GenericTypeCompiler, IdentifierPreparer, SQLCompiler
 from sqlalchemy.sql.visitors import Traversible
 
 from . import remove_public_schema
 from .types import *
 
 logger = logging.getLogger(__name__)
```

### Comparing `questdb-connect-1.0.5/src/questdb_connect/function_names.py` & `questdb-connect-1.0.6/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.5/src/questdb_connect/types.py` & `questdb-connect-1.0.6/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.5/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-1.0.6/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 1.0.5
+Version: 1.0.6
 Summary: SqlAlchemy/Superset library.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-1.0.5/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-1.0.6/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.5/src/superset_ext/__init__.py` & `questdb-connect-1.0.6/src/superset_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.5/src/superset_ext/db_engine_specs/__init__.py` & `questdb-connect-1.0.6/src/superset_ext/db_engine_specs/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.5/src/superset_ext/db_engine_specs/questdb.py` & `questdb-connect-1.0.6/src/superset_ext/db_engine_specs/questdb.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,153 +33,151 @@
     BaseEngineSpec,
     BasicParametersMixin,
     BasicParametersType,
 )
 from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
-from questdb_connect import remove_public_schema, types as questdb_types
+from questdb_connect import remove_public_schema
+from questdb_connect import types as questdb_types
 from questdb_connect.dialect import connection_uri
 from questdb_connect.function_names import FUNCTION_NAMES
 
-
 # Apache Superset requires a Python DB-API database driver, and a SQLAlchemy dialect
 # https://superset.apache.org/docs/databases/installing-database-drivers
 # https://preset.io/blog/building-database-connector/
 # https://preset.io/blog/improving-apache-superset-integration-database-sqlalchemy/
 
 
 class QDBParametersSchema(Schema):
-    username = fields.String(allow_none=True, description=__('user'))
-    password = fields.String(allow_none=True, description=__('password'))
-    host = fields.String(required=True, description=__('host'))
-    port = fields.Integer(allow_none=True, description=__('port'))
-    database = fields.String(allow_none=True, description=__('database'))
+    username = fields.String(allow_none=True, description=__("user"))
+    password = fields.String(allow_none=True, description=__("password"))
+    host = fields.String(required=True, description=__("host"))
+    port = fields.Integer(allow_none=True, description=__("port"))
+    database = fields.String(allow_none=True, description=__("database"))
 
 
 class QDBEngineSpec(BaseEngineSpec, BasicParametersMixin):
-    engine = 'questdb'
-    engine_name = 'QuestDB Connect'
+    engine = "questdb"
+    engine_name = "QuestDB Connect"
     default_driver = "psycopg2"
     encryption_parameters = {"sslmode": "prefer"}
     sqlalchemy_uri_placeholder = "questdb://user:password@host:port/database"
     parameters_schema = QDBParametersSchema()
     time_groupby_inline = False
     allows_hidden_cc_in_orderby = True
     time_secondary_columns = True
     try_remove_schema_from_table_name = True
     max_column_name_length = 120
     supports_dynamic_schema = False
     top_keywords = {}
     # https://en.wikipedia.org/wiki/ISO_8601#Durations
     # https://questdb.io/docs/reference/function/date-time/#date_trunc
     _time_grain_expressions = {
-        None: '{col}',
+        None: "{col}",
         "PT1S": "date_trunc('second', {col})",
         "PT1M": "date_trunc('minute', {col})",
         "PT1H": "date_trunc('hour', {col})",
         "P1D": "date_trunc('day', {col})",
         "P1W": "date_trunc('week', {col})",
         "P1M": "date_trunc('month', {col})",
         "P1Y": "date_trunc('year', {col})",
         "P3M": "date_trunc('quarter', {col})",
     }
     column_type_mappings = (
         (
             re.compile("^LONG256", re.IGNORECASE),
             questdb_types.Long256,
-            GenericDataType.STRING
+            GenericDataType.STRING,
         ),
         (
             re.compile("^BOOLEAN", re.IGNORECASE),
             questdb_types.Boolean,
-            GenericDataType.BOOLEAN
+            GenericDataType.BOOLEAN,
         ),
         (
             re.compile("^BYTE", re.IGNORECASE),
             questdb_types.Byte,
-            GenericDataType.NUMERIC),
+            GenericDataType.NUMERIC,
+        ),
         (
             re.compile("^SHORT", re.IGNORECASE),
             questdb_types.Short,
-            GenericDataType.NUMERIC
-        ),
-        (
-            re.compile("^INT", re.IGNORECASE),
-            questdb_types.Int,
-            GenericDataType.NUMERIC
+            GenericDataType.NUMERIC,
         ),
+        (re.compile("^INT", re.IGNORECASE), questdb_types.Int, GenericDataType.NUMERIC),
         (
             re.compile("^LONG", re.IGNORECASE),
             questdb_types.Long,
-            GenericDataType.NUMERIC
+            GenericDataType.NUMERIC,
         ),
         (
             re.compile("^FLOAT", re.IGNORECASE),
             questdb_types.Float,
-            GenericDataType.NUMERIC
+            GenericDataType.NUMERIC,
         ),
         (
             re.compile("^DOUBLE'", re.IGNORECASE),
             questdb_types.Double,
-            GenericDataType.NUMERIC
+            GenericDataType.NUMERIC,
         ),
         (
             re.compile("^SYMBOL", re.IGNORECASE),
             questdb_types.Symbol,
-            GenericDataType.STRING
+            GenericDataType.STRING,
         ),
         (
             re.compile("^STRING", re.IGNORECASE),
             questdb_types.String,
-            GenericDataType.STRING
+            GenericDataType.STRING,
         ),
         (
             re.compile("^UUID", re.IGNORECASE),
             questdb_types.UUID,
-            GenericDataType.STRING
+            GenericDataType.STRING,
         ),
         (
             re.compile("^CHAR", re.IGNORECASE),
             questdb_types.Char,
-            GenericDataType.STRING
+            GenericDataType.STRING,
         ),
         (
             re.compile("^TIMESTAMP", re.IGNORECASE),
             questdb_types.Timestamp,
-            GenericDataType.TEMPORAL
+            GenericDataType.TEMPORAL,
         ),
         (
             re.compile("^DATE", re.IGNORECASE),
             questdb_types.Date,
-            GenericDataType.TEMPORAL
+            GenericDataType.TEMPORAL,
         ),
         (
             re.compile(r"^GEOHASH\(\d+[b|c]\)", re.IGNORECASE),
             questdb_types.GeohashLong,
-            GenericDataType.STRING
-        )
+            GenericDataType.STRING,
+        ),
     )
 
     @classmethod
     def build_sqlalchemy_uri(
-            cls,
-            parameters: BasicParametersType,
-            encrypted_extra: Optional[Dict[str, str]] = None
+        cls,
+        parameters: BasicParametersType,
+        encrypted_extra: Optional[Dict[str, str]] = None,
     ) -> str:
         return connection_uri(
             parameters.get("host"),
             parameters.get("port"),
             parameters.get("username"),
             parameters.get("password"),
-            parameters.get("database"))
+            parameters.get("database"),
+        )
 
     @classmethod
     def get_default_schema_for_query(cls, database, query) -> Optional[str]:
-        return 'public'
+        return "public"
 
     @classmethod
     def get_text_clause(cls, clause):
         """SQLAlchemy wrapper to ensure text clauses are escaped properly
         :param clause: string clause with potentially unescaped characters
         :return: text clause with escaped characters
         """
@@ -190,34 +188,30 @@
     @classmethod
     def epoch_to_dttm(cls) -> str:
         """SQL expression that converts epoch (seconds) to datetime that can be used
         in a query. The reference column should be denoted as `{col}` in the return
         expression, e.g. "FROM_UNIXTIME({col})"
         :return: SQL Expression
         """
-        return '{col} * 1000000'
+        return "{col} * 1000000"
 
     @classmethod
     def convert_dttm(
-            cls,
-            target_type: str,
-            dttm: datetime,
-            *_args,
-            **_kwargs
+        cls, target_type: str, dttm: datetime, *_args, **_kwargs
     ) -> Optional[str]:
         """Convert a Python `datetime` object to a SQL expression.
         :param target_type: The target type of expression
         :param dttm: The datetime object
         :return: The SQL expression
         """
         type_u = target_type.upper()
-        if type_u == 'DATE':
+        if type_u == "DATE":
             return f"TO_DATE('{dttm.date().isoformat()}', 'YYYY-MM-DD')"
-        if type_u in ('DATETIME', 'TIMESTAMP'):
-            dttm_formatted = dttm.isoformat(sep=" ", timespec="microseconds")
+        if type_u in ("DATETIME", "TIMESTAMP"):
+            dttm_formatted = dttm.isoformat(sep="T", timespec="microseconds")
             return f"TO_TIMESTAMP('{dttm_formatted}', 'yyyy-MM-ddTHH:mm:ss.SSSUUUZ')"
         return None
 
     @classmethod
     def get_datatype(cls, type_code: Any) -> Optional[str]:
         """Change column type code from cursor description to string representation.
         :param type_code: Type code from cursor description
@@ -225,88 +219,86 @@
         """
         if type_code and isinstance(type_code, str):
             return type_code.upper()
         return str(type_code)
 
     @classmethod
     def get_column_spec(
-            cls,
-            native_type: Optional[str],
-            db_extra: Optional[Dict[str, Any]] = None,
-            source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
+        cls,
+        native_type: Optional[str],
+        db_extra: Optional[Dict[str, Any]] = None,
+        source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
     ) -> Optional[utils.ColumnSpec]:
         """Get generic type related specs regarding a native column type.
         :param native_type: Native database type
         :param db_extra: The database extra object
         :param source: Type coming from the database table or cursor description
         :return: ColumnSpec object
         """
         sqla_type = questdb_types.resolve_type_from_name(native_type)
         if not sqla_type:
             return BaseEngineSpec.get_column_spec(native_type, db_extra, source)
         name_u = sqla_type.__visit_name__
         generic_type = None
-        if name_u == 'BOOLEAN':
+        if name_u == "BOOLEAN":
             generic_type = GenericDataType.BOOLEAN
-        elif name_u in ('BYTE', 'SHORT', 'INT', 'LONG', 'FLOAT', 'DOUBLE'):
+        elif name_u in ("BYTE", "SHORT", "INT", "LONG", "FLOAT", "DOUBLE"):
             generic_type = GenericDataType.NUMERIC
-        elif name_u in ('SYMBOL', 'STRING', 'CHAR', 'LONG256', 'UUID'):
+        elif name_u in ("SYMBOL", "STRING", "CHAR", "LONG256", "UUID"):
             generic_type = GenericDataType.STRING
-        elif name_u in ('DATE', 'TIMESTAMP'):
+        elif name_u in ("DATE", "TIMESTAMP"):
             generic_type = GenericDataType.TEMPORAL
-        elif 'GEOHASH' in name_u and '(' in name_u and ')' in name_u:
+        elif "GEOHASH" in name_u and "(" in name_u and ")" in name_u:
             generic_type = GenericDataType.STRING
         return utils.ColumnSpec(
-            sqla_type,
-            generic_type,
-            generic_type == GenericDataType.TEMPORAL
+            sqla_type, generic_type, generic_type == GenericDataType.TEMPORAL
         )
 
     @classmethod
     def get_sqla_column_type(
-            cls,
-            native_type: Optional[str],
-            db_extra: Optional[Dict[str, Any]] = None,
-            source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
+        cls,
+        native_type: Optional[str],
+        db_extra: Optional[Dict[str, Any]] = None,
+        source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
     ) -> Optional[TypeEngine]:
         """Converts native database type to sqlalchemy column type.
         :param native_type: Native database type
         :param db_extra: The database extra object
         :param source: Type coming from the database table or cursor description
         :return: ColumnSpec object
         """
         return questdb_types.resolve_type_from_name(native_type).impl
 
     @classmethod
     def column_datatype_to_string(
-            cls,
-            sqla_column_type: TypeEngine,
-            dialect: Dialect,
+        cls,
+        sqla_column_type: TypeEngine,
+        dialect: Dialect,
     ) -> str:
         """Convert sqlalchemy column type to string representation.
         By default, removes collation and character encoding info to avoid
         unnecessarily long datatypes.
         :param sqla_column_type: SqlAlchemy column type
         :param dialect: Sqlalchemy dialect
         :return: Compiled column type
         """
         return sqla_column_type.copy().compile(dialect=dialect)
 
     @classmethod
     def select_star(
-            cls,
-            database,
-            table_name: str,
-            engine,
-            schema: Optional[str] = None,
-            limit: int = 100,
-            show_cols: bool = False,
-            indent: bool = True,
-            latest_partition: bool = True,
-            cols: Optional[List[Dict[str, Any]]] = None,
+        cls,
+        database,
+        table_name: str,
+        engine,
+        schema: Optional[str] = None,
+        limit: int = 100,
+        show_cols: bool = False,
+        indent: bool = True,
+        latest_partition: bool = True,
+        cols: Optional[List[Dict[str, Any]]] = None,
     ) -> str:
         """Generate a "SELECT * from table_name" query with appropriate limit.
         :param database: Database instance
         :param table_name: Table name, unquoted
         :param engine: SqlAlchemy Engine instance
         :param schema: Schema, unquoted
         :param limit: limit to impose on query
@@ -321,15 +313,15 @@
             table_name,
             engine,
             None,
             limit,
             show_cols,
             indent,
             latest_partition,
-            cols
+            cols,
         )
 
     @classmethod
     def get_function_names(cls, database) -> List[str]:
         """Get a list of function names that are able to be called on the database.
         Used for SQL Lab autocomplete.
         :param database: The database to get functions for
```

### Comparing `questdb-connect-1.0.5/tests/test_dialect.py` & `questdb-connect-1.0.6/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.5/tests/test_superset.py` & `questdb-connect-1.0.6/tests/test_superset.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import pytest
 from superset_ext.db_engine_specs.questdb import QDBEngineSpec
 
 
 def test_build_sqlalchemy_uri():
     request_uri = QDBEngineSpec.build_sqlalchemy_uri({
         'host': 'localhost',
-        'port': 8812,
+        'port': '8812',
         'username': 'admin',
         'password': 'quest',
         'database': 'main',
     })
     assert 'questdb://admin:quest@localhost:8812/main' == request_uri
 
 
@@ -44,20 +44,20 @@
         (
                 "Date",
                 "TO_DATE('2023-04-28', 'YYYY-MM-DD')",
                 datetime.datetime(2023, 4, 28, 23, 55, 59, 281567)
         ),
         (
                 "DateTime",
-                "TO_TIMESTAMP('2023-04-28 23:55:59.281567', 'yyyy-MM-ddTHH:mm:ss.SSSUUUZ')",
+                "TO_TIMESTAMP('2023-04-28T23:55:59.281567', 'yyyy-MM-ddTHH:mm:ss.SSSUUUZ')",
                 datetime.datetime(2023, 4, 28, 23, 55, 59, 281567)
         ),
         (
                 "TimeStamp",
-                "TO_TIMESTAMP('2023-04-28 23:55:59.281567', 'yyyy-MM-ddTHH:mm:ss.SSSUUUZ')",
+                "TO_TIMESTAMP('2023-04-28T23:55:59.281567', 'yyyy-MM-ddTHH:mm:ss.SSSUUUZ')",
                 datetime.datetime(2023, 4, 28, 23, 55, 59, 281567)
         ),
         ("UnknownType", None, datetime.datetime(2023, 4, 28, 23, 55, 59, 281567)),
     ],
 )
 def test_convert_dttm(target_type, expected_result, dttm) -> None:
     # datetime(year, month, day, hour, minute, second, microsecond)
```

### Comparing `questdb-connect-1.0.5/tests/test_types.py` & `questdb-connect-1.0.6/tests/test_types.py`

 * *Files identical despite different names*

