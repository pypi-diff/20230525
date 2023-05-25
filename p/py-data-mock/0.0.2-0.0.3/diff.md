# Comparing `tmp/py-data-mock-0.0.2.tar.gz` & `tmp/py-data-mock-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-data-mock-0.0.2.tar", last modified: Tue May 23 16:41:37 2023, max compression
+gzip compressed data, was "py-data-mock-0.0.3.tar", last modified: Thu May 25 03:13:30 2023, max compression
```

## Comparing `py-data-mock-0.0.2.tar` & `py-data-mock-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/
--rw-rw-r--   0 henry     (1000) henry     (1000)    35149 2023-05-20 20:50:55.000000 py-data-mock-0.0.2/LICENSE
--rw-rw-r--   0 henry     (1000) henry     (1000)      363 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/PKG-INFO
--rw-rw-r--   0 henry     (1000) henry     (1000)     3841 2023-05-23 16:41:34.000000 py-data-mock-0.0.2/README.md
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.693477 py-data-mock-0.0.2/data_mock/
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.693477 py-data-mock-0.0.2/data_mock/google/
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.693477 py-data-mock-0.0.2/data_mock/google/cloud/
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/
--rw-rw-r--   0 henry     (1000) henry     (1000)      583 2023-05-20 20:51:44.000000 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/__init__.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     3969 2023-05-23 07:44:51.000000 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/client.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      301 2023-05-20 20:51:44.000000 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/dataset.py
--rw-rw-r--   0 henry     (1000) henry     (1000)       85 2023-05-20 20:51:44.000000 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/exceptions.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/job/
--rw-rw-r--   0 henry     (1000) henry     (1000)       70 2023-05-20 20:51:44.000000 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/job/__init__.py
--rw-rw-r--   0 henry     (1000) henry     (1000)       80 2023-05-20 20:51:44.000000 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/job/query.py
--rw-rw-r--   0 henry     (1000) henry     (1000)       22 2023-05-20 20:51:44.000000 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/retry.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      169 2023-05-20 20:51:44.000000 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/schema.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     2974 2023-05-23 07:44:51.000000 py-data-mock-0.0.2/data_mock/google/cloud/bigquery/table.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/data_mock/google/cloud/storage/
--rw-rw-r--   0 henry     (1000) henry     (1000)      110 2023-05-23 16:41:34.000000 py-data-mock-0.0.2/data_mock/google/cloud/storage/__init__.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     1228 2023-05-23 16:41:34.000000 py-data-mock-0.0.2/data_mock/google/cloud/storage/blob.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      522 2023-05-23 16:41:34.000000 py-data-mock-0.0.2/data_mock/google/cloud/storage/bucket.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      445 2023-05-23 16:41:34.000000 py-data-mock-0.0.2/data_mock/google/cloud/storage/client.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/data_mock/mock_helpers/
--rw-rw-r--   0 henry     (1000) henry     (1000)     1983 2023-05-23 07:44:51.000000 py-data-mock-0.0.2/data_mock/mock_helpers/provider.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      116 2023-05-23 16:41:34.000000 py-data-mock-0.0.2/data_mock/mock_helpers/writer.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/data_mock/scripts/
--rw-rw-r--   0 henry     (1000) henry     (1000)     2245 2023-05-20 20:51:44.000000 py-data-mock-0.0.2/data_mock/scripts/mkmock.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/py_data_mock.egg-info/
--rw-rw-r--   0 henry     (1000) henry     (1000)      363 2023-05-23 16:41:37.000000 py-data-mock-0.0.2/py_data_mock.egg-info/PKG-INFO
--rw-rw-r--   0 henry     (1000) henry     (1000)      837 2023-05-23 16:41:37.000000 py-data-mock-0.0.2/py_data_mock.egg-info/SOURCES.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-05-23 16:41:37.000000 py-data-mock-0.0.2/py_data_mock.egg-info/dependency_links.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      122 2023-05-23 16:41:37.000000 py-data-mock-0.0.2/py_data_mock.egg-info/top_level.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)       38 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/setup.cfg
--rw-rw-r--   0 henry     (1000) henry     (1000)      636 2023-05-23 16:41:34.000000 py-data-mock-0.0.2/setup.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-23 16:41:37.697477 py-data-mock-0.0.2/tests/
--rw-rw-r--   0 henry     (1000) henry     (1000)     1167 2023-05-20 20:54:11.000000 py-data-mock-0.0.2/tests/test1.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-25 03:13:30.955690 py-data-mock-0.0.3/
+-rw-rw-r--   0 henry     (1000) henry     (1000)    35149 2023-05-20 20:50:55.000000 py-data-mock-0.0.3/LICENSE
+-rw-rw-r--   0 henry     (1000) henry     (1000)      363 2023-05-25 03:13:30.955690 py-data-mock-0.0.3/PKG-INFO
+-rw-rw-r--   0 henry     (1000) henry     (1000)     4391 2023-05-24 05:45:14.000000 py-data-mock-0.0.3/README.md
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-25 03:13:30.951690 py-data-mock-0.0.3/data_mock/
+-rw-rw-r--   0 henry     (1000) henry     (1000)       53 2023-05-25 03:01:07.000000 py-data-mock-0.0.3/data_mock/__init__.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)       43 2023-05-23 07:44:51.000000 py-data-mock-0.0.3/data_mock/exceptions.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-25 03:13:30.951690 py-data-mock-0.0.3/data_mock/google/
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-25 03:13:30.951690 py-data-mock-0.0.3/data_mock/google/cloud/
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-25 03:13:30.955690 py-data-mock-0.0.3/data_mock/google/cloud/bigquery/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      583 2023-05-20 20:51:44.000000 py-data-mock-0.0.3/data_mock/google/cloud/bigquery/__init__.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     4201 2023-05-25 03:01:07.000000 py-data-mock-0.0.3/data_mock/google/cloud/bigquery/client.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      301 2023-05-20 20:51:44.000000 py-data-mock-0.0.3/data_mock/google/cloud/bigquery/dataset.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)       85 2023-05-20 20:51:44.000000 py-data-mock-0.0.3/data_mock/google/cloud/bigquery/exceptions.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-25 03:13:30.955690 py-data-mock-0.0.3/data_mock/google/cloud/bigquery/job/
+-rw-rw-r--   0 henry     (1000) henry     (1000)       70 2023-05-20 20:51:44.000000 py-data-mock-0.0.3/data_mock/google/cloud/bigquery/job/__init__.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)       80 2023-05-20 20:51:44.000000 py-data-mock-0.0.3/data_mock/google/cloud/bigquery/job/query.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)       22 2023-05-20 20:51:44.000000 py-data-mock-0.0.3/data_mock/google/cloud/bigquery/retry.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      169 2023-05-20 20:51:44.000000 py-data-mock-0.0.3/data_mock/google/cloud/bigquery/schema.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2974 2023-05-23 07:44:51.000000 py-data-mock-0.0.3/data_mock/google/cloud/bigquery/table.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-25 03:13:30.955690 py-data-mock-0.0.3/data_mock/google/cloud/storage/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      110 2023-05-23 16:41:34.000000 py-data-mock-0.0.3/data_mock/google/cloud/storage/__init__.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1228 2023-05-23 16:41:34.000000 py-data-mock-0.0.3/data_mock/google/cloud/storage/blob.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      522 2023-05-23 16:41:34.000000 py-data-mock-0.0.3/data_mock/google/cloud/storage/bucket.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      445 2023-05-23 16:41:34.000000 py-data-mock-0.0.3/data_mock/google/cloud/storage/client.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-25 03:13:30.955690 py-data-mock-0.0.3/data_mock/mock_helpers/
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2238 2023-05-25 03:01:07.000000 py-data-mock-0.0.3/data_mock/mock_helpers/provider.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      116 2023-05-23 16:41:34.000000 py-data-mock-0.0.3/data_mock/mock_helpers/writer.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-25 03:13:30.955690 py-data-mock-0.0.3/data_mock/scripts/
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2245 2023-05-20 20:51:44.000000 py-data-mock-0.0.3/data_mock/scripts/mkmock.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-25 03:13:30.955690 py-data-mock-0.0.3/py_data_mock.egg-info/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      363 2023-05-25 03:13:30.000000 py-data-mock-0.0.3/py_data_mock.egg-info/PKG-INFO
+-rw-rw-r--   0 henry     (1000) henry     (1000)      883 2023-05-25 03:13:30.000000 py-data-mock-0.0.3/py_data_mock.egg-info/SOURCES.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-05-25 03:13:30.000000 py-data-mock-0.0.3/py_data_mock.egg-info/dependency_links.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      132 2023-05-25 03:13:30.000000 py-data-mock-0.0.3/py_data_mock.egg-info/top_level.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)       38 2023-05-25 03:13:30.955690 py-data-mock-0.0.3/setup.cfg
+-rw-rw-r--   0 henry     (1000) henry     (1000)      649 2023-05-25 03:01:07.000000 py-data-mock-0.0.3/setup.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-25 03:13:30.955690 py-data-mock-0.0.3/tests/
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1167 2023-05-20 20:54:11.000000 py-data-mock-0.0.3/tests/test1.py
```

### Comparing `py-data-mock-0.0.2/LICENSE` & `py-data-mock-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.2/README.md` & `py-data-mock-0.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -39,38 +39,51 @@
 
 As Subclass
 ------------
 ```python
 
 class Client(bigquery.Client):
 
-    def __init__(self):
+    def register_initial_mock_data(self):
         mock_data = [
                 [('field', 'value')
                     ]
                 ]
-        super().__init__(mock_data = mock_data)
+        self.data_provider.add_data(data = mock_data, tag = 'default')
 
 bigquery_client = Client()
-result = bigquery_client.query(SQL)
+result = bigquery_client.query("""SELECT * FROM TABLE""")
 print(f'total rows are {result.total_rows}')
 for i in result: 
     field_value = i.get('field')
     print(f'field_value is {field_value}')
 ```
 
 Register Data for Each SQL
 --------------------------
 
 You can register results for different queries. In the comment section of the SQL, put:
 ``` py-bigquery-mock-register: <tag> ```
 
 
 ```python
-bigquery_client = bigquery.Client()
+import  data_mock.google.cloud.bigquery  as bigquery
+
+class Client(bigquery.Client):
+
+    def register_initial_mock_data(self):
+        mock_data =[   
+                    [   ('name', '10th & Red River'),
+                        ('status', 'active'),
+                        ('address', '699 East 10th Street')],
+                    [   ('name', '11th & Salina'),
+                        ('status', 'active'),
+                        ('address', '1705 E 11th St')]]
+        self.data_provider.add_data(data = mock_data, tag = 'bikeshare-name-status-address')
+
 
 SQL="""
             /*
             py-bigquery-mock-register: bikeshare-name-status-address
 
             */
         SELECT
@@ -78,44 +91,44 @@
     FROM
       `bigquery-public-data.austin_bikeshare.bikeshare_stations`
       order by name, status, address
     LIMIT
       2
 """
 
-mock_data =[   
-            [   ('name', '10th & Red River'),
-                ('status', 'active'),
-                ('address', '699 East 10th Street')],
-            [   ('name', '11th & Salina'),
-                ('status', 'active'),
-                ('address', '1705 E 11th St')]]
-
-
-bigquery_client.register_mock_data(key = 'bikeshare-name-status-address', 
-        mock_data = mock_data)
-
-result1 = bigquery_client.query(query = "SELECT * FROM `bigquery-public-data.austin_bikeshare.bikeshare_stations`"
-)
+bigquery_client = Client()
+result1 = bigquery_client.query("""SELECT * FROM TABLE""")
 for i in result1:
     print('nothing found, because data not registered')
 result2 = bigquery_client.query(query = SQL)
 for i in result2:
     for j in i.items():
         print(j)
+        """
+('name', '10th & Red River')
+('status', 'active')
+('address', '699 East 10th Street')
+('name', '11th & Salina')
+('status', 'active')
+('address', '1705 E 11th St')
+
+        """
 ```
 
 Custom Classes to Provide Data
 -------------------------------
 
 A class can be used to provide results to a query. The class below will return no data with the first call, but data on the second call.
 The class must provide a method `query_results`, and this method must returns two objects: a generator, and a dictionary of metadata.
 
 
 ```python
+import  data_mock.google.cloud.bigquery  as bigquery
+import data_mock.mock_helpers.provider as provider
+
 class ProviderData1:
 
     def __init__(self):
         self.__call_no = 0
 
     def gen_func1(self):
         for i in range(10):
@@ -129,26 +142,34 @@
         self.__call_no += 1
         if self.__call_no == 1:
             return self.gen_func2(), {'total_rows':0}
         else:
             return self.gen_func1(), {'total_rows':10}
 
 
-client = bigquery.Client(mock_data = ProviderData1())
+class Client(bigquery.Client):
+
+    def register_initial_mock_data(self):
+        self.data_provider.add_data(data =ProviderData1(), tag = 'default')
+
+
+client = Client()
+
+
 sql = "SELECT * FROM table"
 result1 = client.query(query = sql)
-self.assertEqual(result1.total_rows, 0)
+assert result1.total_rows == 0
 #loop should not be entered
 for i in result1:
     assert False
 result2 = client.query(query = sql)
-self.assertEqual(result2.total_rows, 10)
+assert result2.total_rows == 10
 for i in result2:
     for j in i.items():
-        self.assertEqual(j, ('field', 0))
+        assert j ==  ('field', 0)
     break
 
 ```
 Storage
 ========
 
 ```python
```

