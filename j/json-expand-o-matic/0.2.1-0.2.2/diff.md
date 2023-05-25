# Comparing `tmp/json_expand_o_matic-0.2.1.tar.gz` & `tmp/json_expand_o_matic-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_expand_o_matic-0.2.1.tar", last modified: Thu May 25 02:14:13 2023, max compression
+gzip compressed data, was "json_expand_o_matic-0.2.2.tar", last modified: Thu May 25 02:25:52 2023, max compression
```

## Comparing `json_expand_o_matic-0.2.1.tar` & `json_expand_o_matic-0.2.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:14:13.908851 json_expand_o_matic-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-25 02:14:13.908851 json_expand_o_matic-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-25 02:12:26.000000 json_expand_o_matic-0.2.1/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 02:12:16.000000 json_expand_o_matic-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 02:14:13.908851 json_expand_o_matic-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:14:13.900850 json_expand_o_matic-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:14:13.904850 json_expand_o_matic-0.2.1/src/json_expand_o_matic/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic/contractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic/expand_o_matic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic/expander.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic/expansion_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic/leaf_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:14:13.908851 json_expand_o_matic-0.2.1/src/json_expand_o_matic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-25 02:14:13.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-25 02:14:13.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 02:14:13.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 02:14:13.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 02:14:13.000000 json_expand_o_matic-0.2.1/src/json_expand_o_matic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:14:13.908851 json_expand_o_matic-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/tests/test_leaves.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 02:12:05.000000 json_expand_o_matic-0.2.1/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:25:52.719956 json_expand_o_matic-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-25 02:25:52.719956 json_expand_o_matic-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-25 02:23:59.000000 json_expand_o_matic-0.2.2/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 02:23:52.000000 json_expand_o_matic-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 02:25:52.719956 json_expand_o_matic-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:25:52.711955 json_expand_o_matic-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:25:52.715956 json_expand_o_matic-0.2.2/src/json_expand_o_matic/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic/contractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic/expand_o_matic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic/expander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic/expansion_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic/expansion_zipper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic/leaf_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:25:52.715956 json_expand_o_matic-0.2.2/src/json_expand_o_matic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-25 02:25:52.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-25 02:25:52.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 02:25:52.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 02:25:52.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 02:25:52.000000 json_expand_o_matic-0.2.2/src/json_expand_o_matic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:25:52.719956 json_expand_o_matic-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/tests/test_leaves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 02:23:41.000000 json_expand_o_matic-0.2.2/version.txt
```

### Comparing `json_expand_o_matic-0.2.1/LICENSE.txt` & `json_expand_o_matic-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.1/PKG-INFO` & `json_expand_o_matic-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_expand_o_matic
-Version: 0.2.1
+Version: 0.2.2
 Summary: Expand a dict into a collection of subdirectories and json files or contract (un-expand) the output of expand() into a dict.
 Home-page: https://github.com/jcejohnson/JsonExpandOMatic
 Author: James Johnson
 Author-email: jcejohnson@users.noreply.github.com
 Keywords: json,jsonref
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `json_expand_o_matic-0.2.1/README.md` & `json_expand_o_matic-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.1/dev-requirements.txt` & `json_expand_o_matic-0.2.2/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.1/setup.py` & `json_expand_o_matic-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='json_expand_o_matic',
 
-    version='0.2.1',
+    version='0.2.2',
 
     description='Expand a dict into a collection of subdirectories and json files or '
                 'contract (un-expand) the output of expand() into a dict.',
 
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `json_expand_o_matic-0.2.1/src/json_expand_o_matic/__init__.py` & `json_expand_o_matic-0.2.2/src/json_expand_o_matic/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 
     See also: .jsonrefkeeper
 
 """
 
 from .expand_o_matic import JsonExpandOMatic
 
-VERSION = "v0.2.1"
+VERSION = "v0.2.2"
```

### Comparing `json_expand_o_matic-0.2.1/src/json_expand_o_matic/cli.py` & `json_expand_o_matic-0.2.2/src/json_expand_o_matic/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,22 +55,33 @@
         try:
             leaf_nodes.append(json.loads(node))
         except Exception:
             leaf_nodes.append(node)
 
     from .expander import Expander
 
+    expansion_options = {
+        key: func(os.environ.get(var))
+        for key, func, var in [
+            ("pool_size", int, "JEOM_POOL_SIZE"),
+            ("pool_ratio", float, "JEOM_POOL_RATIO"),
+            ("pool_mode", float, "JEOM_POOL_MODE"),
+            ("zip_root", str, "JEOM_ZIP_ROOT"),
+            ("zip_file", str, "JEOM_ZIP_FILE"),
+        ]
+        if var in os.environ
+    }
+
     JsonExpandOMatic(logger=logger, path=output_path).expand(
         data=json.load(open(input_file)),
         root_element="root",
         preserve=False,
         leaf_nodes=leaf_nodes,
         hash_mode=Expander.HASH_MD5,
-        pool_size=int(os.environ.get("JEOM_POOL_SIZE") or 1),
-        pool_ratio=float(os.environ.get("JEOM_POOL_RATIO") or 1),
+        **expansion_options
         # leaf_nodes=["/.*"]
         # leaf_nodes=["/root/actors/.*/movies/.*"]
         # leaf_nodes=[{"/root/actors/.*": ["/[^/]+/movies/.*"]}]
         # # This may be working...
         # leaf_nodes=[
         #     {
         #         ">B:/root/actors/[^/]+$": [
```

### Comparing `json_expand_o_matic-0.2.1/src/json_expand_o_matic/contractor.py` & `json_expand_o_matic-0.2.2/src/json_expand_o_matic/contractor.py`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.1/src/json_expand_o_matic/expand_o_matic.py` & `json_expand_o_matic-0.2.2/src/json_expand_o_matic/expand_o_matic.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
         Parameters
         ----------
         path : str
             Target directory where expand will write the expanded json data
             and/or where contract will find the expanded data to be loaded.
         """
