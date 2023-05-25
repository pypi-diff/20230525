# Comparing `tmp/httpbinx-1.2.3.tar.gz` & `tmp/httpbinx-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpbinx-1.2.3.tar", last modified: Mon May 15 16:27:44 2023, max compression
+gzip compressed data, was "httpbinx-1.3.0.tar", last modified: Thu May 25 17:54:34 2023, max compression
```

## Comparing `httpbinx-1.2.3.tar` & `httpbinx-1.3.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:27:44.344097 httpbinx-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-15 16:27:33.000000 httpbinx-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 16:27:33.000000 httpbinx-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-15 16:27:44.340097 httpbinx-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-15 16:27:33.000000 httpbinx-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:27:44.336096 httpbinx-1.2.3/httpbinx/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:27:44.336096 httpbinx-1.2.3/httpbinx/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:27:44.340097 httpbinx-1.2.3/httpbinx/routers/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/routers/anything.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/routers/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/routers/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/routers/dynamicdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/routers/httpmethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/routers/images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:27:44.340097 httpbinx-1.2.3/httpbinx/routers/inspection/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/routers/inspection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/routers/inspection/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/routers/inspection/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/routers/redirects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/routers/responseformats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/routers/statuscodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:27:44.340097 httpbinx-1.2.3/httpbinx/static/
--rw-r--r--   0 runner    (1001) docker     (123)    14058 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/static/UTF-8-demo.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/static/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:27:44.340097 httpbinx-1.2.3/httpbinx/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/static/images/httbinx_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/static/images/httpbinx_cover.png
--rw-r--r--   0 runner    (1001) docker     (123)    35588 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/static/images/jackal.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/static/images/pig_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/static/images/svg_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/static/images/wolf_1.webp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:27:44.340097 httpbinx-1.2.3/httpbinx/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/templates/moby.html
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/templates/sample.xml
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/templates/trackingscripts.html
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-15 16:27:33.000000 httpbinx-1.2.3/httpbinx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:27:44.336096 httpbinx-1.2.3/httpbinx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-15 16:27:44.000000 httpbinx-1.2.3/httpbinx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-15 16:27:44.000000 httpbinx-1.2.3/httpbinx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:27:44.000000 httpbinx-1.2.3/httpbinx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-15 16:27:44.000000 httpbinx-1.2.3/httpbinx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 16:27:44.000000 httpbinx-1.2.3/httpbinx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 16:27:44.344097 httpbinx-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-15 16:27:33.000000 httpbinx-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:34.754466 httpbinx-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-25 17:54:21.000000 httpbinx-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 17:54:21.000000 httpbinx-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-25 17:54:34.754466 httpbinx-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-25 17:54:21.000000 httpbinx-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:34.746466 httpbinx-1.3.0/httpbinx/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:34.750466 httpbinx-1.3.0/httpbinx/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:34.750466 httpbinx-1.3.0/httpbinx/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/anything.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/dynamicdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/httpmethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:34.750466 httpbinx-1.3.0/httpbinx/routers/inspection/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/inspection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/inspection/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/inspection/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/redirects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/responseformats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/statuscodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:34.750466 httpbinx-1.3.0/httpbinx/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14058 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/static/UTF-8-demo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/static/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:34.750466 httpbinx-1.3.0/httpbinx/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/static/images/httbinx_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/static/images/httpbinx_cover.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35588 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/static/images/jackal.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/static/images/pig_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/static/images/svg_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/static/images/wolf_1.webp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:34.754466 httpbinx-1.3.0/httpbinx/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/templates/moby.html
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/templates/sample.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/templates/trackingscripts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:34.746466 httpbinx-1.3.0/httpbinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-25 17:54:34.000000 httpbinx-1.3.0/httpbinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-25 17:54:34.000000 httpbinx-1.3.0/httpbinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:54:34.000000 httpbinx-1.3.0/httpbinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 17:54:34.000000 httpbinx-1.3.0/httpbinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 17:54:34.000000 httpbinx-1.3.0/httpbinx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:54:34.754466 httpbinx-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-25 17:54:21.000000 httpbinx-1.3.0/setup.py
```

### Comparing `httpbinx-1.2.3/LICENSE` & `httpbinx-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/PKG-INFO` & `httpbinx-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: httpbinx
-Version: 1.2.3
+Version: 1.3.0
 Summary: HTTP Request & Response Service, written in Python + FastAPI.
 Home-page: https://github.com/imleowoo/httpbinx
 Author: Leo
 Author-email: imleowoo@outlook.com
 Maintainer: Leo
 Maintainer-email: imleowoo@outlook.com
 License: MIT
 Project-URL: Source, https://github.com/imleowoo/httpbinx
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![cover](httpbinx/static/images/httpbinx_cover.png)
 
 # httpbinx
 HTTP Request & Response Service, written in Python + FastAPI.
