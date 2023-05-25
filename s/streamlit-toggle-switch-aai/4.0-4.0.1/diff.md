# Comparing `tmp/streamlit_toggle_switch_aai-4.0.tar.gz` & `tmp/streamlit_toggle_switch_aai-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_toggle_switch_aai-4.0.tar", last modified: Thu May 25 21:22:39 2023, max compression
+gzip compressed data, was "streamlit_toggle_switch_aai-4.0.1.tar", last modified: Thu May 25 21:37:05 2023, max compression
```

## Comparing `streamlit_toggle_switch_aai-4.0.tar` & `streamlit_toggle_switch_aai-4.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:22:39.098255 streamlit_toggle_switch_aai-4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-25 21:22:27.000000 streamlit_toggle_switch_aai-4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 21:22:27.000000 streamlit_toggle_switch_aai-4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 21:22:39.098255 streamlit_toggle_switch_aai-4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-25 21:22:27.000000 streamlit_toggle_switch_aai-4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:22:39.098255 streamlit_toggle_switch_aai-4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-25 21:22:27.000000 streamlit_toggle_switch_aai-4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:22:39.090255 streamlit_toggle_switch_aai-4.0/streamlit_toggle/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-25 21:22:27.000000 streamlit_toggle_switch_aai-4.0/streamlit_toggle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:22:39.090255 streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:22:39.094255 streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-25 21:22:27.000000 streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)   197459 2023-05-25 21:22:27.000000 streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-25 21:22:27.000000 streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-25 21:22:27.000000 streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/precache-manifest.0959cad38f1a75e307a821b8795796b0.js
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-25 21:22:27.000000 streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/service-worker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:22:39.090255 streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:22:39.098255 streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   668300 2023-05-25 21:22:27.000000 streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/static/js/2.fd184217.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-25 21:22:27.000000 streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/static/js/2.fd184217.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  2233103 2023-05-25 21:22:27.000000 streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/static/js/2.fd184217.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-25 21:22:27.000000 streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/static/js/main.0725fe9a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-25 21:22:27.000000 streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/static/js/main.0725fe9a.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-25 21:22:27.000000 streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-05-25 21:22:27.000000 streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:22:39.098255 streamlit_toggle_switch_aai-4.0/streamlit_toggle_switch_aai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 21:22:39.000000 streamlit_toggle_switch_aai-4.0/streamlit_toggle_switch_aai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-25 21:22:39.000000 streamlit_toggle_switch_aai-4.0/streamlit_toggle_switch_aai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:22:39.000000 streamlit_toggle_switch_aai-4.0/streamlit_toggle_switch_aai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 21:22:39.000000 streamlit_toggle_switch_aai-4.0/streamlit_toggle_switch_aai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 21:22:39.000000 streamlit_toggle_switch_aai-4.0/streamlit_toggle_switch_aai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:37:05.409325 streamlit_toggle_switch_aai-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-25 21:36:54.000000 streamlit_toggle_switch_aai-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 21:36:54.000000 streamlit_toggle_switch_aai-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 21:37:05.409325 streamlit_toggle_switch_aai-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-25 21:36:54.000000 streamlit_toggle_switch_aai-4.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:37:05.409325 streamlit_toggle_switch_aai-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-25 21:36:54.000000 streamlit_toggle_switch_aai-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:37:05.401324 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-25 21:36:54.000000 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:37:05.401324 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:37:05.405324 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-25 21:36:54.000000 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)   197459 2023-05-25 21:36:54.000000 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-25 21:36:54.000000 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-25 21:36:54.000000 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/precache-manifest.35c58b0385c40a3bc27ede1bf5ca72d3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-25 21:36:54.000000 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:37:05.401324 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:37:05.409325 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   668300 2023-05-25 21:36:54.000000 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/static/js/2.fd184217.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-25 21:36:54.000000 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/static/js/2.fd184217.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  2233103 2023-05-25 21:36:54.000000 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/static/js/2.fd184217.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-25 21:36:54.000000 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/static/js/main.e6714082.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-25 21:36:54.000000 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/static/js/main.e6714082.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-25 21:36:54.000000 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-05-25 21:36:54.000000 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:37:05.409325 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle_switch_aai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 21:37:05.000000 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle_switch_aai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-25 21:37:05.000000 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle_switch_aai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:37:05.000000 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle_switch_aai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 21:37:05.000000 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle_switch_aai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 21:37:05.000000 streamlit_toggle_switch_aai-4.0.1/streamlit_toggle_switch_aai.egg-info/top_level.txt
```

### Comparing `streamlit_toggle_switch_aai-4.0/LICENSE` & `streamlit_toggle_switch_aai-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0/README.md` & `streamlit_toggle_switch_aai-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0/setup.py` & `streamlit_toggle_switch_aai-4.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit_toggle_switch_aai",
-    version="4.0",
+    version="4.0.1",
     author="Carlos D. Serrano",
     author_email="sqlinsights@gmail.com",
     description="Creates a customizable toggle",
     long_description="",
     long_description_content_type="text/plain",
     url="https://github.com/sqlinsights/streamlit-toggle-switch",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_toggle_switch_aai-4.0/streamlit_toggle/__init__.py` & `streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/asset-manifest.json` & `streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/asset-manifest.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8068181818181819%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/main.e6714082.chunk.js')], delete: [2]}",*

 * * "'files'": "{'main.js': './static/js/main.e6714082.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.e6714082.chunk.js.map', "*

 * *            "'precache-manifest.35c58b0385c40a3bc27ede1bf5ca72d3.js': "*

 * *            "'./precache-manifest.35c58b0385c40a3bc27ede1bf5ca72d3.js', delete: "*

 * *            "['precache-manifest.0959cad38f1a75e307a821b8795796b0.js']}"}*

