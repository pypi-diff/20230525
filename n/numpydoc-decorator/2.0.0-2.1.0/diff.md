# Comparing `tmp/numpydoc_decorator-2.0.0.tar.gz` & `tmp/numpydoc_decorator-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpydoc_decorator-2.0.0.tar", max compression
+gzip compressed data, was "numpydoc_decorator-2.1.0.tar", max compression
```

## Comparing `numpydoc_decorator-2.0.0.tar` & `numpydoc_decorator-2.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-03-29 00:06:36.895305 numpydoc_decorator-2.0.0/LICENSE
--rw-r--r--   0        0        0     6671 2023-03-29 00:06:36.895305 numpydoc_decorator-2.0.0/README.md
--rw-r--r--   0        0        0       50 2023-03-29 00:06:36.895305 numpydoc_decorator-2.0.0/numpydoc_decorator/__init__.py
--rw-r--r--   0        0        0     3376 2023-03-29 00:06:36.895305 numpydoc_decorator-2.0.0/numpydoc_decorator/example.py
--rw-r--r--   0        0        0    22794 2023-03-29 00:06:36.895305 numpydoc_decorator-2.0.0/numpydoc_decorator/impl.py
--rw-r--r--   0        0        0      590 2023-03-29 00:09:42.503834 numpydoc_decorator-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     7159 1970-01-01 00:00:00.000000 numpydoc_decorator-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-25 21:39:31.767763 numpydoc_decorator-2.1.0/LICENSE
+-rw-r--r--   0        0        0     6671 2023-05-25 21:39:31.767763 numpydoc_decorator-2.1.0/README.md
+-rw-r--r--   0        0        0       50 2023-05-25 21:39:31.767763 numpydoc_decorator-2.1.0/numpydoc_decorator/__init__.py
+-rw-r--r--   0        0        0     3376 2023-05-25 21:39:31.767763 numpydoc_decorator-2.1.0/numpydoc_decorator/example.py
+-rw-r--r--   0        0        0    24355 2023-05-25 21:39:31.767763 numpydoc_decorator-2.1.0/numpydoc_decorator/impl.py
+-rw-r--r--   0        0        0      590 2023-05-25 21:42:10.484792 numpydoc_decorator-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7159 1970-01-01 00:00:00.000000 numpydoc_decorator-2.1.0/PKG-INFO
```

### Comparing `numpydoc_decorator-2.0.0/LICENSE` & `numpydoc_decorator-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `numpydoc_decorator-2.0.0/README.md` & `numpydoc_decorator-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `numpydoc_decorator-2.0.0/numpydoc_decorator/example.py` & `numpydoc_decorator-2.1.0/numpydoc_decorator/example.py`

 * *Files identical despite different names*

### Comparing `numpydoc_decorator-2.0.0/numpydoc_decorator/impl.py` & `numpydoc_decorator-2.1.0/numpydoc_decorator/impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import functools
+import operator
+import types as _types
+import typing
 from collections.abc import Generator, Iterable, Iterator, Sequence
 from inspect import Parameter, Signature, cleandoc, signature
 from textwrap import dedent, fill, indent
-from typing import Callable, Dict, List, Mapping, Optional
+from typing import Callable, Dict, ForwardRef, List, Mapping, Optional
 from typing import Sequence as SequenceType
 from typing import Tuple, Union
 
-from typing_extensions import Annotated, Literal
+from typing_extensions import Annotated, Literal, _AnnotatedAlias
 from typing_extensions import get_args as typing_get_args
 from typing_extensions import get_origin as typing_get_origin
-from typing_extensions import get_type_hints
 
 NoneType = type(None)
 
 try:
     # check whether numpy is installed
     import numpy
     from numpy.typing import ArrayLike, DTypeLike
@@ -29,52 +32,51 @@
 class DocumentationError(Exception):
     pass
 
 
 def punctuate(s: str):
     # This is possibly controversial, should we be enforcing punctuation? Will
     # do so for now, as it is easy to forget a full stop at the end of a
-    # piece of documentation, but looks better if punctuation is consistent.
+    # piece of documentation, and it looks better if punctuation is consistent.
     if s:
         s = s.strip()
         s = s[0].capitalize() + s[1:]
         if s[-1] not in ".!?:":
             s += "."
     return s
 
 
-# N.B., width of 72 is recommended in PEP8. It's also the default width
-# of the help tab in colab, so keeping under 72 ensures lines don't get
-# broken visually there, which can be confusing.
-
-
 def format_paragraph(s: str, width=72):
