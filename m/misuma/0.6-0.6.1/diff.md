# Comparing `tmp/misuma-0.6.tar.gz` & `tmp/misuma-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misuma-0.6.tar", last modified: Thu May 25 18:23:43 2023, max compression
+gzip compressed data, was "misuma-0.6.1.tar", last modified: Thu May 25 18:35:50 2023, max compression
```

## Comparing `misuma-0.6.tar` & `misuma-0.6.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-25 18:23:43.774645 misuma-0.6/
--rw-r--r--   0 usuario   (1001) usuario   (1001)     1134 2023-05-16 14:58:24.000000 misuma-0.6/LICENSE
--rw-rw-r--   0 usuario   (1001) usuario   (1001)     1918 2023-05-25 18:23:43.774645 misuma-0.6/PKG-INFO
--rw-r--r--   0 usuario   (1001) usuario   (1001)     1480 2023-05-25 18:22:01.000000 misuma-0.6/README.md
-drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-25 18:23:43.774645 misuma-0.6/misuma/
--rw-r--r--   0 usuario   (1001) usuario   (1001)      222 2023-05-18 18:48:32.000000 misuma-0.6/misuma/__init__.py
-drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-25 18:23:43.774645 misuma-0.6/misuma.egg-info/
--rw-rw-r--   0 usuario   (1001) usuario   (1001)     1918 2023-05-25 18:23:43.000000 misuma-0.6/misuma.egg-info/PKG-INFO
--rw-rw-r--   0 usuario   (1001) usuario   (1001)      244 2023-05-25 18:23:43.000000 misuma-0.6/misuma.egg-info/SOURCES.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)        1 2023-05-25 18:23:43.000000 misuma-0.6/misuma.egg-info/dependency_links.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)       50 2023-05-25 18:23:43.000000 misuma-0.6/misuma.egg-info/entry_points.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)       30 2023-05-25 18:23:43.000000 misuma-0.6/misuma.egg-info/requires.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)        7 2023-05-25 18:23:43.000000 misuma-0.6/misuma.egg-info/top_level.txt
--rw-r--r--   0 usuario   (1001) usuario   (1001)      131 2023-05-16 14:58:32.000000 misuma-0.6/pyproject.toml
--rw-rw-r--   0 usuario   (1001) usuario   (1001)       38 2023-05-25 18:23:43.774645 misuma-0.6/setup.cfg
--rw-r--r--   0 usuario   (1001) usuario   (1001)     2177 2023-05-25 18:23:29.000000 misuma-0.6/setup.py
+drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-25 18:35:50.490655 misuma-0.6.1/
+-rw-r--r--   0 usuario   (1001) usuario   (1001)     1134 2023-05-16 14:58:24.000000 misuma-0.6.1/LICENSE
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)     1920 2023-05-25 18:35:50.490655 misuma-0.6.1/PKG-INFO
+-rw-r--r--   0 usuario   (1001) usuario   (1001)     1480 2023-05-25 18:22:01.000000 misuma-0.6.1/README.md
+drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-25 18:35:50.490655 misuma-0.6.1/misuma/
+-rw-r--r--   0 usuario   (1001) usuario   (1001)       91 2023-05-25 18:26:21.000000 misuma-0.6.1/misuma/__init__.py
+drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-25 18:35:50.490655 misuma-0.6.1/misuma.egg-info/
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)     1920 2023-05-25 18:35:50.000000 misuma-0.6.1/misuma.egg-info/PKG-INFO
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)      244 2023-05-25 18:35:50.000000 misuma-0.6.1/misuma.egg-info/SOURCES.txt
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)        1 2023-05-25 18:35:50.000000 misuma-0.6.1/misuma.egg-info/dependency_links.txt
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)       50 2023-05-25 18:35:50.000000 misuma-0.6.1/misuma.egg-info/entry_points.txt
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)       30 2023-05-25 18:35:50.000000 misuma-0.6.1/misuma.egg-info/requires.txt
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)        7 2023-05-25 18:35:50.000000 misuma-0.6.1/misuma.egg-info/top_level.txt
+-rw-r--r--   0 usuario   (1001) usuario   (1001)      131 2023-05-16 14:58:32.000000 misuma-0.6.1/pyproject.toml
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)       38 2023-05-25 18:35:50.490655 misuma-0.6.1/setup.cfg
+-rw-r--r--   0 usuario   (1001) usuario   (1001)     2179 2023-05-25 18:35:42.000000 misuma-0.6.1/setup.py
```

### Comparing `misuma-0.6/LICENSE` & `misuma-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `misuma-0.6/PKG-INFO` & `misuma-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misuma
-Version: 0.6
+Version: 0.6.1
 Summary: Sum two numbers
 Home-page: https://pypi.org/project/misuma
 Author: Bang1329
 Author-email: santiago.hg2292@gmail.com
 License: MIT
 Keywords: Sum Addition
 Platform: UNKNOWN
```

### Comparing `misuma-0.6/README.md` & `misuma-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `misuma-0.6/misuma.egg-info/PKG-INFO` & `misuma-0.6.1/misuma.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misuma
-Version: 0.6
+Version: 0.6.1
 Summary: Sum two numbers
 Home-page: https://pypi.org/project/misuma
 Author: Bang1329
 Author-email: santiago.hg2292@gmail.com
 License: MIT
 Keywords: Sum Addition
 Platform: UNKNOWN
```

### Comparing `misuma-0.6/setup.py` & `misuma-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # CLASSIFIER
     # ######################################################################
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         ],
-    version='0.6',
+    version='0.6.1',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={'': '.'},
     packages=setuptools.find_packages(where='.'),
```

