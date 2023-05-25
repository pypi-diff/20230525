# Comparing `tmp/eia-0.2.0.tar.gz` & `tmp/eia-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eia-0.2.0.tar", last modified: Wed May 24 22:19:15 2023, max compression
+gzip compressed data, was "eia-0.2.1.tar", last modified: Thu May 25 03:53:10 2023, max compression
```

## Comparing `eia-0.2.0.tar` & `eia-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:19:15.470555 eia-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-24 22:18:45.000000 eia-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-24 22:19:15.470555 eia-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-24 22:18:45.000000 eia-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:19:15.470555 eia-0.2.0/eia/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-24 22:18:45.000000 eia-0.2.0/eia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-24 22:18:45.000000 eia-0.2.0/eia/api_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-05-24 22:18:45.000000 eia-0.2.0/eia/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:19:15.470555 eia-0.2.0/eia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-24 22:19:15.000000 eia-0.2.0/eia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-24 22:19:15.000000 eia-0.2.0/eia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:19:15.000000 eia-0.2.0/eia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 22:19:15.000000 eia-0.2.0/eia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-24 22:19:15.000000 eia-0.2.0/eia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-24 22:18:45.000000 eia-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 22:19:15.470555 eia-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:19:15.470555 eia-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-24 22:18:45.000000 eia-0.2.0/tests/test_api_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:53:10.144040 eia-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-25 03:52:33.000000 eia-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-25 03:53:10.144040 eia-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-25 03:52:33.000000 eia-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:53:10.140040 eia-0.2.1/eia/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-25 03:52:33.000000 eia-0.2.1/eia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-25 03:52:33.000000 eia-0.2.1/eia/api_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14466 2023-05-25 03:52:33.000000 eia-0.2.1/eia/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:53:10.140040 eia-0.2.1/eia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-25 03:53:10.000000 eia-0.2.1/eia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-25 03:53:10.000000 eia-0.2.1/eia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 03:53:10.000000 eia-0.2.1/eia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-25 03:53:10.000000 eia-0.2.1/eia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 03:53:10.000000 eia-0.2.1/eia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-25 03:52:33.000000 eia-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 03:53:10.144040 eia-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:53:10.144040 eia-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-25 03:52:33.000000 eia-0.2.1/tests/test_api_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-25 03:52:33.000000 eia-0.2.1/tests/test_client.py
```

### Comparing `eia-0.2.0/LICENSE` & `eia-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eia-0.2.0/PKG-INFO` & `eia-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eia
-Version: 0.2.0
+Version: 0.2.1
 Summary: Client for interacting with the EIA API
 Author: James Campbell
 License: MIT License
         
         Copyright (c) 2023 James Campbell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `eia-0.2.0/README.md` & `eia-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `eia-0.2.0/eia/api_models.py` & `eia-0.2.1/eia/api_models.py`

 * *Files identical despite different names*

### Comparing `eia-0.2.0/eia/client.py` & `eia-0.2.1/eia/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
         """
         if series.endswith("/data"):
             logger.debug(
                 "Removing /data from series name to obtain series info. Do not use the"
                 " /data suffix for getting data using this client."
             )
             series = series[:-5]
-        info = self.series_info(series)
+        info = self.series_info(series, get_facet_info=False)
         if frequency is None:
             frequency = info.defaultFrequency
         if facets is None:
             facets = []
         if sort is None:
             sort = []
         if isinstance(facets, dict):
```

### Comparing `eia-0.2.0/eia.egg-info/PKG-INFO` & `eia-0.2.1/eia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eia
-Version: 0.2.0
+Version: 0.2.1
 Summary: Client for interacting with the EIA API
 Author: James Campbell
 License: MIT License
         
         Copyright (c) 2023 James Campbell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `eia-0.2.0/pyproject.toml` & `eia-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eia"
-version = "0.2.0"
+version = "0.2.1"
 description = "Client for interacting with the EIA API"
 authors = [
   { name = "James Campbell" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
```

### Comparing `eia-0.2.0/tests/test_api_params.py` & `eia-0.2.1/tests/test_api_params.py`

 * *Files identical despite different names*

