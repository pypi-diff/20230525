# Comparing `tmp/mocksafe-0.5.0a0.tar.gz` & `tmp/mocksafe-0.6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mocksafe-0.5.0a0.tar", last modified: Wed May 24 12:17:30 2023, max compression
+gzip compressed data, was "mocksafe-0.6.0a0.tar", last modified: Thu May 25 16:42:01 2023, max compression
```

## Comparing `mocksafe-0.5.0a0.tar` & `mocksafe-0.6.0a0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-24 12:17:30.059701 mocksafe-0.5.0a0/
--rw-r--r--   0 danielmayo   (501) staff       (20)     1068 2023-05-08 16:33:22.000000 mocksafe-0.5.0a0/LICENSE
--rw-r--r--   0 danielmayo   (501) staff       (20)     4781 2023-05-24 12:17:30.059382 mocksafe-0.5.0a0/PKG-INFO
--rw-r--r--   0 danielmayo   (501) staff       (20)     2119 2023-05-24 12:10:10.000000 mocksafe-0.5.0a0/README.rst
-drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-24 12:17:30.028707 mocksafe-0.5.0a0/mocksafe/
--rw-r--r--   0 danielmayo   (501) staff       (20)      476 2023-05-24 12:06:58.000000 mocksafe-0.5.0a0/mocksafe/__init__.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     1165 2023-05-18 16:23:02.000000 mocksafe-0.5.0a0/mocksafe/call_matchers.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     6661 2023-05-23 15:54:53.000000 mocksafe-0.5.0a0/mocksafe/call_type_validator.py
--rw-r--r--   0 danielmayo   (501) staff       (20)      119 2023-05-16 16:52:33.000000 mocksafe-0.5.0a0/mocksafe/custom_types.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     7520 2023-05-24 12:05:28.000000 mocksafe-0.5.0a0/mocksafe/mock.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     1802 2023-05-23 15:54:53.000000 mocksafe-0.5.0a0/mocksafe/spy.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     3294 2023-05-24 05:50:09.000000 mocksafe-0.5.0a0/mocksafe/stub.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     4058 2023-05-18 16:23:02.000000 mocksafe-0.5.0a0/mocksafe/that.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     6464 2023-05-23 15:54:53.000000 mocksafe-0.5.0a0/mocksafe/when_then.py
-drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-24 12:17:30.057428 mocksafe-0.5.0a0/mocksafe.egg-info/
--rw-r--r--   0 danielmayo   (501) staff       (20)     4781 2023-05-24 12:17:29.000000 mocksafe-0.5.0a0/mocksafe.egg-info/PKG-INFO
--rw-r--r--   0 danielmayo   (501) staff       (20)      377 2023-05-24 12:17:29.000000 mocksafe-0.5.0a0/mocksafe.egg-info/SOURCES.txt
--rw-r--r--   0 danielmayo   (501) staff       (20)        1 2023-05-24 12:17:29.000000 mocksafe-0.5.0a0/mocksafe.egg-info/dependency_links.txt
--rw-r--r--   0 danielmayo   (501) staff       (20)        9 2023-05-24 12:17:29.000000 mocksafe-0.5.0a0/mocksafe.egg-info/top_level.txt
--rw-r--r--   0 danielmayo   (501) staff       (20)     1877 2023-05-24 12:08:50.000000 mocksafe-0.5.0a0/pyproject.toml
--rw-r--r--   0 danielmayo   (501) staff       (20)       38 2023-05-24 12:17:30.059771 mocksafe-0.5.0a0/setup.cfg
-drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-24 12:17:30.058924 mocksafe-0.5.0a0/tests/
--rw-r--r--   0 danielmayo   (501) staff       (20)     6604 2023-05-24 12:05:28.000000 mocksafe-0.5.0a0/tests/test_mocksafe.py
+drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-25 16:42:01.012820 mocksafe-0.6.0a0/
+-rw-r--r--   0 danielmayo   (501) staff       (20)     1068 2023-05-08 16:33:22.000000 mocksafe-0.6.0a0/LICENSE
+-rw-r--r--   0 danielmayo   (501) staff       (20)     4934 2023-05-25 16:42:01.012517 mocksafe-0.6.0a0/PKG-INFO
+-rw-r--r--   0 danielmayo   (501) staff       (20)     2272 2023-05-25 16:24:32.000000 mocksafe-0.6.0a0/README.rst
+drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-25 16:42:01.003874 mocksafe-0.6.0a0/mocksafe/
+-rw-r--r--   0 danielmayo   (501) staff       (20)      606 2023-05-25 16:23:03.000000 mocksafe-0.6.0a0/mocksafe/__init__.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     1165 2023-05-18 16:23:02.000000 mocksafe-0.6.0a0/mocksafe/call_matchers.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     6661 2023-05-23 15:54:53.000000 mocksafe-0.6.0a0/mocksafe/call_type_validator.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)      119 2023-05-16 16:52:33.000000 mocksafe-0.6.0a0/mocksafe/custom_types.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     8372 2023-05-25 16:19:06.000000 mocksafe-0.6.0a0/mocksafe/mock.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     5969 2023-05-25 16:19:06.000000 mocksafe-0.6.0a0/mocksafe/mock_property.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     2207 2023-05-25 16:19:06.000000 mocksafe-0.6.0a0/mocksafe/spy.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     3294 2023-05-24 05:50:09.000000 mocksafe-0.6.0a0/mocksafe/stub.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     4067 2023-05-25 16:19:06.000000 mocksafe-0.6.0a0/mocksafe/that.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     7011 2023-05-25 16:19:06.000000 mocksafe-0.6.0a0/mocksafe/when_then.py
+drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-25 16:42:01.010880 mocksafe-0.6.0a0/mocksafe.egg-info/
+-rw-r--r--   0 danielmayo   (501) staff       (20)     4934 2023-05-25 16:42:00.000000 mocksafe-0.6.0a0/mocksafe.egg-info/PKG-INFO
+-rw-r--r--   0 danielmayo   (501) staff       (20)      423 2023-05-25 16:42:00.000000 mocksafe-0.6.0a0/mocksafe.egg-info/SOURCES.txt
+-rw-r--r--   0 danielmayo   (501) staff       (20)        1 2023-05-25 16:42:00.000000 mocksafe-0.6.0a0/mocksafe.egg-info/dependency_links.txt
+-rw-r--r--   0 danielmayo   (501) staff       (20)        9 2023-05-25 16:42:00.000000 mocksafe-0.6.0a0/mocksafe.egg-info/top_level.txt
+-rw-r--r--   0 danielmayo   (501) staff       (20)     1903 2023-05-25 16:23:40.000000 mocksafe-0.6.0a0/pyproject.toml
+-rw-r--r--   0 danielmayo   (501) staff       (20)       38 2023-05-25 16:42:01.012890 mocksafe-0.6.0a0/setup.cfg
+drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-25 16:42:01.012120 mocksafe-0.6.0a0/tests/
+-rw-r--r--   0 danielmayo   (501) staff       (20)     6604 2023-05-24 12:05:28.000000 mocksafe-0.6.0a0/tests/test_mocksafe.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     1167 2023-05-25 16:19:06.000000 mocksafe-0.6.0a0/tests/test_props.py
```

### Comparing `mocksafe-0.5.0a0/LICENSE` & `mocksafe-0.6.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `mocksafe-0.5.0a0/PKG-INFO` & `mocksafe-0.6.0a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocksafe
-Version: 0.5.0a0
+Version: 0.6.0a0
 Summary: A mocking library developed to enable static and runtime type checking of your mocks to keep them in sync with production code.
 License: MIT License
         
         Copyright (c) 2023 Daniel Mayo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,15 +20,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Documentation, https://mocksafe.readthedocs.io/en/0.5/
+Project-URL: Documentation, https://mocksafe.readthedocs.io/en/0.6/
 Project-URL: Source, https://github.com/dmayo3/mocksafe
 Keywords: mock,mocking,typed,typing,typesafe,testing,tests,mocks,magicmock,unittest,stubbing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -51,34 +51,37 @@
 License-File: LICENSE
 
 .. image:: https://github.com/dmayo3/mocksafe/actions/workflows/mocksafe.yml/badge.svg
     :target: https://github.com/dmayo3/mocksafe/actions/workflows/mocksafe.yml?query=branch%3Amain
     :alt: Github Actions Status
 .. image:: https://codecov.io/gh/dmayo3/mocksafe/branch/main/graph/badge.svg?token=S3JI6OOTGF 
     :target: https://codecov.io/gh/dmayo3/mocksafe
-.. image:: https://readthedocs.org/projects/mocksafe/badge/?version=0.5
-    :target: https://mocksafe.readthedocs.io/en/0.5/?badge=0.5
+.. image:: https://readthedocs.org/projects/mocksafe/badge/?version=stable
+    :target: https://mocksafe.readthedocs.io/en/stable/?badge=stable
     :alt: Documentation Status
 .. image:: https://badge.fury.io/py/mocksafe.svg
     :target: https://badge.fury.io/py/mocksafe
     :alt: PyPI Package
+.. image:: https://img.shields.io/badge/semver-2.0.0-blue
+    :target: https://semver.org/
+    :alt: Follows the Semantic Versioning 2.0.0 spec
 .. image:: https://img.shields.io/pypi/pyversions/mocksafe.svg
     :target: https://pypi.org/project/mocksafe
     :alt: Supported versions
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code style: black
 .. image:: http://www.mypy-lang.org/static/mypy_badge.svg
     :target: http://mypy-lang.org/
     :alt: Type checked by mypy
 .. image:: https://img.shields.io/badge/License-MIT-green.svg
     :target: https://github.com/dmayo3/mocksafe/blob/main/LICENSE
     :alt: MIT License
 
-MockSafe v0.5.0-alpha
+MockSafe v0.6.0-alpha
 ---------------------
 
 A mocking library developed to enable static and runtime type checking of your mocks to help keep them up-to-date with your production code.
 
 It has a simple, fluent API and is designed to be used with Python's `assert` statement.
 
 Checkout the docs link below for more information.
@@ -86,18 +89,18 @@
 Install and quickstart
 ----------------------
 
 ::
 
     pip install mocksafe
 
-`Library Usage <https://mocksafe.readthedocs.io/en/0.5/usage.html>`_
+`Library Usage <https://mocksafe.readthedocs.io/en/0.6/usage.html>`_
 
 Links
 ----------------------
 
 :Install: `PyPi <https://pypi.org/project/mocksafe>`_
