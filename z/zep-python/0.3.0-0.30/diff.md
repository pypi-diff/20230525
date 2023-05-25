# Comparing `tmp/zep_python-0.3.0.tar.gz` & `tmp/zep_python-0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zep_python-0.3.0.tar", max compression
+gzip compressed data, was "zep_python-0.30.tar", max compression
```

## Comparing `zep_python-0.3.0.tar` & `zep_python-0.30.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-05-25 18:21:47.636865 zep_python-0.3.0/LICENSE
--rw-r--r--   0        0        0     2393 2023-05-25 18:21:47.636865 zep_python-0.3.0/README.md
--rw-r--r--   0        0        0      873 2023-05-25 18:21:47.640865 zep_python-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      340 2023-05-25 18:21:47.640865 zep_python-0.3.0/zep_python/__init__.py
--rw-r--r--   0        0        0     1236 2023-05-25 18:21:47.640865 zep_python-0.3.0/zep_python/exceptions.py
--rw-r--r--   0        0        0     4956 2023-05-25 18:21:47.640865 zep_python-0.3.0/zep_python/models.py
--rw-r--r--   0        0        0        0 2023-05-25 18:21:47.640865 zep_python-0.3.0/zep_python/py.typed
--rw-r--r--   0        0        0    13465 2023-05-25 18:21:47.640865 zep_python-0.3.0/zep_python/zep_client.py
--rw-r--r--   0        0        0     3073 1970-01-01 00:00:00.000000 zep_python-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-25 18:34:22.817551 zep_python-0.30/LICENSE
+-rw-r--r--   0        0        0     2393 2023-05-25 18:34:22.817551 zep_python-0.30/README.md
+-rw-r--r--   0        0        0      872 2023-05-25 18:34:22.821551 zep_python-0.30/pyproject.toml
+-rw-r--r--   0        0        0      340 2023-05-25 18:34:22.821551 zep_python-0.30/zep_python/__init__.py
+-rw-r--r--   0        0        0     1236 2023-05-25 18:34:22.821551 zep_python-0.30/zep_python/exceptions.py
+-rw-r--r--   0        0        0     4956 2023-05-25 18:34:22.821551 zep_python-0.30/zep_python/models.py
+-rw-r--r--   0        0        0        0 2023-05-25 18:34:22.821551 zep_python-0.30/zep_python/py.typed
+-rw-r--r--   0        0        0    13465 2023-05-25 18:34:22.821551 zep_python-0.30/zep_python/zep_client.py
+-rw-r--r--   0        0        0     3072 1970-01-01 00:00:00.000000 zep_python-0.30/PKG-INFO
```

### Comparing `zep_python-0.3.0/LICENSE` & `zep_python-0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `zep_python-0.3.0/README.md` & `zep_python-0.30/README.md`

 * *Files identical despite different names*

### Comparing `zep_python-0.3.0/pyproject.toml` & `zep_python-0.30/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zep-python"
-version = "0.3.0"
+version = "0.30"
 description = "Zep stores, manages, enriches, indexes, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service."
 authors = ["Daniel Chalef <daniel.chalef@private.org>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = "^0.24.0"
```

### Comparing `zep_python-0.3.0/zep_python/exceptions.py` & `zep_python-0.30/zep_python/exceptions.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.3.0/zep_python/models.py` & `zep_python-0.30/zep_python/models.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.3.0/zep_python/zep_client.py` & `zep_python-0.30/zep_python/zep_client.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.3.0/PKG-INFO` & `zep_python-0.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zep-python
-Version: 0.3.0
+Version: 0.30
 Summary: Zep stores, manages, enriches, indexes, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service.
 Author: Daniel Chalef
 Author-email: daniel.chalef@private.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

