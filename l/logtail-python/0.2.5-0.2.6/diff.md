# Comparing `tmp/logtail-python-0.2.5.tar.gz` & `tmp/logtail-python-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logtail-python-0.2.5.tar", last modified: Fri May  5 17:19:29 2023, max compression
+gzip compressed data, was "logtail-python-0.2.6.tar", last modified: Thu May 25 09:48:28 2023, max compression
```

## Comparing `logtail-python-0.2.5.tar` & `logtail-python-0.2.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-05 17:19:29.126438 logtail-python-0.2.5/
--rw-r--r--   0 simon      (501) staff       (20)      737 2023-02-17 20:58:53.000000 logtail-python-0.2.5/LICENSE.md
--rw-r--r--   0 simon      (501) staff       (20)      115 2023-02-17 20:58:53.000000 logtail-python-0.2.5/MANIFEST.in
--rw-r--r--   0 simon      (501) staff       (20)     2107 2023-05-05 17:19:29.126499 logtail-python-0.2.5/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-03-30 09:34:01.000000 logtail-python-0.2.5/README.md
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-05 17:19:29.124220 logtail-python-0.2.5/logtail/
--rw-r--r--   0 simon      (501) staff       (20)      252 2023-05-05 17:09:07.000000 logtail-python-0.2.5/logtail/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)      141 2023-02-17 20:58:53.000000 logtail-python-0.2.5/logtail/compat.py
--rw-r--r--   0 simon      (501) staff       (20)     2999 2023-03-30 14:07:44.000000 logtail-python-0.2.5/logtail/flusher.py
--rw-r--r--   0 simon      (501) staff       (20)      968 2023-02-17 20:58:53.000000 logtail-python-0.2.5/logtail/formatter.py
--rw-r--r--   0 simon      (501) staff       (20)     2497 2023-05-05 17:05:57.000000 logtail-python-0.2.5/logtail/frame.py
--rw-r--r--   0 simon      (501) staff       (20)     2617 2023-03-30 09:09:04.000000 logtail-python-0.2.5/logtail/handler.py
--rw-r--r--   0 simon      (501) staff       (20)     1156 2023-02-17 20:58:53.000000 logtail-python-0.2.5/logtail/helpers.py
--rw-r--r--   0 simon      (501) staff       (20)      588 2023-03-30 09:24:28.000000 logtail-python-0.2.5/logtail/uploader.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-05 17:19:29.124738 logtail-python-0.2.5/logtail_python.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     2107 2023-05-05 17:19:29.000000 logtail-python-0.2.5/logtail_python.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      909 2023-05-05 17:19:29.000000 logtail-python-0.2.5/logtail_python.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2023-05-05 17:19:29.000000 logtail-python-0.2.5/logtail_python.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)       32 2023-05-05 17:19:29.000000 logtail-python-0.2.5/logtail_python.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)        8 2023-05-05 17:19:29.000000 logtail-python-0.2.5/logtail_python.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)       32 2023-02-17 20:58:53.000000 logtail-python-0.2.5/requirements.txt
--rw-r--r--   0 simon      (501) staff       (20)       67 2023-05-05 17:19:29.126717 logtail-python-0.2.5/setup.cfg
--rw-r--r--   0 simon      (501) staff       (20)     1551 2023-05-05 17:06:09.000000 logtail-python-0.2.5/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       54 2023-03-30 14:07:44.000000 logtail-python-0.2.5/test-requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-05 17:19:29.125531 logtail-python-0.2.5/tests/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-02-17 20:58:53.000000 logtail-python-0.2.5/tests/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-05 17:19:29.126329 logtail-python-0.2.5/tests/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      158 2023-02-19 13:17:27.000000 logtail-python-0.2.5/tests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 simon      (501) staff       (20)    10312 2023-03-30 12:30:52.000000 logtail-python-0.2.5/tests/__pycache__/test_flusher.cpython-311.pyc
--rw-r--r--   0 simon      (501) staff       (20)    11774 2023-03-30 12:30:52.000000 logtail-python-0.2.5/tests/__pycache__/test_formatter.cpython-311.pyc
--rw-r--r--   0 simon      (501) staff       (20)     3465 2023-03-30 12:30:52.000000 logtail-python-0.2.5/tests/__pycache__/test_frame.cpython-311.pyc
--rw-r--r--   0 simon      (501) staff       (20)     8319 2023-03-30 12:30:52.000000 logtail-python-0.2.5/tests/__pycache__/test_handler.cpython-311.pyc
--rw-r--r--   0 simon      (501) staff       (20)     4559 2023-03-30 12:30:52.000000 logtail-python-0.2.5/tests/__pycache__/test_helpers.cpython-311.pyc
--rw-r--r--   0 simon      (501) staff       (20)     2147 2023-03-30 12:30:52.000000 logtail-python-0.2.5/tests/__pycache__/test_uploader.cpython-311.pyc
--rw-r--r--   0 simon      (501) staff       (20)     5061 2023-03-30 14:07:44.000000 logtail-python-0.2.5/tests/test_flusher.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-03-30 14:07:44.000000 logtail-python-0.2.5/tests/test_formatter.py
--rw-r--r--   0 simon      (501) staff       (20)     1953 2023-03-30 14:07:44.000000 logtail-python-0.2.5/tests/test_frame.py
--rw-r--r--   0 simon      (501) staff       (20)     4565 2023-03-30 14:07:44.000000 logtail-python-0.2.5/tests/test_handler.py
--rw-r--r--   0 simon      (501) staff       (20)     1844 2023-03-30 14:07:44.000000 logtail-python-0.2.5/tests/test_helpers.py
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-30 14:07:44.000000 logtail-python-0.2.5/tests/test_uploader.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 09:48:28.914450 logtail-python-0.2.6/
+-rw-r--r--   0 simon      (501) staff       (20)      737 2023-02-17 20:58:53.000000 logtail-python-0.2.6/LICENSE.md
+-rw-r--r--   0 simon      (501) staff       (20)      115 2023-02-17 20:58:53.000000 logtail-python-0.2.6/MANIFEST.in
+-rw-r--r--   0 simon      (501) staff       (20)     2197 2023-05-25 09:48:28.914506 logtail-python-0.2.6/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)     1155 2023-05-25 09:27:43.000000 logtail-python-0.2.6/README.md
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 09:48:28.912140 logtail-python-0.2.6/logtail/
+-rw-r--r--   0 simon      (501) staff       (20)      252 2023-05-25 09:44:00.000000 logtail-python-0.2.6/logtail/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)      141 2023-02-17 20:58:53.000000 logtail-python-0.2.6/logtail/compat.py
+-rw-r--r--   0 simon      (501) staff       (20)     3245 2023-05-25 08:56:12.000000 logtail-python-0.2.6/logtail/flusher.py
+-rw-r--r--   0 simon      (501) staff       (20)      968 2023-02-17 20:58:53.000000 logtail-python-0.2.6/logtail/formatter.py
+-rw-r--r--   0 simon      (501) staff       (20)     2497 2023-05-05 17:05:57.000000 logtail-python-0.2.6/logtail/frame.py
+-rw-r--r--   0 simon      (501) staff       (20)     2626 2023-05-25 09:02:24.000000 logtail-python-0.2.6/logtail/handler.py
+-rw-r--r--   0 simon      (501) staff       (20)     1156 2023-02-17 20:58:53.000000 logtail-python-0.2.6/logtail/helpers.py
+-rw-r--r--   0 simon      (501) staff       (20)      805 2023-05-25 09:41:47.000000 logtail-python-0.2.6/logtail/uploader.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 09:48:28.912713 logtail-python-0.2.6/logtail_python.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     2197 2023-05-25 09:48:28.000000 logtail-python-0.2.6/logtail_python.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      909 2023-05-25 09:48:28.000000 logtail-python-0.2.6/logtail_python.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2023-05-25 09:48:28.000000 logtail-python-0.2.6/logtail_python.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)       32 2023-05-25 09:48:28.000000 logtail-python-0.2.6/logtail_python.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)        8 2023-05-25 09:48:28.000000 logtail-python-0.2.6/logtail_python.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)       32 2023-02-17 20:58:53.000000 logtail-python-0.2.6/requirements.txt
+-rw-r--r--   0 simon      (501) staff       (20)       67 2023-05-25 09:48:28.914692 logtail-python-0.2.6/setup.cfg
+-rw-r--r--   0 simon      (501) staff       (20)     1551 2023-05-25 09:43:39.000000 logtail-python-0.2.6/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       54 2023-03-30 14:07:44.000000 logtail-python-0.2.6/test-requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 09:48:28.913524 logtail-python-0.2.6/tests/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-02-17 20:58:53.000000 logtail-python-0.2.6/tests/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 09:48:28.914329 logtail-python-0.2.6/tests/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      158 2023-02-19 13:17:27.000000 logtail-python-0.2.6/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 simon      (501) staff       (20)    10312 2023-03-30 12:30:52.000000 logtail-python-0.2.6/tests/__pycache__/test_flusher.cpython-311.pyc
+-rw-r--r--   0 simon      (501) staff       (20)    11774 2023-03-30 12:30:52.000000 logtail-python-0.2.6/tests/__pycache__/test_formatter.cpython-311.pyc
+-rw-r--r--   0 simon      (501) staff       (20)     3465 2023-03-30 12:30:52.000000 logtail-python-0.2.6/tests/__pycache__/test_frame.cpython-311.pyc
+-rw-r--r--   0 simon      (501) staff       (20)     8319 2023-03-30 12:30:52.000000 logtail-python-0.2.6/tests/__pycache__/test_handler.cpython-311.pyc
+-rw-r--r--   0 simon      (501) staff       (20)     4559 2023-03-30 12:30:52.000000 logtail-python-0.2.6/tests/__pycache__/test_helpers.cpython-311.pyc
+-rw-r--r--   0 simon      (501) staff       (20)     2147 2023-03-30 12:30:52.000000 logtail-python-0.2.6/tests/__pycache__/test_uploader.cpython-311.pyc
+-rw-r--r--   0 simon      (501) staff       (20)     5061 2023-03-30 14:07:44.000000 logtail-python-0.2.6/tests/test_flusher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-03-30 14:07:44.000000 logtail-python-0.2.6/tests/test_formatter.py
+-rw-r--r--   0 simon      (501) staff       (20)     1953 2023-03-30 14:07:44.000000 logtail-python-0.2.6/tests/test_frame.py
+-rw-r--r--   0 simon      (501) staff       (20)     4565 2023-03-30 14:07:44.000000 logtail-python-0.2.6/tests/test_handler.py
+-rw-r--r--   0 simon      (501) staff       (20)     1844 2023-03-30 14:07:44.000000 logtail-python-0.2.6/tests/test_helpers.py
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-30 14:07:44.000000 logtail-python-0.2.6/tests/test_uploader.py
```

### Comparing `logtail-python-0.2.5/LICENSE.md` & `logtail-python-0.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.5/PKG-INFO` & `logtail-python-0.2.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: logtail-python
-Version: 0.2.5
+Version: 0.2.6
 Summary: Logtail.com client library
 Home-page: https://github.com/logtail/logtail-python
