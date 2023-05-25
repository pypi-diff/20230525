# Comparing `tmp/aiobtclientapi-1.0.3.tar.gz` & `tmp/aiobtclientapi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiobtclientapi-1.0.3.tar", last modified: Tue Apr  4 13:37:27 2023, max compression
+gzip compressed data, was "aiobtclientapi-1.1.0.tar", last modified: Thu May 25 10:32:09 2023, max compression
```

## Comparing `aiobtclientapi-1.0.3.tar` & `aiobtclientapi-1.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-04 13:37:27.311406 aiobtclientapi-1.0.3/
--rw-------   0 ich       (1000) ich       (1000)    35149 2022-07-05 13:26:49.000000 aiobtclientapi-1.0.3/LICENSE
--rw-------   0 ich       (1000) ich       (1000)     1198 2023-04-04 13:37:27.311406 aiobtclientapi-1.0.3/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)      592 2022-08-27 13:56:53.000000 aiobtclientapi-1.0.3/README.rst
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-04 13:37:27.307407 aiobtclientapi-1.0.3/aiobtclientapi/
--rw-------   0 ich       (1000) ich       (1000)     1667 2023-04-04 13:36:57.000000 aiobtclientapi-1.0.3/aiobtclientapi/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     3976 2022-08-05 10:25:54.000000 aiobtclientapi-1.0.3/aiobtclientapi/cli.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-04 13:37:27.307407 aiobtclientapi-1.0.3/aiobtclientapi/clients/
--rw-------   0 ich       (1000) ich       (1000)      208 2022-08-04 15:44:22.000000 aiobtclientapi-1.0.3/aiobtclientapi/clients/__init__.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-04 13:37:27.307407 aiobtclientapi-1.0.3/aiobtclientapi/clients/base/
--rw-------   0 ich       (1000) ich       (1000)       25 2022-06-16 09:50:40.000000 aiobtclientapi-1.0.3/aiobtclientapi/clients/base/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    18036 2022-08-22 10:11:07.000000 aiobtclientapi-1.0.3/aiobtclientapi/clients/base/api.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-04 13:37:27.307407 aiobtclientapi-1.0.3/aiobtclientapi/clients/deluge/
--rw-------   0 ich       (1000) ich       (1000)       27 2022-07-26 09:47:43.000000 aiobtclientapi-1.0.3/aiobtclientapi/clients/deluge/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     5600 2022-08-10 10:57:18.000000 aiobtclientapi-1.0.3/aiobtclientapi/clients/deluge/api.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-04 13:37:27.307407 aiobtclientapi-1.0.3/aiobtclientapi/clients/qbittorrent/
--rw-------   0 ich       (1000) ich       (1000)       32 2022-07-27 09:37:07.000000 aiobtclientapi-1.0.3/aiobtclientapi/clients/qbittorrent/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     5547 2022-08-10 10:57:20.000000 aiobtclientapi-1.0.3/aiobtclientapi/clients/qbittorrent/api.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-04 13:37:27.307407 aiobtclientapi-1.0.3/aiobtclientapi/clients/rtorrent/
--rw-------   0 ich       (1000) ich       (1000)       29 2022-07-27 15:40:51.000000 aiobtclientapi-1.0.3/aiobtclientapi/clients/rtorrent/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     6314 2023-03-15 11:52:03.000000 aiobtclientapi-1.0.3/aiobtclientapi/clients/rtorrent/api.py
--rw-------   0 ich       (1000) ich       (1000)     1558 2022-08-10 11:04:56.000000 aiobtclientapi-1.0.3/aiobtclientapi/clients/rtorrent/utils.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-04 13:37:27.307407 aiobtclientapi-1.0.3/aiobtclientapi/clients/transmission/
--rw-------   0 ich       (1000) ich       (1000)       33 2022-07-30 14:17:58.000000 aiobtclientapi-1.0.3/aiobtclientapi/clients/transmission/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     5761 2023-04-04 10:51:21.000000 aiobtclientapi-1.0.3/aiobtclientapi/clients/transmission/api.py
--rw-------   0 ich       (1000) ich       (1000)      418 2022-07-30 14:17:58.000000 aiobtclientapi-1.0.3/aiobtclientapi/clients/transmission/enums.py
--rw-------   0 ich       (1000) ich       (1000)       69 2022-07-05 13:26:49.000000 aiobtclientapi-1.0.3/aiobtclientapi/constants.py
--rw-------   0 ich       (1000) ich       (1000)     5620 2022-08-04 15:44:58.000000 aiobtclientapi-1.0.3/aiobtclientapi/errors.py
--rw-------   0 ich       (1000) ich       (1000)     7696 2022-08-05 11:03:47.000000 aiobtclientapi-1.0.3/aiobtclientapi/response.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-04 13:37:27.307407 aiobtclientapi-1.0.3/aiobtclientapi/utils/
--rw-------   0 ich       (1000) ich       (1000)     5833 2022-08-10 10:23:06.000000 aiobtclientapi-1.0.3/aiobtclientapi/utils/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     6674 2022-08-01 15:15:03.000000 aiobtclientapi-1.0.3/aiobtclientapi/utils/monitor.py
--rw-------   0 ich       (1000) ich       (1000)     2257 2022-07-20 10:23:53.000000 aiobtclientapi-1.0.3/aiobtclientapi/utils/torrent.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-04 13:37:27.307407 aiobtclientapi-1.0.3/aiobtclientapi.egg-info/
--rw-------   0 ich       (1000) ich       (1000)     1198 2023-04-04 13:37:27.000000 aiobtclientapi-1.0.3/aiobtclientapi.egg-info/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     1021 2023-04-04 13:37:27.000000 aiobtclientapi-1.0.3/aiobtclientapi.egg-info/SOURCES.txt
--rw-------   0 ich       (1000) ich       (1000)        1 2023-04-04 13:37:27.000000 aiobtclientapi-1.0.3/aiobtclientapi.egg-info/dependency_links.txt
--rw-------   0 ich       (1000) ich       (1000)       57 2023-04-04 13:37:27.000000 aiobtclientapi-1.0.3/aiobtclientapi.egg-info/entry_points.txt
--rw-------   0 ich       (1000) ich       (1000)       60 2023-04-04 13:37:27.000000 aiobtclientapi-1.0.3/aiobtclientapi.egg-info/requires.txt
--rw-------   0 ich       (1000) ich       (1000)       15 2023-04-04 13:37:27.000000 aiobtclientapi-1.0.3/aiobtclientapi.egg-info/top_level.txt
--rw-------   0 ich       (1000) ich       (1000)       38 2023-04-04 13:37:27.311406 aiobtclientapi-1.0.3/setup.cfg
--rw-------   0 ich       (1000) ich       (1000)     1384 2023-04-03 17:37:21.000000 aiobtclientapi-1.0.3/setup.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.984227 aiobtclientapi-1.1.0/
+-rw-------   0 ich       (1000) ich       (1000)    35149 2022-07-05 13:26:49.000000 aiobtclientapi-1.1.0/LICENSE
+-rw-------   0 ich       (1000) ich       (1000)     1198 2023-05-25 10:32:09.980227 aiobtclientapi-1.1.0/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)      592 2022-08-27 13:56:53.000000 aiobtclientapi-1.1.0/README.rst
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.976227 aiobtclientapi-1.1.0/aiobtclientapi/
+-rw-------   0 ich       (1000) ich       (1000)     1930 2023-05-25 10:12:34.000000 aiobtclientapi-1.1.0/aiobtclientapi/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     3976 2023-05-14 09:04:17.000000 aiobtclientapi-1.1.0/aiobtclientapi/cli.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.976227 aiobtclientapi-1.1.0/aiobtclientapi/clients/
+-rw-------   0 ich       (1000) ich       (1000)      208 2022-08-04 15:44:22.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/__init__.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.980227 aiobtclientapi-1.1.0/aiobtclientapi/clients/base/
+-rw-------   0 ich       (1000) ich       (1000)       25 2022-06-16 09:50:40.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/base/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    18437 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/base/api.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.980227 aiobtclientapi-1.1.0/aiobtclientapi/clients/deluge/
+-rw-------   0 ich       (1000) ich       (1000)       27 2022-07-26 09:47:43.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/deluge/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     6016 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/deluge/api.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.980227 aiobtclientapi-1.1.0/aiobtclientapi/clients/qbittorrent/
+-rw-------   0 ich       (1000) ich       (1000)       32 2022-07-27 09:37:07.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/qbittorrent/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     5897 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/qbittorrent/api.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.980227 aiobtclientapi-1.1.0/aiobtclientapi/clients/rtorrent/
+-rw-------   0 ich       (1000) ich       (1000)       29 2022-07-27 15:40:51.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/rtorrent/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     6595 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/rtorrent/api.py
+-rw-------   0 ich       (1000) ich       (1000)     1558 2023-05-18 09:45:43.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/rtorrent/utils.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.980227 aiobtclientapi-1.1.0/aiobtclientapi/clients/transmission/
+-rw-------   0 ich       (1000) ich       (1000)       33 2022-07-30 14:17:58.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/transmission/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     6480 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/transmission/api.py
+-rw-------   0 ich       (1000) ich       (1000)      418 2022-07-30 14:17:58.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/transmission/enums.py
+-rw-------   0 ich       (1000) ich       (1000)       69 2022-07-05 13:26:49.000000 aiobtclientapi-1.1.0/aiobtclientapi/constants.py
+-rw-------   0 ich       (1000) ich       (1000)     5466 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.0/aiobtclientapi/errors.py
+-rw-------   0 ich       (1000) ich       (1000)     7696 2022-08-05 11:03:47.000000 aiobtclientapi-1.1.0/aiobtclientapi/response.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.980227 aiobtclientapi-1.1.0/aiobtclientapi/utils/
+-rw-------   0 ich       (1000) ich       (1000)     6024 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.0/aiobtclientapi/utils/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     6674 2022-08-01 15:15:03.000000 aiobtclientapi-1.1.0/aiobtclientapi/utils/monitor.py
+-rw-------   0 ich       (1000) ich       (1000)     2634 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.0/aiobtclientapi/utils/torrent.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.976227 aiobtclientapi-1.1.0/aiobtclientapi.egg-info/
+-rw-------   0 ich       (1000) ich       (1000)     1198 2023-05-25 10:32:09.000000 aiobtclientapi-1.1.0/aiobtclientapi.egg-info/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     1021 2023-05-25 10:32:09.000000 aiobtclientapi-1.1.0/aiobtclientapi.egg-info/SOURCES.txt
+-rw-------   0 ich       (1000) ich       (1000)        1 2023-05-25 10:32:09.000000 aiobtclientapi-1.1.0/aiobtclientapi.egg-info/dependency_links.txt
+-rw-------   0 ich       (1000) ich       (1000)       57 2023-05-25 10:32:09.000000 aiobtclientapi-1.1.0/aiobtclientapi.egg-info/entry_points.txt
+-rw-------   0 ich       (1000) ich       (1000)       60 2023-05-25 10:32:09.000000 aiobtclientapi-1.1.0/aiobtclientapi.egg-info/requires.txt
+-rw-------   0 ich       (1000) ich       (1000)       15 2023-05-25 10:32:09.000000 aiobtclientapi-1.1.0/aiobtclientapi.egg-info/top_level.txt
+-rw-------   0 ich       (1000) ich       (1000)       38 2023-05-25 10:32:09.984227 aiobtclientapi-1.1.0/setup.cfg
+-rw-------   0 ich       (1000) ich       (1000)     1384 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.0/setup.py
```

### Comparing `aiobtclientapi-1.0.3/LICENSE` & `aiobtclientapi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.0.3/PKG-INFO` & `aiobtclientapi-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiobtclientapi
-Version: 1.0.3
+Version: 1.1.0
 Summary: Asynchronous high-level communication with BitTorrent clients
 Home-page: https://codeberg.org/plotski/aiobtclientapi
 Author: plotski
 Author-email: plotski@example.org
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `aiobtclientapi-1.0.3/README.rst` & `aiobtclientapi-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.0.3/aiobtclientapi/__init__.py` & `aiobtclientapi-1.1.0/aiobtclientapi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Asynchronous high-level communication with BitTorrent clients
 """
 
 __project_name__ = 'aiobtclientapi'
 __description__ = 'Asynchronous high-level communication with BitTorrent clients'
 __homepage__ = 'https://codeberg.org/plotski/aiobtclientapi'
-__version__ = '1.0.3'
+__version__ = '1.1.0'
 __author__ = 'plotski'
 __author_email__ = 'plotski@example.org'
 
 # isort:skip_file
 
 from .clients import APIBase
 from .clients import DelugeAPI, QbittorrentAPI, RtorrentAPI, TransmissionAPI
@@ -46,21 +46,32 @@
 
     The name of a client is specified by the `name` attribute of the
     :class:`~.APIBase` subclass.
     """
     return tuple(cls.name for cls in api_classes())
 
 
-def api(name, **kwargs):
+def api_class(name):
     """
-    Instantiate :class:`~.APIBase` subclass
+    Get :class:`~.APIBase` subclass from client name
 
     :param name: :attr:`~.APIBase.name` of the client to instantiate
-    :param kwargs: Arguments for the :attr:`~.APIBase` subclass
 
     :raise ValueError: if `name` is not a known client name
     """
     for cls in api_classes():
         if cls.name == name:
-            return cls(**kwargs)
-
+            return cls
     raise ValueError(f'Unknown client: {name!r}')
+
+
+def api(name, **kwargs):
+    """
+    Instantiate :class:`~.APIBase` subclass
+
+    :param name: :attr:`~.APIBase.name` of the client to instantiate
+    :param kwargs: Arguments for the :attr:`~.APIBase` subclass
+
+    :raise ValueError: if `name` is not a known client name
+    """
+    cls = api_class(name)
+    return cls(**kwargs)
```

