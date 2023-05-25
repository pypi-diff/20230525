# Comparing `tmp/aiobtclientrpc-4.0.0.tar.gz` & `tmp/aiobtclientrpc-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiobtclientrpc-4.0.0.tar", last modified: Mon Apr  3 17:20:37 2023, max compression
+gzip compressed data, was "aiobtclientrpc-5.0.0.tar", last modified: Thu May 25 10:11:57 2023, max compression
```

## Comparing `aiobtclientrpc-4.0.0.tar` & `aiobtclientrpc-5.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 17:20:37.102346 aiobtclientrpc-4.0.0/
--rw-------   0 ich       (1000) ich       (1000)    35149 2021-12-20 12:15:00.000000 aiobtclientrpc-4.0.0/LICENSE
--rw-------   0 ich       (1000) ich       (1000)     1871 2023-04-03 17:20:37.102346 aiobtclientrpc-4.0.0/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     1267 2022-08-27 13:53:43.000000 aiobtclientrpc-4.0.0/README.rst
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 17:20:37.082346 aiobtclientrpc-4.0.0/aiobtclientrpc/
--rw-------   0 ich       (1000) ich       (1000)      672 2023-04-03 17:19:58.000000 aiobtclientrpc-4.0.0/aiobtclientrpc/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    20421 2022-09-11 09:24:18.000000 aiobtclientrpc-4.0.0/aiobtclientrpc/_base.py
--rw-------   0 ich       (1000) ich       (1000)    17105 2023-03-02 11:18:52.000000 aiobtclientrpc-4.0.0/aiobtclientrpc/_deluge.py
--rw-------   0 ich       (1000) ich       (1000)     3374 2023-04-03 16:01:15.000000 aiobtclientrpc-4.0.0/aiobtclientrpc/_errors.py
--rw-------   0 ich       (1000) ich       (1000)     5488 2023-04-03 15:36:25.000000 aiobtclientrpc-4.0.0/aiobtclientrpc/_qbittorrent.py
--rw-------   0 ich       (1000) ich       (1000)    14972 2022-08-10 13:41:56.000000 aiobtclientrpc-4.0.0/aiobtclientrpc/_rtorrent.py
--rw-------   0 ich       (1000) ich       (1000)     4322 2023-04-03 16:46:08.000000 aiobtclientrpc-4.0.0/aiobtclientrpc/_transmission.py
--rw-------   0 ich       (1000) ich       (1000)    13875 2023-03-02 18:36:04.000000 aiobtclientrpc-4.0.0/aiobtclientrpc/_utils.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 17:20:37.086346 aiobtclientrpc-4.0.0/aiobtclientrpc.egg-info/
--rw-------   0 ich       (1000) ich       (1000)     1871 2023-04-03 17:20:37.000000 aiobtclientrpc-4.0.0/aiobtclientrpc.egg-info/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)      815 2023-04-03 17:20:37.000000 aiobtclientrpc-4.0.0/aiobtclientrpc.egg-info/SOURCES.txt
--rw-------   0 ich       (1000) ich       (1000)        1 2023-04-03 17:20:37.000000 aiobtclientrpc-4.0.0/aiobtclientrpc.egg-info/dependency_links.txt
--rw-------   0 ich       (1000) ich       (1000)      100 2023-04-03 17:20:37.000000 aiobtclientrpc-4.0.0/aiobtclientrpc.egg-info/requires.txt
--rw-------   0 ich       (1000) ich       (1000)       21 2023-04-03 17:20:37.000000 aiobtclientrpc-4.0.0/aiobtclientrpc.egg-info/top_level.txt
--rw-------   0 ich       (1000) ich       (1000)       38 2023-04-03 17:20:37.102346 aiobtclientrpc-4.0.0/setup.cfg
--rw-------   0 ich       (1000) ich       (1000)     1352 2022-08-05 09:51:28.000000 aiobtclientrpc-4.0.0/setup.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 17:20:37.094346 aiobtclientrpc-4.0.0/tests/
--rw-------   0 ich       (1000) ich       (1000)        0 2022-02-07 12:05:52.000000 aiobtclientrpc-4.0.0/tests/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    26329 2022-12-18 13:41:34.000000 aiobtclientrpc-4.0.0/tests/base_test.py
--rw-------   0 ich       (1000) ich       (1000)      775 2023-03-02 11:22:02.000000 aiobtclientrpc-4.0.0/tests/common.py
--rw-------   0 ich       (1000) ich       (1000)    34762 2022-08-10 13:42:02.000000 aiobtclientrpc-4.0.0/tests/deluge_test.py
--rw-------   0 ich       (1000) ich       (1000)     1716 2022-06-28 10:56:05.000000 aiobtclientrpc-4.0.0/tests/errors_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 17:20:37.102346 aiobtclientrpc-4.0.0/tests/integration_tests/
--rw-------   0 ich       (1000) ich       (1000)        0 2022-02-13 12:43:38.000000 aiobtclientrpc-4.0.0/tests/integration_tests/__init__.py
--rw-------   0 ich       (1000) ich       (1000)      509 2022-02-14 10:13:02.000000 aiobtclientrpc-4.0.0/tests/integration_tests/common.py
--rw-------   0 ich       (1000) ich       (1000)     2340 2022-12-18 12:59:33.000000 aiobtclientrpc-4.0.0/tests/integration_tests/conftest.py
--rw-------   0 ich       (1000) ich       (1000)     8298 2022-12-18 12:34:20.000000 aiobtclientrpc-4.0.0/tests/integration_tests/integration_test.py
--rw-------   0 ich       (1000) ich       (1000)     1928 2022-02-28 15:30:24.000000 aiobtclientrpc-4.0.0/tests/integration_tests/proxyserver.py
--rw-------   0 ich       (1000) ich       (1000)     8685 2022-08-10 13:42:03.000000 aiobtclientrpc-4.0.0/tests/qbittorrent_test.py
--rw-------   0 ich       (1000) ich       (1000)    31353 2022-08-10 13:42:04.000000 aiobtclientrpc-4.0.0/tests/rtorrent_test.py
--rw-------   0 ich       (1000) ich       (1000)     9948 2023-04-03 16:01:02.000000 aiobtclientrpc-4.0.0/tests/transmission_test.py
--rw-------   0 ich       (1000) ich       (1000)    33220 2023-03-02 18:35:57.000000 aiobtclientrpc-4.0.0/tests/utils_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:11:57.967119 aiobtclientrpc-5.0.0/
+-rw-------   0 ich       (1000) ich       (1000)    35149 2021-12-20 12:15:00.000000 aiobtclientrpc-5.0.0/LICENSE
+-rw-------   0 ich       (1000) ich       (1000)     1922 2023-05-25 10:11:57.967119 aiobtclientrpc-5.0.0/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     1267 2022-08-27 13:53:43.000000 aiobtclientrpc-5.0.0/README.rst
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:11:57.967119 aiobtclientrpc-5.0.0/aiobtclientrpc/
+-rw-------   0 ich       (1000) ich       (1000)      672 2023-05-08 17:36:18.000000 aiobtclientrpc-5.0.0/aiobtclientrpc/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    20421 2023-05-09 09:55:34.000000 aiobtclientrpc-5.0.0/aiobtclientrpc/_base.py
+-rw-------   0 ich       (1000) ich       (1000)    15973 2023-04-29 13:49:49.000000 aiobtclientrpc-5.0.0/aiobtclientrpc/_deluge.py
+-rw-------   0 ich       (1000) ich       (1000)     3888 2023-04-29 14:37:52.000000 aiobtclientrpc-5.0.0/aiobtclientrpc/_errors.py
+-rw-------   0 ich       (1000) ich       (1000)     5488 2023-05-15 09:55:47.000000 aiobtclientrpc-5.0.0/aiobtclientrpc/_qbittorrent.py
+-rw-------   0 ich       (1000) ich       (1000)    14972 2023-04-29 17:55:19.000000 aiobtclientrpc-5.0.0/aiobtclientrpc/_rtorrent.py
+-rw-------   0 ich       (1000) ich       (1000)     4660 2023-04-29 14:37:52.000000 aiobtclientrpc-5.0.0/aiobtclientrpc/_transmission.py
+-rw-------   0 ich       (1000) ich       (1000)    13874 2023-04-29 13:48:48.000000 aiobtclientrpc-5.0.0/aiobtclientrpc/_utils.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:11:57.967119 aiobtclientrpc-5.0.0/aiobtclientrpc.egg-info/
+-rw-------   0 ich       (1000) ich       (1000)     1922 2023-05-25 10:11:57.000000 aiobtclientrpc-5.0.0/aiobtclientrpc.egg-info/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)      815 2023-05-25 10:11:57.000000 aiobtclientrpc-5.0.0/aiobtclientrpc.egg-info/SOURCES.txt
+-rw-------   0 ich       (1000) ich       (1000)        1 2023-05-25 10:11:57.000000 aiobtclientrpc-5.0.0/aiobtclientrpc.egg-info/dependency_links.txt
+-rw-------   0 ich       (1000) ich       (1000)      100 2023-05-25 10:11:57.000000 aiobtclientrpc-5.0.0/aiobtclientrpc.egg-info/requires.txt
+-rw-------   0 ich       (1000) ich       (1000)       21 2023-05-25 10:11:57.000000 aiobtclientrpc-5.0.0/aiobtclientrpc.egg-info/top_level.txt
+-rw-------   0 ich       (1000) ich       (1000)       38 2023-05-25 10:11:57.967119 aiobtclientrpc-5.0.0/setup.cfg
+-rw-------   0 ich       (1000) ich       (1000)     1402 2023-05-25 09:57:55.000000 aiobtclientrpc-5.0.0/setup.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:11:57.967119 aiobtclientrpc-5.0.0/tests/
+-rw-------   0 ich       (1000) ich       (1000)        0 2022-02-07 12:05:52.000000 aiobtclientrpc-5.0.0/tests/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    26329 2022-12-18 13:41:34.000000 aiobtclientrpc-5.0.0/tests/base_test.py
+-rw-------   0 ich       (1000) ich       (1000)      775 2023-03-02 11:22:02.000000 aiobtclientrpc-5.0.0/tests/common.py
+-rw-------   0 ich       (1000) ich       (1000)    35426 2023-05-08 17:01:03.000000 aiobtclientrpc-5.0.0/tests/deluge_test.py
+-rw-------   0 ich       (1000) ich       (1000)     3532 2023-04-29 14:37:52.000000 aiobtclientrpc-5.0.0/tests/errors_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:11:57.967119 aiobtclientrpc-5.0.0/tests/integration_tests/
+-rw-------   0 ich       (1000) ich       (1000)        0 2022-02-13 12:43:38.000000 aiobtclientrpc-5.0.0/tests/integration_tests/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)      947 2023-05-02 05:26:21.000000 aiobtclientrpc-5.0.0/tests/integration_tests/common.py
+-rw-------   0 ich       (1000) ich       (1000)     2751 2023-04-30 12:57:49.000000 aiobtclientrpc-5.0.0/tests/integration_tests/conftest.py
+-rw-------   0 ich       (1000) ich       (1000)     8101 2023-05-02 05:38:37.000000 aiobtclientrpc-5.0.0/tests/integration_tests/integration_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1928 2022-02-28 15:30:24.000000 aiobtclientrpc-5.0.0/tests/integration_tests/proxyserver.py
+-rw-------   0 ich       (1000) ich       (1000)     8685 2022-08-10 13:42:03.000000 aiobtclientrpc-5.0.0/tests/qbittorrent_test.py
+-rw-------   0 ich       (1000) ich       (1000)    31353 2022-08-10 13:42:04.000000 aiobtclientrpc-5.0.0/tests/rtorrent_test.py
+-rw-------   0 ich       (1000) ich       (1000)    10380 2023-04-29 14:38:58.000000 aiobtclientrpc-5.0.0/tests/transmission_test.py
+-rw-------   0 ich       (1000) ich       (1000)    33339 2023-05-08 17:07:14.000000 aiobtclientrpc-5.0.0/tests/utils_test.py
```

### Comparing `aiobtclientrpc-4.0.0/LICENSE` & `aiobtclientrpc-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiobtclientrpc-4.0.0/PKG-INFO` & `aiobtclientrpc-5.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: aiobtclientrpc
-Version: 4.0.0
+Version: 5.0.0
 Summary: Asynchronous low-level communication with BitTorrent clients
 Home-page: https://codeberg.org/plotski/aiobtclientrpc
 Author: plotski
 Author-email: plotski@example.org
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ``aiobtclientrpc`` provides low-level access to the RPC protocols of BitTorrent
 clients. It is supposed to be the basis for a high-level library. If you want to