-Download-URL: https://github.com/logtail/logtail-python/tarball/0.2.5
+Download-URL: https://github.com/logtail/logtail-python/tarball/0.2.6
 Author: Logtail
 Author-email: hello@logtail.com
 License: ISC
 Keywords: api,logtail,logging,client
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
@@ -20,24 +20,26 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# [Logtail](https://betterstack.com/logtail) Python client by [Better Stack](https://betterstack.com/)
+# [Better Stack](https://betterstack.com/logs) Python client
+
+📣 Logtail is now part of Better Stack · [Learn more ⇗](https://betterstack.com/press/introducing-better-stack/)
   
-  [![Logtail python client](https://user-images.githubusercontent.com/19272921/154085622-59997d5a-3f91-4bc9-a815-3b8ead16d28d.jpeg)](https://betterstack.com/logtail)
+[![Better Stack Python client](https://user-images.githubusercontent.com/19272921/154085622-59997d5a-3f91-4bc9-a815-3b8ead16d28d.jpeg)](https://betterstack.com/logs)
 
 
 [![ISC License](https://img.shields.io/badge/license-ISC-ff69b4.svg)](LICENSE.md)
 [![PyPI package](https://badge.fury.io/py/logtail-python.svg)](https://badge.fury.io/py/logtail-python)
-![Logtail python client](https://github.com/logtail/logtail-python/actions/workflows/main.yml/badge.svg?branch=master)
+![Better Stack Python client](https://github.com/logtail/logtail-python/actions/workflows/main.yml/badge.svg?branch=master)
 
-Experience SQL-compatible structured log management based on ClickHouse. [Learn more ⇗](https://logtail.com/)
+Experience SQL-compatible structured log management based on ClickHouse. [Learn more ⇗](https://betterstack.com/logs)
 
 ## Documentation
 
 [Getting started ⇗](https://betterstack.com/docs/logs/python/)
 
 ## Need help?
 Please let us know at [hello@betterstack.com](mailto:hello@betterstack.com). We're happy to help!
```

### Comparing `logtail-python-0.2.5/README.md` & `logtail-python-0.2.6/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-# [Logtail](https://betterstack.com/logtail) Python client by [Better Stack](https://betterstack.com/)
+# [Better Stack](https://betterstack.com/logs) Python client
+
+📣 Logtail is now part of Better Stack · [Learn more ⇗](https://betterstack.com/press/introducing-better-stack/)
   
-  [![Logtail python client](https://user-images.githubusercontent.com/19272921/154085622-59997d5a-3f91-4bc9-a815-3b8ead16d28d.jpeg)](https://betterstack.com/logtail)
+[![Better Stack Python client](https://user-images.githubusercontent.com/19272921/154085622-59997d5a-3f91-4bc9-a815-3b8ead16d28d.jpeg)](https://betterstack.com/logs)
 
 
 [![ISC License](https://img.shields.io/badge/license-ISC-ff69b4.svg)](LICENSE.md)
 [![PyPI package](https://badge.fury.io/py/logtail-python.svg)](https://badge.fury.io/py/logtail-python)
-![Logtail python client](https://github.com/logtail/logtail-python/actions/workflows/main.yml/badge.svg?branch=master)
+![Better Stack Python client](https://github.com/logtail/logtail-python/actions/workflows/main.yml/badge.svg?branch=master)
 
-Experience SQL-compatible structured log management based on ClickHouse. [Learn more ⇗](https://logtail.com/)
+Experience SQL-compatible structured log management based on ClickHouse. [Learn more ⇗](https://betterstack.com/logs)
 
 ## Documentation
 
 [Getting started ⇗](https://betterstack.com/docs/logs/python/)
 
 ## Need help?
 Please let us know at [hello@betterstack.com](mailto:hello@betterstack.com). We're happy to help!
```

### Comparing `logtail-python-0.2.5/logtail/flusher.py` & `logtail-python-0.2.6/logtail/flusher.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,21 +52,25 @@
             time_remaining = _calculate_time_remaining(last_flush, self.flush_interval)
 
         # Send phase: takes the outstanding events (up to `buffer_capacity`
         # count) and sends them to the Logtail endpoint all at once. If the
         # request fails in a way that can be retried, it is retried with an
         # exponential backoff in between attempts.
         if frame:
+            response = None
             for delay in RETRY_SCHEDULE + (None, ):
                 response = self.upload(frame)
                 if not _should_retry(response.status_code):
                     break
                 if delay is not None:
                     time.sleep(delay)
 
+            if response.status_code == 500 and getattr(response, "exception") != None:
+                print('Failed to send logs to Better Stack after {} retries: {}'.format(len(RETRY_SCHEDULE), response.exception))
+
         if shutdown:
             sys.exit(0)
 
 
 def _initial_time_remaining(flush_interval):
     return flush_interval
```

### Comparing `logtail-python-0.2.5/logtail/formatter.py` & `logtail-python-0.2.6/logtail/formatter.py`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.5/logtail/frame.py` & `logtail-python-0.2.6/logtail/frame.py`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.5/logtail/handler.py` & `logtail-python-0.2.6/logtail/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from .compat import queue
 from .helpers import DEFAULT_CONTEXT
 from .flusher import FlushWorker
 from .uploader import Uploader
 from .frame import create_frame
 
-DEFAULT_HOST = 'https://in.logtail.com'
+DEFAULT_HOST = 'https://in.logs.betterstack.com'
 DEFAULT_BUFFER_CAPACITY = 1000
 DEFAULT_FLUSH_INTERVAL = 1
 DEFAULT_RAISE_EXCEPTIONS = False
 DEFAULT_DROP_EXTRA_EVENTS = True
 DEFAULT_INCLUDE_EXTRA_ATTRIBUTES = True
```

### Comparing `logtail-python-0.2.5/logtail/helpers.py` & `logtail-python-0.2.6/logtail/helpers.py`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.5/logtail/uploader.py` & `logtail-python-0.2.6/logtail/uploader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 # coding: utf-8
 from __future__ import print_function, unicode_literals
 import msgpack
 import requests
 
+class Fake500(object):
+    def __init__(self, exception):
+        self.status_code = 500
+        self.exception = exception
 
 class Uploader(object):
     def __init__(self, source_token, host):
         self.source_token = source_token
         self.host = host
         self.session = requests.Session()
         self.headers = {
             'Authorization': 'Bearer %s' % source_token,
             'Content-Type': 'application/msgpack',
         }
 
     def __call__(self, frame):
         data = msgpack.packb(frame, use_bin_type=True)
-        return self.session.post(self.host, data=data, headers=self.headers)
+        try:
+            return self.session.post(self.host, data=data, headers=self.headers)
+        except requests.RequestException as e:
+            return Fake500(e)
```

### Comparing `logtail-python-0.2.5/logtail_python.egg-info/PKG-INFO` & `logtail-python-0.2.6/logtail_python.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: logtail-python
-Version: 0.2.5
+Version: 0.2.6
 Summary: Logtail.com client library
 Home-page: https://github.com/logtail/logtail-python
-Download-URL: https://github.com/logtail/logtail-python/tarball/0.2.5
+Download-URL: https://github.com/logtail/logtail-python/tarball/0.2.6
 Author: Logtail
 Author-email: hello@logtail.com
 License: ISC
 Keywords: api,logtail,logging,client
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
@@ -20,24 +20,26 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# [Logtail](https://betterstack.com/logtail) Python client by [Better Stack](https://betterstack.com/)
+# [Better Stack](https://betterstack.com/logs) Python client
+
+📣 Logtail is now part of Better Stack · [Learn more ⇗](https://betterstack.com/press/introducing-better-stack/)
   
-  [![Logtail python client](https://user-images.githubusercontent.com/19272921/154085622-59997d5a-3f91-4bc9-a815-3b8ead16d28d.jpeg)](https://betterstack.com/logtail)
+[![Better Stack Python client](https://user-images.githubusercontent.com/19272921/154085622-59997d5a-3f91-4bc9-a815-3b8ead16d28d.jpeg)](https://betterstack.com/logs)
 
 
 [![ISC License](https://img.shields.io/badge/license-ISC-ff69b4.svg)](LICENSE.md)
 [![PyPI package](https://badge.fury.io/py/logtail-python.svg)](https://badge.fury.io/py/logtail-python)
-![Logtail python client](https://github.com/logtail/logtail-python/actions/workflows/main.yml/badge.svg?branch=master)
+![Better Stack Python client](https://github.com/logtail/logtail-python/actions/workflows/main.yml/badge.svg?branch=master)
 
-Experience SQL-compatible structured log management based on ClickHouse. [Learn more ⇗](https://logtail.com/)
+Experience SQL-compatible structured log management based on ClickHouse. [Learn more ⇗](https://betterstack.com/logs)
 
 ## Documentation
 
 [Getting started ⇗](https://betterstack.com/docs/logs/python/)
 
 ## Need help?
 Please let us know at [hello@betterstack.com](mailto:hello@betterstack.com). We're happy to help!
```

### Comparing `logtail-python-0.2.5/logtail_python.egg-info/SOURCES.txt` & `logtail-python-0.2.6/logtail_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.5/setup.py` & `logtail-python-0.2.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 import os
 from setuptools import setup
 
 
-VERSION = '0.2.5'
+VERSION = '0.2.6'
 ROOT_DIR = os.path.dirname(__file__)
 
 REQUIREMENTS = [
     line.strip() for line in
     open(os.path.join(ROOT_DIR, 'requirements.txt')).readlines()
 ]
```

### Comparing `logtail-python-0.2.5/tests/__pycache__/test_flusher.cpython-311.pyc` & `logtail-python-0.2.6/tests/__pycache__/test_flusher.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.5/tests/__pycache__/test_formatter.cpython-311.pyc` & `logtail-python-0.2.6/tests/__pycache__/test_formatter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.5/tests/__pycache__/test_frame.cpython-311.pyc` & `logtail-python-0.2.6/tests/__pycache__/test_frame.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.5/tests/__pycache__/test_handler.cpython-311.pyc` & `logtail-python-0.2.6/tests/__pycache__/test_handler.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.5/tests/__pycache__/test_helpers.cpython-311.pyc` & `logtail-python-0.2.6/tests/__pycache__/test_helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.5/tests/__pycache__/test_uploader.cpython-311.pyc` & `logtail-python-0.2.6/tests/__pycache__/test_uploader.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.5/tests/test_flusher.py` & `logtail-python-0.2.6/tests/test_flusher.py`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.5/tests/test_formatter.py` & `logtail-python-0.2.6/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.5/tests/test_frame.py` & `logtail-python-0.2.6/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.5/tests/test_handler.py` & `logtail-python-0.2.6/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.5/tests/test_helpers.py` & `logtail-python-0.2.6/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.5/tests/test_uploader.py` & `logtail-python-0.2.6/tests/test_uploader.py`

 * *Files identical despite different names*

