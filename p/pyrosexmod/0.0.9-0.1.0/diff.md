# Comparing `tmp/pyrosexmod-0.0.9.tar.gz` & `tmp/pyrosexmod-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrosexmod-0.0.9.tar", last modified: Thu May 25 09:21:18 2023, max compression
+gzip compressed data, was "pyrosexmod-0.1.0.tar", last modified: Thu May 25 09:44:39 2023, max compression
```

## Comparing `pyrosexmod-0.0.9.tar` & `pyrosexmod-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:21:18.334339 pyrosexmod-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 09:21:18.330339 pyrosexmod-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:21:18.330339 pyrosexmod-0.0.9/pyrosexmod/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:21:18.330339 pyrosexmod-0.0.9/pyrosexmod/filters/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:21:18.330339 pyrosexmod-0.0.9/pyrosexmod/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/helpers/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:21:18.330339 pyrosexmod-0.0.9/pyrosexmod/listen/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/listen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/listen/listen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/teledl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:21:18.330339 pyrosexmod-0.0.9/pyrosexmod/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/pyrosexmod/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:21:18.330339 pyrosexmod-0.0.9/pyrosexmod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 09:21:18.000000 pyrosexmod-0.0.9/pyrosexmod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 09:21:18.000000 pyrosexmod-0.0.9/pyrosexmod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:21:18.000000 pyrosexmod-0.0.9/pyrosexmod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 09:21:18.000000 pyrosexmod-0.0.9/pyrosexmod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 09:21:18.000000 pyrosexmod-0.0.9/pyrosexmod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:21:18.334339 pyrosexmod-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-25 09:21:05.000000 pyrosexmod-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:44:39.765866 pyrosexmod-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-25 09:44:26.000000 pyrosexmod-0.1.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-25 09:44:26.000000 pyrosexmod-0.1.0/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-25 09:44:26.000000 pyrosexmod-0.1.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 09:44:39.765866 pyrosexmod-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-25 09:44:26.000000 pyrosexmod-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:44:39.761866 pyrosexmod-0.1.0/pyrosexmod/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 09:44:26.000000 pyrosexmod-0.1.0/pyrosexmod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:44:39.761866 pyrosexmod-0.1.0/pyrosexmod/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 09:44:26.000000 pyrosexmod-0.1.0/pyrosexmod/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 09:44:26.000000 pyrosexmod-0.1.0/pyrosexmod/filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:44:39.761866 pyrosexmod-0.1.0/pyrosexmod/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 09:44:26.000000 pyrosexmod-0.1.0/pyrosexmod/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-25 09:44:26.000000 pyrosexmod-0.1.0/pyrosexmod/helpers/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:44:39.761866 pyrosexmod-0.1.0/pyrosexmod/listen/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 09:44:26.000000 pyrosexmod-0.1.0/pyrosexmod/listen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-25 09:44:26.000000 pyrosexmod-0.1.0/pyrosexmod/listen/listen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-25 09:44:26.000000 pyrosexmod-0.1.0/pyrosexmod/teledl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:44:39.761866 pyrosexmod-0.1.0/pyrosexmod/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 09:44:26.000000 pyrosexmod-0.1.0/pyrosexmod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-25 09:44:26.000000 pyrosexmod-0.1.0/pyrosexmod/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:44:39.761866 pyrosexmod-0.1.0/pyrosexmod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 09:44:39.000000 pyrosexmod-0.1.0/pyrosexmod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 09:44:39.000000 pyrosexmod-0.1.0/pyrosexmod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:44:39.000000 pyrosexmod-0.1.0/pyrosexmod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 09:44:39.000000 pyrosexmod-0.1.0/pyrosexmod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 09:44:39.000000 pyrosexmod-0.1.0/pyrosexmod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:44:39.765866 pyrosexmod-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-25 09:44:26.000000 pyrosexmod-0.1.0/setup.py
```

### Comparing `pyrosexmod-0.0.9/COPYING` & `pyrosexmod-0.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.9/COPYING.lesser` & `pyrosexmod-0.1.0/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.9/NOTICE` & `pyrosexmod-0.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.9/PKG-INFO` & `pyrosexmod-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrosexmod
-Version: 0.0.9
+Version: 0.1.0
 Summary: A monkeypatcher add-on for Pyrosex
 Home-page: https://github.com/OTHFamily/pyrosexmod
 Author: OTH
 Author-email: oth@pyrosex.org
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `pyrosexmod-0.0.9/README.md` & `pyrosexmod-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.9/pyrosexmod/helpers/helpers.py` & `pyrosexmod-0.1.0/pyrosexmod/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.9/pyrosexmod/listen/listen.py` & `pyrosexmod-0.1.0/pyrosexmod/listen/listen.py`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.9/pyrosexmod.egg-info/PKG-INFO` & `pyrosexmod-0.1.0/pyrosexmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrosexmod
-Version: 0.0.9
+Version: 0.1.0
 Summary: A monkeypatcher add-on for Pyrosex
 Home-page: https://github.com/OTHFamily/pyrosexmod
 Author: OTH
 Author-email: oth@pyrosex.org
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `pyrosexmod-0.0.9/setup.py` & `pyrosexmod-0.1.0/setup.py`

 * *Files identical despite different names*