```

### Comparing `httpbinx-1.2.3/httpbinx/constants.py` & `httpbinx-1.3.0/httpbinx/constants.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/helpers.py` & `httpbinx-1.3.0/httpbinx/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,29 +19,30 @@
 
 
 def get_templates() -> Jinja2Templates:
     """Dependency function that creates and returns a Jinja2 templates instance"""
     return _templates
 
 
-def to_request_info(request: Request, **extras) -> RequestInfo:
+async def to_request_info(request: Request, **extras) -> RequestInfo:
     """Returns model RequestInfo instance"""
+    await request.body()  # Note: Execute `.stream()` only once.
     attrs = RequestAttrs(request=request)
-    info = attrs.request_info
+    info = await attrs.request_info()
     if extras:
         info.extras.update(extras)
     return info
 
 
 def status_code_response(code: int) -> Response:
     """Returns response object of given status code."""
     # sample redirect
     redirect = dict(headers=dict(location=REDIRECT_LOCATION))
 
-    # https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Status
+    # https://developer.mozilla.org/en-US/docs/Web/HTTP/Status
     code_map = {
         status.HTTP_301_MOVED_PERMANENTLY: redirect,
         status.HTTP_302_FOUND: redirect,
         status.HTTP_303_SEE_OTHER: redirect,
         status.HTTP_304_NOT_MODIFIED: dict(data=''),
         status.HTTP_305_USE_PROXY: redirect,
         status.HTTP_307_TEMPORARY_REDIRECT: redirect,
```

### Comparing `httpbinx-1.2.3/httpbinx/main.py` & `httpbinx-1.3.0/httpbinx/main.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/routers/__init__.py` & `httpbinx-1.3.0/httpbinx/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/routers/anything.py` & `httpbinx-1.3.0/httpbinx/routers/anything.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
     '/anything',  # TODO path regex
     response_model=RequestInfo,
     summary='Returns anything passed in request data.',
     response_description='Anything passed in request',
     methods=['GET', 'POST', 'PUT', 'DELETE', 'PATCH', 'TRACE']
 )
 async def anything(request: Request):
-    return to_request_info(request)
+    return await to_request_info(request)
```

### Comparing `httpbinx-1.2.3/httpbinx/routers/auth.py` & `httpbinx-1.3.0/httpbinx/routers/auth.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/routers/cookies.py` & `httpbinx-1.3.0/httpbinx/routers/cookies.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/routers/dynamicdata.py` & `httpbinx-1.3.0/httpbinx/routers/dynamicdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 )
 async def delay_response(
         *,
         delay: float = Path(..., ge=0, le=10, description='delay seconds'),
         request: Request
 ):
     await asyncio.sleep(delay)
