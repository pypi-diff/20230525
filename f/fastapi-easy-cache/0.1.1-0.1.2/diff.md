# Comparing `tmp/fastapi_easy_cache-0.1.1.tar.gz` & `tmp/fastapi_easy_cache-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_easy_cache-0.1.1.tar", max compression
+gzip compressed data, was "fastapi_easy_cache-0.1.2.tar", max compression
```

## Comparing `fastapi_easy_cache-0.1.1.tar` & `fastapi_easy_cache-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1786 2023-05-21 23:27:29.535697 fastapi_easy_cache-0.1.1/README.md
--rw-r--r--   0        0        0       27 2023-05-21 23:06:18.549908 fastapi_easy_cache-0.1.1/fastapi_easy_cache/__init__.py
--rw-r--r--   0        0        0     3496 2023-05-21 23:14:12.499002 fastapi_easy_cache-0.1.1/fastapi_easy_cache/fastapiCache.py
--rw-r--r--   0        0        0      342 2023-05-21 23:31:51.966617 fastapi_easy_cache-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2302 1970-01-01 00:00:00.000000 fastapi_easy_cache-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1786 2023-05-21 23:27:29.535697 fastapi_easy_cache-0.1.2/README.md
+-rw-r--r--   0        0        0       27 2023-05-21 23:06:18.549908 fastapi_easy_cache-0.1.2/fastapi_easy_cache/__init__.py
+-rw-r--r--   0        0        0     3491 2023-05-25 03:59:17.680182 fastapi_easy_cache-0.1.2/fastapi_easy_cache/fastapiCache.py
+-rw-r--r--   0        0        0      384 2023-05-25 03:59:45.992926 fastapi_easy_cache-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2344 1970-01-01 00:00:00.000000 fastapi_easy_cache-0.1.2/PKG-INFO
```

### Comparing `fastapi_easy_cache-0.1.1/README.md` & `fastapi_easy_cache-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_easy_cache-0.1.1/fastapi_easy_cache/fastapiCache.py` & `fastapi_easy_cache-0.1.2/fastapi_easy_cache/fastapiCache.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             in_memory: set up cache in memory, expected bool
 
         Returns:
             None
         '''
         global db
         if in_memory:
-            db = "file:{dbName}?mode=memory&cache=shared".format(dbName=hashlib.md5(db_path.encode()).hexdigest())
+            db = "file:{dbName}:memory&cache=shared".format(dbName=hashlib.md5(db_path.encode()).hexdigest())
         else:
             db = db_path
         conn = sqlite3.connect(db)
 
         initCur = conn.cursor()
         try:
             initCur.execute('''create table fastapicache(identifier varchar, data TEXT, time integer);''')
```

### Comparing `fastapi_easy_cache-0.1.1/PKG-INFO` & `fastapi_easy_cache-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fastapi-easy-cache
-Version: 0.1.1
-Summary: 
+Version: 0.1.2
+Summary: A simple tool for caching fastapi response
 Author: DrEgg
 Author-email: 102451227+SteelDrEgg@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

