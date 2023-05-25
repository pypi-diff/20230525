# Comparing `tmp/nepattern-0.5.7.tar.gz` & `tmp/nepattern-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepattern-0.5.7.tar", last modified: Sat May 13 07:29:42 2023, max compression
+gzip compressed data, was "nepattern-0.5.8.tar", last modified: Thu May 25 16:55:50 2023, max compression
```

## Comparing `nepattern-0.5.7.tar` & `nepattern-0.5.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 nepattern-0.5.7/LICENSE
--rw-r--r--   0        0        0      703 2023-04-17 06:05:25.529605 nepattern-0.5.7/nepattern/__init__.py
--rw-r--r--   0        0        0     8966 2023-05-13 07:03:55.942573 nepattern-0.5.7/nepattern/base.py
--rw-r--r--   0        0        0     4010 2023-03-31 19:06:53.737926 nepattern-0.5.7/nepattern/context.py
--rw-r--r--   0        0        0     1419 2023-04-17 06:19:02.570290 nepattern-0.5.7/nepattern/context.pyi
--rw-r--r--   0        0        0    15857 2023-05-03 08:15:17.438046 nepattern-0.5.7/nepattern/core.py
--rw-r--r--   0        0        0       63 2022-08-22 03:10:58.502097 nepattern-0.5.7/nepattern/exception.py
--rw-r--r--   0        0        0       26 2023-04-17 06:05:25.556543 nepattern-0.5.7/nepattern/i18n/.config.json
--rw-r--r--   0        0        0      381 2023-04-17 06:05:25.502608 nepattern-0.5.7/nepattern/i18n/en-US.json
--rw-r--r--   0        0        0      353 2023-04-17 06:05:25.567509 nepattern-0.5.7/nepattern/i18n/zh-CN.json
--rw-r--r--   0        0        0    10277 2023-05-03 08:25:00.521491 nepattern-0.5.7/nepattern/main.py
--rw-r--r--   0        0        0      695 2023-04-17 06:21:36.032925 nepattern-0.5.7/nepattern/util.py
--rw-r--r--   0        0        0     1738 2023-05-13 07:29:18.513282 nepattern-0.5.7/pyproject.toml
--rw-r--r--   0        0        0      943 2023-02-25 11:05:27.501329 nepattern-0.5.7/README.md
--rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 nepattern-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 nepattern-0.5.8/LICENSE
+-rw-r--r--   0        0        0      723 2023-05-25 16:53:52.239559 nepattern-0.5.8/nepattern/__init__.py
+-rw-r--r--   0        0        0    10865 2023-05-25 16:54:49.230259 nepattern-0.5.8/nepattern/base.py
+-rw-r--r--   0        0        0     4010 2023-03-31 19:06:53.737926 nepattern-0.5.8/nepattern/context.py
+-rw-r--r--   0        0        0     1419 2023-04-17 06:19:02.570290 nepattern-0.5.8/nepattern/context.pyi
+-rw-r--r--   0        0        0    15999 2023-05-25 16:54:58.101916 nepattern-0.5.8/nepattern/core.py
+-rw-r--r--   0        0        0       63 2022-08-22 03:10:58.502097 nepattern-0.5.8/nepattern/exception.py
+-rw-r--r--   0        0        0       26 2023-04-17 06:05:25.556543 nepattern-0.5.8/nepattern/i18n/.config.json
+-rw-r--r--   0        0        0      381 2023-04-17 06:05:25.502608 nepattern-0.5.8/nepattern/i18n/en-US.json
+-rw-r--r--   0        0        0      353 2023-04-17 06:05:25.567509 nepattern-0.5.8/nepattern/i18n/zh-CN.json
+-rw-r--r--   0        0        0    10438 2023-05-25 16:53:52.258975 nepattern-0.5.8/nepattern/main.py
+-rw-r--r--   0        0        0      695 2023-04-17 06:21:36.032925 nepattern-0.5.8/nepattern/util.py
+-rw-r--r--   0        0        0     1738 2023-05-25 16:54:58.015909 nepattern-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0      943 2023-02-25 11:05:27.501329 nepattern-0.5.8/README.md
+-rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 nepattern-0.5.8/PKG-INFO
```

### Comparing `nepattern-0.5.7/LICENSE` & `nepattern-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.7/nepattern/__init__.py` & `nepattern-0.5.8/nepattern/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from tarina import Empty as Empty  # noqa
 from .base import (
+    DirectPattern,
     MappingPattern,
     RegexPattern,
     SequencePattern,
     SwitchPattern,
     UnionPattern,
 )
 from .context import (
```

### Comparing `nepattern-0.5.7/nepattern/base.py` & `nepattern-0.5.8/nepattern/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,79 @@
 from __future__ import annotations
 
 import re
-from typing import Any, Dict, Iterable, Literal, TypeVar, Union
+from typing import Any, Dict, Iterable, Literal, TypeVar, Match
 
 from tarina import Empty
 from tarina.lang import lang
 
-from .core import BasePattern, MatchMode
+from .core import BasePattern, MatchMode, ValidateResult, ResultFlag
 from .exception import MatchFailed
 
 
-class RegexPattern(BasePattern[Union[dict, tuple]]):
+class DirectPattern(BasePattern):
+    """直接判断"""
+    def __init__(self, target: Any, alias: str | None = None):
+        self.target = target
+        super().__init__("", MatchMode.TYPE_CONVERT, type(target), alias=alias or str(target))
+
+    def prefixed(self):
+        if isinstance(self.target, str):
+            return BasePattern(self.target, alias=self.alias).prefixed()
+        return self
+
+    def suffixed(self):
+        if isinstance(self.target, str):
+            return BasePattern(self.target, alias=self.alias).suffixed()
+        return self
+
+    def match(self, input_: Any):
+        if input_ != self.target:
+            raise MatchFailed(
+                lang.require("nepattern", "content_error").format(target=input_)
+            )
+        return input_
+
+    def validate(self, input_: Any, default: Any = None):
+        if input_ == self.target:
+            return ValidateResult(input_, ResultFlag.VALID)
+        e = MatchFailed(
+            lang.require("nepattern", "content_error").format(target=input_)
+        )
+        if default is None:
+            return ValidateResult(error=e, flag=ResultFlag.ERROR)
+        return ValidateResult(
+            value=None if default is Empty else default, flag=ResultFlag.DEFAULT  # type: ignore
+        )
+
+    def invalidate(self, input_: Any, default: Any = None) -> ValidateResult[Any]:
+        if input_ == self.target:
+            e = MatchFailed(
+                lang.require("nepattern", "content_error").format(target=input_)
+            )
+            if default is None:
+                return ValidateResult(error=e, flag=ResultFlag.ERROR)
+            return ValidateResult(
+                value=None if default is Empty else default, flag=ResultFlag.DEFAULT  # type: ignore
+            )
+        return ValidateResult(input_, flag=ResultFlag.VALID)
+
+class RegexPattern(BasePattern[Match[str]]):
     """针对正则的特化匹配，支持正则组"""
 
     def __init__(self, pattern: str, alias: str | None = None):
-        super().__init__(pattern, origin=Union[dict, tuple], alias=alias or "regex[:group]")  # type: ignore
+        super().__init__(pattern, origin=Match[str], alias=alias or "regex[:group]")  # type: ignore
 
-    def match(self, input_: str | Any):
+    def match(self, input_: str | Any) -> Match[str]:
         if not isinstance(input_, str):
             raise MatchFailed(
                 lang.require("nepattern", "type_error").format(target=input_)
             )
         if mat := self.regex_pattern.match(input_):
-            return mat.groupdict() or mat.groups()
+            return mat
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_)
         )
 
 
 class UnionPattern(BasePattern):
     """多类型参数的匹配"""
