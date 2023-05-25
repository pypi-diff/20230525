# Comparing `tmp/panoptic-0.0.9.dev2.tar.gz` & `tmp/panoptic-0.0.9.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panoptic-0.0.9.dev2.tar", last modified: Thu May 25 09:31:15 2023, max compression
+gzip compressed data, was "panoptic-0.0.9.dev3.tar", last modified: Thu May 25 10:23:56 2023, max compression
```

## Comparing `panoptic-0.0.9.dev2.tar` & `panoptic-0.0.9.dev3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:15.920542 panoptic-0.0.9.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-25 09:31:15.920542 panoptic-0.0.9.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/build_commans.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/description.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:15.912542 panoptic-0.0.9.dev2/panoptic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:15.916542 panoptic-0.0.9.dev2/panoptic/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/compute/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/compute/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/compute/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/compute/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:15.916542 panoptic-0.0.9.dev2/panoptic/core/
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/core/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/core/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/core/image_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:15.916542 panoptic-0.0.9.dev2/panoptic/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:15.916542 panoptic-0.0.9.dev2/panoptic/html/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   121296 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/html/assets/bootstrap-icons-966620f9.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   164352 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/html/assets/bootstrap-icons-c6569d46.woff
--rw-r--r--   0 runner    (1001) docker     (123)   429445 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/html/assets/index-0a222725.css
--rw-r--r--   0 runner    (1001) docker     (123)   257806 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/html/assets/index-7467d80f.js
--rw-r--r--   0 runner    (1001) docker     (123)    67646 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/html/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:15.920542 panoptic-0.0.9.dev2/panoptic/models/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/models/payloads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:15.920542 panoptic-0.0.9.dev2/panoptic/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/scripts/create_db.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/scripts/populate_db.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/panoptic/scripts/to_pca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:15.916542 panoptic-0.0.9.dev2/panoptic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-25 09:31:15.000000 panoptic-0.0.9.dev2/panoptic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-25 09:31:15.000000 panoptic-0.0.9.dev2/panoptic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:31:15.000000 panoptic-0.0.9.dev2/panoptic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-25 09:31:15.000000 panoptic-0.0.9.dev2/panoptic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-25 09:31:15.000000 panoptic-0.0.9.dev2/panoptic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 09:31:15.000000 panoptic-0.0.9.dev2/panoptic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:31:15.920542 panoptic-0.0.9.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-25 09:31:01.000000 panoptic-0.0.9.dev2/thunder-collection_Panoptic.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:23:56.093384 panoptic-0.0.9.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-25 10:23:56.093384 panoptic-0.0.9.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/build_commans.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/description.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:23:56.089384 panoptic-0.0.9.dev3/panoptic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:23:56.089384 panoptic-0.0.9.dev3/panoptic/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/compute/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/compute/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/compute/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/compute/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:23:56.089384 panoptic-0.0.9.dev3/panoptic/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/core/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/core/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/core/image_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:23:56.089384 panoptic-0.0.9.dev3/panoptic/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:23:56.093384 panoptic-0.0.9.dev3/panoptic/html/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   121296 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/html/assets/bootstrap-icons-966620f9.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   164352 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/html/assets/bootstrap-icons-c6569d46.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   429445 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/html/assets/index-0a222725.css
+-rw-r--r--   0 runner    (1001) docker     (123)   257806 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/html/assets/index-7467d80f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    67646 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/html/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:23:56.093384 panoptic-0.0.9.dev3/panoptic/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/models/payloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:23:56.093384 panoptic-0.0.9.dev3/panoptic/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/scripts/create_db.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/scripts/populate_db.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/panoptic/scripts/to_pca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:23:56.089384 panoptic-0.0.9.dev3/panoptic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-25 10:23:56.000000 panoptic-0.0.9.dev3/panoptic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-25 10:23:56.000000 panoptic-0.0.9.dev3/panoptic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 10:23:56.000000 panoptic-0.0.9.dev3/panoptic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-25 10:23:56.000000 panoptic-0.0.9.dev3/panoptic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-25 10:23:56.000000 panoptic-0.0.9.dev3/panoptic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 10:23:56.000000 panoptic-0.0.9.dev3/panoptic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 10:23:56.093384 panoptic-0.0.9.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-25 10:23:37.000000 panoptic-0.0.9.dev3/thunder-collection_Panoptic.json
```

### Comparing `panoptic-0.0.9.dev2/PKG-INFO` & `panoptic-0.0.9.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptic
-Version: 0.0.9.dev2
+Version: 0.0.9.dev3
 License: Mozilla
 Description-Content-Type: text/markdown
 
 # Panoptic
