# Comparing `tmp/interval-tools-0.9.0.tar.gz` & `tmp/interval-tools-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interval-tools-0.9.0.tar", last modified: Mon Dec 19 14:37:02 2022, max compression
+gzip compressed data, was "interval-tools-0.9.1.tar", last modified: Mon Dec 19 14:43:16 2022, max compression
```

## Comparing `interval-tools-0.9.0.tar` & `interval-tools-0.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 lvyao      (501) staff       (20)        0 2022-12-19 14:37:02.872680 interval-tools-0.9.0/
--rw-r--r--   0 lvyao      (501) staff       (20)     1072 2022-05-05 09:43:47.000000 interval-tools-0.9.0/LICENSE
--rw-r--r--   0 lvyao      (501) staff       (20)      867 2022-12-19 14:37:02.872765 interval-tools-0.9.0/PKG-INFO
--rw-r--r--   0 lvyao      (501) staff       (20)      355 2022-12-09 03:45:20.000000 interval-tools-0.9.0/README.md
--rw-r--r--   0 lvyao      (501) staff       (20)       81 2022-05-07 02:35:27.000000 interval-tools-0.9.0/pyproject.toml
--rw-r--r--   0 lvyao      (501) staff       (20)      652 2022-12-19 14:37:02.873021 interval-tools-0.9.0/setup.cfg
-drwxr-xr-x   0 lvyao      (501) staff       (20)        0 2022-12-19 14:37:02.868418 interval-tools-0.9.0/src/
-drwxr-xr-x   0 lvyao      (501) staff       (20)        0 2022-12-19 14:37:02.869222 interval-tools-0.9.0/src/interval/
--rw-r--r--   0 lvyao      (501) staff       (20)      224 2022-06-30 08:42:06.000000 interval-tools-0.9.0/src/interval/__init__.py
-drwxr-xr-x   0 lvyao      (501) staff       (20)        0 2022-12-19 14:37:02.871812 interval-tools-0.9.0/src/interval/ddd/
--rw-r--r--   0 lvyao      (501) staff       (20)      666 2022-12-19 13:06:39.000000 interval-tools-0.9.0/src/interval/ddd/__init__.py
--rw-r--r--   0 lvyao      (501) staff       (20)      286 2022-12-19 12:53:08.000000 interval-tools-0.9.0/src/interval/ddd/dto.py
--rw-r--r--   0 lvyao      (501) staff       (20)      976 2022-12-19 12:38:53.000000 interval-tools-0.9.0/src/interval/ddd/entity.py
--rw-r--r--   0 lvyao      (501) staff       (20)      657 2022-12-19 12:55:47.000000 interval-tools-0.9.0/src/interval/ddd/event.py
--rw-r--r--   0 lvyao      (501) staff       (20)     3214 2022-12-19 12:59:12.000000 interval-tools-0.9.0/src/interval/ddd/exceptions.py
--rw-r--r--   0 lvyao      (501) staff       (20)     2014 2022-12-19 12:39:36.000000 interval-tools-0.9.0/src/interval/ddd/serialization.py
--rw-r--r--   0 lvyao      (501) staff       (20)     2248 2022-12-19 12:39:10.000000 interval-tools-0.9.0/src/interval/ddd/valueobject.py
--rw-r--r--   0 lvyao      (501) staff       (20)     3534 2022-12-19 12:49:59.000000 interval-tools-0.9.0/src/interval/utils.py
-drwxr-xr-x   0 lvyao      (501) staff       (20)        0 2022-12-19 14:37:02.872571 interval-tools-0.9.0/src/interval_tools.egg-info/
--rw-r--r--   0 lvyao      (501) staff       (20)      867 2022-12-19 14:37:02.000000 interval-tools-0.9.0/src/interval_tools.egg-info/PKG-INFO
--rw-r--r--   0 lvyao      (501) staff       (20)      501 2022-12-19 14:37:02.000000 interval-tools-0.9.0/src/interval_tools.egg-info/SOURCES.txt
--rw-r--r--   0 lvyao      (501) staff       (20)        1 2022-12-19 14:37:02.000000 interval-tools-0.9.0/src/interval_tools.egg-info/dependency_links.txt
--rw-r--r--   0 lvyao      (501) staff       (20)       20 2022-12-19 14:37:02.000000 interval-tools-0.9.0/src/interval_tools.egg-info/requires.txt
--rw-r--r--   0 lvyao      (501) staff       (20)        9 2022-12-19 14:37:02.000000 interval-tools-0.9.0/src/interval_tools.egg-info/top_level.txt
+drwxr-xr-x   0 lvyao      (501) staff       (20)        0 2022-12-19 14:43:16.575836 interval-tools-0.9.1/
+-rw-r--r--   0 lvyao      (501) staff       (20)     1072 2022-05-05 09:43:47.000000 interval-tools-0.9.1/LICENSE
+-rw-r--r--   0 lvyao      (501) staff       (20)      867 2022-12-19 14:43:16.575895 interval-tools-0.9.1/PKG-INFO
+-rw-r--r--   0 lvyao      (501) staff       (20)      355 2022-12-09 03:45:20.000000 interval-tools-0.9.1/README.md
+-rw-r--r--   0 lvyao      (501) staff       (20)       81 2022-05-07 02:35:27.000000 interval-tools-0.9.1/pyproject.toml
+-rw-r--r--   0 lvyao      (501) staff       (20)      652 2022-12-19 14:43:16.576140 interval-tools-0.9.1/setup.cfg
+drwxr-xr-x   0 lvyao      (501) staff       (20)        0 2022-12-19 14:43:16.572080 interval-tools-0.9.1/src/
+drwxr-xr-x   0 lvyao      (501) staff       (20)        0 2022-12-19 14:43:16.572927 interval-tools-0.9.1/src/interval/
+-rw-r--r--   0 lvyao      (501) staff       (20)      224 2022-06-30 08:42:06.000000 interval-tools-0.9.1/src/interval/__init__.py
+drwxr-xr-x   0 lvyao      (501) staff       (20)        0 2022-12-19 14:43:16.574924 interval-tools-0.9.1/src/interval/ddd/
+-rw-r--r--   0 lvyao      (501) staff       (20)      667 2022-12-19 14:42:45.000000 interval-tools-0.9.1/src/interval/ddd/__init__.py
+-rw-r--r--   0 lvyao      (501) staff       (20)      286 2022-12-19 12:53:08.000000 interval-tools-0.9.1/src/interval/ddd/dto.py
+-rw-r--r--   0 lvyao      (501) staff       (20)      976 2022-12-19 12:38:53.000000 interval-tools-0.9.1/src/interval/ddd/entity.py
+-rw-r--r--   0 lvyao      (501) staff       (20)      657 2022-12-19 12:55:47.000000 interval-tools-0.9.1/src/interval/ddd/event.py
+-rw-r--r--   0 lvyao      (501) staff       (20)     3214 2022-12-19 12:59:12.000000 interval-tools-0.9.1/src/interval/ddd/exceptions.py
+-rw-r--r--   0 lvyao      (501) staff       (20)     2014 2022-12-19 12:39:36.000000 interval-tools-0.9.1/src/interval/ddd/serialization.py
+-rw-r--r--   0 lvyao      (501) staff       (20)     2248 2022-12-19 12:39:10.000000 interval-tools-0.9.1/src/interval/ddd/valueobject.py
+-rw-r--r--   0 lvyao      (501) staff       (20)     3534 2022-12-19 12:49:59.000000 interval-tools-0.9.1/src/interval/utils.py
+drwxr-xr-x   0 lvyao      (501) staff       (20)        0 2022-12-19 14:43:16.575719 interval-tools-0.9.1/src/interval_tools.egg-info/
+-rw-r--r--   0 lvyao      (501) staff       (20)      867 2022-12-19 14:43:16.000000 interval-tools-0.9.1/src/interval_tools.egg-info/PKG-INFO
+-rw-r--r--   0 lvyao      (501) staff       (20)      501 2022-12-19 14:43:16.000000 interval-tools-0.9.1/src/interval_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 lvyao      (501) staff       (20)        1 2022-12-19 14:43:16.000000 interval-tools-0.9.1/src/interval_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 lvyao      (501) staff       (20)       20 2022-12-19 14:43:16.000000 interval-tools-0.9.1/src/interval_tools.egg-info/requires.txt
+-rw-r--r--   0 lvyao      (501) staff       (20)        9 2022-12-19 14:43:16.000000 interval-tools-0.9.1/src/interval_tools.egg-info/top_level.txt
```

### Comparing `interval-tools-0.9.0/LICENSE` & `interval-tools-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `interval-tools-0.9.0/PKG-INFO` & `interval-tools-0.9.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interval-tools
-Version: 0.9.0
+Version: 0.9.1
 Summary: Utility functions and classes used in applications of Interval Design.
 Home-page: https://github.com/interval-design/python-tools
 Author: Interval Design
 Author-email: yao.lv@interval.im
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `interval-tools-0.9.0/setup.cfg` & `interval-tools-0.9.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = interval-tools
-version = 0.9.0
+version = 0.9.1
 author = Interval Design
 author_email = yao.lv@interval.im
 description = Utility functions and classes used in applications of Interval Design.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/interval-design/python-tools
 classifiers =
