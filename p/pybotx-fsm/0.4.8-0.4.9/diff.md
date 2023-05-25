# Comparing `tmp/pybotx_fsm-0.4.8.tar.gz` & `tmp/pybotx_fsm-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybotx_fsm-0.4.8.tar", max compression
+gzip compressed data, was "pybotx_fsm-0.4.9.tar", max compression
```

## Comparing `pybotx_fsm-0.4.8.tar` & `pybotx_fsm-0.4.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     6078 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/LICENSE.md
--rw-r--r--   0        0        0     5614 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/README.md
--rw-r--r--   0        0        0      192 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/pybotx_fsm/__init__.py
--rw-r--r--   0        0        0     1147 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/pybotx_fsm/collector.py
--rw-r--r--   0        0        0     1711 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/pybotx_fsm/fsm.py
--rw-r--r--   0        0        0     2211 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/pybotx_fsm/middleware.py
--rw-r--r--   0        0        0        0 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/pybotx_fsm/py.typed
--rw-r--r--   0        0        0      451 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/pybotx_fsm/state_repo_proto.py
--rw-r--r--   0        0        0      122 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/pybotx_fsm/templates.py
--rw-r--r--   0        0        0      549 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     6025 1970-01-01 00:00:00.000000 pybotx_fsm-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     6078 2023-05-25 10:03:19.638737 pybotx_fsm-0.4.9/LICENSE.md
+-rw-r--r--   0        0        0     5614 2023-05-25 10:03:19.638737 pybotx_fsm-0.4.9/README.md
+-rw-r--r--   0        0        0      192 2023-05-25 10:03:19.642737 pybotx_fsm-0.4.9/pybotx_fsm/__init__.py
+-rw-r--r--   0        0        0     1147 2023-05-25 10:03:19.642737 pybotx_fsm-0.4.9/pybotx_fsm/collector.py
+-rw-r--r--   0        0        0     1711 2023-05-25 10:03:19.642737 pybotx_fsm-0.4.9/pybotx_fsm/fsm.py
+-rw-r--r--   0        0        0     2211 2023-05-25 10:03:19.642737 pybotx_fsm-0.4.9/pybotx_fsm/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-25 10:03:19.642737 pybotx_fsm-0.4.9/pybotx_fsm/py.typed
+-rw-r--r--   0        0        0      451 2023-05-25 10:03:19.642737 pybotx_fsm-0.4.9/pybotx_fsm/state_repo_proto.py
+-rw-r--r--   0        0        0      122 2023-05-25 10:03:19.642737 pybotx_fsm-0.4.9/pybotx_fsm/templates.py
+-rw-r--r--   0        0        0      549 2023-05-25 10:03:19.642737 pybotx_fsm-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     6076 1970-01-01 00:00:00.000000 pybotx_fsm-0.4.9/PKG-INFO
```

### Comparing `pybotx_fsm-0.4.8/LICENSE.md` & `pybotx_fsm-0.4.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pybotx_fsm-0.4.8/README.md` & `pybotx_fsm-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `pybotx_fsm-0.4.8/pybotx_fsm/collector.py` & `pybotx_fsm-0.4.9/pybotx_fsm/collector.py`

 * *Files identical despite different names*

### Comparing `pybotx_fsm-0.4.8/pybotx_fsm/fsm.py` & `pybotx_fsm-0.4.9/pybotx_fsm/fsm.py`

 * *Files identical despite different names*

### Comparing `pybotx_fsm-0.4.8/pybotx_fsm/middleware.py` & `pybotx_fsm-0.4.9/pybotx_fsm/middleware.py`

 * *Files identical despite different names*

### Comparing `pybotx_fsm-0.4.8/pyproject.toml` & `pybotx_fsm-0.4.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # https://python-poetry.org/docs/
 
 [tool.poetry]
 name = "pybotx-fsm"
-version = "0.4.8"
+version = "0.4.9"
 description = "FSM middleware for using with pybotx"
 readme = "README.md"
 authors = []
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<3.12"
 
 pybotx = ">=0.44.1,<0.56.0"
 
 [tool.poetry.dev-dependencies]
 add-trailing-comma = "2.2.3"
 autoflake = "1.4.0"
 black = "22.3.0"
```

### Comparing `pybotx_fsm-0.4.8/PKG-INFO` & `pybotx_fsm-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pybotx-fsm
-Version: 0.4.8
+Version: 0.4.9
 Summary: FSM middleware for using with pybotx
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pybotx (>=0.44.1,<0.56.0)
 Description-Content-Type: text/markdown
 
 # pybotx-fsm
 
 [![codecov](https://codecov.io/gh/ExpressApp/pybotx-fsm/branch/master/graph/badge.svg?token=JWT9JWU2Z4)](https://codecov.io/gh/ExpressApp/pybotx-fsm)
```

