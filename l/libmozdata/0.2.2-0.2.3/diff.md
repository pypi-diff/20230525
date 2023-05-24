# Comparing `tmp/libmozdata-0.2.2.tar.gz` & `tmp/libmozdata-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libmozdata-0.2.2.tar", last modified: Wed May  3 18:20:38 2023, max compression
+gzip compressed data, was "dist/libmozdata-0.2.3.tar", last modified: Wed May 24 22:18:32 2023, max compression
```

## Comparing `libmozdata-0.2.2.tar` & `libmozdata-0.2.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:20:38.000000 libmozdata-0.2.2/
--rw-r--r--   0 root         (0) root         (0)      155 2023-05-03 18:20:38.000000 libmozdata-0.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      472 2023-05-03 18:20:38.000000 libmozdata-0.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-03 18:20:38.000000 libmozdata-0.2.2/README.md
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-03 18:20:38.000000 libmozdata-0.2.2/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/
--rw-r--r--   0 root         (0) root         (0)     7695 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/BZInfo.py
--rw-r--r--   0 root         (0) root         (0)     1828 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/FXRevision.py
--rw-r--r--   0 root         (0) root         (0)     4268 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/FileStats.py
--rw-r--r--   0 root         (0) root         (0)     5540 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/HGFileInfo.py
--rw-r--r--   0 root         (0) root         (0)      424 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38502 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/bugzilla.py
--rw-r--r--   0 root         (0) root         (0)     4042 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/buildhub.py
--rw-r--r--   0 root         (0) root         (0)     1800 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/config.py
--rw-r--r--   0 root         (0) root         (0)     7286 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/connection.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/fx_trains.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/handler.py
--rw-r--r--   0 root         (0) root         (0)    10234 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/hgmozilla.py
--rw-r--r--   0 root         (0) root         (0)     2764 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/lando.py
--rw-r--r--   0 root         (0) root         (0)    75057 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/modules.json
--rw-r--r--   0 root         (0) root         (0)     2781 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/modules.py
--rw-r--r--   0 root         (0) root         (0)    39379 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/patchanalysis.py
--rw-r--r--   0 root         (0) root         (0)    24340 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/phabricator.py
--rw-r--r--   0 root         (0) root         (0)     6327 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/redash.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/release_owners.py
--rw-r--r--   0 root         (0) root         (0)     8039 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/socorro.py
--rw-r--r--   0 root         (0) root         (0)     8653 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/utils.py
--rw-r--r--   0 root         (0) root         (0)     1564 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/vcs_map.py
--rw-r--r--   0 root         (0) root         (0)     5014 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/versions.py
--rw-r--r--   0 root         (0) root         (0)     3581 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/wiki_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata.egg-info/
--rw-r--r--   0 root         (0) root         (0)      472 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      830 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-03 18:20:38.000000 libmozdata-0.2.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-03 18:20:38.000000 libmozdata-0.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1214 2023-05-03 18:20:38.000000 libmozdata-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:18:32.000000 libmozdata-0.2.3/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-05-24 22:18:31.000000 libmozdata-0.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      472 2023-05-24 22:18:32.000000 libmozdata-0.2.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-24 22:18:31.000000 libmozdata-0.2.3/README.md
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-24 22:18:31.000000 libmozdata-0.2.3/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:18:32.000000 libmozdata-0.2.3/libmozdata/
+-rw-r--r--   0 root         (0) root         (0)     7695 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/BZInfo.py
+-rw-r--r--   0 root         (0) root         (0)     1828 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/FXRevision.py
+-rw-r--r--   0 root         (0) root         (0)     4268 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/FileStats.py
+-rw-r--r--   0 root         (0) root         (0)     5540 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/HGFileInfo.py
+-rw-r--r--   0 root         (0) root         (0)      424 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38900 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/bugzilla.py
+-rw-r--r--   0 root         (0) root         (0)     4042 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/buildhub.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/config.py
+-rw-r--r--   0 root         (0) root         (0)     7286 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/connection.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/fx_trains.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/handler.py
+-rw-r--r--   0 root         (0) root         (0)    10234 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/hgmozilla.py
+-rw-r--r--   0 root         (0) root         (0)     2764 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/lando.py
+-rw-r--r--   0 root         (0) root         (0)    75057 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/modules.json
+-rw-r--r--   0 root         (0) root         (0)     2781 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/modules.py
+-rw-r--r--   0 root         (0) root         (0)    39379 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/patchanalysis.py
+-rw-r--r--   0 root         (0) root         (0)    24114 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/phabricator.py
+-rw-r--r--   0 root         (0) root         (0)     6327 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/redash.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/release_owners.py
+-rw-r--r--   0 root         (0) root         (0)     8039 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/socorro.py
+-rw-r--r--   0 root         (0) root         (0)     8653 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/vcs_map.py
+-rw-r--r--   0 root         (0) root         (0)     5014 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/versions.py
+-rw-r--r--   0 root         (0) root         (0)     3581 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/wiki_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:18:32.000000 libmozdata-0.2.3/libmozdata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      472 2023-05-24 22:18:32.000000 libmozdata-0.2.3/libmozdata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      830 2023-05-24 22:18:32.000000 libmozdata-0.2.3/libmozdata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 22:18:32.000000 libmozdata-0.2.3/libmozdata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 22:18:32.000000 libmozdata-0.2.3/libmozdata.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-24 22:18:32.000000 libmozdata-0.2.3/libmozdata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-24 22:18:32.000000 libmozdata-0.2.3/libmozdata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-24 22:18:31.000000 libmozdata-0.2.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-24 22:18:32.000000 libmozdata-0.2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1214 2023-05-24 22:18:31.000000 libmozdata-0.2.3/setup.py
```

### Comparing `libmozdata-0.2.2/README.md` & `libmozdata-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/BZInfo.py` & `libmozdata-0.2.3/libmozdata/BZInfo.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/FXRevision.py` & `libmozdata-0.2.3/libmozdata/FXRevision.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/FileStats.py` & `libmozdata-0.2.3/libmozdata/FileStats.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/HGFileInfo.py` & `libmozdata-0.2.3/libmozdata/HGFileInfo.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/bugzilla.py` & `libmozdata-0.2.3/libmozdata/bugzilla.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
 import functools
 import re
 
 import requests
 import six
