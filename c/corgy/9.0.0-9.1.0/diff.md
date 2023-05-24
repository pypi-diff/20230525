# Comparing `tmp/corgy-9.0.0.tar.gz` & `tmp/corgy-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corgy-9.0.0.tar", max compression
+gzip compressed data, was "corgy-9.1.0.tar", max compression
```

## Comparing `corgy-9.0.0.tar` & `corgy-9.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    31468 2023-05-17 09:39:56.515288 corgy-9.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1072 2023-05-17 09:39:56.515288 corgy-9.0.0/LICENSE
--rw-r--r--   0        0        0     4196 2023-05-17 09:39:56.515288 corgy-9.0.0/README.md
--rw-r--r--   0        0        0      468 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/__init__.py
--rw-r--r--   0        0        0     2329 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/_actions.py
--rw-r--r--   0        0        0      505 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/_annotations.py
--rw-r--r--   0        0        0    49963 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/_corgy.py
--rw-r--r--   0        0        0     3202 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/_corgychecker.py
--rw-r--r--   0        0        0     6237 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/_corgyparser.py
--rw-r--r--   0        0        0    36993 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/_helpfmt.py
--rw-r--r--   0        0        0    18742 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/_meta.py
--rw-r--r--   0        0        0       64 2023-05-17 09:40:32.351710 corgy-9.0.0/corgy/_version.py
--rw-r--r--   0        0        0        0 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/py.typed
--rw-r--r--   0        0        0     1598 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/types/__init__.py
--rw-r--r--   0        0        0     2382 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/types/_expand.py
--rw-r--r--   0        0        0     3750 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/types/_initargs.py
--rw-r--r--   0        0        0     2777 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/types/_inputfile.py
--rw-r--r--   0        0        0     5464 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/types/_keyvaluepairs.py
--rw-r--r--   0        0        0     5271 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/types/_outputfile.py
--rw-r--r--   0        0        0     9846 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/types/_subclass.py
--rw-r--r--   0        0        0    35396 2023-05-17 09:39:56.515288 corgy-9.0.0/docs/corgy.md
--rw-r--r--   0        0        0    11884 2023-05-17 09:39:56.515288 corgy-9.0.0/docs/corgy.types.md
--rw-r--r--   0        0        0      132 2023-05-17 09:39:56.515288 corgy-9.0.0/docs/index.md
--rw-r--r--   0        0        0     2679 2023-05-17 09:40:32.351710 corgy-9.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/__init__.py
--rw-r--r--   0        0        0    90889 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/test_corgy.py
--rw-r--r--   0        0        0     4240 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/test_corgychecker.py
--rw-r--r--   0        0        0    16681 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/test_corgyparser.py
--rw-r--r--   0        0        0      800 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/test_doctests.py
--rw-r--r--   0        0        0    47095 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/test_helpfmt.py
--rw-r--r--   0        0        0        0 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/types/__init__.py
--rw-r--r--   0        0        0      328 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/types/_pklclasses.py
--rw-r--r--   0        0        0     2002 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/types/_specialtmps.py
--rw-r--r--   0        0        0     3356 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/types/_test_file.py
--rw-r--r--   0        0        0     2678 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/types/test_initargs.py
--rw-r--r--   0        0        0     2496 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/types/test_inputfiles.py
--rw-r--r--   0        0        0     5443 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/types/test_keyvaluepairs.py
--rw-r--r--   0        0        0     5122 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/types/test_outputfiles.py
--rw-r--r--   0        0        0     7082 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/types/test_subclass.py
--rw-r--r--   0        0        0     5497 1970-01-01 00:00:00.000000 corgy-9.0.0/PKG-INFO
+-rw-r--r--   0        0        0    31893 2023-05-24 21:57:06.521003 corgy-9.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1072 2023-05-24 21:57:06.521003 corgy-9.1.0/LICENSE
+-rw-r--r--   0        0        0     4196 2023-05-24 21:57:06.521003 corgy-9.1.0/README.md
+-rw-r--r--   0        0        0      468 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/__init__.py
+-rw-r--r--   0        0        0     2329 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/_actions.py
+-rw-r--r--   0        0        0      505 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/_annotations.py
+-rw-r--r--   0        0        0    53646 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/_corgy.py
+-rw-r--r--   0        0        0     3202 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/_corgychecker.py
+-rw-r--r--   0        0        0     6237 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/_corgyparser.py
+-rw-r--r--   0        0        0    36993 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/_helpfmt.py
+-rw-r--r--   0        0        0    19746 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/_meta.py
+-rw-r--r--   0        0        0       64 2023-05-24 21:57:45.793051 corgy-9.1.0/corgy/_version.py
+-rw-r--r--   0        0        0        0 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/py.typed
+-rw-r--r--   0        0        0     1598 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/types/__init__.py
+-rw-r--r--   0        0        0     2382 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/types/_expand.py
+-rw-r--r--   0        0        0     3750 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/types/_initargs.py
+-rw-r--r--   0        0        0     2777 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/types/_inputfile.py
+-rw-r--r--   0        0        0     5464 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/types/_keyvaluepairs.py
+-rw-r--r--   0        0        0     5271 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/types/_outputfile.py
+-rw-r--r--   0        0        0     9846 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/types/_subclass.py
+-rw-r--r--   0        0        0    36201 2023-05-24 21:57:06.521003 corgy-9.1.0/docs/corgy.md
+-rw-r--r--   0        0        0    11884 2023-05-24 21:57:06.521003 corgy-9.1.0/docs/corgy.types.md
+-rw-r--r--   0        0        0      132 2023-05-24 21:57:06.521003 corgy-9.1.0/docs/index.md
+-rw-r--r--   0        0        0     2697 2023-05-24 21:57:45.793051 corgy-9.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 21:57:06.521003 corgy-9.1.0/tests/__init__.py
+-rw-r--r--   0        0        0    94529 2023-05-24 21:57:06.521003 corgy-9.1.0/tests/test_corgy.py
+-rw-r--r--   0        0        0     4753 2023-05-24 21:57:06.521003 corgy-9.1.0/tests/test_corgychecker.py
+-rw-r--r--   0        0        0    20305 2023-05-24 21:57:06.521003 corgy-9.1.0/tests/test_corgyparser.py
+-rw-r--r--   0        0        0      800 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/test_doctests.py
+-rw-r--r--   0        0        0    47095 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/test_helpfmt.py
+-rw-r--r--   0        0        0        0 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/types/__init__.py
+-rw-r--r--   0        0        0      328 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/types/_pklclasses.py
+-rw-r--r--   0        0        0     2002 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/types/_specialtmps.py
+-rw-r--r--   0        0        0     3356 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/types/_test_file.py
+-rw-r--r--   0        0        0     2678 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/types/test_initargs.py
+-rw-r--r--   0        0        0     2496 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/types/test_inputfiles.py
+-rw-r--r--   0        0        0     5443 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/types/test_keyvaluepairs.py
+-rw-r--r--   0        0        0     5122 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/types/test_outputfiles.py
+-rw-r--r--   0        0        0     7082 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/types/test_subclass.py
+-rw-r--r--   0        0        0     5497 1970-01-01 00:00:00.000000 corgy-9.1.0/PKG-INFO
```

### Comparing `corgy-9.0.0/CHANGELOG.md` & `corgy-9.1.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+## [9.1.0](https://github.com/jayanthkoushik/corgy/compare/v9.0.0...v9.1.0) (2023-05-24)
+
+
+### Features
+
+* add support for `Self` type annotations ([b33ec24](https://github.com/jayanthkoushik/corgy/commit/b33ec24ad762c1dd0655ad4a5af847eb16f15b55))
+
+
+### Bug Fixes
+
+* prioritize custom parsers in `Corgy.add_args_to_parser` ([5cf047f](https://github.com/jayanthkoushik/corgy/commit/5cf047fd6ebb1f1b385ab01587355af680d7002d))
+
 ## [9.0.0](https://github.com/jayanthkoushik/corgy/compare/v8.1.2...v9.0.0) (2023-05-17)
 
 
 ### ⚠ BREAKING CHANGES
 
 * `Corgy.add_args_to_parser` no longer uses `store_`
 actions for types with a single choice defined using `__choices__`. Only
```

### Comparing `corgy-9.0.0/LICENSE` & `corgy-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/README.md` & `corgy-9.1.0/README.md`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/corgy/_actions.py` & `corgy-9.1.0/corgy/_actions.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/corgy/_corgy.py` & `corgy-9.1.0/corgy/_corgy.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,28 +3,44 @@
 import argparse
 import sys
 from argparse import (
     _ActionsContainer,
     _StoreConstAction,
     _StoreFalseAction,
     _StoreTrueAction,
-    Action,
     ArgumentParser,
 )
 from collections import defaultdict
 from collections.abc import Sequence as AbstractSequence
+from dataclasses import dataclass
 from functools import partial
 from importlib import import_module
-from typing import Any, Callable, Dict, IO, Mapping, Optional, Type, TypeVar, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    IO,
+    Mapping,
+    Optional,
+    Sequence,
+    Type,
+    TypeVar,
+    Union,
+)
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
+
 from ._actions import BooleanOptionalAction, OptionalTypeAction
 from ._corgyparser import CorgyParserAction
 from ._helpfmt import CorgyHelpFormatter
 from ._meta import (
     check_val_type,
     CorgyMeta,
     get_concrete_collection_type,
@@ -434,14 +450,42 @@
             ...
         ValueError: error setting `x`: invalid value for type '<class 'T'>': 3:
         expected one of: (1, 2)
 
     Note that choices specified in this way are not type-checked to ensure that they
     match the argument type; in the above example, `__choices__` could be set to
     `(1, "2")`.
+
+    *Self*
+    `Corgy` classes can have attributes of their own type, annotated using
+    `typing.Self`.
+
+        >>> if sys.version_info >= (3, 11):
+        ...     from typing import Self
+        ... else:
+        ...     from typing_extensions import Self
+
+        >>> class C(Corgy):
+        ...     x: int
+        ...     c: Self
+
+        >>> c = C(x=1)
+        >>> c.c = C(x=2)
+        >>> c
+        C(x=1, c=C(x=2))
+
+        >>> class D(C):
+        ...     ...
+
+        >>> c.c = D(x=3)  # doctest: +NORMALIZE_WHITESPACE
+        Traceback (most recent call last):
+            ...
+        ValueError: error setting `c`: invalid value for type 'Self (bound to
+        <class 'C'>)': D(x=3)
+
     """
 
     @classmethod
     def add_args_to_parser(
         cls,
         parser: _ActionsContainer,
         name_prefix: str = "",
@@ -465,14 +509,19 @@
                 individual values using the same syntax as for `Corgy.from_dict`.
 
         Type annotations control how attributes are added to the parser. A number of
         special annotations are parsed and stripped from attribute types to determine
         the parameters for calling `ArgumentParser.add_argument`. These special
         annotations are described below.
 
+        Note: `add_args_to_parser` cannot be used if the type annotation for any
+        attribute of the class includes `Self`, unless a custom parser is defined
+        for such attributes. See docs for `corgyparser` on how to define custom
+        parsers.
+
         *Annotated*
         `typing.Annotated` can be used to add a help message for the argument::
 
             >>> import argparse
             >>> from argparse import ArgumentParser
             >>> from corgy import CorgyHelpFormatter
 
@@ -720,45 +769,216 @@
             if ":" in _k:
                 _grp_name, _var_name = _k.split(":")
                 group_arg_defaults[_grp_name][_var_name] = _v
             elif _k not in cls.__annotations__:
                 raise ValueError(f"default value for unknown argument: `{_k}`")
 
         required_attrs = getattr(cls, "__required")
+        custom_flags = getattr(cls, "__flags")
+        custom_parsers = getattr(cls, "__parsers")
+
+        @dataclass
+        class _Arg:
+            name: str
+            required: Optional[bool] = None
+            positional: Optional[bool] = None
+            dest: Optional[str] = None
+            flags: Optional[Sequence[str]] = None
+            help: Optional[str] = None
+            nargs: Union[int, Literal["+", "*"], None] = None
+            action: Optional[Type[argparse.Action]] = None
+            choices: Optional[Sequence[Any]] = None
+            metavar: Optional[str] = None
+            add_type: Optional[Any] = None
+            const: Optional[Any] = None
+
+            def get_add_kwargs(self) -> Dict[str, Any]:
+                assert self.required is not None
+                assert self.positional is not None
+                assert self.dest is not None
+                kwargs: Dict[str, Any] = {}
+                if (not self.positional) and (self.name in custom_flags):
+                    kwargs["dest"] = self.dest
+                if self.help is not None:
+                    kwargs["help"] = self.help
+                if self.nargs is not None:
+                    kwargs["nargs"] = self.nargs
+                if self.action is not None:
+                    kwargs["action"] = self.action
+                if self.choices is not None:
+                    kwargs["choices"] = self.choices
+
+                if self.name in base_defaults:
+                    kwargs["default"] = base_defaults[self.name]
+                elif self.required and not self.positional:
+                    kwargs["required"] = True
+                elif not self.positional:
+                    kwargs["default"] = argparse.SUPPRESS
+
+                if self.metavar is not None:
+                    kwargs["metavar"] = self.metavar
+                if self.add_type is not None:
+                    kwargs["type"] = self.add_type
+                if self.const is not None:
+                    kwargs["const"] = self.const
+
+                return kwargs
+
+            def process_optional(self, type_) -> Any:
+                if is_optional_type(type_):
+                    self.action = OptionalTypeAction
+                    return type_.__args__[0]
+                return type_
+
+            def process_collection(self, type_) -> Any:
+                _col_type = get_concrete_collection_type(type_)
+                if _col_type is not None:
+                    if (
+                        not hasattr(type_, "__args__")
+                        or not type_.__args__
+                        or isinstance(type_.__args__[0], TypeVar)
+                    ):
+                        raise TypeError(
+                            f"`{self.name}` is a collection, but has no type arguments:"
+                            f" use `{type_}[<types>]"
+                        )
+                    if len(type_.__args__) == 1:
+                        self.nargs = "*"
+                    elif len(type_.__args__) == 2 and type_.__args__[1] is Ellipsis:
+                        # `...` is used to represent non-empty collections, e.g.,
+                        # `Sequence[int, ...]`.
+                        self.nargs = "+"
+                    else:
+                        # Ensure single type.
+                        if any(_a != type_.__args__[0] for _a in type_.__args__[1:]):
+                            raise TypeError(
+                                f"`{self.name}` has unsupported type `{type_}`: only"
+                                f" single-type collections are supported"
+                            )
+                        self.nargs = len(type_.__args__)
+                    return type_.__args__[0]
+                return type_
+
+            def process_choices(self, type_) -> Any:
+                _is_literal_type = is_literal_type(type_)
+                if _is_literal_type:
+                    # Determine if the first choice has `__bases__`, in which case
+                    # the first base class is the type for the argument.
+                    try:
+                        c0_type = type_.__args__[0].__bases__[0]
+                    except AttributeError:
+                        c0_type = type(type_.__args__[0])
+                        f_check_type: Callable[[Any, Any], bool] = isinstance
+                    else:
+                        f_check_type = issubclass
+
+                    # All choices must be of the same type.
+                    if any(not f_check_type(_a, c0_type) for _a in type_.__args__[1:]):
+                        raise TypeError(
+                            f"choices for `{self.name}` not all of type `{c0_type}`: "
+                            f"`{type_.__args__}`"
+                        )
+                    self.choices = type_.__args__
+
+                    # Convert single choice attributes to `store_*` actions.
+                    if (
+                        self.choices is not None
+                        and len(self.choices) == 1
+                        and self.nargs is None
+                        and self.action is None
+                    ):
+                        _choice = self.choices[0]
+                        if _choice is True:
+                            self.action = _StoreTrueAction
+                        elif _choice is False:
+                            self.action = _StoreFalseAction
+                        else:
+                            self.action = _StoreConstAction
+                            self.const = _choice
+                        self.choices = None
+                        return None
+                    return c0_type
+
+                if hasattr(type_, "__choices__"):
+                    self.choices = type_.__choices__
+
+                return type_
 
         for var_name, var_type in cls.attrs().items():
-            var_flags = getattr(cls, "__flags").get(
+            var_arg = _Arg(var_name)
+            var_arg.help = getattr(
+                cls, var_name
+            ).__doc__  # doc is stored in the property
+            var_arg.required = (
+                var_name not in base_defaults and var_name in required_attrs
+            )
+
+            # Determine add flags.
+            var_arg.flags = custom_flags.get(
                 var_name, [f"--{var_name.replace('_', '-')}"]
             )
+            assert var_arg.flags is not None
             if name_prefix:
-                var_flags = [
+                var_arg.flags = [
                     f"--{name_prefix.replace('_', '-')}:{flag.lstrip('-')}"
-                    for flag in var_flags
+                    for flag in var_arg.flags
                 ]
-                var_dest = f"{name_prefix}:{var_name}"
+                var_arg.dest = f"{name_prefix}:{var_name}"
             else:
-                var_dest = var_name
+                var_arg.dest = var_name
 
-            if not any(_flag.startswith("-") for _flag in var_flags):
+            # Determine if argument is positional.
+            if not any(_flag.startswith("-") for _flag in var_arg.flags):
                 # Note: the flags cannot be passed to `add_argument` with `dest` set
                 # to `var_name` since `argparse` will raise an error for passing `dest`
                 # twice (for positional arguments, `argparse` uses the flag to infer the
                 # `dest`).
-                var_flags = [var_name]
-                var_positional = True
-            elif all(_flag.startswith("-") for _flag in var_flags):
-                var_positional = False
+                var_arg.flags = [var_name]
+                var_arg.positional = True
+            elif all(_flag.startswith("-") for _flag in var_arg.flags):
+                var_arg.positional = False
             else:
                 raise TypeError(
                     f"inconsistent positional/optional flags for {var_name}: "
-                    f"{var_flags}"
+                    f"{var_arg.flags}"
                 )
 
-            var_help = getattr(cls, var_name).__doc__  # doc is stored in the property
+            ###################################################################
+            # Check if the variable has a custom parser.
+            if var_name in custom_parsers:
+                _var_parser = custom_parsers[var_name]
+                _var_base_type = var_type
+                # Extract choices if present.
+                if is_literal_type(var_type):
+                    _var_choices = var_type.__args__
+                    try:
+                        _var_base_type = _var_choices[0].__bases__[0]
+                    except AttributeError:
+                        _var_base_type = type(_var_choices[0])
+                elif hasattr(var_type, "__choices__"):
+                    _var_choices = var_type.__choices__
+                else:
+                    _var_choices = None
+
+                var_arg.action = partial(
+                    CorgyParserAction, _var_parser, _var_choices  # type: ignore
+                )
+                var_arg.add_type = str
+                var_arg.nargs = getattr(_var_parser, "__nargs__", None)
+                try:
+                    var_arg.metavar = _var_parser.__metavar__
+                except AttributeError:
+                    try:
+                        var_arg.metavar = _var_base_type.__metavar__
+                    except AttributeError:
+                        pass
+                parser.add_argument(*var_arg.flags, **var_arg.get_add_kwargs())
+                continue
 
+            ###################################################################
             # Check if the variable is also `Corgy` type.
             if type(var_type) is type(cls):
                 # Create an argument group using `<var_type>`.
                 # If there is a default value, pass it using `**defaults`.
                 if var_name in base_defaults:
                     try:
                         grp_defaults = base_defaults[var_name].as_dict()
@@ -772,174 +992,47 @@
                 # Update defaults with any values specified individually.
                 grp_defaults.update(group_arg_defaults.get(var_name, {}))
 
                 grp_parser: _ActionsContainer
                 if flatten_subgrps:
                     grp_parser = base_parser
                 else:
-                    grp_parser = base_parser.add_argument_group(var_dest, var_help)
-                var_type.add_args_to_parser(grp_parser, var_dest, True, grp_defaults)
-                continue
-
-            var_action: Optional[Type[Action]] = None
-
-            # Check if the variable is required on the command line.
-            var_required = var_name not in base_defaults and var_name in required_attrs
-
-            # Check if the variable can be `None`.
-            if is_optional_type(var_type):
-                var_base_type = var_type.__args__[0]
-                var_action = OptionalTypeAction
-            else:
-                var_base_type = var_type
-
-            # Check if the variable is a collection.
-            var_nargs: Union[int, Literal["+", "*", "?"], None] = None
-            _col_type = get_concrete_collection_type(var_base_type)
-            if _col_type is not None:
-                if (
-                    not hasattr(var_base_type, "__args__")
-                    or not var_base_type.__args__
-                    or isinstance(var_base_type.__args__[0], TypeVar)
-                ):
-                    raise TypeError(
-                        f"`{var_name}` is a collection, but has no type arguments: "
-                        f"use `{var_base_type}[<types>]"
-                    )
-                if len(var_base_type.__args__) == 1:
-                    var_nargs = "*"
-                elif (
-                    len(var_base_type.__args__) == 2
-                    and var_base_type.__args__[1] is Ellipsis
-                ):
-                    # `...` is used to represent non-empty collections, e.g.,
-                    # `Sequence[int, ...]`.
-                    var_nargs = "+"
-                else:
-                    # Ensure single type.
-                    if any(
-                        _a != var_base_type.__args__[0]
-                        for _a in var_base_type.__args__[1:]
-                    ):
-                        raise TypeError(
-                            f"`{var_name}` has unsupported type `{var_base_type}`: only"
-                            f" single-type collections are supported"
-                        )
-                    var_nargs = len(var_base_type.__args__)
-                var_base_type = var_base_type.__args__[0]
-
-            # Check if the variable has choices.
-            _is_literal_type = is_literal_type(var_base_type)
-            if _is_literal_type:
-                # Determine if the first choice has `__bases__`, in which case
-                # the first base class is the type for the argument.
-                try:
-                    c0_type = var_base_type.__args__[0].__bases__[0]
-                except AttributeError:
-                    c0_type = type(var_base_type.__args__[0])
-                    f_check_type: Callable[[Any, Any], bool] = isinstance
-                else:
-                    f_check_type = issubclass
-
-                # All choices must be of the same type.
-                if any(
-                    not f_check_type(_a, c0_type) for _a in var_base_type.__args__[1:]
-                ):
-                    raise TypeError(
-                        f"choices for `{var_name}` not all of type `{c0_type}`: "
-                        f"`{var_base_type.__args__}`"
+                    grp_parser = base_parser.add_argument_group(
+                        var_arg.dest, var_arg.help
                     )
-                var_choices = var_base_type.__args__
-                var_base_type = c0_type
-            elif hasattr(var_base_type, "__choices__"):
-                var_choices = var_base_type.__choices__
-            else:
-                var_choices = None
-
-            var_type_metavar: Optional[str] = getattr(
-                var_base_type, "__metavar__", None
-            )
-
-            # Convert single choice attributes to `store_*` actions.
-            if (
-                var_choices is not None
-                and len(var_choices) == 1
-                and var_nargs is None
-                and var_action is None
-                and _is_literal_type
-            ):
-                _choice = var_choices[0]
-                if _choice is True:
-                    var_action = _StoreTrueAction
-                    var_const = None
-                elif _choice is False:
-                    var_action = _StoreFalseAction
-                    var_const = None
-                else:
-                    var_action = _StoreConstAction
-                    var_const = _choice
-                var_choices = None
-                var_base_type = None
-            else:
-                var_const = None
+                var_type.add_args_to_parser(
+                    grp_parser, var_arg.dest, True, grp_defaults
+                )
+                continue
 
+            ###################################################################
             # Check if the variable is boolean. Boolean variables are converted to
-            # `--<var-name>`/`--no-<var-name>` arguments.
-            if (
-                var_base_type is bool
-                and var_nargs is None
-                and var_action is None
-                and var_choices is None
-                and not var_positional
-            ):
-                var_action = BooleanOptionalAction
+            # `--<var-name>`/`--no-<var-name>` arguments (if not positional).
+            if var_type is bool:
+                var_arg.add_type = bool
+                if not var_arg.positional:
+                    var_arg.action = BooleanOptionalAction
+                parser.add_argument(*var_arg.flags, **var_arg.get_add_kwargs())
+                continue
 
-            # Check if the variable has a custom parser.
-            _parsers = getattr(cls, "__parsers")
-            if var_name in _parsers:
-                _var_parser = _parsers[var_name]
-                var_action = partial(
-                    CorgyParserAction, _var_parser, var_choices  # type: ignore
+            ###################################################################
+            # Process annotations.
+            var_base_type = var_type
+            var_base_type = var_arg.process_optional(var_base_type)
+            var_base_type = var_arg.process_collection(var_base_type)
+            var_base_type = var_arg.process_choices(var_base_type)
+
+            if var_base_type is Self:
+                raise TypeError(
+                    "'add_args_to_parser' cannot be used with 'Self' type present"
                 )
-                var_add_type = str
-                var_choices = None  # handled by the parser
-                var_nargs = getattr(_var_parser, "__nargs__", None)
-                _parser_metavar = getattr(_var_parser, "__metavar__", None)
-                if _parser_metavar is not None:
-                    var_type_metavar = _parser_metavar
-            else:
-                var_add_type = var_base_type
 
-            # Add the variable to the parser.
-            _kwargs: Dict[str, Any] = {}
-            if var_name in getattr(cls, "__flags") and not var_positional:
-                _kwargs["dest"] = var_dest
-            if var_help is not None:
-                _kwargs["help"] = var_help
-            if var_nargs is not None:
-                _kwargs["nargs"] = var_nargs
-            if var_action is not None:
-                _kwargs["action"] = var_action
-            if var_choices is not None:
-                _kwargs["choices"] = var_choices
-
-            if var_name in base_defaults:
-                _kwargs["default"] = base_defaults[var_name]
-            elif var_required and not var_positional:
-                _kwargs["required"] = True
-            elif not var_positional:
-                _kwargs["default"] = argparse.SUPPRESS
-
-            if var_type_metavar is not None:
-                _kwargs["metavar"] = var_type_metavar
-            if var_add_type is not None:
-                _kwargs["type"] = var_add_type
-            if var_const is not None:
-                _kwargs["const"] = var_const
-            parser.add_argument(*var_flags, **_kwargs)
+            var_arg.metavar = getattr(var_base_type, "__metavar__", None)
+            var_arg.add_type = var_base_type
+            parser.add_argument(*var_arg.flags, **var_arg.get_add_kwargs())
 
     def __init__(self, **args):
         if self.__class__ is Corgy:
             raise TypeError("`Corgy` is an abstract class and cannot be instantiated")
 
         setattr(self, f"_{self.__class__.__name__.lstrip('_')}__frozen", False)
 
@@ -1067,15 +1160,15 @@
             try:
                 attr_val = getattr(self, attr_name)
             except AttributeError:
                 continue
 
             if recursive:
                 attr_val = dictify_corgys(attr_val)
-                if flatten and isinstance(attr_type, CorgyMeta):
+                if flatten and (isinstance(attr_type, CorgyMeta) or attr_type is Self):
                     for _k, _v in attr_val.items():
                         _flat_key = f"{attr_name}:{_k}"
                         self_dict[_flat_key] = _v
                     continue
 
             self_dict[attr_name] = attr_val
 
@@ -1164,14 +1257,15 @@
             if arg_name in cls_attrs:
                 try:
                     main_args_map[arg_name] = check_val_type(
                         arg_val,
                         cls_attrs[arg_name],
                         try_cast,
                         try_load_corgy_dicts=True,
+                        self_type=cls,
                     )
                 except ValueError as e:
                     raise ValueError(f"error setting `{arg_name}`: {e}") from None
         return cls(**main_args_map)
 
     def load_dict(
         self, d: Dict[str, Any], try_cast: bool = False, strict: bool = False
@@ -1252,15 +1346,19 @@
                 except AttributeError:
                     setattr(self, arg_name, arg_type.from_dict(arg_new_val))
                 else:
                     arg_obj.load_dict(arg_new_val, try_cast, strict)
             else:
                 try:
                     arg_new_val = check_val_type(
-                        arg_new_val, arg_type, try_cast, try_load_corgy_dicts=True
+                        arg_new_val,
+                        arg_type,
+                        try_cast,
+                        try_load_corgy_dicts=True,
+                        self_type=type(self),
                     )
                 except ValueError as e:
                     raise ValueError(f"error setting `{arg_name}`: {e}") from None
                 setattr(self, arg_name, arg_new_val)
 
     @classmethod
     def parse_from_cmdline(
```

### Comparing `corgy-9.0.0/corgy/_corgychecker.py` & `corgy-9.1.0/corgy/_corgychecker.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/corgy/_corgyparser.py` & `corgy-9.1.0/corgy/_corgyparser.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/corgy/_helpfmt.py` & `corgy-9.1.0/corgy/_helpfmt.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/corgy/_meta.py` & `corgy-9.1.0/corgy/_meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 from __future__ import annotations
 
 import sys
 from collections.abc import Sequence as AbstractSequence
 from contextlib import suppress
 from typing import Any, ClassVar, List, Optional, Sequence, Set, Tuple, Union
 
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
+
 if sys.version_info >= (3, 10):
     from types import UnionType
 
 if sys.version_info >= (3, 9):
     from typing import get_type_hints, Literal
 else:
     from typing_extensions import Literal, get_type_hints
@@ -58,15 +63,32 @@
 
 
 def is_literal_type(t) -> bool:
     """Check if the argument is `Literal`."""
     return hasattr(t, "__origin__") and t.__origin__ is Literal
 
 
-def check_val_type(_val, _type, try_cast=False, try_load_corgy_dicts=False):
+def check_val_type(
+    _val, _type, try_cast=False, try_load_corgy_dicts=False, self_type=None
+):
+    if _type is Self:
+        if self_type is None:
+            raise TypeError(
+                f"error type checking '{_val!r}': "
+                f"'Self' not allowed in this context"
+            )
+        _type = self_type
+        instance_check = (
+            lambda _v, _t: type(_v) is _t  # pylint: disable=unidiomatic-typecheck
+        )
+        inst_check_err_type_str = f"Self (bound to {self_type})"
+    else:
+        instance_check = isinstance
+        inst_check_err_type_str = str(_type)
+
     _coll_type = get_concrete_collection_type(_type)
     if _coll_type is not None:
         if not isinstance(_val, _coll_type):
             _cast_type = _coll_type if _coll_type is not AbstractSequence else list
             _cast = False
             if try_cast:
                 try:
@@ -90,48 +112,60 @@
 
         _cast_val_is = []
         if len(_base_types) == 1:
             # All items in `_val` should match the base type.
             for _val_i in _val:
                 _cast_val_is.append(
                     check_val_type(
-                        _val_i, _base_types[0], try_cast, try_load_corgy_dicts
+                        _val_i,
+                        _base_types[0],
+                        try_cast,
+                        try_load_corgy_dicts,
+                        self_type,
                     )
                 )
         elif len(_base_types) == 2 and _base_types[1] is Ellipsis:
             # Same as the previous condition, but `_val` must be non-empty.
             if not _val:
                 raise ValueError(f"expected non-empty collection for type '{_type}'")
             for _val_i in _val:
                 _cast_val_is.append(
                     check_val_type(
-                        _val_i, _base_types[0], try_cast, try_load_corgy_dicts
+                        _val_i,
+                        _base_types[0],
+                        try_cast,
+                        try_load_corgy_dicts,
+                        self_type,
                     )
                 )
         else:
             # There should be a one-to-one correspondence between items in `_val` and
             # items in `_type`.
             if len(_val) != len(_base_types):
                 raise ValueError(
                     f"invalid value for type '{_type}': {_val!r}: "
                     f"expected exactly '{len(_base_types)}' elements"
                 )
             for _val_i, _base_type_i in zip(_val, _base_types):
                 _cast_val_is.append(
-                    check_val_type(_val_i, _base_type_i, try_cast, try_load_corgy_dicts)
+                    check_val_type(
+                        _val_i, _base_type_i, try_cast, try_load_corgy_dicts, self_type
+                    )
                 )
 
         _val = _cast_type(_cast_val_is)
         return _val
 
     if is_optional_type(_type):
         if _val is None:
             return None
         _base_type = _type.__args__[0]
-        return check_val_type(_val, _base_type, try_cast, try_load_corgy_dicts)
+        return check_val_type(
+            _val, _base_type, try_cast, try_load_corgy_dicts, self_type
+        )
 
     if is_literal_type(_type):
         if not hasattr(_type, "__args__") or _val not in _type.__args__:
             raise ValueError(f"invalid value for type '{_type}': {_val!r}")
         return _val
 
     if hasattr(_type, "__choices__"):
@@ -142,15 +176,15 @@
             )
         return _val
 
     if try_load_corgy_dicts and isinstance(_val, dict) and isinstance(_type, CorgyMeta):
         return _type.from_dict(_val, try_cast)
 
     try:
-        _is_inst = isinstance(_val, _type)
+        _is_inst = instance_check(_val, _type)
     except TypeError:
         raise ValueError(f"invalid type: {_type}") from None
 
     if _is_inst:
         return _val
 
     _cast = False
@@ -158,15 +192,17 @@
         try:
             _val = _type(_val)
         except TypeError:
             ...
         else:
             _cast = True
     if not _cast:
-        raise ValueError(f"invalid value for type '{_type}': {_val!r}")
+        raise ValueError(
+            f"invalid value for type '{inst_check_err_type_str}': {_val!r}"
+        )
     return _val
 
 
 class CorgyMeta(type):
     """Metaclass for `Corgy`.
 
     Modifies class creation by parsing type annotations, and creating properties for
@@ -429,15 +465,15 @@
             raise AttributeError(f"no value available for attribute `{var_name}`")
 
         def var_fset(self, val):
             if getattr(self, f"_{cls_name.lstrip('_')}__frozen"):
                 raise TypeError(f"cannot set `{var_name}`: object is frozen")
             _checkers = getattr(self, "__checkers")
             try:
-                check_val_type(val, var_type)
+                check_val_type(val, var_type, self_type=type(self))
                 if var_name in _checkers:
                     _checkers[var_name](val)
             except ValueError as e:
                 raise ValueError(f"error setting `{var_name}`: {e}") from None
 
             setattr(self, f"_{cls_name.lstrip('_')}__{var_name}", val)
```

### Comparing `corgy-9.0.0/corgy/types/__init__.py` & `corgy-9.1.0/corgy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/corgy/types/_expand.py` & `corgy-9.1.0/corgy/types/_expand.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/corgy/types/_initargs.py` & `corgy-9.1.0/corgy/types/_initargs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/corgy/types/_inputfile.py` & `corgy-9.1.0/corgy/types/_inputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/corgy/types/_keyvaluepairs.py` & `corgy-9.1.0/corgy/types/_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/corgy/types/_outputfile.py` & `corgy-9.1.0/corgy/types/_outputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/corgy/types/_subclass.py` & `corgy-9.1.0/corgy/types/_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/docs/corgy.md` & `corgy-9.1.0/docs/corgy.md`

 * *Files 1% similar despite different names*

```diff
@@ -450,14 +450,51 @@
 expected one of: (1, 2)
 ```
 
 Note that choices specified in this way are not type-checked to ensure that they
 match the argument type; in the above example, `__choices__` could be set to
 `(1, "2")`.
 
+*Self*
+`Corgy` classes can have attributes of their own type, annotated using
+`typing.Self`.
+
+```python
+>>> if sys.version_info >= (3, 11):
+...     from typing import Self
+... else:
+...     from typing_extensions import Self
+```
+
+```python
+>>> class C(Corgy):
+...     x: int
+...     c: Self
+```
+
+```python
+>>> c = C(x=1)
+>>> c.c = C(x=2)
+>>> c
+C(x=1, c=C(x=2))
+```
+
+```python
+>>> class D(C):
+...     ...
+```
+
+```python
+>>> c.c = D(x=3)
+Traceback (most recent call last):
+    ...
+ValueError: error setting `c`: invalid value for type 'Self (bound to
+<class 'C'>)': D(x=3)
+```
+
 
 #### _classmethod_ add_args_to_parser(parser, name_prefix='', flatten_subgrps=False, defaults=None)
 Add the class’ `Corgy` attributes to the given parser.
 
 
 * **Parameters**
 
@@ -483,14 +520,19 @@
 
 
 Type annotations control how attributes are added to the parser. A number of
 special annotations are parsed and stripped from attribute types to determine
 the parameters for calling `ArgumentParser.add_argument`. These special
 annotations are described below.
 
+Note: `add_args_to_parser` cannot be used if the type annotation for any
+attribute of the class includes `Self`, unless a custom parser is defined
+for such attributes. See docs for `corgyparser` on how to define custom
+parsers.
+
 *Annotated*
 `typing.Annotated` can be used to add a help message for the argument:
 
 ```python
 >>> import argparse
 >>> from argparse import ArgumentParser
 >>> from corgy import CorgyHelpFormatter
```

### Comparing `corgy-9.0.0/docs/corgy.types.md` & `corgy-9.1.0/docs/corgy.types.md`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/pyproject.toml` & `corgy-9.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "corgy"
-version = "9.0.0"  # managed by `poetry-dynamic-versioning`
+version = "9.1.0"  # managed by `poetry-dynamic-versioning`
 description = "Elegant data classes"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jayanthkoushik/corgy"
 packages = [
   { include = "corgy" },
@@ -74,14 +74,15 @@
 force_alphabetical_sort_within_sections = true
 
 [tool.pylint.FORMAT]
 max-line-length = "88"
 
 [tool.pylint.'MESSAGES CONTROL']
 disable = """
+  duplicate-code,
   fixme,
   missing-docstring,
   invalid-name,
   ungrouped-imports,
   wrong-import-order,
   wrong-import-position,
   import-outside-toplevel,
```

### Comparing `corgy-9.0.0/tests/test_corgy.py` & `corgy-9.1.0/tests/test_corgy.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 from unittest.mock import MagicMock, patch
 
 SequenceType = Sequence
 TupleType = Tuple
 SetType = Set
 ListType = List
 
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
+
 if sys.version_info >= (3, 9):
     from collections.abc import Sequence  # pylint: disable=reimported
     from typing import Annotated, Literal
 
     Tuple = tuple  # type: ignore
     Set = set  # type: ignore
     List = list  # type: ignore
@@ -887,14 +892,59 @@
         class C(Corgy):
             x: Literal
 
         c = C()
         with self.assertRaises(ValueError):
             c.x = 1
 
+    def test_corgy_instance_handles_self_type(self):
+        class B(Corgy):
+            x: int
+
+        class C(B):
+            c: Self
+
+        class D(C):
+            ...
+
+        c = C(x=1, c=C(x=2))
+        with self.assertRaises(ValueError):
+            c.c = B(x=2)
+        with self.assertRaises(ValueError):
+            c.c = D(x=2)
+
+        d = D(x=1, c=D(x=2))
+        with self.assertRaises(ValueError):
+            d.c = C(x=2)
+        with self.assertRaises(ValueError):
+            d.c = B(x=2)
+
+    def test_corgy_instance_handles_nested_self_type(self):
+        class C(Corgy):
+            x: int
+            oc: Optional[Self]
+            lc: List[Self]
+
+        class D(C):
+            ...
+
+        c = C(x=1)
+
+        c.oc = None
+        c.oc = C(x=2)
+        with self.assertRaises(ValueError):
+            c.oc = D(x=2)
+
+        c.lc = []
+        c.lc = [C(x=2), C(x=3)]
+        with self.assertRaises(ValueError):
+            c.lc = [D(x=2)]
+        with self.assertRaises(ValueError):
+            c.lc = [C(x=2), D(x=3)]
+
 
 class TestCorgyInit(TestCase):
     def test_corgy_cls_init_assigns_values_to_attrs(self):
         class C(Corgy):
             x1: int
             x2: str
 
@@ -1151,14 +1201,39 @@
         c.x[1].x[1][2].x = 30
 
         self.assertEqual(
             c.as_dict(recursive=True),
             {"x": ({"x": 1}, {"x": (1.1, [{"x": 10}, {"x": 20}, {"x": 30}], 2)})},
         )
 
+    def test_as_dict_handles_self_type(self):
+        class C(Corgy):
+            x: int
+            c: Self
+
+        c = C(x=1, c=C(x=2))
+        self.assertEqual(c.as_dict(recursive=False), {"x": 1, "c": C(x=2)})
+        self.assertEqual(c.as_dict(recursive=True), {"x": 1, "c": {"x": 2}})
+
+        c = C(x=1, c=C(x=2, c=C(x=3)))
+        self.assertEqual(
+            c.as_dict(recursive=True), {"x": 1, "c": {"x": 2, "c": {"x": 3}}}
+        )
+
+    def test_as_dict_handles_self_in_collections(self):
+        class C(Corgy):
+            x: int
+            lc: List[Self]
+
+        c = C(x=1, lc=[C(x=2), C(x=3, lc=[C(x=4, lc=[])])])
+        self.assertEqual(
+            c.as_dict(recursive=True),
+            {"x": 1, "lc": [{"x": 2}, {"x": 3, "lc": [{"x": 4, "lc": []}]}]},
+        )
+
 
 class TestCorgyFromDict(TestCase):
     def test_cls_from_dict_creates_instance_from_dict(self):
         class C(Corgy):
             x: int
             y: str
 
@@ -1388,14 +1463,33 @@
 
         class C(Corgy):
             x: Required[int]
             g: G
 
         self.assertEqual(C.from_dict({"x": 1, "g:x": 2}), C(x=1, g=G(x=2)))
 
+    def test_from_dict_handles_self_type(self):
+        class C(Corgy):
+            x: int
+            c: Self
+
+        self.assertEqual(C.from_dict({"x": 1, "c": {"x": 2}}), C(x=1, c=C(x=2)))
+
+    def test_from_dict_handles_nested_self_type(self):
+        class C(Corgy):
+            x: int
+            lc: List[Self]
+
+        self.assertEqual(
+            C.from_dict(
+                {"x": 1, "lc": [{"x": 2}, {"x": 3, "lc": [{"x": 4, "lc": []}]}]}
+            ),
+            C(x=1, lc=[C(x=2), C(x=3, lc=[C(x=4, lc=[])])]),
+        )
+
 
 class _LoadDictAsFromDictMeta(type):
     """Metaclass to create a version of `TestCorgyFromDict` for `load_dict`."""
 
     def __new__(cls, name, bases, namespace, **kwds):
         for _item in dir(bases[0]):
             if not _item.startswith("test_") or _item.endswith("_required"):
@@ -1520,14 +1614,23 @@
         class C(Corgy):
             x: Required[int]
 
         c = C(x=1)
         with self.assertRaises(TypeError):
             c.load_dict({}, strict=True)
 
+    def test_load_dict_handles_self_type(self):
+        class C(Corgy):
+            x: int
+            c: Self
+
+        c = C(x=1, c=C(x=2))
+        c.load_dict({"c": {"x": 3}})
+        self.assertEqual(c, C(x=1, c=C(x=3)))
+
 
 class TestCorgyPrinting(TestCase):
     @classmethod
     def setUpClass(cls):
         class _CorgyCls(Corgy):
             x1: Sequence[int]
             x2: Annotated[int, "x2 docstr"]
@@ -2370,14 +2473,38 @@
     def test_add_args_raises_on_inconsistent_flags(self):
         class C(Corgy):
             x: Annotated[int, "x help", ["-x", "the-x"]]
 
         with self.assertRaises(TypeError):
             C.add_args_to_parser(self.parser)
 
+    def test_add_args_raises_if_using_self_type(self):
+        class C(Corgy):
+            x: int
+            c: Self
+
+        with self.assertRaises(TypeError):
+            C.add_args_to_parser(self.parser)
+
+    def test_add_args_raises_if_using_optional_self_type(self):
+        class C(Corgy):
+            x: int
+            oc: Optional[Self]
+
+        with self.assertRaises(TypeError):
+            C.add_args_to_parser(self.parser)
+
+    def test_add_args_raises_if_using_collection_with_self_type(self):
+        class C(Corgy):
+            x: int
+            lc: List[Self]
+
+        with self.assertRaises(TypeError):
+            C.add_args_to_parser(self.parser)
+
 
 class TestCorgyAddRequiredArgsToParser(TestCase):
     def setUp(self):
         self.parser = ArgumentParser()
         self.parser.add_argument = MagicMock()
         self.parser.add_argument_group = MagicMock()
 
@@ -2875,14 +3002,23 @@
             def parsex(s):
                 return sum(map(int, s))
 
         f = BytesIO(b"x = [1, 2, 3]\n")
         c = C.parse_from_toml(f)
         self.assertEqual(c.x, 6)
 
+    def test_toml_file_parsing_handles_self_type(self):
+        class C(Corgy):
+            x: int
+            c: Self
+
+        f = BytesIO(b"x = 1\n[c]\nx = 2\n[c.c]\nx = 3")
+        c = C.parse_from_toml(f)
+        self.assertEqual(c, C(x=1, c=C(x=2, c=C(x=3))))
+
 
 class TestCorgyEquality(TestCase):
     def test_corgy_instance_is_equal_to_itself(self):
         class A(Corgy):
             x: int
 
         a = A(x=1)
```

### Comparing `corgy-9.0.0/tests/test_corgychecker.py` & `corgy-9.1.0/tests/test_corgychecker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,17 @@
+import sys
 from typing import ClassVar
 from unittest import TestCase
 from unittest.mock import MagicMock
 
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
+
 from corgy import Corgy, corgychecker
 
 
 class TestCorgyCustomCheckers(TestCase):
     def test_corgychecker_raises_if_not_passed_name(self):
         with self.assertRaises(TypeError):
 
@@ -164,7 +170,24 @@
         class D(C):
             ...
 
         d = D()
         d.x = 2
         with self.assertRaises(ValueError):
             d.x = 1
+
+    def test_corgychecker_works_with_self_type(self):
+        class C(Corgy):
+            x: int
+            c: Self
+
+            @corgychecker("c")
+            @staticmethod
+            def check(v: Self):
+                if v.x % 2:
+                    raise ValueError
+
+        c = C()
+        c.x = 1
+        c.c = C(x=2)
+        with self.assertRaises(ValueError):
+            c.c = C(x=3)
```

### Comparing `corgy-9.0.0/tests/test_corgyparser.py` & `corgy-9.1.0/tests/test_corgyparser.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 from contextlib import redirect_stderr
 from functools import partial
 from io import StringIO
 from typing import ClassVar, Optional, Tuple
 from unittest import TestCase
 from unittest.mock import MagicMock, patch
 
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
+
 if sys.version_info >= (3, 9):
     from typing import Annotated, Literal
 else:
     from typing_extensions import Annotated, Literal
 
 from corgy import Corgy, corgyparser, Required
 from corgy._corgyparser import CorgyParserAction
@@ -510,7 +515,119 @@
         parser.add_argument = MagicMock()
         _parser_action = partial(CorgyParserAction, C.parsex)
         with patch("corgy._corgy.partial", MagicMock(return_value=_parser_action)):
             C.add_args_to_parser(parser)
         parser.add_argument.assert_called_once_with(
             "--x", type=str, action=_parser_action, required=True
         )
+
+    def test_custom_parser_allows_cmdline_parsing_with_self_type(self):
+        class C(Corgy):
+            x: int
+            c: Self
+
+            @corgyparser("c")
+            @staticmethod
+            def parsec(s):
+                return C(x=int(s))
+
+        parser = ArgumentParser()
+        orig_parse_args = ArgumentParser.parse_args
+        parser.parse_args = lambda: orig_parse_args(parser, ["--x", "1", "--c", "2"])
+
+        c = C.parse_from_cmdline(parser)
+        self.assertEqual(c, C(x=1, c=C(x=2)))
+
+    def test_custom_parser_allows_cmdline_parsing_with_nested_self_type(self):
+        class C(Corgy):
+            x: int
+            tc: Tuple[Self]
+
+            @corgyparser("tc")
+            @staticmethod
+            def parsetc(s):
+                return tuple(C(x=int(si)) for si in s.split(":"))
+
+        parser = ArgumentParser()
+        orig_parse_args = ArgumentParser.parse_args
+        parser.parse_args = lambda: orig_parse_args(
+            parser, ["--x", "1", "--tc", "2:3:4"]
+        )
+
+        c = C.parse_from_cmdline(parser)
+        self.assertEqual(c, C(x=1, tc=(C(x=2), C(x=3), C(x=4))))
+
+    def test_custom_parser_allows_cmdline_parsing_heterogenous_collection(self):
+        class C(Corgy):
+            x: Tuple[int, float, str]
+
+            @corgyparser("x")
+            @staticmethod
+            def parsex(s):
+                s = s.split(":")
+                return (int(s[0]), float(s[1]), s[2])
+
+        parser = ArgumentParser()
+        orig_parse_args = ArgumentParser.parse_args
+        parser.parse_args = lambda: orig_parse_args(parser, ["--x", "2:3.0:4"])
+
+        c = C.parse_from_cmdline(parser)
+        self.assertEqual(c, C(x=(2, 3.0, "4")))
+
+    def test_custom_parser_allows_cmdline_parsing_heterogenous_literal(self):
+        class C(Corgy):
+            x: Literal[1, "2"]
+
+            @corgyparser("x")
+            @staticmethod
+            def parsex(s):
+                if s == "1":
+                    return 1
+                if s == "2":
+                    return "2"
+                raise ValueError(s)
+
+        for val in [1, "2"]:
+            with self.subTest(val=val):
+                valstr = str(val)
+                parser = ArgumentParser()
+                orig_parse_args = ArgumentParser.parse_args
+                # pylint: disable=cell-var-from-loop
+                parser.parse_args = lambda: orig_parse_args(parser, ["--x", valstr])
+
+                c = C.parse_from_cmdline(parser)
+                self.assertEqual(c, C(x=val))
+
+    def test_add_args_uses_correct_metavar_with_custom_parser_and_choices(self):
+        class T:
+            __metavar__ = "custom_t"
+
+        class T1(T):
+            ...
+
+        class T2(T):
+            ...
+
+        class C(Corgy):
+            t: Literal[T1, T2]  # type: ignore
+
+            @corgyparser("t")
+            @staticmethod
+            def parset(s):
+                if s == "t1":
+                    return T1
+                if s == "t2":
+                    return T2
+                raise ValueError(s)
+
+        parser = ArgumentParser()
+        parser.add_argument = MagicMock()
+        _parser_action = partial(CorgyParserAction, C.parset, [T1, T2])
+        with patch("corgy._corgy.partial", MagicMock(return_value=_parser_action)):
+            C.add_args_to_parser(parser)
+        parser.add_argument.assert_called_once_with(
+            "--t",
+            type=str,
+            action=_parser_action,
+            metavar="custom_t",
+            default=argparse.SUPPRESS,
+        )
```

### Comparing `corgy-9.0.0/tests/test_doctests.py` & `corgy-9.1.0/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/tests/test_helpfmt.py` & `corgy-9.1.0/tests/test_helpfmt.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/tests/types/_specialtmps.py` & `corgy-9.1.0/tests/types/_specialtmps.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/tests/types/_test_file.py` & `corgy-9.1.0/tests/types/_test_file.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/tests/types/test_initargs.py` & `corgy-9.1.0/tests/types/test_initargs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/tests/types/test_inputfiles.py` & `corgy-9.1.0/tests/types/test_inputfiles.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/tests/types/test_keyvaluepairs.py` & `corgy-9.1.0/tests/types/test_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/tests/types/test_outputfiles.py` & `corgy-9.1.0/tests/types/test_outputfiles.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/tests/types/test_subclass.py` & `corgy-9.1.0/tests/types/test_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-9.0.0/PKG-INFO` & `corgy-9.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corgy
-Version: 9.0.0
+Version: 9.1.0
 Summary: Elegant data classes
 Home-page: https://github.com/jayanthkoushik/corgy
 License: MIT
 Keywords: data classes,argparse,argument parsing,command line parsing,cli
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.7,<4.0
```

