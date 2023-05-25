# Comparing `tmp/streamlit_toggle_switch_aai-4.0.5.tar.gz` & `tmp/streamlit_toggle_switch_aai-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_toggle_switch_aai-4.0.5.tar", last modified: Thu May 25 21:52:50 2023, max compression
+gzip compressed data, was "streamlit_toggle_switch_aai-4.0.6.tar", last modified: Thu May 25 21:59:01 2023, max compression
```

## Comparing `streamlit_toggle_switch_aai-4.0.5.tar` & `streamlit_toggle_switch_aai-4.0.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:52:50.366105 streamlit_toggle_switch_aai-4.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-25 21:52:32.000000 streamlit_toggle_switch_aai-4.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 21:52:32.000000 streamlit_toggle_switch_aai-4.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 21:52:50.366105 streamlit_toggle_switch_aai-4.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-25 21:52:32.000000 streamlit_toggle_switch_aai-4.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:52:50.366105 streamlit_toggle_switch_aai-4.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-25 21:52:32.000000 streamlit_toggle_switch_aai-4.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:52:50.354105 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-25 21:52:32.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:52:50.350105 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:52:50.358105 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-25 21:52:32.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)   197459 2023-05-25 21:52:32.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-25 21:52:32.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-25 21:52:32.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/precache-manifest.b145425464ab33b4bdef1c2fbcd36ce4.js
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-25 21:52:32.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/service-worker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:52:50.354105 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:52:50.358105 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 21:52:32.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/static/css/main.1aeaa329.chunk.css
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 21:52:32.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/static/css/main.1aeaa329.chunk.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:52:50.366105 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   668301 2023-05-25 21:52:32.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-25 21:52:32.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  2233103 2023-05-25 21:52:32.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-25 21:52:32.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-25 21:52:32.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-25 21:52:32.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-05-25 21:52:32.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:52:50.366105 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle_switch_aai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 21:52:50.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle_switch_aai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-25 21:52:50.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle_switch_aai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:52:50.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle_switch_aai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 21:52:50.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle_switch_aai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 21:52:50.000000 streamlit_toggle_switch_aai-4.0.5/streamlit_toggle_switch_aai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:59:01.180015 streamlit_toggle_switch_aai-4.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-25 21:58:50.000000 streamlit_toggle_switch_aai-4.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 21:58:50.000000 streamlit_toggle_switch_aai-4.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 21:59:01.180015 streamlit_toggle_switch_aai-4.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-25 21:58:50.000000 streamlit_toggle_switch_aai-4.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:59:01.180015 streamlit_toggle_switch_aai-4.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-25 21:58:50.000000 streamlit_toggle_switch_aai-4.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:59:01.168015 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-25 21:58:50.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:59:01.168015 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:59:01.172015 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-25 21:58:50.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)   197459 2023-05-25 21:58:50.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-25 21:58:50.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-25 21:58:50.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/precache-manifest.2776bb5194ede4750115f38121622206.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-25 21:58:50.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:59:01.168015 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:59:01.172015 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-25 21:58:50.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/static/css/main.9ae38243.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-25 21:58:50.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/static/css/main.9ae38243.chunk.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:59:01.180015 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   668301 2023-05-25 21:58:50.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-25 21:58:50.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  2233103 2023-05-25 21:58:50.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-25 21:58:50.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-25 21:58:50.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-25 21:58:50.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-05-25 21:58:50.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:59:01.180015 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle_switch_aai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 21:59:01.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle_switch_aai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-25 21:59:01.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle_switch_aai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:59:01.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle_switch_aai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 21:59:01.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle_switch_aai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 21:59:01.000000 streamlit_toggle_switch_aai-4.0.6/streamlit_toggle_switch_aai.egg-info/top_level.txt
```

### Comparing `streamlit_toggle_switch_aai-4.0.5/LICENSE` & `streamlit_toggle_switch_aai-4.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.5/README.md` & `streamlit_toggle_switch_aai-4.0.6/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.5/setup.py` & `streamlit_toggle_switch_aai-4.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit_toggle_switch_aai",
-    version="4.0.5",
+    version="4.0.6",
     author="Carlos D. Serrano",
     author_email="sqlinsights@gmail.com",
     description="Creates a customizable toggle",
     long_description="",
     long_description_content_type="text/plain",
     url="https://github.com/sqlinsights/streamlit-toggle-switch",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/__init__.py` & `streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/bootstrap.min.css` & `streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/index.html` & `streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><link href="./static/css/main.1aeaa329.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,i=t[0],a=t[1],f=t[2],p=0,s=[];p<i.length;p++)l=i[p],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in a)Object.prototype.hasOwnProperty.call(a,n)&&(e[n]=a[n]);for(c&&c(t);s.length;)s.shift()();return u.push.apply(u,f||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,i=1;i<r.length;i++){var a=r[i];0!==o[a]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var i=this.webpackJsonpstreamlit_toggle_switch=this.webpackJsonpstreamlit_toggle_switch||[],a=i.push.bind(i);i.push=t,i=i.slice();for(var f=0;f<i.length;f++)t(i[f]);var c=a;r()}([])</script><script src="./static/js/2.449282fd.chunk.js"></script><script src="./static/js/main.c16910cb.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><link href="./static/css/main.9ae38243.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,i=t[0],a=t[1],f=t[2],p=0,s=[];p<i.length;p++)l=i[p],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in a)Object.prototype.hasOwnProperty.call(a,n)&&(e[n]=a[n]);for(c&&c(t);s.length;)s.shift()();return u.push.apply(u,f||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,i=1;i<r.length;i++){var a=r[i];0!==o[a]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var i=this.webpackJsonpstreamlit_toggle_switch=this.webpackJsonpstreamlit_toggle_switch||[],a=i.push.bind(i);i.push=t,i=i.slice();for(var f=0;f<i.length;f++)t(i[f]);var c=a;r()}([])</script><script src="./static/js/2.449282fd.chunk.js"></script><script src="./static/js/main.c16910cb.chunk.js"></script></body></html>