@@ -259,13 +306,14 @@
                 return self.switch[...]
             raise MatchFailed(
                 lang.require("nepattern", "content_error").format(target=input_)
             ) from e
 
 
 __all__ = [
+    "DirectPattern",
     "RegexPattern",
     "UnionPattern",
     "SequencePattern",
     "MappingPattern",
     "SwitchPattern",
 ]
```

### Comparing `nepattern-0.5.7/nepattern/context.py` & `nepattern-0.5.8/nepattern/context.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.7/nepattern/context.pyi` & `nepattern-0.5.8/nepattern/context.pyi`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.7/nepattern/core.py` & `nepattern-0.5.8/nepattern/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import re
 from copy import deepcopy
-from dataclasses import dataclass
 from enum import Enum, IntEnum
 from typing import Any, Callable, Generic, TypeVar, overload
 
 from tarina import Empty, generic_isinstance
 from tarina.lang import lang
 
 try:
@@ -44,15 +43,14 @@
 
 T = TypeVar("T")
 TOrigin = TypeVar("TOrigin")
 TVOrigin = TypeVar("TVOrigin")
 TDefault = TypeVar("TDefault")
 
 
-@dataclass(init=False)
 class ValidateResult(Generic[TVOrigin]):
     """参数表达式验证结果"""
     def __init__(
         self,
         value: TVOrigin | type[Empty] = Empty,
         error: Exception | type[Empty] = Empty,
         flag: ResultFlag = ResultFlag.VALID,
@@ -128,14 +126,21 @@
         self, other: type[T] | Callable[[TVOrigin], T] | Any
     ) -> T | Self | ValidateResult[T]:
         return self.step(other)  # type: ignore
 
     def __bool__(self):
         return self.success
 
+    def __repr__(self):
+        if self.flag == ResultFlag.VALID:
+            return f"ValidateResult(value={self._value!r})"
+        if self.flag == ResultFlag.ERROR:
+            return f"ValidateResult(error={self._error!r})"
+        return f"ValidateResult(default={self._value!r})"
+
 
 class BasePattern(Generic[TOrigin]):
     """对参数类型值的包装"""
 
     regex_pattern: TPattern  # type: ignore
     pattern: str
     mode: MatchMode
@@ -275,21 +280,17 @@
         return BasePattern(
             "", MatchMode.KEEP, unit, alias=unit.__name__, accepts=[unit]
         )
 
     @staticmethod
     def on(obj: TOrigin) -> BasePattern[TOrigin]:
         """提供 DataUnit 类型的构造方法"""
-        return BasePattern(
-            "",
-            MatchMode.KEEP,
-            type(obj),
-            alias=str(obj),
-            validators=[lambda x: x == obj],
-        )
+        from .base import DirectPattern
+
+        return DirectPattern(obj)
 
     @staticmethod
     def to(content: Any) -> BasePattern | None:
         """便捷的使用 type_parser 的方法"""
         from .main import type_parser
 
         if isinstance(res := type_parser(content, "allow"), BasePattern):
@@ -473,8 +474,8 @@
 def set_unit(
     target: type[TOrigin], predicate: Callable[..., bool]
 ) -> Annotated[TOrigin, ...]:
     """通过predicate区分同一个类的不同情况"""
     return Annotated[target, predicate]  # type: ignore
 
 
-__all__ = ["MatchMode", "BasePattern", "set_unit", "ValidateResult", "TOrigin"]
+__all__ = ["MatchMode", "BasePattern", "set_unit", "ValidateResult", "TOrigin", "ResultFlag"]
```