-    return to_request_info(request)
+    return await to_request_info(request)
 
 
 @router.get(
     '/drip',
     response_class=StreamingResponse,
     summary='Drips data over a duration after an optional initial delay.',
     response_description='A dripped response.'
```

### Comparing `httpbinx-1.2.3/httpbinx/routers/httpmethods.py` & `httpbinx-1.3.0/httpbinx/routers/httpmethods.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,59 +2,59 @@
 """HTTP Methods"""
 from fastapi import APIRouter
 from starlette.requests import Request
 
 from httpbinx.helpers import to_request_info
 from httpbinx.schemas import RequestInfo
 
-router = APIRouter(tags=['HTTP Methods'],)
+router = APIRouter(tags=['HTTP Methods'])
 
 
 @router.get(
     '/get',
     response_model=RequestInfo,
     response_model_include={'url', 'args', 'headers', 'origin'},
     summary="The request's query parameters.",
     response_description="The request's query parameters."
 )
 async def get(request: Request):
-    return to_request_info(request)
+    return await to_request_info(request)
 
 
 @router.post(
     '/post',
     response_model=RequestInfo,
     summary="The request's POST parameters.",
     response_description="The request's POST parameters."
 )
 async def post(request: Request):
-    return to_request_info(request)
+    return await to_request_info(request)
 
 
 @router.put(
     '/put',
     response_model=RequestInfo,
     summary="The request's PUT parameters.",
     response_description="The request's PUT parameters."
 )
 async def put(request: Request):
-    return to_request_info(request)
+    return await to_request_info(request)
 
 
 @router.delete(
     '/delete',
     response_model=RequestInfo,
     summary="The request's DELETE parameters.",
     response_description="The request's DELETE parameters."
 )
 async def delete(request: Request):
-    return to_request_info(request)
+    return await to_request_info(request)
 
 
 @router.patch(
     '/patch',
     response_model=RequestInfo,
     summary="The request's PATCH parameters.",
     response_description="The request's PATCH parameters."
 )
 async def patch(request: Request):
-    return to_request_info(request)
+    return await to_request_info(request)
```

### Comparing `httpbinx-1.2.3/httpbinx/routers/images.py` & `httpbinx-1.3.0/httpbinx/routers/images.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/routers/inspection/request.py` & `httpbinx-1.3.0/httpbinx/routers/inspection/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,26 @@
     '/headers',
     response_model=RequestInfo,
     response_model_include={'headers'},
     summary="Return the incoming request's HTTP headers.",
     response_description="The request's headers.",
 )
 async def headers(request: Request):
-    return to_request_info(request)
+    return await to_request_info(request)
 
 
 @router.get(
     '/ip',
     response_model=RequestInfo,
     response_model_include={'origin'},
     summary="Returns the requester's IP Address.",
     response_description="The Requester's IP Address."
 )
 async def ip(request: Request):
-    return to_request_info(request)
+    return await to_request_info(request)
 
 
 @router.get(
     '/user-agent',
     summary="Return the incoming requests's User-Agent header.",
     response_description='The request’s User-Agent header.'
 )
```

### Comparing `httpbinx-1.2.3/httpbinx/routers/inspection/response.py` & `httpbinx-1.3.0/httpbinx/routers/inspection/response.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/routers/redirects.py` & `httpbinx-1.3.0/httpbinx/routers/redirects.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/routers/responseformats.py` & `httpbinx-1.3.0/httpbinx/routers/responseformats.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     summary='Returns Brotli-encoded data.',
     response_model=RequestInfo,
     response_class=JSONResponse,
     response_model_include={'origin', 'headers', 'method', 'extras'},
     response_description='Brotli-encoded data.'
 )
 async def brotli_encoded_content(request: Request):
-    info = to_request_info(request, brotli=True)
+    info = await to_request_info(request, brotli=True)
     response = JSONResponse(jsonable_encoder(info))
     compressed = brotli.compress(response.body or b'')
     response.body = compressed
     response.headers['Content-Encoding'] = 'br'
     response.headers['Content-Length'] = str(len(compressed))
     return response
 
@@ -47,15 +47,15 @@
     summary='Returns Deflate-encoded data.',
     response_model=RequestInfo,
     response_class=JSONResponse,
     response_model_include={'origin', 'headers', 'method', 'extras'},
     response_description='Defalte-encoded data.'
 )
 async def deflate_encoded_content(request: Request):
