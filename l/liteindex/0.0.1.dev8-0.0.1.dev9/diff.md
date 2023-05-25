# Comparing `tmp/liteindex-0.0.1.dev8.tar.gz` & `tmp/liteindex-0.0.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteindex-0.0.1.dev8.tar", last modified: Tue May  9 10:18:23 2023, max compression
+gzip compressed data, was "liteindex-0.0.1.dev9.tar", last modified: Wed May 17 12:03:05 2023, max compression
```

## Comparing `liteindex-0.0.1.dev8.tar` & `liteindex-0.0.1.dev9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:23.664692 liteindex-0.0.1.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-09 10:18:13.000000 liteindex-0.0.1.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-09 10:18:23.664692 liteindex-0.0.1.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-09 10:18:13.000000 liteindex-0.0.1.dev8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:23.660692 liteindex-0.0.1.dev8/liteindex/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-09 10:18:13.000000 liteindex-0.0.1.dev8/liteindex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-09 10:18:13.000000 liteindex-0.0.1.dev8/liteindex/any_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-05-09 10:18:13.000000 liteindex-0.0.1.dev8/liteindex/defined_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-09 10:18:13.000000 liteindex-0.0.1.dev8/liteindex/dict_index_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-09 10:18:13.000000 liteindex-0.0.1.dev8/liteindex/file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-09 10:18:13.000000 liteindex-0.0.1.dev8/liteindex/number_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:23.664692 liteindex-0.0.1.dev8/liteindex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-09 10:18:23.000000 liteindex-0.0.1.dev8/liteindex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-09 10:18:23.000000 liteindex-0.0.1.dev8/liteindex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:18:23.000000 liteindex-0.0.1.dev8/liteindex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-09 10:18:23.000000 liteindex-0.0.1.dev8/liteindex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 10:18:23.000000 liteindex-0.0.1.dev8/liteindex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 10:18:23.664692 liteindex-0.0.1.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-09 10:18:13.000000 liteindex-0.0.1.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:03:05.248151 liteindex-0.0.1.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-17 12:02:49.000000 liteindex-0.0.1.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-17 12:03:05.248151 liteindex-0.0.1.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-17 12:02:49.000000 liteindex-0.0.1.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:03:05.244151 liteindex-0.0.1.dev9/liteindex/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-17 12:02:49.000000 liteindex-0.0.1.dev9/liteindex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-17 12:02:49.000000 liteindex-0.0.1.dev9/liteindex/any_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-17 12:02:49.000000 liteindex-0.0.1.dev9/liteindex/defined_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-17 12:02:49.000000 liteindex-0.0.1.dev9/liteindex/dict_index_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-17 12:02:49.000000 liteindex-0.0.1.dev9/liteindex/file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-17 12:02:49.000000 liteindex-0.0.1.dev9/liteindex/number_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16701 2023-05-17 12:02:49.000000 liteindex-0.0.1.dev9/liteindex/query_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:03:05.248151 liteindex-0.0.1.dev9/liteindex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-17 12:03:05.000000 liteindex-0.0.1.dev9/liteindex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-17 12:03:05.000000 liteindex-0.0.1.dev9/liteindex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:03:05.000000 liteindex-0.0.1.dev9/liteindex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-17 12:03:05.000000 liteindex-0.0.1.dev9/liteindex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 12:03:05.000000 liteindex-0.0.1.dev9/liteindex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:03:05.248151 liteindex-0.0.1.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-17 12:02:49.000000 liteindex-0.0.1.dev9/setup.py
```

### Comparing `liteindex-0.0.1.dev8/LICENSE` & `liteindex-0.0.1.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev8/PKG-INFO` & `liteindex-0.0.1.dev9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteindex
-Version: 0.0.1.dev8
+Version: 0.0.1.dev9
 Summary: SQLite based queryable python indexes for dicts and lists
 Home-page: https://github.com/notAI-tech/liteindex
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -47,17 +47,17 @@
         "street": "123 Main St",
         "city": "New York",
         "country": "USA"
     }
 })
 
 # Query the index to retrieve items based on certain conditions
