# Comparing `tmp/dagster-snowflake-0.9.9rc1.tar.gz` & `tmp/dagster-snowflake-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-snowflake-0.9.9rc1.tar", last modified: Thu Sep 17 21:09:06 2020, max compression
+gzip compressed data, was "dagster-snowflake-1.0.5.tar", last modified: Fri Aug 26 13:44:27 2022, max compression
```

## Comparing `dagster-snowflake-0.9.9rc1.tar` & `dagster-snowflake-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,23 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      598 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      137 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake/
--rw-r--r--   0 bobchen    (501) staff       (20)      311 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4573 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake/configs.py
--rw-r--r--   0 bobchen    (501) staff       (20)     5881 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)      504 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake/solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      598 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      629 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       42 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       42 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3080 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake_tests/test_resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1215 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake_tests/test_solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)       95 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)      424 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake_tests/utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1079 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:27.936128 dagster-snowflake-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-snowflake-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2022-08-26 13:33:01.000000 dagster-snowflake-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      666 2022-08-26 13:44:27.936128 dagster-snowflake-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      137 2022-08-26 13:33:01.000000 dagster-snowflake-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:27.936128 dagster-snowflake-1.0.5/dagster_snowflake/
+-rw-r--r--   0 root         (0) root         (0)      496 2022-08-26 13:33:01.000000 dagster-snowflake-1.0.5/dagster_snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5699 2022-08-26 13:33:01.000000 dagster-snowflake-1.0.5/dagster_snowflake/configs.py
+-rw-r--r--   0 root         (0) root         (0)     7045 2022-08-26 13:33:01.000000 dagster-snowflake-1.0.5/dagster_snowflake/db_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-snowflake-1.0.5/dagster_snowflake/py.typed
+-rw-r--r--   0 root         (0) root         (0)     7375 2022-08-26 13:33:01.000000 dagster-snowflake-1.0.5/dagster_snowflake/resources.py
+-rw-r--r--   0 root         (0) root         (0)     3762 2022-08-26 13:33:01.000000 dagster-snowflake-1.0.5/dagster_snowflake/snowflake_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2217 2022-08-26 13:33:01.000000 dagster-snowflake-1.0.5/dagster_snowflake/solids.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-snowflake-1.0.5/dagster_snowflake/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:27.936128 dagster-snowflake-1.0.5/dagster_snowflake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      666 2022-08-26 13:44:27.000000 dagster-snowflake-1.0.5/dagster_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      543 2022-08-26 13:44:27.000000 dagster-snowflake-1.0.5/dagster_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:44:27.000000 dagster-snowflake-1.0.5/dagster_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:44:27.000000 dagster-snowflake-1.0.5/dagster_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      122 2022-08-26 13:44:27.000000 dagster-snowflake-1.0.5/dagster_snowflake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2022-08-26 13:44:27.000000 dagster-snowflake-1.0.5/dagster_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      164 2022-08-26 13:44:27.940127 dagster-snowflake-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1439 2022-08-26 13:33:01.000000 dagster-snowflake-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-snowflake-0.9.9rc1/LICENSE` & `dagster-snowflake-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-0.9.9rc1/PKG-INFO` & `dagster-snowflake-1.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-snowflake
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: Package for Snowflake Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Provides-Extra: snowflake.sqlalchemy
+Provides-Extra: pandas
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-snowflake-0.9.9rc1/dagster_snowflake/configs.py` & `dagster-snowflake-1.0.5/dagster_snowflake/configs.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,102 +16,130 @@
 
     user = Field(StringSource, description="User login name.", is_required=True)
 
     password = Field(StringSource, description="User password.", is_required=True)
 
     database = Field(
         StringSource,
-        description="""Name of the default database to use. After login, you can use USE DATABASE
-         to change the database.""",
+        description="Name of the default database to use. After login, you can use USE DATABASE "
+        " to change the database.",
         is_required=False,
     )
 
     schema = Field(
         StringSource,
-        description="""Name of the default schema to use. After login, you can use USE SCHEMA to
-         change the schema.""",
+        description="Name of the default schema to use. After login, you can use USE SCHEMA to "
+        "change the schema.",
         is_required=False,
     )
 
     role = Field(
         StringSource,
-        description="""Name of the default role to use. After login, you can use USE ROLE to change
-         the role.""",
+        description="Name of the default role to use. After login, you can use USE ROLE to change "
+        " the role.",
         is_required=False,
     )
 
     warehouse = Field(
         StringSource,
-        description="""Name of the default warehouse to use. After login, you can use USE WAREHOUSE
-         to change the role.""",
+        description="Name of the default warehouse to use. After login, you can use USE WAREHOUSE "
+        "to change the role.",
         is_required=False,
     )
 
     autocommit = Field(
         Bool,
-        description="""None by default, which honors the Snowflake parameter AUTOCOMMIT. Set to True
-         or False to enable or disable autocommit mode in the session, respectively.""",
+        description="None by default, which honors the Snowflake parameter AUTOCOMMIT. Set to True "
+        "or False to enable or disable autocommit mode in the session, respectively.",
         is_required=False,
     )
 
     client_prefetch_threads = Field(
         IntSource,
-        description="""Number of threads used to download the results sets (4 by default).
-         Increasing the value improves fetch performance but requires more memory.""",
+        description="Number of threads used to download the results sets (4 by default). "
+        "Increasing the value improves fetch performance but requires more memory.",
         is_required=False,
     )
 
     client_session_keep_alive = Field(
         StringSource,
-        description="""False by default. Set this to True to keep the session active indefinitely,
-         even if there is no activity from the user. Make certain to call the close method to
-         terminate the thread properly or the process may hang.""",
+        description="False by default. Set this to True to keep the session active indefinitely, "
+        "even if there is no activity from the user. Make certain to call the close method to "
+        "terminate the thread properly or the process may hang.",
         is_required=False,
     )
 
     login_timeout = Field(
         IntSource,
-        description="""Timeout in seconds for login. By default, 60 seconds. The login request gives
-         up after the timeout length if the HTTP response is "success".""",
+        description="Timeout in seconds for login. By default, 60 seconds. The login request gives "
+        'up after the timeout length if the HTTP response is "success".',
         is_required=False,
     )
 
     network_timeout = Field(
         IntSource,
-        description='''Timeout in seconds for all other operations. By default, none/infinite. A
-         general request gives up after the timeout length if the HTTP response is not "success"''',
+        description="Timeout in seconds for all other operations. By default, none/infinite. A "
+        "general request gives up after the timeout length if the HTTP response is not 'success'.",
         is_required=False,
     )
 
     ocsp_response_cache_filename = Field(
         StringSource,
-        description="""URI for the OCSP response cache file.
-         By default, the OCSP response cache file is created in the cache directory.""",
+        description="URI for the OCSP response cache file.  By default, the OCSP response cache "
+        "file is created in the cache directory.",
         is_required=False,
     )
 
     validate_default_parameters = Field(
         Bool,
-        description="""False by default. Raise an exception if either one of specified database,
-         schema or warehouse doesn't exists if True.""",
+        description="False by default. Raise an exception if either one of specified database, "
+        "schema or warehouse doesn't exists if True.",
         is_required=False,
     )
 
     paramstyle = Field(
         # TODO should validate only against permissible values for this
         StringSource,
-        description="""pyformat by default for client side binding. Specify qmark or numeric to
-        change bind variable formats for server side binding.""",
+        description="pyformat by default for client side binding. Specify qmark or numeric to "
+        "change bind variable formats for server side binding.",
         is_required=False,
     )
 
     timezone = Field(
         StringSource,
-        description="""None by default, which honors the Snowflake parameter TIMEZONE. Set to a
-         valid time zone (e.g. America/Los_Angeles) to set the session time zone.""",
+        description="None by default, which honors the Snowflake parameter TIMEZONE. Set to a "
+        "valid time zone (e.g. America/Los_Angeles) to set the session time zone.",
+        is_required=False,
+    )
+
+    connector = Field(
+        StringSource,
+        description="Indicate alternative database connection engine. Permissible option is "
+        "'sqlalchemy' otherwise defaults to use the Snowflake Connector for Python.",
+        is_required=False,
+    )
+
+    cache_column_metadata = Field(
+        StringSource,
+        description="Optional parameter when connector is set to sqlalchemy. Snowflake SQLAlchemy "
+        "takes a flag cache_column_metadata=True such that all of column metadata for all tables are "
+        '"cached"',
+        is_required=False,
+    )
+
+    numpy = Field(
+        StringSource,
+        description="Optional parameter when connector is set to sqlalchemy. To enable fetching "
+        "NumPy data types, add numpy=True to the connection parameters.",
+        is_required=False,
+    )
+
+    authenticator = Field(
+        StringSource,
+        description="Optional parameter to specify the authentication mechanism to use.",
         is_required=False,
     )
 
     return {
         "account": account,
         "user": user,
         "password": password,
@@ -124,8 +152,12 @@
         "client_session_keep_alive": client_session_keep_alive,
         "login_timeout": login_timeout,
         "network_timeout": network_timeout,
         "ocsp_response_cache_filename": ocsp_response_cache_filename,
         "validate_default_parameters": validate_default_parameters,
         "paramstyle": paramstyle,
         "timezone": timezone,
+        "connector": connector,
+        "cache_column_metadata": cache_column_metadata,
+        "numpy": numpy,
+        "authenticator": authenticator,
     }