### Comparing `aiobtclientapi-1.0.3/aiobtclientapi/cli.py` & `aiobtclientapi-1.1.0/aiobtclientapi/cli.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.0.3/aiobtclientapi/clients/base/api.py` & `aiobtclientapi-1.1.0/aiobtclientapi/clients/base/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Base class for client APIs
 """
 
 import abc
 import asyncio
 import collections
+import os
 
 import aiobtclientrpc
 
 from ... import errors, utils
 from ...response import Response
 
 import logging  # isort:skip
@@ -52,22 +53,22 @@
         """
         Run coroutine in background
 
         :param coro: Coroutine or any other argument for :func:`asyncio.create_task`
         :param name: Identifier to help with debugging
         :param done_callback: Synchronous callable that is called with the
             return value of `coro`
-        :param detach: Whether to wait this task to finish
+        :param detach: Whether to always wait for `coro` to return
 
             If this is set to a truthy value, `coro` is cancelled by
             :meth:`wait_for_background_tasks` and
             :class:`~.asyncio.CancelledError` is ignored.
 
             If this is set to a falsy value, :meth:`wait_for_background_tasks`
-            blocks until `coro` has finished.
+            blocks until `coro` returns.
 
         :return: :class:`asyncio.Task` instance
         """
         # Store references to background tasks so they don't get garbage
         # collected.
         # https://docs.python.org/3/library/asyncio-task.html#asyncio.create_task
         # Also remember if we care about the task to finish or not.
@@ -131,18 +132,18 @@
             except asyncio.CancelledError:
                 if not taskinfo.detached:
                     raise
                 else:
                     _log.debug('%s: Ignoring cancelled background task: %r', self.label, taskinfo.task.get_name())
 
     monitor_interval = 0.1
-    """Seconds between requests when waiting for some change"""
+    """Seconds between requests when waiting for an RPC request to take effect"""
 
     monitor_timeout = 3
-    """Maximum number of seconds before waiting for something fails"""
+    """Maximum number of seconds before waiting for an RPC response fails"""
 
     common_rpc_error_map = {}
     """
     Mapping of regular expressions to exceptions for all :meth:`call` calls
 
     See :meth:`aiobtclientrpc.RPCError.translate`.
     """
@@ -199,14 +200,15 @@
         except aiobtclientrpc.TimeoutError as e:
             raise errors.TimeoutError(f'{e}: {self.url}')
         except aiobtclientrpc.ConnectionError as e:
             raise errors.ConnectionError(f'{e}: {self.url}')
 
     @staticmethod
     def _normalize_infohash(infohash):
+        # Concrete clients may need special infohash values (e.g. all upper case)
         return utils.Infohash(infohash)
 
     async def get_infohashes(self):
         """
         Return sequence of all known infohashes
 
         :raise ConnectionError: if the connection can't be established
