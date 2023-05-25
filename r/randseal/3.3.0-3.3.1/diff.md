# Comparing `tmp/randseal-3.3.0.tar.gz` & `tmp/randseal-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randseal-3.3.0.tar", last modified: Wed May 24 18:57:42 2023, max compression
+gzip compressed data, was "randseal-3.3.1.tar", last modified: Thu May 25 15:46:54 2023, max compression
```

## Comparing `randseal-3.3.0.tar` & `randseal-3.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 18:57:42.821952 randseal-3.3.0/
--rw-rw-rw-   0        0        0     1073 2023-01-28 21:24:47.000000 randseal-3.3.0/LICENCE
--rw-rw-rw-   0        0        0       65 2023-01-19 20:30:45.000000 randseal-3.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1129 2023-05-24 18:57:42.821952 randseal-3.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      667 2023-01-04 03:58:05.000000 randseal-3.3.0/README.md
--rw-rw-rw-   0        0        0      159 2023-05-24 18:56:43.000000 randseal-3.3.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-24 18:57:42.797748 randseal-3.3.0/randseal/
--rw-rw-rw-   0        0        0     1171 2023-03-09 16:58:34.000000 randseal-3.3.0/randseal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 18:57:42.821952 randseal-3.3.0/randseal/archive/
--rw-rw-rw-   0        0        0     1135 2023-01-28 21:25:20.000000 randseal-3.3.0/randseal/archive/__init__.py
--rw-rw-rw-   0        0        0     1715 2023-05-24 18:16:41.000000 randseal-3.3.0/randseal/archive/one.py
--rw-rw-rw-   0        0        0     6526 2023-05-24 18:43:14.000000 randseal-3.3.0/randseal/client.py
--rw-rw-rw-   0        0        0      539 2023-04-26 19:56:52.000000 randseal-3.3.0/randseal/errors.py
--rw-rw-rw-   0        0        0      639 2023-03-10 16:48:34.000000 randseal-3.3.0/randseal/timestamp.py
--rw-rw-rw-   0        0        0      787 2023-04-26 19:52:24.000000 randseal-3.3.0/randseal/vars.py
-drwxrwxrwx   0        0        0        0 2023-05-24 18:57:42.814231 randseal-3.3.0/randseal.egg-info/
--rw-rw-rw-   0        0        0     1129 2023-05-24 18:57:42.000000 randseal-3.3.0/randseal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-05-24 18:57:42.000000 randseal-3.3.0/randseal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 18:57:42.000000 randseal-3.3.0/randseal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-24 18:57:42.000000 randseal-3.3.0/randseal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      560 2023-05-24 18:57:42.830982 randseal-3.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 15:46:54.728621 randseal-3.3.1/
+-rw-rw-rw-   0        0        0     1073 2023-01-28 21:24:47.000000 randseal-3.3.1/LICENCE
+-rw-rw-rw-   0        0        0       65 2023-01-19 20:30:45.000000 randseal-3.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1129 2023-05-25 15:46:54.729622 randseal-3.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      667 2023-01-04 03:58:05.000000 randseal-3.3.1/README.md
+-rw-rw-rw-   0        0        0      159 2023-05-24 18:56:43.000000 randseal-3.3.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-25 15:46:54.687094 randseal-3.3.1/randseal/
+-rw-rw-rw-   0        0        0     1171 2023-03-09 16:58:34.000000 randseal-3.3.1/randseal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:46:54.728621 randseal-3.3.1/randseal/archive/
+-rw-rw-rw-   0        0        0     1135 2023-01-28 21:25:20.000000 randseal-3.3.1/randseal/archive/__init__.py
+-rw-rw-rw-   0        0        0     1715 2023-05-24 18:16:41.000000 randseal-3.3.1/randseal/archive/one.py
+-rw-rw-rw-   0        0        0     6511 2023-05-25 15:46:02.000000 randseal-3.3.1/randseal/client.py
+-rw-rw-rw-   0        0        0      539 2023-04-26 19:56:52.000000 randseal-3.3.1/randseal/errors.py
+-rw-rw-rw-   0        0        0      639 2023-03-10 16:48:34.000000 randseal-3.3.1/randseal/timestamp.py
+-rw-rw-rw-   0        0        0      787 2023-04-26 19:52:24.000000 randseal-3.3.1/randseal/vars.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:46:54.725622 randseal-3.3.1/randseal.egg-info/
+-rw-rw-rw-   0        0        0     1129 2023-05-25 15:46:54.000000 randseal-3.3.1/randseal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-05-25 15:46:54.000000 randseal-3.3.1/randseal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 15:46:54.000000 randseal-3.3.1/randseal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-25 15:46:54.000000 randseal-3.3.1/randseal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      560 2023-05-25 15:46:54.734622 randseal-3.3.1/setup.cfg
```

### Comparing `randseal-3.3.0/LICENCE` & `randseal-3.3.1/LICENCE`

 * *Files identical despite different names*

### Comparing `randseal-3.3.0/PKG-INFO` & `randseal-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: randseal
-Version: 3.3.0
+Version: 3.3.1
 Summary: Generates random seal images for discord.py or py-cord
 Home-page: https://github.com/mariohero24/randseal
 Author: Guard Boi
 Author-email: guard@cowbot.xyz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `randseal-3.3.0/README.md` & `randseal-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `randseal-3.3.0/randseal/__init__.py` & `randseal-3.3.1/randseal/__init__.py`

 * *Files identical despite different names*

### Comparing `randseal-3.3.0/randseal/archive/__init__.py` & `randseal-3.3.1/randseal/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `randseal-3.3.0/randseal/archive/one.py` & `randseal-3.3.1/randseal/archive/one.py`

 * *Files identical despite different names*

