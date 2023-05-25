# Comparing `tmp/jhdata-1.0.8.tar.gz` & `tmp/jhdata-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jhdata-1.0.8.tar", last modified: Sun Feb  5 21:45:37 2023, max compression
+gzip compressed data, was "jhdata-1.0.9.tar", last modified: Mon Feb  6 19:03:00 2023, max compression
```

## Comparing `jhdata-1.0.8.tar` & `jhdata-1.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 21:45:37.463525 jhdata-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-05 21:45:24.000000 jhdata-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-02-05 21:45:37.463525 jhdata-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-02-05 21:45:24.000000 jhdata-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 21:45:37.459525 jhdata-1.0.8/jhdata/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-05 21:45:24.000000 jhdata-1.0.8/jhdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-02-05 21:45:24.000000 jhdata-1.0.8/jhdata/connections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 21:45:37.463525 jhdata-1.0.8/jhdata/data_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-05 21:45:24.000000 jhdata-1.0.8/jhdata/data_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-02-05 21:45:24.000000 jhdata-1.0.8/jhdata/data_tools/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-02-05 21:45:24.000000 jhdata-1.0.8/jhdata/data_tools/dataframes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-02-05 21:45:24.000000 jhdata-1.0.8/jhdata/data_tools/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-05 21:45:24.000000 jhdata-1.0.8/jhdata/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-02-05 21:45:24.000000 jhdata-1.0.8/jhdata/filehelper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 21:45:37.463525 jhdata-1.0.8/jhdata/loads/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-02-05 21:45:24.000000 jhdata-1.0.8/jhdata/loads/Load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-02-05 21:45:24.000000 jhdata-1.0.8/jhdata/loads/LoadStep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-02-05 21:45:24.000000 jhdata-1.0.8/jhdata/loads/Reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-02-05 21:45:24.000000 jhdata-1.0.8/jhdata/loads/Writer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-05 21:45:24.000000 jhdata-1.0.8/jhdata/loads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-05 21:45:24.000000 jhdata-1.0.8/jhdata/loads/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-02-05 21:45:24.000000 jhdata-1.0.8/jhdata/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 21:45:37.463525 jhdata-1.0.8/jhdata/rest_apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-05 21:45:24.000000 jhdata-1.0.8/jhdata/rest_apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-02-05 21:45:24.000000 jhdata-1.0.8/jhdata/rest_apis/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-02-05 21:45:24.000000 jhdata-1.0.8/jhdata/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 21:45:37.463525 jhdata-1.0.8/jhdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-02-05 21:45:37.000000 jhdata-1.0.8/jhdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-05 21:45:37.000000 jhdata-1.0.8/jhdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-05 21:45:37.000000 jhdata-1.0.8/jhdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-05 21:45:37.000000 jhdata-1.0.8/jhdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-05 21:45:37.000000 jhdata-1.0.8/jhdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-05 21:45:24.000000 jhdata-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-05 21:45:37.463525 jhdata-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-02-05 21:45:24.000000 jhdata-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:00.219197 jhdata-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-06 19:02:46.000000 jhdata-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-02-06 19:03:00.219197 jhdata-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-02-06 19:02:46.000000 jhdata-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:00.219197 jhdata-1.0.9/jhdata/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-06 19:02:46.000000 jhdata-1.0.9/jhdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-02-06 19:02:46.000000 jhdata-1.0.9/jhdata/connections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:00.219197 jhdata-1.0.9/jhdata/data_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 19:02:46.000000 jhdata-1.0.9/jhdata/data_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-02-06 19:02:46.000000 jhdata-1.0.9/jhdata/data_tools/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-02-06 19:02:46.000000 jhdata-1.0.9/jhdata/data_tools/dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-02-06 19:02:46.000000 jhdata-1.0.9/jhdata/data_tools/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-06 19:02:46.000000 jhdata-1.0.9/jhdata/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-02-06 19:02:46.000000 jhdata-1.0.9/jhdata/filehelper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:00.219197 jhdata-1.0.9/jhdata/loads/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-02-06 19:02:46.000000 jhdata-1.0.9/jhdata/loads/Load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-02-06 19:02:46.000000 jhdata-1.0.9/jhdata/loads/LoadStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-02-06 19:02:46.000000 jhdata-1.0.9/jhdata/loads/Reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-02-06 19:02:46.000000 jhdata-1.0.9/jhdata/loads/Writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 19:02:46.000000 jhdata-1.0.9/jhdata/loads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-06 19:02:46.000000 jhdata-1.0.9/jhdata/loads/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-02-06 19:02:46.000000 jhdata-1.0.9/jhdata/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:00.219197 jhdata-1.0.9/jhdata/rest_apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 19:02:46.000000 jhdata-1.0.9/jhdata/rest_apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-02-06 19:02:46.000000 jhdata-1.0.9/jhdata/rest_apis/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-02-06 19:02:46.000000 jhdata-1.0.9/jhdata/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:00.219197 jhdata-1.0.9/jhdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-02-06 19:03:00.000000 jhdata-1.0.9/jhdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-06 19:03:00.000000 jhdata-1.0.9/jhdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 19:03:00.000000 jhdata-1.0.9/jhdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-06 19:03:00.000000 jhdata-1.0.9/jhdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-06 19:03:00.000000 jhdata-1.0.9/jhdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-06 19:02:46.000000 jhdata-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 19:03:00.219197 jhdata-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-02-06 19:02:46.000000 jhdata-1.0.9/setup.py
```

### Comparing `jhdata-1.0.8/LICENSE` & `jhdata-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jhdata-1.0.8/jhdata/connections.py` & `jhdata-1.0.9/jhdata/connections.py`

 * *Files identical despite different names*

### Comparing `jhdata-1.0.8/jhdata/data_tools/database.py` & `jhdata-1.0.9/jhdata/data_tools/database.py`

 * *Files 9% similar despite different names*

```diff
@@ -73,14 +73,12 @@
         statement = exists(table)
         for key in table_schema.primary_keys():
             statement = statement.where(table.c[key] == item[key])
 
         statement = select(statement)
         item_exists = filehelper.sql(statement).fetchone()[0]
         if item_exists:
