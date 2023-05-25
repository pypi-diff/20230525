# Comparing `tmp/dict_hash-1.1.8.tar.gz` & `tmp/dict_hash-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dict_hash-1.1.8.tar", last modified: Sun Jul 19 08:16:04 2020, max compression
+gzip compressed data, was "dist/dict_hash-1.1.9.tar", last modified: Sun Jul 19 08:24:40 2020, max compression
```

## Comparing `dict_hash-1.1.8.tar` & `dict_hash-1.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2020-07-19 08:16:04.000000 dict_hash-1.1.8/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)        0 2020-07-19 08:00:24.000000 dict_hash-1.1.8/MANIFEST.in
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     5690 2020-07-19 08:16:04.000000 dict_hash-1.1.8/PKG-INFO
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     4289 2020-07-19 08:00:24.000000 dict_hash-1.1.8/README.rst
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2020-07-19 08:16:04.000000 dict_hash-1.1.8/dict_hash/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      210 2020-07-19 08:00:24.000000 dict_hash-1.1.8/dict_hash/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       65 2020-07-19 08:15:57.000000 dict_hash-1.1.8/dict_hash/__version__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     3287 2020-07-19 08:08:48.000000 dict_hash-1.1.8/dict_hash/dict_hash.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1322 2020-07-19 08:00:24.000000 dict_hash-1.1.8/dict_hash/hashable.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      531 2020-07-19 08:00:24.000000 dict_hash-1.1.8/dict_hash/validate_consistent_hash.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2020-07-19 08:16:04.000000 dict_hash-1.1.8/dict_hash.egg-info/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     5690 2020-07-19 08:16:04.000000 dict_hash-1.1.8/dict_hash.egg-info/PKG-INFO
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      325 2020-07-19 08:16:04.000000 dict_hash-1.1.8/dict_hash.egg-info/SOURCES.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2020-07-19 08:16:04.000000 dict_hash-1.1.8/dict_hash.egg-info/dependency_links.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      130 2020-07-19 08:16:04.000000 dict_hash-1.1.8/dict_hash.egg-info/requires.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       10 2020-07-19 08:16:04.000000 dict_hash-1.1.8/dict_hash.egg-info/top_level.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       38 2020-07-19 08:16:04.000000 dict_hash-1.1.8/setup.cfg
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1799 2020-07-19 08:15:40.000000 dict_hash-1.1.8/setup.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2020-07-19 08:24:40.000000 dict_hash-1.1.9/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)        0 2020-07-19 08:00:24.000000 dict_hash-1.1.9/MANIFEST.in
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     5690 2020-07-19 08:24:40.000000 dict_hash-1.1.9/PKG-INFO
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     4289 2020-07-19 08:00:24.000000 dict_hash-1.1.9/README.rst
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2020-07-19 08:24:40.000000 dict_hash-1.1.9/dict_hash/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      210 2020-07-19 08:00:24.000000 dict_hash-1.1.9/dict_hash/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       65 2020-07-19 08:24:35.000000 dict_hash-1.1.9/dict_hash/__version__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     3287 2020-07-19 08:08:48.000000 dict_hash-1.1.9/dict_hash/dict_hash.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1322 2020-07-19 08:00:24.000000 dict_hash-1.1.9/dict_hash/hashable.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      531 2020-07-19 08:00:24.000000 dict_hash-1.1.9/dict_hash/validate_consistent_hash.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2020-07-19 08:24:40.000000 dict_hash-1.1.9/dict_hash.egg-info/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     5690 2020-07-19 08:24:40.000000 dict_hash-1.1.9/dict_hash.egg-info/PKG-INFO
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      325 2020-07-19 08:24:40.000000 dict_hash-1.1.9/dict_hash.egg-info/SOURCES.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2020-07-19 08:24:40.000000 dict_hash-1.1.9/dict_hash.egg-info/dependency_links.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      130 2020-07-19 08:24:40.000000 dict_hash-1.1.9/dict_hash.egg-info/requires.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       10 2020-07-19 08:24:40.000000 dict_hash-1.1.9/dict_hash.egg-info/top_level.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       38 2020-07-19 08:24:40.000000 dict_hash-1.1.9/setup.cfg
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1799 2020-07-19 08:20:35.000000 dict_hash-1.1.9/setup.py
```

### Comparing `dict_hash-1.1.8/PKG-INFO` & `dict_hash-1.1.9/dict_hash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dict_hash
-Version: 1.1.8
+Name: dict-hash
+Version: 1.1.9
 Summary: Simple python tool to hash dictionaries using both default hash and sha256.
 Home-page: https://github.com/LucaCappelletti94/dict_hash
 Author: Luca Cappelletti
 Author-email: cappelletti.luca94@gmail.com
 License: MIT
 Description: dict_hash
         =========================================================================================
```

### Comparing `dict_hash-1.1.8/README.rst` & `dict_hash-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `dict_hash-1.1.8/dict_hash/dict_hash.py` & `dict_hash-1.1.9/dict_hash/dict_hash.py`

 * *Files identical despite different names*

### Comparing `dict_hash-1.1.8/dict_hash/hashable.py` & `dict_hash-1.1.9/dict_hash/hashable.py`

 * *Files identical despite different names*

### Comparing `dict_hash-1.1.8/dict_hash/validate_consistent_hash.py` & `dict_hash-1.1.9/dict_hash/validate_consistent_hash.py`

 * *Files identical despite different names*

### Comparing `dict_hash-1.1.8/dict_hash.egg-info/PKG-INFO` & `dict_hash-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dict-hash
-Version: 1.1.8
+Name: dict_hash
+Version: 1.1.9
 Summary: Simple python tool to hash dictionaries using both default hash and sha256.
 Home-page: https://github.com/LucaCappelletti94/dict_hash
 Author: Luca Cappelletti
 Author-email: cappelletti.luca94@gmail.com
 License: MIT
 Description: dict_hash
         =========================================================================================
```

### Comparing `dict_hash-1.1.8/setup.py` & `dict_hash-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,12 +61,12 @@
         'Programming Language :: Python :: 3'
     ],
     packages=find_packages(exclude=['contrib', 'docs', 'tests*']),
     tests_require=test_deps,
     install_requires=[
         "pandas",
         "numpy",
-        "deflate_dict>=1.0.7",
+        "deflate_dict>=1.0.8",
         "numba"
     ],
     extras_require=extras,
 )
```

