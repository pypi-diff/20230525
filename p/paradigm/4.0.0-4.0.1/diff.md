# Comparing `tmp/paradigm-4.0.0.tar.gz` & `tmp/paradigm-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradigm-4.0.0.tar", last modified: Tue Feb  7 22:04:58 2023, max compression
+gzip compressed data, was "paradigm-4.0.1.tar", last modified: Thu May 25 06:23:56 2023, max compression
```

## Comparing `paradigm-4.0.0.tar` & `paradigm-4.0.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:04:58.764972 paradigm-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-07 22:04:47.000000 paradigm-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-07 22:04:47.000000 paradigm-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-02-07 22:04:58.764972 paradigm-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-02-07 22:04:47.000000 paradigm-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:04:58.760972 paradigm-4.0.0/paradigm/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:04:58.760972 paradigm-4.0.0/paradigm/_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/annotated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:04:58.760972 paradigm-4.0.0/paradigm/_core/arboreal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/arboreal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/arboreal/construction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/arboreal/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    18958 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/arboreal/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/arboreal/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/arboreal/kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/arboreal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    24186 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/namespacing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/pretty.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/scoping.py
--rw-r--r--   0 runner    (1001) docker     (123)    26235 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)    47999 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/stubs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/_core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/base.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 22:04:47.000000 paradigm-4.0.0/paradigm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:04:58.760972 paradigm-4.0.0/paradigm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-02-07 22:04:58.000000 paradigm-4.0.0/paradigm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-02-07 22:04:58.000000 paradigm-4.0.0/paradigm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 22:04:58.000000 paradigm-4.0.0/paradigm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-07 22:04:58.000000 paradigm-4.0.0/paradigm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-07 22:04:58.000000 paradigm-4.0.0/paradigm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-07 22:04:47.000000 paradigm-4.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-07 22:04:58.764972 paradigm-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-02-07 22:04:47.000000 paradigm-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:23:56.882045 paradigm-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-25 06:23:47.000000 paradigm-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 06:23:47.000000 paradigm-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-25 06:23:56.882045 paradigm-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-25 06:23:47.000000 paradigm-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:23:56.882045 paradigm-4.0.1/paradigm/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:23:56.882045 paradigm-4.0.1/paradigm/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/annotated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:23:56.882045 paradigm-4.0.1/paradigm/_core/arboreal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/arboreal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/arboreal/construction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/arboreal/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/arboreal/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/arboreal/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/arboreal/kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/arboreal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24186 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/namespacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/scoping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26241 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47999 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/_core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:23:47.000000 paradigm-4.0.1/paradigm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:23:56.882045 paradigm-4.0.1/paradigm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-25 06:23:56.000000 paradigm-4.0.1/paradigm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-25 06:23:56.000000 paradigm-4.0.1/paradigm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 06:23:56.000000 paradigm-4.0.1/paradigm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 06:23:56.000000 paradigm-4.0.1/paradigm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 06:23:56.000000 paradigm-4.0.1/paradigm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 06:23:47.000000 paradigm-4.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-25 06:23:56.882045 paradigm-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-25 06:23:47.000000 paradigm-4.0.1/setup.py
```

### Comparing `paradigm-4.0.0/LICENSE` & `paradigm-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/PKG-INFO` & `paradigm-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradigm
-Version: 4.0.0
+Version: 4.0.1
 Summary: Python objects metadata parser.
 Home-page: https://github.com/lycantropos/paradigm/
 Download-URL: https://github.com/lycantropos/paradigm/archive/master.zip
 Author: Azat Ibrakov
 Author-email: azatibrakov@gmail.com
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paradigm-4.0.0/README.md` & `paradigm-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/paradigm/_core/annotated.py` & `paradigm-4.0.1/paradigm/_core/annotated.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/paradigm/_core/arboreal/construction.py` & `paradigm-4.0.1/paradigm/_core/arboreal/construction.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/paradigm/_core/arboreal/conversion.py` & `paradigm-4.0.1/paradigm/_core/arboreal/conversion.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/paradigm/_core/arboreal/evaluation.py` & `paradigm-4.0.1/paradigm/_core/arboreal/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import types
 import typing as t
 import weakref
 from collections import ChainMap
 from functools import singledispatch
 from importlib import import_module
 
-from typing_extensions import Self
+import typing_extensions as te
 
 from paradigm._core import (catalog,
                             namespacing,
                             scoping,
                             sources,
                             stubs)
 from . import (construction,
@@ -69,14 +69,40 @@
       parent_namespace: namespacing.Namespace) -> t.Any:
     return evaluate_operator_node(ast_node.op)(
             evaluate_expression_node(ast_node.operand, module_path,
                                      parent_path, parent_namespace)
     )
 
 
