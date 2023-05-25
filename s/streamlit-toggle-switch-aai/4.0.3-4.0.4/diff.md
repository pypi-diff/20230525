# Comparing `tmp/streamlit_toggle_switch_aai-4.0.3.tar.gz` & `tmp/streamlit_toggle_switch_aai-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_toggle_switch_aai-4.0.3.tar", last modified: Thu May 25 21:45:29 2023, max compression
+gzip compressed data, was "streamlit_toggle_switch_aai-4.0.4.tar", last modified: Thu May 25 21:47:57 2023, max compression
```

## Comparing `streamlit_toggle_switch_aai-4.0.3.tar` & `streamlit_toggle_switch_aai-4.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:45:29.051698 streamlit_toggle_switch_aai-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-25 21:45:17.000000 streamlit_toggle_switch_aai-4.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 21:45:17.000000 streamlit_toggle_switch_aai-4.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 21:45:29.051698 streamlit_toggle_switch_aai-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-25 21:45:17.000000 streamlit_toggle_switch_aai-4.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:45:29.051698 streamlit_toggle_switch_aai-4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-25 21:45:17.000000 streamlit_toggle_switch_aai-4.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:45:29.047697 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-25 21:45:17.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:45:29.043697 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:45:29.047697 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-25 21:45:17.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)   197459 2023-05-25 21:45:17.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-25 21:45:17.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-25 21:45:17.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/precache-manifest.0698cefac7acc79a5abe6b12ecffb20f.js
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-25 21:45:17.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/service-worker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:45:29.043697 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:45:29.047697 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 21:45:17.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/static/css/main.89a22949.chunk.css
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 21:45:17.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/static/css/main.89a22949.chunk.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:45:29.051698 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   668301 2023-05-25 21:45:17.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-25 21:45:17.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  2233103 2023-05-25 21:45:17.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-25 21:45:17.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-25 21:45:17.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-25 21:45:17.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-05-25 21:45:17.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:45:29.051698 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle_switch_aai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 21:45:28.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle_switch_aai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-25 21:45:29.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle_switch_aai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:45:28.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle_switch_aai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 21:45:28.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle_switch_aai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 21:45:28.000000 streamlit_toggle_switch_aai-4.0.3/streamlit_toggle_switch_aai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:47:57.323648 streamlit_toggle_switch_aai-4.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-25 21:47:46.000000 streamlit_toggle_switch_aai-4.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 21:47:46.000000 streamlit_toggle_switch_aai-4.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 21:47:57.323648 streamlit_toggle_switch_aai-4.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-25 21:47:46.000000 streamlit_toggle_switch_aai-4.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:47:57.323648 streamlit_toggle_switch_aai-4.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-25 21:47:46.000000 streamlit_toggle_switch_aai-4.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:47:57.315648 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-25 21:47:46.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:47:57.315648 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:47:57.319648 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-25 21:47:46.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)   197459 2023-05-25 21:47:46.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-25 21:47:46.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-25 21:47:46.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/precache-manifest.b145425464ab33b4bdef1c2fbcd36ce4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-25 21:47:46.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:47:57.315648 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:47:57.319648 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 21:47:46.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/static/css/main.1aeaa329.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 21:47:46.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/static/css/main.1aeaa329.chunk.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:47:57.323648 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   668301 2023-05-25 21:47:46.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-25 21:47:46.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  2233103 2023-05-25 21:47:46.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-25 21:47:46.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-25 21:47:46.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-25 21:47:46.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-05-25 21:47:46.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:47:57.323648 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle_switch_aai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 21:47:57.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle_switch_aai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-25 21:47:57.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle_switch_aai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:47:57.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle_switch_aai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 21:47:57.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle_switch_aai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 21:47:57.000000 streamlit_toggle_switch_aai-4.0.4/streamlit_toggle_switch_aai.egg-info/top_level.txt
```

### Comparing `streamlit_toggle_switch_aai-4.0.3/LICENSE` & `streamlit_toggle_switch_aai-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.3/README.md` & `streamlit_toggle_switch_aai-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.3/setup.py` & `streamlit_toggle_switch_aai-4.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit_toggle_switch_aai",
-    version="4.0.3",
+    version="4.0.4",
     author="Carlos D. Serrano",
     author_email="sqlinsights@gmail.com",
     description="Creates a customizable toggle",
     long_description="",
     long_description_content_type="text/plain",
     url="https://github.com/sqlinsights/streamlit-toggle-switch",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/__init__.py` & `streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/asset-manifest.json` & `streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/asset-manifest.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8196428571428571%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/css/main.1aeaa329.chunk.css')], delete: [2]}",*

 * * "'files'": "{'main.css': './static/css/main.1aeaa329.chunk.css', "*

 * *            "'precache-manifest.b145425464ab33b4bdef1c2fbcd36ce4.js': "*

 * *            "'./precache-manifest.b145425464ab33b4bdef1c2fbcd36ce4.js', "*

 * *            "'static/css/main.1aeaa329.chunk.css.map': './static/css/main.1aeaa329.chunk.css.map', "*

 * *            "delete: ['precache-manifest.0698cefac7acc79a5abe6b12ecffb20f.js', "*

 * *            "'static/css/mai […]*