+from requests import HTTPError
 
 import libmozdata.versions
 
 from . import config, utils
 from .connection import Connection, Query
 from .handler import Handler
 
@@ -1053,14 +1054,22 @@
         header["X-Bugzilla-API-Key"] = self.get_apikey()
         return header
 
     def __urls_cb(self, res):
         if not self.url_handler.isactive():
             return
 
+        if not isinstance(res, dict):
+            # This is a workaround to handle cases where Bugzilla returns 200
+            # response with HTML content instead of 4xx error.
+            # See https://github.com/mozilla/libmozdata/issues/227
+            if self.RAISE_ERROR:
+                raise HTTPError("The response is not a valid JSON")
+            return
+
         self.url_handler.handle(res["url"])
 
 
 class BugzillaComponent(Connection):
     """
     Connection to bugzilla.mozilla.org
     """
```

### Comparing `libmozdata-0.2.2/libmozdata/buildhub.py` & `libmozdata-0.2.3/libmozdata/buildhub.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/config.py` & `libmozdata-0.2.3/libmozdata/config.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/connection.py` & `libmozdata-0.2.3/libmozdata/connection.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/fx_trains.py` & `libmozdata-0.2.3/libmozdata/fx_trains.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,18 +10,44 @@
 
     Documentations: https://whattrainisitnow.com/about
     """
 
     URL = "https://whattrainisitnow.com/api/"
     TIMEOUT = 30
 
+    _instance = None
+
+    def __init__(self, cache: bool = True) -> None:
+        """Constructor
+
+        Args:
+            cache: If True, the API responses will be cached.
+        """
+
+        self._cache = {} if cache else None
+
+    @classmethod
+    def get_instance(cls):
+        """Get the singleton instance of FirefoxTrains."""
+        if cls._instance is None:
+            cls._instance = cls()
+        return cls._instance
+
     def __get(self, path):
+        if self._cache is not None and path in self._cache:
+            return self._cache[path]
+
         resp = requests.get(self.URL + path, timeout=self.TIMEOUT)
         resp.raise_for_status()
-        return resp.json()
+        resp_json = resp.json()
+
+        if self._cache is not None:
+            self._cache[path] = resp_json
+
+        return resp_json
 
     def get_release_schedule(self, channel):
         """Get the release schedule for a given channel.
 
         Args:
             channel (str): The channel to get the release schedule for. Can be
                 a version number or one of the beta or nightly keywords.
```

### Comparing `libmozdata-0.2.2/libmozdata/handler.py` & `libmozdata-0.2.3/libmozdata/handler.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/hgmozilla.py` & `libmozdata-0.2.3/libmozdata/hgmozilla.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/lando.py` & `libmozdata-0.2.3/libmozdata/lando.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/modules.json` & `libmozdata-0.2.3/libmozdata/modules.json`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/modules.py` & `libmozdata-0.2.3/libmozdata/modules.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/patchanalysis.py` & `libmozdata-0.2.3/libmozdata/patchanalysis.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/phabricator.py` & `libmozdata-0.2.3/libmozdata/phabricator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 import collections
 import enum
-import functools
 import json
 import logging
 from urllib.parse import urlencode, urlparse
 
 import hglib
 import requests
 
@@ -42,22 +41,14 @@
 class ArtifactType(enum.Enum):
     Host = "host"
     WorkingCopy = "working-copy"
     File = "file"
     Uri = "uri"
 
 
-@functools.lru_cache(maxsize=2048)
-def revision_exists_on_central(revision):
-    url = HGMO_JSON_REV_URL_TEMPLATE.format(revision)
-    resp = requests.get(url)
-    resp.raise_for_status()
-    return resp.ok
-
-
 def revision_available(repo, revision):
     """
     Check if a revision is available on a Mercurial repo
     """
     try:
         repo.identify(revision)
         return True
```

### Comparing `libmozdata-0.2.2/libmozdata/redash.py` & `libmozdata-0.2.3/libmozdata/redash.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/release_owners.py` & `libmozdata-0.2.3/libmozdata/release_owners.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/socorro.py` & `libmozdata-0.2.3/libmozdata/socorro.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/utils.py` & `libmozdata-0.2.3/libmozdata/utils.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/vcs_map.py` & `libmozdata-0.2.3/libmozdata/vcs_map.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/versions.py` & `libmozdata-0.2.3/libmozdata/versions.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata/wiki_parser.py` & `libmozdata-0.2.3/libmozdata/wiki_parser.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/libmozdata.egg-info/SOURCES.txt` & `libmozdata-0.2.3/libmozdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.2/setup.py` & `libmozdata-0.2.3/setup.py`

 * *Files identical despite different names*

