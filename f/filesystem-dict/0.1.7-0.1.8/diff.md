# Comparing `tmp/filesystem-dict-0.1.7.tar.gz` & `tmp/filesystem-dict-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filesystem-dict-0.1.7.tar", last modified: Wed May 17 17:19:35 2023, max compression
+gzip compressed data, was "filesystem-dict-0.1.8.tar", last modified: Thu May 25 17:04:16 2023, max compression
```

## Comparing `filesystem-dict-0.1.7.tar` & `filesystem-dict-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 17:19:35.558137 filesystem-dict-0.1.7/
--rw-r--r--   0 user      (1000) user      (1000)      666 2023-05-15 20:22:54.000000 filesystem-dict-0.1.7/LICENSE.txt
--rw-r--r--   0 user      (1000) user      (1000)     1149 2023-05-17 17:19:35.558137 filesystem-dict-0.1.7/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      834 2023-05-17 08:45:31.000000 filesystem-dict-0.1.7/README.md
--rw-r--r--   0 user      (1000) user      (1000)      476 2023-05-17 17:19:35.558137 filesystem-dict-0.1.7/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)       69 2023-05-15 20:55:49.000000 filesystem-dict-0.1.7/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 17:19:35.558137 filesystem-dict-0.1.7/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 17:19:35.558137 filesystem-dict-0.1.7/src/filesystem_dict.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1149 2023-05-17 17:19:35.000000 filesystem-dict-0.1.7/src/filesystem_dict.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      276 2023-05-17 17:19:35.000000 filesystem-dict-0.1.7/src/filesystem_dict.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-17 17:19:35.000000 filesystem-dict-0.1.7/src/filesystem_dict.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        7 2023-05-17 17:19:35.000000 filesystem-dict-0.1.7/src/filesystem_dict.egg-info/top_level.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 17:19:35.558137 filesystem-dict-0.1.7/src/fsdict/
--rw-r--r--   0 user      (1000) user      (1000)       27 2023-05-16 07:52:47.000000 filesystem-dict-0.1.7/src/fsdict/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     5850 2023-05-17 17:17:59.000000 filesystem-dict-0.1.7/src/fsdict/fsdict.py
--rw-r--r--   0 user      (1000) user      (1000)     1116 2023-05-16 08:07:12.000000 filesystem-dict-0.1.7/src/fsdict/utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-25 17:04:16.935187 filesystem-dict-0.1.8/
+-rw-r--r--   0 user      (1000) user      (1000)      666 2023-05-23 14:03:54.000000 filesystem-dict-0.1.8/LICENSE.txt
+-rw-r--r--   0 user      (1000) user      (1000)     1149 2023-05-25 17:04:16.935187 filesystem-dict-0.1.8/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      834 2023-05-23 14:03:54.000000 filesystem-dict-0.1.8/README.md
+-rw-r--r--   0 user      (1000) user      (1000)      476 2023-05-25 17:04:16.935187 filesystem-dict-0.1.8/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)       69 2023-05-23 14:03:54.000000 filesystem-dict-0.1.8/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-25 17:04:16.935187 filesystem-dict-0.1.8/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-25 17:04:16.935187 filesystem-dict-0.1.8/src/filesystem_dict.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1149 2023-05-25 17:04:16.000000 filesystem-dict-0.1.8/src/filesystem_dict.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      276 2023-05-25 17:04:16.000000 filesystem-dict-0.1.8/src/filesystem_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-25 17:04:16.000000 filesystem-dict-0.1.8/src/filesystem_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        7 2023-05-25 17:04:16.000000 filesystem-dict-0.1.8/src/filesystem_dict.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-25 17:04:16.935187 filesystem-dict-0.1.8/src/fsdict/
+-rw-r--r--   0 user      (1000) user      (1000)       27 2023-05-23 14:03:54.000000 filesystem-dict-0.1.8/src/fsdict/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     5850 2023-05-23 14:03:54.000000 filesystem-dict-0.1.8/src/fsdict/fsdict.py
+-rw-r--r--   0 user      (1000) user      (1000)     1116 2023-05-25 17:01:14.000000 filesystem-dict-0.1.8/src/fsdict/utils.py
```

### Comparing `filesystem-dict-0.1.7/LICENSE.txt` & `filesystem-dict-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `filesystem-dict-0.1.7/PKG-INFO` & `filesystem-dict-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filesystem-dict
-Version: 0.1.7
+Version: 0.1.8
 Summary: Dictionary like access to the filesystem.
 Home-page: https://github.com/MNayer/fsdict
 Author: MNayer
 Author-email: marie.nayer@web.de
 License: 0BSD
 Keywords: dictionary,filesystem
 Description-Content-Type: text/markdown
```

### Comparing `filesystem-dict-0.1.7/README.md` & `filesystem-dict-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `filesystem-dict-0.1.7/src/filesystem_dict.egg-info/PKG-INFO` & `filesystem-dict-0.1.8/src/filesystem_dict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filesystem-dict
-Version: 0.1.7
+Version: 0.1.8
 Summary: Dictionary like access to the filesystem.
 Home-page: https://github.com/MNayer/fsdict
 Author: MNayer
 Author-email: marie.nayer@web.de
 License: 0BSD
 Keywords: dictionary,filesystem
 Description-Content-Type: text/markdown
```

### Comparing `filesystem-dict-0.1.7/src/fsdict/fsdict.py` & `filesystem-dict-0.1.8/src/fsdict/fsdict.py`

 * *Files identical despite different names*

### Comparing `filesystem-dict-0.1.7/src/fsdict/utils.py` & `filesystem-dict-0.1.8/src/fsdict/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -36,18 +36,18 @@
 
 
 def rmsymlink(path):
     os.unlink(path)
 
 
 def rm(path):
-    if path.is_dir():
-        rmtree(path)
     if path.is_symlink():
         rmsymlink(path)
+    if path.is_dir():
+        rmtree(path)
     if path.is_file():
         rmfile(path)
 
 
 def symlink(src, dst):
     os.symlink(src, dst)
```