```

### Comparing `streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/precache-manifest.b145425464ab33b4bdef1c2fbcd36ce4.js` & `streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/precache-manifest.2776bb5194ede4750115f38121622206.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 self.__precacheManifest = (self.__precacheManifest || []).concat([{
-    "revision": "4171d7b3200fe62c9f1b3eaec5776447",
+    "revision": "ab63f280601f5302f1585a193064274e",
     "url": "./index.html"
 }, {
-    "revision": "589e8f3e9b489f0ac7d9",
-    "url": "./static/css/main.1aeaa329.chunk.css"
+    "revision": "8ccf9348471a9cde32d6",
+    "url": "./static/css/main.9ae38243.chunk.css"
 }, {
     "revision": "cfe9d6e9d3f4a92105c7",
     "url": "./static/js/2.449282fd.chunk.js"
 }, {
     "revision": "fbabe484400fd249a0740ba2c0d294dd",
     "url": "./static/js/2.449282fd.chunk.js.LICENSE.txt"
 }, {
-    "revision": "589e8f3e9b489f0ac7d9",
+    "revision": "8ccf9348471a9cde32d6",
     "url": "./static/js/main.c16910cb.chunk.js"
 }, {
     "revision": "5ab337871dec8eeaf644",
     "url": "./static/js/runtime-main.fd5c39a2.js"
 }]);
```

### Comparing `streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/service-worker.js` & `streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/service-worker.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
  * and re-run your build process.
  * See https://goo.gl/2aRDsh
  */
 
 importScripts("https://storage.googleapis.com/workbox-cdn/releases/4.3.1/workbox-sw.js");
 
 importScripts(
-    "./precache-manifest.b145425464ab33b4bdef1c2fbcd36ce4.js"
+    "./precache-manifest.2776bb5194ede4750115f38121622206.js"
 );
 
 self.addEventListener('message', (event) => {
     if (event.data && event.data.type === 'SKIP_WAITING') {
         self.skipWaiting();
     }
 });