+_T = t.TypeVar('_T')
+
+
+def _all_not_none(
+        value: t.List[t.Optional[_T]]
+) -> te.TypeGuard[t.List[_T]]:
+    return all(element is not None for element in value)
+
+
+@evaluate_expression_node.register(ast.Dict)
+def _(ast_node: ast.Dict,
+      module_path: catalog.Path,
+      parent_path: catalog.Path,
+      parent_namespace: namespacing.Namespace) -> t.Any:
+    assert _all_not_none(ast_node.keys), ast_node.keys
+    return {
+        evaluate_expression_node(
+                key, module_path, parent_path, parent_namespace
+        ):
+            evaluate_expression_node(
+                    value, module_path, parent_path, parent_namespace
+            )
+        for key, value in zip(ast_node.keys, ast_node.values)
+    }
+
+
 @evaluate_operator_node.register(ast.BitAnd)
 def _(ast_node: ast.BitAnd) -> t.Any:
     return operator.and_
 
 
 @evaluate_operator_node.register(ast.BitOr)
 def _(ast_node: ast.BitOr) -> t.Any:
@@ -279,15 +305,15 @@
         parent_namespace: namespacing.Namespace,
         *,
         builtins_module_path: catalog.Path
         = catalog.module_path_from_module(builtins),
         modules_cache: t.MutableMapping[catalog.Path, types.ModuleType]
         = weakref.WeakValueDictionary(),
         objects_cache: t.MutableMapping[catalog.QualifiedPath, t.Any]
-        = weakref.WeakValueDictionary([((('_typeshed',), ('Self',)), Self)])
+        = weakref.WeakValueDictionary([((('_typeshed',), ('Self',)), te.Self)])
 ) -> t.Any:
     module_name = catalog.path_to_string(module_path)
     try:
         module = import_module(module_name)
     except ImportError:
         if not object_path:
             try:
@@ -432,14 +458,15 @@
     def _(ast_node: ast.Num,
           module_path: catalog.Path,
           parent_path: catalog.Path,
           parent_namespace: namespacing.Namespace) -> t.Any:
         return ast_node.n
 
 
+    @evaluate_expression_node.register(ast.Bytes)
     @evaluate_expression_node.register(ast.Str)
     def _(ast_node: ast.Str,
           module_path: catalog.Path,
           parent_path: catalog.Path,
           parent_namespace: namespacing.Namespace) -> t.Any:
         return ast_node.s
```

### Comparing `paradigm-4.0.0/paradigm/_core/arboreal/execution.py` & `paradigm-4.0.1/paradigm/_core/arboreal/execution.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/paradigm/_core/arboreal/utils.py` & `paradigm-4.0.1/paradigm/_core/arboreal/utils.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/paradigm/_core/caching.py` & `paradigm-4.0.1/paradigm/_core/caching.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/paradigm/_core/catalog.py` & `paradigm-4.0.1/paradigm/_core/catalog.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/paradigm/_core/discovery.py` & `paradigm-4.0.1/paradigm/_core/discovery.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/paradigm/_core/execution.py` & `paradigm-4.0.1/paradigm/_core/execution.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/paradigm/_core/file_system.py` & `paradigm-4.0.1/paradigm/_core/file_system.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/paradigm/_core/index.py` & `paradigm-4.0.1/paradigm/_core/index.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/paradigm/_core/models.py` & `paradigm-4.0.1/paradigm/_core/models.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/paradigm/_core/modules.py` & `paradigm-4.0.1/paradigm/_core/modules.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/paradigm/_core/pretty.py` & `paradigm-4.0.1/paradigm/_core/pretty.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/paradigm/_core/scoping.py` & `paradigm-4.0.1/paradigm/_core/scoping.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/paradigm/_core/signatures.py` & `paradigm-4.0.1/paradigm/_core/signatures.py`

 * *Files 0% similar despite different names*

```diff
@@ -612,15 +612,15 @@
         module_path: _catalog.Path,
         parent_path: _catalog.Path
 ) -> _t.List[_Parameter]:
     # double-reversing since parameters with default arguments go last
     parameters_with_defaults_ast: _t.List[
         _t.Tuple[_ast.arg, _t.Optional[_ast.expr]]
     ] = list(_zip_longest(reversed(signature_ast.args),
-                          signature_ast.defaults))[::-1]
+                          signature_ast.defaults[::-1]))[::-1]
     kind = _ParameterKind.POSITIONAL_ONLY
     return [_parameter_from_ast_node(parameter_ast, default_ast, module_path,
                                      parent_path, kind)
             for parameter_ast, default_ast in parameters_with_defaults_ast]
 
 
 def _to_variadic_keyword_parameter(
```

### Comparing `paradigm-4.0.0/paradigm/_core/sources.py` & `paradigm-4.0.1/paradigm/_core/sources.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/paradigm/_core/stubs.py` & `paradigm-4.0.1/paradigm/_core/stubs.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/paradigm/_core/utils.py` & `paradigm-4.0.1/paradigm/_core/utils.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/paradigm.egg-info/PKG-INFO` & `paradigm-4.0.1/paradigm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradigm
-Version: 4.0.0
+Version: 4.0.1
 Summary: Python objects metadata parser.
 Home-page: https://github.com/lycantropos/paradigm/
 Download-URL: https://github.com/lycantropos/paradigm/archive/master.zip
 Author: Azat Ibrakov
 Author-email: azatibrakov@gmail.com
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paradigm-4.0.0/paradigm.egg-info/SOURCES.txt` & `paradigm-4.0.1/paradigm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paradigm-4.0.0/setup.py` & `paradigm-4.0.1/setup.py`

 * *Files identical despite different names*