### Comparing `randseal-3.3.0/randseal/client.py` & `randseal-3.3.1/randseal/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from aiofiles import open as iopen
 from io import BytesIO, TextIOWrapper
 from asyncio import get_event_loop, AbstractEventLoop, iscoroutine
 from random import randrange
 from traceback import format_exception
 from json import loads, dumps, load, dump
 from typing import AsyncIterator, Iterator, Coroutine, Any
-from .errors import StatusException, BaseException, InvalidType
+from .errors import StatusException, InvalidType
 from os import path
 from sys import stderr
 from aiofiles.threadpool.text import AsyncTextIOWrapper
 from .vars import MAX_NUMBER, BLANK
 
 class Client:
 	"""The main `Client` class for this package
```

### Comparing `randseal-3.3.0/randseal/errors.py` & `randseal-3.3.1/randseal/errors.py`

 * *Files identical despite different names*

### Comparing `randseal-3.3.0/randseal/timestamp.py` & `randseal-3.3.1/randseal/timestamp.py`

 * *Files identical despite different names*

### Comparing `randseal-3.3.0/randseal/vars.py` & `randseal-3.3.1/randseal/vars.py`

 * *Files identical despite different names*

### Comparing `randseal-3.3.0/randseal.egg-info/PKG-INFO` & `randseal-3.3.1/randseal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: randseal
-Version: 3.3.0
+Version: 3.3.1
 Summary: Generates random seal images for discord.py or py-cord
 Home-page: https://github.com/mariohero24/randseal
 Author: Guard Boi
 Author-email: guard@cowbot.xyz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `randseal-3.3.0/setup.cfg` & `randseal-3.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2072 616e 6473 6561 6c0d 0a76 6572   = randseal..ver
-00000020: 7369 6f6e 203d 2033 2e33 2e30 0d0a 6175  sion = 3.3.0..au
+00000020: 7369 6f6e 203d 2033 2e33 2e31 0d0a 6175  sion = 3.3.1..au
 00000030: 7468 6f72 203d 2047 7561 7264 2042 6f69  thor = Guard Boi
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2067 7561 7264 4063 6f77 626f 742e 7879   guard@cowbot.xy
 00000060: 7a0d 0a64 6573 6372 6970 7469 6f6e 203d  z..description =
 00000070: 2047 656e 6572 6174 6573 2072 616e 646f   Generates rando
 00000080: 6d20 7365 616c 2069 6d61 6765 7320 666f  m seal images fo
 00000090: 7220 6469 7363 6f72 642e 7079 206f 7220  r discord.py or
```

