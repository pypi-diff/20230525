# Comparing `tmp/fast-nbs-0.0.1.tar.gz` & `tmp/fast-nbs-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-nbs-0.0.1.tar", last modified: Thu May 25 02:50:26 2023, max compression
+gzip compressed data, was "fast-nbs-0.0.1a0.tar", last modified: Wed May 17 01:26:56 2023, max compression
```

## Comparing `fast-nbs-0.0.1.tar` & `fast-nbs-0.0.1a0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 02:50:26.148537 fast-nbs-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-05-14 01:20:08.000000 fast-nbs-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2942 2023-05-25 02:50:26.148537 fast-nbs-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      544 2023-05-17 01:26:40.000000 fast-nbs-0.0.1/README.md
--rw-rw-rw-   0        0        0     6185 2023-05-25 02:49:52.000000 fast-nbs-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 02:50:26.148537 fast-nbs-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 02:50:26.132913 fast-nbs-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 02:50:26.148537 fast-nbs-0.0.1/src/fast_nbs.egg-info/
--rw-rw-rw-   0        0        0     2942 2023-05-25 02:50:26.000000 fast-nbs-0.0.1/src/fast_nbs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-05-25 02:50:26.000000 fast-nbs-0.0.1/src/fast_nbs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 02:50:26.000000 fast-nbs-0.0.1/src/fast_nbs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-05-25 02:50:26.000000 fast-nbs-0.0.1/src/fast_nbs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 02:50:26.000000 fast-nbs-0.0.1/src/fast_nbs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 02:50:26.148537 fast-nbs-0.0.1/src/fastnbs/
--rw-rw-rw-   0        0        0       25 2023-05-17 01:13:07.000000 fast-nbs-0.0.1/src/fastnbs/__init__.py
--rw-rw-rw-   0        0        0     2832 2023-05-17 01:13:07.000000 fast-nbs-0.0.1/src/fastnbs/nbs.py
--rw-rw-rw-   0        0        0      885 2023-05-17 01:06:11.000000 fast-nbs-0.0.1/src/fastnbs/vis.py
+drwxrwxrwx   0        0        0        0 2023-05-17 01:26:56.511315 fast-nbs-0.0.1a0/
+-rw-rw-rw-   0        0        0     1088 2023-05-14 01:20:08.000000 fast-nbs-0.0.1a0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2944 2023-05-17 01:26:56.511315 fast-nbs-0.0.1a0/PKG-INFO
+-rw-rw-rw-   0        0        0      544 2023-05-17 01:26:40.000000 fast-nbs-0.0.1a0/README.md
+-rw-rw-rw-   0        0        0     6187 2023-05-17 01:03:51.000000 fast-nbs-0.0.1a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 01:26:56.511315 fast-nbs-0.0.1a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 01:26:56.498321 fast-nbs-0.0.1a0/src/
+drwxrwxrwx   0        0        0        0 2023-05-17 01:26:56.508347 fast-nbs-0.0.1a0/src/fast_nbs.egg-info/
+-rw-rw-rw-   0        0        0     2944 2023-05-17 01:26:56.000000 fast-nbs-0.0.1a0/src/fast_nbs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-05-17 01:26:56.000000 fast-nbs-0.0.1a0/src/fast_nbs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 01:26:56.000000 fast-nbs-0.0.1a0/src/fast_nbs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-17 01:26:56.000000 fast-nbs-0.0.1a0/src/fast_nbs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-17 01:26:56.000000 fast-nbs-0.0.1a0/src/fast_nbs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 01:26:56.510317 fast-nbs-0.0.1a0/src/fastnbs/
+-rw-rw-rw-   0        0        0       25 2023-05-17 01:13:07.000000 fast-nbs-0.0.1a0/src/fastnbs/__init__.py
+-rw-rw-rw-   0        0        0     2832 2023-05-17 01:13:07.000000 fast-nbs-0.0.1a0/src/fastnbs/nbs.py
+-rw-rw-rw-   0        0        0      885 2023-05-17 01:06:11.000000 fast-nbs-0.0.1a0/src/fastnbs/vis.py
```

### Comparing `fast-nbs-0.0.1/LICENSE.txt` & `fast-nbs-0.0.1a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fast-nbs-0.0.1/PKG-INFO` & `fast-nbs-0.0.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-nbs
-Version: 0.0.1
+Version: 0.0.1a0
 Summary: Import jupyter notebooks fast
 Author-email: Donghua Chen <douglaschan@126.com>
 License: MIT License
         
         Copyright (c) 2023 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fast-nbs-0.0.1/README.md` & `fast-nbs-0.0.1a0/README.md`

 * *Files identical despite different names*

### Comparing `fast-nbs-0.0.1/pyproject.toml` & `fast-nbs-0.0.1a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "fast-nbs"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.1"  # Required
+version = "0.0.1a0"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Import jupyter notebooks fast"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `fast-nbs-0.0.1/src/fast_nbs.egg-info/PKG-INFO` & `fast-nbs-0.0.1a0/src/fast_nbs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-nbs
-Version: 0.0.1
+Version: 0.0.1a0
 Summary: Import jupyter notebooks fast
 Author-email: Donghua Chen <douglaschan@126.com>
 License: MIT License
         
         Copyright (c) 2023 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fast-nbs-0.0.1/src/fastnbs/nbs.py` & `fast-nbs-0.0.1a0/src/fastnbs/nbs.py`

 * *Files identical despite different names*

### Comparing `fast-nbs-0.0.1/src/fastnbs/vis.py` & `fast-nbs-0.0.1a0/src/fastnbs/vis.py`

 * *Files identical despite different names*