-:Docs:    `Read The Docs <https://mocksafe.readthedocs.io/en/0.5/>`_
+:Docs:    `Read The Docs <https://mocksafe.readthedocs.io/en/0.6/>`_
 :License: `MIT <https://github.com/dmayo3/mocksafe/blob/main/LICENSE>`_
 :Source:  `GitHub <https://github.com/dmayo3/mocksafe>`_
 :Issues:  `GitHub Issues <https://github.com/dmayo3/mocksafe/issues>`_
 :Discussion:  `Questions & Feedback <https://github.com/dmayo3/mocksafe/discussions>`_
```

### Comparing `mocksafe-0.5.0a0/README.rst` & `mocksafe-0.6.0a0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 .. image:: https://github.com/dmayo3/mocksafe/actions/workflows/mocksafe.yml/badge.svg
     :target: https://github.com/dmayo3/mocksafe/actions/workflows/mocksafe.yml?query=branch%3Amain
     :alt: Github Actions Status
 .. image:: https://codecov.io/gh/dmayo3/mocksafe/branch/main/graph/badge.svg?token=S3JI6OOTGF 
     :target: https://codecov.io/gh/dmayo3/mocksafe
-.. image:: https://readthedocs.org/projects/mocksafe/badge/?version=0.5
-    :target: https://mocksafe.readthedocs.io/en/0.5/?badge=0.5
+.. image:: https://readthedocs.org/projects/mocksafe/badge/?version=stable
+    :target: https://mocksafe.readthedocs.io/en/stable/?badge=stable
     :alt: Documentation Status
 .. image:: https://badge.fury.io/py/mocksafe.svg
     :target: https://badge.fury.io/py/mocksafe
     :alt: PyPI Package
