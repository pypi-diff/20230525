# Comparing `tmp/json_expand_o_matic-0.2.2.tar.gz` & `tmp/json_expand_o_matic-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_expand_o_matic-0.2.2.tar", last modified: Thu May 25 02:25:52 2023, max compression
+gzip compressed data, was "json_expand_o_matic-0.2.3.tar", last modified: Thu May 25 02:45:09 2023, max compression
```

## Comparing `json_expand_o_matic-0.2.2.tar` & `json_expand_o_matic-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:25:52.719956 json_expand_o_matic-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-25 02:25:52.719956 json_expand_o_matic-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-25 02:23:59.000000 json_expand_o_matic-0.2.2/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 02:23:52.000000 json_expand_o_matic-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 02:25:52.719956 json_expand_o_matic-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:25:52.711955 json_expand_o_matic-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:25:52.715956 json_expand_o_matic-0.2.2/src/json_expand_o_matic/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic/contractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic/expand_o_matic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic/expander.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic/expansion_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic/expansion_zipper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic/leaf_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:25:52.715956 json_expand_o_matic-0.2.2/src/json_expand_o_matic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-25 02:25:52.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-25 02:25:52.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 02:25:52.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 02:25:52.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 02:25:52.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:25:52.719956 json_expand_o_matic-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/tests/test_leaves.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:45:09.617488 json_expand_o_matic-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-25 02:45:09.617488 json_expand_o_matic-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-25 02:43:35.000000 json_expand_o_matic-0.2.3/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 02:43:21.000000 json_expand_o_matic-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 02:45:09.617488 json_expand_o_matic-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:45:09.613489 json_expand_o_matic-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:45:09.617488 json_expand_o_matic-0.2.3/src/json_expand_o_matic/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic/contractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic/expand_o_matic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic/expander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic/expansion_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic/expansion_zipper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic/leaf_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:45:09.617488 json_expand_o_matic-0.2.3/src/json_expand_o_matic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-25 02:45:09.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-25 02:45:09.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 02:45:09.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 02:45:09.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 02:45:09.000000 json_expand_o_matic-0.2.3/src/json_expand_o_matic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:45:09.617488 json_expand_o_matic-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/tests/test_leaves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 02:43:13.000000 json_expand_o_matic-0.2.3/version.txt
```

### Comparing `json_expand_o_matic-0.2.2/LICENSE.txt` & `json_expand_o_matic-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.2/PKG-INFO` & `json_expand_o_matic-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_expand_o_matic
-Version: 0.2.2
+Version: 0.2.3
 Summary: Expand a dict into a collection of subdirectories and json files or contract (un-expand) the output of expand() into a dict.
 Home-page: https://github.com/jcejohnson/JsonExpandOMatic
 Author: James Johnson
 Author-email: jcejohnson@users.noreply.github.com
 Keywords: json,jsonref
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `json_expand_o_matic-0.2.2/README.md` & `json_expand_o_matic-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.2/dev-requirements.txt` & `json_expand_o_matic-0.2.3/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.2/setup.py` & `json_expand_o_matic-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='json_expand_o_matic',
 
-    version='0.2.2',
+    version='0.2.3',
 
     description='Expand a dict into a collection of subdirectories and json files or '
                 'contract (un-expand) the output of expand() into a dict.',
 
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `json_expand_o_matic-0.2.2/src/json_expand_o_matic/__init__.py` & `json_expand_o_matic-0.2.3/src/json_expand_o_matic/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 
     See also: .jsonrefkeeper
 
 """
 
 from .expand_o_matic import JsonExpandOMatic
 
-VERSION = "v0.2.2"
+VERSION = "v0.2.3"
```

### Comparing `json_expand_o_matic-0.2.2/src/json_expand_o_matic/cli.py` & `json_expand_o_matic-0.2.3/src/json_expand_o_matic/cli.py`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.2/src/json_expand_o_matic/contractor.py` & `json_expand_o_matic-0.2.3/src/json_expand_o_matic/contractor.py`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.2/src/json_expand_o_matic/expand_o_matic.py` & `json_expand_o_matic-0.2.3/src/json_expand_o_matic/expand_o_matic.py`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.2/src/json_expand_o_matic/expander.py` & `json_expand_o_matic-0.2.3/src/json_expand_o_matic/expander.py`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.2/src/json_expand_o_matic/expansion_pool.py` & `json_expand_o_matic-0.2.3/src/json_expand_o_matic/expansion_pool.py`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.2/src/json_expand_o_matic/expansion_zipper.py` & `json_expand_o_matic-0.2.3/src/json_expand_o_matic/expansion_zipper.py`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.2/src/json_expand_o_matic/leaf_node.py` & `json_expand_o_matic-0.2.3/src/json_expand_o_matic/leaf_node.py`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.2/src/json_expand_o_matic.egg-info/PKG-INFO` & `json_expand_o_matic-0.2.3/src/json_expand_o_matic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-expand-o-matic
-Version: 0.2.2
+Version: 0.2.3
 Summary: Expand a dict into a collection of subdirectories and json files or contract (un-expand) the output of expand() into a dict.
 Home-page: https://github.com/jcejohnson/JsonExpandOMatic
 Author: James Johnson
 Author-email: jcejohnson@users.noreply.github.com
 Keywords: json,jsonref
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `json_expand_o_matic-0.2.2/src/json_expand_o_matic.egg-info/SOURCES.txt` & `json_expand_o_matic-0.2.3/src/json_expand_o_matic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.2/tests/test_leaves.py` & `json_expand_o_matic-0.2.3/tests/test_leaves.py`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.2/tests/test_simple.py` & `json_expand_o_matic-0.2.3/tests/test_simple.py`

 * *Files identical despite different names*