```diff
@@ -1,18 +1,18 @@
 {
     "entrypoints": [
         "static/js/runtime-main.fd5c39a2.js",
         "static/js/2.fd184217.chunk.js",
-        "static/js/main.0725fe9a.chunk.js"
+        "static/js/main.e6714082.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.0725fe9a.chunk.js",
-        "main.js.map": "./static/js/main.0725fe9a.chunk.js.map",
-        "precache-manifest.0959cad38f1a75e307a821b8795796b0.js": "./precache-manifest.0959cad38f1a75e307a821b8795796b0.js",
+        "main.js": "./static/js/main.e6714082.chunk.js",
+        "main.js.map": "./static/js/main.e6714082.chunk.js.map",
+        "precache-manifest.35c58b0385c40a3bc27ede1bf5ca72d3.js": "./precache-manifest.35c58b0385c40a3bc27ede1bf5ca72d3.js",
         "runtime-main.js": "./static/js/runtime-main.fd5c39a2.js",
         "runtime-main.js.map": "./static/js/runtime-main.fd5c39a2.js.map",
         "service-worker.js": "./service-worker.js",
         "static/js/2.fd184217.chunk.js": "./static/js/2.fd184217.chunk.js",
         "static/js/2.fd184217.chunk.js.LICENSE.txt": "./static/js/2.fd184217.chunk.js.LICENSE.txt",
         "static/js/2.fd184217.chunk.js.map": "./static/js/2.fd184217.chunk.js.map"
     }
```

