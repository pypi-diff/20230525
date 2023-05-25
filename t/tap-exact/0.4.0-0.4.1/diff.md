# Comparing `tmp/tap_exact-0.4.0.tar.gz` & `tmp/tap_exact-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_exact-0.4.0.tar", max compression
+gzip compressed data, was "tap_exact-0.4.1.tar", max compression
```

## Comparing `tap_exact-0.4.0.tar` & `tap_exact-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      932 2023-05-25 08:57:52.556947 tap_exact-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.4.0/tap_exact/__init__.py
--rw-r--r--   0        0        0     2661 2023-05-25 09:03:37.456947 tap_exact-0.4.0/tap_exact/client.py
--rw-r--r--   0        0        0    27526 2023-05-25 09:04:32.326947 tap_exact-0.4.0/tap_exact/streams.py
--rw-r--r--   0        0        0     1727 2023-05-25 08:12:48.176947 tap_exact-0.4.0/tap_exact/tap.py
--rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.4.0/tap_exact/tests/__init__.py
--rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.4.0/tap_exact/tests/test_core.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.4.0/setup.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      932 2023-05-25 10:58:50.606947 tap_exact-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.4.1/tap_exact/__init__.py
+-rw-r--r--   0        0        0     1860 2023-05-25 10:58:44.536947 tap_exact-0.4.1/tap_exact/client.py
+-rw-r--r--   0        0        0    27526 2023-05-25 09:04:32.326947 tap_exact-0.4.1/tap_exact/streams.py
+-rw-r--r--   0        0        0     1727 2023-05-25 08:12:48.176947 tap_exact-0.4.1/tap_exact/tap.py
+-rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.4.1/tap_exact/tests/__init__.py
+-rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.4.1/tap_exact/tests/test_core.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.4.1/setup.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.4.1/PKG-INFO
```

### Comparing `tap_exact-0.4.0/pyproject.toml` & `tap_exact-0.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-exact"
-version = "0.4.0"
+version = "0.4.1"
 description = "`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK."
 authors = ["Janick Otten"]
 keywords = [
     "ELT",
     "Exact Online",
 ]
 license = "Apache 2.0"
```

### Comparing `tap_exact-0.4.0/tap_exact/client.py` & `tap_exact-0.4.1/tap_exact/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,70 +9,50 @@
 from singer_sdk.helpers.jsonpath import extract_jsonpath
 from singer_sdk.streams import Stream
 
 from exactonline.api import ExactApi
 from exactonline.storage.ini import IniStorage
 from exactonline.storage.base import ExactOnlineConfig 
 from singer_sdk.tap_base import Tap
-from singer_sdk.pagination import BaseHATEOASPaginator
 
 from exactonline.resource import GET
 from datetime import datetime
-from time import sleep
+
+import abc
 
 SCHEMAS_DIR = Path(__file__).parent / Path("./schemas")
 
 
 class ExactOnlineStream(Stream):
+    __metaclass__ = abc.ABCMeta
+    
     # The fields that have /Date(unixmilliseconds)/ objects that should be converted into datetime objects
     date_fields = []
 
     """ExactOnline stream class."""
     def __init__(self, tap: Tap) -> None:
         super().__init__(tap)
         storage = IniStorage(self.config.get("config_file_location"))
         self.division = storage.get_division()
         self.conn = ExactApi(storage=storage)
 
-    def get_new_paginator(self) -> BaseHATEOASPaginator:
-        return ExactOnlinePaginator()
-    
+    @abc.abstractmethod
     def get_path(self, context: Optional[dict]) -> str:
         """Return the path of the Exact API"""
-        return NotImplementedError
+        raise NotImplementedError("Please implement this method")
 
     def get_records(self, context: Optional[dict]) -> Iterable[dict]:
         """Return a generator or row-type dictionary objects"""
         
-        # Create paginator instance
-        paginator = self.get_new_paginator()
-
         # Construct the url
         url = 'v1/%d/%s' % (self.division, self.get_path(context))
 
-        # Loop until paginator is finished
-        while not paginator.finished and url is not None:
-            # Execute the request
-            resp = self.conn.rest(GET( url ))
-
-            for row in resp:
-                
-                # We loop through the keys that should be modified
-                for date_field in self.date_fields:
-                    row[date_field] = datetime.fromtimestamp( int(row[date_field][6:-2]) / 1000.0 )
-
-                yield row
-
-            # Get the next page url
-            url = paginator.get_next_url(resp)
-
-            # Sleep 1 second to prevent too many requests per minute
-            sleep(1)
-
+        # Execute the request
+        resp = self.conn.rest(GET( url ))
 
-class ExactOnlinePaginator(BaseHATEOASPaginator):
-    def get_next_url(self, response):
-        # Parse __next from response
-        next_url = response.json().get("__next")
+        for row in resp:
+            
+            # We loop through the keys that should be modified
+            for date_field in self.date_fields:
+                row[date_field] = datetime.fromtimestamp( int(row[date_field][6:-2]) / 1000.0 )
 
-        # Remove url and preceding slash from url, else return None
-        return next_url.remove(self.storage.get_rest_url() + '/', '') if next_url else None
+            yield row
```

### Comparing `tap_exact-0.4.0/tap_exact/streams.py` & `tap_exact-0.4.1/tap_exact/streams.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.4.0/tap_exact/tap.py` & `tap_exact-0.4.1/tap_exact/tap.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.4.0/tap_exact/tests/test_core.py` & `tap_exact-0.4.1/tap_exact/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.4.0/setup.py` & `tap_exact-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'s3': ['fs-s3fs>=1.1.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['tap-exact = tap_exact.tap:TapExactOnline.cli']}
 
 setup_kwargs = {
     'name': 'tap-exact',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': '`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.',
     'long_description': 'None',
     'author': 'Janick Otten',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tap_exact-0.4.0/PKG-INFO` & `tap_exact-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-exact
-Version: 0.4.0
+Version: 0.4.1
 Summary: `tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,Exact Online
 Author: Janick Otten
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

