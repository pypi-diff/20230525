# Comparing `tmp/dash_deckgl-0.1.0.tar.gz` & `tmp/dash_deckgl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_deckgl-0.1.0.tar", last modified: Thu May 25 20:46:48 2023, max compression
+gzip compressed data, was "dash_deckgl-0.1.1.tar", last modified: Thu May 25 20:56:20 2023, max compression
```

## Comparing `dash_deckgl-0.1.0.tar` & `dash_deckgl-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-25 20:46:48.800489 dash_deckgl-0.1.0/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-23 00:50:44.000000 dash_deckgl-0.1.0/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)      226 2023-05-25 20:46:42.000000 dash_deckgl-0.1.0/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)      212 2023-05-25 20:46:48.796489 dash_deckgl-0.1.0/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     3899 2023-05-25 19:30:16.000000 dash_deckgl-0.1.0/README.md
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-25 20:46:48.796489 dash_deckgl-0.1.0/dash_deckgl/
--rw-rw-r--   0 dave      (1000) dave      (1000)     2849 2023-05-25 20:45:14.000000 dash_deckgl-0.1.0/dash_deckgl/DashDeckgl.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2513 2023-05-25 20:45:04.000000 dash_deckgl-0.1.0/dash_deckgl/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)       66 2023-05-25 20:45:14.000000 dash_deckgl-0.1.0/dash_deckgl/_imports_.py
--rw-rw-r--   0 dave      (1000) dave      (1000)  1202621 2023-05-25 20:45:12.000000 dash_deckgl-0.1.0/dash_deckgl/dash_deckgl.min.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    17642 2023-05-25 20:45:12.000000 dash_deckgl-0.1.0/dash_deckgl/deckgl.js
--rw-rw-r--   0 dave      (1000) dave      (1000)     2796 2023-05-25 20:45:14.000000 dash_deckgl-0.1.0/dash_deckgl/metadata.json
--rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-05-25 20:45:13.000000 dash_deckgl-0.1.0/dash_deckgl/package-info.json
--rw-rw-r--   0 dave      (1000) dave      (1000)   800972 2023-05-25 20:45:12.000000 dash_deckgl-0.1.0/dash_deckgl/vendor.js
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-25 20:46:48.796489 dash_deckgl-0.1.0/dash_deckgl.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)      212 2023-05-25 20:46:48.000000 dash_deckgl-0.1.0/dash_deckgl.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      397 2023-05-25 20:46:48.000000 dash_deckgl-0.1.0/dash_deckgl.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-25 20:46:48.000000 dash_deckgl-0.1.0/dash_deckgl.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       12 2023-05-25 20:46:48.000000 dash_deckgl-0.1.0/dash_deckgl.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-05-25 20:13:47.000000 dash_deckgl-0.1.0/package.json
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-05-25 20:46:48.800489 dash_deckgl-0.1.0/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)      510 2023-05-23 00:50:44.000000 dash_deckgl-0.1.0/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-25 20:56:20.692072 dash_deckgl-0.1.1/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-23 00:50:44.000000 dash_deckgl-0.1.1/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)      226 2023-05-25 20:46:42.000000 dash_deckgl-0.1.1/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2026 2023-05-25 20:56:20.692072 dash_deckgl-0.1.1/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3899 2023-05-25 19:30:16.000000 dash_deckgl-0.1.1/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-25 20:56:20.692072 dash_deckgl-0.1.1/dash_deckgl/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2849 2023-05-25 20:45:14.000000 dash_deckgl-0.1.1/dash_deckgl/DashDeckgl.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2513 2023-05-25 20:45:04.000000 dash_deckgl-0.1.1/dash_deckgl/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)       66 2023-05-25 20:45:14.000000 dash_deckgl-0.1.1/dash_deckgl/_imports_.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)  1202621 2023-05-25 20:45:12.000000 dash_deckgl-0.1.1/dash_deckgl/dash_deckgl.min.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)    17642 2023-05-25 20:45:12.000000 dash_deckgl-0.1.1/dash_deckgl/deckgl.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2796 2023-05-25 20:45:14.000000 dash_deckgl-0.1.1/dash_deckgl/metadata.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-05-25 20:45:13.000000 dash_deckgl-0.1.1/dash_deckgl/package-info.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)   800972 2023-05-25 20:45:12.000000 dash_deckgl-0.1.1/dash_deckgl/vendor.js
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-25 20:56:20.692072 dash_deckgl-0.1.1/dash_deckgl.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2026 2023-05-25 20:56:20.000000 dash_deckgl-0.1.1/dash_deckgl.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      397 2023-05-25 20:56:20.000000 dash_deckgl-0.1.1/dash_deckgl.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-25 20:56:20.000000 dash_deckgl-0.1.1/dash_deckgl.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       12 2023-05-25 20:56:20.000000 dash_deckgl-0.1.1/dash_deckgl.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-05-25 20:51:53.000000 dash_deckgl-0.1.1/package.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-05-25 20:56:20.692072 dash_deckgl-0.1.1/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)      653 2023-05-25 20:56:07.000000 dash_deckgl-0.1.1/setup.py
```

### Comparing `dash_deckgl-0.1.0/README.md` & `dash_deckgl-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.1.0/dash_deckgl/DashDeckgl.py` & `dash_deckgl-0.1.1/dash_deckgl/DashDeckgl.py`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.1.0/dash_deckgl/__init__.py` & `dash_deckgl-0.1.1/dash_deckgl/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.1.0/dash_deckgl/dash_deckgl.min.js` & `dash_deckgl-0.1.1/dash_deckgl/dash_deckgl.min.js`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.1.0/dash_deckgl/deckgl.js` & `dash_deckgl-0.1.1/dash_deckgl/deckgl.js`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.1.0/dash_deckgl/metadata.json` & `dash_deckgl-0.1.1/dash_deckgl/metadata.json`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.1.0/dash_deckgl/package-info.json` & `dash_deckgl-0.1.1/dash_deckgl/package-info.json`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.1.0/dash_deckgl/vendor.js` & `dash_deckgl-0.1.1/dash_deckgl/vendor.js`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.1.0/package.json` & `dash_deckgl-0.1.1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.1'"}*

```diff
@@ -66,9 +66,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_deckgl -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

