# Comparing `tmp/pysnc-1.1.5a0.tar.gz` & `tmp/pysnc-1.1.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysnc-1.1.5a0.tar", max compression
+gzip compressed data, was "pysnc-1.1.5a1.tar", max compression
```

## Comparing `pysnc-1.1.5a0.tar` & `pysnc-1.1.5a1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1052 2023-05-24 21:33:54.039764 pysnc-1.1.5a0/LICENSE
--rw-r--r--   0        0        0     1590 2023-05-24 21:33:54.039764 pysnc-1.1.5a0/README.md
--rw-r--r--   0        0        0     1058 2023-05-24 21:35:45.113412 pysnc-1.1.5a0/pyproject.toml
--rw-r--r--   0        0        0      129 2023-05-24 21:33:54.039764 pysnc-1.1.5a0/pysnc/__init__.py
--rw-r--r--   0        0        0       98 2023-05-24 21:33:54.039764 pysnc-1.1.5a0/pysnc/__version__.py
--rw-r--r--   0        0        0     9386 2023-05-24 21:33:54.039764 pysnc-1.1.5a0/pysnc/attachment.py
--rw-r--r--   0        0        0     3757 2023-05-24 21:33:54.039764 pysnc-1.1.5a0/pysnc/auth.py
--rw-r--r--   0        0        0    15673 2023-05-24 21:33:54.039764 pysnc-1.1.5a0/pysnc/client.py
--rw-r--r--   0        0        0     1002 2023-05-24 21:33:54.043763 pysnc-1.1.5a0/pysnc/exceptions.py
--rw-r--r--   0        0        0     3867 2023-05-24 21:33:54.043763 pysnc-1.1.5a0/pysnc/query.py
--rw-r--r--   0        0        0    38858 2023-05-24 21:33:54.043763 pysnc-1.1.5a0/pysnc/record.py
--rw-r--r--   0        0        0      846 2023-05-24 21:33:54.043763 pysnc-1.1.5a0/pysnc/utils.py
--rw-r--r--   0        0        0     2618 1970-01-01 00:00:00.000000 pysnc-1.1.5a0/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-05-24 22:01:02.490748 pysnc-1.1.5a1/LICENSE
+-rw-r--r--   0        0        0     1590 2023-05-24 22:01:02.490748 pysnc-1.1.5a1/README.md
+-rw-r--r--   0        0        0     1058 2023-05-24 22:01:27.514738 pysnc-1.1.5a1/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-05-24 22:01:02.494748 pysnc-1.1.5a1/pysnc/__init__.py
+-rw-r--r--   0        0        0       98 2023-05-24 22:01:02.494748 pysnc-1.1.5a1/pysnc/__version__.py
+-rw-r--r--   0        0        0     9386 2023-05-24 22:01:02.494748 pysnc-1.1.5a1/pysnc/attachment.py
+-rw-r--r--   0        0        0     3757 2023-05-24 22:01:02.494748 pysnc-1.1.5a1/pysnc/auth.py
+-rw-r--r--   0        0        0    15673 2023-05-24 22:01:02.494748 pysnc-1.1.5a1/pysnc/client.py
+-rw-r--r--   0        0        0     1002 2023-05-24 22:01:02.494748 pysnc-1.1.5a1/pysnc/exceptions.py
+-rw-r--r--   0        0        0     3867 2023-05-24 22:01:02.494748 pysnc-1.1.5a1/pysnc/query.py
+-rw-r--r--   0        0        0    38858 2023-05-24 22:01:02.494748 pysnc-1.1.5a1/pysnc/record.py
+-rw-r--r--   0        0        0      846 2023-05-24 22:01:02.494748 pysnc-1.1.5a1/pysnc/utils.py
+-rw-r--r--   0        0        0     2618 1970-01-01 00:00:00.000000 pysnc-1.1.5a1/PKG-INFO
```

### Comparing `pysnc-1.1.5a0/LICENSE` & `pysnc-1.1.5a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.5a0/README.md` & `pysnc-1.1.5a1/README.md`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.5a0/pyproject.toml` & `pysnc-1.1.5a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysnc"
-version = "1.1.5a0"
+version = "1.1.5a1"
 description = "Python SNC (REST) API"
 authors = ["Matthew Gill <matthew.gill@servicenow.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ServiceNow/PySNC"
 documentation = "https://servicenow.github.io/PySNC/"
 keywords = ["servicenow", "snc"]
```

### Comparing `pysnc-1.1.5a0/pysnc/attachment.py` & `pysnc-1.1.5a1/pysnc/attachment.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.5a0/pysnc/auth.py` & `pysnc-1.1.5a1/pysnc/auth.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.5a0/pysnc/client.py` & `pysnc-1.1.5a1/pysnc/client.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.5a0/pysnc/exceptions.py` & `pysnc-1.1.5a1/pysnc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.5a0/pysnc/query.py` & `pysnc-1.1.5a1/pysnc/query.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.5a0/pysnc/record.py` & `pysnc-1.1.5a1/pysnc/record.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.5a0/pysnc/utils.py` & `pysnc-1.1.5a1/pysnc/utils.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.5a0/PKG-INFO` & `pysnc-1.1.5a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysnc
-Version: 1.1.5a0
+Version: 1.1.5a1
 Summary: Python SNC (REST) API
 Home-page: https://github.com/ServiceNow/PySNC
 License: MIT
 Keywords: servicenow,snc
 Author: Matthew Gill
 Author-email: matthew.gill@servicenow.com
 Requires-Python: >=3.8,<4.0
```