```

### Comparing `dagster-snowflake-0.9.9rc1/dagster_snowflake/resources.py` & `dagster-snowflake-1.0.5/dagster_snowflake/resources.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import sys
 import warnings
 from contextlib import closing, contextmanager
+from typing import Mapping
 
-from dagster import check, resource
+import pandas as pd
+
+import dagster._check as check
+from dagster import resource
 
 from .configs import define_snowflake_config
 
 try:
     import snowflake.connector
 except ImportError:
     msg = (
@@ -17,82 +21,125 @@
         "dagster-snowflake to fix this error."
     )
     warnings.warn(msg)
     raise
 
 
 class SnowflakeConnection:
-    def __init__(self, context):  # pylint: disable=too-many-locals
+    def __init__(self, config: Mapping[str, str], log):  # pylint: disable=too-many-locals
         # Extract parameters from resource config. Note that we can't pass None values to
         # snowflake.connector.connect() because they will override the default values set within the
         # connector; remove them from the conn_args dict.
-        self.conn_args = {
-            k: context.resource_config.get(k)
-            for k in (
-                "account",
-                "user",
-                "password",
-                "database",
-                "schema",
-                "role",
-                "warehouse",
-                "autocommit",
-                "client_prefetch_threads",
-                "client_session_keep_alive",
-                "login_timeout",
-                "network_timeout",
-                "ocsp_response_cache_filename",
-                "validate_default_parameters",
-                "paramstyle",
-                "timezone",
-            )
-            if context.resource_config.get(k) is not None
-        }
+        self.connector = config.get("connector", None)
+
+        if self.connector == "sqlalchemy":
+            self.conn_args = {
+                k: config.get(k)
+                for k in (
+                    "account",
+                    "user",
+                    "password",
+                    "database",
+                    "schema",
+                    "role",
+                    "warehouse",
+                    "cache_column_metadata",
+                    "numpy",
+                )
+                if config.get(k) is not None
+            }
+
+        else:
+            self.conn_args = {
+                k: config.get(k)
+                for k in (
+                    "account",
+                    "user",
+                    "password",
+                    "database",
+                    "schema",
+                    "role",
+                    "warehouse",
+                    "autocommit",
+                    "client_prefetch_threads",
+                    "client_session_keep_alive",
+                    "login_timeout",
+                    "network_timeout",
+                    "ocsp_response_cache_filename",
+                    "validate_default_parameters",
+                    "paramstyle",
+                    "timezone",
+                    "authenticator",
+                )
+                if config.get(k) is not None
+            }
 
         self.autocommit = self.conn_args.get("autocommit", False)
