# Comparing `tmp/obsession-1.2.0.tar.gz` & `tmp/obsession-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obsession-1.2.0.tar", last modified: Thu Jun 23 14:47:10 2022, max compression
+gzip compressed data, was "obsession-1.2.1.tar", last modified: Thu May 25 12:29:14 2023, max compression
```

## Comparing `obsession-1.2.0.tar` & `obsession-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2022-06-23 14:47:10.823778 obsession-1.2.0/
--rw-r--r--   0 oliver    (1001) wheel        (0)      958 2022-06-23 14:46:19.000000 obsession-1.2.0/CHANGELOG.rst
--rw-r--r--   0 oliver    (1001) wheel        (0)    11358 2022-06-23 14:46:18.000000 obsession-1.2.0/LICENSE.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)       53 2022-06-23 14:46:18.000000 obsession-1.2.0/MANIFEST.in
--rw-r--r--   0 oliver    (1001) wheel        (0)     2833 2022-06-23 14:47:10.823919 obsession-1.2.0/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)     1949 2022-06-23 14:46:18.000000 obsession-1.2.0/README.rst
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2022-06-23 14:47:10.822089 obsession-1.2.0/obsession/
--rw-r--r--   0 oliver    (1001) wheel        (0)    12731 2022-06-23 14:46:18.000000 obsession-1.2.0/obsession/__init__.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2022-06-23 14:47:10.823576 obsession-1.2.0/obsession/tests/
--rw-r--r--   0 oliver    (1001) wheel        (0)     9624 2022-06-23 14:46:18.000000 obsession-1.2.0/obsession/tests/test_session.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2022-06-23 14:47:10.823277 obsession-1.2.0/obsession.egg-info/
--rw-r--r--   0 oliver    (1001) wheel        (0)     2833 2022-06-23 14:47:09.000000 obsession-1.2.0/obsession.egg-info/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)      253 2022-06-23 14:47:10.000000 obsession-1.2.0/obsession.egg-info/SOURCES.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)        1 2022-06-23 14:47:10.000000 obsession-1.2.0/obsession.egg-info/dependency_links.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)       10 2022-06-23 14:47:10.000000 obsession-1.2.0/obsession.egg-info/top_level.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)      833 2022-06-23 14:47:10.824641 obsession-1.2.0/setup.cfg
--rw-r--r--   0 oliver    (1001) wheel        (0)      636 2022-06-23 14:46:18.000000 obsession-1.2.0/setup.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-25 12:29:14.121261 obsession-1.2.1/
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1085 2023-05-25 12:28:41.000000 obsession-1.2.1/CHANGELOG.rst
+-rw-r--r--   0 oliver    (1001) wheel        (0)    11358 2023-05-25 12:28:41.000000 obsession-1.2.1/LICENSE.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)       53 2023-05-25 12:28:41.000000 obsession-1.2.1/MANIFEST.in
+-rw-r--r--   0 oliver    (1001) wheel        (0)     2813 2023-05-25 12:29:14.121366 obsession-1.2.1/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1949 2023-05-25 12:28:41.000000 obsession-1.2.1/README.rst
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-25 12:29:14.120011 obsession-1.2.1/obsession/
+-rw-r--r--   0 oliver    (1001) wheel        (0)    12734 2023-05-25 12:28:41.000000 obsession-1.2.1/obsession/__init__.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-25 12:29:14.121075 obsession-1.2.1/obsession/tests/
+-rw-r--r--   0 oliver    (1001) wheel        (0)     9624 2023-05-25 12:28:41.000000 obsession-1.2.1/obsession/tests/test_session.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-25 12:29:14.120860 obsession-1.2.1/obsession.egg-info/
+-rw-r--r--   0 oliver    (1001) wheel        (0)     2813 2023-05-25 12:29:13.000000 obsession-1.2.1/obsession.egg-info/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)      253 2023-05-25 12:29:13.000000 obsession-1.2.1/obsession.egg-info/SOURCES.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)        1 2023-05-25 12:29:13.000000 obsession-1.2.1/obsession.egg-info/dependency_links.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)       10 2023-05-25 12:29:13.000000 obsession-1.2.1/obsession.egg-info/top_level.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)      833 2023-05-25 12:29:14.122043 obsession-1.2.1/setup.cfg
+-rw-r--r--   0 oliver    (1001) wheel        (0)      636 2023-05-25 12:28:41.000000 obsession-1.2.1/setup.py
```

### Comparing `obsession-1.2.0/CHANGELOG.rst` & `obsession-1.2.1/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+1.2.1 (released 2023-05-25)
+---------------------------
+
+- Bugfix: fix content iterator not being closed in SessionMiddleware
+
 1.2.0 (released 2022-06-23)
 ---------------------------
 
 - Bugfix: fix error in MemoryBackend.modified_at()
 - Add tests for python 3.8 - 3.11
 - Expire session cookie when the session is deleted
 - Auto extend cookie lifetime while session is active
```

### Comparing `obsession-1.2.0/LICENSE.txt` & `obsession-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `obsession-1.2.0/PKG-INFO` & `obsession-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: obsession
-Version: 1.2.0
+Version: 1.2.1
 Summary: Server-side HTTP sessions
 Home-page: https://hg.sr.ht/~olly/obsession/
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: wsgi session sessions management cookie
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -80,9 +79,7 @@
     s = environ['ob.session']
     s.load_id('my_session_id')
 
     # Delete the session.
     # This removes all data from the backend storage and deletes the client's
     # session cookie
     session.delete()
-
-
```

### Comparing `obsession-1.2.0/README.rst` & `obsession-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `obsession-1.2.0/obsession/__init__.py` & `obsession-1.2.1/obsession/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,19 +421,19 @@
         set_id_middleware=id_persister.set_id_middleware,
         get_id=id_persister.get_id,
         SESSION_KEY=SESSION_KEY,
         backend=backend,
     ):
 
         session = environ[SESSION_KEY] = Session(environ, backend, get_id)
-        content = None
-        try:
-            yield from id_persister.set_id_middleware(
+        content = id_persister.set_id_middleware(
                 session, app, environ, start_response
             )
+        try:
+            yield from content
         finally:
             try:
                 if session.dirty and session.data:
                     backend.save(session.id, session.data)
             finally:
                 close = getattr(content, "close", None)
                 if close is not None:
```

### Comparing `obsession-1.2.0/obsession/tests/test_session.py` & `obsession-1.2.1/obsession/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `obsession-1.2.0/obsession.egg-info/PKG-INFO` & `obsession-1.2.1/obsession.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: obsession
-Version: 1.2.0
+Version: 1.2.1
 Summary: Server-side HTTP sessions
 Home-page: https://hg.sr.ht/~olly/obsession/
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: wsgi session sessions management cookie
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -80,9 +79,7 @@
     s = environ['ob.session']
     s.load_id('my_session_id')
 
     # Delete the session.
     # This removes all data from the backend storage and deletes the client's
     # session cookie
     session.delete()
-
-
```

### Comparing `obsession-1.2.0/setup.cfg` & `obsession-1.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = obsession
-version = 1.2.0
+version = 1.2.1
 description = Server-side HTTP sessions
 long_description = file: README.rst
 author = Oliver Cope
 author_email = oliver@redgecko.org
 url = https://hg.sr.ht/~olly/obsession/
 license = Apache
 keywords = wsgi session sessions management cookie
```

### Comparing `obsession-1.2.0/setup.py` & `obsession-1.2.1/setup.py`

 * *Files identical despite different names*

