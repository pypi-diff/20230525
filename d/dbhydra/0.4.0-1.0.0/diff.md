# Comparing `tmp/dbhydra-0.4.0.tar.gz` & `tmp/dbhydra-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbhydra-0.4.0.tar", last modified: Sun Mar 12 23:53:59 2023, max compression
+gzip compressed data, was "dbhydra-1.0.0.tar", last modified: Thu May 25 14:49:13 2023, max compression
```

## Comparing `dbhydra-0.4.0.tar` & `dbhydra-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-03-12 23:53:59.417405 dbhydra-0.4.0/
--rw-rw-rw-   0        0        0     1091 2020-12-30 01:44:56.000000 dbhydra-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     2117 2023-03-12 23:53:59.416408 dbhydra-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1636 2021-12-29 21:54:01.000000 dbhydra-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-12 23:53:59.398455 dbhydra-0.4.0/dbhydra/
--rw-rw-rw-   0        0        0        0 2020-12-30 01:44:56.000000 dbhydra-0.4.0/dbhydra/__init__.py
--rw-rw-rw-   0        0        0     1682 2022-10-17 21:58:06.000000 dbhydra-0.4.0/dbhydra/dbhydra_builder.py
--rw-rw-rw-   0        0        0    62294 2023-03-12 23:52:29.000000 dbhydra-0.4.0/dbhydra/dbhydra_core.py
--rw-rw-rw-   0        0        0     2405 2022-10-17 21:58:06.000000 dbhydra-0.4.0/dbhydra/dbhydra_liquibase.py
--rw-rw-rw-   0        0        0      757 2022-10-17 21:58:06.000000 dbhydra-0.4.0/dbhydra/dbhydra_model.py
--rw-rw-rw-   0        0        0      337 2020-12-30 01:44:56.000000 dbhydra-0.4.0/dbhydra/dbhydra_mysql_example - kopie.py
--rw-rw-rw-   0        0        0     3815 2022-10-17 21:58:06.000000 dbhydra-0.4.0/dbhydra/dbhydra_mysql_example.py
--rw-rw-rw-   0        0        0      782 2022-10-17 21:58:06.000000 dbhydra-0.4.0/dbhydra/dbhydra_pandas_framework.py
--rw-rw-rw-   0        0        0     2472 2022-10-17 21:58:06.000000 dbhydra-0.4.0/dbhydra/migrator_example.py
--rw-rw-rw-   0        0        0     1836 2021-09-10 13:04:36.000000 dbhydra-0.4.0/dbhydra/mongo.py
--rw-rw-rw-   0        0        0      448 2021-12-29 18:11:09.000000 dbhydra-0.4.0/dbhydra/test.py
-drwxrwxrwx   0        0        0        0 2023-03-12 23:53:59.415410 dbhydra-0.4.0/dbhydra/tests/
--rw-rw-rw-   0        0        0        0 2023-03-12 23:52:29.000000 dbhydra-0.4.0/dbhydra/tests/__init__.py
--rw-rw-rw-   0        0        0      508 2023-03-12 23:52:29.000000 dbhydra-0.4.0/dbhydra/tests/test_cases.py
--rw-rw-rw-   0        0        0     1979 2023-03-12 23:52:29.000000 dbhydra-0.4.0/dbhydra/tests/test_mongo.py
--rw-rw-rw-   0        0        0     3126 2023-03-12 23:52:29.000000 dbhydra-0.4.0/dbhydra/tests/test_sql.py
-drwxrwxrwx   0        0        0        0 2023-03-12 23:53:59.409426 dbhydra-0.4.0/dbhydra.egg-info/
--rw-rw-rw-   0        0        0     2117 2023-03-12 23:53:58.000000 dbhydra-0.4.0/dbhydra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-03-12 23:53:59.000000 dbhydra-0.4.0/dbhydra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-12 23:53:58.000000 dbhydra-0.4.0/dbhydra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-03-12 23:53:58.000000 dbhydra-0.4.0/dbhydra.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-12 23:53:59.000000 dbhydra-0.4.0/dbhydra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-12 23:53:59.417405 dbhydra-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      782 2023-03-12 23:52:50.000000 dbhydra-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:49:13.151783 dbhydra-1.0.0/
+-rw-rw-rw-   0        0        0     1091 2020-12-30 01:44:56.000000 dbhydra-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2117 2023-05-25 14:49:13.149788 dbhydra-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1636 2021-12-29 21:54:01.000000 dbhydra-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 14:49:13.049056 dbhydra-1.0.0/dbhydra/
+-rw-rw-rw-   0        0        0        0 2020-12-30 01:44:56.000000 dbhydra-1.0.0/dbhydra/__init__.py
+-rw-rw-rw-   0        0        0     1682 2022-10-17 21:58:06.000000 dbhydra-1.0.0/dbhydra/dbhydra_builder.py
+-rw-rw-rw-   0        0        0    66388 2023-05-25 14:48:28.000000 dbhydra-1.0.0/dbhydra/dbhydra_core.py
+-rw-rw-rw-   0        0        0     2405 2022-10-17 21:58:06.000000 dbhydra-1.0.0/dbhydra/dbhydra_liquibase.py
+-rw-rw-rw-   0        0        0      757 2022-10-17 21:58:06.000000 dbhydra-1.0.0/dbhydra/dbhydra_model.py
+-rw-rw-rw-   0        0        0      337 2020-12-30 01:44:56.000000 dbhydra-1.0.0/dbhydra/dbhydra_mysql_example - kopie.py
+-rw-rw-rw-   0        0        0     3815 2022-10-17 21:58:06.000000 dbhydra-1.0.0/dbhydra/dbhydra_mysql_example.py
+-rw-rw-rw-   0        0        0      782 2022-10-17 21:58:06.000000 dbhydra-1.0.0/dbhydra/dbhydra_pandas_framework.py
+-rw-rw-rw-   0        0        0     2472 2022-10-17 21:58:06.000000 dbhydra-1.0.0/dbhydra/migrator_example.py
+-rw-rw-rw-   0        0        0     1836 2021-09-10 13:04:36.000000 dbhydra-1.0.0/dbhydra/mongo.py
+-rw-rw-rw-   0        0        0      448 2021-12-29 18:11:09.000000 dbhydra-1.0.0/dbhydra/test.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:49:13.147794 dbhydra-1.0.0/dbhydra/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-12 23:52:29.000000 dbhydra-1.0.0/dbhydra/tests/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-03-12 23:52:29.000000 dbhydra-1.0.0/dbhydra/tests/test_cases.py
+-rw-rw-rw-   0        0        0     1979 2023-03-12 23:52:29.000000 dbhydra-1.0.0/dbhydra/tests/test_mongo.py
+-rw-rw-rw-   0        0        0     3126 2023-03-12 23:52:29.000000 dbhydra-1.0.0/dbhydra/tests/test_sql.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:49:13.087952 dbhydra-1.0.0/dbhydra.egg-info/
+-rw-rw-rw-   0        0        0     2117 2023-05-25 14:49:11.000000 dbhydra-1.0.0/dbhydra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-05-25 14:49:12.000000 dbhydra-1.0.0/dbhydra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 14:49:11.000000 dbhydra-1.0.0/dbhydra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-25 14:49:11.000000 dbhydra-1.0.0/dbhydra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 14:49:12.000000 dbhydra-1.0.0/dbhydra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 14:49:13.152780 dbhydra-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      782 2023-05-25 14:49:03.000000 dbhydra-1.0.0/setup.py
```

### Comparing `dbhydra-0.4.0/LICENSE` & `dbhydra-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbhydra-0.4.0/PKG-INFO` & `dbhydra-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 0.4.0
+Version: 1.0.0
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dbhydra-0.4.0/README.md` & `dbhydra-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dbhydra-0.4.0/dbhydra/dbhydra_builder.py` & `dbhydra-1.0.0/dbhydra/dbhydra_builder.py`

 * *Files identical despite different names*

### Comparing `dbhydra-0.4.0/dbhydra/dbhydra_core.py` & `dbhydra-1.0.0/dbhydra/dbhydra_core.py`

 * *Files 9% similar despite different names*

```diff
@@ -97,28 +97,27 @@
             migration_dict = {
                 "modify_column": {"table_name": instance.name, "column_name": args[0], "column_type": args[1]}}
             print(migration_dict)
         # TODO: add other methods
 
         migrator = instance.db1.migrator
         migrator.migration_list.append(migration_dict)