+.. image:: https://img.shields.io/badge/semver-2.0.0-blue
+    :target: https://semver.org/
+    :alt: Follows the Semantic Versioning 2.0.0 spec
 .. image:: https://img.shields.io/pypi/pyversions/mocksafe.svg
     :target: https://pypi.org/project/mocksafe
     :alt: Supported versions
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code style: black
 .. image:: http://www.mypy-lang.org/static/mypy_badge.svg
     :target: http://mypy-lang.org/
     :alt: Type checked by mypy
 .. image:: https://img.shields.io/badge/License-MIT-green.svg
     :target: https://github.com/dmayo3/mocksafe/blob/main/LICENSE
     :alt: MIT License
 
-MockSafe v0.5.0-alpha
+MockSafe v0.6.0-alpha
 ---------------------
 
 A mocking library developed to enable static and runtime type checking of your mocks to help keep them up-to-date with your production code.
 
 It has a simple, fluent API and is designed to be used with Python's `assert` statement.
 
 Checkout the docs link below for more information.
@@ -34,18 +37,18 @@
 Install and quickstart
 ----------------------
 
 ::
 
     pip install mocksafe
 
-`Library Usage <https://mocksafe.readthedocs.io/en/0.5/usage.html>`_
+`Library Usage <https://mocksafe.readthedocs.io/en/0.6/usage.html>`_
 
 Links
 ----------------------
 
 :Install: `PyPi <https://pypi.org/project/mocksafe>`_
