# Comparing `tmp/ziper-0.1.2.tar.gz` & `tmp/ziper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziper-0.1.2.tar", max compression
+gzip compressed data, was "ziper-0.1.3.tar", max compression
```

## Comparing `ziper-0.1.2.tar` & `ziper-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-05-24 02:08:04.922551 ziper-0.1.2/LICENSE
--rw-r--r--   0        0        0      455 2023-05-25 16:43:34.371815 ziper-0.1.2/README.md
--rw-r--r--   0        0        0      480 2023-05-25 16:28:57.315027 ziper-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       31 2023-05-24 02:08:34.702454 ziper-0.1.2/ziper/__init__.py
--rw-r--r--   0        0        0     3353 2023-05-25 16:37:38.342037 ziper-0.1.2/ziper/iter.py
--rw-r--r--   0        0        0        0 2023-05-25 16:49:43.359035 ziper-0.1.2/ziper/py.typed
--rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 ziper-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-24 02:08:04.922551 ziper-0.1.3/LICENSE
+-rw-r--r--   0        0        0      453 2023-05-25 18:54:12.835621 ziper-0.1.3/README.md
+-rw-r--r--   0        0        0      506 2023-05-25 18:17:41.197798 ziper-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-05-24 02:08:34.702454 ziper-0.1.3/ziper/__init__.py
+-rw-r--r--   0        0        0     3540 2023-05-25 18:39:02.895670 ziper-0.1.3/ziper/iter.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:49:43.359035 ziper-0.1.3/ziper/py.typed
+-rw-r--r--   0        0        0     1208 1970-01-01 00:00:00.000000 ziper-0.1.3/PKG-INFO
```

### Comparing `ziper-0.1.2/LICENSE` & `ziper-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ziper-0.1.2/ziper/iter.py` & `ziper-0.1.3/ziper/iter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import itertools
+import more_itertools as mitertools
 
 from typing import (
     Iterable,
     Iterator,
     Generic,
     Optional,
     TypeVar,
@@ -133,7 +134,11 @@
     def inspect(self, f: Fn[T, None]) -> Iter[T]:
 
         def inspector(x: T) -> T:
             f(x)
             return x
 
         return self.map(inspector)
+
+    def chunks(self, size: int) -> Iter[Iter[T]]:
+        it = mitertools.ichunked(self, size)
+        return Iter(it).map(lambda chunk: Iter(chunk))
```

### Comparing `ziper-0.1.2/PKG-INFO` & `ziper-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: ziper
-Version: 0.1.2
+Version: 0.1.3
 Summary: Rust-like iterator for Python
 Home-page: https://github.com/cospectrum/ziper
 License: Apache-2.0
 Author: cospectrum
 Author-email: severinalexeyv@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
 Project-URL: Repository, https://github.com/cospectrum/ziper
 Description-Content-Type: text/markdown
 
 # ziper
 
 Rust-like iterator for Python
 
@@ -38,18 +39,18 @@
 
 ```py
 from ziper import Iter
 
 xs = ['1', '2', 'a', '3', '4', 'b', 'c']
 ys = [6, 7, 8, 9]
 
-result: list = (
+evens: list = (
     Iter(xs)
     .filter(lambda x: x.isdecimal())
     .map(int)
     .chain(ys)
     .filter(lambda x: x % 2 == 0)
     .collect(list)
 )
-assert result == [2, 4, 6, 8]
+assert evens == [2, 4, 6, 8]
 ```
```

