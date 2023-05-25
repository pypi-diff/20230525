# Comparing `tmp/mmigrator-0.2.0.tar.gz` & `tmp/mmigrator-0.2.2.tar.gz`

## Comparing `mmigrator-0.2.0.tar` & `mmigrator-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,21 @@
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 mmigrator-0.2.0/mmigrator.config.json
--rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 mmigrator-0.2.0/package.sh
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mmigrator-0.2.0/requirements.txt
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mmigrator-0.2.0/migrations/20230521104216_one.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mmigrator-0.2.0/migrations/20230521104220_two.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 mmigrator-0.2.0/migrations/20230521104224_three.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/__init__.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/cli.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/constants.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/db.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/migration.py
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/migration_manager.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/process.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/config_manager/__init__.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/config_manager/config_manager.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/config_manager/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/types/__init__.py
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 mmigrator-0.2.0/tests/helpers.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 mmigrator-0.2.0/tests/test_migration_manager.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mmigrator-0.2.0/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mmigrator-0.2.0/LICENSE
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 mmigrator-0.2.0/README.md
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 mmigrator-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 mmigrator-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 mmigrator-0.2.2/package.sh
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mmigrator-0.2.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.2.2/src/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 mmigrator-0.2.2/src/mmigrator/__init__.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 mmigrator-0.2.2/src/mmigrator/cli.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mmigrator-0.2.2/src/mmigrator/constants.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 mmigrator-0.2.2/src/mmigrator/db.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 mmigrator-0.2.2/src/mmigrator/migration.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 mmigrator-0.2.2/src/mmigrator/migration_manager.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mmigrator-0.2.2/src/mmigrator/process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.2.2/src/mmigrator/config_manager/__init__.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 mmigrator-0.2.2/src/mmigrator/config_manager/config_manager.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 mmigrator-0.2.2/src/mmigrator/config_manager/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.2.2/src/mmigrator/types/__init__.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 mmigrator-0.2.2/tests/helpers.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 mmigrator-0.2.2/tests/test_migration_manager.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mmigrator-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mmigrator-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 mmigrator-0.2.2/README.md
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 mmigrator-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 mmigrator-0.2.2/PKG-INFO
```

### Comparing `mmigrator-0.2.0/src/mmigrator/cli.py` & `mmigrator-0.2.2/src/mmigrator/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .migration_manager import MigrationManager
 from .constants import HELP_TEMPLATE
 
 
 args = sys.argv[1:]
 
 
-def get_args_with_option(option) -> (str, str):
+def get_args_with_option(option):
     arg, *opt = args
 
     if len(opt) and opt[0] != option:
         raise Exception(f'Unrecognized parameter {opt}')
 
     return arg, opt[0] if len(opt) else None
```

### Comparing `mmigrator-0.2.0/src/mmigrator/constants.py` & `mmigrator-0.2.2/src/mmigrator/constants.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.2.0/src/mmigrator/db.py` & `mmigrator-0.2.2/src/mmigrator/db.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-from typing import Any, Mapping
-
 import pymongo
-from pymongo.database import Database
 
 
-def connect_db(connection: dict) -> Database[Mapping[str, Any] | Any]:
+def connect_db(connection):
     mongo_user = connection['user']
     mongo_db = connection['database']
     mongo_password = connection['password']
     mongo_host = connection['host']
     mongo_port = connection['port']
 
     if not (mongo_host or mongo_port or mongo_port):
```

### Comparing `mmigrator-0.2.0/src/mmigrator/migration.py` & `mmigrator-0.2.2/src/mmigrator/migration.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import sys
 import os
 from datetime import datetime
 from .constants import MIGRATION_TEMPLATE
 
 
 class Migration(object):
-    __name: str = None
-    __filename: str = None
+    __name = None
+    __filename = None
     __db = None
-    __dist: str = None
+    __dist = None
 
     @property
     def name(self):
         return self.__name
 
-    def __init__(self, name: str, dist: str, db=None):
+    def __init__(self, name, dist, db=None):
         self.__name = name
         self.__dist = dist
         self.__filename = f'{os.getcwd()}/{dist}/{name}.py'
         self.__db = db
 
     def generate(self):
         self.__name = f'{self.__get_time_mark()}_{snakecase.convert(self.__name)}'
```

### Comparing `mmigrator-0.2.0/src/mmigrator/migration_manager.py` & `mmigrator-0.2.2/src/mmigrator/migration_manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import os
+import re
 from .db import connect_db
 from .config_manager.config_manager import ConfigManager
 from .migration import Migration
 from .constants import MMIGRATOR_COLLECTION
-from typing import Any, Mapping
-from pymongo.database import Database
 
 
 class MigrationManager(object):
-    __db: Database[Mapping[str, Any] | Any] = None
-    __config: dict = None
-    __version: str = None
-    __dist: str = None
+    __db = None
+    __config = None
+    __version = None
+    __dist = None
 
     def __init__(self):
         MigrationManager.init()
         
         self.__config = ConfigManager.read_config()
 
         self.__dist = self.__config['dist']
@@ -87,20 +86,25 @@
 
     def __persist_version(self):
         self.__db[MMIGRATOR_COLLECTION].update_one(
             {},
             {'$set': {'version': self.__version}}
         )
 
