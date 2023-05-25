# Comparing `tmp/pyrosexmod-0.1.1.tar.gz` & `tmp/pyrosexmod-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrosexmod-0.1.1.tar", last modified: Thu May 25 10:26:16 2023, max compression
+gzip compressed data, was "pyrosexmod-0.1.2.tar", last modified: Thu May 25 10:43:27 2023, max compression
```

## Comparing `pyrosexmod-0.1.1.tar` & `pyrosexmod-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:26:16.064503 pyrosexmod-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-25 10:26:04.000000 pyrosexmod-0.1.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-25 10:26:04.000000 pyrosexmod-0.1.1/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-25 10:26:04.000000 pyrosexmod-0.1.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 10:26:16.064503 pyrosexmod-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-25 10:26:04.000000 pyrosexmod-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:26:16.064503 pyrosexmod-0.1.1/pyrosexmod/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 10:26:04.000000 pyrosexmod-0.1.1/pyrosexmod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:26:16.064503 pyrosexmod-0.1.1/pyrosexmod/filters/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 10:26:04.000000 pyrosexmod-0.1.1/pyrosexmod/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 10:26:04.000000 pyrosexmod-0.1.1/pyrosexmod/filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:26:16.064503 pyrosexmod-0.1.1/pyrosexmod/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 10:26:04.000000 pyrosexmod-0.1.1/pyrosexmod/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-25 10:26:04.000000 pyrosexmod-0.1.1/pyrosexmod/helpers/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:26:16.064503 pyrosexmod-0.1.1/pyrosexmod/listen/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 10:26:04.000000 pyrosexmod-0.1.1/pyrosexmod/listen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-25 10:26:04.000000 pyrosexmod-0.1.1/pyrosexmod/listen/listen.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-25 10:26:04.000000 pyrosexmod-0.1.1/pyrosexmod/teledl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:26:16.064503 pyrosexmod-0.1.1/pyrosexmod/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 10:26:04.000000 pyrosexmod-0.1.1/pyrosexmod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-25 10:26:04.000000 pyrosexmod-0.1.1/pyrosexmod/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:26:16.064503 pyrosexmod-0.1.1/pyrosexmod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 10:26:16.000000 pyrosexmod-0.1.1/pyrosexmod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 10:26:16.000000 pyrosexmod-0.1.1/pyrosexmod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 10:26:16.000000 pyrosexmod-0.1.1/pyrosexmod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 10:26:16.000000 pyrosexmod-0.1.1/pyrosexmod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 10:26:16.000000 pyrosexmod-0.1.1/pyrosexmod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 10:26:16.064503 pyrosexmod-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-25 10:26:04.000000 pyrosexmod-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:43:27.512914 pyrosexmod-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-25 10:43:15.000000 pyrosexmod-0.1.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-25 10:43:15.000000 pyrosexmod-0.1.2/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-25 10:43:15.000000 pyrosexmod-0.1.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 10:43:27.508913 pyrosexmod-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-25 10:43:15.000000 pyrosexmod-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:43:27.504913 pyrosexmod-0.1.2/pyrosexmod/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 10:43:15.000000 pyrosexmod-0.1.2/pyrosexmod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:43:27.508913 pyrosexmod-0.1.2/pyrosexmod/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 10:43:15.000000 pyrosexmod-0.1.2/pyrosexmod/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 10:43:15.000000 pyrosexmod-0.1.2/pyrosexmod/filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:43:27.508913 pyrosexmod-0.1.2/pyrosexmod/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 10:43:15.000000 pyrosexmod-0.1.2/pyrosexmod/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-25 10:43:15.000000 pyrosexmod-0.1.2/pyrosexmod/helpers/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:43:27.508913 pyrosexmod-0.1.2/pyrosexmod/listen/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 10:43:15.000000 pyrosexmod-0.1.2/pyrosexmod/listen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-25 10:43:15.000000 pyrosexmod-0.1.2/pyrosexmod/listen/listen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-25 10:43:15.000000 pyrosexmod-0.1.2/pyrosexmod/teledl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:43:27.508913 pyrosexmod-0.1.2/pyrosexmod/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 10:43:15.000000 pyrosexmod-0.1.2/pyrosexmod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-25 10:43:15.000000 pyrosexmod-0.1.2/pyrosexmod/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:43:27.508913 pyrosexmod-0.1.2/pyrosexmod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 10:43:27.000000 pyrosexmod-0.1.2/pyrosexmod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 10:43:27.000000 pyrosexmod-0.1.2/pyrosexmod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 10:43:27.000000 pyrosexmod-0.1.2/pyrosexmod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 10:43:27.000000 pyrosexmod-0.1.2/pyrosexmod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 10:43:27.000000 pyrosexmod-0.1.2/pyrosexmod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 10:43:27.512914 pyrosexmod-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-25 10:43:15.000000 pyrosexmod-0.1.2/setup.py
```

### Comparing `pyrosexmod-0.1.1/COPYING` & `pyrosexmod-0.1.2/COPYING`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.1.1/COPYING.lesser` & `pyrosexmod-0.1.2/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.1.1/NOTICE` & `pyrosexmod-0.1.2/NOTICE`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.1.1/PKG-INFO` & `pyrosexmod-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrosexmod
-Version: 0.1.1
+Version: 0.1.2
 Summary: A monkeypatcher add-on for Pyrosex
 Home-page: https://github.com/OTHFamily/pyrosexmod
 Author: OTH
 Author-email: oth@pyrosex.org
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `pyrosexmod-0.1.1/README.md` & `pyrosexmod-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.1.1/pyrosexmod/helpers/helpers.py` & `pyrosexmod-0.1.2/pyrosexmod/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.1.1/pyrosexmod/listen/listen.py` & `pyrosexmod-0.1.2/pyrosexmod/listen/listen.py`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.1.1/pyrosexmod.egg-info/PKG-INFO` & `pyrosexmod-0.1.2/pyrosexmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrosexmod
-Version: 0.1.1
+Version: 0.1.2
 Summary: A monkeypatcher add-on for Pyrosex
 Home-page: https://github.com/OTHFamily/pyrosexmod
 Author: OTH
 Author-email: oth@pyrosex.org
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `pyrosexmod-0.1.1/setup.py` & `pyrosexmod-0.1.2/setup.py`

 * *Files identical despite different names*