-:Docs:    `Read The Docs <https://mocksafe.readthedocs.io/en/0.5/>`_
+:Docs:    `Read The Docs <https://mocksafe.readthedocs.io/en/0.6/>`_
 :License: `MIT <https://github.com/dmayo3/mocksafe/blob/main/LICENSE>`_
 :Source:  `GitHub <https://github.com/dmayo3/mocksafe>`_
 :Issues:  `GitHub Issues <https://github.com/dmayo3/mocksafe/issues>`_
 :Discussion:  `Questions & Feedback <https://github.com/dmayo3/mocksafe/discussions>`_
```

### Comparing `mocksafe-0.5.0a0/mocksafe/call_matchers.py` & `mocksafe-0.6.0a0/mocksafe/call_matchers.py`

 * *Files identical despite different names*

### Comparing `mocksafe-0.5.0a0/mocksafe/call_type_validator.py` & `mocksafe-0.6.0a0/mocksafe/call_type_validator.py`

 * *Files identical despite different names*

### Comparing `mocksafe-0.5.0a0/mocksafe/mock.py` & `mocksafe-0.6.0a0/mocksafe/mock.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 import inspect
 from itertools import count
 from types import ModuleType
-from typing import Generic, TypeVar, Optional, Union, Any, cast
+from typing import Generic, TypeVar, Optional, Union, Any, cast, get_type_hints
 from mocksafe.custom_types import MethodName, CallMatcher, Call
-from mocksafe.spy import MethodSpy
+from mocksafe.spy import MethodSpy, CallRecorder
 from mocksafe.stub import MethodStub, ResultsProvider
 from mocksafe.call_matchers import ExactCallMatcher
 
 
 T = TypeVar("T")
 V = TypeVar("V")
 M = TypeVar("M", bound=ModuleType)
