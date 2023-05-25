# Comparing `tmp/dbt-invoke-0.2.2.tar.gz` & `tmp/dbt-invoke-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-invoke-0.2.2.tar", last modified: Wed May 24 00:47:42 2023, max compression
+gzip compressed data, was "dbt-invoke-0.2.3.tar", last modified: Thu May 25 16:02:16 2023, max compression
```

## Comparing `dbt-invoke-0.2.2.tar` & `dbt-invoke-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:47:42.184163 dbt-invoke-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 00:47:27.000000 dbt-invoke-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-05-24 00:47:42.184163 dbt-invoke-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-05-24 00:47:27.000000 dbt-invoke-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:47:42.180163 dbt-invoke-0.2.2/dbt_invoke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 00:47:27.000000 dbt-invoke-0.2.2/dbt_invoke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:47:42.184163 dbt-invoke-0.2.2/dbt_invoke/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 00:47:27.000000 dbt-invoke-0.2.2/dbt_invoke/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-05-24 00:47:27.000000 dbt-invoke-0.2.2/dbt_invoke/internal/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 00:47:27.000000 dbt-invoke-0.2.2/dbt_invoke/internal/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-24 00:47:27.000000 dbt-invoke-0.2.2/dbt_invoke/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    33712 2023-05-24 00:47:27.000000 dbt-invoke-0.2.2/dbt_invoke/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:47:42.184163 dbt-invoke-0.2.2/dbt_invoke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-05-24 00:47:41.000000 dbt-invoke-0.2.2/dbt_invoke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-24 00:47:42.000000 dbt-invoke-0.2.2/dbt_invoke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 00:47:41.000000 dbt-invoke-0.2.2/dbt_invoke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-24 00:47:41.000000 dbt-invoke-0.2.2/dbt_invoke.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-24 00:47:41.000000 dbt-invoke-0.2.2/dbt_invoke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 00:47:41.000000 dbt-invoke-0.2.2/dbt_invoke.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 00:47:42.184163 dbt-invoke-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-24 00:47:27.000000 dbt-invoke-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:02:16.217635 dbt-invoke-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 16:02:05.000000 dbt-invoke-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-05-25 16:02:16.217635 dbt-invoke-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-05-25 16:02:05.000000 dbt-invoke-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:02:16.217635 dbt-invoke-0.2.3/dbt_invoke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:02:05.000000 dbt-invoke-0.2.3/dbt_invoke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:02:16.217635 dbt-invoke-0.2.3/dbt_invoke/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:02:05.000000 dbt-invoke-0.2.3/dbt_invoke/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-05-25 16:02:05.000000 dbt-invoke-0.2.3/dbt_invoke/internal/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 16:02:05.000000 dbt-invoke-0.2.3/dbt_invoke/internal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-25 16:02:05.000000 dbt-invoke-0.2.3/dbt_invoke/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33712 2023-05-25 16:02:05.000000 dbt-invoke-0.2.3/dbt_invoke/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:02:16.217635 dbt-invoke-0.2.3/dbt_invoke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-05-25 16:02:16.000000 dbt-invoke-0.2.3/dbt_invoke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-25 16:02:16.000000 dbt-invoke-0.2.3/dbt_invoke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:02:16.000000 dbt-invoke-0.2.3/dbt_invoke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 16:02:16.000000 dbt-invoke-0.2.3/dbt_invoke.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 16:02:16.000000 dbt-invoke-0.2.3/dbt_invoke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 16:02:16.000000 dbt-invoke-0.2.3/dbt_invoke.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 16:02:16.217635 dbt-invoke-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-25 16:02:05.000000 dbt-invoke-0.2.3/setup.py
```

### Comparing `dbt-invoke-0.2.2/LICENSE` & `dbt-invoke-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-invoke-0.2.2/PKG-INFO` & `dbt-invoke-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-invoke
-Version: 0.2.2
+Version: 0.2.3
 Summary: dbt-invoke is a CLI for creating, updating, and deleting dbt property files.
 Home-page: https://github.com/Dashlane/dbt-invoke
 Author: Robert Astel, Jennifer Zhan, Vincent Dragonette
 Author-email: rob.astel@gmail.com
 License: Apache License 2.0
 Description: # dbt-invoke
```

### Comparing `dbt-invoke-0.2.2/README.md` & `dbt-invoke-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-invoke-0.2.2/dbt_invoke/internal/_utils.py` & `dbt-invoke-0.2.3/dbt_invoke/internal/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     """
     Parse a yaml file
 
     :param location: The location of the yaml file to parse
     :return: The contents of the yaml file
     """
     yaml = YAML(typ="rt")
+    yaml.preserve_quotes = True
     with open(location, 'r') as stream:
         try:
             parsed_yaml = yaml.load(stream)
             return parsed_yaml
         except YAMLError as exc:
             sys.exit(exc)
 
@@ -97,14 +98,15 @@
 
     :param location: The location to which to write the yaml file
     :param data: The object which will be written to the yaml file
     :param mode: The mode in which to open the yaml file
     :return: None
     """
     yaml = YAML(typ="rt")
+    yaml.preserve_quotes = True
     try:
         with open(location, mode) as stream:
             yaml.dump(data, stream)
     except YAMLError as exc:
         sys.exit(exc)
```

### Comparing `dbt-invoke-0.2.2/dbt_invoke/properties.py` & `dbt-invoke-0.2.3/dbt_invoke/properties.py`

 * *Files identical despite different names*

### Comparing `dbt-invoke-0.2.2/dbt_invoke.egg-info/PKG-INFO` & `dbt-invoke-0.2.3/dbt_invoke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-invoke
-Version: 0.2.2
+Version: 0.2.3
 Summary: dbt-invoke is a CLI for creating, updating, and deleting dbt property files.
 Home-page: https://github.com/Dashlane/dbt-invoke
 Author: Robert Astel, Jennifer Zhan, Vincent Dragonette
 Author-email: rob.astel@gmail.com
 License: Apache License 2.0
 Description: # dbt-invoke
```

### Comparing `dbt-invoke-0.2.2/setup.py` & `dbt-invoke-0.2.3/setup.py`

 * *Files identical despite different names*