-        migrator.migration_list_to_json()
+        # migrator.migration_list_to_json()
         function(instance, *args, **kw)
 
     return (new_function)
 
 
 # class DataMigrator:
 
 
 
 class Migrator:
-    def __init__(self, db=None, db2=None):
+    def __init__(self, db=None):
         self.db = db
-        self.db2 = db2
         self.migration_number = 1
         self.migration_list = []
 
     def process_migration_dict(self, migration_dict):
         assert len(migration_dict.keys()) == 1
         operation = list(migration_dict.keys())[0]
         options = migration_dict[operation]
@@ -232,14 +231,35 @@
             columns.insert(0, "id")
             return_types.insert(0, "int")
 
         return columns, return_types
 
 
 class AbstractDB(abc.ABC):
+    typing_to_python_mapping = {
+        'List': 'list',
+        'Dict': 'dict',
+        'Tuple': 'tuple',
+        'Set': 'set',
+        'Union': 'object',
+        'Optional': 'object',
+        # 'FrozenSet': frozenset,
+        # 'Deque': list,
+        # 'Any': object,
+        #
+        # 'Callable': object,
+        # 'Type': type,
+        # 'TypeVar': object,
+        # 'Generic': object,
+        # 'Sequence': list,
+        # 'Iterable': list,
+        # 'Mapping': dict,
+        # 'AbstractSet': set,
+    }
+    python_database_type_mapping = {}
     def __init__(self, config_file="config.ini", db_details=None):
         if db_details is None:
             db_details = read_connection_details(config_file)
 
         self.locally = True
         if db_details["LOCALLY"] == "False":
             self.locally = False
