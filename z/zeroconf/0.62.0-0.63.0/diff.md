# Comparing `tmp/zeroconf-0.62.0.tar.gz` & `tmp/zeroconf-0.63.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroconf-0.62.0.tar", max compression
+gzip compressed data, was "zeroconf-0.63.0.tar", max compression
```

## Comparing `zeroconf-0.62.0.tar` & `zeroconf-0.63.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    50964 2023-05-04 00:48:01.431215 zeroconf-0.62.0/CHANGELOG.md
--rw-r--r--   0        0        0    24380 2023-05-04 00:48:00.591214 zeroconf-0.62.0/COPYING
--rw-r--r--   0        0        0     4407 2023-05-04 00:48:00.595214 zeroconf-0.62.0/README.rst
--rw-r--r--   0        0        0     1060 2023-05-04 00:48:00.595214 zeroconf-0.62.0/build_ext.py
--rw-r--r--   0        0        0     6770 2023-05-04 00:48:00.595214 zeroconf-0.62.0/docs/Makefile
--rw-r--r--   0        0        0      234 2023-05-04 00:48:00.595214 zeroconf-0.62.0/docs/api.rst
--rw-r--r--   0        0        0     8145 2023-05-04 00:48:00.595214 zeroconf-0.62.0/docs/conf.py
--rw-r--r--   0        0        0      991 2023-05-04 00:48:00.595214 zeroconf-0.62.0/docs/index.rst
--rw-r--r--   0        0        0     3995 2023-05-04 00:48:01.511215 zeroconf-0.62.0/pyproject.toml
--rw-r--r--   0        0        0     3868 2023-05-04 00:48:01.443215 zeroconf-0.62.0/src/zeroconf/__init__.py
--rw-r--r--   0        0        0      511 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_cache.pxd
--rw-r--r--   0        0        0     8493 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_cache.py
--rw-r--r--   0        0        0    39043 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_core.py
--rw-r--r--   0        0        0     2061 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_dns.pxd
--rw-r--r--   0        0        0    18218 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_dns.py
--rw-r--r--   0        0        0     2167 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_exceptions.py
--rw-r--r--   0        0        0    25863 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_handlers.py
--rw-r--r--   0        0        0     2916 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_history.py
--rw-r--r--   0        0        0     2980 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_logger.py
--rw-r--r--   0        0        0      971 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_protocol/__init__.py
--rw-r--r--   0        0        0     2573 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_protocol/incoming.pxd
--rw-r--r--   0        0        0    13999 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_protocol/incoming.py
--rw-r--r--   0        0        0     1950 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_protocol/outgoing.pxd
--rw-r--r--   0        0        0    17758 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_protocol/outgoing.py
--rw-r--r--   0        0        0     2355 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_services/__init__.py
--rw-r--r--   0        0        0    22413 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_services/browser.py
--rw-r--r--   0        0        0    25364 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_services/info.py
--rw-r--r--   0        0        0     3964 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_services/registry.py
--rw-r--r--   0        0        0     3003 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_services/types.py
--rw-r--r--   0        0        0     2909 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_updates.py
--rw-r--r--   0        0        0      971 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_utils/__init__.py
--rw-r--r--   0        0        0     4144 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_utils/asyncio.py
--rw-r--r--   0        0        0     6904 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_utils/name.py
--rw-r--r--   0        0        0    15252 2023-05-04 00:48:00.595214 zeroconf-0.62.0/src/zeroconf/_utils/net.py
--rw-r--r--   0        0        0     1308 2023-05-04 00:48:00.599214 zeroconf-0.62.0/src/zeroconf/_utils/time.py
--rw-r--r--   0        0        0    11084 2023-05-04 00:48:00.599214 zeroconf-0.62.0/src/zeroconf/asyncio.py
--rw-r--r--   0        0        0     4469 2023-05-04 00:48:00.599214 zeroconf-0.62.0/src/zeroconf/const.py
--rw-r--r--   0        0        0        0 2023-05-04 00:48:00.599214 zeroconf-0.62.0/src/zeroconf/py.typed
--rw-r--r--   0        0        0     2416 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/__init__.py
--rw-r--r--   0        0        0      668 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/conftest.py
--rw-r--r--   0        0        0      971 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/services/__init__.py
--rw-r--r--   0        0        0    42950 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/services/test_browser.py
--rw-r--r--   0        0        0    45244 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/services/test_info.py
--rw-r--r--   0        0        0     4923 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/services/test_registry.py
--rw-r--r--   0        0        0     6273 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/services/test_types.py
--rw-r--r--   0        0        0    45016 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_asyncio.py
--rw-r--r--   0        0        0     8830 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_cache.py
--rw-r--r--   0        0        0    29468 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_core.py
--rw-r--r--   0        0        0    14686 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_dns.py
--rw-r--r--   0        0        0     5022 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_exceptions.py
--rw-r--r--   0        0        0    63127 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_handlers.py
--rw-r--r--   0        0        0     2580 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_history.py
--rw-r--r--   0        0        0     6640 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_init.py
--rw-r--r--   0        0        0     3396 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_logger.py
--rw-r--r--   0        0        0    41672 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_protocol.py
--rw-r--r--   0        0        0     9477 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_services.py
--rw-r--r--   0        0        0     2240 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/test_updates.py
--rw-r--r--   0        0        0      971 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     5101 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/utils/test_asyncio.py
--rw-r--r--   0        0        0     2045 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/utils/test_name.py
--rw-r--r--   0        0        0     9413 2023-05-04 00:48:00.599214 zeroconf-0.62.0/tests/utils/test_net.py
--rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.62.0/setup.py
--rw-r--r--   0        0        0     6297 1970-01-01 00:00:00.000000 zeroconf-0.62.0/PKG-INFO
+-rw-r--r--   0        0        0    51686 2023-05-25 13:00:19.908389 zeroconf-0.63.0/CHANGELOG.md
+-rw-r--r--   0        0        0    24380 2023-05-25 13:00:19.112391 zeroconf-0.63.0/COPYING
+-rw-r--r--   0        0        0     4407 2023-05-25 13:00:19.112391 zeroconf-0.63.0/README.rst
+-rw-r--r--   0        0        0     1060 2023-05-25 13:00:19.112391 zeroconf-0.63.0/build_ext.py
+-rw-r--r--   0        0        0     6770 2023-05-25 13:00:19.112391 zeroconf-0.63.0/docs/Makefile
+-rw-r--r--   0        0        0      234 2023-05-25 13:00:19.112391 zeroconf-0.63.0/docs/api.rst
+-rw-r--r--   0        0        0     8145 2023-05-25 13:00:19.112391 zeroconf-0.63.0/docs/conf.py
+-rw-r--r--   0        0        0      991 2023-05-25 13:00:19.112391 zeroconf-0.63.0/docs/index.rst
+-rw-r--r--   0        0        0     3995 2023-05-25 13:00:19.996389 zeroconf-0.63.0/pyproject.toml
+-rw-r--r--   0        0        0     3868 2023-05-25 13:00:19.928389 zeroconf-0.63.0/src/zeroconf/__init__.py
+-rw-r--r--   0        0        0      545 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_cache.pxd
+-rw-r--r--   0        0        0     8567 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_cache.py
+-rw-r--r--   0        0        0    39051 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_core.py
+-rw-r--r--   0        0        0     2061 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_dns.pxd
+-rw-r--r--   0        0        0    18218 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_dns.py
+-rw-r--r--   0        0        0     2167 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_exceptions.py
+-rw-r--r--   0        0        0    25955 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_handlers.py
+-rw-r--r--   0        0        0     2916 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_history.py
+-rw-r--r--   0        0        0     2980 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_logger.py
+-rw-r--r--   0        0        0      971 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_protocol/__init__.py
+-rw-r--r--   0        0        0     2573 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_protocol/incoming.pxd
+-rw-r--r--   0        0        0    13999 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_protocol/incoming.py
+-rw-r--r--   0        0        0     1950 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_protocol/outgoing.pxd
+-rw-r--r--   0        0        0    17758 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_protocol/outgoing.py
+-rw-r--r--   0        0        0     2355 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_services/__init__.py
+-rw-r--r--   0        0        0    22413 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_services/browser.py
+-rw-r--r--   0        0        0    25426 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_services/info.py
+-rw-r--r--   0        0        0     3948 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_services/registry.py
+-rw-r--r--   0        0        0     3003 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_services/types.py
+-rw-r--r--   0        0        0     2909 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_updates.py
+-rw-r--r--   0        0        0      971 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_utils/__init__.py
+-rw-r--r--   0        0        0     4144 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_utils/asyncio.py
+-rw-r--r--   0        0        0     6904 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_utils/name.py
+-rw-r--r--   0        0        0    15252 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_utils/net.py
+-rw-r--r--   0        0        0     1308 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_utils/time.py
+-rw-r--r--   0        0        0    11084 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/asyncio.py
+-rw-r--r--   0        0        0     4469 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/const.py
+-rw-r--r--   0        0        0        0 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/py.typed
+-rw-r--r--   0        0        0     2416 2023-05-25 13:00:19.116391 zeroconf-0.63.0/tests/__init__.py
+-rw-r--r--   0        0        0      668 2023-05-25 13:00:19.116391 zeroconf-0.63.0/tests/conftest.py
+-rw-r--r--   0        0        0      971 2023-05-25 13:00:19.116391 zeroconf-0.63.0/tests/services/__init__.py
+-rw-r--r--   0        0        0    42950 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/services/test_browser.py
+-rw-r--r--   0        0        0    45244 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/services/test_info.py
+-rw-r--r--   0        0        0     4157 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/services/test_registry.py
+-rw-r--r--   0        0        0     6273 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/services/test_types.py
+-rw-r--r--   0        0        0    45016 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_asyncio.py
+-rw-r--r--   0        0        0     8830 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_cache.py
+-rw-r--r--   0        0        0    29468 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_core.py
+-rw-r--r--   0        0        0    14686 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_dns.py
+-rw-r--r--   0        0        0     5022 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0    67458 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_handlers.py
+-rw-r--r--   0        0        0     2580 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_history.py
+-rw-r--r--   0        0        0     6640 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_init.py
+-rw-r--r--   0        0        0     3396 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_logger.py
+-rw-r--r--   0        0        0    41672 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_protocol.py
+-rw-r--r--   0        0        0     9477 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_services.py
+-rw-r--r--   0        0        0     2240 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_updates.py
+-rw-r--r--   0        0        0      971 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     5101 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/utils/test_asyncio.py
+-rw-r--r--   0        0        0     2045 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/utils/test_name.py
+-rw-r--r--   0        0        0     9413 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/utils/test_net.py
+-rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.63.0/setup.py
+-rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 zeroconf-0.63.0/PKG-INFO
```

### Comparing `zeroconf-0.62.0/CHANGELOG.md` & `zeroconf-0.63.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.63.0 (2023-05-25)
+### Feature
+* Small speed up to fetch dns addresses from ServiceInfo ([#1176](https://github.com/python-zeroconf/python-zeroconf/issues/1176)) ([`4deaa6e`](https://github.com/python-zeroconf/python-zeroconf/commit/4deaa6ed7c9161db55bf16ec068ab7260bbd4976))
+* Speed up the service registry ([#1174](https://github.com/python-zeroconf/python-zeroconf/issues/1174)) ([`360ceb2`](https://github.com/python-zeroconf/python-zeroconf/commit/360ceb2548c4c4974ff798aac43a6fff9803ea0e))
+* Improve dns cache performance ([#1172](https://github.com/python-zeroconf/python-zeroconf/issues/1172)) ([`bb496a1`](https://github.com/python-zeroconf/python-zeroconf/commit/bb496a1dd5fa3562c0412cb064d14639a542592e))
+
 ## v0.62.0 (2023-05-04)
 ### Feature
 * Improve performance of ServiceBrowser outgoing query scheduler ([#1170](https://github.com/python-zeroconf/python-zeroconf/issues/1170)) ([`963d022`](https://github.com/python-zeroconf/python-zeroconf/commit/963d022ef82b615540fa7521d164a98a6c6f5209))
 
 ## v0.61.0 (2023-05-03)
 ### Feature
 * Speed up parsing NSEC records ([#1169](https://github.com/python-zeroconf/python-zeroconf/issues/1169)) ([`06fa94d`](https://github.com/python-zeroconf/python-zeroconf/commit/06fa94d87b4f0451cb475a921ce1d8e9562e0f26))
```

### Comparing `zeroconf-0.62.0/COPYING` & `zeroconf-0.63.0/COPYING`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/README.rst` & `zeroconf-0.63.0/README.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/build_ext.py` & `zeroconf-0.63.0/build_ext.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/docs/Makefile` & `zeroconf-0.63.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/docs/conf.py` & `zeroconf-0.63.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/docs/index.rst` & `zeroconf-0.63.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/pyproject.toml` & `zeroconf-0.63.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeroconf"
-version = "0.62.0"
+version = "0.63.0"
 description = "A pure python implementation of multicast DNS service discovery"
 authors = ["Paul Scott-Murphy", "William McBrine", "Jakub Stasiak", "J. Nick Koston"]
 license = "LGPL"
 readme = "README.rst"
 repository = "https://github.com/python-zeroconf/python-zeroconf"
 documentation = "https://python-zeroconf.readthedocs.io"
 classifiers=[
```

### Comparing `zeroconf-0.62.0/src/zeroconf/__init__.py` & `zeroconf-0.63.0/src/zeroconf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 from ._utils.time import (  # noqa # import needed for backwards compat
     current_time_millis,
     millis_to_seconds,
 )
 
 __author__ = 'Paul Scott-Murphy, William McBrine'
 __maintainer__ = 'Jakub Stasiak <jakub@stasiak.at>'
-__version__ = '0.62.0'
+__version__ = '0.63.0'
 __license__ = 'LGPL'
 
 
 __all__ = [
     "__version__",
     "Zeroconf",
     "ServiceInfo",
```

### Comparing `zeroconf-0.62.0/src/zeroconf/_cache.py` & `zeroconf-0.63.0/src/zeroconf/_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,40 +130,43 @@
         the event loop.
         """
         store = self.cache.get(entry.key)
         if store is None:
             return None
         return store.get(entry)
 
-    def async_all_by_details(self, name: str, type_: int, class_: int) -> Iterator[DNSRecord]:
+    def async_all_by_details(self, name: _str, type_: int, class_: int) -> Iterator[DNSRecord]:
         """Gets all matching entries by details.
 
         This function is not threadsafe and must be called from
         the event loop.
         """
         key = name.lower()
-        for entry in self.cache.get(key, []):
+        records = self.cache.get(key)
+        if records is None:
+            return
+        for entry in records:
             if _dns_record_matches(entry, key, type_, class_):
                 yield entry
 
     def async_entries_with_name(self, name: str) -> Dict[DNSRecord, DNSRecord]:
         """Returns a dict of entries whose key matches the name.
 
         This function is not threadsafe and must be called from
         the event loop.
         """
-        return self.cache.get(name.lower(), {})
+        return self.cache.get(name.lower()) or {}
 
     def async_entries_with_server(self, name: str) -> Dict[DNSRecord, DNSRecord]:
         """Returns a dict of entries whose key matches the server.
 
         This function is not threadsafe and must be called from
         the event loop.
         """
-        return self.service_cache.get(name.lower(), {})
+        return self.service_cache.get(name.lower()) or {}
 
     # The below functions are threadsafe and do not need to be run in the
     # event loop, however they all make copies so they significantly
     # inefficent
 
     def get(self, entry: DNSEntry) -> Optional[DNSRecord]:
         """Gets an entry by key.  Will return None if there is no
```

### Comparing `zeroconf-0.62.0/src/zeroconf/_core.py` & `zeroconf-0.63.0/src/zeroconf/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -741,15 +741,15 @@
         """Unregister a service."""
         info.set_server_if_missing()
         self.registry.async_remove(info)
         # If another server uses the same addresses, we do not want to send
         # goodbye packets for the address records
 
         assert info.server is not None
-        entries = self.registry.async_get_infos_server(info.server)
+        entries = self.registry.async_get_infos_server(info.server.lower())
         broadcast_addresses = not bool(entries)
         return asyncio.ensure_future(
             self._async_broadcast_service(info, _UNREGISTER_TIME, 0, broadcast_addresses)
         )
 
     def generate_unregister_all_services(self) -> Optional[DNSOutgoing]:
         """Generate a DNSOutgoing goodbye for all services and remove them from the registry."""
```

### Comparing `zeroconf-0.62.0/src/zeroconf/_dns.pxd` & `zeroconf-0.63.0/src/zeroconf/_dns.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/_dns.py` & `zeroconf-0.63.0/src/zeroconf/_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/_exceptions.py` & `zeroconf-0.63.0/src/zeroconf/_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/_handlers.py` & `zeroconf-0.63.0/src/zeroconf/_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,37 +251,37 @@
             dns_pointer = DNSPointer(
                 _SERVICE_TYPE_ENUMERATION_NAME, _TYPE_PTR, _CLASS_IN, _DNS_OTHER_TTL, stype, now
             )
             if not known_answers.suppresses(dns_pointer):
                 answer_set[dns_pointer] = set()
 
     def _add_pointer_answers(
-        self, name: str, answer_set: _AnswerWithAdditionalsType, known_answers: DNSRRSet, now: float
+        self, lower_name: str, answer_set: _AnswerWithAdditionalsType, known_answers: DNSRRSet, now: float
     ) -> None:
         """Answer PTR/ANY question."""
-        for service in self.registry.async_get_infos_type(name):
+        for service in self.registry.async_get_infos_type(lower_name):
             # Add recommended additional answers according to
             # https://tools.ietf.org/html/rfc6763#section-12.1.
             dns_pointer = service.dns_pointer(created=now)
             if known_answers.suppresses(dns_pointer):
                 continue
             additionals: Set[DNSRecord] = {service.dns_service(created=now), service.dns_text(created=now)}
             additionals |= _get_address_and_nsec_records(service, now)
             answer_set[dns_pointer] = additionals
 
     def _add_address_answers(
         self,
-        name: str,
+        lower_name: str,
         answer_set: _AnswerWithAdditionalsType,
         known_answers: DNSRRSet,
         now: float,
         type_: int,
     ) -> None:
         """Answer A/AAAA/ANY question."""
-        for service in self.registry.async_get_infos_server(name):
+        for service in self.registry.async_get_infos_server(lower_name):
             answers: List[DNSAddress] = []
             additionals: Set[DNSRecord] = set()
             seen_types: Set[int] = set()
             for dns_address in service.dns_addresses(created=now):
                 seen_types.add(dns_address.type)
                 if dns_address.type != type_:
                     additionals.add(dns_address)
@@ -301,29 +301,30 @@
     def _answer_question(
         self,
         question: DNSQuestion,
         known_answers: DNSRRSet,
         now: float,
     ) -> _AnswerWithAdditionalsType:
         answer_set: _AnswerWithAdditionalsType = {}
+        question_lower_name = question.name.lower()
 
-        if question.type == _TYPE_PTR and question.name.lower() == _SERVICE_TYPE_ENUMERATION_NAME:
+        if question.type == _TYPE_PTR and question_lower_name == _SERVICE_TYPE_ENUMERATION_NAME:
             self._add_service_type_enumeration_query_answers(answer_set, known_answers, now)
             return answer_set
 
         type_ = question.type
 
         if type_ in (_TYPE_PTR, _TYPE_ANY):
-            self._add_pointer_answers(question.name, answer_set, known_answers, now)
+            self._add_pointer_answers(question_lower_name, answer_set, known_answers, now)
 
         if type_ in (_TYPE_A, _TYPE_AAAA, _TYPE_ANY):
-            self._add_address_answers(question.name, answer_set, known_answers, now, type_)
+            self._add_address_answers(question_lower_name, answer_set, known_answers, now, type_)
 
         if type_ in (_TYPE_SRV, _TYPE_TXT, _TYPE_ANY):
-            service = self.registry.async_get_info_name(question.name)
+            service = self.registry.async_get_info_name(question_lower_name)
             if service is not None:
                 if type_ in (_TYPE_SRV, _TYPE_ANY):
                     # Add recommended additional answers according to
                     # https://tools.ietf.org/html/rfc6763#section-12.2.
                     dns_service = service.dns_service(created=now)
                     if not known_answers.suppresses(dns_service):
                         answer_set[dns_service] = _get_address_and_nsec_records(service, now)
```

### Comparing `zeroconf-0.62.0/src/zeroconf/_history.py` & `zeroconf-0.63.0/src/zeroconf/_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/_logger.py` & `zeroconf-0.63.0/src/zeroconf/_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/_protocol/__init__.py` & `zeroconf-0.63.0/src/zeroconf/_protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/_protocol/incoming.pxd` & `zeroconf-0.63.0/src/zeroconf/_protocol/incoming.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/_protocol/incoming.py` & `zeroconf-0.63.0/src/zeroconf/_protocol/incoming.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/_protocol/outgoing.pxd` & `zeroconf-0.63.0/src/zeroconf/_protocol/outgoing.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/_protocol/outgoing.py` & `zeroconf-0.63.0/src/zeroconf/_protocol/outgoing.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/_services/__init__.py` & `zeroconf-0.63.0/src/zeroconf/_services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/_services/browser.py` & `zeroconf-0.63.0/src/zeroconf/_services/browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/_services/info.py` & `zeroconf-0.63.0/src/zeroconf/_services/info.py`

 * *Files 0% similar despite different names*

```diff
@@ -475,20 +475,23 @@
     def dns_addresses(
         self,
         override_ttl: Optional[int] = None,
         version: IPVersion = IPVersion.All,
         created: Optional[float] = None,
     ) -> List[DNSAddress]:
         """Return matching DNSAddress from ServiceInfo."""
+        name = self.server or self.name
+        ttl = override_ttl if override_ttl is not None else self.host_ttl
+        class_ = _CLASS_IN | _CLASS_UNIQUE
         return [
             DNSAddress(
-                self.server or self.name,
+                name,
                 _TYPE_AAAA if address.version == 6 else _TYPE_A,
-                _CLASS_IN | _CLASS_UNIQUE,
-                override_ttl if override_ttl is not None else self.host_ttl,
+                class_,
+                ttl,
                 address.packed,
                 created=created,
             )
             for address in self.ip_addresses_by_version(version)
         ]
 
     def dns_pointer(self, override_ttl: Optional[int] = None, created: Optional[float] = None) -> DNSPointer:
```

### Comparing `zeroconf-0.62.0/src/zeroconf/_services/registry.py` & `zeroconf-0.63.0/src/zeroconf/_services/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     def async_get_service_infos(self) -> List[ServiceInfo]:
         """Return all ServiceInfo."""
         return list(self._services.values())
 
     def async_get_info_name(self, name: str) -> Optional[ServiceInfo]:
         """Return all ServiceInfo for the name."""
-        return self._services.get(name.lower())
+        return self._services.get(name)
 
     def async_get_types(self) -> List[str]:
         """Return all types."""
         return list(self.types.keys())
 
     def async_get_infos_type(self, type_: str) -> List[ServiceInfo]:
         """Return all ServiceInfo matching type."""
@@ -72,15 +72,15 @@
 
     def async_get_infos_server(self, server: str) -> List[ServiceInfo]:
         """Return all ServiceInfo matching server."""
         return self._async_get_by_index(self.servers, server)
 
     def _async_get_by_index(self, records: Dict[str, List], key: str) -> List[ServiceInfo]:
         """Return all ServiceInfo matching the index."""
-        return [self._services[name] for name in records.get(key.lower(), [])]
+        return [self._services[name] for name in records.get(key, [])]
 
     def _add(self, info: ServiceInfo) -> None:
         """Add a new service under the lock."""
         assert info.server_key is not None, "ServiceInfo must have a server"
         if info.key in self._services:
             raise ServiceNameAlreadyRegistered
```

### Comparing `zeroconf-0.62.0/src/zeroconf/_services/types.py` & `zeroconf-0.63.0/src/zeroconf/_services/types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/_updates.py` & `zeroconf-0.63.0/src/zeroconf/_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/_utils/__init__.py` & `zeroconf-0.63.0/src/zeroconf/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/_utils/asyncio.py` & `zeroconf-0.63.0/src/zeroconf/_utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/_utils/name.py` & `zeroconf-0.63.0/src/zeroconf/_utils/name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/_utils/net.py` & `zeroconf-0.63.0/src/zeroconf/_utils/net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/_utils/time.py` & `zeroconf-0.63.0/src/zeroconf/_utils/time.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/asyncio.py` & `zeroconf-0.63.0/src/zeroconf/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/src/zeroconf/const.py` & `zeroconf-0.63.0/src/zeroconf/const.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/__init__.py` & `zeroconf-0.63.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/conftest.py` & `zeroconf-0.63.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/services/__init__.py` & `zeroconf-0.63.0/tests/services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/services/test_browser.py` & `zeroconf-0.63.0/tests/services/test_browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/services/test_info.py` & `zeroconf-0.63.0/tests/services/test_info.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/services/test_registry.py` & `zeroconf-0.63.0/tests/services/test_registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,26 +106,7 @@
         registry.async_add(info)
 
         assert registry.async_get_service_infos() == [info]
         assert registry.async_get_info_name(registration_name.lower()) == info
         assert registry.async_get_infos_type(type_.lower()) == [info]
         assert registry.async_get_infos_server("ash-2.local.") == [info]
         assert registry.async_get_types() == [type_.lower()]
-
-    def test_lookups_lower_case_by_upper_case(self):
-        type_ = "_test-srvc-type._tcp.local."
-        name = "xxxyyy"
-        registration_name = f"{name}.{type_}"
-
-        desc = {'path': '/~paulsm/'}
-        info = ServiceInfo(
-            type_, registration_name, 80, 0, 0, desc, "ash-2.local.", addresses=[socket.inet_aton("10.0.1.2")]
-        )
-
-        registry = r.ServiceRegistry()
-        registry.async_add(info)
-
-        assert registry.async_get_service_infos() == [info]
-        assert registry.async_get_info_name(registration_name.upper()) == info
-        assert registry.async_get_infos_type(type_.upper()) == [info]
-        assert registry.async_get_infos_server("ASH-2.local.") == [info]
-        assert registry.async_get_types() == [type_]
```

### Comparing `zeroconf-0.62.0/tests/services/test_types.py` & `zeroconf-0.63.0/tests/services/test_types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/test_asyncio.py` & `zeroconf-0.63.0/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/test_cache.py` & `zeroconf-0.63.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/test_core.py` & `zeroconf-0.63.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/test_dns.py` & `zeroconf-0.63.0/tests/test_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/test_exceptions.py` & `zeroconf-0.63.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/test_handlers.py` & `zeroconf-0.63.0/tests/test_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,14 +338,40 @@
     # unregister
     zc.registry.async_remove(info)
     zc.close()
 
 
 @unittest.skipIf(not has_working_ipv6(), 'Requires IPv6')
 @unittest.skipIf(os.environ.get('SKIP_IPV6'), 'IPv6 tests disabled')
+def test_aaaa_query_upper_case():
+    """Test that queries for AAAA records work and should respond right away with an upper case name."""
+    zc = Zeroconf(interfaces=['127.0.0.1'])
+    type_ = "_knownaaaservice._tcp.local."
+    name = "knownname"
+    registration_name = f"{name}.{type_}"
+    desc = {'path': '/~paulsm/'}
+    server_name = "ash-2.local."
+    ipv6_address = socket.inet_pton(socket.AF_INET6, "2001:db8::1")
+    info = ServiceInfo(type_, registration_name, 80, 0, 0, desc, server_name, addresses=[ipv6_address])
+    zc.registry.async_add(info)
+
+    generated = r.DNSOutgoing(const._FLAGS_QR_QUERY)
+    question = r.DNSQuestion(server_name.upper(), const._TYPE_AAAA, const._CLASS_IN)
+    generated.add_question(question)
+    packets = generated.packets()
+    question_answers = zc.query_handler.async_response([r.DNSIncoming(packet) for packet in packets], False)
+    mcast_answers = list(question_answers.mcast_now)
+    assert mcast_answers[0].address == ipv6_address  # type: ignore[attr-defined]
+    # unregister
+    zc.registry.async_remove(info)
+    zc.close()
+
+
+@unittest.skipIf(not has_working_ipv6(), 'Requires IPv6')
+@unittest.skipIf(os.environ.get('SKIP_IPV6'), 'IPv6 tests disabled')
 def test_a_and_aaaa_record_fate_sharing():
     """Test that queries for AAAA always return A records in the additionals and should respond right away."""
     zc = Zeroconf(interfaces=['127.0.0.1'])
     type_ = "_a-and-aaaa-service._tcp.local."
     name = "knownname"
     registration_name = f"{name}.{type_}"
     desc = {'path': '/~paulsm/'}
@@ -477,14 +503,56 @@
     assert question_answers.ucast
     assert question_answers.mcast_now
     assert not question_answers.mcast_aggregate
     assert not question_answers.mcast_aggregate_last_second
     zc.close()
 
 
+@pytest.mark.asyncio
+async def test_probe_answered_immediately_with_uppercase_name():
+    """Verify probes are responded to immediately with an uppercase name."""
+    # instantiate a zeroconf instance
+    zc = Zeroconf(interfaces=['127.0.0.1'])
+
+    # service definition
+    type_ = "_test-srvc-type._tcp.local."
+    name = "xxxyyy"
+    registration_name = f"{name}.{type_}"
+    desc = {'path': '/~paulsm/'}
+    info = ServiceInfo(
+        type_, registration_name, 80, 0, 0, desc, "ash-2.local.", addresses=[socket.inet_aton("10.0.1.2")]
+    )
+    zc.registry.async_add(info)
+    query = r.DNSOutgoing(const._FLAGS_QR_QUERY)
+    question = r.DNSQuestion(info.type.upper(), const._TYPE_PTR, const._CLASS_IN)
+    query.add_question(question)
+    query.add_authorative_answer(info.dns_pointer())
+    question_answers = zc.query_handler.async_response(
+        [r.DNSIncoming(packet) for packet in query.packets()], False
+    )
+    assert not question_answers.ucast
+    assert not question_answers.mcast_aggregate
+    assert not question_answers.mcast_aggregate_last_second
+    assert question_answers.mcast_now
+
+    query = r.DNSOutgoing(const._FLAGS_QR_QUERY)
+    question = r.DNSQuestion(info.type, const._TYPE_PTR, const._CLASS_IN)
+    question.unicast = True
+    query.add_question(question)
+    query.add_authorative_answer(info.dns_pointer())
+    question_answers = zc.query_handler.async_response(
+        [r.DNSIncoming(packet) for packet in query.packets()], False
+    )
+    assert question_answers.ucast
+    assert question_answers.mcast_now
+    assert not question_answers.mcast_aggregate
+    assert not question_answers.mcast_aggregate_last_second
+    zc.close()
+
+
 def test_qu_response():
     """Handle multicast incoming with the QU bit set."""
     # instantiate a zeroconf instance
     zc = Zeroconf(interfaces=['127.0.0.1'])
 
     # service definition
     type_ = "_test-srvc-type._tcp.local."
@@ -838,14 +906,53 @@
 
     # unregister
     zc.registry.async_remove(info)
     zc.registry.async_remove(info2)
     zc.close()
 
 
+def test_upper_case_enumeration_query():
+    zc = Zeroconf(interfaces=['127.0.0.1'])
+    type_ = "_otherknown._tcp.local."
+    name = "knownname"
+    registration_name = f"{name}.{type_}"
+    desc = {'path': '/~paulsm/'}
+    server_name = "ash-2.local."
+    info = ServiceInfo(
+        type_, registration_name, 80, 0, 0, desc, server_name, addresses=[socket.inet_aton("10.0.1.2")]
+    )
+    zc.registry.async_add(info)
+
+    type_2 = "_otherknown2._tcp.local."
+    name = "knownname"
+    registration_name2 = f"{name}.{type_2}"
+    desc = {'path': '/~paulsm/'}
+    server_name2 = "ash-3.local."
+    info2 = ServiceInfo(
+        type_2, registration_name2, 80, 0, 0, desc, server_name2, addresses=[socket.inet_aton("10.0.1.2")]
+    )
+    zc.registry.async_add(info2)
+    _clear_cache(zc)
+
+    # Test PTR supression
+    generated = r.DNSOutgoing(const._FLAGS_QR_QUERY)
+    question = r.DNSQuestion(const._SERVICE_TYPE_ENUMERATION_NAME.upper(), const._TYPE_PTR, const._CLASS_IN)
+    generated.add_question(question)
+    packets = generated.packets()
+    question_answers = zc.query_handler.async_response([r.DNSIncoming(packet) for packet in packets], False)
+    assert not question_answers.ucast
+    assert not question_answers.mcast_now
+    assert question_answers.mcast_aggregate
+    assert not question_answers.mcast_aggregate_last_second
+    # unregister
+    zc.registry.async_remove(info)
+    zc.registry.async_remove(info2)
+    zc.close()
+
+
 # This test uses asyncio because it needs to access the cache directly
 # which is not threadsafe
 @pytest.mark.asyncio
 async def test_qu_response_only_sends_additionals_if_sends_answer():
     """Test that a QU response does not send additionals unless it sends the answer as well."""
     # instantiate a zeroconf instance
     aiozc = AsyncZeroconf(interfaces=['127.0.0.1'])
```

### Comparing `zeroconf-0.62.0/tests/test_history.py` & `zeroconf-0.63.0/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/test_init.py` & `zeroconf-0.63.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/test_logger.py` & `zeroconf-0.63.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/test_protocol.py` & `zeroconf-0.63.0/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/test_services.py` & `zeroconf-0.63.0/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/test_updates.py` & `zeroconf-0.63.0/tests/test_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/utils/__init__.py` & `zeroconf-0.63.0/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/utils/test_asyncio.py` & `zeroconf-0.63.0/tests/utils/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/utils/test_name.py` & `zeroconf-0.63.0/tests/utils/test_name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/tests/utils/test_net.py` & `zeroconf-0.63.0/tests/utils/test_net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.62.0/setup.py` & `zeroconf-0.63.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['ifaddr>=0.1.7']
 
 extras_require = \
 {':python_version < "3.11"': ['async-timeout>=3.0.0']}
 
 setup_kwargs = {
     'name': 'zeroconf',
-    'version': '0.62.0',
+    'version': '0.63.0',
     'description': 'A pure python implementation of multicast DNS service discovery',
     'long_description': 'python-zeroconf\n===============\n\n.. image:: https://github.com/python-zeroconf/python-zeroconf/workflows/CI/badge.svg\n   :target: https://github.com/python-zeroconf/python-zeroconf?query=workflow%3ACI+branch%3Amaster\n\n.. image:: https://img.shields.io/pypi/v/zeroconf.svg\n    :target: https://pypi.python.org/pypi/zeroconf\n\n.. image:: https://codecov.io/gh/python-zeroconf/python-zeroconf/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/python-zeroconf/python-zeroconf\n\n`Documentation <https://python-zeroconf.readthedocs.io/en/latest/>`_.\n\nThis is fork of pyzeroconf, Multicast DNS Service Discovery for Python,\noriginally by Paul Scott-Murphy (https://github.com/paulsm/pyzeroconf),\nmodified by William McBrine (https://github.com/wmcbrine/pyzeroconf).\n\nThe original William McBrine\'s fork note::\n\n    This fork is used in all of my TiVo-related projects: HME for Python\n    (and therefore HME/VLC), Network Remote, Remote Proxy, and pyTivo.\n    Before this, I was tracking the changes for zeroconf.py in three\n    separate repos. I figured I should have an authoritative source.\n\n    Although I make changes based on my experience with TiVos, I expect that\n    they\'re generally applicable. This version also includes patches found\n    on the now-defunct (?) Launchpad repo of pyzeroconf, and elsewhere\n    around the net -- not always well-documented, sorry.\n\nCompatible with:\n\n* Bonjour\n* Avahi\n\nCompared to some other Zeroconf/Bonjour/Avahi Python packages, python-zeroconf:\n\n* isn\'t tied to Bonjour or Avahi\n* doesn\'t use D-Bus\n* doesn\'t force you to use particular event loop or Twisted (asyncio is used under the hood but not required)\n* is pip-installable\n* has PyPI distribution\n* has an optional cython extension for performance (pure python is supported as well)\n\nPython compatibility\n--------------------\n\n* CPython 3.7+\n* PyPy3.7 7.3+\n\nVersioning\n----------\n\nThis project uses semantic versioning.\n\nStatus\n------\n\nThis project is actively maintained.\n\nTraffic Reduction\n-----------------\n\nBefore version 0.32, most traffic reduction techniques described in https://datatracker.ietf.org/doc/html/rfc6762#section-7\nwhere not implemented which could lead to excessive network traffic.  It is highly recommended that version 0.32 or later\nis used if this is a concern.\n\nIPv6 support\n------------\n\nIPv6 support is relatively new and currently limited, specifically:\n\n* `InterfaceChoice.All` is an alias for `InterfaceChoice.Default` on non-POSIX\n  systems.\n* Dual-stack IPv6 sockets are used, which may not be supported everywhere (some\n  BSD variants do not have them).\n* Listening on localhost (`::1`) does not work. Help with understanding why is\n  appreciated.\n\nHow to get python-zeroconf?\n===========================\n\n* PyPI page https://pypi.org/project/zeroconf/\n* GitHub project https://github.com/python-zeroconf/python-zeroconf\n\nThe easiest way to install python-zeroconf is using pip::\n\n    pip install zeroconf\n\n\n\nHow do I use it?\n================\n\nHere\'s an example of browsing for a service:\n\n.. code-block:: python\n\n    from zeroconf import ServiceBrowser, ServiceListener, Zeroconf\n\n\n    class MyListener(ServiceListener):\n\n        def update_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} updated")\n\n        def remove_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} removed")\n\n        def add_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            info = zc.get_service_info(type_, name)\n            print(f"Service {name} added, service info: {info}")\n\n\n    zeroconf = Zeroconf()\n    listener = MyListener()\n    browser = ServiceBrowser(zeroconf, "_http._tcp.local.", listener)\n    try:\n        input("Press enter to exit...\\n\\n")\n    finally:\n        zeroconf.close()\n\n.. note::\n\n    Discovery and service registration use *all* available network interfaces by default.\n    If you want to customize that you need to specify ``interfaces`` argument when\n    constructing ``Zeroconf`` object (see the code for details).\n\nIf you don\'t know the name of the service you need to browse for, try:\n\n.. code-block:: python\n\n    from zeroconf import ZeroconfServiceTypes\n    print(\'\\n\'.join(ZeroconfServiceTypes.find()))\n\nSee examples directory for more.\n\nChangelog\n=========\n\n`Changelog <CHANGELOG.md>`_\n\nLicense\n=======\n\nLGPL, see COPYING file for details.\n',
     'author': 'Paul Scott-Murphy',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/python-zeroconf/python-zeroconf',
```

### Comparing `zeroconf-0.62.0/PKG-INFO` & `zeroconf-0.63.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroconf
-Version: 0.62.0
+Version: 0.63.0
 Summary: A pure python implementation of multicast DNS service discovery
 Home-page: https://github.com/python-zeroconf/python-zeroconf
 License: LGPL
 Author: Paul Scott-Murphy
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -16,19 +16,14 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: async-timeout (>=3.0.0) ; python_version < "3.11"
 Requires-Dist: ifaddr (>=0.1.7)
 Project-URL: Bug Tracker, https://github.com/python-zeroconf/python-zeroconf/issues
 Project-URL: Changelog, https://github.com/python-zeroconf/python-zeroconf/blob/master/CHANGELOG.md
```