```

### Comparing `interval-tools-0.9.0/src/interval/ddd/__init__.py` & `interval-tools-0.9.1/src/interval/ddd/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,14 @@
     IntegrityError,
     InternalError,
     ProgrammingError,
     NotSupportedError,
     DBAPIErrorWrapper,
     STANDARD_DBAPI_ERRORS
 )
-from valueobject import (
+from .valueobject import (
     ValueObject,
     IntegerRef,
     StringRef,
     UUIDRef,
     OIDRef
 )
```

### Comparing `interval-tools-0.9.0/src/interval/ddd/entity.py` & `interval-tools-0.9.1/src/interval/ddd/entity.py`

 * *Files identical despite different names*

### Comparing `interval-tools-0.9.0/src/interval/ddd/event.py` & `interval-tools-0.9.1/src/interval/ddd/event.py`

 * *Files identical despite different names*

### Comparing `interval-tools-0.9.0/src/interval/ddd/exceptions.py` & `interval-tools-0.9.1/src/interval/ddd/exceptions.py`

 * *Files identical despite different names*

### Comparing `interval-tools-0.9.0/src/interval/ddd/serialization.py` & `interval-tools-0.9.1/src/interval/ddd/serialization.py`

 * *Files identical despite different names*

### Comparing `interval-tools-0.9.0/src/interval/ddd/valueobject.py` & `interval-tools-0.9.1/src/interval/ddd/valueobject.py`

 * *Files identical despite different names*

### Comparing `interval-tools-0.9.0/src/interval/utils.py` & `interval-tools-0.9.1/src/interval/utils.py`

 * *Files identical despite different names*

### Comparing `interval-tools-0.9.0/src/interval_tools.egg-info/PKG-INFO` & `interval-tools-0.9.1/src/interval_tools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interval-tools
-Version: 0.9.0
+Version: 0.9.1
 Summary: Utility functions and classes used in applications of Interval Design.
 Home-page: https://github.com/interval-design/python-tools
 Author: Interval Design
 Author-email: yao.lv@interval.im
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

