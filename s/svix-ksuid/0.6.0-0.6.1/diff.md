# Comparing `tmp/svix-ksuid-0.6.0.tar.gz` & `tmp/svix-ksuid-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svix-ksuid-0.6.0.tar", last modified: Fri Aug 27 01:02:31 2021, max compression
+gzip compressed data, was "svix-ksuid-0.6.1.tar", last modified: Thu May 25 12:47:09 2023, max compression
```

## Comparing `svix-ksuid-0.6.0.tar` & `svix-ksuid-0.6.1.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-08-27 01:02:31.151725 svix-ksuid-0.6.0/
--rw-r--r--   0 tom       (1000) tom       (1000)     1087 2021-07-12 10:31:00.000000 svix-ksuid-0.6.0/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)     5206 2021-08-27 01:02:31.151725 svix-ksuid-0.6.0/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     4094 2021-08-17 15:19:24.000000 svix-ksuid-0.6.0/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-08-27 01:02:31.151725 svix-ksuid-0.6.0/ksuid/
--rw-r--r--   0 tom       (1000) tom       (1000)      120 2021-08-17 15:19:24.000000 svix-ksuid-0.6.0/ksuid/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4007 2021-08-27 00:59:46.000000 svix-ksuid-0.6.0/ksuid/ksuid.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2021-07-12 10:31:15.000000 svix-ksuid-0.6.0/ksuid/py.typed
--rw-r--r--   0 tom       (1000) tom       (1000)      196 2021-07-12 10:31:00.000000 svix-ksuid-0.6.0/pyproject.toml
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2021-08-27 01:02:31.151725 svix-ksuid-0.6.0/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)     1850 2021-08-27 01:01:51.000000 svix-ksuid-0.6.0/setup.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-08-27 01:02:31.151725 svix-ksuid-0.6.0/svix_ksuid.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     5206 2021-08-27 01:02:31.000000 svix-ksuid-0.6.0/svix_ksuid.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      291 2021-08-27 01:02:31.000000 svix-ksuid-0.6.0/svix_ksuid.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2021-08-27 01:02:31.000000 svix-ksuid-0.6.0/svix_ksuid.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2021-07-12 10:31:15.000000 svix-ksuid-0.6.0/svix_ksuid.egg-info/not-zip-safe
--rw-r--r--   0 tom       (1000) tom       (1000)       16 2021-08-27 01:02:31.000000 svix-ksuid-0.6.0/svix_ksuid.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        6 2021-08-27 01:02:31.000000 svix-ksuid-0.6.0/svix_ksuid.egg-info/top_level.txt
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-25 12:47:09.827973 svix-ksuid-0.6.1/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1087 2021-07-12 10:31:00.000000 svix-ksuid-0.6.1/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)     5318 2023-05-25 12:47:09.827973 svix-ksuid-0.6.1/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     4226 2023-05-25 12:26:03.000000 svix-ksuid-0.6.1/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-25 12:47:09.827973 svix-ksuid-0.6.1/ksuid/
+-rw-r--r--   0 tom       (1000) tom       (1000)      120 2021-08-17 15:19:24.000000 svix-ksuid-0.6.1/ksuid/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4033 2023-05-25 12:26:03.000000 svix-ksuid-0.6.1/ksuid/ksuid.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2021-07-12 10:31:15.000000 svix-ksuid-0.6.1/ksuid/py.typed
+-rw-r--r--   0 tom       (1000) tom       (1000)      196 2021-07-12 10:31:00.000000 svix-ksuid-0.6.1/pyproject.toml
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-05-25 12:47:09.827973 svix-ksuid-0.6.1/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)     1850 2023-05-25 12:26:36.000000 svix-ksuid-0.6.1/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-25 12:47:09.827973 svix-ksuid-0.6.1/svix_ksuid.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     5318 2023-05-25 12:47:09.000000 svix-ksuid-0.6.1/svix_ksuid.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      311 2023-05-25 12:47:09.000000 svix-ksuid-0.6.1/svix_ksuid.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-05-25 12:47:09.000000 svix-ksuid-0.6.1/svix_ksuid.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2021-07-12 10:31:15.000000 svix-ksuid-0.6.1/svix_ksuid.egg-info/not-zip-safe
+-rw-r--r--   0 tom       (1000) tom       (1000)       16 2023-05-25 12:47:09.000000 svix-ksuid-0.6.1/svix_ksuid.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        6 2023-05-25 12:47:09.000000 svix-ksuid-0.6.1/svix_ksuid.egg-info/top_level.txt
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-25 12:47:09.827973 svix-ksuid-0.6.1/tests/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4980 2022-01-29 11:28:54.000000 svix-ksuid-0.6.1/tests/test_ksuid.py
```

### Comparing `svix-ksuid-0.6.0/LICENSE` & `svix-ksuid-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `svix-ksuid-0.6.0/PKG-INFO` & `svix-ksuid-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: svix-ksuid
-Version: 0.6.0
+Version: 0.6.1
 Summary:  A pure-Python KSUID implementation
 Home-page: https://github.com/svixhq/python-ksuid/
 Author: Svix
 Author-email: development@svix.com
 License: MIT
 Keywords: svix,ksuid
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -30,39 +29,41 @@
 <h1 align="center">
   <a href="https://www.svix.com">
     <img width="120" src="https://avatars.githubusercontent.com/u/80175132?s=200&v=4" />
     <p align="center">Svix - Webhooks as a service</p>
   </a>
 </h1>
 
-# Svix-KSUID
+# Svix-KSUID (Python)
 
 ![API-Lint](https://github.com/svixhq/python-ksuid/workflows/lint/badge.svg)
 ![Frontend-Lint](https://github.com/svixhq/python-ksuid/workflows/test/badge.svg)
 ![GitHub tag](https://img.shields.io/github/tag/svixhq/python-ksuid.svg)
 [![PyPI](https://img.shields.io/pypi/v/svix-ksuid.svg)](https://pypi.python.org/pypi/svix-ksuid/)
 [![Join our slack](https://img.shields.io/badge/Slack-join%20the%20community-blue?logo=slack&style=social)](https://www.svix.com/slack/)
 
 This library is inspired by [Segment's KSUID](https://segment.com/blog/a-brief-history-of-the-uuid/) implementation:
 https://github.com/segmentio/ksuid
 
+For the Rust version, please check out https://github.com/svix/rust-ksuid
+
 ## What is a ksuid?
 
 A ksuid is a K sorted UID. In other words, a KSUID also stores a date component, so that ksuids can be approximately 
 sorted based on the time they were created. 
 
 Read more [here](https://segment.com/blog/a-brief-history-of-the-uuid/).
 
 ## Usage
 
 ```
 pip install svix-ksuid
 ```
 
-```
+```python
 from ksuid import Ksuid
 
 ksuid = Ksuid()
 ```
 
 ### Higher timestamp accuracy mode
 
@@ -72,27 +73,27 @@
 
 The code too is fully compatible:
 
 ```
 pip install svix-ksuid
 ```
 
-```
+```python
 from ksuid import KsuidMs
 
 ksuid = KsuidMs()
 ```
 
 ## Examples
 
 ### Default ksuid
 
 Generate a ksuid without passing a specific datetime
 
-```
+```python
 In [1]: from ksuid import Ksuid
 
 In [2]: ksuid = Ksuid()
 
 In [3]: f"Base62: {ksuid}"
 Out[3]: 'Base62: 1srOrx2ZWZBpBUvZwXKQmoEYga2'
 
@@ -107,15 +108,15 @@
 
 In [7]: f"Payload: {ksuid.payload}"
 Out[7]: "Payload: b'\\xe1\\x93>7\\xf2up\\x87c\\xad\\xc7tZ\\xf5\\xe7\\xf2'"
 ```
 
 ### ksuid from datetime
 