-        self.path = os.path.abspath(path)
+        self.path = path
+        self.abspath = os.path.abspath(path)
         self.logger = logger
 
     def expand(self, data, root_element="root", preserve=True, leaf_nodes=[], **expander_options):
         """Expand a dict into a collection of subdirectories and json files.
 
         Creates:
         - {self.path}/{root_element}.json
@@ -48,15 +49,15 @@
         if preserve:
             data = json.loads(json.dumps(data))
 
         from .expander import Expander
 
         expander = Expander(
             logger=self.logger,
-            path=self.path,
+            path=self.abspath,
             data={root_element: data},
             leaf_nodes=LeafNode.construct(leaf_nodes),
             **expander_options,
         )
         result = expander.execute()
         self.hashcodes = expander.hashcodes
 
@@ -79,8 +80,8 @@
         --------
         dict or list
             The data that was originally expanded.
         """
 
         from .contractor import Contractor
 
-        return Contractor(logger=self.logger, path=self.path, root_element=root_element).execute()
+        return Contractor(logger=self.logger, path=self.abspath, root_element=root_element).execute()
```

### Comparing `json_expand_o_matic-0.2.1/src/json_expand_o_matic/expander.py` & `json_expand_o_matic-0.2.2/src/json_expand_o_matic/expander.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import collections
 import hashlib
 import json
 import os
 
-from .expansion_pool import ExpansionPool
 from .leaf_node import LeafNode
 
 
 class Expander:
     """Expand a dict or list into one or more json files."""
 
     HASH_MD5 = "HASH_MD5"
@@ -16,20 +15,27 @@
         assert isinstance(data, dict) or isinstance(data, list)
 
         self.logger = logger
         self.path = path
         self.data = data
         self.leaf_nodes = leaf_nodes
 
-        self.work = None
-
         self.options = options if options is not None else dict()
+
+        # options will not include pool or zip options when called recursively.
         self.pool_options = {
             key: self.options.pop(key) for key in {key for key in self.options.keys() if key.startswith("pool_")}
         }
+        self.zip_options = {
+            key: self.options.pop(key) for key in {key for key in self.options.keys() if key.startswith("zip_")}
+        }
+
+        assert (
+            (not self.pool_options and not self.zip_options) or self.pool_options or self.zip_options
+        ), f"Cannot mix {sorted(self.pool_options.keys())} and {sorted(self.zip_options.keys())}"
 
         self.ref_key = self.options.get("ref_key", "$ref")
 
         self.json_dump_kwargs = self.options.get(
             "json_dump_kwargs", {"indent": "", "sort_keys": False, "separators": (",", ":")}
         )
 
@@ -47,26 +53,37 @@
 
     def execute(self):
         """Expand self.data into one or more json files."""
 
         # Replace the _dump() method with a no-op for the root of the data.
         self._dump = lambda *args: None
 
-        pool = ExpansionPool(logger=self.logger, **self.pool_options)
-        self.work = pool.work
+        if self.zip_options:
+            from .expansion_zipper import ExpansionZipper
+
+            pool, work = ExpansionZipper(logger=self.logger, output_path=self.path, **self.zip_options).setup()
+            self.path = pool.zip_root
+        elif self.pool_options:
+            from .expansion_pool import ExpansionPool
+
+            pool, work = ExpansionPool(logger=self.logger, **self.pool_options).setup()
+        else:
+            from .expansion_pool import ExpansionPool
+
+            pool, work = ExpansionPool(logger=self.logger, pool_disable=True).setup()
 
-        expansion = self._execute(indent=0, my_path_component=os.path.basename(self.path), traversal="")
+        expansion = self._execute(indent=0, my_path_component=os.path.basename(self.path), traversal="", work=work)
 
-        pool.drain()
+        pool.finalize()
 
         self._hashcodes_cleanup()
 
         return expansion
 
-    def _execute(self, traversal, indent, my_path_component):
+    def _execute(self, traversal, indent, my_path_component, work):
         """Main...
 
         Parameters
         ----------
         indent : int
             Used to indent log messages so that we can see the data tree.
         traversal : string
@@ -79,17 +96,18 @@
 
         Returns:
         --------
         dict
             data
         """
 
-        self.traversal = traversal
         self.indent = indent
         self.my_path_component = my_path_component