-# (e.g., age >= 25, city = "New York")
+# (e.g., age <= 25, city = "New York")
 query = {
-    "age": (">=", 25),
+    "age": (None, 25),
     "address": {
         "city": "New York"
     }
 }
 results = index.search(query)
 
 for result in results:
```

### Comparing `liteindex-0.0.1.dev8/README.md` & `liteindex-0.0.1.dev9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -29,17 +29,17 @@
         "street": "123 Main St",
         "city": "New York",
         "country": "USA"
     }
 })
 
 # Query the index to retrieve items based on certain conditions
-# (e.g., age >= 25, city = "New York")
+# (e.g., age <= 25, city = "New York")
 query = {
-    "age": (">=", 25),
+    "age": (None, 25),
     "address": {
         "city": "New York"
     }
 }
 results = index.search(query)
 
 for result in results:
```

### Comparing `liteindex-0.0.1.dev8/liteindex/any_index.py` & `liteindex-0.0.1.dev9/liteindex/any_index.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev8/liteindex/defined_index.py` & `liteindex-0.0.1.dev9/liteindex/defined_index.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import json
 import sqlite3
-from typing import Any, Union, List, Iterator, Optional, Dict, Tuple
+import random
+from query_parser import search_query, distinct_query, count_query, delete_query
 
 
 class DefinedIndex:
-    def __init__(
-        self, name: str, schema: Optional[dict] = None, db_path: str = ":memory:"
-    ):
+    def __init__(self, name, schema=None, db_path=":memory:", auto_key=False):
         self.name = name
         self.db_path = db_path
+        self.auto_key = auto_key
         self._connection = sqlite3.connect(self.db_path, uri=True)
         self._connection.row_factory = sqlite3.Row
         if schema is None:
             self.schema = self._load_schema_from_table()
         else:
             self.schema = schema
             self._validate_schema()
+        self.column_type_map = {
+            key: self._get_column_type(value) for key, value in self.schema.items()
+        }
+
         self._initialize_db()
 
     def _initialize_db(self):
         self._connection.execute("PRAGMA journal_mode=WAL")
         self._connection.execute("PRAGMA synchronous=NORMAL")
         self._create_table()
 
@@ -30,21 +34,31 @@
         )
         result = cursor.fetchone()
         if result is None:
             raise ValueError(f"Table {self.name} does not exist in the database")
         sql = result["sql"]
         column_defs = re.findall(r"\((.*)\)", sql)[0].split(",")
         schema = {}
+
         for column_def in column_defs:
-            column_name = column_def.split()[0]
-            column_type = column_def.split()[1]
+            column_name, column_type, *rest = column_def.split()
+            if column_name == "id":
+                self.auto_key = "INTEGER" in column_type
             schema[column_name] = self._get_value_from_column_type(column_type)
         return schema
 
-    def _get_value_from_column_type(self, column_type: str):
+    def drop(self):
+        """
+        Drops the table from the database.
+        """
+        query = f"DROP TABLE IF EXISTS {self.name}"
+        self._connection.execute(query)
+        self._connection.commit()
+
+    def _get_value_from_column_type(self, column_type):
         if column_type.startswith("TEXT"):
             return ""
         elif column_type == "NUMBER":
             return 0
         elif column_type == "JSON":
             return {}
         elif column_type == "INTEGER":
@@ -63,73 +77,83 @@
 
     def _create_table(self):
         columns = []
         for key, value in self.schema.items():
             column_type = self._get_column_type(value)
             columns.append(f"{key} {column_type}")
         columns_str = ", ".join(columns)
+        id_column = (
+            "id INTEGER PRIMARY KEY AUTOINCREMENT"
+            if self.auto_key
+            else "id TEXT PRIMARY KEY"
+        )
         self._connection.execute(
-            f"CREATE TABLE IF NOT EXISTS {self.name} (id TEXT PRIMARY KEY, {columns_str})"
+            f"CREATE TABLE IF NOT EXISTS {self.name} ({id_column}, {columns_str})"
         )
         self._connection.commit()
 
