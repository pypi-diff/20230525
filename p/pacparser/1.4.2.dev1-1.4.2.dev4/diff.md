# Comparing `tmp/pacparser-1.4.2.dev1.tar.gz` & `tmp/pacparser-1.4.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pacparser-1.4.2.dev1.tar", last modified: Thu May 25 18:01:50 2023, max compression
+gzip compressed data, was "pacparser-1.4.2.dev4.tar", last modified: Thu May 25 19:09:35 2023, max compression
```

## Comparing `pacparser-1.4.2.dev1.tar` & `pacparser-1.4.2.dev4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:01:50.121781 pacparser-1.4.2.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-25 18:01:34.000000 pacparser-1.4.2.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-25 18:01:50.117780 pacparser-1.4.2.dev1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:01:50.117780 pacparser-1.4.2.dev1/pacparser/
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-25 18:01:34.000000 pacparser-1.4.2.dev1/pacparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:01:50.117780 pacparser-1.4.2.dev1/pacparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-25 18:01:50.000000 pacparser-1.4.2.dev1/pacparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-25 18:01:50.000000 pacparser-1.4.2.dev1/pacparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 18:01:50.000000 pacparser-1.4.2.dev1/pacparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 18:01:50.000000 pacparser-1.4.2.dev1/pacparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-25 18:01:34.000000 pacparser-1.4.2.dev1/pacparser_py.c
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 18:01:50.121781 pacparser-1.4.2.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-25 18:01:34.000000 pacparser-1.4.2.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:35.977335 pacparser-1.4.2.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-25 19:09:24.000000 pacparser-1.4.2.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-25 19:09:35.977335 pacparser-1.4.2.dev4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:35.977335 pacparser-1.4.2.dev4/pacparser/
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-25 19:09:24.000000 pacparser-1.4.2.dev4/pacparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:35.977335 pacparser-1.4.2.dev4/pacparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-25 19:09:35.000000 pacparser-1.4.2.dev4/pacparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-25 19:09:35.000000 pacparser-1.4.2.dev4/pacparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:09:35.000000 pacparser-1.4.2.dev4/pacparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 19:09:35.000000 pacparser-1.4.2.dev4/pacparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-25 19:09:24.000000 pacparser-1.4.2.dev4/pacparser_py.c
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 19:09:35.977335 pacparser-1.4.2.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-25 19:09:24.000000 pacparser-1.4.2.dev4/setup.py
```

### Comparing `pacparser-1.4.2.dev1/pacparser/__init__.py` & `pacparser-1.4.2.dev4/pacparser/__init__.py`

 * *Files identical despite different names*

### Comparing `pacparser-1.4.2.dev1/pacparser_py.c` & `pacparser-1.4.2.dev4/pacparser_py.c`

 * *Files identical despite different names*

### Comparing `pacparser-1.4.2.dev1/setup.py` & `pacparser-1.4.2.dev4/setup.py`

 * *Files identical despite different names*

