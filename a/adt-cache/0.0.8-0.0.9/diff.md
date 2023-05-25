# Comparing `tmp/adt_cache-0.0.8.tar.gz` & `tmp/adt_cache-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adt_cache-0.0.8.tar", last modified: Thu May 25 13:04:45 2023, max compression
+gzip compressed data, was "dist/adt_cache-0.0.9.tar", last modified: Thu May 25 14:22:23 2023, max compression
```

## Comparing `adt_cache-0.0.8.tar` & `adt_cache-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-25 13:04:45.000000 adt_cache-0.0.8/
--rw-r--r--   0 nezah      (501) staff       (20)      597 2023-05-25 13:04:45.000000 adt_cache-0.0.8/PKG-INFO
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-25 13:04:45.000000 adt_cache-0.0.8/cache/
--rw-r--r--   0 nezah      (501) staff       (20)     3584 2023-05-25 13:04:42.000000 adt_cache-0.0.8/cache/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)     1071 2023-04-05 05:19:07.000000 adt_cache-0.0.8/LICENSE
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-25 13:04:45.000000 adt_cache-0.0.8/adt_cache.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      597 2023-05-25 13:04:45.000000 adt_cache-0.0.8/adt_cache.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      176 2023-05-25 13:04:45.000000 adt_cache-0.0.8/adt_cache.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        6 2023-05-25 13:04:45.000000 adt_cache-0.0.8/adt_cache.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-25 13:04:45.000000 adt_cache-0.0.8/adt_cache.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)      172 2023-04-05 05:18:33.000000 adt_cache-0.0.8/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      548 2023-05-25 13:04:42.000000 adt_cache-0.0.8/setup.py
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-25 13:04:45.000000 adt_cache-0.0.8/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-25 14:22:23.000000 adt_cache-0.0.9/
+-rw-r--r--   0 nezah      (501) staff       (20)      597 2023-05-25 14:22:23.000000 adt_cache-0.0.9/PKG-INFO
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-25 14:22:23.000000 adt_cache-0.0.9/cache/
+-rw-r--r--   0 nezah      (501) staff       (20)     3584 2023-05-25 13:04:42.000000 adt_cache-0.0.9/cache/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1098 2023-05-25 14:22:21.000000 adt_cache-0.0.9/cache/filecache.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1071 2023-04-05 05:19:07.000000 adt_cache-0.0.9/LICENSE
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-25 14:22:23.000000 adt_cache-0.0.9/adt_cache.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      597 2023-05-25 14:22:23.000000 adt_cache-0.0.9/adt_cache.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      195 2023-05-25 14:22:23.000000 adt_cache-0.0.9/adt_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        6 2023-05-25 14:22:23.000000 adt_cache-0.0.9/adt_cache.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-25 14:22:23.000000 adt_cache-0.0.9/adt_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)      172 2023-04-05 05:18:33.000000 adt_cache-0.0.9/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      548 2023-05-25 14:22:21.000000 adt_cache-0.0.9/setup.py
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-25 14:22:23.000000 adt_cache-0.0.9/setup.cfg
```

### Comparing `adt_cache-0.0.8/PKG-INFO` & `adt_cache-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt_cache
-Version: 0.0.8
+Version: 0.0.9
 Summary: abstract cache with in memory cache or redis (sentinel)
 Home-page: https://github.com/cheddars/pypi_adt_cache
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `adt_cache-0.0.8/cache/__init__.py` & `adt_cache-0.0.9/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `adt_cache-0.0.8/LICENSE` & `adt_cache-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adt_cache-0.0.8/adt_cache.egg-info/PKG-INFO` & `adt_cache-0.0.9/adt_cache.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt-cache
-Version: 0.0.8
+Version: 0.0.9
 Summary: abstract cache with in memory cache or redis (sentinel)
 Home-page: https://github.com/cheddars/pypi_adt_cache
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `adt_cache-0.0.8/setup.py` & `adt_cache-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="adt_cache",
-    version="0.0.8",
+    version="0.0.9",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="abstract cache with in memory cache or redis (sentinel)",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/pypi_adt_cache",
     packages=setuptools.find_packages(),
```