-```
+```python
 In [1]: datetime = datetime(year=2021, month=5, day=19, hour=1, minute=1, second=1, microsecond=1)
 
 In [2]: datetime
 Out[2]: datetime.datetime(2021, 5, 19, 1, 1, 1, 1)
 
 In [3]: ksuid = Ksuid(datetime)
 
@@ -124,15 +125,15 @@
 
 In [5]: ksuid.timestamp
 Out[5]: 1621407661
 ```
 
 ### ksuid from base62
 
-```
+```python
 In [1]: ksuid = Ksuid()
 
 In [2]: ksuid.timestamp
 Out[2]: 1621634852
 
 In [3]: f"Base62: {ksuid}"
 Out[3]: 'Base62: 1srdszO8Xy2cR6CnARnvxCfRmK4'
@@ -141,29 +142,29 @@
 
 In [5]: ksuid_from_base62.timestamp
 Out[5]: 1621634852
 ```
 
 ### ksuid from bytes
 
-```
+```python
 In [1]: ksuid = Ksuid()
 
 In [2]: ksuid_from_bytes = ksuid.from_bytes(bytes(ksuid))
 
 In [3]: f"ksuid: {ksuid}, ksuid_from_bytes: {ksuid_from_bytes}"
 Out[3]: 'ksuid: 1sreAHoz6myPhXghsOdVBoec3Vr, ksuid_from_bytes: 1sreAHoz6myPhXghsOdVBoec3Vr'
 
 In [4]: ksuid == ksuid_from_bytes
 Out[4]: True
 ```
 
 ### Compare ksuid(s)
 
-```
+```python
 In [1]: ksuid_1 = Ksuid()
 
 In [2]: ksuid_2 = Ksuid.from_bytes(bytes(ksuid_1))
 
 In [3]: f"ksuid_1: {ksuid_1}, ksuid_2: {ksuid_2}"
 Out[3]: 'ksuid_1: 1sreAHoz6myPhXghsOdVBoec3Vr, ksuid_2: 1sreAHoz6myPhXghsOdVBoec3Vr'
 
@@ -176,15 +177,15 @@
 In [6]: ksuid_2
 Out[6]: 1tM9eRSTrHIrrH5SMEW24rtvIOF
 ```
 
 
 ### Order of ksuid(s)
 
-```
+```python
 In [1]: ksuid_1 = Ksuid()
 
 In [2]: ksuid_1.timestamp
 Out[2]: 1621963256
 
 In [3]: ksuid_2 = Ksuid()
 
@@ -203,9 +204,7 @@
 In [8]: ksuid_1 > ksuid_2
 Out[8]: False
 ```
 
 ### License
 
 ksuid source code is available under an MIT [License](./LICENSE).
-
-
```

#### html2text {}

