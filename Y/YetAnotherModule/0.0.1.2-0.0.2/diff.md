# Comparing `tmp/YetAnotherModule-0.0.1.2.tar.gz` & `tmp/YetAnotherModule-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YetAnotherModule-0.0.1.2.tar", last modified: Sat May 20 19:37:46 2023, max compression
+gzip compressed data, was "YetAnotherModule-0.0.2.tar", last modified: Wed May 24 23:33:37 2023, max compression
```

## Comparing `YetAnotherModule-0.0.1.2.tar` & `YetAnotherModule-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:37:46.930689 YetAnotherModule-0.0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-20 19:37:33.000000 YetAnotherModule-0.0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-20 19:37:46.930689 YetAnotherModule-0.0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-20 19:37:33.000000 YetAnotherModule-0.0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:37:46.926689 YetAnotherModule-0.0.1.2/YAPM/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-20 19:37:33.000000 YetAnotherModule-0.0.1.2/YAPM/Matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-20 19:37:33.000000 YetAnotherModule-0.0.1.2/YAPM/Random.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-20 19:37:33.000000 YetAnotherModule-0.0.1.2/YAPM/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:37:46.930689 YetAnotherModule-0.0.1.2/YetAnotherModule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-20 19:37:46.000000 YetAnotherModule-0.0.1.2/YetAnotherModule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-20 19:37:46.000000 YetAnotherModule-0.0.1.2/YetAnotherModule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 19:37:46.000000 YetAnotherModule-0.0.1.2/YetAnotherModule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-20 19:37:46.000000 YetAnotherModule-0.0.1.2/YetAnotherModule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 19:37:46.930689 YetAnotherModule-0.0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-20 19:37:33.000000 YetAnotherModule-0.0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:33:37.002341 YetAnotherModule-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-24 23:33:25.000000 YetAnotherModule-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-24 23:33:37.002341 YetAnotherModule-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-24 23:33:25.000000 YetAnotherModule-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:33:37.002341 YetAnotherModule-0.0.2/YAPM/
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-24 23:33:25.000000 YetAnotherModule-0.0.2/YAPM/Matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-24 23:33:25.000000 YetAnotherModule-0.0.2/YAPM/Other.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-24 23:33:25.000000 YetAnotherModule-0.0.2/YAPM/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:33:37.002341 YetAnotherModule-0.0.2/YetAnotherModule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-24 23:33:36.000000 YetAnotherModule-0.0.2/YetAnotherModule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-24 23:33:36.000000 YetAnotherModule-0.0.2/YetAnotherModule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 23:33:36.000000 YetAnotherModule-0.0.2/YetAnotherModule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 23:33:36.000000 YetAnotherModule-0.0.2/YetAnotherModule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 23:33:37.002341 YetAnotherModule-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-24 23:33:25.000000 YetAnotherModule-0.0.2/setup.py
```

### Comparing `YetAnotherModule-0.0.1.2/LICENSE` & `YetAnotherModule-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `YetAnotherModule-0.0.1.2/PKG-INFO` & `YetAnotherModule-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 Metadata-Version: 2.1
 Name: YetAnotherModule
-Version: 0.0.1.2
+Version: 0.0.2
 Summary: Yet Another Python Module.
 Home-page: https://github.com/carson-coder/Yet-Another-Python-Module
 Author: Carson
 Author-email: carsondpool@gmail.com
 License: LICENSE
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Yet Another Python Module (YAPM)
 A module where I put random stuff. Feel free to update, add, or optimize stuff just keep the syntax the same.
 
+Works with python 3.10>=
+
+## Versions
+versions go by w.x.y.z
+
+w is the amount of big updates
+x is the amount of middle updates
+y is the amount of smaller updates
+z is the amount of smallest updates. Like big fixes.
+
 ## Contributing
 If you want to contribue fork this repo and make a pull request.
 Make sure that your contribution
 
  - [ ] Keeps syntax the same (eg. function(a, b) should beable to be ran as function(a, b) without an error)
  - [ ] Useful
  - [ ] Doesn't make functions slower
```

### Comparing `YetAnotherModule-0.0.1.2/YAPM/Random.py` & `YetAnotherModule-0.0.2/YAPM/Other.py`

 * *Files identical despite different names*

### Comparing `YetAnotherModule-0.0.1.2/YetAnotherModule.egg-info/PKG-INFO` & `YetAnotherModule-0.0.2/YetAnotherModule.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 Metadata-Version: 2.1
 Name: YetAnotherModule
-Version: 0.0.1.2
+Version: 0.0.2
 Summary: Yet Another Python Module.
 Home-page: https://github.com/carson-coder/Yet-Another-Python-Module
 Author: Carson
 Author-email: carsondpool@gmail.com
 License: LICENSE
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Yet Another Python Module (YAPM)
 A module where I put random stuff. Feel free to update, add, or optimize stuff just keep the syntax the same.
 
+Works with python 3.10>=
+
+## Versions
+versions go by w.x.y.z
+
+w is the amount of big updates
+x is the amount of middle updates
+y is the amount of smaller updates
+z is the amount of smallest updates. Like big fixes.
+
 ## Contributing
 If you want to contribue fork this repo and make a pull request.
 Make sure that your contribution
 
  - [ ] Keeps syntax the same (eg. function(a, b) should beable to be ran as function(a, b) without an error)
  - [ ] Useful
  - [ ] Doesn't make functions slower
```