@@ -236,14 +238,19 @@
     async def add(self, *torrents, location=None, stopped=False, verify=True):
         """
         Add torrents to client
 
         :param torrents: Paths or URLs to torrent files, ``magnet:`` URIs or
             infohashes
         :param str location: Download directory or `None` to use the default
+
+            This should be an absolute path. If it isn't, it is made absolute
+            based on the current working directory, which may be surprising or
+            even non-sensical if the client is running in a different
+            environment.
         :param bool stopped: Whether the torrent is active right away
         :param bool verify: Whether any existing files from the torrent are
             hashed by the client to make sure they are not corrupt
 
         :return: :class:`~.Response` instance with these custom attributes:
 
             `added`
@@ -251,15 +258,15 @@
 
             `already_added`
                 Infohashes of torrents that were already added
         """
         return await Response.from_call(
             self._add_torrents(
                 torrents=torrents,
-                location=location,
+                location=str(os.path.abspath(location)) if location else None,
                 stopped=stopped,
                 verify=verify,
             ),
             attributes={
                 'added': [],
                 'already_added': [],
             },
@@ -421,14 +428,15 @@
                 ).return_value_equals(True)
 
             except errors.TimeoutError:
                 # Verifying may never start because all files are missing or
                 # because the torrent is very small and verification was
                 # finished before Monitor's first call.
                 _log.debug('Verification finished immediately: %r', infohash)