```diff
@@ -1,69 +1,70 @@
-Metadata-Version: 2.1 Name: svix-ksuid Version: 0.6.0 Summary: A pure-Python
+Metadata-Version: 2.1 Name: svix-ksuid Version: 0.6.1 Summary: A pure-Python
 KSUID implementation Home-page: https://github.com/svixhq/python-ksuid/ Author:
 Svix Author-email: development@svix.com License: MIT Keywords: svix,ksuid
-Platform: UNKNOWN Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Information Technology Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python Classifier: Topic :: Software Development ::
-Libraries :: Application Frameworks Classifier: Topic :: Software Development
-:: Libraries :: Python Modules Classifier: Topic :: Software Development ::
-Libraries Classifier: Topic :: Software Development Classifier: Typing :: Typed
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Information Technology Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python Classifier: Topic :: Software Development :: Libraries ::
+Application Frameworks Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development Classifier: Typing :: Typed
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE
          [https://avatars.githubusercontent.com/u/80175132?s=200&v=4]
                          Svix_-_Webhooks_as_a_service
-# Svix-KSUID ![API-Lint](https://github.com/svixhq/python-ksuid/workflows/lint/
-badge.svg) ![Frontend-Lint](https://github.com/svixhq/python-ksuid/workflows/
-test/badge.svg) ![GitHub tag](https://img.shields.io/github/tag/svixhq/python-
-ksuid.svg) [![PyPI](https://img.shields.io/pypi/v/svix-ksuid.svg)](https://
-pypi.python.org/pypi/svix-ksuid/) [![Join our slack](https://img.shields.io/
-badge/Slack-join%20the%20community-blue?logo=slack&style=social)](https://
-www.svix.com/slack/) This library is inspired by [Segment's KSUID](https://
-segment.com/blog/a-brief-history-of-the-uuid/) implementation: https://
-github.com/segmentio/ksuid ## What is a ksuid? A ksuid is a K sorted UID. In
-other words, a KSUID also stores a date component, so that ksuids can be
-approximately sorted based on the time they were created. Read more [here]
-(https://segment.com/blog/a-brief-history-of-the-uuid/). ## Usage ``` pip
-install svix-ksuid ``` ``` from ksuid import Ksuid ksuid = Ksuid() ``` ###
-Higher timestamp accuracy mode Ksuids have a 1 second accuracy which is not
-sufficient for all use-cases. That's why this library exposes a higher accuracy
-mode which supports accuracy of up to 4ms. It's fully compatible with normal
-ksuids, in fact, it outputs valid ksuids. The difference is that it sacrifices
-one byte of the random payload in favor of this accuracy. The code too is fully
-compatible: ``` pip install svix-ksuid ``` ``` from ksuid import KsuidMs ksuid
-= KsuidMs() ``` ## Examples ### Default ksuid Generate a ksuid without passing
-a specific datetime ``` In [1]: from ksuid import Ksuid In [2]: ksuid = Ksuid()
-In [3]: f"Base62: {ksuid}" Out[3]: 'Base62: 1srOrx2ZWZBpBUvZwXKQmoEYga2' In
-[4]: f"Bytes: {bytes(ksuid)}" Out[4]: "Bytes:
-b'\\r5\\xc43\\xe1\\x93>7\\xf2up\\x87c\\xad\\xc7tZ\\xf5\\xe7\\xf2'" In [5]:
-f"Datetime: {ksuid.datetime}" Out[5]: 'Datetime: 2021-05-21 14:04:03' In [6]:
-f"Timestamp: {ksuid.timestamp}" Out[6]: 'Timestamp: 1621627443' In [7]:
+# Svix-KSUID (Python) ![API-Lint](https://github.com/svixhq/python-ksuid/
+workflows/lint/badge.svg) ![Frontend-Lint](https://github.com/svixhq/python-
+ksuid/workflows/test/badge.svg) ![GitHub tag](https://img.shields.io/github/
+tag/svixhq/python-ksuid.svg) [![PyPI](https://img.shields.io/pypi/v/svix-
+ksuid.svg)](https://pypi.python.org/pypi/svix-ksuid/) [![Join our slack](https:
+//img.shields.io/badge/Slack-join%20the%20community-
+blue?logo=slack&style=social)](https://www.svix.com/slack/) This library is
+inspired by [Segment's KSUID](https://segment.com/blog/a-brief-history-of-the-
+uuid/) implementation: https://github.com/segmentio/ksuid For the Rust version,
+please check out https://github.com/svix/rust-ksuid ## What is a ksuid? A ksuid
+is a K sorted UID. In other words, a KSUID also stores a date component, so
+that ksuids can be approximately sorted based on the time they were created.
+Read more [here](https://segment.com/blog/a-brief-history-of-the-uuid/). ##
+Usage ``` pip install svix-ksuid ``` ```python from ksuid import Ksuid ksuid =
+Ksuid() ``` ### Higher timestamp accuracy mode Ksuids have a 1 second accuracy
+which is not sufficient for all use-cases. That's why this library exposes a
+higher accuracy mode which supports accuracy of up to 4ms. It's fully
+compatible with normal ksuids, in fact, it outputs valid ksuids. The difference
+is that it sacrifices one byte of the random payload in favor of this accuracy.
+The code too is fully compatible: ``` pip install svix-ksuid ``` ```python from
+ksuid import KsuidMs ksuid = KsuidMs() ``` ## Examples ### Default ksuid
+Generate a ksuid without passing a specific datetime ```python In [1]: from
+ksuid import Ksuid In [2]: ksuid = Ksuid() In [3]: f"Base62: {ksuid}" Out[3]:
+'Base62: 1srOrx2ZWZBpBUvZwXKQmoEYga2' In [4]: f"Bytes: {bytes(ksuid)}" Out[4]:
+"Bytes: b'\\r5\\xc43\\xe1\\x93>7\\xf2up\\x87c\\xad\\xc7tZ\\xf5\\xe7\\xf2'" In
+[5]: f"Datetime: {ksuid.datetime}" Out[5]: 'Datetime: 2021-05-21 14:04:03' In
+[6]: f"Timestamp: {ksuid.timestamp}" Out[6]: 'Timestamp: 1621627443' In [7]:
 f"Payload: {ksuid.payload}" Out[7]: "Payload:
 b'\\xe1\\x93>7\\xf2up\\x87c\\xad\\xc7tZ\\xf5\\xe7\\xf2'" ``` ### ksuid from
-datetime ``` In [1]: datetime = datetime(year=2021, month=5, day=19, hour=1,
-minute=1, second=1, microsecond=1) In [2]: datetime Out[2]: datetime.datetime
-(2021, 5, 19, 1, 1, 1, 1) In [3]: ksuid = Ksuid(datetime) In [4]:
-ksuid.datetime Out[4]: datetime.datetime(2021, 5, 19, 1, 1, 1) In [5]:
-ksuid.timestamp Out[5]: 1621407661 ``` ### ksuid from base62 ``` In [1]: ksuid
-= Ksuid() In [2]: ksuid.timestamp Out[2]: 1621634852 In [3]: f"Base62: {ksuid}"
-Out[3]: 'Base62: 1srdszO8Xy2cR6CnARnvxCfRmK4' In [4]: ksuid_from_base62 =
-Ksuid.from_base62("1srdszO8Xy2cR6CnARnvxCfRmK4") In [5]:
-ksuid_from_base62.timestamp Out[5]: 1621634852 ``` ### ksuid from bytes ``` In
-[1]: ksuid = Ksuid() In [2]: ksuid_from_bytes = ksuid.from_bytes(bytes(ksuid))
-In [3]: f"ksuid: {ksuid}, ksuid_from_bytes: {ksuid_from_bytes}" Out[3]: 'ksuid:
-1sreAHoz6myPhXghsOdVBoec3Vr, ksuid_from_bytes: 1sreAHoz6myPhXghsOdVBoec3Vr' In
-[4]: ksuid == ksuid_from_bytes Out[4]: True ``` ### Compare ksuid(s) ``` In
-[1]: ksuid_1 = Ksuid() In [2]: ksuid_2 = Ksuid.from_bytes(bytes(ksuid_1)) In
-[3]: f"ksuid_1: {ksuid_1}, ksuid_2: {ksuid_2}" Out[3]: 'ksuid_1:
-1sreAHoz6myPhXghsOdVBoec3Vr, ksuid_2: 1sreAHoz6myPhXghsOdVBoec3Vr' In [4]:
-ksuid_1 == ksuid_2 Out[4]: True In [5]: ksuid_1 Out[5]:
-1tM9eRSTrHIrrH5SMEW24rtvIOF In [6]: ksuid_2 Out[6]: 1tM9eRSTrHIrrH5SMEW24rtvIOF
-``` ### Order of ksuid(s) ``` In [1]: ksuid_1 = Ksuid() In [2]:
-ksuid_1.timestamp Out[2]: 1621963256 In [3]: ksuid_2 = Ksuid() In [4]:
-ksuid_2.timestamp Out[4]: 1621963266 In [5]: ksuid_1 < ksuid_2 Out[5]: True In
-[6]: ksuid_1 <= ksuid_2 Out[6]: True In [7]: ksuid_1 >= ksuid_2 Out[7]: False
-In [8]: ksuid_1 > ksuid_2 Out[8]: False ``` ### License ksuid source code is
-available under an MIT [License](./LICENSE).
+datetime ```python In [1]: datetime = datetime(year=2021, month=5, day=19,
+hour=1, minute=1, second=1, microsecond=1) In [2]: datetime Out[2]:
+datetime.datetime(2021, 5, 19, 1, 1, 1, 1) In [3]: ksuid = Ksuid(datetime) In
+[4]: ksuid.datetime Out[4]: datetime.datetime(2021, 5, 19, 1, 1, 1) In [5]:
+ksuid.timestamp Out[5]: 1621407661 ``` ### ksuid from base62 ```python In [1]:
+ksuid = Ksuid() In [2]: ksuid.timestamp Out[2]: 1621634852 In [3]: f"Base62:
+{ksuid}" Out[3]: 'Base62: 1srdszO8Xy2cR6CnARnvxCfRmK4' In [4]:
+ksuid_from_base62 = Ksuid.from_base62("1srdszO8Xy2cR6CnARnvxCfRmK4") In [5]:
+ksuid_from_base62.timestamp Out[5]: 1621634852 ``` ### ksuid from bytes
+```python In [1]: ksuid = Ksuid() In [2]: ksuid_from_bytes = ksuid.from_bytes
+(bytes(ksuid)) In [3]: f"ksuid: {ksuid}, ksuid_from_bytes: {ksuid_from_bytes}"
+Out[3]: 'ksuid: 1sreAHoz6myPhXghsOdVBoec3Vr, ksuid_from_bytes:
+1sreAHoz6myPhXghsOdVBoec3Vr' In [4]: ksuid == ksuid_from_bytes Out[4]: True ```
+### Compare ksuid(s) ```python In [1]: ksuid_1 = Ksuid() In [2]: ksuid_2 =
+Ksuid.from_bytes(bytes(ksuid_1)) In [3]: f"ksuid_1: {ksuid_1}, ksuid_2:
+{ksuid_2}" Out[3]: 'ksuid_1: 1sreAHoz6myPhXghsOdVBoec3Vr, ksuid_2:
+1sreAHoz6myPhXghsOdVBoec3Vr' In [4]: ksuid_1 == ksuid_2 Out[4]: True In [5]:
+ksuid_1 Out[5]: 1tM9eRSTrHIrrH5SMEW24rtvIOF In [6]: ksuid_2 Out[6]:
+1tM9eRSTrHIrrH5SMEW24rtvIOF ``` ### Order of ksuid(s) ```python In [1]: ksuid_1
+= Ksuid() In [2]: ksuid_1.timestamp Out[2]: 1621963256 In [3]: ksuid_2 = Ksuid
+() In [4]: ksuid_2.timestamp Out[4]: 1621963266 In [5]: ksuid_1 < ksuid_2 Out
+[5]: True In [6]: ksuid_1 <= ksuid_2 Out[6]: True In [7]: ksuid_1 >= ksuid_2
+Out[7]: False In [8]: ksuid_1 > ksuid_2 Out[8]: False ``` ### License ksuid
+source code is available under an MIT [License](./LICENSE).
```

### Comparing `svix-ksuid-0.6.0/README.md` & `svix-ksuid-0.6.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 <h1 align="center">
   <a href="https://www.svix.com">
     <img width="120" src="https://avatars.githubusercontent.com/u/80175132?s=200&v=4" />
     <p align="center">Svix - Webhooks as a service</p>
   </a>
 </h1>
 
-# Svix-KSUID
+# Svix-KSUID (Python)
 
 ![API-Lint](https://github.com/svixhq/python-ksuid/workflows/lint/badge.svg)
 ![Frontend-Lint](https://github.com/svixhq/python-ksuid/workflows/test/badge.svg)
 ![GitHub tag](https://img.shields.io/github/tag/svixhq/python-ksuid.svg)
 [![PyPI](https://img.shields.io/pypi/v/svix-ksuid.svg)](https://pypi.python.org/pypi/svix-ksuid/)
 [![Join our slack](https://img.shields.io/badge/Slack-join%20the%20community-blue?logo=slack&style=social)](https://www.svix.com/slack/)
 
 This library is inspired by [Segment's KSUID](https://segment.com/blog/a-brief-history-of-the-uuid/) implementation:
 https://github.com/segmentio/ksuid
 
+For the Rust version, please check out https://github.com/svix/rust-ksuid
+
 ## What is a ksuid?
 
 A ksuid is a K sorted UID. In other words, a KSUID also stores a date component, so that ksuids can be approximately 
 sorted based on the time they were created. 
 
 Read more [here](https://segment.com/blog/a-brief-history-of-the-uuid/).
 
 ## Usage
 
 ```
 pip install svix-ksuid
 ```
 
-```
+```python
 from ksuid import Ksuid
 
 ksuid = Ksuid()
 ```
 
 ### Higher timestamp accuracy mode
 
@@ -43,27 +45,27 @@
 
 The code too is fully compatible:
 
 ```
 pip install svix-ksuid
 ```
 
-```
+```python
 from ksuid import KsuidMs
 
 ksuid = KsuidMs()
 ```
 
 ## Examples
 
 ### Default ksuid
 
 Generate a ksuid without passing a specific datetime
 
-```
+```python
 In [1]: from ksuid import Ksuid
 
 In [2]: ksuid = Ksuid()
 
 In [3]: f"Base62: {ksuid}"
 Out[3]: 'Base62: 1srOrx2ZWZBpBUvZwXKQmoEYga2'
 
@@ -78,15 +80,15 @@
 
 In [7]: f"Payload: {ksuid.payload}"
 Out[7]: "Payload: b'\\xe1\\x93>7\\xf2up\\x87c\\xad\\xc7tZ\\xf5\\xe7\\xf2'"
 ```
 
 ### ksuid from datetime
 
-```
+```python
 In [1]: datetime = datetime(year=2021, month=5, day=19, hour=1, minute=1, second=1, microsecond=1)
 
 In [2]: datetime
 Out[2]: datetime.datetime(2021, 5, 19, 1, 1, 1, 1)
 
 In [3]: ksuid = Ksuid(datetime)
 
@@ -95,15 +97,15 @@
 
 In [5]: ksuid.timestamp
 Out[5]: 1621407661
 ```
 
 ### ksuid from base62
 
-```
+```python
 In [1]: ksuid = Ksuid()
 
 In [2]: ksuid.timestamp
 Out[2]: 1621634852
 
 In [3]: f"Base62: {ksuid}"
 Out[3]: 'Base62: 1srdszO8Xy2cR6CnARnvxCfRmK4'
@@ -112,29 +114,29 @@
 
 In [5]: ksuid_from_base62.timestamp
 Out[5]: 1621634852
 ```
 
 ### ksuid from bytes
 
-```
+```python
 In [1]: ksuid = Ksuid()
 
 In [2]: ksuid_from_bytes = ksuid.from_bytes(bytes(ksuid))
 
 In [3]: f"ksuid: {ksuid}, ksuid_from_bytes: {ksuid_from_bytes}"
 Out[3]: 'ksuid: 1sreAHoz6myPhXghsOdVBoec3Vr, ksuid_from_bytes: 1sreAHoz6myPhXghsOdVBoec3Vr'
 
 In [4]: ksuid == ksuid_from_bytes
 Out[4]: True
 ```
 
 ### Compare ksuid(s)
 
-```
+```python
 In [1]: ksuid_1 = Ksuid()
 
 In [2]: ksuid_2 = Ksuid.from_bytes(bytes(ksuid_1))
 
 In [3]: f"ksuid_1: {ksuid_1}, ksuid_2: {ksuid_2}"
 Out[3]: 'ksuid_1: 1sreAHoz6myPhXghsOdVBoec3Vr, ksuid_2: 1sreAHoz6myPhXghsOdVBoec3Vr'
 
@@ -147,15 +149,15 @@
 In [6]: ksuid_2
 Out[6]: 1tM9eRSTrHIrrH5SMEW24rtvIOF
 ```
 
 
 ### Order of ksuid(s)
 
-```
+```python
 In [1]: ksuid_1 = Ksuid()
 
 In [2]: ksuid_1.timestamp
 Out[2]: 1621963256
 
 In [3]: ksuid_2 = Ksuid()
```

#### html2text {}

```diff
@@ -1,54 +1,55 @@
          [https://avatars.githubusercontent.com/u/80175132?s=200&v=4]
                          Svix_-_Webhooks_as_a_service
-# Svix-KSUID ![API-Lint](https://github.com/svixhq/python-ksuid/workflows/lint/
-badge.svg) ![Frontend-Lint](https://github.com/svixhq/python-ksuid/workflows/
-test/badge.svg) ![GitHub tag](https://img.shields.io/github/tag/svixhq/python-
-ksuid.svg) [![PyPI](https://img.shields.io/pypi/v/svix-ksuid.svg)](https://
-pypi.python.org/pypi/svix-ksuid/) [![Join our slack](https://img.shields.io/
-badge/Slack-join%20the%20community-blue?logo=slack&style=social)](https://
-www.svix.com/slack/) This library is inspired by [Segment's KSUID](https://
-segment.com/blog/a-brief-history-of-the-uuid/) implementation: https://
-github.com/segmentio/ksuid ## What is a ksuid? A ksuid is a K sorted UID. In
-other words, a KSUID also stores a date component, so that ksuids can be
-approximately sorted based on the time they were created. Read more [here]
-(https://segment.com/blog/a-brief-history-of-the-uuid/). ## Usage ``` pip
-install svix-ksuid ``` ``` from ksuid import Ksuid ksuid = Ksuid() ``` ###
-Higher timestamp accuracy mode Ksuids have a 1 second accuracy which is not
-sufficient for all use-cases. That's why this library exposes a higher accuracy
-mode which supports accuracy of up to 4ms. It's fully compatible with normal
-ksuids, in fact, it outputs valid ksuids. The difference is that it sacrifices
-one byte of the random payload in favor of this accuracy. The code too is fully
-compatible: ``` pip install svix-ksuid ``` ``` from ksuid import KsuidMs ksuid
-= KsuidMs() ``` ## Examples ### Default ksuid Generate a ksuid without passing
-a specific datetime ``` In [1]: from ksuid import Ksuid In [2]: ksuid = Ksuid()
-In [3]: f"Base62: {ksuid}" Out[3]: 'Base62: 1srOrx2ZWZBpBUvZwXKQmoEYga2' In
-[4]: f"Bytes: {bytes(ksuid)}" Out[4]: "Bytes:
-b'\\r5\\xc43\\xe1\\x93>7\\xf2up\\x87c\\xad\\xc7tZ\\xf5\\xe7\\xf2'" In [5]:
-f"Datetime: {ksuid.datetime}" Out[5]: 'Datetime: 2021-05-21 14:04:03' In [6]:
-f"Timestamp: {ksuid.timestamp}" Out[6]: 'Timestamp: 1621627443' In [7]:
+# Svix-KSUID (Python) ![API-Lint](https://github.com/svixhq/python-ksuid/
+workflows/lint/badge.svg) ![Frontend-Lint](https://github.com/svixhq/python-
+ksuid/workflows/test/badge.svg) ![GitHub tag](https://img.shields.io/github/
+tag/svixhq/python-ksuid.svg) [![PyPI](https://img.shields.io/pypi/v/svix-
+ksuid.svg)](https://pypi.python.org/pypi/svix-ksuid/) [![Join our slack](https:
+//img.shields.io/badge/Slack-join%20the%20community-
+blue?logo=slack&style=social)](https://www.svix.com/slack/) This library is
+inspired by [Segment's KSUID](https://segment.com/blog/a-brief-history-of-the-
+uuid/) implementation: https://github.com/segmentio/ksuid For the Rust version,
+please check out https://github.com/svix/rust-ksuid ## What is a ksuid? A ksuid
+is a K sorted UID. In other words, a KSUID also stores a date component, so
+that ksuids can be approximately sorted based on the time they were created.
+Read more [here](https://segment.com/blog/a-brief-history-of-the-uuid/). ##
+Usage ``` pip install svix-ksuid ``` ```python from ksuid import Ksuid ksuid =
+Ksuid() ``` ### Higher timestamp accuracy mode Ksuids have a 1 second accuracy
+which is not sufficient for all use-cases. That's why this library exposes a
+higher accuracy mode which supports accuracy of up to 4ms. It's fully
+compatible with normal ksuids, in fact, it outputs valid ksuids. The difference
+is that it sacrifices one byte of the random payload in favor of this accuracy.
+The code too is fully compatible: ``` pip install svix-ksuid ``` ```python from
+ksuid import KsuidMs ksuid = KsuidMs() ``` ## Examples ### Default ksuid
+Generate a ksuid without passing a specific datetime ```python In [1]: from
+ksuid import Ksuid In [2]: ksuid = Ksuid() In [3]: f"Base62: {ksuid}" Out[3]:
+'Base62: 1srOrx2ZWZBpBUvZwXKQmoEYga2' In [4]: f"Bytes: {bytes(ksuid)}" Out[4]:
+"Bytes: b'\\r5\\xc43\\xe1\\x93>7\\xf2up\\x87c\\xad\\xc7tZ\\xf5\\xe7\\xf2'" In
+[5]: f"Datetime: {ksuid.datetime}" Out[5]: 'Datetime: 2021-05-21 14:04:03' In
+[6]: f"Timestamp: {ksuid.timestamp}" Out[6]: 'Timestamp: 1621627443' In [7]:
 f"Payload: {ksuid.payload}" Out[7]: "Payload:
 b'\\xe1\\x93>7\\xf2up\\x87c\\xad\\xc7tZ\\xf5\\xe7\\xf2'" ``` ### ksuid from
-datetime ``` In [1]: datetime = datetime(year=2021, month=5, day=19, hour=1,
-minute=1, second=1, microsecond=1) In [2]: datetime Out[2]: datetime.datetime
-(2021, 5, 19, 1, 1, 1, 1) In [3]: ksuid = Ksuid(datetime) In [4]:
-ksuid.datetime Out[4]: datetime.datetime(2021, 5, 19, 1, 1, 1) In [5]:
-ksuid.timestamp Out[5]: 1621407661 ``` ### ksuid from base62 ``` In [1]: ksuid
-= Ksuid() In [2]: ksuid.timestamp Out[2]: 1621634852 In [3]: f"Base62: {ksuid}"
-Out[3]: 'Base62: 1srdszO8Xy2cR6CnARnvxCfRmK4' In [4]: ksuid_from_base62 =
-Ksuid.from_base62("1srdszO8Xy2cR6CnARnvxCfRmK4") In [5]:
-ksuid_from_base62.timestamp Out[5]: 1621634852 ``` ### ksuid from bytes ``` In
-[1]: ksuid = Ksuid() In [2]: ksuid_from_bytes = ksuid.from_bytes(bytes(ksuid))
-In [3]: f"ksuid: {ksuid}, ksuid_from_bytes: {ksuid_from_bytes}" Out[3]: 'ksuid:
-1sreAHoz6myPhXghsOdVBoec3Vr, ksuid_from_bytes: 1sreAHoz6myPhXghsOdVBoec3Vr' In
-[4]: ksuid == ksuid_from_bytes Out[4]: True ``` ### Compare ksuid(s) ``` In
-[1]: ksuid_1 = Ksuid() In [2]: ksuid_2 = Ksuid.from_bytes(bytes(ksuid_1)) In
-[3]: f"ksuid_1: {ksuid_1}, ksuid_2: {ksuid_2}" Out[3]: 'ksuid_1:
-1sreAHoz6myPhXghsOdVBoec3Vr, ksuid_2: 1sreAHoz6myPhXghsOdVBoec3Vr' In [4]:
-ksuid_1 == ksuid_2 Out[4]: True In [5]: ksuid_1 Out[5]:
-1tM9eRSTrHIrrH5SMEW24rtvIOF In [6]: ksuid_2 Out[6]: 1tM9eRSTrHIrrH5SMEW24rtvIOF
-``` ### Order of ksuid(s) ``` In [1]: ksuid_1 = Ksuid() In [2]:
-ksuid_1.timestamp Out[2]: 1621963256 In [3]: ksuid_2 = Ksuid() In [4]:
-ksuid_2.timestamp Out[4]: 1621963266 In [5]: ksuid_1 < ksuid_2 Out[5]: True In
-[6]: ksuid_1 <= ksuid_2 Out[6]: True In [7]: ksuid_1 >= ksuid_2 Out[7]: False
-In [8]: ksuid_1 > ksuid_2 Out[8]: False ``` ### License ksuid source code is
-available under an MIT [License](./LICENSE).
+datetime ```python In [1]: datetime = datetime(year=2021, month=5, day=19,
+hour=1, minute=1, second=1, microsecond=1) In [2]: datetime Out[2]:
+datetime.datetime(2021, 5, 19, 1, 1, 1, 1) In [3]: ksuid = Ksuid(datetime) In
+[4]: ksuid.datetime Out[4]: datetime.datetime(2021, 5, 19, 1, 1, 1) In [5]:
+ksuid.timestamp Out[5]: 1621407661 ``` ### ksuid from base62 ```python In [1]:
+ksuid = Ksuid() In [2]: ksuid.timestamp Out[2]: 1621634852 In [3]: f"Base62:
+{ksuid}" Out[3]: 'Base62: 1srdszO8Xy2cR6CnARnvxCfRmK4' In [4]:
+ksuid_from_base62 = Ksuid.from_base62("1srdszO8Xy2cR6CnARnvxCfRmK4") In [5]:
+ksuid_from_base62.timestamp Out[5]: 1621634852 ``` ### ksuid from bytes
+```python In [1]: ksuid = Ksuid() In [2]: ksuid_from_bytes = ksuid.from_bytes
+(bytes(ksuid)) In [3]: f"ksuid: {ksuid}, ksuid_from_bytes: {ksuid_from_bytes}"
+Out[3]: 'ksuid: 1sreAHoz6myPhXghsOdVBoec3Vr, ksuid_from_bytes:
+1sreAHoz6myPhXghsOdVBoec3Vr' In [4]: ksuid == ksuid_from_bytes Out[4]: True ```
+### Compare ksuid(s) ```python In [1]: ksuid_1 = Ksuid() In [2]: ksuid_2 =
+Ksuid.from_bytes(bytes(ksuid_1)) In [3]: f"ksuid_1: {ksuid_1}, ksuid_2:
+{ksuid_2}" Out[3]: 'ksuid_1: 1sreAHoz6myPhXghsOdVBoec3Vr, ksuid_2:
+1sreAHoz6myPhXghsOdVBoec3Vr' In [4]: ksuid_1 == ksuid_2 Out[4]: True In [5]:
+ksuid_1 Out[5]: 1tM9eRSTrHIrrH5SMEW24rtvIOF In [6]: ksuid_2 Out[6]:
+1tM9eRSTrHIrrH5SMEW24rtvIOF ``` ### Order of ksuid(s) ```python In [1]: ksuid_1
+= Ksuid() In [2]: ksuid_1.timestamp Out[2]: 1621963256 In [3]: ksuid_2 = Ksuid
+() In [4]: ksuid_2.timestamp Out[4]: 1621963266 In [5]: ksuid_1 < ksuid_2 Out
+[5]: True In [6]: ksuid_1 <= ksuid_2 Out[6]: True In [7]: ksuid_1 >= ksuid_2
+Out[7]: False In [8]: ksuid_1 > ksuid_2 Out[8]: False ``` ### License ksuid
+source code is available under an MIT [License](./LICENSE).
```

### Comparing `svix-ksuid-0.6.0/ksuid/ksuid.py` & `svix-ksuid-0.6.1/ksuid/ksuid.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     def datetime(self) -> datetime:
         unix_time = self.timestamp
 
         return datetime.fromtimestamp(unix_time, tz=timezone.utc)
 
     @property
     def timestamp(self) -> float:
-        return int.from_bytes(self._uid[: self.TIMESTAMP_LENGTH_IN_BYTES], "big") + EPOCH_STAMP
+        return float(int.from_bytes(self._uid[: self.TIMESTAMP_LENGTH_IN_BYTES], "big") + EPOCH_STAMP)
 
     @property
     def payload(self) -> bytes:
         """Returns the payload of the Ksuid with the timestamp encoded portion removed"""
 
         return self._uid[self.TIMESTAMP_LENGTH_IN_BYTES :]
 
@@ -125,9 +125,10 @@
         timestamp = round((dt.timestamp() - EPOCH_STAMP) * self.TIMESTAMP_MULTIPLIER)
 
         return int.to_bytes(timestamp, self.TIMESTAMP_LENGTH_IN_BYTES, "big") + payload
 
     @property
     def timestamp(self) -> float:
         return (
-            int.from_bytes(self._uid[: self.TIMESTAMP_LENGTH_IN_BYTES], "big") / self.TIMESTAMP_MULTIPLIER
-        ) + EPOCH_STAMP
+            float(int.from_bytes(self._uid[: self.TIMESTAMP_LENGTH_IN_BYTES], "big")) / self.TIMESTAMP_MULTIPLIER
+            + EPOCH_STAMP
+        )
```

### Comparing `svix-ksuid-0.6.0/setup.py` & `svix-ksuid-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import find_packages, setup  # noqa: H301
 
 NAME = "svix-ksuid"
-VERSION = "0.6.0"
+VERSION = "0.6.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `svix-ksuid-0.6.0/svix_ksuid.egg-info/PKG-INFO` & `svix-ksuid-0.6.1/svix_ksuid.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: svix-ksuid
-Version: 0.6.0
+Version: 0.6.1
 Summary:  A pure-Python KSUID implementation
 Home-page: https://github.com/svixhq/python-ksuid/
 Author: Svix
 Author-email: development@svix.com
 License: MIT
 Keywords: svix,ksuid
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -30,39 +29,41 @@
 <h1 align="center">
   <a href="https://www.svix.com">
     <img width="120" src="https://avatars.githubusercontent.com/u/80175132?s=200&v=4" />
     <p align="center">Svix - Webhooks as a service</p>
   </a>
 </h1>
 
-# Svix-KSUID
+# Svix-KSUID (Python)
 
 ![API-Lint](https://github.com/svixhq/python-ksuid/workflows/lint/badge.svg)
 ![Frontend-Lint](https://github.com/svixhq/python-ksuid/workflows/test/badge.svg)
 ![GitHub tag](https://img.shields.io/github/tag/svixhq/python-ksuid.svg)
 [![PyPI](https://img.shields.io/pypi/v/svix-ksuid.svg)](https://pypi.python.org/pypi/svix-ksuid/)
 [![Join our slack](https://img.shields.io/badge/Slack-join%20the%20community-blue?logo=slack&style=social)](https://www.svix.com/slack/)
 
 This library is inspired by [Segment's KSUID](https://segment.com/blog/a-brief-history-of-the-uuid/) implementation:
 https://github.com/segmentio/ksuid
 
+For the Rust version, please check out https://github.com/svix/rust-ksuid
+
 ## What is a ksuid?
 
 A ksuid is a K sorted UID. In other words, a KSUID also stores a date component, so that ksuids can be approximately 
 sorted based on the time they were created. 
 
 Read more [here](https://segment.com/blog/a-brief-history-of-the-uuid/).
 
 ## Usage
 
 ```
 pip install svix-ksuid
 ```
 
-```
+```python
 from ksuid import Ksuid
 
 ksuid = Ksuid()
 ```
 
 ### Higher timestamp accuracy mode
 
@@ -72,27 +73,27 @@
 
 The code too is fully compatible:
 
 ```
 pip install svix-ksuid
 ```
 
-```
+```python
 from ksuid import KsuidMs
 
 ksuid = KsuidMs()
 ```
 
 ## Examples
 
 ### Default ksuid
 
 Generate a ksuid without passing a specific datetime
 
-```
+```python
 In [1]: from ksuid import Ksuid
 
 In [2]: ksuid = Ksuid()
 
 In [3]: f"Base62: {ksuid}"
 Out[3]: 'Base62: 1srOrx2ZWZBpBUvZwXKQmoEYga2'
 
@@ -107,15 +108,15 @@
 
 In [7]: f"Payload: {ksuid.payload}"
 Out[7]: "Payload: b'\\xe1\\x93>7\\xf2up\\x87c\\xad\\xc7tZ\\xf5\\xe7\\xf2'"
 ```
 
 ### ksuid from datetime
 
-```
+```python
 In [1]: datetime = datetime(year=2021, month=5, day=19, hour=1, minute=1, second=1, microsecond=1)
 
 In [2]: datetime
 Out[2]: datetime.datetime(2021, 5, 19, 1, 1, 1, 1)
 
 In [3]: ksuid = Ksuid(datetime)
 
@@ -124,15 +125,15 @@
 
 In [5]: ksuid.timestamp
 Out[5]: 1621407661
 ```
 
 ### ksuid from base62
 
-```
+```python
 In [1]: ksuid = Ksuid()
 
 In [2]: ksuid.timestamp
 Out[2]: 1621634852
 
 In [3]: f"Base62: {ksuid}"
 Out[3]: 'Base62: 1srdszO8Xy2cR6CnARnvxCfRmK4'
@@ -141,29 +142,29 @@
 
 In [5]: ksuid_from_base62.timestamp
 Out[5]: 1621634852
 ```
 
 ### ksuid from bytes
 
-```
+```python
 In [1]: ksuid = Ksuid()
 
 In [2]: ksuid_from_bytes = ksuid.from_bytes(bytes(ksuid))
 
 In [3]: f"ksuid: {ksuid}, ksuid_from_bytes: {ksuid_from_bytes}"
 Out[3]: 'ksuid: 1sreAHoz6myPhXghsOdVBoec3Vr, ksuid_from_bytes: 1sreAHoz6myPhXghsOdVBoec3Vr'
 
 In [4]: ksuid == ksuid_from_bytes
 Out[4]: True
 ```
 
 ### Compare ksuid(s)
 
-```
+```python
 In [1]: ksuid_1 = Ksuid()
 
 In [2]: ksuid_2 = Ksuid.from_bytes(bytes(ksuid_1))
 
 In [3]: f"ksuid_1: {ksuid_1}, ksuid_2: {ksuid_2}"
 Out[3]: 'ksuid_1: 1sreAHoz6myPhXghsOdVBoec3Vr, ksuid_2: 1sreAHoz6myPhXghsOdVBoec3Vr'
 
@@ -176,15 +177,15 @@
 In [6]: ksuid_2
 Out[6]: 1tM9eRSTrHIrrH5SMEW24rtvIOF
 ```
 
 
 ### Order of ksuid(s)
 
-```
+```python
 In [1]: ksuid_1 = Ksuid()
 
 In [2]: ksuid_1.timestamp
 Out[2]: 1621963256
 
 In [3]: ksuid_2 = Ksuid()
 
@@ -203,9 +204,7 @@
 In [8]: ksuid_1 > ksuid_2
 Out[8]: False
 ```
 
 ### License
 
 ksuid source code is available under an MIT [License](./LICENSE).
-
-
```

#### html2text {}

```diff
@@ -1,69 +1,70 @@
-Metadata-Version: 2.1 Name: svix-ksuid Version: 0.6.0 Summary: A pure-Python
+Metadata-Version: 2.1 Name: svix-ksuid Version: 0.6.1 Summary: A pure-Python
 KSUID implementation Home-page: https://github.com/svixhq/python-ksuid/ Author:
 Svix Author-email: development@svix.com License: MIT Keywords: svix,ksuid
-Platform: UNKNOWN Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Information Technology Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python Classifier: Topic :: Software Development ::
-Libraries :: Application Frameworks Classifier: Topic :: Software Development
-:: Libraries :: Python Modules Classifier: Topic :: Software Development ::
-Libraries Classifier: Topic :: Software Development Classifier: Typing :: Typed
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Information Technology Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python Classifier: Topic :: Software Development :: Libraries ::
+Application Frameworks Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development Classifier: Typing :: Typed
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE
          [https://avatars.githubusercontent.com/u/80175132?s=200&v=4]
                          Svix_-_Webhooks_as_a_service
-# Svix-KSUID ![API-Lint](https://github.com/svixhq/python-ksuid/workflows/lint/
-badge.svg) ![Frontend-Lint](https://github.com/svixhq/python-ksuid/workflows/
-test/badge.svg) ![GitHub tag](https://img.shields.io/github/tag/svixhq/python-
-ksuid.svg) [![PyPI](https://img.shields.io/pypi/v/svix-ksuid.svg)](https://
-pypi.python.org/pypi/svix-ksuid/) [![Join our slack](https://img.shields.io/
-badge/Slack-join%20the%20community-blue?logo=slack&style=social)](https://
-www.svix.com/slack/) This library is inspired by [Segment's KSUID](https://
-segment.com/blog/a-brief-history-of-the-uuid/) implementation: https://
-github.com/segmentio/ksuid ## What is a ksuid? A ksuid is a K sorted UID. In
-other words, a KSUID also stores a date component, so that ksuids can be
-approximately sorted based on the time they were created. Read more [here]
-(https://segment.com/blog/a-brief-history-of-the-uuid/). ## Usage ``` pip
-install svix-ksuid ``` ``` from ksuid import Ksuid ksuid = Ksuid() ``` ###
-Higher timestamp accuracy mode Ksuids have a 1 second accuracy which is not
-sufficient for all use-cases. That's why this library exposes a higher accuracy
-mode which supports accuracy of up to 4ms. It's fully compatible with normal
-ksuids, in fact, it outputs valid ksuids. The difference is that it sacrifices
-one byte of the random payload in favor of this accuracy. The code too is fully
-compatible: ``` pip install svix-ksuid ``` ``` from ksuid import KsuidMs ksuid
-= KsuidMs() ``` ## Examples ### Default ksuid Generate a ksuid without passing
-a specific datetime ``` In [1]: from ksuid import Ksuid In [2]: ksuid = Ksuid()
-In [3]: f"Base62: {ksuid}" Out[3]: 'Base62: 1srOrx2ZWZBpBUvZwXKQmoEYga2' In
-[4]: f"Bytes: {bytes(ksuid)}" Out[4]: "Bytes:
-b'\\r5\\xc43\\xe1\\x93>7\\xf2up\\x87c\\xad\\xc7tZ\\xf5\\xe7\\xf2'" In [5]:
-f"Datetime: {ksuid.datetime}" Out[5]: 'Datetime: 2021-05-21 14:04:03' In [6]:
-f"Timestamp: {ksuid.timestamp}" Out[6]: 'Timestamp: 1621627443' In [7]:
+# Svix-KSUID (Python) ![API-Lint](https://github.com/svixhq/python-ksuid/
+workflows/lint/badge.svg) ![Frontend-Lint](https://github.com/svixhq/python-
+ksuid/workflows/test/badge.svg) ![GitHub tag](https://img.shields.io/github/
+tag/svixhq/python-ksuid.svg) [![PyPI](https://img.shields.io/pypi/v/svix-
+ksuid.svg)](https://pypi.python.org/pypi/svix-ksuid/) [![Join our slack](https:
+//img.shields.io/badge/Slack-join%20the%20community-
+blue?logo=slack&style=social)](https://www.svix.com/slack/) This library is
+inspired by [Segment's KSUID](https://segment.com/blog/a-brief-history-of-the-
+uuid/) implementation: https://github.com/segmentio/ksuid For the Rust version,
+please check out https://github.com/svix/rust-ksuid ## What is a ksuid? A ksuid
+is a K sorted UID. In other words, a KSUID also stores a date component, so
+that ksuids can be approximately sorted based on the time they were created.
+Read more [here](https://segment.com/blog/a-brief-history-of-the-uuid/). ##
+Usage ``` pip install svix-ksuid ``` ```python from ksuid import Ksuid ksuid =
+Ksuid() ``` ### Higher timestamp accuracy mode Ksuids have a 1 second accuracy
+which is not sufficient for all use-cases. That's why this library exposes a
+higher accuracy mode which supports accuracy of up to 4ms. It's fully
+compatible with normal ksuids, in fact, it outputs valid ksuids. The difference
+is that it sacrifices one byte of the random payload in favor of this accuracy.
+The code too is fully compatible: ``` pip install svix-ksuid ``` ```python from
+ksuid import KsuidMs ksuid = KsuidMs() ``` ## Examples ### Default ksuid
+Generate a ksuid without passing a specific datetime ```python In [1]: from
+ksuid import Ksuid In [2]: ksuid = Ksuid() In [3]: f"Base62: {ksuid}" Out[3]:
+'Base62: 1srOrx2ZWZBpBUvZwXKQmoEYga2' In [4]: f"Bytes: {bytes(ksuid)}" Out[4]:
+"Bytes: b'\\r5\\xc43\\xe1\\x93>7\\xf2up\\x87c\\xad\\xc7tZ\\xf5\\xe7\\xf2'" In
+[5]: f"Datetime: {ksuid.datetime}" Out[5]: 'Datetime: 2021-05-21 14:04:03' In
+[6]: f"Timestamp: {ksuid.timestamp}" Out[6]: 'Timestamp: 1621627443' In [7]:
 f"Payload: {ksuid.payload}" Out[7]: "Payload:
 b'\\xe1\\x93>7\\xf2up\\x87c\\xad\\xc7tZ\\xf5\\xe7\\xf2'" ``` ### ksuid from
-datetime ``` In [1]: datetime = datetime(year=2021, month=5, day=19, hour=1,
-minute=1, second=1, microsecond=1) In [2]: datetime Out[2]: datetime.datetime
-(2021, 5, 19, 1, 1, 1, 1) In [3]: ksuid = Ksuid(datetime) In [4]:
-ksuid.datetime Out[4]: datetime.datetime(2021, 5, 19, 1, 1, 1) In [5]:
-ksuid.timestamp Out[5]: 1621407661 ``` ### ksuid from base62 ``` In [1]: ksuid
-= Ksuid() In [2]: ksuid.timestamp Out[2]: 1621634852 In [3]: f"Base62: {ksuid}"
-Out[3]: 'Base62: 1srdszO8Xy2cR6CnARnvxCfRmK4' In [4]: ksuid_from_base62 =
-Ksuid.from_base62("1srdszO8Xy2cR6CnARnvxCfRmK4") In [5]:
-ksuid_from_base62.timestamp Out[5]: 1621634852 ``` ### ksuid from bytes ``` In
-[1]: ksuid = Ksuid() In [2]: ksuid_from_bytes = ksuid.from_bytes(bytes(ksuid))
-In [3]: f"ksuid: {ksuid}, ksuid_from_bytes: {ksuid_from_bytes}" Out[3]: 'ksuid:
-1sreAHoz6myPhXghsOdVBoec3Vr, ksuid_from_bytes: 1sreAHoz6myPhXghsOdVBoec3Vr' In
-[4]: ksuid == ksuid_from_bytes Out[4]: True ``` ### Compare ksuid(s) ``` In
-[1]: ksuid_1 = Ksuid() In [2]: ksuid_2 = Ksuid.from_bytes(bytes(ksuid_1)) In
-[3]: f"ksuid_1: {ksuid_1}, ksuid_2: {ksuid_2}" Out[3]: 'ksuid_1:
-1sreAHoz6myPhXghsOdVBoec3Vr, ksuid_2: 1sreAHoz6myPhXghsOdVBoec3Vr' In [4]:
-ksuid_1 == ksuid_2 Out[4]: True In [5]: ksuid_1 Out[5]:
-1tM9eRSTrHIrrH5SMEW24rtvIOF In [6]: ksuid_2 Out[6]: 1tM9eRSTrHIrrH5SMEW24rtvIOF
-``` ### Order of ksuid(s) ``` In [1]: ksuid_1 = Ksuid() In [2]:
-ksuid_1.timestamp Out[2]: 1621963256 In [3]: ksuid_2 = Ksuid() In [4]:
-ksuid_2.timestamp Out[4]: 1621963266 In [5]: ksuid_1 < ksuid_2 Out[5]: True In
-[6]: ksuid_1 <= ksuid_2 Out[6]: True In [7]: ksuid_1 >= ksuid_2 Out[7]: False
-In [8]: ksuid_1 > ksuid_2 Out[8]: False ``` ### License ksuid source code is
-available under an MIT [License](./LICENSE).
+datetime ```python In [1]: datetime = datetime(year=2021, month=5, day=19,
+hour=1, minute=1, second=1, microsecond=1) In [2]: datetime Out[2]:
+datetime.datetime(2021, 5, 19, 1, 1, 1, 1) In [3]: ksuid = Ksuid(datetime) In
+[4]: ksuid.datetime Out[4]: datetime.datetime(2021, 5, 19, 1, 1, 1) In [5]:
+ksuid.timestamp Out[5]: 1621407661 ``` ### ksuid from base62 ```python In [1]:
+ksuid = Ksuid() In [2]: ksuid.timestamp Out[2]: 1621634852 In [3]: f"Base62:
+{ksuid}" Out[3]: 'Base62: 1srdszO8Xy2cR6CnARnvxCfRmK4' In [4]:
+ksuid_from_base62 = Ksuid.from_base62("1srdszO8Xy2cR6CnARnvxCfRmK4") In [5]:
+ksuid_from_base62.timestamp Out[5]: 1621634852 ``` ### ksuid from bytes
+```python In [1]: ksuid = Ksuid() In [2]: ksuid_from_bytes = ksuid.from_bytes
+(bytes(ksuid)) In [3]: f"ksuid: {ksuid}, ksuid_from_bytes: {ksuid_from_bytes}"
+Out[3]: 'ksuid: 1sreAHoz6myPhXghsOdVBoec3Vr, ksuid_from_bytes:
+1sreAHoz6myPhXghsOdVBoec3Vr' In [4]: ksuid == ksuid_from_bytes Out[4]: True ```
+### Compare ksuid(s) ```python In [1]: ksuid_1 = Ksuid() In [2]: ksuid_2 =
+Ksuid.from_bytes(bytes(ksuid_1)) In [3]: f"ksuid_1: {ksuid_1}, ksuid_2:
+{ksuid_2}" Out[3]: 'ksuid_1: 1sreAHoz6myPhXghsOdVBoec3Vr, ksuid_2:
+1sreAHoz6myPhXghsOdVBoec3Vr' In [4]: ksuid_1 == ksuid_2 Out[4]: True In [5]:
+ksuid_1 Out[5]: 1tM9eRSTrHIrrH5SMEW24rtvIOF In [6]: ksuid_2 Out[6]:
+1tM9eRSTrHIrrH5SMEW24rtvIOF ``` ### Order of ksuid(s) ```python In [1]: ksuid_1
+= Ksuid() In [2]: ksuid_1.timestamp Out[2]: 1621963256 In [3]: ksuid_2 = Ksuid
+() In [4]: ksuid_2.timestamp Out[4]: 1621963266 In [5]: ksuid_1 < ksuid_2 Out
+[5]: True In [6]: ksuid_1 <= ksuid_2 Out[6]: True In [7]: ksuid_1 >= ksuid_2
+Out[7]: False In [8]: ksuid_1 > ksuid_2 Out[8]: False ``` ### License ksuid
+source code is available under an MIT [License](./LICENSE).
```

