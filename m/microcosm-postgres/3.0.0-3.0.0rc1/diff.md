# Comparing `tmp/microcosm-postgres-3.0.0.tar.gz` & `tmp/microcosm-postgres-3.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/microcosm-postgres-3.0.0.tar", last modified: Thu May 25 09:11:11 2023, max compression
+gzip compressed data, was "dist/microcosm-postgres-3.0.0rc1.tar", last modified: Tue May 23 16:48:26 2023, max compression
```

## Comparing `microcosm-postgres-3.0.0.tar` & `microcosm-postgres-3.0.0rc1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-25 09:11:11.000000 microcosm-postgres-3.0.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)      427 2023-05-25 09:11:11.000000 microcosm-postgres-3.0.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4030 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-25 09:11:11.000000 microcosm-postgres-3.0.0/microcosm_postgres/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1038 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/cloning.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2465 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/context.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      531 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/createall.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4357 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/dag.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1026 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/diff.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-25 09:11:11.000000 microcosm-postgres-3.0.0/microcosm_postgres/encryption/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/encryption/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3874 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/encryption/encryptor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      420 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/encryption/factories.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6331 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/encryption/models.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3194 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/encryption/providers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3310 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/encryption/registry.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3607 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/encryption/store.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1613 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/errors.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-25 09:11:11.000000 microcosm-postgres-3.0.0/microcosm_postgres/factories/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/factories/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4859 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/factories/engine.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1605 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/factories/engine_routing_strategy.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      901 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/factories/sessionmaker.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      802 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/health.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      150 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/identifiers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2369 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/metrics.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7786 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/migrate.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5042 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/models.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2425 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/operations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9517 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/store.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-25 09:11:11.000000 microcosm-postgres-3.0.0/microcosm_postgres/temporary/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       73 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/temporary/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      621 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/temporary/context.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1164 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/temporary/copy.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1880 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/temporary/factories.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1798 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/temporary/methods.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1096 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/toposort.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1907 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/microcosm_postgres/types.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-25 09:11:11.000000 microcosm-postgres-3.0.0/microcosm_postgres.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      427 2023-05-25 09:11:11.000000 microcosm-postgres-3.0.0/microcosm_postgres.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1493 2023-05-25 09:11:11.000000 microcosm-postgres-3.0.0/microcosm_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-25 09:11:11.000000 microcosm-postgres-3.0.0/microcosm_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      770 2023-05-25 09:11:11.000000 microcosm-postgres-3.0.0/microcosm_postgres.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-25 09:11:11.000000 microcosm-postgres-3.0.0/microcosm_postgres.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      304 2023-05-25 09:11:11.000000 microcosm-postgres-3.0.0/microcosm_postgres.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2023-05-25 09:11:11.000000 microcosm-postgres-3.0.0/microcosm_postgres.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      776 2023-05-25 09:11:11.000000 microcosm-postgres-3.0.0/setup.cfg
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2143 2023-05-25 09:08:33.000000 microcosm-postgres-3.0.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      430 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4030 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1038 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/cloning.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2430 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/context.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      531 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/createall.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4357 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/dag.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1026 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/diff.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3874 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/encryptor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      420 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/factories.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6331 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/models.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3194 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/providers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3310 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/registry.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3607 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/store.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1613 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/errors.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/factories/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/factories/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4859 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/factories/engine.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1605 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/factories/engine_routing_strategy.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      901 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/factories/sessionmaker.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      802 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/health.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      150 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/identifiers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2369 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/metrics.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7786 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/migrate.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5042 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/models.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2425 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/operations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9517 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/store.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       73 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      621 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/context.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1164 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/copy.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1880 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/factories.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1798 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/methods.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1096 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/toposort.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1907 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/types.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      430 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1493 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      770 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      304 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      776 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/setup.cfg
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2146 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/setup.py
```

### Comparing `microcosm-postgres-3.0.0/LICENSE` & `microcosm-postgres-3.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/README.md` & `microcosm-postgres-3.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/cloning.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/cloning.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/context.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,64 +6,63 @@
 from functools import wraps
 
 from sqlalchemy.orm import scoped_session
 
 from microcosm_postgres.operations import new_session, recreate_all
 
 
-class SessionContextFactory:
-    def __init__(self) -> None:
-        self.session_cls = None
-        self.expire_on_commit = False
-
-    @property
-    def session(self):
-        assert self.session_cls is not None, "Session not initialized"
-        return self.session_cls()
-
-    def __call__(self, graph, expire_on_commit=False):
-        self.session_cls = scoped_session(
-            lambda: new_session(graph, expire_on_commit)
-        )
-        self.expire_on_commit = expire_on_commit
-        return Context(graph, self.session_cls)
-
-    def make(self, graph, expire_on_commit=False):
-        return self(graph).open()
+class SessionContext:
+    """
+    Save current session in well-known location and provide context management.
 
+    New in version 3.0.0:
+        Now thread safe using a `scoped_session`.
+    """
+    session = None
 
-class Context:
-    def __init__(self, graph, session_cls):
+    def __init__(self, graph, expire_on_commit=False):
         self.graph = graph
-        self.session_cls = session_cls
+        self.expire_on_commit = expire_on_commit
+        self.session_cls = scoped_session(
+            lambda: new_session(self.graph, self.expire_on_commit)
+        )
 
     def open(self):
-        self.session = self.session_cls()
+        SessionContext.session = self.session_cls()
         return self
 
     def close(self):
-        self.session_cls.remove()
+        if SessionContext.session:
+            self.session_cls.remove()
+            SessionContext.session = None
 
     def recreate_all(self):
         """
         Recreate all database tables, but only in a testing context.
         """
         if self.graph.metadata.testing:
             recreate_all(self.graph)
 
+    @classmethod
+    def make(cls, graph, expire_on_commit=False):
+        """
+        Create an opened context.
+
+        """
+        return cls(graph, expire_on_commit).open()
+
+    # context manager
+
     def __enter__(self):
         return self.open()
 
     def __exit__(self, *args, **kwargs):
         self.close()
 
 
-SessionContext = SessionContextFactory()
-
-
 @contextmanager
 def transaction(commit=True):
     """
     Wrap a context with a commit/rollback.
 
     """
     try:
```

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/createall.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/createall.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/dag.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/dag.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/diff.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/diff.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/encryption/encryptor.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/encryptor.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/encryption/models.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/models.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/encryption/providers.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/providers.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/encryption/registry.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/registry.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/encryption/store.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/store.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/errors.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/errors.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/factories/engine.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/factories/engine.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/factories/engine_routing_strategy.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/factories/engine_routing_strategy.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/factories/sessionmaker.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/factories/sessionmaker.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/health.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/health.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/metrics.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/metrics.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/migrate.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/migrate.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/models.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/models.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/operations.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/operations.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/store.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/store.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/temporary/context.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/context.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/temporary/copy.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/copy.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/temporary/factories.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/factories.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/temporary/methods.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/methods.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/toposort.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/toposort.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres/types.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/types.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres.egg-info/SOURCES.txt` & `microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/microcosm_postgres.egg-info/entry_points.txt` & `microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/setup.cfg` & `microcosm-postgres-3.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-3.0.0/setup.py` & `microcosm-postgres-3.0.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import find_packages, setup
 
 
 project = "microcosm-postgres"
-version = "3.0.0"
+version = "3.0.0rc1"
 
 setup(
     name=project,
     version=version,
     description="Opinionated persistence with PostgreSQL",
     author="Globality Engineering",
     author_email="engineering@globality.com",
```