```diff
@@ -1,22 +1,22 @@
 {
     "entrypoints": [
         "static/js/runtime-main.fd5c39a2.js",
         "static/js/2.449282fd.chunk.js",
-        "static/css/main.89a22949.chunk.css",
+        "static/css/main.1aeaa329.chunk.css",
         "static/js/main.c16910cb.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.css": "./static/css/main.89a22949.chunk.css",
+        "main.css": "./static/css/main.1aeaa329.chunk.css",
         "main.js": "./static/js/main.c16910cb.chunk.js",
         "main.js.map": "./static/js/main.c16910cb.chunk.js.map",
-        "precache-manifest.0698cefac7acc79a5abe6b12ecffb20f.js": "./precache-manifest.0698cefac7acc79a5abe6b12ecffb20f.js",
+        "precache-manifest.b145425464ab33b4bdef1c2fbcd36ce4.js": "./precache-manifest.b145425464ab33b4bdef1c2fbcd36ce4.js",
         "runtime-main.js": "./static/js/runtime-main.fd5c39a2.js",
         "runtime-main.js.map": "./static/js/runtime-main.fd5c39a2.js.map",
         "service-worker.js": "./service-worker.js",
-        "static/css/main.89a22949.chunk.css.map": "./static/css/main.89a22949.chunk.css.map",
+        "static/css/main.1aeaa329.chunk.css.map": "./static/css/main.1aeaa329.chunk.css.map",
         "static/js/2.449282fd.chunk.js": "./static/js/2.449282fd.chunk.js",
         "static/js/2.449282fd.chunk.js.LICENSE.txt": "./static/js/2.449282fd.chunk.js.LICENSE.txt",
         "static/js/2.449282fd.chunk.js.map": "./static/js/2.449282fd.chunk.js.map"
     }
 }
```

