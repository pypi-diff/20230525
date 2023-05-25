# Comparing `tmp/aiohttp_test_utils-0.2.1.tar.gz` & `tmp/aiohttp_test_utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_test_utils-0.2.1.tar", last modified: Thu Feb 16 07:47:25 2023, max compression
+gzip compressed data, was "aiohttp_test_utils-0.3.0.tar", last modified: Thu May 25 17:55:23 2023, max compression
```

## Comparing `aiohttp_test_utils-0.2.1.tar` & `aiohttp_test_utils-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-02-16 07:47:25.143128 aiohttp_test_utils-0.2.1/
--rw-rw-rw-   0        0        0      527 2023-02-16 07:47:25.144116 aiohttp_test_utils-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       46 2023-02-16 05:06:40.000000 aiohttp_test_utils-0.2.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-16 07:47:25.135139 aiohttp_test_utils-0.2.1/aiohttp_test_utils/
--rw-rw-rw-   0        0        0     1646 2023-02-16 07:47:22.000000 aiohttp_test_utils-0.2.1/aiohttp_test_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-16 07:47:25.142148 aiohttp_test_utils-0.2.1/aiohttp_test_utils.egg-info/
--rw-rw-rw-   0        0        0      527 2023-02-16 07:47:25.000000 aiohttp_test_utils-0.2.1/aiohttp_test_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-02-16 07:47:25.000000 aiohttp_test_utils-0.2.1/aiohttp_test_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-16 07:47:25.000000 aiohttp_test_utils-0.2.1/aiohttp_test_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-02-16 07:47:25.000000 aiohttp_test_utils-0.2.1/aiohttp_test_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-02-16 07:47:25.000000 aiohttp_test_utils-0.2.1/aiohttp_test_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-16 05:09:35.000000 aiohttp_test_utils-0.2.1/aiohttp_test_utils.egg-info/zip-safe
--rw-rw-rw-   0        0        0      152 2023-02-16 05:08:57.000000 aiohttp_test_utils-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      710 2023-02-16 07:47:25.145114 aiohttp_test_utils-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 17:55:23.463968 aiohttp_test_utils-0.3.0/
+-rw-rw-rw-   0        0        0      532 2023-05-25 17:55:23.463968 aiohttp_test_utils-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       46 2023-02-16 05:06:40.000000 aiohttp_test_utils-0.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 17:55:23.463968 aiohttp_test_utils-0.3.0/aiohttp_test_utils/
+-rw-rw-rw-   0        0        0     1751 2023-05-25 17:55:20.000000 aiohttp_test_utils-0.3.0/aiohttp_test_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:55:23.463968 aiohttp_test_utils-0.3.0/aiohttp_test_utils.egg-info/
+-rw-rw-rw-   0        0        0      532 2023-05-25 17:55:23.000000 aiohttp_test_utils-0.3.0/aiohttp_test_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-25 17:55:23.000000 aiohttp_test_utils-0.3.0/aiohttp_test_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 17:55:23.000000 aiohttp_test_utils-0.3.0/aiohttp_test_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-25 17:55:23.000000 aiohttp_test_utils-0.3.0/aiohttp_test_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-25 17:55:23.000000 aiohttp_test_utils-0.3.0/aiohttp_test_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-16 05:09:35.000000 aiohttp_test_utils-0.3.0/aiohttp_test_utils.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1012 2023-05-25 17:54:50.000000 aiohttp_test_utils-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 17:55:23.463968 aiohttp_test_utils-0.3.0/setup.cfg
```

### Comparing `aiohttp_test_utils-0.2.1/aiohttp_test_utils/__init__.py` & `aiohttp_test_utils-0.3.0/aiohttp_test_utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-__version__ = '0.2.1'
+__version__ = '0.3.0'
 
 from asyncio import new_event_loop
 from unittest.mock import patch
 
-from pytest import fixture
 from decouple import config
+from pytest import fixture
 
 
 def init_tests():
     global RECORD_MODE, OFFLINE_MODE, TESTS_PATH
 
     config.search_path = TESTS_PATH = config._caller_path()
 
     RECORD_MODE = config('RECORD_MODE', False, cast=bool)
     OFFLINE_MODE = config('OFFLINE_MODE', False, cast=bool) and not RECORD_MODE
 
 
+class EqualToEverything:
+    def __eq__(self, other):
+        return True
+
 class FakeResponse:
 
     file = ''
+    url = EqualToEverything()
 
     async def read(self):
         with open(self.file, 'rb') as f:
             content = f.read()
         return content
```