@@ -322,16 +342,26 @@
         self.cursor.execute(query)
         self.cursor.commit()
 
     def close_connection(self):
         self.connection.close()
         print("DB connection closed")
 
-    def initialize_migrator(self, other_db=None):
-        self.migrator = Migrator(self, other_db)
+    def initialize_migrator(self):
+        self.migrator = Migrator(self)
+
+    def _convert_column_type_dict_from_python(self, column_type_dict):
+        """
+        First apply mapping from python typing module to standard python.
+        Then apply mapping from python to database types
+        """
+        typing_python_mapping = {column_name: self.typing_to_python_mapping.get(column_type,column_type) for column_name, column_type in column_type_dict.items()}
+        return {column_name: self.python_database_type_mapping[column_type] for column_name, column_type in typing_python_mapping.items()}
+
+
 
 
 class AbstractDBPostgres(AbstractDB):
     # TODO: Config_mongo.ini in postgres?
     def __init__(self, config_file="config-mongo.ini", db_details=None):
         super().__init__(config_file, db_details)
 
@@ -410,14 +440,26 @@
                   "referenced_column_id": row[3] - 1}  # minus 1 because of indexing from 0
             foreign_keys.append(fk)
 
         return (foreign_keys)
 
 
 class Mysqldb(AbstractDB):
+
+    python_database_type_mapping = PYTHON_TO_MYSQL_DATA_MAPPING = \
+    {
+    'int': "int",
+    'float': "double",
+    'str': "varchar(255)",
+    'list': "varchar(255)",
+    'dict': "varchar(255)",
+    'bool': "tinyint",
+    'datetime': "datetime"
+    }
+
     def connect_locally(self):
         self.connection = MySQLdb.connect(host=self.DB_SERVER, user=self.DB_USERNAME, password=self.DB_PASSWORD,
                                           database=self.DB_DATABASE)
         self.cursor = self.connection.cursor()
         print("DB connection established")
 
     def connect_remotely(self):
@@ -498,30 +540,32 @@
         for i, table in enumerate(tables):
             table_dict[table] = PostgresTable.init_all_columns(self, table)
 
         return (table_dict)
 
 
 class BigQueryDb(AbstractDB):