-    def _get_column_type(self, value: Any) -> str:
+    def _get_column_type(self, value):
         if isinstance(value, bool):
             return "INTEGER"  # SQLite does not have a native BOOLEAN type, but INTEGER can store 0 (False) or 1 (True)
         elif isinstance(value, (int, float)):
             return "NUMBER"
         elif isinstance(value, (list, dict)):
             return "JSON"
         else:
             return "TEXT"
 
-    def _process_query_conditions(
-        self, query: Dict, prefix: Optional[List[str]] = None
-    ) -> Tuple[List[str], List]:
-        where_conditions = []
-        params = []
-
-        if prefix is None:
-            prefix = []
-
-        def process_nested_query(
-            value: Union[Dict, Tuple, List, int, str, float], prefix: List[str]
-        ) -> None:
-            nonlocal where_conditions, params
-            column = (
-                "json_extract(" + prefix[0] + ", '$." + ".".join(prefix[1:]) + "')"
-                if len(prefix) > 1
-                else prefix[0]
-            )
+    def add(self, value):
+        if not self.auto_key:
+            raise ValueError("The add function can only be used when auto_key is True")
+
+        if isinstance(value, dict):
+            value_list = [value]
+        elif isinstance(value, list):
+            value_list = value
+        else:
+            raise ValueError("The add function accepts a dict or a list of dicts")
 
-            if isinstance(value, dict):
-                for sub_key, sub_value in value.items():
-                    process_nested_query(sub_value, prefix + [sub_key])
-            elif isinstance(value, tuple):
-                if value[0] is not None:
-                    where_conditions.append(f"{column} >= ?")
-                    params.append(value[0])
-                if value[1] is not None:
-                    where_conditions.append(f"{column} <= ?")
-                    params.append(value[1])
-            elif isinstance(value, list):
-                where_conditions.append(
-                    f"{column} IN ({', '.join(['?' for _ in value])})"
-                )
-                params.extend(value)
-            else:
-                where_conditions.append(f"{column} = ?")
-                params.append(value)
+        for item in value_list:
+            keys = []
+            values = []
+            placeholders = []
+            for key, val in item.items():
+                if key == "id":
+                    raise ValueError(
+                        "The add function should not include an 'id' key in the input dict"
+                    )
+
+                keys.append(key)
+
+                if isinstance(val, (list, dict)):
+                    val = json.dumps(val)
+
+                values.append(val)
+                placeholders.append("?")
+            keys_str = ", ".join(keys)
+            placeholders_str = ", ".join(placeholders)
+
+            query = f"""
+            INSERT INTO {self.name} ({keys_str})
+            VALUES ({placeholders_str})
+            """
 
-        for key, value in query.items():
-            process_nested_query(value, [key])
+            cursor = self._connection.execute(query, values)
+            self._connection.commit()
 
-        return where_conditions, params
+            # Get the autogenerated id for the last inserted row
+            auto_id = cursor.lastrowid
+            return auto_id
+
+    def set(self, key, value):
+        if self.auto_key and isinstance(key, str):
+            raise KeyError(
+                "The index has auto_key. use add Function to add new items to the index"
+            )
 
-    def set(self, key: Union[str, Tuple[str, Union[str, int]]], value: Any) -> None:
         if isinstance(key, tuple):
             id, column, *keys = key
 
             if not keys:
                 if isinstance(value, (list, dict)):
                     value = json.dumps(value)
 