```

### Comparing `streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js` & `streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.LICENSE.txt` & `streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.map` & `streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js` & `streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js.map` & `streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9523809523809524%*

 * *Differences: {"'sourcesContent'": "{insert: [(0, 'import {\\n  ComponentProps,\\n  Streamlit,\\n  "*

 * *                     'withStreamlitConnection,\\n} from "streamlit-component-lib"\\nimport React, '*

 * *                     '{ useEffect } from "react"\\nimport { createTheme } from '*

 * *                     "\\'@material-ui/core/styles\\';\\nimport { Typography,Switch, Grid } from "*

 * *                     '"@material-ui/core";\\nimport { ThemeProvider } from '*

 * *                     "\\'@material-ui/styles\\';\\nimport \\'./style. […]*

```diff
@@ -65,12 +65,12 @@
     ],
     "sourceRoot": "",
     "sources": [
         "streamlit_toggle.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
-        "import {\n  ComponentProps,\n  Streamlit,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { useEffect } from \"react\"\nimport { createTheme } from '@material-ui/core/styles';\nimport { Typography,Switch, Grid } from \"@material-ui/core\";\nimport { ThemeProvider } from '@material-ui/styles';\nimport './style.css'\n\n\n\nconst StreamlitToogle = (props: ComponentProps) => {\n\n  const {default_value, label_end, label_start,justify, active_color, inactive_color, track_color} = props.args;\n  useEffect(() => Streamlit.setFrameHeight());\n\n\n  const handleChange = (event: React.ChangeEvent<HTMLInputElement>) => {\n    setState({ ...state, [event.target.name]: event.target.checked });\n    Streamlit.setComponentValue(event.target.checked );\n  };\n  const [state, setState] = React.useState({\n      checkStatus: default_value\n  });\n\n  const snowflakeTheme = createTheme({\n    overrides: {\n      MuiSwitch: {\n        switchBase:\n         {\n          // Controls default (unchecked) color for the thumb\n          color: inactive_color\n        },\n        colorSecondary: {\n          \"&$checked\": {\n            // Controls checked color for the thumb\n            color: active_color\n          }\n        },\n        track: {\n          // Controls default (unchecked) color for the track\n          opacity: 0.1,\n          backgroundColor: track_color,\n          \"$checked$checked + &\": {\n            opacity: 1,\n            backgroundColor: track_color,\n\n          }\n        }\n      }\n    }\n  });\n\n  return (\n    <ThemeProvider theme={snowflakeTheme}>\n    <Typography  component=\"div\" variant=\"subtitle1\" paragraph={false} gutterBottom={false}>\n    <Grid component=\"label\" container justifyContent={justify}>\n      <Grid item className=\"beforeText\">{label_start}</Grid>\n      <Grid item>\n      <Switch\n          checked={state.checkStatus}\n          onChange={handleChange}\n          name=\"checkStatus\"/>\n      </Grid>\n      <Grid item className=\"afterText\">{label_end}</Grid> \n    </Grid>\n    </Typography>\n    </ThemeProvider>\n  );\n}\n\nexport default withStreamlitConnection(StreamlitToogle);\n",
+        "import {\n  ComponentProps,\n  Streamlit,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { useEffect } from \"react\"\nimport { createTheme } from '@material-ui/core/styles';\nimport { Typography,Switch, Grid } from \"@material-ui/core\";\nimport { ThemeProvider } from '@material-ui/styles';\nimport './style.css'\n\n\n\nconst StreamlitToogle = (props: ComponentProps) => {\n\n  const {default_value, label_end, label_start,justify, active_color, inactive_color, track_color} = props.args;\n  useEffect(() => Streamlit.setFrameHeight());\n\n\n  const handleChange = (event: React.ChangeEvent<HTMLInputElement>) => {\n    setState({ ...state, [event.target.name]: event.target.checked });\n    Streamlit.setComponentValue(event.target.checked );\n  };\n  const [state, setState] = React.useState({\n      checkStatus: default_value\n  });\n\n  const snowflakeTheme = createTheme({\n    overrides: {\n      MuiSwitch: {\n        switchBase:\n         {\n          // Controls default (unchecked) color for the thumb\n          color: inactive_color\n        },\n        colorSecondary: {\n          \"&$checked\": {\n            // Controls checked color for the thumb\n            color: active_color\n          }\n        },\n        track: {\n          // Controls default (unchecked) color for the track\n          opacity: 0.1,\n          backgroundColor: track_color,\n          \"$checked$checked + &\": {\n            opacity: 1,\n            backgroundColor: track_color,\n\n          }\n        }\n      }\n    }\n  });\n\n  return (\n    <ThemeProvider theme={snowflakeTheme}>\n    <Typography  component=\"div\" variant=\"subtitle1\" paragraph={false} gutterBottom={false}>\n    <Grid component=\"label\" container justifyContent={justify}> \n      <Grid item className=\"beforeText\">{label_start}</Grid>\n      <Grid item>\n      <Switch\n          checked={state.checkStatus}\n          onChange={handleChange}\n          name=\"checkStatus\"/>\n      </Grid>\n      <Grid item className=\"afterText\">{label_end}</Grid> \n    </Grid>\n    </Typography>\n    </ThemeProvider>\n  );\n}\n\nexport default withStreamlitConnection(StreamlitToogle);\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport StreamlitToggleSwitch from \"./streamlit_toggle\"\n\n\nReactDOM.render(\n  <React.StrictMode>\n    <StreamlitToggleSwitch />\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js` & `streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.5/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js.map` & `streamlit_toggle_switch_aai-4.0.6/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.5/streamlit_toggle_switch_aai.egg-info/SOURCES.txt` & `streamlit_toggle_switch_aai-4.0.6/streamlit_toggle_switch_aai.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 MANIFEST.in
 README.md
 setup.py
 streamlit_toggle/__init__.py
 streamlit_toggle/frontend/build/asset-manifest.json
 streamlit_toggle/frontend/build/bootstrap.min.css
 streamlit_toggle/frontend/build/index.html
-streamlit_toggle/frontend/build/precache-manifest.b145425464ab33b4bdef1c2fbcd36ce4.js
+streamlit_toggle/frontend/build/precache-manifest.2776bb5194ede4750115f38121622206.js
 streamlit_toggle/frontend/build/service-worker.js
-streamlit_toggle/frontend/build/static/css/main.1aeaa329.chunk.css
-streamlit_toggle/frontend/build/static/css/main.1aeaa329.chunk.css.map
+streamlit_toggle/frontend/build/static/css/main.9ae38243.chunk.css
+streamlit_toggle/frontend/build/static/css/main.9ae38243.chunk.css.map
 streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js
 streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.LICENSE.txt
 streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.map
 streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js
 streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js.map
 streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js
 streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js.map
```