```

### Comparing `aiobtclientrpc-4.0.0/README.rst` & `aiobtclientrpc-5.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `aiobtclientrpc-4.0.0/aiobtclientrpc/__init__.py` & `aiobtclientrpc-5.0.0/aiobtclientrpc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Asynchronous low-level communication with BitTorrent clients
 """
 
 __project_name__ = 'aiobtclientrpc'
 __description__ = 'Asynchronous low-level communication with BitTorrent clients'
 __homepage__ = 'https://codeberg.org/plotski/aiobtclientrpc'
-__version__ = '4.0.0'
+__version__ = '5.0.0'
 __author__ = 'plotski'
 __author_email__ = 'plotski@example.org'
 
 # isort:skip_file
 
 from ._base import RPCBase
 from ._errors import *
```

### Comparing `aiobtclientrpc-4.0.0/aiobtclientrpc/_base.py` & `aiobtclientrpc-5.0.0/aiobtclientrpc/_base.py`

 * *Files identical despite different names*

### Comparing `aiobtclientrpc-4.0.0/aiobtclientrpc/_deluge.py` & `aiobtclientrpc-5.0.0/aiobtclientrpc/_deluge.py`

 * *Files 12% similar despite different names*

```diff
@@ -417,55 +417,14 @@
             f'{self.MESSAGE_HEADER_FORMAT}{body_len}s',
             self.PROTOCOL_VERSION,
             body_len,
             body,
         )
         self._transport.write(packed)
 
-    _valid_types = {
-        list,
-        tuple,
-        dict,
-        str,
-        bytes,
-        int,
-        float,
-        bool,
-        type(None),
-    }
-
-    def _convert_to_valid_type(self, data):
-        # rencode only allows specific types. Here we convert subclasses of
-        # these types back to allowed types.
-
-        data_type = type(data)
-        if data_type == list:
-            return [
-                self._convert_to_valid_type(item)
-                for item in data
-            ]
-        elif data_type == tuple:
-            return tuple(
-                self._convert_to_valid_type(item)
-                for item in data
-            )
-        elif data_type == dict:
-            return {
-                self._convert_to_valid_type(k) : self._convert_to_valid_type(v)
-                for k, v in data.items()
-            }
-        elif data_type in self._valid_types:
-            return data
-
-        for t in self._valid_types:
-            if isinstance(data, t):
-                return self._convert_to_valid_type(t(data))
-
-        raise TypeError(f'Unsupported type: {type(data).__name__}: {data!r}')
-
     def send_request(self, request):
         _log.debug('Sending request #%d: %r', request.id, request)
         self._requests[request.id] = request
         self._transfer_messages(request.format_message())
         return request.future
```