@@ -181,15 +205,56 @@
             VALUES ({placeholders_str})
             ON CONFLICT(id) DO UPDATE SET {update_str}
             """
 
             self._connection.execute(query, values * 2)
             self._connection.commit()
 
-    def get(self, id: str, *keys: Union[str, int]) -> Optional[Any]:
+    def delete(self, x, return_deleted=False):
+        to_del_keys = []
+        to_del_by_query = None
+
+        if isinstance(x, str):
+            to_del_keys = [x]
+        elif isinstance(x, (list, tuple, set)):
+            to_del_keys = list(x)
+        elif isinstance(x, dict):
+            to_del_by_query = x
+
+        to_return = None
+
+        if to_del_keys:
+            if return_deleted:
+                select_query_str = f"SELECT * FROM {self.name} WHERE id IN ({', '.join(['?' for _ in to_del_keys])})"
+                to_return = [
+                    self.__row_to_id_and_item(row)
+                    for row in self._connection.execute(select_query_str, to_del_keys)
+                ]
+
+            delete_query_str = f"DELETE FROM {self.name} WHERE id IN ({', '.join(['?' for _ in to_del_keys])})"
+            self._connection.execute(delete_query_str, to_del_keys)
+            self._connection.commit()
+
+        elif to_del_by_query is not None:
+            if return_deleted:
+                to_return = list(self.search(query=to_del_by_query))
+                to_del_keys = [_ for _, __ in to_return]
+                delete_query_str = f"DELETE FROM {self.name} WHERE id IN ({', '.join(['?' for _ in to_del_keys])})"
+                self._connection.execute(delete_query_str, to_del_keys)
+                self._connection.commit()
+            else:
+                delete_query_str, params = delete_query(
+                    self.name, to_del_by_query, self.column_type_map
+                )
+                self._connection.execute(delete_query_str, params)
+                self._connection.commit()
+
+        return to_return
+
+    def get(self, id, *keys):
         """Retrieve an item or a specific key path value from the item in the index by its id."""
         value = None
         if len(keys) == 1:
             query = f"SELECT {keys[0]} FROM {self.name} WHERE id = ?"
             cursor = self._connection.execute(query, (id,))
             row = cursor.fetchone()
             if row:
@@ -216,91 +281,82 @@
                 value = self.__row_to_id_and_item(row)[1]
 
         if not value:
             raise KeyError(f"Key {id} {keys} not found in index {self.name}")
 
         return value
 
-    def __getitem__(
-        self, key: Union[str, Tuple[str, Union[str, int]]]
-    ) -> Optional[Any]:
+    def __getitem__(self, key):
         if isinstance(key, tuple):
             id, *keys = key
             return self.get(id, *keys)
         else:
             id = key
             return self.get(id)
 
-    def __row_to_id_and_item(self, row: sqlite3.Row) -> Tuple[str, Dict[str, Any]]:
+    def __row_to_id_and_item(self, row):
         item = dict(row)
         for k, v in item.items():
             try:
                 item[k] = json.loads(v)
             except:
                 pass
 
         return item["id"], item
 
     def search(
         self,
-        query: Optional[Dict],
-        sort_by: Optional[str] = None,
-        reversed_sort: Optional[bool] = False,
-    ) -> List[Dict]:
-
-        if query:
-            where_conditions, params = self._process_query_conditions(query)
-            where_clause = " AND ".join(where_conditions)
-            query = f"SELECT * FROM {self.name} WHERE {where_clause}"
-        else:
-            query = f"SELECT * FROM {self.name}"
-            params = []
-
-        if sort_by:
-            query += f" ORDER BY {sort_by}"
-            if reversed_sort:
-                query += " DESC"
-
+        query={},
+        sort_by=None,
+        reversed_sort=False,
+        n=None,
+        page=None,
+        page_size=50,
+        select_columns=None,
+    ):
+        query, params = search_query(
+            table_name=self.name,
+            query=query,
+            column_type_map=self.column_type_map,
+            sort_by=sort_by,
+            reversed_sort=reversed_sort,
+            n=n,
+            page=page,
+            page_size=page_size,
+            select_columns=select_columns,
+        )
         cursor = self._connection.execute(query, params)
-        for row in cursor:
-            yield self.__row_to_id_and_item(row)
-
-    def count(self, query: Optional[Dict] = None) -> int:
-        if query:
-            where_conditions, params = self._process_query_conditions(query)
-            where_clause = " AND ".join(where_conditions)
-            query = f"SELECT COUNT(*) FROM {self.name} WHERE {where_clause}"
-        else:
-            query = f"SELECT COUNT(*) FROM {self.name}"
-            params = []
 
-        cursor = self._connection.execute(query, params)
-        return cursor.fetchone()[0]
+        def gen():
+            for row in cursor:
+                yield self.__row_to_id_and_item(row)
 
-    def sum(self, column: str, query: Optional[Dict] = None) -> float:
-        if query:
-            where_conditions, params = self._process_query_conditions(query)
-            where_clause = " AND ".join(where_conditions)
-            query = f"SELECT SUM({column}) FROM {self.name} WHERE {where_clause}"
+        if n is None and page is None:
+            return gen()
         else:
-            query = f"SELECT SUM({column}) FROM {self.name}"
-            params = []
+            return [self.__row_to_id_and_item(row) for row in cursor.fetchall()]
+
+    def count(self, query={}):
+        query, params = count_query(
+            table_name=self.name, query=query, column_type_map=self.column_type_map
+        )
         cursor = self._connection.execute(query, params)
-        return cursor.fetchone()[0]
+        row = cursor.fetchone()
+        return row[0]
 
-    def average(self, column: str, query: Optional[Dict] = None) -> float:
-        if query:
-            where_conditions, params = self._process_query_conditions(query)
-            where_clause = " AND ".join(where_conditions)
-            query = f"SELECT AVG({column}) FROM {self.name} WHERE {where_clause}"
-        else:
-            query = f"SELECT AVG({column}) FROM {self.name}"
-            params = []
+    def distinct(self, column, query={}):
+        query, params = distinct_query(
+            table_name=self.name,
+            column=column,
+            query=query,
+            column_type_map=self.column_type_map,
+        )
         cursor = self._connection.execute(query, params)
-        return cursor.fetchone()[0]
+        row = cursor.fetchone()
+        return row[0]
 
 
 if __name__ == "__main__":
     # Define the schema for the index
     schema = {
         "name": "",
         "age": 0,
@@ -332,21 +388,18 @@
     index.set(("1", "years", 1), 4)
     print(index.get("1"))
 
     index.set(("1", "address", "state"), "updated NY 2")
     print(index.get("1"))
 
     # Search for items in the index
-    query = {"age": (None, 35)}
+    query = {"age": {"$lte": 35}}
     results = index.search(query)
     for result in results:
         print("--", result)
 
     # Count the number of items matching a query
     count = index.count(query)
     print("Count:", count)
 
-    # Calculate the sum and average of a numeric column for items matching a query
-    total_age = index.sum("age", query)
-    average_age = index.average("age", query)
-    print("Total age:", total_age)
-    print("Average age:", average_age)
+    # distinct the number of items matching a query
+    distinct = index.distinct("age", query)
```

### Comparing `liteindex-0.0.1.dev8/liteindex/dict_index_helpers.py` & `liteindex-0.0.1.dev9/liteindex/dict_index_helpers.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev8/liteindex/file_index.py` & `liteindex-0.0.1.dev9/liteindex/file_index.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev8/liteindex/number_index.py` & `liteindex-0.0.1.dev9/liteindex/number_index.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev8/liteindex.egg-info/PKG-INFO` & `liteindex-0.0.1.dev9/liteindex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteindex
-Version: 0.0.1.dev8
+Version: 0.0.1.dev9
 Summary: SQLite based queryable python indexes for dicts and lists
 Home-page: https://github.com/notAI-tech/liteindex
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -47,17 +47,17 @@
         "street": "123 Main St",
         "city": "New York",
         "country": "USA"
     }
 })
 
 # Query the index to retrieve items based on certain conditions
-# (e.g., age >= 25, city = "New York")
+# (e.g., age <= 25, city = "New York")
 query = {
-    "age": (">=", 25),
+    "age": (None, 25),
     "address": {
         "city": "New York"
     }
 }
 results = index.search(query)
 
 for result in results:
```

### Comparing `liteindex-0.0.1.dev8/setup.py` & `liteindex-0.0.1.dev9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "liteindex"
 DESCRIPTION = "SQLite based queryable python indexes for dicts and lists"
 URL = "https://github.com/notAI-tech/liteindex"
 EMAIL = "praneeth@bpraneeth.com"
 AUTHOR = "BEDAPUDI PRANEETH"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.1.dev8"
+VERSION = "0.0.1.dev9"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
 ]
 
 # What packages are optional?
 EXTRAS = {
```