### Comparing `py-data-mock-0.0.2/data_mock/google/cloud/bigquery/__init__.py` & `py-data-mock-0.0.3/data_mock/google/cloud/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.2/data_mock/google/cloud/bigquery/client.py` & `py-data-mock-0.0.3/data_mock/google/cloud/bigquery/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from . import exceptions
 from .  import table as _table
 from .job import query as job_query
 from . import retry as retries
 from . import dataset as _dataset
 import data_mock.mock_helpers.provider as provider
+import data_mock.exceptions as exceptions
 
 from typing import Union, Optional
 
 # these values do nothing
 DEFAULT_RETRY = None
 DEFAULT_TIMEOUT = None
 DEFAULT_JOB_RETRY = None
@@ -15,41 +15,48 @@
 
 class Client:
 
     def __init__(self, project = None, mock_data = None, 
             mock_list_of_tables = None):
         self.project = project
         self.__list_of_tables = mock_list_of_tables
-        self._data_provider = provider.ProvideData()
+        self.data_provider = provider.ProvideData()
         if mock_data:
-            self._data_provider.add_data(data = mock_data, tag = 'default_')
+            self.data_provider.add_data(data = mock_data, tag = 'default')
+        self.register_initial_mock_data()
 
     def register_mock_data(self, key, mock_data):