@@ -151,18 +151,14 @@
     def __class__(self: SafeMock):
         return self._original_class
 
     def __repr__(self: SafeMock) -> str:
         return f"SafeMock[{self._name}]"
 
     def __getattr__(self: SafeMock, attr_name: str) -> MethodMock:
-        if attr_name in getattr(self._spec, "__attrs__", []):
-            # Field attribute defined on the original class
-            raise AttributeError(f"{self}.{attr_name} attribute value not set.")
-
         original_attr = self.get_original_attr(attr_name)
 
         if isinstance(original_attr, property):
             raise ValueError(
                 (
                     "MockSafe doesn't currently support properties, "
                     f"so {self}.{attr_name} could not be mocked."
@@ -175,25 +171,48 @@
                 self._spec, str(self), attr_name, signature
             )
 
         return self._mocks[attr_name]
 
     def get_original_attr(self: SafeMock, attr_name: str) -> Any:
         try:
+            spec_annotations = get_type_hints(self._spec)
+        except (KeyError, AttributeError):
+            # get_type_hints() can blow up on mocked modules
+            # as they are not real classes
+            spec_annotations = {}
+
+        if attr_name in spec_annotations:
+            # Field attribute annotated on the original class but with
+            # no value for it stubbed on the mock object yet
+
+            # TODO: attempt to return a default value for it based on the
+            # annotation type
+            raise AttributeError(f"{self}.{attr_name} field value not stubbed.")
+
+        if attr_name in getattr(self._spec, "__attrs__", []):
+            # Field attribute defined on the original class but with
+            # no value for it stubbed on the mock object yet.
+
+            # Note that __attrs__ is not a Python standard, it's a convention
+            # used by the requests library.
+            raise AttributeError(f"{self}.{attr_name} field value not stubbed.")
+
+        try:
             return getattr(self._spec, attr_name)
         except AttributeError:
             raise AttributeError(
                 (
                     f"{self}.{attr_name} attribute doesn't exist on the "
                     f"original mocked type/module {self._original}."
                 ),
             ) from None
 
 
-class MethodMock(Generic[T]):
+class MethodMock(CallRecorder, Generic[T]):
     def __init__(
         self: MethodMock,
         spec: type[T],
         parent_name: str,
         name: MethodName,
         signature: inspect.Signature,
     ):
```

### Comparing `mocksafe-0.5.0a0/mocksafe/spy.py` & `mocksafe-0.6.0a0/mocksafe/spy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,38 @@
 from __future__ import annotations
 from inspect import Signature
-from typing import Generic, TypeVar
+from typing import Generic, TypeVar, Protocol, runtime_checkable
 from collections.abc import Callable
 from mocksafe.custom_types import MethodName, Call
 from mocksafe.call_type_validator import CallTypeValidator
 
 
 T = TypeVar("T")
 
 
-class MethodSpy(Generic[T]):
+@runtime_checkable
+class CallRecorder(Protocol):
+    """
+    Generic Protocol for getting information about
+    mocked / spied calls.
+    """
+
+    @property
+    def name(self: CallRecorder) -> MethodName:
+        ...
+
+    @property
+    def calls(self: CallRecorder) -> list[Call]:
+        ...
+
+    def nth_call(self: CallRecorder, n: int) -> Call:
+        ...
+
+
+class MethodSpy(CallRecorder, Generic[T]):
     def __init__(
         self: MethodSpy,
         name: MethodName,
         delegate: Callable[..., T],
         signature: Signature,
     ):
         self._name = name
```

### Comparing `mocksafe-0.5.0a0/mocksafe/stub.py` & `mocksafe-0.6.0a0/mocksafe/stub.py`

 * *Files identical despite different names*

### Comparing `mocksafe-0.5.0a0/mocksafe/that.py` & `mocksafe-0.6.0a0/mocksafe/that.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 from __future__ import annotations
-from typing import Union
-from collections.abc import Callable
+from typing import Union, Any
 from mocksafe.custom_types import Call
-from mocksafe.mock import MethodMock
+from mocksafe.spy import CallRecorder
 
 
 Args = tuple
 
 
-def that(mock_method: Callable) -> MockCalls:
+def that(mocked: Any) -> MockCalls:
     """
     Used to assert how a mocked method was called.
 
-    :param mock_method: a method on a mock object
+    :param mocked: a method on a mock object
     :rtype: MockCalls
 
     :Example:
         >>> assert that(mock_random.random).was_not_called
 
     :Example:
         >>> that(mock_random.random)
-        MockCalls[random();num_calls=0]
+        MockCalls[random;num_calls=0]
     """
-    if not isinstance(mock_method, MethodMock):
-        raise ValueError("Not a SafeMocked method: mock_method")
-    return MockCalls(mock_method)
+    if not isinstance(mocked, CallRecorder):
+        raise TypeError(
+            f"Expected a mocked method/function/property but got '{mocked}'"
+            f" ({type(mocked)})"
+        )
+    return MockCalls(mocked)
 
 
-def spy(mock_method: Callable) -> MockCalls:
+def spy(mocked: Any) -> MockCalls:
     """
     This is used to capture the arguments that were
-    passed when the given ``mock_method`` was called,
+    passed when the given ``mocked`` was called,
     which is useful for making more detailed assertions
     on the contents.
 
     The ``spy()`` function is actually an alias for ``that()``.
 
     Both are just syntactic sugar to make your code flow more
     fluently, for example ``assert that(mock.foo).was_called``
     versus ``args = spy(mock.foo).last_call``.
 
-    :param mock_method: a method on a mock object
+    :param mocked: a method on a mock object
     :rtype: MockCalls
 
     :Example:
         >>> spy(mock_random.random)
-        MockCalls[random();num_calls=0]
+        MockCalls[random;num_calls=0]
 
     :Example:
         >>> spy(mock_random.random).was_not_called
         True
 
     :Example:
         >>> when(mock_random.random).any_call().then_return(0.123)
@@ -61,15 +63,15 @@
     :Example:
         >>> when(mock_random.randint).any_call().then_return(5)
         >>> mock_random.randint(0, 10)
         5
         >>> spy(mock_random.randint).last_call
         (0, 10)
     """
-    return that(mock_method)
+    return that(mocked)
 
 
 class MockCalls:
     """
     Provides information about calls made to a mocked method.
 
     This object returned by both :meth:`mocksafe.that` and :meth:`mocksafe.spy`.
@@ -100,42 +102,42 @@
         5
         >>> mock_random.randint(10, 20)
         13
         >>> assert that(mock_random.randint).last_call == (10, 20)
         >>> assert that(mock_random.randint).nth_call(0) == ((), {"a":1, "b":10})
     """
 
-    def __init__(self: MockCalls, method_mock: MethodMock):
-        self._method_mock = method_mock
+    def __init__(self: MockCalls, call_recorder: CallRecorder):
+        self._call_recorder = call_recorder
 
     def __repr__(self: MockCalls) -> str:
-        return f"MockCalls[{self._method_mock.name}();num_calls={self.num_calls}]"
+        return f"MockCalls[{self._call_recorder.name};num_calls={self.num_calls}]"
 
     @property
     def was_called(self: MockCalls) -> bool:
         """Return whether the mocked method was called at least once."""
         return self.num_calls > 0
 
     @property
     def was_not_called(self: MockCalls) -> bool:
         """Return whether the mocked method was not called."""
         return not self.was_called
 
     @property
     def num_calls(self: MockCalls) -> int:
         """Returns the number of calls made to the mocked method."""
-        return len(self._method_mock.calls)
+        return len(self._call_recorder.calls)
 
     @property
     def last_call(self: MockCalls) -> Union[Args, Call]:
         """Returns details of the last call made to the mocked method."""
         return self.nth_call(-1)
 
     def nth_call(self: MockCalls, n: int) -> Union[Args, Call]:
         """Returns details of the Nth call made to the mocked method."""
-        call = self._method_mock.nth_call(n)
+        call = self._call_recorder.nth_call(n)
 
         args, kwargs = call
 
         if kwargs:
             return call
         return args
```

### Comparing `mocksafe-0.5.0a0/mocksafe/when_then.py` & `mocksafe-0.6.0a0/mocksafe/when_then.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
-from typing import Generic, Union, TypeVar
+from typing import Generic, Union, TypeVar, Any
 from collections.abc import Callable
 from mocksafe.custom_types import CallMatcher
-from mocksafe.mock import MethodMock, ResultsProvider
+from mocksafe.mock import SafeMock, MethodMock, ResultsProvider
+from mocksafe.mock_property import PropertyStubber
 from mocksafe.call_matchers import AnyCallMatcher, CustomCallMatcher
 
 
 T = TypeVar("T")
 ANY_CALL: CallMatcher = AnyCallMatcher()
 
 
@@ -27,14 +28,29 @@
     if not isinstance(mock_method, MethodMock):
         raise ValueError(
             f"Not a SafeMocked method: {mock_method} ({type(mock_method)})"
         )
     return WhenStubber(mock_method)
 
 
+def stub(mock_object: Any) -> PropertyStubber:
+    """
+    Prepare to stub a property on ``mock_object``.
+
+    See the :doc:`../mocking` page for more details and an
+    example of how to mock, stub, and verify a property.
+
+    See also: :class:`mocksafe.PropertyStubber`
+    See also: :class:`mocksafe.MockProperty`
+    """
+    if not isinstance(mock_object, SafeMock):
+        raise ValueError(f"Not a SafeMocked object: {mock_object}")
+    return PropertyStubber(mock_object)
+
+
 class WhenStubber(Generic[T]):
     """
     Set up conditions for when a stub is to be used.
 
     :Example:
         >>> when(mock_random.random).any_call().then_return(0.31)
```

### Comparing `mocksafe-0.5.0a0/mocksafe.egg-info/PKG-INFO` & `mocksafe-0.6.0a0/mocksafe.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocksafe
-Version: 0.5.0a0
+Version: 0.6.0a0
 Summary: A mocking library developed to enable static and runtime type checking of your mocks to keep them in sync with production code.
 License: MIT License
         
         Copyright (c) 2023 Daniel Mayo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,15 +20,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Documentation, https://mocksafe.readthedocs.io/en/0.5/
+Project-URL: Documentation, https://mocksafe.readthedocs.io/en/0.6/
 Project-URL: Source, https://github.com/dmayo3/mocksafe
 Keywords: mock,mocking,typed,typing,typesafe,testing,tests,mocks,magicmock,unittest,stubbing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -51,34 +51,37 @@
 License-File: LICENSE
 
 .. image:: https://github.com/dmayo3/mocksafe/actions/workflows/mocksafe.yml/badge.svg
     :target: https://github.com/dmayo3/mocksafe/actions/workflows/mocksafe.yml?query=branch%3Amain
     :alt: Github Actions Status
 .. image:: https://codecov.io/gh/dmayo3/mocksafe/branch/main/graph/badge.svg?token=S3JI6OOTGF 
     :target: https://codecov.io/gh/dmayo3/mocksafe
-.. image:: https://readthedocs.org/projects/mocksafe/badge/?version=0.5
-    :target: https://mocksafe.readthedocs.io/en/0.5/?badge=0.5
+.. image:: https://readthedocs.org/projects/mocksafe/badge/?version=stable
+    :target: https://mocksafe.readthedocs.io/en/stable/?badge=stable
     :alt: Documentation Status
 .. image:: https://badge.fury.io/py/mocksafe.svg
     :target: https://badge.fury.io/py/mocksafe
     :alt: PyPI Package
+.. image:: https://img.shields.io/badge/semver-2.0.0-blue
+    :target: https://semver.org/
+    :alt: Follows the Semantic Versioning 2.0.0 spec
 .. image:: https://img.shields.io/pypi/pyversions/mocksafe.svg
     :target: https://pypi.org/project/mocksafe
     :alt: Supported versions
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code style: black
 .. image:: http://www.mypy-lang.org/static/mypy_badge.svg
     :target: http://mypy-lang.org/
     :alt: Type checked by mypy
 .. image:: https://img.shields.io/badge/License-MIT-green.svg
     :target: https://github.com/dmayo3/mocksafe/blob/main/LICENSE
     :alt: MIT License
 
-MockSafe v0.5.0-alpha
+MockSafe v0.6.0-alpha
 ---------------------
 
 A mocking library developed to enable static and runtime type checking of your mocks to help keep them up-to-date with your production code.
 
 It has a simple, fluent API and is designed to be used with Python's `assert` statement.
 
 Checkout the docs link below for more information.
@@ -86,18 +89,18 @@
 Install and quickstart
 ----------------------
 
 ::
 
     pip install mocksafe
 
-`Library Usage <https://mocksafe.readthedocs.io/en/0.5/usage.html>`_
+`Library Usage <https://mocksafe.readthedocs.io/en/0.6/usage.html>`_
 
 Links
 ----------------------
 
 :Install: `PyPi <https://pypi.org/project/mocksafe>`_
-:Docs:    `Read The Docs <https://mocksafe.readthedocs.io/en/0.5/>`_
+:Docs:    `Read The Docs <https://mocksafe.readthedocs.io/en/0.6/>`_
 :License: `MIT <https://github.com/dmayo3/mocksafe/blob/main/LICENSE>`_
 :Source:  `GitHub <https://github.com/dmayo3/mocksafe>`_
 :Issues:  `GitHub Issues <https://github.com/dmayo3/mocksafe/issues>`_
 :Discussion:  `Questions & Feedback <https://github.com/dmayo3/mocksafe/discussions>`_
```

### Comparing `mocksafe-0.5.0a0/pyproject.toml` & `mocksafe-0.6.0a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mocksafe"
-version = "0.5.0-alpha"
+version = "0.6.0-alpha"
 
 description = "A mocking library developed to enable static and runtime type checking of your mocks to keep them in sync with production code."
 
 requires-python = ">= 3.9"
 readme = "README.rst"
 license = { file = "LICENSE" }
 classifiers = [
@@ -28,33 +28,33 @@
     "Framework :: Pytest",
     "Typing :: Typed",
 ]
 keywords = ["mock", "mocking", "typed", "typing", "typesafe", "testing", "tests", "mocks", "magicmock", "unittest", "stubbing"]
 dependencies = []
 
 [project.urls]
-Documentation = "https://mocksafe.readthedocs.io/en/0.5/"
+Documentation = "https://mocksafe.readthedocs.io/en/0.6/"
 Source = "https://github.com/dmayo3/mocksafe"
 
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools", "wheel"]
 
 [tool.bumpver]
-current_version = "0.5.0-alpha"
+current_version = "0.6.0-alpha"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
     'version = "{version}"',
 ]
 "mocksafe/__init__.py" = [
-    "{version}",
+    '__version__ = "{version}"',
 ]
 "README.rst" = [
-    "{version}",
+    'MockSafe v{version}',
 ]
```

### Comparing `mocksafe-0.5.0a0/tests/test_mocksafe.py` & `mocksafe-0.6.0a0/tests/test_mocksafe.py`

 * *Files identical despite different names*