+    # N.B., width of 72 is recommended in PEP8. It's also the default width
+    # of the help tab in colab, so keeping under 72 ensures lines don't get
+    # broken visually there, which can be confusing.
+
     return fill(punctuate(dedent(s.strip(newline))), width=width) + newline
 
 
 def format_indented_paragraph(s: str):
-    # reduce width to account for indent
+    # Reduce width to 68 to account for indent.
     return indent(format_paragraph(s, width=68), prefix="    ")
 
 
 def format_paragraphs(s: str):
     prep = dedent(s.strip(newline))
     paragraphs = prep.split(newline + newline)
     docstring = ""
     for paragraph in paragraphs:
         if (
             paragraph.startswith(" ")
             or paragraph.startswith("..")
             or paragraph.startswith(">")
             or paragraph.startswith("[")
         ):
-            # leave this as-is
+            # assume code or similar, leave this as-is
             docstring += paragraph + newline + newline
         else:
-            # fill
+            # assume text, fill
             docstring += fill(punctuate(paragraph)) + newline + newline
     return docstring
 
 
 def format_indented_paragraphs(s: str):
     return indent(format_paragraphs(s), prefix="    ")
 
@@ -84,15 +86,15 @@
     # display parameters in order given in function signature
     for param_name, param in sig.parameters.items():
         if param_name == "self":
             # assume this is a method, don't document self parameter
             continue
 
         if param_name not in parameters:
-            # account for documentation of parameters and other parameters separately
+            # allow for documentation of parameters and other parameters separately
             continue
 
         # add parameter name, accounting for variable parameters
         if param.kind == Parameter.VAR_POSITIONAL:
             # *args
             docstring += "*" + param_name
 
@@ -102,15 +104,15 @@
 
         else:
             # standard parameter
             docstring += param_name + " :"
 
             # handle type annotation
             if param.annotation is not Parameter.empty:
-                docstring += " " + format_type(param.annotation)
+                docstring += " " + humanize_type(param.annotation)
 
             # handle default value
             if param.default is not Parameter.empty:
                 if param.annotation is not Parameter.empty:
                     docstring += ","
                 docstring += " optional"
                 if param.default is not None:
@@ -121,67 +123,84 @@
         param_doc = parameters[param_name]
         docstring += format_indented_paragraphs(param_doc).strip(newline)
         docstring += newline
 
     return docstring
 
 
-def format_type(t):
-    # This is probably a bit hacky, could be improved.
+def humanize_type(t):
+    # Here we attempt to provide some kind of human-readable representation
+    # of types used in type hints.
+
     t_orig = typing_get_origin(t)
     t_args = typing_get_args(t)
 
     if t == NoneType:
         return "None"
 
+    elif isinstance(t, str):
+        return t
+
+    elif isinstance(t, ForwardRef):
+        return t.__forward_arg__
+
     elif numpy and t == ArrayLike:
         return "array_like"
 
     elif numpy and t == Optional[ArrayLike]:
         return "array_like or None"
 
     elif numpy and t == DTypeLike:
         return "data-type"
 
     elif numpy and t == Optional[DTypeLike]:
         return "data-type or None"
 
-    # special handling for annotated types
     elif t_orig == Annotated:
+        # special handling for annotated types
         x = t_args[0]
-        return format_type(x)
+        return humanize_type(x)
 
-    # special handling for union types
     elif t_orig == Union and t_args:
-        return " or ".join([format_type(x) for x in t_args])
+        # special handling for union types
+        return " or ".join([humanize_type(x) for x in t_args])
 
     elif t_orig == Optional and t_args:
         x = t_args[0]
-        return format_type(x) + " or None"
+        return humanize_type(x) + " or None"
 
-    # humanize Literal types
     elif t_orig == Literal and t_args:
+        # humanize Literal types
         return "{" + ", ".join([repr(i) for i in t_args]) + "}"
 
-    # humanize sequence types
     elif t_orig in [list, List, Sequence, SequenceType] and t_args:
+        # humanize sequence types
         x = t_args[0]
-        return format_type(t_orig).lower() + " of " + format_type(x)
+        return humanize_type(t_orig).lower() + " of " + humanize_type(x)
 
-    # humanize variable length tuples
     elif t_orig in [tuple, Tuple] and t_args and Ellipsis in t_args:
+        # humanize variable length tuples
         x = t_args[0]
-        return "tuple of " + format_type(x)
+        return "tuple of " + humanize_type(x)
+
+    elif t_orig and t_args:
+        # deal with any other generic types
+        return (
+            f"{humanize_type(t_orig)}[{', '.join([humanize_type(t) for t in t_args])}]"
+        )
+
+    elif hasattr(t, "__name__"):
+        # assume some other kind of class
+        return t.__name__
 
     else:
