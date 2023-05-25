# Comparing `tmp/typing_extensions-4.6.1.tar.gz` & `tmp/typing_extensions-4.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typing_extensions-4.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "typing_extensions-4.6.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `typing_extensions-4.6.1.tar` & `typing_extensions-4.6.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10437 2023-05-24 03:05:07.789039 typing_extensions-4.6.1/CHANGELOG.md
--rw-r--r--   0        0        0    12787 2022-12-31 19:31:45.654412 typing_extensions-4.6.1/LICENSE
--rw-r--r--   0        0        0     1290 2023-05-22 00:14:41.277524 typing_extensions-4.6.1/README.md
--rw-r--r--   0        0        0     1916 2023-05-24 03:05:07.789784 typing_extensions-4.6.1/pyproject.toml
--rw-r--r--   0        0        0      426 2022-12-31 19:31:45.655964 typing_extensions-4.6.1/src/_typed_dict_test_helper.py
--rw-r--r--   0        0        0   168884 2023-05-24 03:02:38.054358 typing_extensions-4.6.1/src/test_typing_extensions.py
--rw-r--r--   0        0        0   104451 2023-05-24 03:02:38.059891 typing_extensions-4.6.1/src/typing_extensions.py
--rw-r--r--   0        0        0      135 2023-05-22 00:37:39.060665 typing_extensions-4.6.1/tox.ini
--rw-r--r--   0        0        0     2786 1970-01-01 00:00:00.000000 typing_extensions-4.6.1/PKG-INFO
+-rw-r--r--   0        0        0    10760 2023-05-25 13:13:20.271098 typing_extensions-4.6.2/CHANGELOG.md
+-rw-r--r--   0        0        0    12787 2022-12-31 19:31:45.654412 typing_extensions-4.6.2/LICENSE
+-rw-r--r--   0        0        0     1290 2023-05-22 00:14:41.277524 typing_extensions-4.6.2/README.md
+-rw-r--r--   0        0        0     1916 2023-05-25 13:13:20.271880 typing_extensions-4.6.2/pyproject.toml
+-rw-r--r--   0        0        0      426 2022-12-31 19:31:45.655964 typing_extensions-4.6.2/src/_typed_dict_test_helper.py
+-rw-r--r--   0        0        0   170054 2023-05-25 13:09:56.284393 typing_extensions-4.6.2/src/test_typing_extensions.py
+-rw-r--r--   0        0        0   104592 2023-05-25 13:09:56.295773 typing_extensions-4.6.2/src/typing_extensions.py
+-rw-r--r--   0        0        0      135 2023-05-22 00:37:39.060665 typing_extensions-4.6.2/tox.ini
+-rw-r--r--   0        0        0     2786 1970-01-01 00:00:00.000000 typing_extensions-4.6.2/PKG-INFO
```

### Comparing `typing_extensions-4.6.1/CHANGELOG.md` & `typing_extensions-4.6.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# Release 4.6.2 (May 25, 2023)
+
+- Fix use of `@deprecated` on classes with `__new__` but no `__init__`.
+  Patch by Jelle Zijlstra.
+- Fix regression in version 4.6.1 where comparing a generic class against a
+  runtime-checkable protocol using `isinstance()` would cause `AttributeError`
+  to be raised if using Python 3.7.
+
 # Release 4.6.1 (May 23, 2023)
 
 - Change deprecated `@runtime` to formal API `@runtime_checkable` in the error
   message. Patch by Xuehai Pan.
 - Fix regression in 4.6.0 where attempting to define a `Protocol` that was
   generic over a `ParamSpec` or a `TypeVarTuple` would cause `TypeError` to be
   raised. Patch by Alex Waygood.
```

### Comparing `typing_extensions-4.6.1/LICENSE` & `typing_extensions-4.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `typing_extensions-4.6.1/README.md` & `typing_extensions-4.6.2/README.md`

 * *Files identical despite different names*

### Comparing `typing_extensions-4.6.1/pyproject.toml` & `typing_extensions-4.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["flit_core >=3.4,<4"]
 build-backend = "flit_core.buildapi"
 
 # Project metadata
 [project]
 name = "typing_extensions"