### Comparing `aiobtclientrpc-4.0.0/aiobtclientrpc/_errors.py` & `aiobtclientrpc-5.0.0/aiobtclientrpc/_errors.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,50 @@
 import re
 
 
 class Error(Exception):
     """Base class for all exceptions raised by this package"""
 
     def __eq__(self, other):
-        return (
-            type(self) is type(other)
-            and str(self) == str(other)
-        )
+        if isinstance(other, type(self)):
+            return str(self) == str(other)
+        else:
+            return NotImplemented
 
 
 class RPCError(Error):
     """
     Generic RPC error
 
     This can be some kind of miscommunication with the RPC service (e.g. unknown
     method called, invalid or missing argument, etc), which should be a
     considered a bug. But it can also be a normal error message (e.g. unknown
     torrent), that should be communicated to the user.
     """
 
+    def __init__(self, msg, info=None):
+        super().__init__(msg)
+        self._info = info
+
+    @property
+    def info(self):
+        """
+        """
+        return self._info
+
+    def __repr__(self):
+        return f'{type(self).__name__}({str(self)!r}, info={self._info!r})'
+
+    def __eq__(self, other):
+        equal = super().__eq__(other)
+        if equal is True and hasattr(other, 'info'):
+            return other.info == self.info
+        else:
+            return equal
+
     def translate(self, map):
         # By using r-string we don't have to escape backslashes
         r"""
         Turn this exception into another one based on regular expressions
 
         :param map: Mapping of regular expression strings to target exception
             instances
```

### Comparing `aiobtclientrpc-4.0.0/aiobtclientrpc/_qbittorrent.py` & `aiobtclientrpc-5.0.0/aiobtclientrpc/_qbittorrent.py`

 * *Files identical despite different names*

### Comparing `aiobtclientrpc-4.0.0/aiobtclientrpc/_rtorrent.py` & `aiobtclientrpc-5.0.0/aiobtclientrpc/_rtorrent.py`

 * *Files identical despite different names*

### Comparing `aiobtclientrpc-4.0.0/aiobtclientrpc/_transmission.py` & `aiobtclientrpc-5.0.0/aiobtclientrpc/_transmission.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,15 +130,27 @@
         await self._request('session-stats')
 
     async def _disconnect(self):
         # Forget CSRF header
         self._http_headers.clear()
 
     async def _call(self, method, args=None, **kwargs):
+        # Combine keyword arguments and dictionary (`args`)
         if args:
             kwargs.update(args)
+
         response = await self._request(method, **kwargs)
+
         try:
-            # Any error message is in "result" field in the returned JSON object
-            return response.json()
+            result = response.json()
         except Exception:
             raise _errors.RPCError(f'Unexpected response: {response.text}')
+        else:
+            message = result.get('result')
+            if message == 'success':
+                return result
+            else:
+                # Transmission errors are all lower case
+                raise _errors.RPCError(
+                    message.capitalize(),
+                    info=result.get('arguments', None),
+                )
```

### Comparing `aiobtclientrpc-4.0.0/aiobtclientrpc/_utils.py` & `aiobtclientrpc-5.0.0/aiobtclientrpc/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,15 +465,15 @@
     elif data_type == tuple:
         return tuple(
             convert_to_basic_type(item)
             for item in data
         )
     elif data_type == dict:
         return {
-            convert_to_basic_type(k) : convert_to_basic_type(v)
+            convert_to_basic_type(k): convert_to_basic_type(v)
             for k, v in data.items()
         }
     elif data_type in _basic_types:
         return data
 
     else:
         for t in _basic_types:
```

### Comparing `aiobtclientrpc-4.0.0/aiobtclientrpc.egg-info/PKG-INFO` & `aiobtclientrpc-5.0.0/aiobtclientrpc.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: aiobtclientrpc
-Version: 4.0.0
+Version: 5.0.0
 Summary: Asynchronous low-level communication with BitTorrent clients
 Home-page: https://codeberg.org/plotski/aiobtclientrpc
 Author: plotski
 Author-email: plotski@example.org
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ``aiobtclientrpc`` provides low-level access to the RPC protocols of BitTorrent
 clients. It is supposed to be the basis for a high-level library. If you want to
```

### Comparing `aiobtclientrpc-4.0.0/aiobtclientrpc.egg-info/SOURCES.txt` & `aiobtclientrpc-5.0.0/aiobtclientrpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiobtclientrpc-4.0.0/setup.py` & `aiobtclientrpc-5.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     url=get_var('__homepage__'),
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
     ],
     python_requires='>=3.7',
     install_requires=[
         'async-timeout==4.*',
         'httpx==0.*,>=0.20.0',
         'httpx-socks==0.7.*',
```

### Comparing `aiobtclientrpc-4.0.0/tests/base_test.py` & `aiobtclientrpc-5.0.0/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `aiobtclientrpc-4.0.0/tests/common.py` & `aiobtclientrpc-5.0.0/tests/common.py`

 * *Files identical despite different names*

### Comparing `aiobtclientrpc-4.0.0/tests/deluge_test.py` & `aiobtclientrpc-5.0.0/tests/deluge_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,21 +139,29 @@
     argvalues=(False, True),
 )
 @pytest.mark.asyncio
 async def test_DelugeRPC_disconnect(has_client, mocker):
     rpc = _deluge.DelugeRPC()
     catch_connection_exceptions_mock = mocker.patch('aiobtclientrpc._utils.catch_connection_exceptions',
                                                     AsyncMock(return_value='catch_connection_exceptions return value'))
+    client_mock = Mock(logout=Mock(return_value='client.logout coroutine'))
+
     if has_client:
-        rpc._client = client_mock = Mock(logout=Mock(return_value='client.logout coroutine'))
+        rpc._client = client_mock
+    else:
+        assert not hasattr(rpc, '_client')
 
-        await rpc._disconnect()
+    await rpc._disconnect()
 
+    if has_client:
         assert catch_connection_exceptions_mock.call_args_list == [call('client.logout coroutine')]
         assert client_mock.logout.call_args_list == [call()]
+    else:
+        assert catch_connection_exceptions_mock.call_args_list == []
+        assert client_mock.logout.call_args_list == []
 
     assert not hasattr(rpc, '_client')
 
 
 @pytest.mark.asyncio
 async def test_DelugeRPC_call(mocker):
     rpc = _deluge.DelugeRPC()
@@ -180,19 +188,23 @@
 async def test_DelugeRPC_unsubscribe(mocker):
     client = _deluge.DelugeRPC()
     mocker.patch.object(client, 'call', AsyncMock())
     await client._unsubscribe('foo_event')
     assert client.call.call_args_list == []
 
 
-async def test_DelugeRPCClient_connection_lost():
-    client = _deluge._DelugeRPCClient(host='localhost', port=123, on_connection_lost=Mock())
+@pytest.mark.parametrize('on_connection_lost', (None, Mock()))
+async def test_DelugeRPCClient_connection_lost(on_connection_lost):
+    client = _deluge._DelugeRPCClient(host='localhost', port=123, on_connection_lost=on_connection_lost)
     client._protocol = 'foo'
     client._connection_lost()
-    assert client._on_connection_lost.call_args_list == [call()]
+    if on_connection_lost:
+        assert client._on_connection_lost.call_args_list == [call()]
+    else:
+        assert client._on_connection_lost is None
     assert client._protocol is None
 
 
 @pytest.mark.parametrize('iscoroutinefunction', (True, False))
 @pytest.mark.asyncio
 async def test_DelugeRPCClient_event_received(iscoroutinefunction, mocker):
     client = _deluge._DelugeRPCClient(host='localhost', port=123, event_handler=Mock())
@@ -465,41 +477,48 @@
     protocol.connection_made(transport)
     assert protocol._transport is transport
     if on_connection_made:
         assert protocol._on_connection_made.call_args_list == [call()]
 
 
 @pytest.mark.parametrize('on_connection_lost', (False, True))
+@pytest.mark.parametrize('has_requests', (False, True))
 @pytest.mark.parametrize(
     argnames='exception, exp_exception',
     argvalues=(
         (None, _errors.ConnectionError('Connection lost')),
         (_errors.RPCError('error message'), _errors.RPCError('error message')),
     ),
     ids=lambda v: repr(v),
 )
-def test_DelugeRPCProtocol_connection_lost(exception, exp_exception, on_connection_lost, mocker):
+def test_DelugeRPCProtocol_connection_lost(exception, exp_exception, has_requests, on_connection_lost, mocker):
     protocol = _deluge._DelugeRPCProtocol(
         on_connection_lost=Mock() if on_connection_lost else None,
     )
     mocker.patch.object(protocol, 'close')
     mocker.patch.object(protocol, '_reset_internal_state')
     _deluge._DelugeRPCRequest._next_id = 123
     finished_request = Mock(future=Mock(done=Mock(return_value=True)))
     unfinished_request = Mock(future=Mock(done=Mock(return_value=False)))
-    protocol._requests = {
-        23: finished_request,
-        24: unfinished_request
-    }
+    if has_requests:
+        protocol._requests = {
+            23: finished_request,
+            24: unfinished_request,
+        }
+    else:
+        protocol._requests = {}
 
     protocol.connection_lost(exception)
 
     assert finished_request.future.set_exception.call_args_list == []
     assert finished_request.future.set_result.call_args_list == []
-    assert unfinished_request.future.set_exception.call_args_list == [call(exp_exception)]
+    if has_requests:
+        assert unfinished_request.future.set_exception.call_args_list == [call(exp_exception)]
+    else:
+        assert unfinished_request.future.set_exception.call_args_list == []
     assert unfinished_request.future.set_result.call_args_list == []
     assert protocol._requests == {}
     assert protocol.close.call_args_list == [call()]
     assert protocol._reset_internal_state.call_args_list == [call()]
     if on_connection_lost:
         assert protocol._on_connection_lost.call_args_list == [call()]
```

### Comparing `aiobtclientrpc-4.0.0/tests/integration_tests/conftest.py` & `aiobtclientrpc-5.0.0/tests/integration_tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,71 +7,93 @@
 import pytest
 
 import aiobtclientrpc
 
 PACKAGE_NAME = 'tests.' + os.path.basename(os.path.dirname(__file__))
 
 
+def log(*args):
+    print('CONFTEST:', ' '.join(str(arg) for arg in args))
+
+
 def _get_server_modules():
     server_modules = []
     servers_path = os.path.join(os.path.dirname(__file__), 'servers')
-    print(servers_path)
+    log(servers_path)
 
     for filepath in sorted(os.listdir(servers_path)):
         filename = os.path.basename(filepath)
         if not filename.startswith('_') and filename.endswith('.py'):
             module_name = filename[:-len('.py')]
             module = importlib.import_module(f'.{module_name}', package=f'{PACKAGE_NAME}.servers')
             server_modules.append(module)
     return server_modules
 
 
 @pytest.fixture(
-    params=_get_server_modules(), ids=lambda module: module.name,
+    params=_get_server_modules(),
+    scope='session',
+    ids=lambda module: module.name,
 )
-def api(request, tmp_path):
+def _server_info(request, tmp_path_factory):
     module = request.param
+    tmp_path = tmp_path_factory.mktemp('X')
     info = module.run(tmp_path)
 
+    def server_info():
+        return info
+
     try:
         run_server(info, tmp_path)
-        client = aiobtclientrpc.client(info['client_name'], url=info['server_url'])
-        api_module = importlib.import_module('.' + info['client_name'], package=f'{PACKAGE_NAME}.apis')
-        api = api_module.API(client)
-        yield api
+        yield server_info
     finally:
         kill_server(info['server_name'])
 
 
+@pytest.fixture
+async def api(_server_info):
+    info = _server_info()
+
+    client = aiobtclientrpc.client(info['client_name'], url=info['server_url'])
+    api_module = importlib.import_module('.' + info['client_name'], package=f'{PACKAGE_NAME}.apis')
+    api = api_module.API(client)
+    await api.reset()
+    yield api
+
+
 _running_servers = {}
 
 def run_server(info, tmp_path):
+    log('Running server:', info['server_name'], info['server_url'])
+
     try:
         info['proc'] = subprocess.Popen(
             shlex.split(info['server_start_cmd']),
             shell=False,
         )
     except FileNotFoundError:
         pytest.skip(info['server_name'] + ' is not installed')
 
     _running_servers[info['server_name']] = info
 
     # Check if server_start_cmd failed, e.g. due to invalid arguments
     if info['proc'].poll() is None:
-        print('Started', info['server_name'], 'successfully')
+        log('Server is now running:', info['server_name'])
         # Wait for RPC interface to come up
         time.sleep(3)
 
     # Process should still be running (poll() returns None); otherwise report
     # stdout/stderr
     if info['proc'].poll() is not None:
         raise RuntimeError(f'Failed to run {info["server_start_cmd"]}')
 
 
 def kill_server(name):
+    log('Killing server:', name)
+
     info = _running_servers.get(name, {})
     if info.get('proc', None):
         server_stop_cmd = info.get('server_stop_cmd')
         if server_stop_cmd:
             subprocess.run(shlex.split(server_stop_cmd), shell=False)
         else:
             info['proc'].terminate()
```

### Comparing `aiobtclientrpc-4.0.0/tests/integration_tests/integration_test.py` & `aiobtclientrpc-5.0.0/tests/integration_tests/integration_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,35 +44,38 @@
 async def test_api_as_context_manager(api, tmp_path):
     for _ in range(3):
         async with api.client:
             await api.perform_simple_request()
 
 
 @pytest.mark.parametrize('paused', (True, False), ids=lambda paused: 'paused' if paused else 'started')
-@pytest.mark.parametrize('as_file', (True, False), ids=lambda as_file: 'as_file' if as_file else 'as_bytes')
 @pytest.mark.asyncio
-async def test_add_torrents(as_file, paused, api, tmp_path):
-    infohashes = sorted([
-        '4435ef55af79b350e7b85d5b330a7886a61e3bdf',
-        'd5a34e9eb4709e265f0f03a1c8ab60890dcb94a9',
-    ])
+async def test_add_and_remove_torrents(paused, api, tmp_path):
+    torrents = common.get_test_torrents()
+    infohashes = sorted(torrents.values())
 
     try:
-        return_value = await api.add_torrent_files(
-            torrent_filepaths=(
-                common.get_torrent_filepath(infohashes[0]),
-                common.get_torrent_filepath(infohashes[1]),
-            ),
-            as_file=as_file,
+        # Add torrents
+        added_infohashes = await api.add_torrents(
+            torrent_filepaths=list(torrents),
             paused=paused,
         )
-        assert return_value == infohashes
+        assert added_infohashes == infohashes
+
+        # Confirm the torrents are added
         torrent_list = await api.get_torrent_list()
         assert torrent_list == infohashes
 
+        # Remove torrents
+        await api.remove_torrents(infohashes)
+
+        # Confirm the torrents are removed
+        torrent_list = await api.get_torrent_list()
+        assert torrent_list == []
+
     finally:
         await api.client.disconnect()
 
 
 @pytest.mark.skipif(sys.version_info < (3, 8), reason='Avoid BrokenResourceError on Python 3.7')
 @pytest.mark.parametrize(
     argnames='start_proxy',
@@ -162,69 +165,66 @@
                 await api.perform_simple_request()
     finally:
         await api.client.disconnect()
 
 
 @pytest.mark.asyncio
 async def test_event_subscriptions_survive_reconnecting(api, tmp_path):
-    infohashes = sorted([
-        '4435ef55af79b350e7b85d5b330a7886a61e3bdf',
-        'd5a34e9eb4709e265f0f03a1c8ab60890dcb94a9',
-    ])
+    torrents = common.get_test_torrents(map='infohash:filepath')
+    infohashes = sorted(torrents.keys())
 
     torrent_added_handler = Mock()
 
     async with api.client:
         try:
             await api.on_torrent_added(torrent_added_handler)
         except NotImplementedError as e:
             assert str(e) == f'Events are not supported for {api.client.label}'
             pytest.skip(str(e))
         else:
-            await api.add_torrent_files(
-                torrent_filepaths=[common.get_torrent_filepath(infohashes[0])],
+            await api.add_torrents(
+                torrent_filepaths=[torrents[infohashes[0]]],
             )
             assert torrent_added_handler.call_args_list == [
                 call(infohashes[0]),
             ]
 
     # Re-connect and check if torrent_added_handler() is still called
     async with api.client:
-        await api.add_torrent_files(
-            torrent_filepaths=[common.get_torrent_filepath(infohashes[1])],
+        await api.add_torrents(
+            torrent_filepaths=[torrents[infohashes[1]]],
         )
         assert torrent_added_handler.call_args_list == [
             call(infohashes[0]),
             call(infohashes[1]),
         ]
 
 
 @pytest.mark.asyncio
 async def test_waiting_for_event(api, tmp_path):
-    infohashes = sorted([
-        '4435ef55af79b350e7b85d5b330a7886a61e3bdf',
-        'd5a34e9eb4709e265f0f03a1c8ab60890dcb94a9',
-    ])
+    torrents = common.get_test_torrents(map='infohash:filepath')
+    infohashes = sorted(torrents.keys())
 
     async with api.client:
         coros = [
             api.wait_for_torrent_added(),
-            api.add_torrent_files(
+            api.add_torrents(
                 torrent_filepaths=[
-                    common.get_torrent_filepath(infohash)
+                    torrents[infohash]
                     for infohash in infohashes
                 ],
             ),
         ]
 
         return_values = await asyncio.gather(*coros, return_exceptions=True)
         assert len(return_values) == 2
         wait_for_torrent_added_return_value = return_values[0]
-        add_torrent_files_return_value = return_values[1]
+        add_torrents_return_value = return_values[1]
 
         if wait_for_torrent_added_return_value is not None:
             assert type(wait_for_torrent_added_return_value) is NotImplementedError
-            assert str(wait_for_torrent_added_return_value) == f'Events are not supported for {api.client.label}'
-            pytest.skip(str(wait_for_torrent_added_return_value))
+            msg = f'Events are not supported for {api.client.label}'
+            assert msg == str(wait_for_torrent_added_return_value)
+            pytest.skip(msg)
 
         else:
-            assert add_torrent_files_return_value == infohashes
+            assert add_torrents_return_value == infohashes
```

### Comparing `aiobtclientrpc-4.0.0/tests/integration_tests/proxyserver.py` & `aiobtclientrpc-5.0.0/tests/integration_tests/proxyserver.py`

 * *Files identical despite different names*

### Comparing `aiobtclientrpc-4.0.0/tests/qbittorrent_test.py` & `aiobtclientrpc-5.0.0/tests/qbittorrent_test.py`

 * *Files identical despite different names*

### Comparing `aiobtclientrpc-4.0.0/tests/rtorrent_test.py` & `aiobtclientrpc-5.0.0/tests/rtorrent_test.py`

 * *Files identical despite different names*

### Comparing `aiobtclientrpc-4.0.0/tests/transmission_test.py` & `aiobtclientrpc-5.0.0/tests/transmission_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,23 +208,31 @@
     argvalues=(
         (
             'some_method',
             None,
             {'foo': 'bar'},
             {'foo': 'bar'},
             Mock(json=Mock(side_effect=ValueError()), text='The Error.'),
-            _errors.RPCError('Unexpected response: The Error.'),
+            _errors.RPCError('Unexpected response: The Error.', info=None),
         ),
         (
             'some_method',
             None,
             {'foo': 'bar'},
             {'foo': 'bar'},
             Mock(json=Mock(return_value={'result': 'no success'})),
+            _errors.RPCError('No success', info=None),
+        ),
+        (
+            'some_method',
             None,
+            {'foo': 'bar'},
+            {'foo': 'bar'},
+            Mock(json=Mock(return_value={'result': 'no success', 'arguments': 'more information'})),
+            _errors.RPCError('No success', info='more information'),
         ),
         (
             'some_method',
             None,
             {'foo': 'bar'},
             {'foo': 'bar'},
             Mock(json=Mock(return_value={'result': 'success'})),
@@ -243,14 +251,17 @@
 )
 @pytest.mark.asyncio
 async def test_call(method, args, kwargs, exp_params, response, exp_exception, mocker):
     rpc = _transmission.TransmissionRPC()
     mocker.patch.object(rpc, '_request', AsyncMock(return_value=response))
 
     if exp_exception:
-        with pytest.raises(type(exp_exception), match=rf'^{re.escape(str(exp_exception))}$'):
+        with pytest.raises(type(exp_exception), match=rf'^{re.escape(str(exp_exception))}$') as info:
             await rpc._call(method, args=args, **kwargs)
+        exception = info.value
+        assert exception.info == exp_exception.info
+
     else:
         return_value = await rpc._call(method, args=args, **kwargs)
         assert return_value is response.json.return_value
 
     assert rpc._request.call_args_list == [call(method, **exp_params)]
```

### Comparing `aiobtclientrpc-4.0.0/tests/utils_test.py` & `aiobtclientrpc-5.0.0/tests/utils_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,14 +158,17 @@
          {'scheme': 'file', 'host': None, 'port': None, 'path': 'foo:bar@localhost', 'username': None, 'password': None}),
         ('file://localhost:123',
          {'scheme': 'file', 'host': None, 'port': None, 'path': 'localhost:123', 'username': None, 'password': None}),
         ('file://localhost:arf',
          {'scheme': 'file', 'host': None, 'port': None, 'path': 'localhost:arf', 'username': None, 'password': None}),
         ('/absolute/path',
          {'scheme': 'file', 'host': None, 'port': None, 'path': '/absolute/path', 'username': None, 'password': None}),
+
+        # Unsupported type
+        (['not', 'an', 'url'], TypeError("Unsupported type: list: ['not', 'an', 'url']")),
     ),
     ids=lambda v: str(v),
 )
 def test_URL_parsing(url, exp_parts_or_exception):
     def make_url(url):
         if url is not None:
             return _utils.URL(url)
```

