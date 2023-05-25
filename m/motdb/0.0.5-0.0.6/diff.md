# Comparing `tmp/motdb-0.0.5.tar.gz` & `tmp/motdb-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motdb-0.0.5.tar", last modified: Thu May 25 19:56:33 2023, max compression
+gzip compressed data, was "motdb-0.0.6.tar", last modified: Thu May 25 20:14:46 2023, max compression
```

## Comparing `motdb-0.0.5.tar` & `motdb-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 19:56:33.096906 motdb-0.0.5/
--rw-r--r--   0 mfsteele   (502) staff       (20)     1063 2023-05-18 14:54:10.000000 motdb-0.0.5/LICENSE
--rw-r--r--   0 mfsteele   (502) staff       (20)       81 2023-05-23 19:19:31.000000 motdb-0.0.5/MANIFEST.in
--rw-r--r--   0 mfsteele   (502) staff       (20)     1775 2023-05-25 19:56:33.096706 motdb-0.0.5/PKG-INFO
--rw-r--r--   0 mfsteele   (502) staff       (20)       53 2023-05-23 15:39:33.000000 motdb-0.0.5/README.md
--rw-r--r--   0 mfsteele   (502) staff       (20)     1139 2023-05-25 19:56:27.000000 motdb-0.0.5/pyproject.toml
--rw-r--r--   0 mfsteele   (502) staff       (20)       38 2023-05-25 19:56:33.096952 motdb-0.0.5/setup.cfg
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 19:56:33.083539 motdb-0.0.5/src/
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 19:56:33.084788 motdb-0.0.5/src/motdb/
--rw-r--r--   0 mfsteele   (502) staff       (20)       25 2023-05-25 19:56:27.000000 motdb-0.0.5/src/motdb/__init__.py
--rw-r--r--   0 mfsteele   (502) staff       (20)       89 2023-05-23 18:08:52.000000 motdb-0.0.5/src/motdb/__main__.py
--rw-r--r--   0 mfsteele   (502) staff       (20)      305 2023-05-25 19:35:55.000000 motdb-0.0.5/src/motdb/dbx.py
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 19:56:33.083732 motdb-0.0.5/src/motdb/inc/
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 19:56:33.086031 motdb-0.0.5/src/motdb/inc/json/
--rw-r--r--   0 mfsteele   (502) staff       (20)  1606047 2023-05-23 19:17:04.000000 motdb-0.0.5/src/motdb/inc/json/dict_tracy.json
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 19:56:33.088207 motdb-0.0.5/src/motdb/inc/whls/
--rw-r--r--   0 mfsteele   (502) staff       (20)   700282 2023-05-23 16:39:38.000000 motdb-0.0.5/src/motdb/inc/whls/pysqlite3-0.5.0-cp310-cp310-macosx_13_0_arm64.whl
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 19:56:33.096463 motdb-0.0.5/src/motdb/tools/
--rw-r--r--   0 mfsteele   (502) staff       (20)        0 2023-05-25 19:30:54.000000 motdb-0.0.5/src/motdb/tools/__init__.py
--rw-r--r--   0 mfsteele   (502) staff       (20)     6678 2023-05-25 18:44:54.000000 motdb-0.0.5/src/motdb/tools/cli_tools.py
--rw-r--r--   0 mfsteele   (502) staff       (20)     4847 2023-05-25 18:44:54.000000 motdb-0.0.5/src/motdb/tools/path_tools.py
--rw-r--r--   0 mfsteele   (502) staff       (20)     5782 2023-05-25 18:44:54.000000 motdb-0.0.5/src/motdb/tools/print_tools.py
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 19:56:33.085892 motdb-0.0.5/src/motdb.egg-info/
--rw-r--r--   0 mfsteele   (502) staff       (20)     1775 2023-05-25 19:56:33.000000 motdb-0.0.5/src/motdb.egg-info/PKG-INFO
--rw-r--r--   0 mfsteele   (502) staff       (20)      527 2023-05-25 19:56:33.000000 motdb-0.0.5/src/motdb.egg-info/SOURCES.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)        1 2023-05-25 19:56:33.000000 motdb-0.0.5/src/motdb.egg-info/dependency_links.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)       46 2023-05-25 19:56:33.000000 motdb-0.0.5/src/motdb.egg-info/entry_points.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)       64 2023-05-25 19:56:33.000000 motdb-0.0.5/src/motdb.egg-info/requires.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)        6 2023-05-25 19:56:33.000000 motdb-0.0.5/src/motdb.egg-info/top_level.txt
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:14:46.596654 motdb-0.0.6/
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1063 2023-05-18 14:54:10.000000 motdb-0.0.6/LICENSE
+-rw-r--r--   0 mfsteele   (502) staff       (20)       81 2023-05-23 19:19:31.000000 motdb-0.0.6/MANIFEST.in
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1775 2023-05-25 20:14:46.596468 motdb-0.0.6/PKG-INFO
+-rw-r--r--   0 mfsteele   (502) staff       (20)       53 2023-05-23 15:39:33.000000 motdb-0.0.6/README.md
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1139 2023-05-25 20:14:40.000000 motdb-0.0.6/pyproject.toml
+-rw-r--r--   0 mfsteele   (502) staff       (20)       38 2023-05-25 20:14:46.596711 motdb-0.0.6/setup.cfg
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:14:46.579995 motdb-0.0.6/src/
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:14:46.583318 motdb-0.0.6/src/motdb/
+-rw-r--r--   0 mfsteele   (502) staff       (20)       25 2023-05-25 20:14:40.000000 motdb-0.0.6/src/motdb/__init__.py
+-rw-r--r--   0 mfsteele   (502) staff       (20)       89 2023-05-23 18:08:52.000000 motdb-0.0.6/src/motdb/__main__.py
+-rw-r--r--   0 mfsteele   (502) staff       (20)      311 2023-05-25 20:14:14.000000 motdb-0.0.6/src/motdb/dbx.py
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:14:46.580516 motdb-0.0.6/src/motdb/inc/
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:14:46.585846 motdb-0.0.6/src/motdb/inc/json/
+-rw-r--r--   0 mfsteele   (502) staff       (20)  1606047 2023-05-23 19:17:04.000000 motdb-0.0.6/src/motdb/inc/json/dict_tracy.json
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:14:46.590795 motdb-0.0.6/src/motdb/inc/whls/
+-rw-r--r--   0 mfsteele   (502) staff       (20)   700282 2023-05-23 16:39:38.000000 motdb-0.0.6/src/motdb/inc/whls/pysqlite3-0.5.0-cp310-cp310-macosx_13_0_arm64.whl
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:14:46.596203 motdb-0.0.6/src/motdb/tools/
+-rw-r--r--   0 mfsteele   (502) staff       (20)        0 2023-05-25 19:30:54.000000 motdb-0.0.6/src/motdb/tools/__init__.py
+-rw-r--r--   0 mfsteele   (502) staff       (20)     6678 2023-05-25 18:44:54.000000 motdb-0.0.6/src/motdb/tools/cli_tools.py
+-rw-r--r--   0 mfsteele   (502) staff       (20)     4847 2023-05-25 18:44:54.000000 motdb-0.0.6/src/motdb/tools/path_tools.py
+-rw-r--r--   0 mfsteele   (502) staff       (20)     5782 2023-05-25 18:44:54.000000 motdb-0.0.6/src/motdb/tools/print_tools.py
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:14:46.585643 motdb-0.0.6/src/motdb.egg-info/
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1775 2023-05-25 20:14:46.000000 motdb-0.0.6/src/motdb.egg-info/PKG-INFO
+-rw-r--r--   0 mfsteele   (502) staff       (20)      527 2023-05-25 20:14:46.000000 motdb-0.0.6/src/motdb.egg-info/SOURCES.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)        1 2023-05-25 20:14:46.000000 motdb-0.0.6/src/motdb.egg-info/dependency_links.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)       46 2023-05-25 20:14:46.000000 motdb-0.0.6/src/motdb.egg-info/entry_points.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)       64 2023-05-25 20:14:46.000000 motdb-0.0.6/src/motdb.egg-info/requires.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)        6 2023-05-25 20:14:46.000000 motdb-0.0.6/src/motdb.egg-info/top_level.txt
```

### Comparing `motdb-0.0.5/LICENSE` & `motdb-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `motdb-0.0.5/PKG-INFO` & `motdb-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motdb
-Version: 0.0.5
+Version: 0.0.6
 Summary: Một Database Layer to ... Bind Them (All)
 Author-email: Mike Steele <mike@mikesteele.us>
 License: MIT License
         
         Copyright (c) 2023 soulrx
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `motdb-0.0.5/pyproject.toml` & `motdb-0.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "motdb"
-version = "0.0.5"
+version = "0.0.6"
 description = "Một Database Layer to ... Bind Them (All)"
 readme = "README.md"
 authors = [{ name = "Mike Steele", email = "mike@mikesteele.us" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -29,15 +29,15 @@
 [project.urls]
 Homepage = "https://github.com/soulrx/motdb"
 
 [project.scripts]
 motdb = "motdb.__main__:main"
 
 [tool.bumpver]
-current_version = "0.0.5"
+current_version = "0.0.6"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `motdb-0.0.5/src/motdb/inc/json/dict_tracy.json` & `motdb-0.0.6/src/motdb/inc/json/dict_tracy.json`

 * *Files identical despite different names*

### Comparing `motdb-0.0.5/src/motdb/inc/whls/pysqlite3-0.5.0-cp310-cp310-macosx_13_0_arm64.whl` & `motdb-0.0.6/src/motdb/inc/whls/pysqlite3-0.5.0-cp310-cp310-macosx_13_0_arm64.whl`

 * *Files identical despite different names*

### Comparing `motdb-0.0.5/src/motdb/tools/cli_tools.py` & `motdb-0.0.6/src/motdb/tools/cli_tools.py`

 * *Files identical despite different names*

### Comparing `motdb-0.0.5/src/motdb/tools/path_tools.py` & `motdb-0.0.6/src/motdb/tools/path_tools.py`

 * *Files identical despite different names*

### Comparing `motdb-0.0.5/src/motdb/tools/print_tools.py` & `motdb-0.0.6/src/motdb/tools/print_tools.py`

 * *Files identical despite different names*

### Comparing `motdb-0.0.5/src/motdb.egg-info/PKG-INFO` & `motdb-0.0.6/src/motdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motdb
-Version: 0.0.5
+Version: 0.0.6
 Summary: Một Database Layer to ... Bind Them (All)
 Author-email: Mike Steele <mike@mikesteele.us>
 License: MIT License
         
         Copyright (c) 2023 soulrx
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `motdb-0.0.5/src/motdb.egg-info/SOURCES.txt` & `motdb-0.0.6/src/motdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