### Comparing `streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/bootstrap.min.css` & `streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/index.html` & `streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><link href="./static/css/main.89a22949.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,i=t[0],a=t[1],f=t[2],p=0,s=[];p<i.length;p++)l=i[p],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in a)Object.prototype.hasOwnProperty.call(a,n)&&(e[n]=a[n]);for(c&&c(t);s.length;)s.shift()();return u.push.apply(u,f||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,i=1;i<r.length;i++){var a=r[i];0!==o[a]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var i=this.webpackJsonpstreamlit_toggle_switch=this.webpackJsonpstreamlit_toggle_switch||[],a=i.push.bind(i);i.push=t,i=i.slice();for(var f=0;f<i.length;f++)t(i[f]);var c=a;r()}([])</script><script src="./static/js/2.449282fd.chunk.js"></script><script src="./static/js/main.c16910cb.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><link href="./static/css/main.1aeaa329.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,i=t[0],a=t[1],f=t[2],p=0,s=[];p<i.length;p++)l=i[p],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in a)Object.prototype.hasOwnProperty.call(a,n)&&(e[n]=a[n]);for(c&&c(t);s.length;)s.shift()();return u.push.apply(u,f||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,i=1;i<r.length;i++){var a=r[i];0!==o[a]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var i=this.webpackJsonpstreamlit_toggle_switch=this.webpackJsonpstreamlit_toggle_switch||[],a=i.push.bind(i);i.push=t,i=i.slice();for(var f=0;f<i.length;f++)t(i[f]);var c=a;r()}([])</script><script src="./static/js/2.449282fd.chunk.js"></script><script src="./static/js/main.c16910cb.chunk.js"></script></body></html>
```

### Comparing `streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/precache-manifest.0698cefac7acc79a5abe6b12ecffb20f.js` & `streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/precache-manifest.b145425464ab33b4bdef1c2fbcd36ce4.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 self.__precacheManifest = (self.__precacheManifest || []).concat([{
-    "revision": "3ce2148ea4430ec1555283c5988fcda3",
+    "revision": "4171d7b3200fe62c9f1b3eaec5776447",
     "url": "./index.html"
 }, {
-    "revision": "b062545f00d158fc553c",
-    "url": "./static/css/main.89a22949.chunk.css"
+    "revision": "589e8f3e9b489f0ac7d9",
+    "url": "./static/css/main.1aeaa329.chunk.css"
 }, {
     "revision": "cfe9d6e9d3f4a92105c7",
     "url": "./static/js/2.449282fd.chunk.js"
 }, {
     "revision": "fbabe484400fd249a0740ba2c0d294dd",
     "url": "./static/js/2.449282fd.chunk.js.LICENSE.txt"
 }, {
-    "revision": "b062545f00d158fc553c",
+    "revision": "589e8f3e9b489f0ac7d9",
     "url": "./static/js/main.c16910cb.chunk.js"
 }, {
     "revision": "5ab337871dec8eeaf644",
     "url": "./static/js/runtime-main.fd5c39a2.js"
 }]);
```

### Comparing `streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/service-worker.js` & `streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/service-worker.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
  * and re-run your build process.
  * See https://goo.gl/2aRDsh
  */
 
 importScripts("https://storage.googleapis.com/workbox-cdn/releases/4.3.1/workbox-sw.js");
 
 importScripts(
-    "./precache-manifest.0698cefac7acc79a5abe6b12ecffb20f.js"
+    "./precache-manifest.b145425464ab33b4bdef1c2fbcd36ce4.js"
 );
 
 self.addEventListener('message', (event) => {
     if (event.data && event.data.type === 'SKIP_WAITING') {
         self.skipWaiting();
     }
 });
```

### Comparing `streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js` & `streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.LICENSE.txt` & `streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.map` & `streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js` & `streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js.map` & `streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js` & `streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.3/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js.map` & `streamlit_toggle_switch_aai-4.0.4/streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_toggle_switch_aai-4.0.3/streamlit_toggle_switch_aai.egg-info/SOURCES.txt` & `streamlit_toggle_switch_aai-4.0.4/streamlit_toggle_switch_aai.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 MANIFEST.in
 README.md
 setup.py
 streamlit_toggle/__init__.py
 streamlit_toggle/frontend/build/asset-manifest.json
 streamlit_toggle/frontend/build/bootstrap.min.css
 streamlit_toggle/frontend/build/index.html
-streamlit_toggle/frontend/build/precache-manifest.0698cefac7acc79a5abe6b12ecffb20f.js
+streamlit_toggle/frontend/build/precache-manifest.b145425464ab33b4bdef1c2fbcd36ce4.js
 streamlit_toggle/frontend/build/service-worker.js
-streamlit_toggle/frontend/build/static/css/main.89a22949.chunk.css
-streamlit_toggle/frontend/build/static/css/main.89a22949.chunk.css.map
+streamlit_toggle/frontend/build/static/css/main.1aeaa329.chunk.css
+streamlit_toggle/frontend/build/static/css/main.1aeaa329.chunk.css.map
 streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js
 streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.LICENSE.txt
 streamlit_toggle/frontend/build/static/js/2.449282fd.chunk.js.map
 streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js
 streamlit_toggle/frontend/build/static/js/main.c16910cb.chunk.js.map
 streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js
 streamlit_toggle/frontend/build/static/js/runtime-main.fd5c39a2.js.map
```

