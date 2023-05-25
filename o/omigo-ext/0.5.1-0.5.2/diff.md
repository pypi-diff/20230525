# Comparing `tmp/omigo_ext-0.5.1.tar.gz` & `tmp/omigo_ext-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omigo_ext-0.5.1.tar", last modified: Thu May 25 19:10:22 2023, max compression
+gzip compressed data, was "omigo_ext-0.5.2.tar", last modified: Thu May 25 19:17:08 2023, max compression
```

## Comparing `omigo_ext-0.5.1.tar` & `omigo_ext-0.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:10:22.486436 omigo_ext-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-25 19:10:22.486436 omigo_ext-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:39.000000 omigo_ext-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 19:09:39.000000 omigo_ext-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-25 19:10:22.486436 omigo_ext-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:10:22.482436 omigo_ext-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:10:22.486436 omigo_ext-0.5.1/src/omigo_ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:09:39.000000 omigo_ext-0.5.1/src/omigo_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-25 19:09:39.000000 omigo_ext-0.5.1/src/omigo_ext/etl_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-05-25 19:09:39.000000 omigo_ext-0.5.1/src/omigo_ext/graph_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-25 19:09:39.000000 omigo_ext-0.5.1/src/omigo_ext/graphviz_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-25 19:09:39.000000 omigo_ext-0.5.1/src/omigo_ext/kafka_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-25 19:09:39.000000 omigo_ext-0.5.1/src/omigo_ext/multithread_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-05-25 19:09:39.000000 omigo_ext-0.5.1/src/omigo_ext/ws_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:10:22.486436 omigo_ext-0.5.1/src/omigo_ext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-25 19:10:22.000000 omigo_ext-0.5.1/src/omigo_ext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-25 19:10:22.000000 omigo_ext-0.5.1/src/omigo_ext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:10:22.000000 omigo_ext-0.5.1/src/omigo_ext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-25 19:10:22.000000 omigo_ext-0.5.1/src/omigo_ext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 19:10:22.000000 omigo_ext-0.5.1/src/omigo_ext.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:17:08.084353 omigo_ext-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-25 19:17:08.084353 omigo_ext-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:29.000000 omigo_ext-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 19:16:29.000000 omigo_ext-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-25 19:17:08.084353 omigo_ext-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:17:08.084353 omigo_ext-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:17:08.084353 omigo_ext-0.5.2/src/omigo_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:29.000000 omigo_ext-0.5.2/src/omigo_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-25 19:16:29.000000 omigo_ext-0.5.2/src/omigo_ext/etl_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-05-25 19:16:29.000000 omigo_ext-0.5.2/src/omigo_ext/graph_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-25 19:16:29.000000 omigo_ext-0.5.2/src/omigo_ext/graphviz_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-25 19:16:29.000000 omigo_ext-0.5.2/src/omigo_ext/kafka_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-25 19:16:29.000000 omigo_ext-0.5.2/src/omigo_ext/multithread_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-05-25 19:16:29.000000 omigo_ext-0.5.2/src/omigo_ext/ws_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:17:08.084353 omigo_ext-0.5.2/src/omigo_ext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-25 19:17:08.000000 omigo_ext-0.5.2/src/omigo_ext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-25 19:17:08.000000 omigo_ext-0.5.2/src/omigo_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:17:08.000000 omigo_ext-0.5.2/src/omigo_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-25 19:17:08.000000 omigo_ext-0.5.2/src/omigo_ext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 19:17:08.000000 omigo_ext-0.5.2/src/omigo_ext.egg-info/top_level.txt
```

### Comparing `omigo_ext-0.5.1/setup.cfg` & `omigo_ext-0.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = omigo_ext
-version = 0.5.1
+version = 0.5.2
 author = amit jaiswal
 author_email = amit.jaiswal@gmail.com
 description = Extensions for omigo_core package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CrowdStrike/omigo-data-analytics
 project_urls =
```

### Comparing `omigo_ext-0.5.1/src/omigo_ext/etl_ext.py` & `omigo_ext-0.5.2/src/omigo_ext/etl_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.1/src/omigo_ext/graph_ext.py` & `omigo_ext-0.5.2/src/omigo_ext/graph_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.1/src/omigo_ext/graphviz_ext.py` & `omigo_ext-0.5.2/src/omigo_ext/graphviz_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.1/src/omigo_ext/kafka_ext.py` & `omigo_ext-0.5.2/src/omigo_ext/kafka_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.1/src/omigo_ext/multithread_ext.py` & `omigo_ext-0.5.2/src/omigo_ext/multithread_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.1/src/omigo_ext/ws_ext.py` & `omigo_ext-0.5.2/src/omigo_ext/ws_ext.py`

 * *Files identical despite different names*