-            print("Item already exists")
             return
 
     statement = insert(table).values(**item)
-    print(statement)
 
     return filehelper.sql(statement)
```

### Comparing `jhdata-1.0.8/jhdata/data_tools/dataframes.py` & `jhdata-1.0.9/jhdata/data_tools/dataframes.py`

 * *Files identical despite different names*

### Comparing `jhdata-1.0.8/jhdata/data_tools/schemas.py` & `jhdata-1.0.9/jhdata/data_tools/schemas.py`

 * *Files identical despite different names*

### Comparing `jhdata-1.0.8/jhdata/dates.py` & `jhdata-1.0.9/jhdata/dates.py`

 * *Files identical despite different names*

### Comparing `jhdata-1.0.8/jhdata/filehelper.py` & `jhdata-1.0.9/jhdata/filehelper.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,20 +168,19 @@
         engine = self.get_engine()
         return pd.read_sql_table(table_name, engine, **kwargs)
 
     # Write a DataFrame into a SQL table
     def write_sql(self, table_name: str, df: pd.DataFrame, table_schema: Schema = None, if_exists="replace", index=False, **kwargs):
         engine = self.get_engine()
         result = df.to_sql(table_name, engine, if_exists=if_exists, index=index, **kwargs)
-        print("Wrote to table", table_name, "- result:", result)
+        self.logger.success(f"Wrote to table {table_name} - result: {result}")
 
     # Read schema from disk
     def read_schema(self, path: str):
         schema_dict = json.loads(self.read_text(f"schemas/{path}.json"))
-        print(schema_dict)
         return Schema(schema_dict)
 
     # Read schema from default location for a SQL table
     def read_table_schema(self, table_name: str, schema_name: str = None):
         if schema_name is None:
             return self.read_schema(table_name)
         else:
```

### Comparing `jhdata-1.0.8/jhdata/loads/Load.py` & `jhdata-1.0.9/jhdata/loads/Load.py`

 * *Files identical despite different names*

### Comparing `jhdata-1.0.8/jhdata/loads/LoadStep.py` & `jhdata-1.0.9/jhdata/loads/LoadStep.py`

 * *Files identical despite different names*

### Comparing `jhdata-1.0.8/jhdata/loads/Reader.py` & `jhdata-1.0.9/jhdata/loads/Reader.py`

 * *Files identical despite different names*

### Comparing `jhdata-1.0.8/jhdata/loads/Writer.py` & `jhdata-1.0.9/jhdata/loads/Writer.py`

 * *Files identical despite different names*

### Comparing `jhdata-1.0.8/jhdata/logger.py` & `jhdata-1.0.9/jhdata/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,17 @@
 
     def warn(self, message: str):
         self.log("warn", message)
 
     def fail(self, message: str):
         self.log("fail", message)
 
+    def success(self, message: str):
+        self.log("ok", message)
+
     def exception(self, exception: Exception):
         self.fail(f"{exception.__class__}: {exception}")
 
     def log_list(self, messages):
         self.messages += messages
 
     def merge(self, logger):
```

### Comparing `jhdata-1.0.8/jhdata/rest_apis/request_queue.py` & `jhdata-1.0.9/jhdata/rest_apis/request_queue.py`

 * *Files identical despite different names*

### Comparing `jhdata-1.0.8/jhdata/secrets.py` & `jhdata-1.0.9/jhdata/secrets.py`

 * *Files identical despite different names*

### Comparing `jhdata-1.0.8/jhdata.egg-info/SOURCES.txt` & `jhdata-1.0.9/jhdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jhdata-1.0.8/setup.py` & `jhdata-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 NAME = "jhdata"
 DESCRIPTION = "Abstractions around cloud file interfaces (WIP)"
 URL = "https://github.com/jothapunkt/jhdata"
 EMAIL = "jakob-hoefner@web.de"
 AUTHOR = "Jothapunkt"
-VERSION = "1.0.8"
+VERSION = "1.0.9"
 REQUIRED = [
     "requests",
     "boto3",
     "s3fs",
     "pandas",
     "pyarrow",
     "sqlalchemy",
```

