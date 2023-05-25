# Comparing `tmp/json_expand_o_matic-0.2.0.tar.gz` & `tmp/json_expand_o_matic-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_expand_o_matic-0.2.0.tar", last modified: Sun Mar  5 20:21:38 2023, max compression
+gzip compressed data, was "json_expand_o_matic-0.2.1.tar", last modified: Thu May 25 02:14:13 2023, max compression
```

## Comparing `json_expand_o_matic-0.2.0.tar` & `json_expand_o_matic-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 20:21:38.479142 json_expand_o_matic-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-05 20:20:13.000000 json_expand_o_matic-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-05 20:20:13.000000 json_expand_o_matic-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-03-05 20:21:38.479142 json_expand_o_matic-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-03-05 20:20:13.000000 json_expand_o_matic-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-03-05 20:20:26.000000 json_expand_o_matic-0.2.0/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-05 20:20:13.000000 json_expand_o_matic-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-05 20:20:21.000000 json_expand_o_matic-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-05 20:21:38.479142 json_expand_o_matic-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-03-05 20:20:13.000000 json_expand_o_matic-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 20:21:38.475142 json_expand_o_matic-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 20:21:38.479142 json_expand_o_matic-0.2.0/src/json_expand_o_matic/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-05 20:20:13.000000 json_expand_o_matic-0.2.0/src/json_expand_o_matic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-03-05 20:20:13.000000 json_expand_o_matic-0.2.0/src/json_expand_o_matic/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-05 20:20:13.000000 json_expand_o_matic-0.2.0/src/json_expand_o_matic/contractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-03-05 20:20:13.000000 json_expand_o_matic-0.2.0/src/json_expand_o_matic/expand_o_matic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-03-05 20:20:13.000000 json_expand_o_matic-0.2.0/src/json_expand_o_matic/expander.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-03-05 20:20:13.000000 json_expand_o_matic-0.2.0/src/json_expand_o_matic/leaf_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 20:21:38.479142 json_expand_o_matic-0.2.0/src/json_expand_o_matic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-03-05 20:21:38.000000 json_expand_o_matic-0.2.0/src/json_expand_o_matic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-05 20:21:38.000000 json_expand_o_matic-0.2.0/src/json_expand_o_matic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 20:21:38.000000 json_expand_o_matic-0.2.0/src/json_expand_o_matic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-05 20:21:38.000000 json_expand_o_matic-0.2.0/src/json_expand_o_matic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-05 20:21:38.000000 json_expand_o_matic-0.2.0/src/json_expand_o_matic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 20:21:38.479142 json_expand_o_matic-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 20:20:13.000000 json_expand_o_matic-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-03-05 20:20:13.000000 json_expand_o_matic-0.2.0/tests/test_leaves.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-03-05 20:20:13.000000 json_expand_o_matic-0.2.0/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-05 20:20:13.000000 json_expand_o_matic-0.2.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:14:13.908851 json_expand_o_matic-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-25 02:14:13.908851 json_expand_o_matic-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-25 02:12:26.000000 json_expand_o_matic-0.2.1/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 02:12:16.000000 json_expand_o_matic-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 02:14:13.908851 json_expand_o_matic-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:14:13.900850 json_expand_o_matic-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:14:13.904850 json_expand_o_matic-0.2.1/src/json_expand_o_matic/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic/contractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic/expand_o_matic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic/expander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic/expansion_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic/leaf_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:14:13.908851 json_expand_o_matic-0.2.1/src/json_expand_o_matic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-25 02:14:13.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-25 02:14:13.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 02:14:13.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 02:14:13.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 02:14:13.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:14:13.908851 json_expand_o_matic-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/tests/test_leaves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/version.txt
```

### Comparing `json_expand_o_matic-0.2.0/LICENSE.txt` & `json_expand_o_matic-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.0/PKG-INFO` & `json_expand_o_matic-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_expand_o_matic
-Version: 0.2.0
+Version: 0.2.1
 Summary: Expand a dict into a collection of subdirectories and json files or contract (un-expand) the output of expand() into a dict.
 Home-page: https://github.com/jcejohnson/JsonExpandOMatic
 Author: James Johnson
 Author-email: jcejohnson@users.noreply.github.com
 Keywords: json,jsonref
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `json_expand_o_matic-0.2.0/README.md` & `json_expand_o_matic-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.0/dev-requirements.txt` & `json_expand_o_matic-0.2.1/dev-requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,42 +10,30 @@
     # via pytest
 babel==2.12.1
     # via sphinx
 black==23.1.0
     # via -r dev-requirements.in
 bump2version==1.0.1
     # via -r dev-requirements.in
-cachetools==5.3.0
-    # via tox
 certifi==2022.12.7
     # via requests
-chardet==5.1.0
-    # via tox
 charset-normalizer==3.0.1
     # via requests
 click==8.1.3
     # via black
 colorama==0.4.6
-    # via
-    #   pytest-resource-path
-    #   tox
+    # via pytest-resource-path
 coloredlogs==15.0.1
     # via -r dev-requirements.in
 coverage[toml]==7.2.1
     # via pytest-cov
-distlib==0.3.6
-    # via virtualenv
 docutils==0.19
     # via sphinx
 exceptiongroup==1.1.0
     # via pytest
-filelock==3.9.0
-    # via
-    #   tox
-    #   virtualenv
 flake8==6.0.0
     # via
     #   -r dev-requirements.in
     #   pep8-naming
 humanfriendly==10.0
     # via coloredlogs
 idna==3.4
@@ -71,39 +59,30 @@
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
 packaging==23.0
     # via
     #   black
-    #   pyproject-api
     #   pytest
     #   sphinx
-    #   tox
 pathspec==0.11.0
     # via black
 pep8-naming==0.13.3
     # via -r dev-requirements.in
 platformdirs==3.1.0
-    # via
-    #   black
-    #   tox
-    #   virtualenv
+    # via black
 pluggy==1.0.0
-    # via
-    #   pytest
-    #   tox
+    # via pytest
 pycodestyle==2.10.0
     # via flake8
 pyflakes==3.0.1
     # via flake8
 pygments==2.14.0
     # via sphinx
-pyproject-api==1.5.0
-    # via tox
 pytest==7.2.2
     # via
     #   -r dev-requirements.in
     #   pytest-cov
     #   pytest-resource-path
 pytest-cov==4.0.0
     # via -r dev-requirements.in
@@ -128,22 +107,16 @@
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
 tomli==2.0.1
     # via
     #   black
     #   coverage
     #   mypy
-    #   pyproject-api
     #   pytest
-    #   tox
-tox==4.4.6
-    # via -r dev-requirements.in
 typing-extensions==4.5.0
     # via
     #   black
     #   mypy
 urllib3==1.26.14
     # via requests
-virtualenv==20.20.0
-    # via tox
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `json_expand_o_matic-0.2.0/setup.py` & `json_expand_o_matic-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='json_expand_o_matic',
 