-    info = to_request_info(request, deflated=True)
+    info = await to_request_info(request, deflated=True)
     response = JSONResponse(jsonable_encoder(info))
     obj = zlib.compressobj()
     deflated = obj.compress(response.body or b'')
     deflated += obj.flush()
     response.body = deflated
     response.headers['Content-Encoding'] = 'deflate'
     response.headers['Content-Length'] = str(len(deflated))
@@ -65,15 +65,15 @@
 @router.get(
     '/gzip',
     response_model=RequestInfo,
     summary='Returns GZip-encoded data.',
     response_description='GZip-encoded data.'
 )
 async def gzip_encoded_content(request: Request):
-    info = to_request_info(request, gzipped=True)
+    info = await to_request_info(request, gzipped=True)
     response = JSONResponse(jsonable_encoder(info))
     compressed = gzip.compress(response.body or b'')
     response.body = compressed
     response.headers['Content-Encoding'] = 'gzip'
     response.headers['Content-Length'] = str(len(compressed))
     return response
```

### Comparing `httpbinx-1.2.3/httpbinx/routers/statuscodes.py` & `httpbinx-1.3.0/httpbinx/routers/statuscodes.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/schemas.py` & `httpbinx-1.3.0/httpbinx/schemas.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from enum import Enum
 from functools import lru_cache
-from typing import Optional
+import json
 from typing import Union
 
 from pydantic import AnyHttpUrl
 from pydantic import BaseModel
 from pydantic import Field
 from starlette.requests import Request
 
