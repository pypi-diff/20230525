# Comparing `tmp/kn_flatten_json-0.0.6.tar.gz` & `tmp/kn_flatten_json-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kn_flatten_json-0.0.6.tar", last modified: Thu May 25 06:45:25 2023, max compression
+gzip compressed data, was "dist\kn_flatten_json-0.0.7.tar", last modified: Mon May 22 08:33:09 2023, max compression
```

## Comparing `kn_flatten_json-0.0.6.tar` & `kn_flatten_json-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 06:45:25.000000 kn_flatten_json-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-05-25 06:45:25.000000 kn_flatten_json-0.0.6/kn_flatten_json/
--rw-rw-rw-   0        0        0     8985 2023-05-25 06:44:53.000000 kn_flatten_json-0.0.6/kn_flatten_json/kn_flatten_json.py
--rw-rw-rw-   0        0        0       58 2023-05-22 08:36:10.000000 kn_flatten_json-0.0.6/kn_flatten_json/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:45:25.000000 kn_flatten_json-0.0.6/kn_flatten_json.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-25 06:45:24.000000 kn_flatten_json-0.0.6/kn_flatten_json.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2267 2023-05-25 06:45:24.000000 kn_flatten_json-0.0.6/kn_flatten_json.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-05-25 06:45:24.000000 kn_flatten_json-0.0.6/kn_flatten_json.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       16 2023-05-25 06:45:24.000000 kn_flatten_json-0.0.6/kn_flatten_json.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2267 2023-05-25 06:45:25.000000 kn_flatten_json-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1266 2023-02-03 07:02:29.000000 kn_flatten_json-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-25 06:45:25.000000 kn_flatten_json-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1006 2023-05-25 06:44:49.000000 kn_flatten_json-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:33:09.000000 kn_flatten_json-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-05-22 08:33:09.000000 kn_flatten_json-0.0.7/kn_flatten_json/
+-rw-rw-rw-   0        0        0     5051 2023-05-22 08:17:44.000000 kn_flatten_json-0.0.7/kn_flatten_json/kn_flatten_json.py
+-rw-rw-rw-   0        0        0       40 2023-05-22 08:30:04.000000 kn_flatten_json-0.0.7/kn_flatten_json/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:33:09.000000 kn_flatten_json-0.0.7/kn_flatten_json.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-22 08:33:09.000000 kn_flatten_json-0.0.7/kn_flatten_json.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2267 2023-05-22 08:33:09.000000 kn_flatten_json-0.0.7/kn_flatten_json.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-22 08:33:09.000000 kn_flatten_json-0.0.7/kn_flatten_json.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       16 2023-05-22 08:33:09.000000 kn_flatten_json-0.0.7/kn_flatten_json.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2267 2023-05-22 08:33:09.000000 kn_flatten_json-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1266 2023-02-03 07:02:29.000000 kn_flatten_json-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 08:33:09.000000 kn_flatten_json-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1006 2023-05-22 08:32:00.000000 kn_flatten_json-0.0.7/setup.py
```

### Comparing `kn_flatten_json-0.0.6/kn_flatten_json.egg-info/PKG-INFO` & `kn_flatten_json-0.0.7/kn_flatten_json.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kn-flatten-json
-Version: 0.0.6
+Version: 0.0.7
 Summary: kn_flatten_json
 Home-page: UNKNOWN
 Author: Sukriti
 Author-email: sukriti.saluja@kockpit.in
 License: UNKNOWN
 Description: 
         # Project description
```

### Comparing `kn_flatten_json-0.0.6/PKG-INFO` & `kn_flatten_json-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kn_flatten_json
-Version: 0.0.6
+Version: 0.0.7
 Summary: kn_flatten_json
 Home-page: UNKNOWN
 Author: Sukriti
 Author-email: sukriti.saluja@kockpit.in
 License: UNKNOWN
 Description: 
         # Project description
```

### Comparing `kn_flatten_json-0.0.6/README.md` & `kn_flatten_json-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `kn_flatten_json-0.0.6/setup.py` & `kn_flatten_json-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 from pathlib import Path
 this_directory = Path(__file__).parent
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'kn_flatten_json'
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
 
 # Setting up
 setup(
     name="kn_flatten_json",
```