-    def __init__(self, credentials_path, project_id, dataset_name):
-        # super().__init__(None,None)
-        self.credentials_path = credentials_path
-        self.project_id = project_id
-        self.dataset = dataset_name
+    def __init__(self, db_details):
+        self.credentials_path = db_details["DB_SERVER"]
+        self.dataset = db_details["DB_DATABASE"]
+
+
+        self.locally = False
 
         self.credentials = service_account.Credentials.from_service_account_file(self.credentials_path, scopes=[
             "https://www.googleapis.com/auth/cloud-platform"], )
 
 
     def connect_remotely(self):
         self.client = bigquery.Client(credentials=self.credentials, project=self.credentials.project_id)
 
     def connect_locally(self):
         raise Exception("Cannot connect locally to Big Query")
 
+
     def close_connection(self):
         self.client.close()
 
     def select_to_df(self, query):
         print(query)
         df = pd.read_gbq(query=query, project_id=self.project_id, credentials=self.credentials)
 
@@ -544,35 +588,17 @@
 
         return (table_dict)
 
 
 
 
     def execute(self, query):
-        # query_job = self.client.query(
-        #     """
-        #     SELECT
-        #       CONCAT(
-        #         'https://stackoverflow.com/questions/',
-        #         CAST(id as STRING)) as url,
-        #       view_count
-        #     FROM `bigquery-public-data.stackoverflow.posts_questions`
-        #     WHERE tags like '%google-bigquery%'
-        #     ORDER BY view_count DESC
-        #     LIMIT 10"""
-        # )
-
         query_job = self.client.query(query)
-
         results = query_job.result()  # Waits for job to complete.