@@ -32,20 +32,20 @@
 
     References:
         - AnyHttpUrl vs HttpUrl: https://docs.pydantic.dev/usage/types/#urls
     """
 
     url: AnyHttpUrl = Field(title='Request URL')
     args: dict = Field(default_factory=dict, title='Request Args')
-    form: dict = Field(default_factory=dict, title='Request Form')
-    data: str = Field('', title='Request Data')
     headers: dict = Field(default_factory=dict, title='Request Headers')
     origin: str = Field('', title="Client's IP")
+    form: dict = Field(default_factory=dict, title='Request Form')
+    data: Union[str, bytes] = Field('', title='Request Data')
     files: dict = Field(default_factory=dict, title='Upload Files')
-    json_data: Optional[Union[str, list]] = Field(
+    json_data: Union[dict, list, str] = Field(
         None, alias='json', title='Content-Type: application/json'
     )
     method: HTTPMethod = Field(HTTPMethod.get, title='HTTP Request Method')
     extras: dict = Field(default_factory=dict, title='The Other Information')
 
     @classmethod
     def get_properties(cls):
@@ -91,57 +91,58 @@
                 out[k] = exist.append(v) \
                     if isinstance(exist, list) else [exist, v]
             else:
                 out[k] = v
         return out
 
     @property
-    def form(self):
-        """TODO request form"""
-        return dict()
-
-    @property
-    def data(self):
-        """TODO request data."""
-        return ''
-
-    @property
     def headers(self):
         """request headers."""
         # TODO CaseInsensitiveDict
         return dict(self.request.headers)
 
     @property
     def client_host(self) -> str:
         """request client host."""
         return self.request.client.host
 
     @property
-    def files(self):
-        """TODO request files."""
-        return ''
+    async def data(self):
+        """request data"""
+        return await self.request.body()
 
     @property
-    def json(self):
-        """TODO request json."""
-        return None
+    async def form(self):
+        """request form-data"""
+        return await self.request.form()
+
+    @property
+    async def json(self):
+        """request json"""
+        try:
+            return await self.request.json()
+        except json.decoder.JSONDecodeError:
+            pass
+
+    @property
+    async def files(self):
+        """TODO request files."""
+        return {}
 
     @property
     def user_agent(self) -> str:
         """request headers User-Agent"""
         return self.request.headers.get('User-Agent')
 
-    @property
-    @lru_cache(maxsize=1)
-    def request_info(self) -> RequestInfo:
+    async def request_info(self) -> RequestInfo:
         """fastapi object `Request` to model `RequestInfo`"""
         return RequestInfo(
             url=self.url,
             args=self.args,
-            form=self.form,
-            data=self.data,
             headers=self.headers,
             origin=self.client_host,
-            files=self.files,
-            json_data=self.json,
+            data=await self.data,
+            form=await self.form,
+            files=await self.files,
+            json=await self.json,
             method=self.method,
         )
```

### Comparing `httpbinx-1.2.3/httpbinx/static/UTF-8-demo.txt` & `httpbinx-1.3.0/httpbinx/static/UTF-8-demo.txt`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/static/favicon.png` & `httpbinx-1.3.0/httpbinx/static/favicon.png`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/static/images/httbinx_logo.png` & `httpbinx-1.3.0/httpbinx/static/images/httbinx_logo.png`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/static/images/httpbinx_cover.png` & `httpbinx-1.3.0/httpbinx/static/images/httpbinx_cover.png`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/static/images/jackal.jpg` & `httpbinx-1.3.0/httpbinx/static/images/jackal.jpg`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/static/images/pig_icon.png` & `httpbinx-1.3.0/httpbinx/static/images/pig_icon.png`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/static/images/svg_logo.svg` & `httpbinx-1.3.0/httpbinx/static/images/svg_logo.svg`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/static/images/wolf_1.webp` & `httpbinx-1.3.0/httpbinx/static/images/wolf_1.webp`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/templates/index.html` & `httpbinx-1.3.0/httpbinx/templates/index.html`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/templates/moby.html` & `httpbinx-1.3.0/httpbinx/templates/moby.html`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/templates/sample.xml` & `httpbinx-1.3.0/httpbinx/templates/sample.xml`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx/templates/trackingscripts.html` & `httpbinx-1.3.0/httpbinx/templates/trackingscripts.html`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/httpbinx.egg-info/PKG-INFO` & `httpbinx-1.3.0/httpbinx.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: httpbinx
-Version: 1.2.3
+Version: 1.3.0
 Summary: HTTP Request & Response Service, written in Python + FastAPI.
 Home-page: https://github.com/imleowoo/httpbinx
 Author: Leo
 Author-email: imleowoo@outlook.com
 Maintainer: Leo
 Maintainer-email: imleowoo@outlook.com
 License: MIT
 Project-URL: Source, https://github.com/imleowoo/httpbinx
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![cover](httpbinx/static/images/httpbinx_cover.png)
 
 # httpbinx
 HTTP Request & Response Service, written in Python + FastAPI.
```

### Comparing `httpbinx-1.2.3/httpbinx.egg-info/SOURCES.txt` & `httpbinx-1.3.0/httpbinx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `httpbinx-1.2.3/setup.py` & `httpbinx-1.3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 # -*- coding: utf-8 -*-
-from os.path import dirname
-from os.path import join
+from pathlib import Path
 
 from setuptools import find_packages
 from setuptools import setup
 
-with open(join(dirname(__file__), 'httpbinx', 'VERSION'), 'r') as vf:
-    version = vf.read().strip()
+version = (Path(__file__).parent / 'httpbinx' / 'VERSION').read_text('ascii').strip()
 
 install_requires = [
     'fastapi',
     'pydantic',
     'uvicorn',
     'starlette',
     'jinja2',
     'brotli',
+    'python-multipart'
+]
+
+test_require = [
+    'httpx',  # https://fastapi.tiangolo.com/tutorial/testing/
+    'pytest-cov',
+    'pytest-mock',
+    'pytest-xdist',
+    'pytest',
 ]
 
 setup(
     name='httpbinx',
     version=version,
     description='HTTP Request & Response Service, '
                 'written in Python + FastAPI.',
@@ -36,23 +43,24 @@
     # license
     license='MIT',
 
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     packages=find_packages(
         include=['httpbinx'],
     ),
     include_package_data=True,
     install_requires=install_requires,
-    python_requires='>=3.6',
+    tests_require=test_require,
+    python_requires='>=3.7',
     project_urls={
         'Source': 'https://github.com/imleowoo/httpbinx',
     },
 )
```