```

### Comparing `panoptic-0.0.9.dev2/description.md` & `panoptic-0.0.9.dev3/description.md`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/api.py` & `panoptic-0.0.9.dev3/panoptic/api.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/compute/ocr.py` & `panoptic-0.0.9.dev3/panoptic/compute/ocr.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/compute/similarity.py` & `panoptic-0.0.9.dev3/panoptic/compute/similarity.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/compute/transform.py` & `panoptic-0.0.9.dev3/panoptic/compute/transform.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/compute/utils.py` & `panoptic-0.0.9.dev3/panoptic/compute/utils.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/core/__init__.py` & `panoptic-0.0.9.dev3/panoptic/core/__init__.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/core/db.py` & `panoptic-0.0.9.dev3/panoptic/core/db.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/core/db_utils.py` & `panoptic-0.0.9.dev3/panoptic/core/db_utils.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/core/image_importer.py` & `panoptic-0.0.9.dev3/panoptic/core/image_importer.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/html/assets/bootstrap-icons-966620f9.woff2` & `panoptic-0.0.9.dev3/panoptic/html/assets/bootstrap-icons-966620f9.woff2`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/html/assets/bootstrap-icons-c6569d46.woff` & `panoptic-0.0.9.dev3/panoptic/html/assets/bootstrap-icons-c6569d46.woff`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/html/assets/index-0a222725.css` & `panoptic-0.0.9.dev3/panoptic/html/assets/index-0a222725.css`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/html/assets/index-7467d80f.js` & `panoptic-0.0.9.dev3/panoptic/html/assets/index-7467d80f.js`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/html/favicon.ico` & `panoptic-0.0.9.dev3/panoptic/html/favicon.ico`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/main.py` & `panoptic-0.0.9.dev3/panoptic/main.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/models/models.py` & `panoptic-0.0.9.dev3/panoptic/models/models.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/models/payloads.py` & `panoptic-0.0.9.dev3/panoptic/models/payloads.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/scripts/create_db.sql` & `panoptic-0.0.9.dev3/panoptic/scripts/create_db.sql`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/scripts/populate_db.sql` & `panoptic-0.0.9.dev3/panoptic/scripts/populate_db.sql`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic/scripts/to_pca.py` & `panoptic-0.0.9.dev3/panoptic/scripts/to_pca.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/panoptic.egg-info/PKG-INFO` & `panoptic-0.0.9.dev3/panoptic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptic
-Version: 0.0.9.dev2
+Version: 0.0.9.dev3
 License: Mozilla
 Description-Content-Type: text/markdown
 
 # Panoptic
```

### Comparing `panoptic-0.0.9.dev2/panoptic.egg-info/SOURCES.txt` & `panoptic-0.0.9.dev3/panoptic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev2/setup.py` & `panoptic-0.0.9.dev3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def parse_requirements(req_file):
     with open(req_file) as fp:
         _requires = fp.read()
     return _requires
 
 
 NAME = "panoptic"
-VERSION = "0.0.9.dev2"
+VERSION = "0.0.9.dev3"
 # Get dependencies from requirement files
 SETUP_REQUIRES = ['setuptools', 'setuptools-git', 'wheel']
 INSTALL_REQUIRES = parse_requirements('requirements.txt')
 LONG_DESCRIPTION = ""
 
 with open(os.path.join(os.path.dirname(__file__), 'description.md'), 'r') as f:
     LONG_DESCRIPTION = f.read()
```

### Comparing `panoptic-0.0.9.dev2/thunder-collection_Panoptic.json` & `panoptic-0.0.9.dev3/thunder-collection_Panoptic.json`

 * *Files identical despite different names*