-
-        for row in results:
-            print(row)
-
-            # print("{} : {} views".format(row.id, row.link,row.title))
+        return results
 
 
 class MongoDb(AbstractDBMongo):
 
     def connect_locally(self):
         self.connection = pymongo.MongoClient(
             host=self.DB_SERVER,
@@ -763,16 +789,24 @@
     def insert_from_df(self, df, batch=1, try_mode=False, debug_mode=False, adjust_df=False, insert_id=False):
 
         if adjust_df:
             df = self._adjust_df(df, debug_mode)
 
         if insert_id:
             assert len(df.columns) == len(self.columns)
+            assert set(df.columns) == set(self.columns)
         else:
             assert len(df.columns) + 1 == len(self.columns) # +1 because of id column
+            sql_columns = set(self.columns)
+            sql_columns.remove('id')
+            assert set(df.columns) == sql_columns
+
+        df = df[self.columns]
+
+
         pd_nullable_dtypes = {pd.Int8Dtype(), pd.Int16Dtype(), pd.Int32Dtype(), pd.Int64Dtype(),
                               pd.UInt8Dtype(), pd.UInt16Dtype(), pd.UInt32Dtype(), pd.UInt64Dtype(),
                               pd.Float32Dtype(), pd.Float64Dtype()}
         pd_nullable_columns = df.dtypes.isin(pd_nullable_dtypes)
 
         # cast pd nullable columns to float - changing to 'NULL' then proceeds without an error.
         # in database floats are again casted to integers where required
@@ -786,14 +820,26 @@
         rows = df.values.tolist()
         for i, row in enumerate(rows):
             for j, record in enumerate(row):
                 if type(record) == str:
                     rows[i][j] = "'" + record + "'"
         self.insert(rows, batch=batch, try_mode=try_mode, debug_mode=False, insert_id=insert_id)
 
+    #TODO: need to solve inserting in different column_order
+    #check df column names, permute if needed
+    def insert_from_column_value_dict(self, dict, insert_id=False):
+        df = pd.DataFrame(dict, index=[0])
+        self.insert_from_df(df, insert_id=insert_id)
+
+    def insert_from_column_value_dict_list(self, list, insert_id=False):
+        df = pd.DataFrame(list)
+        self.insert_from_df(df, insert_id=insert_id)
+
+
+
     def delete(self, where=None):
 
         if where is None:
             query = "DELETE FROM " + self.name
         else:
             query = "DELETE FROM " + self.name + " WHERE " + where
         print(query)
@@ -810,17 +856,14 @@
     def initialize_columns(self):
         information_schema_table = Table(self.db1, 'INFORMATION_SCHEMA.COLUMNS')
         query = f"SELECT COLUMN_NAME FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_NAME  = '" + self.name + "';"
         columns = information_schema_table.select(query)
         self.columns = columns
 
     def initialize_types(self):
-        # information_schema_table = Table(self.db1, 'INFORMATION_SCHEMA.COLUMNS', ['DATA_TYPE'], ['nvarchar(50)'])
-        # query = f"SELECT DATA_TYPE FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_NAME  = '" + self.name + "'"
-        # types = information_schema_table.select(query)
         self.types = self.get_all_types()
 
     def get_all_columns(self):
         information_schema_table = Table(self.db1, 'INFORMATION_SCHEMA.COLUMNS')
         query = "SELECT COLUMN_NAME FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_NAME  = '" + self.name + "'"
         columns = information_schema_table.select(query)
 
@@ -832,23 +875,23 @@
         self.types = postgres_types
 
     def get_all_types(self):
 
         information_schema_table = Table(self.db1, 'INFORMATION_SCHEMA.COLUMNS', ['DATA_TYPE'], ['nvarchar(50)'])
         query = "SELECT DATA_TYPE,character_maximum_length FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_NAME  = '" + self.name + "'"
         types = information_schema_table.select(query)
-        types = [x[0] for x in types]
-        types = [x.lower() for x in types]
-        lengths = [x[1] for x in types]
+        data_types = [x[0].lower() for x in types]
+        date_lengths = [x[1] for x in types]
+
+        mysql_types = list(map(lambda x: POSTGRES_TO_MYSQL_DATA_MAPPING.get(x, x), data_types))
 
-        mysql_types = list(map(lambda x: POSTGRES_TO_MYSQL_DATA_MAPPING.get(x, x), types))
 
         for i in range(len(mysql_types)):
-            if lengths[i] is not None:
-                mysql_types[i] = mysql_types[i] + f"({lengths[i]})"
+            if date_lengths[i] is not None:
+                mysql_types[i] = mysql_types[i] + f"({date_lengths[i]})"
 
         return (mysql_types)
 
 
     def select_all(self):
         print(super().select_all())
         return [i for i in super().select_all()]
@@ -998,35 +1041,46 @@
         try:
             self.db1.execute(command)
             index = self.columns.index(column_name)
             self.types[index] = new_column_type
         except Exception as e:
             print("Cant add column to table.")
 
-class BigQueryTable():
-    def __init__(self, db, name, columns=None, types=None):
+class BigQueryTable(AbstractSelectable):
+    def __init__(self, db1, name, columns=None, types=None):
         self.name = name
-        self.db = db
+        self.db1 = db1
         self.columns = columns
         self.types = types
 
     @classmethod
     def init_all_columns(cls, db1, name):
         temporary_table = cls(db1, name)
         columns,types = temporary_table.get_all_columns_and_types()
 
         return (cls(db1, name, columns, types))
 
     def get_all_columns_and_types(self):
-        results = self.db.client.get_table(self.name)
+        results = self.db1.client.get_table(f"{self.db1.credentials.project_id}.{self.db1.dataset}.{self.name}")
         column_names = [x.name for x in results.schema ]
         column_types = [x.field_type for x in results.schema]
         return column_names, column_types
 
 
+    def select(self, query):
+
+        """given SELECT query returns Python list"""
+        """Columns give the number of selected columns"""
+        print(query)
+        # rows =  self.db1.client.query(query).result()
+        rows = self.db1.execute(query)
+        return rows
+
+
+
 
 class MongoTable():
     def __init__(self, db, name, columns=[], types=[]):
         self.name = name
         self.db1 = db
         print("==========================================")
         print(type(db))
@@ -1306,49 +1360,82 @@
 
 
 class MysqlTable(MysqlSelectable, AbstractTable):
     def __init__(self, db1, name, columns=None, types=None):
         super().__init__(db1, name, columns)
         self.types = types
 
+    @classmethod
+    def init_from_column_type_dict(cls, db1, name, column_type_dict):
+        column_converted_type_dict = db1._convert_column_type_dict_from_python(column_type_dict)
+        columns = list(column_converted_type_dict.keys())
+        types = list(column_converted_type_dict.values())
+        return cls(db1, name, columns, types)
+
     def initialize_columns(self):
         information_schema_table = Table(self.db1, 'INFORMATION_SCHEMA.COLUMNS')
         query = f"SELECT COLUMN_NAME FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_SCHEMA = '{self.db1.DB_DATABASE}' AND  TABLE_NAME  = '" + self.name + "';"
         columns = information_schema_table.select(query)
         self.columns = columns
 
     def convert_types_from_mysql(self):
         pass
 
     def initialize_types(self):
-        # information_schema_table = Table(self.db1, 'INFORMATION_SCHEMA.COLUMNS', ['DATA_TYPE'], ['nvarchar(50)'])
-        # query = f"SELECT COLUMN_TYPE FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_SCHEMA = '{self.db1.DB_DATABASE}' AND TABLE_NAME  = '" + self.name + "'"
-        # types = information_schema_table.select(query)
         self.types = self.get_all_types()
 
     def get_all_columns(self):
         information_schema_table = Table(self.db1, 'INFORMATION_SCHEMA.COLUMNS')
         query = f"SELECT COLUMN_NAME FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_SCHEMA = '{self.db1.DB_DATABASE}' AND TABLE_NAME  = '" + self.name + "'"
         columns = information_schema_table.select(query)
 
         return (columns)
 
     def get_all_types(self):
 
+        data_types, data_lengths = self.get_data_types_and_character_lengths()
+        for i in range(len(data_types)):
+            if data_lengths[i] is not None:
+                data_types[i] = data_types[i] + f"({data_lengths[i]})"
+        return (data_types)
+
+
+    """
+        Returns a list of data types, where each element represents the category of the data ('varchar', 'int', etc.). 
+        If a data type has an associated length, the length value will be included in a corresponding element of the
+        data_lengths list, otherwise the element will have a None value. For example, 'varchar(255)' would return
+        'varchar' in the data_types list and 255 in the data_lengths list.
+    """
+    def get_data_types_and_character_lengths(self):
         information_schema_table = Table(self.db1, 'INFORMATION_SCHEMA.COLUMNS', ['DATA_TYPE'], ['nvarchar(50)'])
         query = f"SELECT DATA_TYPE,character_maximum_length FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_SCHEMA = '{self.db1.DB_DATABASE}' AND TABLE_NAME  = '" + self.name + "'"
         types = information_schema_table.select(query)
-        only_types = [x[0] for x in types]
-        lengths = [x[1] for x in types]
+        data_types = [x[0] for x in types]
+        data_lengths = [x[1] for x in types]
+
+        return data_types,data_lengths
+
+    def get_converted_python_types(self):
+        SQL_TO_PYTHON = {v: k for k, v in PYTHON_TO_MYSQL_DATA_MAPPING.items()}
+        python_types = []
+        for type in self.types:
+            if "varchar" in type:
+                python_types.append("str")
+            elif type in SQL_TO_PYTHON:
+                python_types.append(SQL_TO_PYTHON[type])
+            else:
+                raise Exception("Unsupported type")
 
-        for i in range(len(only_types)):
-            if lengths[i] is not None:
-                only_types[i] = only_types[i] + f"({lengths[i]})"
-        return (only_types)
+        return python_types
 
+    def get_nullable_columns(self):
+        information_schema_table = Table(self.db1, 'INFORMATION_SCHEMA.COLUMNS')
+        query = f"SELECT COLUMN_NAME FROM INFORMATION_SCHEMA.COLUMNS where TABLE_SCHEMA = '{self.db1.DB_DATABASE}' and TABLE_NAME = '{self.name}' and IS_NULLABLE = 'YES'"
+        nullable_columns = information_schema_table.select(query)
+        return (nullable_columns)
 
 
     @classmethod
     def init_all_columns(cls, db1, name):
         temporary_table = cls(db1, name)
         columns = temporary_table.get_all_columns()
         types = temporary_table.get_all_types()
@@ -1369,14 +1456,23 @@
         Returns the biggest id from table
         """
 
         last_id = self.select(f"SELECT id FROM {self.name} ORDER BY id DESC LIMIT 1;")
 
         return last_id[0][0]
 
+    def get_num_of_records(self):
+        """
+        Returns the number of records in table
+        """
+
+        num_of_records = self.select(f"SELECT COUNT(*) FROM {self.name};")
+
+        return num_of_records[0][0]
+
     def drop(self):
         query = "DROP TABLE " + self.name + ";"
         print(query)
         self.db1.execute(query)
 
     # @save_migration #TODO: Uncomment
     def create(self, foreign_keys=None):
@@ -1658,8 +1754,30 @@
 def df_to_dict(df, column1, column2):
     dictionary = df.set_index(column1).to_dict()[column2]
     return (dictionary)
 
 
 def dict_to_df(dictionary, column1, column2):
     df = pd.DataFrame(list(dictionary.items()), columns=[column1, column2])
-    return (df)
+    return (df)
+
+from pydantic import BaseModel
+from typing import List, Dict
+
+class AbstractModel(abc.ABC, BaseModel):
+    def generate_dbhydra_table(self, db1, name):
+        structure_dict = create_table_structure_dict(self)
+        #TODO: what type of table, TEST
+        dbhydra_table = MysqlTable(db1, name, list(structure_dict.keys()), list(structure_dict.values()))
+        return dbhydra_table
+
+
+
+def create_table_structure_dict(api_class_instance):
+    """
+    Accepts instance of API data class (e.g. APIDatabase) and converts it to dictionary {attribute_name: attribute_type}
+    """
+    table_structure_dict = {"id": "int"}
+    table_structure_dict = {**table_structure_dict,
+                            **{attribute_name: attribute_type.__name__ for attribute_name, attribute_type in api_class_instance.__annotations__.items()}}
+
+    return table_structure_dict
```

### Comparing `dbhydra-0.4.0/dbhydra/dbhydra_liquibase.py` & `dbhydra-1.0.0/dbhydra/dbhydra_liquibase.py`

 * *Files identical despite different names*

### Comparing `dbhydra-0.4.0/dbhydra/dbhydra_model.py` & `dbhydra-1.0.0/dbhydra/dbhydra_model.py`

 * *Files identical despite different names*

### Comparing `dbhydra-0.4.0/dbhydra/dbhydra_mysql_example.py` & `dbhydra-1.0.0/dbhydra/dbhydra_mysql_example.py`

 * *Files identical despite different names*

### Comparing `dbhydra-0.4.0/dbhydra/dbhydra_pandas_framework.py` & `dbhydra-1.0.0/dbhydra/dbhydra_pandas_framework.py`

 * *Files identical despite different names*

### Comparing `dbhydra-0.4.0/dbhydra/migrator_example.py` & `dbhydra-1.0.0/dbhydra/migrator_example.py`

 * *Files identical despite different names*

### Comparing `dbhydra-0.4.0/dbhydra/mongo.py` & `dbhydra-1.0.0/dbhydra/mongo.py`

 * *Files identical despite different names*

### Comparing `dbhydra-0.4.0/dbhydra/tests/test_mongo.py` & `dbhydra-1.0.0/dbhydra/tests/test_mongo.py`

 * *Files identical despite different names*

### Comparing `dbhydra-0.4.0/dbhydra/tests/test_sql.py` & `dbhydra-1.0.0/dbhydra/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `dbhydra-0.4.0/dbhydra.egg-info/PKG-INFO` & `dbhydra-1.0.0/dbhydra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 0.4.0
+Version: 1.0.0
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dbhydra-0.4.0/dbhydra.egg-info/SOURCES.txt` & `dbhydra-1.0.0/dbhydra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbhydra-0.4.0/setup.py` & `dbhydra-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='dbhydra',
-    version='0.4.0',
+    version='1.0.0',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Data science friendly ORM combining Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/dbhydra',
     packages=setuptools.find_packages(),
```

