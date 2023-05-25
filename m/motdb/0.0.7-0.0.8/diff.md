# Comparing `tmp/motdb-0.0.7.tar.gz` & `tmp/motdb-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motdb-0.0.7.tar", last modified: Thu May 25 20:41:50 2023, max compression
+gzip compressed data, was "motdb-0.0.8.tar", last modified: Thu May 25 20:47:32 2023, max compression
```

## Comparing `motdb-0.0.7.tar` & `motdb-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:41:50.947338 motdb-0.0.7/
--rw-r--r--   0 mfsteele   (502) staff       (20)     1063 2023-05-18 14:54:10.000000 motdb-0.0.7/LICENSE
--rw-r--r--   0 mfsteele   (502) staff       (20)       81 2023-05-23 19:19:31.000000 motdb-0.0.7/MANIFEST.in
--rw-r--r--   0 mfsteele   (502) staff       (20)     1775 2023-05-25 20:41:50.947187 motdb-0.0.7/PKG-INFO
--rw-r--r--   0 mfsteele   (502) staff       (20)       53 2023-05-23 15:39:33.000000 motdb-0.0.7/README.md
--rw-r--r--   0 mfsteele   (502) staff       (20)     1139 2023-05-25 20:41:45.000000 motdb-0.0.7/pyproject.toml
--rw-r--r--   0 mfsteele   (502) staff       (20)       38 2023-05-25 20:41:50.947385 motdb-0.0.7/setup.cfg
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:41:50.936202 motdb-0.0.7/src/
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:41:50.937655 motdb-0.0.7/src/motdb/
--rw-r--r--   0 mfsteele   (502) staff       (20)       25 2023-05-25 20:41:45.000000 motdb-0.0.7/src/motdb/__init__.py
--rw-r--r--   0 mfsteele   (502) staff       (20)       89 2023-05-23 18:08:52.000000 motdb-0.0.7/src/motdb/__main__.py
--rw-r--r--   0 mfsteele   (502) staff       (20)      840 2023-05-25 20:41:07.000000 motdb-0.0.7/src/motdb/dbx.py
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:41:50.936396 motdb-0.0.7/src/motdb/inc/
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:41:50.938618 motdb-0.0.7/src/motdb/inc/json/
--rw-r--r--   0 mfsteele   (502) staff       (20)  1606047 2023-05-23 19:17:04.000000 motdb-0.0.7/src/motdb/inc/json/dict_tracy.json
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:41:50.941771 motdb-0.0.7/src/motdb/inc/whls/
--rw-r--r--   0 mfsteele   (502) staff       (20)   700282 2023-05-23 16:39:38.000000 motdb-0.0.7/src/motdb/inc/whls/pysqlite3-0.5.0-cp310-cp310-macosx_13_0_arm64.whl
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:41:50.946162 motdb-0.0.7/src/motdb/samples/
--rw-r--r--   0 mfsteele   (502) staff       (20)       32 2023-05-25 20:34:27.000000 motdb-0.0.7/src/motdb/samples/__init__.py
--rw-r--r--   0 mfsteele   (502) staff       (20)       52 2023-05-25 20:35:57.000000 motdb-0.0.7/src/motdb/samples/sample.py
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:41:50.946883 motdb-0.0.7/src/motdb/tools/
--rw-r--r--   0 mfsteele   (502) staff       (20)        0 2023-05-25 19:30:54.000000 motdb-0.0.7/src/motdb/tools/__init__.py
--rw-r--r--   0 mfsteele   (502) staff       (20)     6678 2023-05-25 18:44:54.000000 motdb-0.0.7/src/motdb/tools/cli_tools.py
--rw-r--r--   0 mfsteele   (502) staff       (20)     4542 2023-05-25 20:28:34.000000 motdb-0.0.7/src/motdb/tools/path_tools.py
--rw-r--r--   0 mfsteele   (502) staff       (20)     5782 2023-05-25 18:44:54.000000 motdb-0.0.7/src/motdb/tools/print_tools.py
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:41:50.938491 motdb-0.0.7/src/motdb.egg-info/
--rw-r--r--   0 mfsteele   (502) staff       (20)     1775 2023-05-25 20:41:50.000000 motdb-0.0.7/src/motdb.egg-info/PKG-INFO
--rw-r--r--   0 mfsteele   (502) staff       (20)      585 2023-05-25 20:41:50.000000 motdb-0.0.7/src/motdb.egg-info/SOURCES.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)        1 2023-05-25 20:41:50.000000 motdb-0.0.7/src/motdb.egg-info/dependency_links.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)       46 2023-05-25 20:41:50.000000 motdb-0.0.7/src/motdb.egg-info/entry_points.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)       64 2023-05-25 20:41:50.000000 motdb-0.0.7/src/motdb.egg-info/requires.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)        6 2023-05-25 20:41:50.000000 motdb-0.0.7/src/motdb.egg-info/top_level.txt
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:47:32.377163 motdb-0.0.8/
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1063 2023-05-18 14:54:10.000000 motdb-0.0.8/LICENSE
+-rw-r--r--   0 mfsteele   (502) staff       (20)       81 2023-05-23 19:19:31.000000 motdb-0.0.8/MANIFEST.in
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1775 2023-05-25 20:47:32.377008 motdb-0.0.8/PKG-INFO
+-rw-r--r--   0 mfsteele   (502) staff       (20)       53 2023-05-23 15:39:33.000000 motdb-0.0.8/README.md
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1139 2023-05-25 20:47:27.000000 motdb-0.0.8/pyproject.toml
+-rw-r--r--   0 mfsteele   (502) staff       (20)       38 2023-05-25 20:47:32.377202 motdb-0.0.8/setup.cfg
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:47:32.364102 motdb-0.0.8/src/
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:47:32.365481 motdb-0.0.8/src/motdb/
+-rw-r--r--   0 mfsteele   (502) staff       (20)       25 2023-05-25 20:47:27.000000 motdb-0.0.8/src/motdb/__init__.py
+-rw-r--r--   0 mfsteele   (502) staff       (20)       89 2023-05-23 18:08:52.000000 motdb-0.0.8/src/motdb/__main__.py
+-rw-r--r--   0 mfsteele   (502) staff       (20)      841 2023-05-25 20:46:40.000000 motdb-0.0.8/src/motdb/dbx.py
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:47:32.364296 motdb-0.0.8/src/motdb/inc/
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:47:32.366437 motdb-0.0.8/src/motdb/inc/json/
+-rw-r--r--   0 mfsteele   (502) staff       (20)  1606047 2023-05-23 19:17:04.000000 motdb-0.0.8/src/motdb/inc/json/dict_tracy.json
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:47:32.368647 motdb-0.0.8/src/motdb/inc/whls/
+-rw-r--r--   0 mfsteele   (502) staff       (20)   700282 2023-05-23 16:39:38.000000 motdb-0.0.8/src/motdb/inc/whls/pysqlite3-0.5.0-cp310-cp310-macosx_13_0_arm64.whl
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:47:32.375856 motdb-0.0.8/src/motdb/samples/
+-rw-r--r--   0 mfsteele   (502) staff       (20)       32 2023-05-25 20:34:27.000000 motdb-0.0.8/src/motdb/samples/__init__.py
+-rw-r--r--   0 mfsteele   (502) staff       (20)       52 2023-05-25 20:35:57.000000 motdb-0.0.8/src/motdb/samples/sample.py
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:47:32.376699 motdb-0.0.8/src/motdb/tools/
+-rw-r--r--   0 mfsteele   (502) staff       (20)        0 2023-05-25 19:30:54.000000 motdb-0.0.8/src/motdb/tools/__init__.py
+-rw-r--r--   0 mfsteele   (502) staff       (20)     6678 2023-05-25 18:44:54.000000 motdb-0.0.8/src/motdb/tools/cli_tools.py
+-rw-r--r--   0 mfsteele   (502) staff       (20)     4542 2023-05-25 20:28:34.000000 motdb-0.0.8/src/motdb/tools/path_tools.py
+-rw-r--r--   0 mfsteele   (502) staff       (20)     5782 2023-05-25 18:44:54.000000 motdb-0.0.8/src/motdb/tools/print_tools.py
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-25 20:47:32.366318 motdb-0.0.8/src/motdb.egg-info/
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1775 2023-05-25 20:47:32.000000 motdb-0.0.8/src/motdb.egg-info/PKG-INFO
+-rw-r--r--   0 mfsteele   (502) staff       (20)      585 2023-05-25 20:47:32.000000 motdb-0.0.8/src/motdb.egg-info/SOURCES.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)        1 2023-05-25 20:47:32.000000 motdb-0.0.8/src/motdb.egg-info/dependency_links.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)       46 2023-05-25 20:47:32.000000 motdb-0.0.8/src/motdb.egg-info/entry_points.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)       64 2023-05-25 20:47:32.000000 motdb-0.0.8/src/motdb.egg-info/requires.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)        6 2023-05-25 20:47:32.000000 motdb-0.0.8/src/motdb.egg-info/top_level.txt
```

### Comparing `motdb-0.0.7/LICENSE` & `motdb-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `motdb-0.0.7/PKG-INFO` & `motdb-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motdb
-Version: 0.0.7
+Version: 0.0.8
 Summary: Một Database Layer to ... Bind Them (All)
 Author-email: Mike Steele <mike@mikesteele.us>
 License: MIT License
         
         Copyright (c) 2023 soulrx
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `motdb-0.0.7/pyproject.toml` & `motdb-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "motdb"
-version = "0.0.7"
+version = "0.0.8"
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
-current_version = "0.0.7"
+current_version = "0.0.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `motdb-0.0.7/src/motdb/dbx.py` & `motdb-0.0.8/src/motdb/dbx.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
       cli = Cli()
       print(THISD)
       with open('dbx.toml','wb') as f:
          f.write(sample.toml_file+'\n')
 
     with open("dbx.toml", "rb") as f:
         cfg = tomli.load(f)