+        # fallback
         s = repr(t)
-        # deal with built-in classes like int, etc.
-        if s.startswith("<class"):
-            s = t.__name__
-        s = s.replace("typing.", "")
+        if s.startswith("typing."):
+            s = s[7:]
         return s
 
 
 def format_returns(returns: Union[str, bool, Mapping[str, str]], sig: Signature):
     if returns is True:
         return format_returns_auto(sig.return_annotation)
     if isinstance(returns, str):
@@ -190,25 +209,25 @@
         return format_returns_named(returns, sig.return_annotation)
     else:
         raise TypeError("returns must be str or Mapping")
 
 
 def format_returns_auto(return_annotation):
     assert return_annotation is not Parameter.empty
-    docstring = format_type(return_annotation) + newline
+    docstring = humanize_type(return_annotation) + newline
     return docstring
 
 
 def format_returns_unnamed(returns: str, return_annotation):
     if return_annotation is Parameter.empty:
         # just assume it's a description of the return value
         docstring = format_paragraph(returns)
     else:
         # provide the type
-        docstring = format_type(return_annotation) + newline
+        docstring = humanize_type(return_annotation) + newline
         docstring += format_indented_paragraph(returns)
     docstring += newline
     return docstring
 
 
 def format_returns_named(returns: Mapping[str, str], return_annotation):
     docstring = ""
@@ -243,15 +262,15 @@
 
     for (return_name, return_doc), return_type in zip(returns.items(), return_types):
         if return_type is Parameter.empty:
             docstring += return_name.strip() + " :"
         else:
             if isinstance(return_name, str):
                 docstring += return_name.strip() + " : "
-            docstring += format_type(return_type)
+            docstring += humanize_type(return_type)
         docstring += newline
         if isinstance(return_doc, str):
             docstring += format_indented_paragraph(return_doc)
     docstring += newline
 
     return docstring
 
@@ -390,14 +409,37 @@
         return t_args[0]
     if t_orig == Union and len(t_args) == 2 and t_args[1] == NoneType:
         # compatibility for PY37
         return t_args[0]
     return t
 
 
+def strip_extras(t):
+    """Strips Annotated from a given type. Borrowed from typing_extensions."""
+    if isinstance(t, _AnnotatedAlias):
+        return strip_extras(t.__origin__)
+    if isinstance(t, typing._GenericAlias):
+        stripped_args = tuple(strip_extras(a) for a in t.__args__)
+        if stripped_args == t.__args__:
+            return t
+        return t.copy_with(stripped_args)
+    if hasattr(_types, "GenericAlias") and isinstance(t, _types.GenericAlias):
+        stripped_args = tuple(strip_extras(a) for a in t.__args__)
+        if stripped_args == t.__args__:
+            return t
+        return _types.GenericAlias(t.__origin__, stripped_args)
+    if hasattr(_types, "UnionType") and isinstance(t, _types.UnionType):
+        stripped_args = tuple(strip_extras(a) for a in t.__args__)
+        if stripped_args == t.__args__:
+            return t
+        return functools.reduce(operator.or_, stripped_args)
+
+    return t
+
+
 def get_annotated_doc(t, default=None):
     t_orig = typing_get_origin(t)
     t_args = typing_get_args(t)
     if t_orig == Annotated:
         # assume first annotation provides documentation
         x = t_args[1]
         if isinstance(x, str):
@@ -606,15 +648,18 @@
         # final cleanup
         docstring = newline + cleandoc(docstring) + newline
 
         # attach the docstring
         f.__doc__ = docstring
 
         # strip Annotated types, these are unreadable in built-in help() function
-        f.__annotations__ = get_type_hints(f, include_extras=include_extras)
+        if not include_extras:
+            f.__annotations__ = {
+                k: strip_extras(v) for k, v in f.__annotations__.items()
+            }
 
         return f
 
     return decorator
 
 
 # eat our own dogfood
```

### Comparing `numpydoc_decorator-2.0.0/pyproject.toml` & `numpydoc_decorator-2.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numpydoc_decorator"
-version = "2.0.0"
+version = "2.1.0"
 description = ""
 authors = ["Alistair Miles <alimanfoo@googlemail.com>"]
 readme = "README.md"
 packages = [{include = "numpydoc_decorator"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `numpydoc_decorator-2.0.0/PKG-INFO` & `numpydoc_decorator-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numpydoc-decorator
-Version: 2.0.0
+Version: 2.1.0
 Summary: 
 Author: Alistair Miles
 Author-email: alimanfoo@googlemail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

