# Comparing `tmp/synthwave-0.1.5.tar.gz` & `tmp/synthwave-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthwave-0.1.5.tar", max compression
+gzip compressed data, was "synthwave-0.1.6.tar", max compression
```

## Comparing `synthwave-0.1.5.tar` & `synthwave-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     2293 2023-05-25 18:36:33.052986 synthwave-0.1.5/README.md
--rw-r--r--   0        0        0      563 2023-05-25 18:54:36.661696 synthwave-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      473 2023-05-25 17:08:52.810976 synthwave-0.1.5/synthwave/__init__.py
--rw-r--r--   0        0        0     1543 2023-05-25 18:24:16.834867 synthwave-0.1.5/synthwave/__main__.py
--rw-r--r--   0        0        0    42590 2023-05-25 16:49:53.959907 synthwave-0.1.5/synthwave/data.json
--rw-r--r--   0        0        0      729 2023-05-24 22:11:59.931095 synthwave-0.1.5/synthwave/event.py
--rw-r--r--   0        0        0     6613 2023-05-25 18:03:51.971616 synthwave-0.1.5/synthwave/field.py
--rw-r--r--   0        0        0      342 2023-05-25 18:11:48.622143 synthwave-0.1.5/synthwave/stream.py
--rw-r--r--   0        0        0      160 2023-05-24 21:50:00.797905 synthwave-0.1.5/synthwave/utils.py
--rw-r--r--   0        0        0     2847 1970-01-01 00:00:00.000000 synthwave-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-05-25 19:07:16.687062 synthwave-0.1.6/LICENSE.md
+-rw-r--r--   0        0        0     2293 2023-05-25 18:36:33.052986 synthwave-0.1.6/README.md
+-rw-r--r--   0        0        0      587 2023-05-25 19:09:39.083066 synthwave-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      473 2023-05-25 17:08:52.810976 synthwave-0.1.6/synthwave/__init__.py
+-rw-r--r--   0        0        0     1543 2023-05-25 18:24:16.834867 synthwave-0.1.6/synthwave/__main__.py
+-rw-r--r--   0        0        0    42590 2023-05-25 16:49:53.959907 synthwave-0.1.6/synthwave/data.json
+-rw-r--r--   0        0        0      729 2023-05-24 22:11:59.931095 synthwave-0.1.6/synthwave/event.py
+-rw-r--r--   0        0        0     6613 2023-05-25 18:03:51.971616 synthwave-0.1.6/synthwave/field.py
+-rw-r--r--   0        0        0      342 2023-05-25 18:11:48.622143 synthwave-0.1.6/synthwave/stream.py
+-rw-r--r--   0        0        0      160 2023-05-24 21:50:00.797905 synthwave-0.1.6/synthwave/utils.py
+-rw-r--r--   0        0        0     2869 1970-01-01 00:00:00.000000 synthwave-0.1.6/PKG-INFO
```

### Comparing `synthwave-0.1.5/README.md` & `synthwave-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `synthwave-0.1.5/pyproject.toml` & `synthwave-0.1.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "synthwave"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Mat Leonard <leonard.mat@gmail.com>"]
 readme = "README.md"
-license = "MIT"
-homepage = "https://mcleonard.github.com/synthwave"
+license = "BSD 3-Clause"
+homepage = "https://mcleonard.github.io/synthwave/html/index.html"
 repository = "https://github.com/mcleonard/synthwave"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 requests = "^2.31.0"
 validators = "^0.20.0"
```

### Comparing `synthwave-0.1.5/synthwave/__main__.py` & `synthwave-0.1.6/synthwave/__main__.py`

 * *Files identical despite different names*

### Comparing `synthwave-0.1.5/synthwave/data.json` & `synthwave-0.1.6/synthwave/data.json`

 * *Files identical despite different names*

### Comparing `synthwave-0.1.5/synthwave/event.py` & `synthwave-0.1.6/synthwave/event.py`

 * *Files identical despite different names*

### Comparing `synthwave-0.1.5/synthwave/field.py` & `synthwave-0.1.6/synthwave/field.py`

 * *Files identical despite different names*

### Comparing `synthwave-0.1.5/PKG-INFO` & `synthwave-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: synthwave
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
-Home-page: https://mcleonard.github.com/synthwave
-License: MIT
+Home-page: https://mcleonard.github.io/synthwave/html/index.html
+License: BSD 3-Clause
 Author: Mat Leonard
 Author-email: leonard.mat@gmail.com
 Requires-Python: >=3.11,<4.0
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Project-URL: Repository, https://github.com/mcleonard/synthwave
 Description-Content-Type: text/markdown
```

