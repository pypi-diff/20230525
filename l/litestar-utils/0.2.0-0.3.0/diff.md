# Comparing `tmp/litestar_utils-0.2.0.tar.gz` & `tmp/litestar_utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litestar_utils-0.2.0.tar", max compression
+gzip compressed data, was "litestar_utils-0.3.0.tar", max compression
```

## Comparing `litestar_utils-0.2.0.tar` & `litestar_utils-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1096 2023-05-04 13:26:52.978226 litestar_utils-0.2.0/LICENSE
--rw-r--r--   0        0        0      312 2023-05-21 09:17:20.959053 litestar_utils-0.2.0/litestar_utils/__init__.py
--rw-r--r--   0        0        0     1118 2023-05-21 09:17:20.959053 litestar_utils-0.2.0/litestar_utils/text.py
--rw-r--r--   0        0        0     1916 2023-05-04 16:04:09.230309 litestar_utils-0.2.0/litestar_utils/timing.py
--rw-r--r--   0        0        0      562 2023-05-21 09:17:20.959053 litestar_utils-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2629 2023-05-21 09:17:20.959053 litestar_utils-0.2.0/README.md
--rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 litestar_utils-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-05-04 13:26:52.978226 litestar_utils-0.3.0/LICENSE
+-rw-r--r--   0        0        0      430 2023-05-25 08:49:19.450820 litestar_utils-0.3.0/litestar_utils/__init__.py
+-rw-r--r--   0        0        0     1345 2023-05-25 08:49:19.450820 litestar_utils-0.3.0/litestar_utils/https_redirect.py
+-rw-r--r--   0        0        0     1118 2023-05-24 16:24:32.451154 litestar_utils-0.3.0/litestar_utils/text.py
+-rw-r--r--   0        0        0     1916 2023-05-04 16:04:09.230309 litestar_utils-0.3.0/litestar_utils/timing.py
+-rw-r--r--   0        0        0      562 2023-05-25 08:49:19.452494 litestar_utils-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3291 2023-05-25 08:49:19.449831 litestar_utils-0.3.0/README.md
+-rw-r--r--   0        0        0     3687 1970-01-01 00:00:00.000000 litestar_utils-0.3.0/PKG-INFO
```

### Comparing `litestar_utils-0.2.0/LICENSE` & `litestar_utils-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `litestar_utils-0.2.0/litestar_utils/text.py` & `litestar_utils-0.3.0/litestar_utils/text.py`

 * *Files identical despite different names*

### Comparing `litestar_utils-0.2.0/litestar_utils/timing.py` & `litestar_utils-0.3.0/litestar_utils/timing.py`

 * *Files identical despite different names*

### Comparing `litestar_utils-0.2.0/pyproject.toml` & `litestar_utils-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "litestar-utils"
-version = "0.2.0"
+version = "0.3.0"
 description = "Utilities for the Litestar framework."
 authors = ["Alessandro Ferrini <alessandro.ferrini@apptecsrl.com>"]
 readme = "README.md"
 packages = [{include = "litestar_utils"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `litestar_utils-0.2.0/README.md` & `litestar_utils-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -97,7 +97,31 @@
 
 expected = "emailatexmapledotcom"
 input_string = "email@exmaple.com"
 options = SlugifyOptions(replacements=[("@", "at"), [".", "dot"]])
 assert slugify(input_string, options=options) == expected
 
 ```
+### HTTPS Redirect Middleware:
+Use the `HTTPSRedirectMiddleware` middleware to redirect all the incoming requests from `http` or `ws` to `https` or `wss`.
+
+Ported from [starlette HTTPSRedirectMiddleware](https://www.starlette.io/middleware/#httpsredirectmiddleware)
+
+```python
+from litestar import Litestar, get
+from litestar_utils import HTTPSRedirectMiddleware
+
+
+@get("/")
+async def hello_world() -> str:
+    return "Hello, world!"
+
+
+@get("/base", exclude_timing=True)
+async def base_all() -> str:
+    return "All your base are belong to us"
+
+app = Litestar(
+    [hello_world, base_all],
+    middleware=[HTTPSRedirectMiddleware],
+)
+```
```

### Comparing `litestar_utils-0.2.0/PKG-INFO` & `litestar_utils-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litestar-utils
-Version: 0.2.0
+Version: 0.3.0
 Summary: Utilities for the Litestar framework.
 Author: Alessandro Ferrini
 Author-email: alessandro.ferrini@apptecsrl.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -112,8 +112,32 @@
 
 expected = "emailatexmapledotcom"
 input_string = "email@exmaple.com"
 options = SlugifyOptions(replacements=[("@", "at"), [".", "dot"]])
 assert slugify(input_string, options=options) == expected
 
 ```
+### HTTPS Redirect Middleware:
+Use the `HTTPSRedirectMiddleware` middleware to redirect all the incoming requests from `http` or `ws` to `https` or `wss`.
+
+Ported from [starlette HTTPSRedirectMiddleware](https://www.starlette.io/middleware/#httpsredirectmiddleware)
+
+```python
+from litestar import Litestar, get
+from litestar_utils import HTTPSRedirectMiddleware
+
+
+@get("/")
+async def hello_world() -> str:
+    return "Hello, world!"
+
+
+@get("/base", exclude_timing=True)
+async def base_all() -> str:
+    return "All your base are belong to us"
+
+app = Litestar(
+    [hello_world, base_all],
+    middleware=[HTTPSRedirectMiddleware],
+)
+```
```

