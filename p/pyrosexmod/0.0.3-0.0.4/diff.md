# Comparing `tmp/pyrosexmod-0.0.3.tar.gz` & `tmp/pyrosexmod-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrosexmod-0.0.3.tar", last modified: Sun May  7 11:36:28 2023, max compression
+gzip compressed data, was "pyrosexmod-0.0.4.tar", last modified: Thu May 25 06:37:43 2023, max compression
```

## Comparing `pyrosexmod-0.0.3.tar` & `pyrosexmod-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:36:28.153687 pyrosexmod-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-07 11:36:16.000000 pyrosexmod-0.0.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-07 11:36:16.000000 pyrosexmod-0.0.3/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-07 11:36:16.000000 pyrosexmod-0.0.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-07 11:36:28.153687 pyrosexmod-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-07 11:36:16.000000 pyrosexmod-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:36:28.153687 pyrosexmod-0.0.3/pyrosexmod/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-07 11:36:16.000000 pyrosexmod-0.0.3/pyrosexmod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:36:28.153687 pyrosexmod-0.0.3/pyrosexmod/filters/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-07 11:36:16.000000 pyrosexmod-0.0.3/pyrosexmod/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-07 11:36:16.000000 pyrosexmod-0.0.3/pyrosexmod/filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:36:28.153687 pyrosexmod-0.0.3/pyrosexmod/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 11:36:16.000000 pyrosexmod-0.0.3/pyrosexmod/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-07 11:36:16.000000 pyrosexmod-0.0.3/pyrosexmod/helpers/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:36:28.153687 pyrosexmod-0.0.3/pyrosexmod/listen/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-07 11:36:16.000000 pyrosexmod-0.0.3/pyrosexmod/listen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-07 11:36:16.000000 pyrosexmod-0.0.3/pyrosexmod/listen/listen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:36:28.153687 pyrosexmod-0.0.3/pyrosexmod/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-07 11:36:16.000000 pyrosexmod-0.0.3/pyrosexmod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-07 11:36:16.000000 pyrosexmod-0.0.3/pyrosexmod/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:36:28.153687 pyrosexmod-0.0.3/pyrosexmod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-07 11:36:28.000000 pyrosexmod-0.0.3/pyrosexmod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-07 11:36:28.000000 pyrosexmod-0.0.3/pyrosexmod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 11:36:28.000000 pyrosexmod-0.0.3/pyrosexmod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 11:36:28.000000 pyrosexmod-0.0.3/pyrosexmod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 11:36:28.000000 pyrosexmod-0.0.3/pyrosexmod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 11:36:28.153687 pyrosexmod-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-07 11:36:16.000000 pyrosexmod-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:37:43.248069 pyrosexmod-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-25 06:37:27.000000 pyrosexmod-0.0.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-25 06:37:27.000000 pyrosexmod-0.0.4/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-25 06:37:27.000000 pyrosexmod-0.0.4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 06:37:43.248069 pyrosexmod-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-25 06:37:27.000000 pyrosexmod-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:37:43.244069 pyrosexmod-0.0.4/pyrosexmod/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 06:37:27.000000 pyrosexmod-0.0.4/pyrosexmod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:37:43.248069 pyrosexmod-0.0.4/pyrosexmod/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 06:37:27.000000 pyrosexmod-0.0.4/pyrosexmod/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 06:37:27.000000 pyrosexmod-0.0.4/pyrosexmod/filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:37:43.248069 pyrosexmod-0.0.4/pyrosexmod/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 06:37:27.000000 pyrosexmod-0.0.4/pyrosexmod/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-25 06:37:27.000000 pyrosexmod-0.0.4/pyrosexmod/helpers/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:37:43.248069 pyrosexmod-0.0.4/pyrosexmod/listen/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 06:37:27.000000 pyrosexmod-0.0.4/pyrosexmod/listen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-25 06:37:27.000000 pyrosexmod-0.0.4/pyrosexmod/listen/listen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-25 06:37:27.000000 pyrosexmod-0.0.4/pyrosexmod/teledl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:37:43.248069 pyrosexmod-0.0.4/pyrosexmod/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 06:37:27.000000 pyrosexmod-0.0.4/pyrosexmod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-25 06:37:27.000000 pyrosexmod-0.0.4/pyrosexmod/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:37:43.248069 pyrosexmod-0.0.4/pyrosexmod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-25 06:37:43.000000 pyrosexmod-0.0.4/pyrosexmod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 06:37:43.000000 pyrosexmod-0.0.4/pyrosexmod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 06:37:43.000000 pyrosexmod-0.0.4/pyrosexmod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 06:37:43.000000 pyrosexmod-0.0.4/pyrosexmod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 06:37:43.000000 pyrosexmod-0.0.4/pyrosexmod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 06:37:43.248069 pyrosexmod-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-25 06:37:27.000000 pyrosexmod-0.0.4/setup.py
```

### Comparing `pyrosexmod-0.0.3/COPYING` & `pyrosexmod-0.0.4/COPYING`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.3/COPYING.lesser` & `pyrosexmod-0.0.4/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.3/NOTICE` & `pyrosexmod-0.0.4/NOTICE`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.3/PKG-INFO` & `pyrosexmod-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrosexmod
-Version: 0.0.3
+Version: 0.0.4
 Summary: A monkeypatcher add-on for Pyrosex
 Home-page: https://github.com/OTHFamily/pyrosexmod
 Author: OTH
 Author-email: oth@pyrosex.org
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `pyrosexmod-0.0.3/README.md` & `pyrosexmod-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.3/pyrosexmod/helpers/helpers.py` & `pyrosexmod-0.0.4/pyrosexmod/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.3/pyrosexmod/listen/listen.py` & `pyrosexmod-0.0.4/pyrosexmod/listen/listen.py`

 * *Files identical despite different names*

### Comparing `pyrosexmod-0.0.3/pyrosexmod.egg-info/PKG-INFO` & `pyrosexmod-0.0.4/pyrosexmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrosexmod
-Version: 0.0.3
+Version: 0.0.4
 Summary: A monkeypatcher add-on for Pyrosex
 Home-page: https://github.com/OTHFamily/pyrosexmod
 Author: OTH
 Author-email: oth@pyrosex.org
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `pyrosexmod-0.0.3/setup.py` & `pyrosexmod-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,9 +21,9 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-    install_requires=["pyrosex>=0.0.3"],
+    install_requires=["pyrosex>=0.0.3", "yt-dlp"],
 )
```

