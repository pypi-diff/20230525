# Comparing `tmp/synthwave-0.1.4.tar.gz` & `tmp/synthwave-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthwave-0.1.4.tar", max compression
+gzip compressed data, was "synthwave-0.1.5.tar", max compression
```

## Comparing `synthwave-0.1.4.tar` & `synthwave-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2293 2023-05-25 18:36:33.052986 synthwave-0.1.4/README.md
--rw-r--r--   0        0        0      441 2023-05-25 18:42:22.714697 synthwave-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      473 2023-05-25 17:08:52.810976 synthwave-0.1.4/synthwave/__init__.py
--rw-r--r--   0        0        0     1543 2023-05-25 18:24:16.834867 synthwave-0.1.4/synthwave/__main__.py
--rw-r--r--   0        0        0    42590 2023-05-25 16:49:53.959907 synthwave-0.1.4/synthwave/data.json
--rw-r--r--   0        0        0      729 2023-05-24 22:11:59.931095 synthwave-0.1.4/synthwave/event.py
--rw-r--r--   0        0        0     6613 2023-05-25 18:03:51.971616 synthwave-0.1.4/synthwave/field.py
--rw-r--r--   0        0        0      342 2023-05-25 18:11:48.622143 synthwave-0.1.4/synthwave/stream.py
--rw-r--r--   0        0        0      160 2023-05-24 21:50:00.797905 synthwave-0.1.4/synthwave/utils.py
--rw-r--r--   0        0        0     2669 1970-01-01 00:00:00.000000 synthwave-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2293 2023-05-25 18:36:33.052986 synthwave-0.1.5/README.md
+-rw-r--r--   0        0        0      563 2023-05-25 18:54:36.661696 synthwave-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      473 2023-05-25 17:08:52.810976 synthwave-0.1.5/synthwave/__init__.py
+-rw-r--r--   0        0        0     1543 2023-05-25 18:24:16.834867 synthwave-0.1.5/synthwave/__main__.py
+-rw-r--r--   0        0        0    42590 2023-05-25 16:49:53.959907 synthwave-0.1.5/synthwave/data.json
+-rw-r--r--   0        0        0      729 2023-05-24 22:11:59.931095 synthwave-0.1.5/synthwave/event.py
+-rw-r--r--   0        0        0     6613 2023-05-25 18:03:51.971616 synthwave-0.1.5/synthwave/field.py
+-rw-r--r--   0        0        0      342 2023-05-25 18:11:48.622143 synthwave-0.1.5/synthwave/stream.py
+-rw-r--r--   0        0        0      160 2023-05-24 21:50:00.797905 synthwave-0.1.5/synthwave/utils.py
+-rw-r--r--   0        0        0     2847 1970-01-01 00:00:00.000000 synthwave-0.1.5/PKG-INFO
```

### Comparing `synthwave-0.1.4/README.md` & `synthwave-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `synthwave-0.1.4/synthwave/__main__.py` & `synthwave-0.1.5/synthwave/__main__.py`

 * *Files identical despite different names*

### Comparing `synthwave-0.1.4/synthwave/data.json` & `synthwave-0.1.5/synthwave/data.json`

 * *Files identical despite different names*

### Comparing `synthwave-0.1.4/synthwave/event.py` & `synthwave-0.1.5/synthwave/event.py`

 * *Files identical despite different names*

### Comparing `synthwave-0.1.4/synthwave/field.py` & `synthwave-0.1.5/synthwave/field.py`

 * *Files identical despite different names*

### Comparing `synthwave-0.1.4/PKG-INFO` & `synthwave-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: synthwave
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
+Home-page: https://mcleonard.github.com/synthwave
+License: MIT
 Author: Mat Leonard
 Author-email: leonard.mat@gmail.com
 Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
+Project-URL: Repository, https://github.com/mcleonard/synthwave
 Description-Content-Type: text/markdown
 
 # Synthwave: A Stream of Synthetic Events
 
 The goal here is to provide a stream of synthetic data similar to events you would see in a normal business. This can be used to generate data for testing, development, and for learning.
 
 The user defines the events they want emitted and this will write them to stdout, a file, or POST as JSON data to a URL (not tested yet).
```

