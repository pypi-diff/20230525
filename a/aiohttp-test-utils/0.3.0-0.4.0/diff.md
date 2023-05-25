# Comparing `tmp/aiohttp_test_utils-0.3.0.tar.gz` & `tmp/aiohttp_test_utils-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_test_utils-0.3.0.tar", last modified: Thu May 25 17:55:23 2023, max compression
+gzip compressed data, was "aiohttp_test_utils-0.4.0.tar", last modified: Thu May 25 19:45:31 2023, max compression
```

## Comparing `aiohttp_test_utils-0.3.0.tar` & `aiohttp_test_utils-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 17:55:23.463968 aiohttp_test_utils-0.3.0/
--rw-rw-rw-   0        0        0      532 2023-05-25 17:55:23.463968 aiohttp_test_utils-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       46 2023-02-16 05:06:40.000000 aiohttp_test_utils-0.3.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-25 17:55:23.463968 aiohttp_test_utils-0.3.0/aiohttp_test_utils/
--rw-rw-rw-   0        0        0     1751 2023-05-25 17:55:20.000000 aiohttp_test_utils-0.3.0/aiohttp_test_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:55:23.463968 aiohttp_test_utils-0.3.0/aiohttp_test_utils.egg-info/
--rw-rw-rw-   0        0        0      532 2023-05-25 17:55:23.000000 aiohttp_test_utils-0.3.0/aiohttp_test_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-05-25 17:55:23.000000 aiohttp_test_utils-0.3.0/aiohttp_test_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 17:55:23.000000 aiohttp_test_utils-0.3.0/aiohttp_test_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-25 17:55:23.000000 aiohttp_test_utils-0.3.0/aiohttp_test_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-25 17:55:23.000000 aiohttp_test_utils-0.3.0/aiohttp_test_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-16 05:09:35.000000 aiohttp_test_utils-0.3.0/aiohttp_test_utils.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1012 2023-05-25 17:54:50.000000 aiohttp_test_utils-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 17:55:23.463968 aiohttp_test_utils-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 19:45:31.526536 aiohttp_test_utils-0.4.0/
+-rw-rw-rw-   0        0        0      532 2023-05-25 19:45:31.526536 aiohttp_test_utils-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       46 2023-02-16 05:06:40.000000 aiohttp_test_utils-0.4.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 19:45:31.518121 aiohttp_test_utils-0.4.0/aiohttp_test_utils/
+-rw-rw-rw-   0        0        0     1768 2023-05-25 19:45:28.000000 aiohttp_test_utils-0.4.0/aiohttp_test_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 19:45:31.526536 aiohttp_test_utils-0.4.0/aiohttp_test_utils.egg-info/
+-rw-rw-rw-   0        0        0      532 2023-05-25 19:45:31.000000 aiohttp_test_utils-0.4.0/aiohttp_test_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-25 19:45:31.000000 aiohttp_test_utils-0.4.0/aiohttp_test_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 19:45:31.000000 aiohttp_test_utils-0.4.0/aiohttp_test_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-25 19:45:31.000000 aiohttp_test_utils-0.4.0/aiohttp_test_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-25 19:45:31.000000 aiohttp_test_utils-0.4.0/aiohttp_test_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-16 05:09:35.000000 aiohttp_test_utils-0.4.0/aiohttp_test_utils.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1012 2023-05-25 17:54:50.000000 aiohttp_test_utils-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 19:45:31.526536 aiohttp_test_utils-0.4.0/setup.cfg
```

### Comparing `aiohttp_test_utils-0.3.0/PKG-INFO` & `aiohttp_test_utils-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp_test_utils
-Version: 0.3.0
+Version: 0.4.0
 Summary: a small library used for testing aiohttp projects
 Author-email: 5j9 <5j9@users.noreply.github.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/5j9/aiohttp_test_utils
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `aiohttp_test_utils-0.3.0/aiohttp_test_utils/__init__.py` & `aiohttp_test_utils-0.4.0/aiohttp_test_utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.3.0'
+__version__ = '0.4.0'
 
 from asyncio import new_event_loop
 from unittest.mock import patch
 
 from decouple import config
 from pytest import fixture
 
@@ -20,14 +20,15 @@
     def __eq__(self, other):
         return True
 
 class FakeResponse:
 
     file = ''
     url = EqualToEverything()
+    history = ()
 
     async def read(self):
         with open(self.file, 'rb') as f:
             content = f.read()
         return content
```

### Comparing `aiohttp_test_utils-0.3.0/aiohttp_test_utils.egg-info/PKG-INFO` & `aiohttp_test_utils-0.4.0/aiohttp_test_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-test-utils
-Version: 0.3.0
+Version: 0.4.0
 Summary: a small library used for testing aiohttp projects
 Author-email: 5j9 <5j9@users.noreply.github.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/5j9/aiohttp_test_utils
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `aiohttp_test_utils-0.3.0/pyproject.toml` & `aiohttp_test_utils-0.4.0/pyproject.toml`

 * *Files identical despite different names*