-        self._data_provider.add_data(data = mock_data, tag = key)
+        self.data_provider.add_data(data = mock_data, tag = key)
+
+    def register_initial_mock_data(self):
+        pass
 
     def query(self, query,
-        job_config: job_query.QueryJobConfig = None,
+        job_config: Optional[job_query.QueryJobConfig] = None,
         job_id: str = None,
         job_id_prefix: str = None,
         location: str = None,
         project: str = None,
         retry: retries.Retry = DEFAULT_RETRY,
         timeout: TimeoutType = DEFAULT_TIMEOUT,
         job_retry: retries.Retry = DEFAULT_JOB_RETRY,
               ):
         """
         all args ignored except query
         """
         key = self._get_sql_key(query)
         if key:
-            data, m = self._data_provider.get_data(key)
+            data, m = self.data_provider.get_data(key)
             if not data:
                 raise exceptions.InvalidMockData(f'{key} not found in registered_data')
         else:
-            data, m = self._data_provider.get_data('default_')
+            try:
+                data, m = self.data_provider.get_data('default')
+            except TypeError:
+                raise exceptions.InvalidMockData(f'bad class')
         return _table.RowIterator(data = data, m = m)
 
     def create_table(self,
             table: Union[str, _table.Table, _table.TableReference, _table.TableListItem],
             exists_ok: bool = False,
             retry: retries.Retry = DEFAULT_RETRY,
             timeout: TimeoutType = DEFAULT_TIMEOUT,
```

### Comparing `py-data-mock-0.0.2/data_mock/google/cloud/bigquery/table.py` & `py-data-mock-0.0.3/data_mock/google/cloud/bigquery/table.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.2/data_mock/google/cloud/storage/blob.py` & `py-data-mock-0.0.3/data_mock/google/cloud/storage/blob.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.2/data_mock/google/cloud/storage/bucket.py` & `py-data-mock-0.0.3/data_mock/google/cloud/storage/bucket.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.2/data_mock/mock_helpers/provider.py` & `py-data-mock-0.0.3/data_mock/mock_helpers/provider.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import types
+from typing import Union, List
 import data_mock.exceptions
 from data_mock.google.cloud import bigquery
 #from bigquery import SchemaField
+import types
 
 class QueryResultsFromList:
 
     def __init__(self, data):
         self.data = data
         self.make_schema()
 
@@ -34,29 +36,33 @@
 
 
 class ProvideData:
 
     def __init__(self):
         self.dict = {}
 
-    def data_from_list(self, data:[[()]], tag:str ) -> QueryResultsFromList:
+    def data_from_list(self, data:List, tag:str ):
         self._test_valid_data(data)
         self.dict[tag] = QueryResultsFromList(data = data)
 
-    def add_data(self, data:[list], tag:str):
+    def add_data(self, data:List, tag:str):
         if isinstance(data, list):
             self.data_from_list(data, tag)
         else:
             self.dict[tag] = data
 
-    def get_data(self, key:str) -> [None, types.GeneratorType]:
+    def get_data(self, key:str) -> Union[None, types.GeneratorType]:
         if not self.dict.get(key):
             return None, None
         if not  hasattr(self.dict[key], 'query_results'):
             raise data_mock.exceptions.InvalidMockData('object does not have query_results')
+        if not isinstance(self.dict[key].query_results, types.MethodType):
+            msg = '"query_results" is  not a method; did you pass the class rather than class()?'
+            raise data_mock.exceptions.InvalidMockData(msg)
+
 
         return self.dict[key].query_results()
 
     def _test_valid_data(self, data):
         if not isinstance(data, list):
             raise data_mock.exceptions.InvalidMockData(f'{data} is not a list')
         errors = []
```

### Comparing `py-data-mock-0.0.2/data_mock/scripts/mkmock.py` & `py-data-mock-0.0.3/data_mock/scripts/mkmock.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.2/py_data_mock.egg-info/SOURCES.txt` & `py-data-mock-0.0.3/py_data_mock.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 LICENSE
 README.md
 setup.py
+data_mock/__init__.py
+data_mock/exceptions.py
 data_mock/google/cloud/bigquery/__init__.py
 data_mock/google/cloud/bigquery/client.py
 data_mock/google/cloud/bigquery/dataset.py
 data_mock/google/cloud/bigquery/exceptions.py
 data_mock/google/cloud/bigquery/retry.py
 data_mock/google/cloud/bigquery/schema.py
 data_mock/google/cloud/bigquery/table.py
```

### Comparing `py-data-mock-0.0.2/setup.py` & `py-data-mock-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(
     name='py-data-mock',
-    version='0.0.2',    
+    version='0.0.3',    
     scripts=['data_mock/scripts/mkmock.py'],
     description='Mock Data',
     url='https://github.com/paulhtremblay/py-data-mock',
     author='Henry Tremblay',
     author_email='paulhtremblay@gmail.com',
     license='GNU GENERAL PUBLIC LICENSE',
     packages=['data_mock/google/cloud/bigquery/job', 'data_mock/google/cloud/bigquery',
-        'data_mock/google/cloud/storage','data_mock/mock_helpers',
+        'data_mock/google/cloud/storage','data_mock/mock_helpers', 'data_mock',
         ],
      classifiers=[
         'Programming Language :: Python :: 3',
         'Topic :: Software Development :: Testing :: Mocking'
     ],
 )
```

### Comparing `py-data-mock-0.0.2/tests/test1.py` & `py-data-mock-0.0.3/tests/test1.py`

 * *Files identical despite different names*