-    version='0.2.0',
+    version='0.2.1',
 
     description='Expand a dict into a collection of subdirectories and json files or '
                 'contract (un-expand) the output of expand() into a dict.',
 
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `json_expand_o_matic-0.2.0/src/json_expand_o_matic/__init__.py` & `json_expand_o_matic-0.2.1/src/json_expand_o_matic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 
     See also: .jsonrefkeeper
 
 """
 
 from .expand_o_matic import JsonExpandOMatic
 
-VERSION = "v0.2.0"
+VERSION = "v0.2.1"
```

### Comparing `json_expand_o_matic-0.2.0/src/json_expand_o_matic/cli.py` & `json_expand_o_matic-0.2.1/src/json_expand_o_matic/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import logging
+import os
 import sys
 
 from . import VERSION, JsonExpandOMatic
 
 # NOTE: This isn't meant to be a fully functional cli.
 #       Mostly because I don't want to impose a dependency (click) on you.
 #       It is simply here as a quick way to interact with the library.
@@ -59,15 +60,17 @@
     from .expander import Expander
 
     JsonExpandOMatic(logger=logger, path=output_path).expand(
         data=json.load(open(input_file)),
         root_element="root",
         preserve=False,
         leaf_nodes=leaf_nodes,
-        hash_mode=Expander.HASH_MD5
+        hash_mode=Expander.HASH_MD5,
+        pool_size=int(os.environ.get("JEOM_POOL_SIZE") or 1),
+        pool_ratio=float(os.environ.get("JEOM_POOL_RATIO") or 1),
         # leaf_nodes=["/.*"]
         # leaf_nodes=["/root/actors/.*/movies/.*"]
         # leaf_nodes=[{"/root/actors/.*": ["/[^/]+/movies/.*"]}]
         # # This may be working...
         # leaf_nodes=[
         #     {
         #         ">B:/root/actors/[^/]+$": [
```

### Comparing `json_expand_o_matic-0.2.0/src/json_expand_o_matic/contractor.py` & `json_expand_o_matic-0.2.1/src/json_expand_o_matic/contractor.py`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.0/src/json_expand_o_matic/expand_o_matic.py` & `json_expand_o_matic-0.2.1/src/json_expand_o_matic/expand_o_matic.py`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.0/src/json_expand_o_matic/expander.py` & `json_expand_o_matic-0.2.1/src/json_expand_o_matic/expander.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import collections
 import hashlib
 import json
 import os
 
+from .expansion_pool import ExpansionPool
 from .leaf_node import LeafNode
 
 
 class Expander:
     """Expand a dict or list into one or more json files."""
 
     HASH_MD5 = "HASH_MD5"
@@ -15,36 +16,52 @@
         assert isinstance(data, dict) or isinstance(data, list)
 
         self.logger = logger
         self.path = path
         self.data = data
         self.leaf_nodes = leaf_nodes
 
-        self.ref_key = options.get("ref_key", "$ref")
+        self.work = None
 
-        self.hash_mode = options.get("hash_mode", None)
+        self.options = options if options is not None else dict()
+        self.pool_options = {
+            key: self.options.pop(key) for key in {key for key in self.options.keys() if key.startswith("pool_")}
+        }
+
+        self.ref_key = self.options.get("ref_key", "$ref")
+
+        self.json_dump_kwargs = self.options.get(
+            "json_dump_kwargs", {"indent": "", "sort_keys": False, "separators": (",", ":")}
+        )
+
+        self.hash_mode = self.options.get("hash_mode", None)
         if self.hash_mode == Expander.HASH_MD5:
             self._hash_function = self._hash_md5
         else:
-            self._hash_function = lambda *args, **kwargs: False
+            self._hash_function = lambda *args, **kwargs: (None, None)
 
         # Map hashcodes of dict objects to the json files they are saved as.
         #   key   -- hashcode as specified by self.hash_mode
         #   value -- list of files w/ hashcode
         # We can use these in a 2nd pass to create $refs to identical objects.
         self.hashcodes = collections.defaultdict(lambda: list())
 
     def execute(self):
         """Expand self.data into one or more json files."""
 
         # Replace the _dump() method with a no-op for the root of the data.
         self._dump = lambda *args: None
 
+        pool = ExpansionPool(logger=self.logger, **self.pool_options)
+        self.work = pool.work
+
         expansion = self._execute(indent=0, my_path_component=os.path.basename(self.path), traversal="")
 
+        pool.drain()
+
         self._hashcodes_cleanup()
 
         return expansion
 
     def _execute(self, traversal, indent, my_path_component):
         """Main...
 
@@ -109,31 +126,33 @@
 
         Always returns True so that _is_leaf_node() is less gross.
         """
 
         if leaf_node and not leaf_node.WHAT == LeafNode.What.DUMP:
             return True
 
-        directory = os.path.dirname(self.path)
-        filename = f"{self.path}.json"
+        dumps = json.dumps(self.data, **self.json_dump_kwargs)
 
-        # Use tabs for indents.
-        # This will save a surprising amount of space in large files.
-        dumps = json.dumps(self.data, indent="\t", sort_keys=True)
+        directory = os.path.dirname(self.path)
+        filename = os.path.basename(self.path)
+        data_file = f"{filename}.json"
 
-        self._json_save(directory, filename, dumps)
+        checksum, checksumfile_suffix = self._hash_function(dumps)
+        checksum_file = f"{filename}.{checksumfile_suffix}"
 
-        checksum = self._hash_function(dumps)
         if checksum:
-            self.hashcodes[checksum].append(filename)
+            self.work.append((directory, data_file, dumps, checksum_file, checksum))
+            self.hashcodes[checksum].append(data_file)
+        else:
+            self.work.append((directory, data_file, dumps, None, None))
 
         # Build a reference to the file we just wrote.
         directory = os.path.basename(directory)
-        filename = os.path.basename(filename)
-        self.data = {self.ref_key: f"{directory}/{filename}"}
+        data_file = os.path.basename(data_file)
+        self.data = {self.ref_key: f"{directory}/{data_file}"}
 
         return True
 
     def _hashcodes_cleanup(self):
         """Strip self.path from the hashcodes' files in case we want to make $refs from them.
         Also removes any entries having less than two files.
         """
@@ -141,68 +160,62 @@
         self.hashcodes = {k: [f[l:] for f in v] for k, v in self.hashcodes.items() if len(v) > 1}
 
     def _hash_md5(self, dumps):
         """Compute and save the md5 hashcode of `dumps`.
         Returns checksum.
         """
         checksum = hashlib.md5(dumps.encode()).hexdigest()
-        filename = f"{self.path}.md5"
-        with open(filename, "w") as f:
-            f.write(checksum)
-        return checksum
+        return checksum, "md5"
 
     def _is_leaf_node(self, when):
         for c in self.leaf_nodes:
             if c.comment or not c.match(string=self.traversal, when=when):
                 continue
 
             if not c.children:
                 return self._dump(c)
 
             self._log(f">>> Expand children of [{c.raw}]")
-            Expander(
-                logger=self.logger,
+            self._recursion_instance(
                 path=os.path.dirname(self.path),
                 data={os.path.basename(self.path): self.data},
                 leaf_nodes=c.children,
             )._execute(indent=self.indent + 2, my_path_component=os.path.basename(self.path), traversal="")
             self._log(f"<<< Expand children of [{c.raw}]")
 
             return self._dump(c)
 
         return False
 
-    def _json_save(self, directory, filename, dumps):
-        try:
-            # Assume that the path will already exist.
-            # We'll take a hit on the first file in each new path but save the overhead
-            # of checking on each subsequent one. This assumes that most objects will
-            # have multiple nested objects.
-            with open(filename, "w") as f:
-                f.write(dumps)
-        except FileNotFoundError:
-            os.makedirs(directory)
-            with open(filename, "w") as f:
-                f.write(dumps)
-
     def _log(self, string):
         self.logger.debug(" " * self.indent + string)
 
+    def _recursion_instance(self, *, path, data, leaf_nodes):
+        instance = Expander(
+            logger=self.logger,
+            #
+            data=data,
+            leaf_nodes=leaf_nodes,
+            path=path,
+            #
+            **self.options,
+        )
+        instance.work = self.work
+        return instance
+
     def _recursively_expand(self, *, key):
         if not (isinstance(self.data[key], dict) or isinstance(self.data[key], list)):
             return
 
         path_component = str(key).replace(":", "_").replace("/", "_").replace("\\", "_").replace(" ", "_")
 
-        expander = Expander(
-            logger=self.logger,
+        expander = self._recursion_instance(
             path=os.path.join(self.path, path_component),
             data=self.data[key],
             leaf_nodes=self.leaf_nodes,
-            hash_mode=self.hash_mode,
         )
         self.data[key] = expander._execute(
             indent=self.indent + 2, my_path_component=path_component, traversal=f"{self.traversal}/{key}"
         )
 
         # Add the child's hashcodes to our own so that when we unroll the recursion the root
         # will not need to recurse again to collect the entire list.
```

### Comparing `json_expand_o_matic-0.2.0/src/json_expand_o_matic/leaf_node.py` & `json_expand_o_matic-0.2.1/src/json_expand_o_matic/leaf_node.py`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.0/src/json_expand_o_matic.egg-info/PKG-INFO` & `json_expand_o_matic-0.2.1/src/json_expand_o_matic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-expand-o-matic
-Version: 0.2.0
+Version: 0.2.1
 Summary: Expand a dict into a collection of subdirectories and json files or contract (un-expand) the output of expand() into a dict.
 Home-page: https://github.com/jcejohnson/JsonExpandOMatic
 Author: James Johnson
 Author-email: jcejohnson@users.noreply.github.com
 Keywords: json,jsonref
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `json_expand_o_matic-0.2.0/src/json_expand_o_matic.egg-info/SOURCES.txt` & `json_expand_o_matic-0.2.1/src/json_expand_o_matic.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 setup.py
 version.txt
 src/json_expand_o_matic/__init__.py
 src/json_expand_o_matic/cli.py
 src/json_expand_o_matic/contractor.py
 src/json_expand_o_matic/expand_o_matic.py
 src/json_expand_o_matic/expander.py
+src/json_expand_o_matic/expansion_pool.py
 src/json_expand_o_matic/leaf_node.py
 src/json_expand_o_matic.egg-info/PKG-INFO
 src/json_expand_o_matic.egg-info/SOURCES.txt
 src/json_expand_o_matic.egg-info/dependency_links.txt
 src/json_expand_o_matic.egg-info/entry_points.txt
 src/json_expand_o_matic.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `json_expand_o_matic-0.2.0/tests/test_leaves.py` & `json_expand_o_matic-0.2.1/tests/test_leaves.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 class TestLeaves:
     """Test `leaf_node` functionality."""
 
     # Our raw test data.
     _raw_data = None
 
+    @pytest.fixture(params=[False, True])
+    def threaded(self, request):
+        return request.param
+
     @pytest.fixture
     def raw_data(self, resource_path_root):
         if not TestLeaves._raw_data:
             TestLeaves._raw_data = json.loads((resource_path_root / "actor-data.json").read_text())
         return TestLeaves._raw_data
 
     # Fixtures to provide copies of the raw data to each test function.
@@ -24,43 +28,45 @@
     def test_data(self, raw_data):
         return json.loads(json.dumps(raw_data))
 
     @pytest.fixture
     def original_data(self, raw_data):
         return json.loads(json.dumps(raw_data))
 
-    def test_actors1(self, tmpdir, test_data, original_data):
+    def test_actors1(self, tmpdir, test_data, original_data, threaded):
         """Verify that we can create a json file for each actor and not recurse any further."""
 
-        self._actors_test(tmpdir, test_data, original_data, "/root/actors/.*")
+        self._actors_test(tmpdir, test_data, original_data, "/root/actors/.*", threaded)
 
-    def test_actors2(self, tmpdir, test_data, original_data):
+    def test_actors2(self, tmpdir, test_data, original_data, threaded):
         """Same as test_actors1 but with a more precise regex."""
 
-        self._actors_test(tmpdir, test_data, original_data, "/root/actors/[^/]+")
+        self._actors_test(tmpdir, test_data, original_data, "/root/actors/[^/]+", threaded)
 
-    def test_charlie1(self, tmpdir, test_data, original_data):
+    def test_charlie1(self, tmpdir, test_data, original_data, threaded):
         """Verify that we can single out an actor."""
-        self._charlie_test(tmpdir, test_data, original_data, "/root/actors/charlie_chaplin")
+        self._charlie_test(tmpdir, test_data, original_data, "/root/actors/charlie_chaplin", threaded)
 
-    def test_charlie2(self, tmpdir, test_data, original_data):
+    def test_charlie2(self, tmpdir, test_data, original_data, threaded):
         """Like test_charlie1 but with a loose wildcard."""
-        self._charlie_test(tmpdir, test_data, original_data, "/root/actors/[abcxyz].*")
+        self._charlie_test(tmpdir, test_data, original_data, "/root/actors/[abcxyz].*", threaded)
 
-    def test_charlie3(self, tmpdir, test_data, original_data):
+    def test_charlie3(self, tmpdir, test_data, original_data, threaded):
         """Like test_charlie1 but with tighter regex."""
-        self._charlie_test(tmpdir, test_data, original_data, "/root/actors/[abcxyz][^/]+")
+        self._charlie_test(tmpdir, test_data, original_data, "/root/actors/[abcxyz][^/]+", threaded)
 
-    def test_nested1(self, tmpdir, test_data, original_data):
+    def test_threaded_nested1(self, tmpdir, test_data, original_data, threaded):
         """Test a simple leaf_nodes scenario."""
+
         expanded = JsonExpandOMatic(path=tmpdir).expand(
             test_data,
             root_element="root",
             preserve=False,
             leaf_nodes=[{"/root/actors/.*": ["/[^/]+/movies/.*", "/[^/]+/filmography"]}],
+            threaded=threaded,
         )
         assert expanded == {"root": {"$ref": f"{tmpdir.basename}/root.json"}}
 
         # This is the same thing you would expect in the non-nested case.
         self._assert_root(tmpdir)
         self._assert_actors(tmpdir)
 
@@ -80,15 +86,15 @@
         assert os.path.exists(f"{tmpdir}/root/actors/charlie_chaplin/spouses")
         assert os.path.exists(f"{tmpdir}/root/actors/charlie_chaplin/spouses/oona_oneill.json")
         assert os.path.exists(f"{tmpdir}/root/actors/charlie_chaplin/spouses/oona_oneill")
         assert os.path.exists(f"{tmpdir}/root/actors/charlie_chaplin/spouses/oona_oneill/children.json")
         assert os.path.exists(f"{tmpdir}/root/actors/dwayne_johnson/hobbies.json")
         assert not os.path.exists(f"{tmpdir}/root/actors/dwayne_johnson/hobbies")
 
-    def test_nested1_equivalency(self, tmpdir, test_data, original_data):
+    def test_nested1_equivalency(self, tmpdir, test_data, original_data, threaded):
         """
         In a nested leaf-node expression the dict key is treated as it
         would be in the non-nested case.
 
         The nested functionality takes the file written by that expression
         and feeds it back through JsonExpandOMatic with the dict's value
         as the new leaf_nodes parameter value.
@@ -100,28 +106,30 @@
         import glob
 
         JsonExpandOMatic(path=f"{tmpdir}/n").expand(
             test_data,
             root_element="root",
             preserve=False,
             leaf_nodes=[{"/root/actors/.*": ["/[^/]+/movies/.*", "/[^/]+/filmography"]}],
+            threaded=threaded,
         )
         nested_files = [x.replace(f"{tmpdir}/n", "") for x in glob.glob(f"{tmpdir}/n", recursive=True)]
 
         JsonExpandOMatic(path=f"{tmpdir}/f").expand(
             test_data,
             root_element="root",
             preserve=False,
             leaf_nodes=["/root/actors/.*/movies/.*", "/root/actors/.*/filmography"],
+            threaded=threaded,
         )
         flattened_files = [x.replace(f"{tmpdir}/f", "") for x in glob.glob(f"{tmpdir}/f", recursive=True)]
 
         assert nested_files == flattened_files
 
-    def test_nested2(self, tmpdir, test_data, original_data):
+    def test_nested2(self, tmpdir, test_data, original_data, threaded):
         """Test a targeted leaf_node exmple.
 
         The expressions listed in the dict value are relative to the
         element matched by the dict key expression.
         Our previous examlpes used a regex to ignore that but we can do
         interesting things with it if we want.
 
@@ -129,14 +137,15 @@
         and Charlie Chaplin's spouses.
         """
         expanded = JsonExpandOMatic(path=tmpdir).expand(
             test_data,
             root_element="root",
             preserve=False,
             leaf_nodes=[{"/root/actors/.*": ["/dwayne_johnson/movies", "/charlie_chaplin/spouses"]}],
+            threaded=threaded,
         )
         assert expanded == {"root": {"$ref": f"{tmpdir.basename}/root.json"}}
 
         # This is the same thing you would expect in the non-nested case.
         self._assert_root(tmpdir)
         self._assert_actors(tmpdir)
 
@@ -148,15 +157,15 @@
         assert os.path.exists(f"{tmpdir}/root/actors/charlie_chaplin/movies.json")
         assert os.path.exists(f"{tmpdir}/root/actors/charlie_chaplin/movies")
         assert os.path.exists(f"{tmpdir}/root/actors/charlie_chaplin/spouses.json")
         assert not os.path.exists(f"{tmpdir}/root/actors/charlie_chaplin/spouses")
         assert os.path.exists(f"{tmpdir}/root/actors/dwayne_johnson/movies.json")
         assert not os.path.exists(f"{tmpdir}/root/actors/dwayne_johnson/movies")
 
-    def xtest_enhanced_nested1(self, tmpdir, test_data, original_data):
+    def xtest_enhanced_nested1(self, tmpdir, test_data, original_data, threaded):
         """Enhanced nested #1...
 
         But what if we want a single json file per actor to include
         everything about that actor _except_ movies and a separate
         movies.json for each actor with all of that actor's movie data?
 
         You might initially have thought that we would do:
@@ -197,14 +206,15 @@
         """
 
         JsonExpandOMatic(path=tmpdir).expand(
             test_data,
             root_element="root",
             preserve=False,
             leaf_nodes=[{"/root/actors/.*": ["/[^/]+/movies/.*", "<A:/.*"]}],
+            threaded=threaded,
         )
 
         # This is the same thing you would expect in the non-nested case.
         self._assert_root(tmpdir)
         self._assert_actors(tmpdir)
 
         # Unlike the non-nested case with regex "/root/actors/.*", the nested case
@@ -228,17 +238,21 @@
 
         with open(f"{tmpdir}/root/actors/charlie_chaplin.json") as f:
             data = json.load(f)
             assert data.get("spouses", None)
             assert data.get["spouses"].get("lita_grey", None)
             assert data.get["spouses"]["lita_grey"].get("children", None)
 
-    def _actors_test(self, tmpdir, test_data, original_data, regex):
+    def _actors_test(self, tmpdir, test_data, original_data, regex, threaded):
         expanded = JsonExpandOMatic(path=tmpdir).expand(
-            test_data, root_element="root", preserve=False, leaf_nodes=[regex]
+            test_data,
+            root_element="root",
+            preserve=False,
+            leaf_nodes=[regex],
+            threaded=threaded,
         )
 
         # preserve=True allows mangling of test_data by expand()
         assert test_data != original_data
 
         # expand() returns a new representation of `data`
         assert expanded == {"root": {"$ref": f"{tmpdir.basename}/root.json"}}
@@ -250,17 +264,21 @@
         # Our leaf-node regex (/root/actors/.*) tells expand to create a
         # per-actor file but not the per-actor directory or anything below that.
         self._assert_root(tmpdir)
         self._assert_actors(tmpdir)
         self._assert_actor_dirs(tmpdir, f=_not)
         self._assert_movies(tmpdir, f=_not)
 
-    def _charlie_test(self, tmpdir, test_data, original_data, regex):
+    def _charlie_test(self, tmpdir, test_data, original_data, regex, threaded):
         expanded = JsonExpandOMatic(path=tmpdir).expand(
-            test_data, root_element="root", preserve=False, leaf_nodes=[regex]
+            test_data,
+            root_element="root",
+            preserve=False,
+            leaf_nodes=[regex],
+            threaded=threaded,
         )
         assert expanded == {"root": {"$ref": f"{tmpdir.basename}/root.json"}}
 
         self._assert_root(tmpdir)
         self._assert_actors(tmpdir)
 
         # No recursion for Charlie Chaplin
```

### Comparing `json_expand_o_matic-0.2.0/tests/test_simple.py` & `json_expand_o_matic-0.2.1/tests/test_simple.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,50 +17,58 @@
     def raw_data(self, resource_path_root):
         if not TestSimple._raw_data:
             TestSimple._raw_data = json.loads((resource_path_root / "actor-data.json").read_text())
         return TestSimple._raw_data
 
     # Fixtures to provide copies of the raw data to each test function.
 
+    @pytest.fixture(params=[False, True])
+    def threaded(self, request):
+        return request.param
+
     @pytest.fixture
     def test_data(self, raw_data):
         return json.loads(json.dumps(raw_data))
 
     @pytest.fixture
     def original_data(self, raw_data):
         return json.loads(json.dumps(raw_data))
 
     def test_equivalency(self, test_data, original_data):
         # Assert that independent copies of the raw data are equivalent.
         assert test_data == original_data
 
-    def test_expand_preserve(self, tmpdir, test_data, original_data):
-        expanded = JsonExpandOMatic(path=tmpdir).expand(test_data, root_element="root", preserve=True)
+    def test_expand_preserve(self, tmpdir, test_data, original_data, threaded):
+        expanded = JsonExpandOMatic(path=tmpdir).expand(
+            test_data, root_element="root", preserve=True, threaded=threaded
+        )
 
         # preserve=True prevents mangling of test_data by expand()
         assert test_data == original_data
 
         # expand() returns a new representation of `data`
         assert expanded == {"root": {"$ref": f"{tmpdir.basename}/root.json"}}
 
-    def test_expand_mangle(self, tmpdir, test_data, original_data):
-        expanded = JsonExpandOMatic(path=tmpdir).expand(test_data, root_element="root", preserve=False)
+    def test_expand_mangle(self, tmpdir, test_data, original_data, threaded):
+        expanded = JsonExpandOMatic(path=tmpdir).expand(
+            test_data, root_element="root", preserve=False, threaded=threaded
+        )
 
         # preserve=True allows mangling of test_data by expand()
         assert test_data != original_data
 
         # test_data is the content of "{tmpdir.basename}/root.json"
         assert test_data == {"actors": {"$ref": "root/actors.json"}}
         assert test_data == json.loads(tmpdir.join("root.json").read())
 
         # expand() returns a new representation of `data`
         assert expanded == {"root": {"$ref": f"{tmpdir.basename}/root.json"}}
 
-    def test_file_exixtence(self, tmpdir, test_data, original_data):
-        expanded = JsonExpandOMatic(path=tmpdir).expand(test_data, root_element="root")
+    def test_file_exixtence(self, tmpdir, test_data, original_data, threaded):
+        expanded = JsonExpandOMatic(path=tmpdir).expand(test_data, root_element="root", threaded=threaded)
         assert expanded == {"root": {"$ref": f"{tmpdir.basename}/root.json"}}
 
         # This is the wrapper around the original data
         assert os.path.exists(f"{tmpdir}/root.json")
         assert os.path.exists(f"{tmpdir}/root")
 
         # Now we look at the original data's files
@@ -86,29 +94,33 @@
         # a file but not a directory (since there was nothing to recurse into).
         assert os.path.exists(f"{tmpdir}/root/actors/dwayne_johnson/hobbies.json")
         assert not os.path.exists(f"{tmpdir}/root/actors/dwayne_johnson/hobbies")
 
         # I'm not going to go any deeper. You get the idea...
         # See `test_leaves.py` for some more interesting things about the files.
 
-    def test_contract(self, tmpdir, test_data, original_data):
-        expanded = JsonExpandOMatic(path=tmpdir).expand(test_data, root_element="root", preserve=False)
+    def test_contract(self, tmpdir, test_data, original_data, threaded):
+        expanded = JsonExpandOMatic(path=tmpdir).expand(
+            test_data, root_element="root", preserve=False, threaded=threaded
+        )
         assert expanded == {"root": {"$ref": f"{tmpdir.basename}/root.json"}}
 
         # We can use JsonExpandOMatic() to load the expanded data from the filesystem.
         # Note that this returns the original data exactly, the `root` wrapper is removed.
         contracted = JsonExpandOMatic(path=tmpdir).contract(root_element="root")
         assert contracted == original_data
 
         # Or we can use jsonref.load() to do the same.
         with open(f"{tmpdir}/root.json") as f:
             assert jsonref.load(f, base_uri=f"file://{tmpdir}/") == original_data
 
-    def test_jsonref(self, tmpdir, test_data, original_data):
-        expanded = JsonExpandOMatic(path=tmpdir).expand(test_data, root_element="root", preserve=False)
+    def test_jsonref(self, tmpdir, test_data, original_data, threaded):
+        expanded = JsonExpandOMatic(path=tmpdir).expand(
+            test_data, root_element="root", preserve=False, threaded=threaded
+        )
 
         # We can use jsonref to load this new representation.
         # Note that loading in this way exposes the wrapping element `root`.
         # `tmpdir` must be a fully qualified path.
         loaded = jsonref.loads(json.dumps(expanded), base_uri=f"file://{tmpdir.dirname}/")
         assert loaded == {"root": original_data}
         assert loaded["root"] == original_data
```