+
             else:
                 yield ('verifying', infohash)
 
     async def verify_wait(self, *infohashes, interval=(0.3, 3)):
         """
         Asynchronous generator that yields ``(infohash, progress)`` tuples
 
@@ -450,27 +458,27 @@
             interval_min = interval_max = interval
         elif isinstance(interval, tuple) and len(interval) == 2:
             interval_min, interval_max = interval
         else:
             raise TypeError(f'Invalid interval: {interval!r}')
 
         waiters = [
-            self._verify_wait_torrent(
+            self._verify_wait(
                 self._normalize_infohash(infohash),
                 interval_min,
                 interval_max,
             )
             for infohash in infohashes
         ]
 
         async for coro in utils.merge_async_generators(*waiters):
             infohash, progress_or_exception = await coro
             yield (infohash, progress_or_exception)
 
-    async def _verify_wait_torrent(self, infohash, interval_min, interval_max):
+    async def _verify_wait(self, infohash, interval_min, interval_max):
         assert isinstance(infohash, utils.Infohash)
 
         interval = utils.DynamicInterval(
             name=infohash,
             min=interval_min,
             max=interval_max,
             progress_getter=utils.partial(self._get_verifying_progress, infohash),
```

### Comparing `aiobtclientapi-1.0.3/aiobtclientapi/clients/deluge/api.py` & `aiobtclientapi-1.1.0/aiobtclientapi/clients/deluge/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,85 +28,92 @@
         return await self.call('core.get_session_state')
 
     def _normalize_infohash(self, infohash):
         # Deluge doesn't seem to understand uppercase infohashes (wtf!)
         return super()._normalize_infohash(infohash.lower())
 
     async def _get_torrent_fields(self, infohash, *fields):
-        # Deluge returns {} if:
-        #   1. No torrent with `infohash` exists
-        #   2. None of the `fields` are valid
-
-        # Validate `infohash`
-        infohashes = await self.get_infohashes()
-        if infohash not in infohashes:
-            raise errors.NoSuchTorrentError(infohash)
-
         response = await self.call('core.get_torrent_status', infohash, keys=fields)
+        if response:
+            # Return only requested fields
+            try:
+                return {f: response[f] for f in fields}
+            except KeyError as e:
+                field = e.args[0]
+                raise errors.ValueError(f'Unknown field: {field!r}')
 
-        # Only return requested fields
-        try:
-            return {f: response[f] for f in fields}
-        except KeyError as e:
-            field = e.args[0]
-            raise errors.ValueError(f'Unknown field: {field!r}')
-
-    async def _add_torrents(self, *, torrents, location, stopped, verify):
-        request_args = {
-            'add_paused': bool(stopped),
-            'seed_mode': not bool(verify),
-        }
-        if location:
-            request_args['download_location'] = str(location)
-
-        async for result in super()._add_torrents(torrents, **request_args):
-            yield result
+        else:
+            # Deluge returns an empty `dict` if:
+            #   1. No torrent with `infohash` exists
+            #   2. None of the `fields` are valid
+            infohashes = await self.get_infohashes()
+            if infohash not in infohashes:
+                raise errors.NoSuchTorrentError(infohash)
+            else:
+                raise RuntimeError(f'Unexpected response: {response!r}')
 
-    async def _add_torrent(self, torrent, **request_args):
-        kwargs = {'options': request_args}
+    async def _make_add_torrent_args(self, *, torrent, location, stopped, verify):
+        rpc_args = {
+            'options': utils.without_None_values({
+                'add_paused': bool(stopped),
+                'seed_mode': not bool(verify),
+                'download_location': location,
+            }),
+        }
 
         if utils.is_magnet(torrent):
             rpc_function = 'core.add_torrent_magnet'
-            kwargs['uri'] = str(torrent)
+            rpc_args['uri'] = str(torrent)
 
         elif utils.is_infohash(torrent):
             rpc_function = 'core.add_torrent_magnet'
-            kwargs['uri'] = f'magnet:?xt=urn:btih:{torrent}'
+            rpc_args['uri'] = f'magnet:?xt=urn:btih:{torrent}'
 
         else:
             if utils.is_url(torrent):
                 torrent_bytes = await utils.torrent.download_bytes(torrent)
             else:
                 # Assume `torrent` is local file
                 torrent_bytes = utils.torrent.read_bytes(torrent)
 
-            # Assume local torrent file
-            kwargs['filedump'] = str(
+            rpc_args['filedump'] = str(
                 base64.b64encode(torrent_bytes),
                 encoding='ascii',
             )
-            kwargs['filename'] = os.path.basename(torrent)
+            rpc_args['filename'] = os.path.basename(torrent)
             rpc_function = 'core.add_torrent_file'
 
-        # Add torrent
+        return rpc_function, rpc_args
+
+    async def _add_torrent(self, torrent, *, location, stopped, verify):
+        rpc_function, rpc_args = await self._make_add_torrent_args(
+            torrent=torrent,
+            location=location,
+            stopped=stopped,
+            verify=verify,
+        )
+
         try:
-            infohash = await self.call(rpc_function, **kwargs)
+            infohash = await self.call(rpc_function, **rpc_args)
             yield ('added', infohash)
 
         except aiobtclientrpc.RPCError as e:
             dupe_regex = re.compile(r'Torrent already (?:in session|being added) \(([0-9a-zA-Z]+)\)')
             match = dupe_regex.search(str(e))
             if match:
                 infohash = match.group(1)
                 yield ('already_added', infohash)
                 yield errors.TorrentAlreadyAdded(infohash, torrent)
             else:
                 raise e.translate({
+                    # Invalid torrent
                     r'decoding filedump failed': errors.InvalidTorrentError(torrent),
+                    # Invalid magnet URI
                     r'invalid magnet info': errors.InvalidTorrentError(torrent),
+                    r'non-hexadecimal number found': errors.InvalidTorrentError(torrent),
                 })
 
     async def _start_torrent(self, infohash):
         # Check current state
         state = await self._get_torrent_field(infohash, 'state')
         if state == 'Error':
             yield ('errors', 'Cannot start torrent in error state')
```

### Comparing `aiobtclientapi-1.0.3/aiobtclientapi/clients/qbittorrent/api.py` & `aiobtclientapi-1.1.0/aiobtclientapi/clients/qbittorrent/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,89 +19,98 @@
     """
 
     async def _get_infohashes(self):
         torrents = await self.call('torrents/info')
         return (t['hash'] for t in torrents)
 
     async def _get_torrent_fields(self, infohash, *fields):
