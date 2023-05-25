# Comparing `tmp/adt_cache-0.0.7.tar.gz` & `tmp/adt_cache-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adt_cache-0.0.7.tar", last modified: Mon Apr 24 15:13:40 2023, max compression
+gzip compressed data, was "dist/adt_cache-0.0.8.tar", last modified: Thu May 25 13:04:45 2023, max compression
```

## Comparing `adt_cache-0.0.7.tar` & `adt_cache-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 15:13:40.000000 adt_cache-0.0.7/
--rw-r--r--   0 nezah      (501) staff       (20)      597 2023-04-24 15:13:40.000000 adt_cache-0.0.7/PKG-INFO
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 15:13:40.000000 adt_cache-0.0.7/cache/
--rw-r--r--   0 nezah      (501) staff       (20)     2613 2023-04-24 15:13:39.000000 adt_cache-0.0.7/cache/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)     1071 2023-04-05 05:19:07.000000 adt_cache-0.0.7/LICENSE
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 15:13:40.000000 adt_cache-0.0.7/adt_cache.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      597 2023-04-24 15:13:39.000000 adt_cache-0.0.7/adt_cache.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      176 2023-04-24 15:13:39.000000 adt_cache-0.0.7/adt_cache.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        6 2023-04-24 15:13:39.000000 adt_cache-0.0.7/adt_cache.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-04-24 15:13:39.000000 adt_cache-0.0.7/adt_cache.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)      172 2023-04-05 05:18:33.000000 adt_cache-0.0.7/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      548 2023-04-24 15:13:39.000000 adt_cache-0.0.7/setup.py
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-04-24 15:13:40.000000 adt_cache-0.0.7/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-25 13:04:45.000000 adt_cache-0.0.8/
+-rw-r--r--   0 nezah      (501) staff       (20)      597 2023-05-25 13:04:45.000000 adt_cache-0.0.8/PKG-INFO
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-25 13:04:45.000000 adt_cache-0.0.8/cache/
+-rw-r--r--   0 nezah      (501) staff       (20)     3584 2023-05-25 13:04:42.000000 adt_cache-0.0.8/cache/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1071 2023-04-05 05:19:07.000000 adt_cache-0.0.8/LICENSE
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-25 13:04:45.000000 adt_cache-0.0.8/adt_cache.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      597 2023-05-25 13:04:45.000000 adt_cache-0.0.8/adt_cache.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      176 2023-05-25 13:04:45.000000 adt_cache-0.0.8/adt_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        6 2023-05-25 13:04:45.000000 adt_cache-0.0.8/adt_cache.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-25 13:04:45.000000 adt_cache-0.0.8/adt_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)      172 2023-04-05 05:18:33.000000 adt_cache-0.0.8/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      548 2023-05-25 13:04:42.000000 adt_cache-0.0.8/setup.py
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-25 13:04:45.000000 adt_cache-0.0.8/setup.cfg
```

### Comparing `adt_cache-0.0.7/PKG-INFO` & `adt_cache-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt_cache
-Version: 0.0.7
+Version: 0.0.8
 Summary: abstract cache with in memory cache or redis (sentinel)
 Home-page: https://github.com/cheddars/pypi_adt_cache
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `adt_cache-0.0.7/cache/__init__.py` & `adt_cache-0.0.8/cache/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from abc import abstractmethod, ABCMeta
-from typing import List, Dict, Literal
+from typing import List, Dict
 import redis
 
 logger = logging.getLogger("adt_cache")
 
 
 class AdtCache(metaclass=ABCMeta):
     def __init__(self):
@@ -24,20 +24,49 @@
 
     @abstractmethod
     def keys(self):
         pass
 
     @abstractmethod
     def hget(self, hash_name: str) -> Dict:
+        """
+        hash_name 에 저장된 dict 를 가져온다.
+        :param hash_name:
+        :return:
+        """
         pass
 
     @abstractmethod
     def hset(self, hash_name: str, dict: Dict[str, any]):
+        """
+        hash_name 에 dict 를 저장한다.
+        :param hash_name:
+        :param dict:
+        :return:
+        """
         pass
 
+    @abstractmethod
+    def get(self, key: str) -> str:
+        """
+        key 에 저장된 값을 가져온다.
+        :param key:
+        :return:
+        """
+        pass
+
+    @abstractmethod
+    def set(self, key: str, value: str):
+        """
+        key 에 value 를 저장한다.
+        :param key:
+        :param value:
+        :return:
+        """
+        pass
 
 class RedisCache(AdtCache):
     def __init__(self, host: str, port: int, db: int, expire_mins: int=60*24, clear_cache=False, decode_res=True):
         logger.info(f"init redis cache with {host}:{port}:{db}")
         super().__init__()
         self.redis = redis.Redis(host=host, port=port, db=db, decode_responses=decode_res)
         self.expire_mins=expire_mins
@@ -61,14 +90,21 @@
         return self.redis.hgetall(hash_name)
 
     def hset(self, hash_name: str, dict: Dict[str, any]):
         for items in dict.items():
             self.redis.hset(hash_name, items[0], items[1])
         self.redis.expire(hash_name, 60 * self.expire_mins)
 
+    def get(self, key: str) -> str:
+        return self.redis.get(key)
+
+    def set(self, key: str, value: str):
+        self.redis.set(key, value)
+        self.redis.expire(key, 60 * self.expire_mins)
+
 
 class MemoryCache(AdtCache):
     def __init__(self):
         super().__init__()
         self.cache = {}
 
     def intersect(self, key, vals: List):
@@ -88,7 +124,14 @@
         return self.cache.keys()
 
     def hget(self, hash_name: str) -> Dict :
         return self.cache.get(hash_name)
 
     def hset(self, hash_name: str, dict: Dict[str, any]):
         self.cache[hash_name] = dict
+
+    def get(self, key: str) -> str:
+        return self.cache.get(key)
+
+    def set(self, key: str, value: str):
+        self.cache[key] = value
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adt_cache-0.0.7/LICENSE` & `adt_cache-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adt_cache-0.0.7/adt_cache.egg-info/PKG-INFO` & `adt_cache-0.0.8/adt_cache.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt-cache
-Version: 0.0.7
+Version: 0.0.8
 Summary: abstract cache with in memory cache or redis (sentinel)
 Home-page: https://github.com/cheddars/pypi_adt_cache
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `adt_cache-0.0.7/setup.py` & `adt_cache-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="adt_cache",
-    version="0.0.7",
+    version="0.0.8",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="abstract cache with in memory cache or redis (sentinel)",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/pypi_adt_cache",
     packages=setuptools.find_packages(),
```