-        self.log = context.log_manager
+        self.log = log
 
     @contextmanager
-    def get_connection(self):
-        conn = snowflake.connector.connect(**self.conn_args)
-        yield conn
-        if not self.autocommit:
-            conn.commit()
-        conn.close()
+    def get_connection(self, raw_conn=True):
+        if self.connector == "sqlalchemy":
+            from snowflake.sqlalchemy import URL  # pylint: disable=no-name-in-module,import-error
+            from sqlalchemy import create_engine
+
+            engine = create_engine(URL(**self.conn_args))
+            conn = engine.raw_connection() if raw_conn else engine.connect()
+
+            yield conn
+            conn.close()
+            engine.dispose()
+        else:
+            conn = snowflake.connector.connect(**self.conn_args)
+
+            yield conn
+            if not self.autocommit:
+                conn.commit()
+            conn.close()
 
-    def execute_query(self, sql, parameters=None, fetch_results=False):
+    def execute_query(self, sql, parameters=None, fetch_results=False, use_pandas_result=False):
         check.str_param(sql, "sql")
         check.opt_dict_param(parameters, "parameters")
         check.bool_param(fetch_results, "fetch_results")
 
         with self.get_connection() as conn:
             with closing(conn.cursor()) as cursor:
                 if sys.version_info[0] < 3:
                     sql = sql.encode("utf-8")
 
                 self.log.info("Executing query: " + sql)
                 cursor.execute(sql, parameters)  # pylint: disable=E1101
                 if fetch_results:
                     return cursor.fetchall()  # pylint: disable=E1101