-version = "4.6.1"
+version = "4.6.2"
 description = "Backported and Experimental Type Hints for Python 3.7+"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = [
     "annotations",
     "backport",
```

### Comparing `typing_extensions-4.6.1/src/test_typing_extensions.py` & `typing_extensions-4.6.2/src/test_typing_extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,23 +353,25 @@
 
         with self.assertWarnsRegex(DeprecationWarning, "A will go away soon"):
             A()
         with self.assertWarnsRegex(DeprecationWarning, "A will go away soon"):
             with self.assertRaises(TypeError):
                 A(42)
 
+    def test_class_with_init(self):
         @deprecated("HasInit will go away soon")
         class HasInit:
             def __init__(self, x):
                 self.x = x
 
         with self.assertWarnsRegex(DeprecationWarning, "HasInit will go away soon"):
             instance = HasInit(42)
         self.assertEqual(instance.x, 42)
 
+    def test_class_with_new(self):
         has_new_called = False
 
         @deprecated("HasNew will go away soon")
         class HasNew:
             def __new__(cls, x):
                 nonlocal has_new_called
                 has_new_called = True
@@ -378,14 +380,16 @@
             def __init__(self, x) -> None:
                 self.x = x
 
         with self.assertWarnsRegex(DeprecationWarning, "HasNew will go away soon"):
             instance = HasNew(42)
         self.assertEqual(instance.x, 42)
         self.assertTrue(has_new_called)
+
+    def test_class_with_inherited_new(self):
         new_base_called = False
 
         class NewBase:
             def __new__(cls, x):
                 nonlocal new_base_called
                 new_base_called = True
                 return super().__new__(cls)
@@ -398,14 +402,31 @@
             pass
 
         with self.assertWarnsRegex(DeprecationWarning, "HasInheritedNew will go away soon"):
             instance = HasInheritedNew(42)
         self.assertEqual(instance.x, 42)
         self.assertTrue(new_base_called)
 
+    def test_class_with_new_but_no_init(self):
+        new_called = False
+
+        @deprecated("HasNewNoInit will go away soon")
+        class HasNewNoInit:
+            def __new__(cls, x):
+                nonlocal new_called
+                new_called = True
+                obj = super().__new__(cls)
+                obj.x = x
+                return obj
+
+        with self.assertWarnsRegex(DeprecationWarning, "HasNewNoInit will go away soon"):
+            instance = HasNewNoInit(42)
+        self.assertEqual(instance.x, 42)
+        self.assertTrue(new_called)
+
     def test_function(self):
         @deprecated("b will go away soon")
         def b():
             pass
 
         with self.assertWarnsRegex(DeprecationWarning, "b will go away soon"):
             b()
@@ -2242,14 +2263,36 @@
         f = Foo()
         self.assertNotIsInstance(f, HasX)
         f.x = 42
         self.assertIsInstance(f, HasX)
         del f.x
         self.assertNotIsInstance(f, HasX)
 
+    def test_protocols_isinstance_generic_classes(self):
+        T = TypeVar("T")
+
+        class Foo(Generic[T]):
+            x: T
+
+            def __init__(self, x):
+                self.x = x
+
+        class Bar(Foo[int]):
+            ...
+
+        @runtime_checkable
+        class HasX(Protocol):
+            x: int
+
+        foo = Foo(1)
+        self.assertIsInstance(foo, HasX)
+
+        bar = Bar(2)
+        self.assertIsInstance(bar, HasX)
+
     def test_protocols_support_register(self):
         @runtime_checkable
         class P(Protocol):
             x = 1
         class PM(Protocol):
             def meth(self): pass
         class D(PM): pass
@@ -4326,14 +4369,15 @@
                 A = G[int]
                 self.assertIs(A.__origin__, G)
                 self.assertEqual(A.__args__, (int,))
                 self.assertEqual(A.__parameters__, ())
 
                 a = A(3)
                 self.assertIs(type(a), G)
+                self.assertIsInstance(a, G)
                 self.assertEqual(a.x, 3)
 
                 things = "arguments" if sys.version_info >= (3, 11) else "parameters"
 
                 with self.assertRaisesRegex(TypeError, f'Too many {things}'):
                     G[int, str]
```

### Comparing `typing_extensions-4.6.1/src/typing_extensions.py` & `typing_extensions-4.6.2/src/typing_extensions.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import inspect
 import operator
 import sys
 import types as _types
 import typing
 import warnings
 
-
 __all__ = [
     # Super-special typing primitives.
     'Any',
     'ClassVar',
     'Concatenate',
     'Final',
     'LiteralString',
@@ -655,15 +654,17 @@
 
                 # ...or in annotations, if it is a sub-protocol.
                 annotations = getattr(base, '__annotations__', {})
                 if (
                     isinstance(annotations, collections.abc.Mapping)
                     and attr in annotations
                     and issubclass(other, (typing.Generic, _ProtocolMeta))
-                    and other._is_protocol
+                    # All subclasses of Generic have an _is_proto attribute on 3.8+
+                    # But not on 3.7
+                    and getattr(other, "_is_protocol", False)
                 ):
                     break
             else:
                 return NotImplemented
         return True
 
     def _check_proto_bases(cls):
@@ -2492,19 +2493,19 @@
             elif isinstance(__arg, type):
                 original_new = __arg.__new__
                 has_init = __arg.__init__ is not object.__init__
 
                 @functools.wraps(original_new)
                 def __new__(cls, *args, **kwargs):
                     warnings.warn(__msg, category=category, stacklevel=stacklevel + 1)
-                    # Mirrors a similar check in object.__new__.
-                    if not has_init and (args or kwargs):
-                        raise TypeError(f"{cls.__name__}() takes no arguments")
                     if original_new is not object.__new__:
                         return original_new(cls, *args, **kwargs)
+                    # Mirrors a similar check in object.__new__.
+                    elif not has_init and (args or kwargs):
+                        raise TypeError(f"{cls.__name__}() takes no arguments")
                     else:
                         return original_new(cls)
 
                 __arg.__new__ = staticmethod(__new__)
                 __arg.__deprecated__ = __new__.__deprecated__ = __msg
                 return __arg
             elif callable(__arg):
```

### Comparing `typing_extensions-4.6.1/PKG-INFO` & `typing_extensions-4.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typing_extensions
-Version: 4.6.1
+Version: 4.6.2
 Summary: Backported and Experimental Type Hints for Python 3.7+
 Keywords: annotations,backport,checker,checking,function,hinting,hints,type,typechecking,typehinting,typehints,typing
 Author-email: "Guido van Rossum, Jukka Lehtosalo, Łukasz Langa, Michael Lee" <levkivskyi@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