### Comparing `streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/bootstrap.min.css` & `streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/index.html` & `streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,i=t[0],a=t[1],f=t[2],p=0,s=[];p<i.length;p++)l=i[p],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in a)Object.prototype.hasOwnProperty.call(a,n)&&(e[n]=a[n]);for(c&&c(t);s.length;)s.shift()();return u.push.apply(u,f||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,i=1;i<r.length;i++){var a=r[i];0!==o[a]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var i=this.webpackJsonpstreamlit_toggle_switch=this.webpackJsonpstreamlit_toggle_switch||[],a=i.push.bind(i);i.push=t,i=i.slice();for(var f=0;f<i.length;f++)t(i[f]);var c=a;r()}([])</script><script src="./static/js/2.fd184217.chunk.js"></script><script src="./static/js/main.0725fe9a.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,i=t[0],a=t[1],f=t[2],p=0,s=[];p<i.length;p++)l=i[p],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in a)Object.prototype.hasOwnProperty.call(a,n)&&(e[n]=a[n]);for(c&&c(t);s.length;)s.shift()();return u.push.apply(u,f||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,i=1;i<r.length;i++){var a=r[i];0!==o[a]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var i=this.webpackJsonpstreamlit_toggle_switch=this.webpackJsonpstreamlit_toggle_switch||[],a=i.push.bind(i);i.push=t,i=i.slice();for(var f=0;f<i.length;f++)t(i[f]);var c=a;r()}([])</script><script src="./static/js/2.fd184217.chunk.js"></script><script src="./static/js/main.e6714082.chunk.js"></script></body></html>
```

### Comparing `streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/precache-manifest.0959cad38f1a75e307a821b8795796b0.js` & `streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/precache-manifest.35c58b0385c40a3bc27ede1bf5ca72d3.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 self.__precacheManifest = (self.__precacheManifest || []).concat([{
-    "revision": "fbf117520c671719b36f9abd6c3400b0",
+    "revision": "95cdd3a18335c11a574f242e40e68e5a",
     "url": "./index.html"
 }, {
     "revision": "76b67cc7883c1debe40e",
     "url": "./static/js/2.fd184217.chunk.js"
 }, {
     "revision": "fbabe484400fd249a0740ba2c0d294dd",
     "url": "./static/js/2.fd184217.chunk.js.LICENSE.txt"
 }, {
-    "revision": "ed47cea2ba6aee1f7f7a",
-    "url": "./static/js/main.0725fe9a.chunk.js"
+    "revision": "b696b4ca6752a74bf13e",
+    "url": "./static/js/main.e6714082.chunk.js"
 }, {
     "revision": "5ab337871dec8eeaf644",
     "url": "./static/js/runtime-main.fd5c39a2.js"
 }]);
```

### Comparing `streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/service-worker.js` & `streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/service-worker.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
  * and re-run your build process.
  * See https://goo.gl/2aRDsh
  */
 
 importScripts("https://storage.googleapis.com/workbox-cdn/releases/4.3.1/workbox-sw.js");
 
 importScripts(
-    "./precache-manifest.0959cad38f1a75e307a821b8795796b0.js"
+    "./precache-manifest.35c58b0385c40a3bc27ede1bf5ca72d3.js"
 );
 
 self.addEventListener('message', (event) => {
     if (event.data && event.data.type === 'SKIP_WAITING') {
         self.skipWaiting();
     }
 });
```

### Comparing `streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/static/js/2.fd184217.chunk.js` & `streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/static/js/2.fd184217.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/static/js/2.fd184217.chunk.js.LICENSE.txt` & `streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/static/js/2.fd184217.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/static/js/2.fd184217.chunk.js.map` & `streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/static/js/2.fd184217.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/static/js/main.0725fe9a.chunk.js` & `streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/static/js/main.e6714082.chunk.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -12,83 +12,85 @@
                 o = a.n(n),
                 l = a(2),
                 i = a(5),
                 s = a(3),
                 u = a(27),
                 m = a(34),
                 h = a(64),