+                if use_pandas_result:
+                    return cursor.fetch_pandas_all()
 
-    def execute_queries(self, sql_queries, parameters=None, fetch_results=False):
+    def execute_queries(
+        self, sql_queries, parameters=None, fetch_results=False, use_pandas_result=False
+    ):
         check.list_param(sql_queries, "sql_queries", of_type=str)
         check.opt_dict_param(parameters, "parameters")
         check.bool_param(fetch_results, "fetch_results")
 
-        results = []
+        if use_pandas_result:
+            results = pd.DataFrame()
+        else:
+            results = []
         with self.get_connection() as conn:
             with closing(conn.cursor()) as cursor:
                 for sql in sql_queries:
                     if sys.version_info[0] < 3:
                         sql = sql.encode("utf-8")
                     self.log.info("Executing query: " + sql)
                     cursor.execute(sql, parameters)  # pylint: disable=E1101
                     if fetch_results:
-                        results.append(cursor.fetchall())  # pylint: disable=E1101
+                        if use_pandas_result:
+                            results = results.append(cursor.fetch_pandas_all())
+                        else:
+                            results.append(cursor.fetchall())  # pylint: disable=E1101
 
         return results if fetch_results else None
 
     def load_table_from_local_parquet(self, src, table):
         check.str_param(src, "src")
         check.str_param(table, "table")
 
@@ -117,45 +164,42 @@
 
     A simple example of loading data into Snowflake and subsequently querying that data is shown below:
 
     Examples:
 
     .. code-block:: python
 
-        from dagster import execute_pipeline, pipeline, DependencyDefinition, ModeDefinition
+        from dagster import job, op
         from dagster_snowflake import snowflake_resource
 
-        @solid(required_resource_keys={'snowflake'})
+        @op(required_resource_keys={'snowflake'})
         def get_one(context):
             context.resources.snowflake.execute_query('SELECT 1')
 
-        @pipeline(
-            mode_defs=[ModeDefinition(resource_defs={'snowflake': snowflake_resource})],
-        )
-        def snowflake_pipeline():
+        @job(resource_defs={'snowflake': snowflake_resource})
+        def my_snowflake_job():
             get_one()
 
-        result = execute_pipeline(
-            snowflake_pipeline,
-            {
+        my_snowflake_job.execute_in_process(
+            run_config={
                 'resources': {
                     'snowflake': {
                         'config': {
                             'account': {'env': 'SNOWFLAKE_ACCOUNT'},
                             'user': {'env': 'SNOWFLAKE_USER'},
                             'password': {'env': 'SNOWFLAKE_PASSWORD'},
                             'database': {'env': 'SNOWFLAKE_DATABASE'},
                             'schema': {'env': 'SNOWFLAKE_SCHEMA'},
                             'warehouse': {'env': 'SNOWFLAKE_WAREHOUSE'},
                         }
                     }
                 }
-            },
+            }
         )
 
     """
-    return SnowflakeConnection(context)
+    return SnowflakeConnection(context.resource_config, context.log)
 
 
 def _filter_password(args):
     """Remove password from connection args for logging"""
     return {k: v for k, v in args.items() if k != "password"}
```

### Comparing `dagster-snowflake-0.9.9rc1/dagster_snowflake.egg-info/PKG-INFO` & `dagster-snowflake-1.0.5/dagster_snowflake.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-snowflake
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: Package for Snowflake Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Provides-Extra: snowflake.sqlalchemy
+Provides-Extra: pandas
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-snowflake-0.9.9rc1/dagster_snowflake.egg-info/SOURCES.txt` & `dagster-snowflake-1.0.5/dagster_snowflake.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 dagster_snowflake/__init__.py
 dagster_snowflake/configs.py
+dagster_snowflake/db_io_manager.py
+dagster_snowflake/py.typed
 dagster_snowflake/resources.py
+dagster_snowflake/snowflake_io_manager.py
 dagster_snowflake/solids.py
 dagster_snowflake/version.py
 dagster_snowflake.egg-info/PKG-INFO
 dagster_snowflake.egg-info/SOURCES.txt
 dagster_snowflake.egg-info/dependency_links.txt
 dagster_snowflake.egg-info/not-zip-safe
 dagster_snowflake.egg-info/requires.txt
-dagster_snowflake.egg-info/top_level.txt
-dagster_snowflake_tests/__init__.py
-dagster_snowflake_tests/test_resources.py
-dagster_snowflake_tests/test_solids.py
-dagster_snowflake_tests/test_version.py
-dagster_snowflake_tests/utils.py
+dagster_snowflake.egg-info/top_level.txt
```