-        # qBittorrent returns all torrents if it can't find `infohash`. To
-        # mitigate this, we must first check if infohash exists.
-        known_infohashes = await self.get_infohashes()
-        if infohash not in known_infohashes:
-            raise errors.NoSuchTorrentError(infohash)
+        torrents = await self.call('torrents/info', hashes=[infohash])
+        if torrents and len(torrents) == 1:
+            torrent = torrents[0]
+            # Only return wanted information
+            try:
+                return {field: torrent[field] for field in fields}
+            except KeyError as e:
+                field = e.args[0]
+                raise errors.ValueError(f'Unknown field: {field!r}')
 
         else:
-            torrents = await self.call('torrents/info', hashes=[infohash])
-            if len(torrents) == 1:
-                torrent = torrents[0]
-                # Only return wanted information
-                try:
-                    return {field: torrent[field] for field in fields}
-                except KeyError as e:
-                    field = e.args[0]
-                    raise errors.ValueError(f'Unknown field: {field!r}')
-
-            raise RuntimeError(f'Unexpected response: {torrents!r}')
+            # qBittorrent returns all torrents if it can't find `infohash`
+            known_infohashes = await self.get_infohashes()
+            if infohash not in known_infohashes:
+                raise errors.NoSuchTorrentError(infohash)
+            else:
+                raise RuntimeError(f'Unexpected response: {torrents!r}')
 
-    async def _add_torrents(self, *, torrents, location, stopped, verify):
-        request_args = {
+    async def _make_add_torrent_args(self, *, torrent, location, stopped, verify):
+        rpc_args = utils.without_None_values({
             'paused': 'true' if stopped else 'false',
             'skip_checking': 'false' if verify else 'true',
-        }
-        if location:
-            request_args['savepath'] = str(location)
-
-        async for result in super()._add_torrents(torrents, **request_args):
-            yield result
+            'savepath': location,
+        })
 
-    async def _add_torrent(self, torrent, **request_args):
         if utils.is_magnet(torrent):
-            request_args['urls'] = [str(torrent)]
-            request_files = ()
-            infohash = utils.torrent.read(torrent).infohash
+            rpc_args['urls'] = [str(torrent)]
+            infohash = utils.torrent.get_infohash(torrent)
 
         elif utils.is_infohash(torrent):
-            request_args['urls'] = [f'magnet:?xt=urn:btih:{torrent}']
-            request_files = ()
-            infohash = str(torrent)
+            rpc_args['urls'] = [f'magnet:?xt=urn:btih:{torrent}']
+            infohash = utils.torrent.get_infohash(torrent)
 
         else:
             if utils.is_url(torrent):
                 torrent_bytes = await utils.torrent.download_bytes(torrent)
             else:
                 # Assume `torrent` is local file
                 torrent_bytes = utils.torrent.read_bytes(torrent)
-
-            request_files = (
+            infohash = utils.torrent.get_infohash(torrent_bytes)
+            rpc_args['files'] = (
                 ('filename', (
                     os.path.basename(torrent),   # File name
                     torrent_bytes,               # File content
                     'application/x-bittorrent',  # MIME type
                 )),
             )
-            infohash = utils.torrent.read(torrent_bytes).infohash
 
-        # qBittorrent doesn't report pre-existing torrents, it just "Fails."
-        if infohash in await self.get_infohashes():
-            yield ('already_added', infohash)
-            yield errors.TorrentAlreadyAdded(infohash, name=torrent)
+        return rpc_args, infohash
+
+    async def _add_torrent(self, torrent, *, location, stopped, verify):
+        rpc_args, infohash = await self._make_add_torrent_args(
+            torrent=torrent,
+            location=location,
+            stopped=stopped,
+            verify=verify,
+        )
+
+        try:
+            response = await self.call('torrents/add', **rpc_args)
+
+        except aiobtclientrpc.RPCError as e:
+            raise e.translate({
+                r'not a valid torrent': errors.InvalidTorrentError(torrent),
+            })
 
         else:
-            response = await self.call('torrents/add', files=request_files, **request_args)
             if response == 'Fails.':
-                raise errors.InvalidTorrentError(torrent)
+                # qBittorrent doesn't report duplicate torrents, it just "Fails."
+                # with HTTP status "200 OK"
+                print(infohash, 'in', await self.get_infohashes())
+                if infohash in await self.get_infohashes():
+                    yield ('already_added', infohash)
+                    yield errors.TorrentAlreadyAdded(infohash, name=torrent)
+                else:
+                    raise errors.InvalidTorrentError(torrent)
 
             else:
                 # Wait for command to take effect
                 await utils.Monitor(
                     call=self.get_infohashes,
                     interval=self.monitor_interval,
                     timeout=self.monitor_timeout,
                 ).return_value_contains(infohash)
-
                 yield ('added', infohash)
 
     async def _start_torrent(self, infohash):
         # Check current state
         state = await self._get_torrent_field(infohash, 'state')
         if not state.startswith('paused'):
             yield ('already_started', infohash)
```

### Comparing `aiobtclientapi-1.0.3/aiobtclientapi/clients/rtorrent/api.py` & `aiobtclientapi-1.1.0/aiobtclientapi/clients/rtorrent/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,75 +37,80 @@
             self.multicall(
                 *((field, infohash) for field in fields),
                 as_dict=True,
             ),
             infohash=infohash,
         )
 