-    def __get_files_list(self) -> (list[str], int):
-        files = [f.rsplit(".")[0] for f in os.listdir(self.__dist)[::-1] if not f.startswith('__')]
-        files = sorted(files, key=lambda x: int(x.split('_', 1)[0]))
-        last_index = files.index(self.__version) if self.__version in files else -1
+    def __get_files_list(self):
+        try:
+            files = [f.rsplit(".")[0] for f in os.listdir(self.__dist) if re.match(r'^\d+_\w+\.py$', f)]
+            files = sorted(files, key=lambda x: int(x.split('_', 1)[0]))
+
+            last_index = files.index(self.__version) if self.__version in files else -1
 
-        return files, last_index
+            return files, last_index
+        except Exception as e:
+            print('>>>', e)
+            raise Exception('Failed to load a list of files associated to migrations.')
 
     def __init_version(self):
         if MMIGRATOR_COLLECTION not in self.__db.list_collection_names():
             self.__db.create_collection(MMIGRATOR_COLLECTION)
             self.__db[MMIGRATOR_COLLECTION].insert_one({'version': None})
         
         self.__version = self.__db[MMIGRATOR_COLLECTION].find_one()['version']
```

### Comparing `mmigrator-0.2.0/src/mmigrator/config_manager/config_manager.py` & `mmigrator-0.2.2/src/mmigrator/config_manager/config_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,22 +16,22 @@
             with open(CONFIG_FILE_NAME, 'w') as f:
                 f.write(conf)
             
         if not os.path.exists(CONFIG_FILE_NAME):
             init()
 
     @staticmethod
-    def read_config() -> dict:
+    def read_config():
         with open(CONFIG_FILE_NAME, 'r') as f:
             cfg = json.loads(f.read())
 
         for k, v in cfg['connection'].items():
             if v and re.match(r'^.+\[.+\]$', v):
                 file, var = re.sub(r'[\[\]]', ' ', v).strip().split(' ')
                 cfg['connection'][k] = load_var(file, var)
 
         return cfg
 
     @staticmethod
-    def init_dist(dist: str):
+    def init_dist(dist):
         if not os.path.exists(dist):
             os.mkdir(dist)
```

### Comparing `mmigrator-0.2.0/src/mmigrator/config_manager/helpers.py` & `mmigrator-0.2.2/src/mmigrator/config_manager/helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import re
 import json
 
 
-def try_load_from_json(varname: str, data: str) -> str | None:
-    data = json.loads(data)
-    return data.get(varname)
+def try_load_from_json(varname, data):
+    return json.loads(data).get(varname)
 
 
-def try_load_from_dotenv(varname: str, data: str) -> str | None:
+def try_load_from_dotenv(varname, data):
     m = re.search(fr'{varname}\s?=\s?(.+)', data)
+
     return m[1] if m else None
 
 
-def load_var(filename: str, varname: str) -> str:
+def load_var(filename, varname):
     var_value = None
 
     with open(filename, 'r') as f:
         data = f.read()
 
     if re.match(r'^.*\.json$', filename):
         var_value = try_load_from_json(varname, data)
```

### Comparing `mmigrator-0.2.0/tests/helpers.py` & `mmigrator-0.2.2/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.2.0/tests/test_migration_manager.py` & `mmigrator-0.2.2/tests/test_migration_manager.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.2.0/LICENSE` & `mmigrator-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mmigrator-0.2.0/README.md` & `mmigrator-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # MongoDb Migrator
-Migration engine for MongoDB
+Migration engine for MongoDB\
+Supports CLI
 
 ## Installation
 
 ```bash
 $ python -m pip install mmigrator
 ```
 
@@ -37,15 +38,15 @@
 
 ### Help
 ```bash
 $ mmigrator help
 ```
 
 ### Init configs
-optional, wil l run automatically on any migration command*
+optional, will run automatically on any migration command*
 #### CLI 
 ```bash
 $ mmigrator init
 ```
 
 #### from code:
 ```py
```

### Comparing `mmigrator-0.2.0/pyproject.toml` & `mmigrator-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mmigrator"
-version = "0.2.0"
+version = "0.2.2"
 authors = [
   { name="Serhii Kovalov", email="moiserge.k@gmail.com" },
 ]
 description = "Migration engine for MongoDB"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mmigrator-0.2.0/PKG-INFO` & `mmigrator-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmigrator
-Version: 0.2.0
+Version: 0.2.2
 Summary: Migration engine for MongoDB
 Project-URL: Homepage, https://github.com/sergekovalev/mmigrator
 Project-URL: Bug Tracker, https://github.com/sergekovalev/mmigrator/issues
 Author-email: Serhii Kovalov <moiserge.k@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,16 @@
 Requires-Python: >=3.7
 Requires-Dist: pydantic
 Requires-Dist: pymongo
 Requires-Dist: snakecase
 Description-Content-Type: text/markdown
 
 # MongoDb Migrator
-Migration engine for MongoDB
+Migration engine for MongoDB\
+Supports CLI
 
 ## Installation
 
 ```bash
 $ python -m pip install mmigrator
 ```
 
@@ -54,15 +55,15 @@
 
 ### Help
 ```bash
 $ mmigrator help
 ```
 
 ### Init configs
-optional, wil l run automatically on any migration command*
+optional, will run automatically on any migration command*
 #### CLI 
 ```bash
 $ mmigrator init
 ```
 
 #### from code:
 ```py
```