### Comparing `nepattern-0.5.7/nepattern/main.py` & `nepattern-0.5.8/nepattern/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     from typing import Annotated, get_args, get_origin  # type: ignore
 except ImportError:
     from typing_extensions import Annotated, get_args, get_origin
 
 
 from .context import global_patterns, all_patterns
 from .core import BasePattern, MatchMode
-from .base import UnionPattern, MappingPattern, SequencePattern, RegexPattern, SwitchPattern
+from .base import UnionPattern, MappingPattern, SequencePattern, RegexPattern, SwitchPattern, DirectPattern
 from .util import AllParam, GenericAlias, RawStr, CGenericAlias
 
 _Contents = (Union, types.UnionType, Literal) if sys.version_info >= (3, 10) else (Union, Literal)  # pragma: no cover
 
 
 AnyOne = BasePattern(r".+", MatchMode.KEEP, Any, alias="any")
 """匹配任意内容的表达式"""
@@ -215,21 +215,25 @@
             else [anno],
             origin=Any if sig.return_annotation == Empty else sig.return_annotation,
             converter=item if len(sig.parameters) == 2 else lambda _, x: item(x),
             model=MatchMode.TYPE_CONVERT,
         )
     if isinstance(item, str):
         if item.startswith("re:"):
-            return RegexPattern(item[3:])
+            pat = item[3:]
+            return BasePattern(pat, alias=f"'{pat}'")
+        if item.startswith("rep:"):
+            pat = item[4:]
+            return RegexPattern(pat, alias=f"'{pat}'")
         if "|" in item:
             names = item.split("|")
             return UnionPattern(all_patterns().get(i, i) for i in names if i)
-        return BasePattern(item, alias=f"'{item}'")
+        return DirectPattern(item)
     if isinstance(item, RawStr):
-        return BasePattern(item.value, alias=f"'{item.value}'")
+        return DirectPattern(item.value, alias=f"'{item.value}'")
     if isinstance(
         item, (list, tuple, set, ABCSeq, ABCMuSeq, ABCSet, ABCMuSet)
     ):  # Args[foo, [123, int]]
         return UnionPattern(
             map(lambda x: type_parser(x) if inspect.isclass(x) else x, item)
         )
     if isinstance(item, (dict, ABCMap, ABCMuMap)):
```

### Comparing `nepattern-0.5.7/nepattern/util.py` & `nepattern-0.5.8/nepattern/util.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.7/pyproject.toml` & `nepattern-0.5.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nepattern"
-version = "0.5.7"
+version = "0.5.8"
 description = "a complex pattern, support typing"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "typing-extensions>=4.5.0",
     "tarina>=0.3.3",
```

### Comparing `nepattern-0.5.7/README.md` & `nepattern-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.7/PKG-INFO` & `nepattern-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nepattern
-Version: 0.5.7
+Version: 0.5.8
 Summary: a complex pattern, support typing
 License: MIT
 Keywords: typing,pattern,converter,validator
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