-    async def _add_torrents(self, *, torrents, location, stopped, verify):
-        request_args = {
-            'stopped': bool(stopped),
-            'verify': bool(verify),
-            'location': str(location) if location else None
-        }
-
-        async for result in super()._add_torrents(torrents, **request_args):
-            yield result
-
-    async def _add_torrent(self, torrent, *, location, stopped, verify):
+    async def _make_add_torrent_args(self, *, torrent, location, stopped, verify):
         if utils.is_magnet(torrent):
-            args = ['', str(torrent)]
-            infohash = utils.torrent.read(torrent).infohash
-            load_method = await self.get_supported_method('load.start_verbose')
+            rpc_method = 'load.start_verbose'
+            rpc_args = ['', str(torrent)]
+            infohash = utils.torrent.get_infohash(torrent)
 
         elif utils.is_infohash(torrent):
-            args = ['', f'magnet:?xt=urn:btih:{torrent}']
-            infohash = str(torrent)
-            load_method = await self.get_supported_method('load.start_verbose')
+            rpc_method = 'load.start_verbose'
+            rpc_args = ['', f'magnet:?xt=urn:btih:{torrent}']
+            infohash = utils.torrent.get_infohash(torrent)
 
         else:
             if utils.is_url(torrent):
                 torrent_bytes = await utils.torrent.download_bytes(torrent)
             else:
                 # Assume `torrent` is local file
                 torrent_bytes = utils.torrent.read_bytes(torrent)
 
-            load_method = await self.get_supported_method(
-                'load.raw_start_verbose',
-                'load.raw_start',
-            )
-
+            # Add fast_resume fields?
             if not verify and location:
                 torrent_bytes = rtorrent_utils.add_resume_fields(
                     utils.torrent.read(torrent_bytes),
                     location,
                 )
-            args = ['', torrent_bytes]
-            infohash = utils.torrent.read(torrent_bytes).infohash
+
+            # load.raw_start_verbose was added in 0.9.7 (?)
+            # Is 0.9.6 and earlier still popular?
+            rpc_method = await self.get_supported_method(
+                'load.raw_start_verbose',
+                'load.raw_start',
+            )
+            rpc_args = ['', torrent_bytes]
+            infohash = utils.torrent.get_infohash(torrent_bytes)
 
         if location:
-            args.append('d.directory.set="' + location.replace('"', r'\"') + '"')
+            rpc_args.append('d.directory.set="' + location.replace('"', r'\"') + '"')
+
+        return rpc_method, rpc_args, infohash
 
+    async def _add_torrent(self, torrent, *, location, stopped, verify):
+        rpc_method, rpc_args, infohash = await self._make_add_torrent_args(
+            torrent=torrent,
+            location=location,
+            stopped=stopped,
+            verify=verify,
+        )
+
+        # rtorrent silently ignores if the torrent is already added.
         if infohash in await self.get_infohashes():
             yield ('already_added', infohash)
             yield errors.TorrentAlreadyAdded(infohash, torrent)
 
         else:
-            await self.call(load_method, *args)
+            await self.call(rpc_method, *rpc_args)
 
-            # Infohash is not known if `torrent` is an URL
             # Wait for command to take effect
             await utils.Monitor(
                 call=self.get_infohashes,
                 interval=self.monitor_interval,
                 timeout=self.monitor_timeout,
             ).return_value_contains(infohash)
-
             yield ('added', infohash)
 
+            # rtorrent always verifies. If we stop the torrent immediately,
+            # it also stops verifying and we have to tell it again to
+            # verify.
             if stopped:
                 yield await self.stop(infohash)
                 if verify:
                     yield await self.verify(infohash)
 
     async def _start_torrent(self, infohash):
         # Check current state
