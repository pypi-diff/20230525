# Comparing `tmp/wrighter-plugins-0.0.1.tar.gz` & `tmp/wrighter-plugins-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrighter-plugins-0.0.1.tar", last modified: Mon Feb 13 21:11:09 2023, max compression
+gzip compressed data, was "wrighter-plugins-0.0.2.tar", last modified: Thu May 25 11:51:05 2023, max compression
```

## Comparing `wrighter-plugins-0.0.1.tar` & `wrighter-plugins-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:11:09.989361 wrighter-plugins-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-13 21:10:59.000000 wrighter-plugins-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-02-13 21:11:09.989361 wrighter-plugins-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-02-13 21:10:59.000000 wrighter-plugins-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 21:11:09.989361 wrighter-plugins-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-02-13 21:10:59.000000 wrighter-plugins-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:11:09.989361 wrighter-plugins-0.0.1/wrighter_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-02-13 21:10:59.000000 wrighter-plugins-0.0.1/wrighter_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-02-13 21:10:59.000000 wrighter-plugins-0.0.1/wrighter_plugins/async_stealth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-02-13 21:10:59.000000 wrighter-plugins-0.0.1/wrighter_plugins/json_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-02-13 21:10:59.000000 wrighter-plugins-0.0.1/wrighter_plugins/network_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-02-13 21:10:59.000000 wrighter-plugins-0.0.1/wrighter_plugins/page_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-02-13 21:10:59.000000 wrighter-plugins-0.0.1/wrighter_plugins/resource_blocker.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-02-13 21:10:59.000000 wrighter-plugins-0.0.1/wrighter_plugins/sync_stealth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:11:09.989361 wrighter-plugins-0.0.1/wrighter_plugins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-02-13 21:11:09.000000 wrighter-plugins-0.0.1/wrighter_plugins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-02-13 21:11:09.000000 wrighter-plugins-0.0.1/wrighter_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 21:11:09.000000 wrighter-plugins-0.0.1/wrighter_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-13 21:11:09.000000 wrighter-plugins-0.0.1/wrighter_plugins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-13 21:11:09.000000 wrighter-plugins-0.0.1/wrighter_plugins.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:51:05.368507 wrighter-plugins-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-25 11:50:51.000000 wrighter-plugins-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-25 11:51:05.368507 wrighter-plugins-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-25 11:50:51.000000 wrighter-plugins-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-25 11:50:51.000000 wrighter-plugins-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:51:05.368507 wrighter-plugins-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:50:51.000000 wrighter-plugins-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:51:05.364507 wrighter-plugins-0.0.2/wrighter_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-25 11:50:51.000000 wrighter-plugins-0.0.2/wrighter_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-25 11:50:51.000000 wrighter-plugins-0.0.2/wrighter_plugins/json_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-25 11:50:51.000000 wrighter-plugins-0.0.2/wrighter_plugins/network_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-25 11:50:51.000000 wrighter-plugins-0.0.2/wrighter_plugins/page_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-25 11:50:51.000000 wrighter-plugins-0.0.2/wrighter_plugins/resource_blocker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-25 11:50:51.000000 wrighter-plugins-0.0.2/wrighter_plugins/stealth_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-25 11:50:51.000000 wrighter-plugins-0.0.2/wrighter_plugins/stealth_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:51:05.368507 wrighter-plugins-0.0.2/wrighter_plugins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-25 11:51:05.000000 wrighter-plugins-0.0.2/wrighter_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-25 11:51:05.000000 wrighter-plugins-0.0.2/wrighter_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:51:05.000000 wrighter-plugins-0.0.2/wrighter_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-25 11:51:05.000000 wrighter-plugins-0.0.2/wrighter_plugins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 11:51:05.000000 wrighter-plugins-0.0.2/wrighter_plugins.egg-info/top_level.txt
```

### Comparing `wrighter-plugins-0.0.1/LICENSE` & `wrighter-plugins-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wrighter-plugins-0.0.1/wrighter_plugins/json_scraper.py` & `wrighter-plugins-0.0.2/wrighter_plugins/json_scraper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import json
 from fnmatch import fnmatch
 from json import JSONDecodeError
 
-from jsonpath_ng import jsonpath, parse
+from jsonpath_ng import parse
 from jsonschema import ValidationError, validate
 from stdl import fs
-from wrighter.plugin import Plugin, Request, Response, page
+from stdl.fs import bytes_readable
+from wrighter.plugin import Plugin, Response, page
 
 
 class JsonScraper(Plugin):
     def __init__(
         self,
         url_pattern: str = "*://*.*/*",
         schema: dict | None = None,
@@ -16,21 +18,17 @@
         verbose: bool = False,
     ) -> None:
         self.verbose = verbose
         super().__init__()
         self.url_pattern = url_pattern
         self.schema = schema
         self.jsonpath = parse(json_path) if json_path else None
-        self.data = []
+        self.data: list[dict] = []
 
-    def log(self, text: str):
-        if self.verbose:
-            print(text)
-
-    def is_schema_valid(self, data: dict):
+    def is_schema_valid(self, data: dict) -> bool:
         if self.schema is None:
             return True
         try:
             validate(data, schema=self.schema)
             return True
         except ValidationError:
             return False
@@ -44,19 +42,30 @@
     def handler(self, response: Response) -> None:
         if not fnmatch(response.url, self.url_pattern):
             return
         try:
             data: dict = response.json()
         except (JSONDecodeError, UnicodeDecodeError):
             return
+        except Exception as e:
+            self.logger.debug(
+                "Unknown exception occured while parsing response as JSON", exception=e
+            )
+            return
+
         if not self.is_schema_valid(data):
+            self.logger.debug(f"JSON response from '{response.url}' doesn't match provided schema")
             return
-        data = self.process_data(data)  # type:ignore
-        if data:
-            self.log(data)
+        json_data = self.process_data(data)  # type:ignore
+        if json_data:
+            self.logger.info(
+                f"Extracted data from '{response.url}'", size=bytes_readable(len(json.dumps(data)))
+            )
+            data = {"data": json_data, "url": response.url}
             self.data.append(data)
 
     def export_data(self, filepath: str) -> None:
+        self.logger.info(f"Exporting extracted data to '{filepath}'")
         fs.json_dump(self.data, filepath)
 
 
 __all__ = ["JsonScraper"]
```

### Comparing `wrighter-plugins-0.0.1/wrighter_plugins/resource_blocker.py` & `wrighter-plugins-0.0.2/wrighter_plugins/resource_blocker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from playwright.sync_api import Page, Route
-from stdl.str_u import FG, colored, BG
-
 from wrighter.plugin import Plugin, context
 
 DEFAULT_RESOURCE_EXCLUSIONS = ["image", "stylesheet", "media", "font", "other"]
 
 
 class ResourceBlocker(Plugin):
     """
@@ -19,24 +17,20 @@
     ) -> None:
         self.url_pattern = url_pattern
         self.blocked_resoruces = blocked_resources
         self.verbose = verbose
 
         super().__init__()
 
-    def log(self, url: str):
-        print(f"{colored('BLOCKED',background= BG.LIGHT_RED)} {url}")
-
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(url_pattern={self.url_pattern}, blocked_resources={self.blocked_resoruces})"
 
     def handler(self, route: Route):
         if route.request.resource_type in self.blocked_resoruces:
-            if self.verbose:
-                self.log(route.request.url)
+            self.logger.info(f"BLOCKED {route.request.url}")
             return route.abort()
         return route.continue_()
 
     @context("on", "page")
     def context_on_page(self, page: Page) -> None:
         page.route(url=self.url_pattern, handler=self.handler)
```