-                d = a(65),
-                b = a(66),
+                b = a(65),
+                d = a(66),
                 g = a(63),
                 k = Object(u.b)((function(e) {
                     var t = e.args,
                         a = t.default_value,
                         n = t.label_end,
                         o = t.label_start,
                         k = t.justify,
                         p = t.active_color,
-                        E = t.inactive_color,
-                        f = t.track_color;
+                        f = t.inactive_color,
+                        E = t.track_color;
                     Object(c.useEffect)((function() {
                         return u.a.setFrameHeight()
                     }));
                     var _ = r.a.useState({
                             checkStatus: a
                         }),
                         j = Object(l.a)(_, 2),
                         v = j[0],
                         O = j[1],
                         S = Object(m.a)({
                             overrides: {
                                 MuiSwitch: {
                                     switchBase: {
-                                        color: E
+                                        color: f
                                     },
                                     colorSecondary: {
                                         "&$checked": {
                                             color: p
                                         }
                                     },
                                     track: {
                                         opacity: .1,
-                                        backgroundColor: f,
+                                        backgroundColor: E,
                                         "$checked$checked + &": {
                                             opacity: 1,
-                                            backgroundColor: f
+                                            backgroundColor: E
                                         }
                                     }
                                 }
                             }
                         });
                     return r.a.createElement(g.a, {
                         theme: S
                     }, r.a.createElement(h.a, {
                         component: "div",
                         variant: "subtitle1",
                         paragraph: !1,
                         gutterBottom: !1
-                    }, r.a.createElement(d.a, {
+                    }, r.a.createElement(b.a, {
                         component: "label",
                         container: !0,
                         justifyContent: k
-                    }, r.a.createElement(d.a, {
-                        item: !0
-                    }, o), r.a.createElement(d.a, {
-                        item: !0
                     }, r.a.createElement(b.a, {
+                        item: !0,
+                        className: "beforeText"
+                    }, o), r.a.createElement(b.a, {
+                        item: !0
+                    }, r.a.createElement(d.a, {
                         checked: v.checkStatus,
                         onChange: function(e) {
                             O(Object(s.a)(Object(s.a)({}, v), {}, Object(i.a)({}, e.target.name, e.target.checked))), u.a.setComponentValue(e.target.checked)
                         },
                         name: "checkStatus"
-                    })), r.a.createElement(d.a, {
-                        item: !0
+                    })), r.a.createElement(b.a, {
+                        item: !0,
+                        className: "afterText"
                     }, n))))
                 }));
             o.a.render(r.a.createElement(r.a.StrictMode, null, r.a.createElement(k, null)), document.getElementById("root"))
         }
     },
     [
         [38, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.0725fe9a.chunk.js.map
+//# sourceMappingURL=main.e6714082.chunk.js.map
```

### Comparing `streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/static/js/main.0725fe9a.chunk.js.map` & `streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/static/js/main.e6714082.chunk.js.map`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8083333333333333%*

 * *Differences: {"'file'": "'static/js/main.e6714082.chunk.js'",*

 * * "'mappings'": "'wRAwEeA,eA5DS,SAACC,GAEvB,IAAAC,EAAmGD,EAAME,KAAlGC,EAAaF,EAAbE,cAAeC,EAASH,EAATG,UAAWC,EAAWJ,EAAXI,YAAYC,EAAOL,EAAPK,QAASC,EAAYN,EAAZM,aAAcC,EAAcP,EAAdO,eAAgBC,EAAWR,EAAXQ,YACpFC,qBAAU,kBAAMC,IAAUC,oBAG1B,IAIAC,EAA0BC,IAAMC,SAAS,CACrCC,YAAab,IACfc,EAAAC,YAAAL,EAAA,GAFKM,EAAKF,EAAA,GAAEG,EAAQH,EAAA,GAIhBI,EAAiBC,YAAY,CACjCC,UAAW,CACTC,UAAW,CACTC,WACC,CAECC,MAAOlB,GAETmB,eAAgB,CACd,YAAa,CAEXD,MAAOnB,IAGXqB,MAAO,CAELC,QAAS,GACTC,gBAAiBrB,EACjB, […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.0725fe9a.chunk.js",
-    "mappings": "wRAwEeA,eA5DS,SAACC,GAEvB,IAAAC,EAAmGD,EAAME,KAAlGC,EAAaF,EAAbE,cAAeC,EAASH,EAATG,UAAWC,EAAWJ,EAAXI,YAAYC,EAAOL,EAAPK,QAASC,EAAYN,EAAZM,aAAcC,EAAcP,EAAdO,eAAgBC,EAAWR,EAAXQ,YACpFC,qBAAU,kBAAMC,IAAUC,oBAG1B,IAIAC,EAA0BC,IAAMC,SAAS,CACrCC,YAAab,IACfc,EAAAC,YAAAL,EAAA,GAFKM,EAAKF,EAAA,GAAEG,EAAQH,EAAA,GAIhBI,EAAiBC,YAAY,CACjCC,UAAW,CACTC,UAAW,CACTC,WACC,CAECC,MAAOlB,GAETmB,eAAgB,CACd,YAAa,CAEXD,MAAOnB,IAGXqB,MAAO,CAELC,QAAS,GACTC,gBAAiBrB,EACjB,uBAAwB,CACtBoB,QAAS,EACTC,gBAAiBrB,QAQ3B,OACEK,IAAAiB,cAACC,IAAa,CAACC,MAAOZ,GACtBP,IAAAiB,cAACG,IAAU,CAAEC,UAAU,MAAMC,QAAQ,YAAYC,WAAW,EAAOC,cAAc,GACjFxB,IAAAiB,cAACQ,IAAI,CAACJ,UAAU,QAAQK,WAAS,EAACC,eAAgBnC,GAChDQ,IAAAiB,cAACQ,IAAI,CAACG,MAAI,GAAGrC,GACbS,IAAAiB,cAACQ,IAAI,CAACG,MAAI,GACV5B,IAAAiB,cAACY,IAAM,CACHC,QAASzB,EAAMH,YACf6B,SA5Ca,SAACC,GACpB1B,EAAQ2B,wBAAC,GAAK5B,GAAK,GAAA6B,YAAA,GAAGF,EAAMG,OAAOC,KAAOJ,EAAMG,OAAOL,WACvDjC,IAAUwC,kBAAkBL,EAAMG,OAAOL,UA2CnCM,KAAK,iBAETpC,IAAAiB,cAACQ,IAAI,CAACG,MAAI,GAAEtC,SC5DlBgD,IAASC,OACPvC,IAAAiB,cAACjB,IAAMwC,WAAU,KACfxC,IAAAiB,cAACwB,EAAqB,OAExBC,SAASC,eAAe,W",
+    "file": "static/js/main.e6714082.chunk.js",
+    "mappings": "wRAwEeA,eA5DS,SAACC,GAEvB,IAAAC,EAAmGD,EAAME,KAAlGC,EAAaF,EAAbE,cAAeC,EAASH,EAATG,UAAWC,EAAWJ,EAAXI,YAAYC,EAAOL,EAAPK,QAASC,EAAYN,EAAZM,aAAcC,EAAcP,EAAdO,eAAgBC,EAAWR,EAAXQ,YACpFC,qBAAU,kBAAMC,IAAUC,oBAG1B,IAIAC,EAA0BC,IAAMC,SAAS,CACrCC,YAAab,IACfc,EAAAC,YAAAL,EAAA,GAFKM,EAAKF,EAAA,GAAEG,EAAQH,EAAA,GAIhBI,EAAiBC,YAAY,CACjCC,UAAW,CACTC,UAAW,CACTC,WACC,CAECC,MAAOlB,GAETmB,eAAgB,CACd,YAAa,CAEXD,MAAOnB,IAGXqB,MAAO,CAELC,QAAS,GACTC,gBAAiBrB,EACjB,uBAAwB,CACtBoB,QAAS,EACTC,gBAAiBrB,QAQ3B,OACEK,IAAAiB,cAACC,IAAa,CAACC,MAAOZ,GACtBP,IAAAiB,cAACG,IAAU,CAAEC,UAAU,MAAMC,QAAQ,YAAYC,WAAW,EAAOC,cAAc,GACjFxB,IAAAiB,cAACQ,IAAI,CAACJ,UAAU,QAAQK,WAAS,EAACC,eAAgBnC,GAChDQ,IAAAiB,cAACQ,IAAI,CAACG,MAAI,EAACC,UAAU,cAActC,GACnCS,IAAAiB,cAACQ,IAAI,CAACG,MAAI,GACV5B,IAAAiB,cAACa,IAAM,CACHC,QAAS1B,EAAMH,YACf8B,SA5Ca,SAACC,GACpB3B,EAAQ4B,wBAAC,GAAK7B,GAAK,GAAA8B,YAAA,GAAGF,EAAMG,OAAOC,KAAOJ,EAAMG,OAAOL,WACvDlC,IAAUyC,kBAAkBL,EAAMG,OAAOL,UA2CnCM,KAAK,iBAETrC,IAAAiB,cAACQ,IAAI,CAACG,MAAI,EAACC,UAAU,aAAavC,SC5DxCiD,IAASC,OACPxC,IAAAiB,cAACjB,IAAMyC,WAAU,KACfzC,IAAAiB,cAACyB,EAAqB,OAExBC,SAASC,eAAe,W",
     "names": [
         "withStreamlitConnection",
         "props",
         "_props$args",
         "args",
         "default_value",
         "label_end",
@@ -42,14 +42,15 @@
         "variant",
         "paragraph",
         "gutterBottom",
         "Grid",
         "container",
         "justifyContent",
         "item",
+        "className",
         "Switch",
         "checked",
         "onChange",
         "event",
         "_objectSpread",
         "_defineProperty",
         "target",
@@ -64,12 +65,12 @@
     ],
     "sourceRoot": "",
     "sources": [
         "streamlit_toggle.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
-        "import {\n  ComponentProps,\n  Streamlit,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { useEffect } from \"react\"\nimport { createTheme } from '@material-ui/core/styles';\nimport { Typography,Switch, Grid } from \"@material-ui/core\";\nimport { ThemeProvider } from '@material-ui/styles';\n\n\n\nconst StreamlitToogle = (props: ComponentProps) => {\n\n  const {default_value, label_end, label_start,justify, active_color, inactive_color, track_color} = props.args;\n  useEffect(() => Streamlit.setFrameHeight());\n\n\n  const handleChange = (event: React.ChangeEvent<HTMLInputElement>) => {\n    setState({ ...state, [event.target.name]: event.target.checked });\n    Streamlit.setComponentValue(event.target.checked );\n  };\n  const [state, setState] = React.useState({\n      checkStatus: default_value\n  });\n\n  const snowflakeTheme = createTheme({\n    overrides: {\n      MuiSwitch: {\n        switchBase:\n         {\n          // Controls default (unchecked) color for the thumb\n          color: inactive_color\n        },\n        colorSecondary: {\n          \"&$checked\": {\n            // Controls checked color for the thumb\n            color: active_color\n          }\n        },\n        track: {\n          // Controls default (unchecked) color for the track\n          opacity: 0.1,\n          backgroundColor: track_color,\n          \"$checked$checked + &\": {\n            opacity: 1,\n            backgroundColor: track_color,\n\n          }\n        }\n      }\n    }\n  });\n\n  return (\n    <ThemeProvider theme={snowflakeTheme}>\n    <Typography  component=\"div\" variant=\"subtitle1\" paragraph={false} gutterBottom={false}>\n    <Grid component=\"label\" container justifyContent={justify}>\n      <Grid item >{label_start}</Grid>\n      <Grid item>\n      <Switch\n          checked={state.checkStatus}\n          onChange={handleChange}\n          name=\"checkStatus\"/>\n      </Grid>\n      <Grid item>{label_end}</Grid> \n    </Grid>\n    </Typography>\n    </ThemeProvider>\n  );\n}\n\nexport default withStreamlitConnection(StreamlitToogle);\n",
+        "import {\n  ComponentProps,\n  Streamlit,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { useEffect } from \"react\"\nimport { createTheme } from '@material-ui/core/styles';\nimport { Typography,Switch, Grid } from \"@material-ui/core\";\nimport { ThemeProvider } from '@material-ui/styles';\n\n\n\nconst StreamlitToogle = (props: ComponentProps) => {\n\n  const {default_value, label_end, label_start,justify, active_color, inactive_color, track_color} = props.args;\n  useEffect(() => Streamlit.setFrameHeight());\n\n\n  const handleChange = (event: React.ChangeEvent<HTMLInputElement>) => {\n    setState({ ...state, [event.target.name]: event.target.checked });\n    Streamlit.setComponentValue(event.target.checked );\n  };\n  const [state, setState] = React.useState({\n      checkStatus: default_value\n  });\n\n  const snowflakeTheme = createTheme({\n    overrides: {\n      MuiSwitch: {\n        switchBase:\n         {\n          // Controls default (unchecked) color for the thumb\n          color: inactive_color\n        },\n        colorSecondary: {\n          \"&$checked\": {\n            // Controls checked color for the thumb\n            color: active_color\n          }\n        },\n        track: {\n          // Controls default (unchecked) color for the track\n          opacity: 0.1,\n          backgroundColor: track_color,\n          \"$checked$checked + &\": {\n            opacity: 1,\n            backgroundColor: track_color,\n\n          }\n        }\n      }\n    }\n  });\n\n  return (\n    <ThemeProvider theme={snowflakeTheme}>\n    <Typography  component=\"div\" variant=\"subtitle1\" paragraph={false} gutterBottom={false}>\n    <Grid component=\"label\" container justifyContent={justify}>\n      <Grid item className=\"beforeText\">{label_start}</Grid>\n      <Grid item>\n      <Switch\n          checked={state.checkStatus}\n          onChange={handleChange}\n          name=\"checkStatus\"/>\n      </Grid>\n      <Grid item className=\"afterText\">{label_end}</Grid> \n    </Grid>\n    </Typography>\n    </ThemeProvider>\n  );\n}\n\nexport default withStreamlitConnection(StreamlitToogle);\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport StreamlitToggleSwitch from \"./streamlit_toggle\"\n\n\nReactDOM.render(\n  <React.StrictMode>\n    <StreamlitToggleSwitch />\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js` & `streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js.map` & `streamlit_toggle_switch_aai-4.0.1/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0/streamlit_toggle_switch_aai.egg-info/SOURCES.txt` & `streamlit_toggle_switch_aai-4.0.1/streamlit_toggle_switch_aai.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 MANIFEST.in
 README.md
 setup.py
 streamlit_toggle/__init__.py
 streamlit_toggle/frontend/build/asset-manifest.json
 streamlit_toggle/frontend/build/bootstrap.min.css
 streamlit_toggle/frontend/build/index.html
-streamlit_toggle/frontend/build/precache-manifest.0959cad38f1a75e307a821b8795796b0.js
+streamlit_toggle/frontend/build/precache-manifest.35c58b0385c40a3bc27ede1bf5ca72d3.js
 streamlit_toggle/frontend/build/service-worker.js
 streamlit_toggle/frontend/build/static/js/2.fd184217.chunk.js
 streamlit_toggle/frontend/build/static/js/2.fd184217.chunk.js.LICENSE.txt
 streamlit_toggle/frontend/build/static/js/2.fd184217.chunk.js.map
-streamlit_toggle/frontend/build/static/js/main.0725fe9a.chunk.js
-streamlit_toggle/frontend/build/static/js/main.0725fe9a.chunk.js.map
+streamlit_toggle/frontend/build/static/js/main.e6714082.chunk.js
+streamlit_toggle/frontend/build/static/js/main.e6714082.chunk.js.map
 streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js
 streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js.map
 streamlit_toggle_switch_aai.egg-info/PKG-INFO
 streamlit_toggle_switch_aai.egg-info/SOURCES.txt
 streamlit_toggle_switch_aai.egg-info/dependency_links.txt
 streamlit_toggle_switch_aai.egg-info/requires.txt
 streamlit_toggle_switch_aai.egg-info/top_level.txt
```