```

### Comparing `aiobtclientapi-1.0.3/aiobtclientapi/clients/rtorrent/utils.py` & `aiobtclientapi-1.1.0/aiobtclientapi/clients/rtorrent/utils.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.0.3/aiobtclientapi/clients/transmission/api.py` & `aiobtclientapi-1.1.0/aiobtclientapi/clients/transmission/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 API for the Transmission daemon
 """
 
 import base64
-import os
 
 import aiobtclientrpc
 
 from ... import errors, utils
 from .. import base
 from . import enums
 
@@ -35,75 +34,92 @@
                 return {field: torrent[field] for field in fields}
             except KeyError as e:
                 field = e.args[0]
                 raise errors.ValueError(f'Unknown field: {field!r}')
         else:
             raise RuntimeError(f'Unexpected torrent list: {torrents!r}')
 
-    async def _add_torrents(self, *, torrents, location, stopped, verify):
-        # TODO: Make verification optional when/if it's ever supported upstream
-        if not verify:
+    async def _add_torrents(self, torrents, **kwargs):
+        # TODO: Provide a different warning for Transmission 4.*, which decides
+        # on its own if the content is verified
+        if not kwargs.get('verify', True):
             yield errors.Warning(f'Adding torrents without verification is not supported by {self.label}')
 
-        request_args = {
-            'paused': bool(stopped),
-        }
-        if location:
-            request_args['download-dir'] = str(os.path.abspath(location))
-
-        async for result in super()._add_torrents(torrents, **request_args):
+        async for result in super()._add_torrents(torrents, **kwargs):
             yield result
 
-    async def _add_torrent(self, torrent, **request_args):
+    async def _make_add_torrent_args(self, *, torrent, location, stopped, verify):
+        rpc_args = utils.without_None_values({
+            'paused': bool(stopped),
+            'download-dir': location,
+        })
+
         if utils.is_magnet(torrent):
-            request_args['filename'] = str(torrent)
+            rpc_args['filename'] = str(torrent)
 
         elif utils.is_infohash(torrent):
-            request_args['filename'] = f'magnet:?xt=urn:btih:{torrent}'
+            rpc_args['filename'] = f'magnet:?xt=urn:btih:{torrent}'
 
         else:
             if utils.is_url(torrent):
                 torrent_bytes = await utils.torrent.download_bytes(torrent)
             else:
                 # Assume `torrent` is local file
                 torrent_bytes = utils.torrent.read_bytes(torrent)
 
-            # Assume local file
-            request_args['metainfo'] = str(
+            rpc_args['metainfo'] = str(
                 base64.b64encode(torrent_bytes),
                 encoding='ascii',
             )
 
-        # Add torrent
-        result = await self.call('torrent-add', request_args)
+        return rpc_args
+
+    async def _add_torrent(self, torrent, *, location, stopped, verify):
+        rpc_args = await self._make_add_torrent_args(
+            torrent=torrent,
+            location=location,
+            stopped=stopped,
+            verify=verify,
+        )
+
+        try:
+            result = await self.call('torrent-add', rpc_args)
+
+        except aiobtclientrpc.RPCError as e:
+            # Transmission 4.* sends
+            # {"result": "duplicate torrent", "arguments": {"torrent-duplicate": ...}}
+            if e.info and 'torrent-duplicate' in e.info:
+                infohash = e.info['torrent-duplicate']['hashString']
+                yield ('already_added', infohash)
+                yield errors.TorrentAlreadyAdded(infohash, name=torrent)
 
-        # Handle error message
-        if result['result'] != 'success':
-            error = result['result']
-            if error in (
+            else:
+                raise e.translate({
                     # Transmission 3.*
-                    'invalid or corrupt torrent file',
+                    r'Invalid or corrupt': errors.InvalidTorrentError(torrent),
                     # Transmission 4.*
-                    'unrecognized info',
-            ):
-                raise errors.InvalidTorrentError(torrent)
-
-        # Get torrent hash or error message
-        arguments = result['arguments']
-        if 'torrent-added' in arguments:
-            infohash = arguments['torrent-added']['hashString']
-            yield ('added', arguments['torrent-added']['hashString'])
-
-        elif 'torrent-duplicate' in arguments:
-            infohash = arguments['torrent-duplicate']['hashString']
-            yield ('already_added', infohash)
-            yield errors.TorrentAlreadyAdded(infohash, name=torrent)
+                    r'Unrecognized info': errors.InvalidTorrentError(torrent),
+                })
 
         else:
-            raise RuntimeError(f'Unexpected response: {result}')
+            arguments = result['arguments']
+
+            # Transmission 3.* sends
+            # {"result": "success", "arguments": {"torrent-duplicate": ...}}
+            if 'torrent-duplicate' in arguments:
+                infohash = arguments['torrent-duplicate']['hashString']
+                yield ('already_added', infohash)
+                yield errors.TorrentAlreadyAdded(infohash, name=torrent)
+
+            elif 'torrent-added' in arguments:
+                infohash = arguments['torrent-added']['hashString']
+                yield ('added', arguments['torrent-added']['hashString'])
+
+            else:
+                raise RuntimeError(f'Unexpected response: {result}')
 
     async def _start_torrent(self, infohash):
         # Check current state
         status = await self._get_torrent_field(infohash, 'status')
         if status != enums.TR_STATUS.STOPPED:
             yield ('already_started', infohash)
             yield errors.TorrentAlreadyStarted(infohash)
```

### Comparing `aiobtclientapi-1.0.3/aiobtclientapi/errors.py` & `aiobtclientapi-1.1.0/aiobtclientapi/errors.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,18 +16,19 @@
         ├── InvalidTorrentError
         ├── AddTorrentError
         ├── StartTorrentError
         ├── StopTorrentError
         └── VerifyTorrentError
 
     Warning
-    ├── TorrentAlreadyAdded
-    ├── TorrentAlreadyStarted
-    ├── TorrentAlreadyStopped
-    └── TorrentAlreadyVerifying
+    └── TorrentWarning
+        ├── TorrentAlreadyAdded
+        ├── TorrentAlreadyStarted
+        ├── TorrentAlreadyStopped
+        └── TorrentAlreadyVerifying
 """
 
 
 class Error(Exception):
     """Parent class of all fatal exceptions"""
 
     def __eq__(self, other):
@@ -127,92 +128,84 @@
 
     def __init__(self, cause):
         super().__init__(f'Verifying torrent failed: {cause}')
 
 
 class Warning(Exception):
     """
-    Success with acceptable, non-serious side effects (e.g. adding duplicate
-    torrent)
+    Generic warning about an acceptable, non-serious issue (e.g. adding
+    duplicate torrent)
     """
 
     def __eq__(self, other):
         return (
             type(self) is type(other)
             and str(self) == str(other)
         )
 
 
-class TorrentAlreadyAdded(Warning):
+class TorrentWarning(Warning):
     """
-    Torrent was already added
+    :class:`Warning` about a torrent that provides the infohash and an
+    optional name
 
     :param infohash: Infohash of the torrent
-    :param name: Torrent name or user-provided torrent file path, magnet URI,
-        etc
+    :param name: Torrent name or user-provided torrent file, magnet URI, etc
 
     `infohash` should be a machine-readable ID while `name` should be a
-    user-readable ID.
+    user-readable ID or an argument from user.
     """
 
+    _msg_with_name = NotImplemented
+    _msg_without_name = NotImplemented
+
     def __init__(self, infohash, name=None):
         if name and name != infohash:
-            super().__init__(f'Torrent already added: {name}: {infohash}')
+            msg_format = self._msg_with_name
         else:
-            super().__init__(f'Torrent already added: {infohash}')
+            msg_format = self._msg_without_name
 
+        if msg_format is NotImplemented:
+            raise RuntimeError(f'You are supposed to subclass {type(self).__name__}')
+        else:
+            msg = msg_format.format(infohash=infohash, name=name)
+            super().__init__(msg)
+            self._infohash = infohash
+            self._name = name
 