+        self.traversal = traversal
+        self.work = work
 
         self._log(f"path [{self.path}] traversal [{self.traversal}]")
 
         if self._is_leaf_node(LeafNode.When.BEFORE):
             return self.data
 
         for key in self._data_iter():
@@ -171,58 +189,52 @@
             if c.comment or not c.match(string=self.traversal, when=when):
                 continue
 
             if not c.children:
                 return self._dump(c)
 
             self._log(f">>> Expand children of [{c.raw}]")
-            self._recursion_instance(
-                path=os.path.dirname(self.path),
-                data={os.path.basename(self.path): self.data},
-                leaf_nodes=c.children,
-            )._execute(indent=self.indent + 2, my_path_component=os.path.basename(self.path), traversal="")
+            expander = self._recursion_instance(
+                path=os.path.dirname(self.path), data={os.path.basename(self.path): self.data}, leaf_nodes=c.children
+            )
+            expander._execute(
+                indent=self.indent + 2, my_path_component=os.path.basename(self.path), traversal="", work=self.work
+            )
             self._log(f"<<< Expand children of [{c.raw}]")
 
             return self._dump(c)
 
         return False
 
     def _log(self, string):
         self.logger.debug(" " * self.indent + string)
 
-    def _recursion_instance(self, *, path, data, leaf_nodes):
-        instance = Expander(
-            logger=self.logger,
-            #
-            data=data,
-            leaf_nodes=leaf_nodes,
-            path=path,
-            #
-            **self.options,
-        )
-        instance.work = self.work
-        return instance
-
     def _recursively_expand(self, *, key):
         if not (isinstance(self.data[key], dict) or isinstance(self.data[key], list)):
             return
 
         path_component = str(key).replace(":", "_").replace("/", "_").replace("\\", "_").replace(" ", "_")
 
         expander = self._recursion_instance(
-            path=os.path.join(self.path, path_component),
-            data=self.data[key],
-            leaf_nodes=self.leaf_nodes,
+            path=os.path.join(self.path, path_component), data=self.data[key], leaf_nodes=self.leaf_nodes
         )
         self.data[key] = expander._execute(
-            indent=self.indent + 2, my_path_component=path_component, traversal=f"{self.traversal}/{key}"
+            indent=self.indent + 2,
+            my_path_component=path_component,
+            traversal=f"{self.traversal}/{key}",
+            work=self.work,
         )
 
         # Add the child's hashcodes to our own so that when we unroll the recursion the root
         # will not need to recurse again to collect the entire list.
         for hashcode in expander.hashcodes:
             if hashcode in self.hashcodes:
                 self.hashcodes[hashcode] += expander.hashcodes[hashcode]
             else:
                 self.hashcodes[hashcode] = expander.hashcodes[hashcode]
 
+    def _recursion_instance(self, *, path, data, leaf_nodes):  # key, path_component):
+        expander = Expander(logger=self.logger, path=path, data=data, leaf_nodes=leaf_nodes, **self.options)
+
+        return expander
+
         # self.data[key] = {"$ref": f"{self.my_path_component}/{path_component}.json"}
```

### Comparing `json_expand_o_matic-0.2.1/src/json_expand_o_matic/leaf_node.py` & `json_expand_o_matic-0.2.2/src/json_expand_o_matic/leaf_node.py`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.1/src/json_expand_o_matic.egg-info/PKG-INFO` & `json_expand_o_matic-0.2.2/src/json_expand_o_matic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-expand-o-matic
-Version: 0.2.1
+Version: 0.2.2
 Summary: Expand a dict into a collection of subdirectories and json files or contract (un-expand) the output of expand() into a dict.
 Home-page: https://github.com/jcejohnson/JsonExpandOMatic
 Author: James Johnson
 Author-email: jcejohnson@users.noreply.github.com
 Keywords: json,jsonref
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `json_expand_o_matic-0.2.1/src/json_expand_o_matic.egg-info/SOURCES.txt` & `json_expand_o_matic-0.2.2/src/json_expand_o_matic.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 version.txt
 src/json_expand_o_matic/__init__.py
 src/json_expand_o_matic/cli.py
 src/json_expand_o_matic/contractor.py
 src/json_expand_o_matic/expand_o_matic.py
 src/json_expand_o_matic/expander.py
 src/json_expand_o_matic/expansion_pool.py
+src/json_expand_o_matic/expansion_zipper.py
 src/json_expand_o_matic/leaf_node.py
 src/json_expand_o_matic.egg-info/PKG-INFO
 src/json_expand_o_matic.egg-info/SOURCES.txt
 src/json_expand_o_matic.egg-info/dependency_links.txt
 src/json_expand_o_matic.egg-info/entry_points.txt
 src/json_expand_o_matic.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `json_expand_o_matic-0.2.1/tests/test_leaves.py` & `json_expand_o_matic-0.2.2/tests/test_leaves.py`

 * *Files identical despite different names*

### Comparing `json_expand_o_matic-0.2.1/tests/test_simple.py` & `json_expand_o_matic-0.2.2/tests/test_simple.py`

 * *Files identical despite different names*

