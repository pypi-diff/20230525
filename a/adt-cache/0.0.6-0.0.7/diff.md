# Comparing `tmp/adt_cache-0.0.6.tar.gz` & `tmp/adt_cache-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adt_cache-0.0.6.tar", last modified: Mon Apr 24 15:01:56 2023, max compression
+gzip compressed data, was "dist/adt_cache-0.0.7.tar", last modified: Mon Apr 24 15:13:40 2023, max compression
```

## Comparing `adt_cache-0.0.6.tar` & `adt_cache-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 15:01:56.000000 adt_cache-0.0.6/
--rw-r--r--   0 nezah      (501) staff       (20)      597 2023-04-24 15:01:56.000000 adt_cache-0.0.6/PKG-INFO
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 15:01:56.000000 adt_cache-0.0.6/cache/
--rw-r--r--   0 nezah      (501) staff       (20)     2543 2023-04-24 15:01:55.000000 adt_cache-0.0.6/cache/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)     1071 2023-04-05 05:19:07.000000 adt_cache-0.0.6/LICENSE
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 15:01:56.000000 adt_cache-0.0.6/adt_cache.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      597 2023-04-24 15:01:56.000000 adt_cache-0.0.6/adt_cache.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      176 2023-04-24 15:01:56.000000 adt_cache-0.0.6/adt_cache.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        6 2023-04-24 15:01:56.000000 adt_cache-0.0.6/adt_cache.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-04-24 15:01:56.000000 adt_cache-0.0.6/adt_cache.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)      172 2023-04-05 05:18:33.000000 adt_cache-0.0.6/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      548 2023-04-24 15:01:55.000000 adt_cache-0.0.6/setup.py
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-04-24 15:01:56.000000 adt_cache-0.0.6/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 15:13:40.000000 adt_cache-0.0.7/
+-rw-r--r--   0 nezah      (501) staff       (20)      597 2023-04-24 15:13:40.000000 adt_cache-0.0.7/PKG-INFO
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 15:13:40.000000 adt_cache-0.0.7/cache/
+-rw-r--r--   0 nezah      (501) staff       (20)     2613 2023-04-24 15:13:39.000000 adt_cache-0.0.7/cache/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1071 2023-04-05 05:19:07.000000 adt_cache-0.0.7/LICENSE
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 15:13:40.000000 adt_cache-0.0.7/adt_cache.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      597 2023-04-24 15:13:39.000000 adt_cache-0.0.7/adt_cache.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      176 2023-04-24 15:13:39.000000 adt_cache-0.0.7/adt_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        6 2023-04-24 15:13:39.000000 adt_cache-0.0.7/adt_cache.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-04-24 15:13:39.000000 adt_cache-0.0.7/adt_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)      172 2023-04-05 05:18:33.000000 adt_cache-0.0.7/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      548 2023-04-24 15:13:39.000000 adt_cache-0.0.7/setup.py
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-04-24 15:13:40.000000 adt_cache-0.0.7/setup.cfg
```

### Comparing `adt_cache-0.0.6/PKG-INFO` & `adt_cache-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt_cache
-Version: 0.0.6
+Version: 0.0.7
 Summary: abstract cache with in memory cache or redis (sentinel)
 Home-page: https://github.com/cheddars/pypi_adt_cache
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `adt_cache-0.0.6/cache/__init__.py` & `adt_cache-0.0.7/cache/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from abc import abstractmethod, ABCMeta
-from typing import List, Dict
+from typing import List, Dict, Literal
 import redis
 
 logger = logging.getLogger("adt_cache")
 
 
 class AdtCache(metaclass=ABCMeta):
     def __init__(self):
@@ -32,18 +32,18 @@
 
     @abstractmethod
     def hset(self, hash_name: str, dict: Dict[str, any]):
         pass
 
 
 class RedisCache(AdtCache):
-    def __init__(self, host: str, port, db, expire_mins=60*24, clear_cache=False):
+    def __init__(self, host: str, port: int, db: int, expire_mins: int=60*24, clear_cache=False, decode_res=True):
         logger.info(f"init redis cache with {host}:{port}:{db}")
         super().__init__()
-        self.redis = redis.Redis(host=host, port=port, db=db)
+        self.redis = redis.Redis(host=host, port=port, db=db, decode_responses=decode_res)
         self.expire_mins=expire_mins
         if clear_cache:
             self.redis.flushdb()
 
     def intersect(self, key, vals: List):
         return [val for val in vals if self.redis.sismember(key, val)]
```

### Comparing `adt_cache-0.0.6/LICENSE` & `adt_cache-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `adt_cache-0.0.6/adt_cache.egg-info/PKG-INFO` & `adt_cache-0.0.7/adt_cache.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt-cache
-Version: 0.0.6
+Version: 0.0.7
 Summary: abstract cache with in memory cache or redis (sentinel)
 Home-page: https://github.com/cheddars/pypi_adt_cache
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `adt_cache-0.0.6/setup.py` & `adt_cache-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="adt_cache",
-    version="0.0.6",
+    version="0.0.7",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="abstract cache with in memory cache or redis (sentinel)",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/pypi_adt_cache",
     packages=setuptools.find_packages(),
```