-class TorrentAlreadyStarted(Warning):
-    """
-    Torrent is already started
+    @property
+    def infohash(self):
+        """Infohash of the relevant torrent"""
+        return self._infohash
 
-    :param infohash: Infohash of the torrent
-    :param name: Torrent name or user-provided torrent file path, magnet URI,
-        etc
+    @property
+    def name(self):
+        """Name of the relevant torrent or `None`"""
+        return self._name
 
-    `infohash` should be a machine-readable ID while `name` should be a
-    user-readable ID.
-    """
 
-    def __init__(self, infohash, name=None):
-        if name and name != infohash:
-            super().__init__(f'Torrent already started: {name}: {infohash}')
-        else:
-            super().__init__(f'Torrent already started: {infohash}')
+class TorrentAlreadyAdded(TorrentWarning):
+    """Torrent was already added"""
 
+    _msg_with_name = 'Torrent already added: {name}: {infohash}'
+    _msg_without_name = 'Torrent already added: {infohash}'
 
-class TorrentAlreadyStopped(Warning):
-    """
-    Torrent is already stopped
 
-    :param infohash: Infohash of the torrent
-    :param name: Torrent name or user-provided torrent file path, magnet URI,
-        etc
+class TorrentAlreadyStarted(TorrentWarning):
+    """Torrent is already started"""
 
-    `infohash` should be a machine-readable ID while `name` should be a
-    user-readable ID.
-    """
+    _msg_with_name = 'Torrent already started: {name}: {infohash}'
+    _msg_without_name = 'Torrent already started: {infohash}'
 
-    def __init__(self, infohash, name=None):
-        if name and name != infohash:
-            super().__init__(f'Torrent already stopped: {name}: {infohash}')
-        else:
-            super().__init__(f'Torrent already stopped: {infohash}')
 
+class TorrentAlreadyStopped(TorrentWarning):
+    """Torrent is already stopped"""
 
-class TorrentAlreadyVerifying(Warning):
-    """
-    Torrent is already being verified
+    _msg_with_name = 'Torrent already stopped: {name}: {infohash}'
+    _msg_without_name = 'Torrent already stopped: {infohash}'
 
-    :param infohash: Infohash of the torrent
-    :param name: Torrent name or user-provided torrent file path, magnet URI,
-        etc
 
-    `infohash` should be a machine-readable ID while `name` should be a
-    user-readable ID.
-    """
+class TorrentAlreadyVerifying(TorrentWarning):
+    """Torrent is already being verified"""
 
-    def __init__(self, infohash, name=None):
-        if name and name != infohash:
-            super().__init__(f'Torrent already verifying: {name}: {infohash}')
-        else:
-            super().__init__(f'Torrent already verifying: {infohash}')
+    _msg_with_name = 'Torrent already verifying: {name}: {infohash}'
+    _msg_without_name = 'Torrent already verifying: {infohash}'
```

### Comparing `aiobtclientapi-1.0.3/aiobtclientapi/response.py` & `aiobtclientapi-1.1.0/aiobtclientapi/response.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.0.3/aiobtclientapi/utils/__init__.py` & `aiobtclientapi-1.1.0/aiobtclientapi/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     match = is_infohash_regex.search(str(string))
     return bool(match and match.string == match.group(1))
 
 
 class Infohash(str):
     """Case-insensitive string of exactly 40 hexadecimal digits"""
 
-    # Maybe save a few bytes of RAM
+    # Maybe save a few bytes of memory
     __slots__ = ()
 
     def __new__(cls, string):
         s = str(string)
         if not is_infohash_regex.search(s):
             raise errors.ValueError(f'Invalid infohash: {string!r}')
         else:
@@ -198,7 +198,16 @@
             async def return_result(result, exception):
                 if exception:
                     raise exception
                 else:
                     return result
 
             yield return_result(result, exception)
+
+
+def without_None_values(dct):
+    """Return copy of `dct` without the keys that map to `None`"""
+    return {
+        k: v
+        for k, v in dct.items()
+        if v is not None
+    }
```

### Comparing `aiobtclientapi-1.0.3/aiobtclientapi/utils/monitor.py` & `aiobtclientapi-1.1.0/aiobtclientapi/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.0.3/aiobtclientapi/utils/torrent.py` & `aiobtclientapi-1.1.0/aiobtclientapi/utils/torrent.py`

 * *Files 12% similar despite different names*

```diff
@@ -71,7 +71,23 @@
     """
     Return :class:`bytes` from torrent file URL
 
     This is just a convenient wrapper around :func:`~.download` with a
     reasonable `maxsize` argument.
     """
     return await utils.download(url, maxsize=constants.MAX_TORRENT_SIZE)
+
+
+def get_infohash(torrent):
+    """
+    Get `torrent` infohash
+
+    :param torrent: Path to torrent file, magnet URI, raw metainfo
+        (:class:`bytes`) or infohash
+
+    :raise ReadError: if reading `torrent` fails
+    """
+    if utils.is_infohash(torrent):
+        infohash = torrent
+    else:
+        infohash = read(torrent).infohash
+    return utils.Infohash(infohash)
```

### Comparing `aiobtclientapi-1.0.3/aiobtclientapi.egg-info/PKG-INFO` & `aiobtclientapi-1.1.0/aiobtclientapi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiobtclientapi
-Version: 1.0.3
+Version: 1.1.0
 Summary: Asynchronous high-level communication with BitTorrent clients
 Home-page: https://codeberg.org/plotski/aiobtclientapi
 Author: plotski
 Author-email: plotski@example.org
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `aiobtclientapi-1.0.3/aiobtclientapi.egg-info/SOURCES.txt` & `aiobtclientapi-1.1.0/aiobtclientapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.0.3/setup.py` & `aiobtclientapi-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,14 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
     ],
     python_requires='>=3.8',
     install_requires=[
-        'aiobtclientrpc==4.*',
+        'aiobtclientrpc==5.*',
         'async-timeout==4.*',
         'httpx==0.*',
         'torf==4.*',
     ],
     entry_points={'console_scripts': ['btclient = aiobtclientapi.cli:run_sync']},
 )
```