-        locals()['cfg'] = cfg
+        globals()['cfg'] = cfg
 
   except Exception as e:
      print(str(e))
 
 class DB:
     """ Base Database Class """
     def __init__(self, *kw):
```

### Comparing `motdb-0.0.7/src/motdb/inc/json/dict_tracy.json` & `motdb-0.0.8/src/motdb/inc/json/dict_tracy.json`

 * *Files identical despite different names*

### Comparing `motdb-0.0.7/src/motdb/inc/whls/pysqlite3-0.5.0-cp310-cp310-macosx_13_0_arm64.whl` & `motdb-0.0.8/src/motdb/inc/whls/pysqlite3-0.5.0-cp310-cp310-macosx_13_0_arm64.whl`

 * *Files identical despite different names*

### Comparing `motdb-0.0.7/src/motdb/tools/cli_tools.py` & `motdb-0.0.8/src/motdb/tools/cli_tools.py`

 * *Files identical despite different names*

### Comparing `motdb-0.0.7/src/motdb/tools/path_tools.py` & `motdb-0.0.8/src/motdb/tools/path_tools.py`

 * *Files identical despite different names*

### Comparing `motdb-0.0.7/src/motdb/tools/print_tools.py` & `motdb-0.0.8/src/motdb/tools/print_tools.py`

 * *Files identical despite different names*

### Comparing `motdb-0.0.7/src/motdb.egg-info/PKG-INFO` & `motdb-0.0.8/src/motdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motdb
-Version: 0.0.7
+Version: 0.0.8
 Summary: Một Database Layer to ... Bind Them (All)
 Author-email: Mike Steele <mike@mikesteele.us>
 License: MIT License
         
         Copyright (c) 2023 soulrx
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `motdb-0.0.7/src/motdb.egg-info/SOURCES.txt` & `motdb-0.0.8/src/motdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

