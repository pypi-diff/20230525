# Comparing `tmp/ziper-0.1.0.tar.gz` & `tmp/ziper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziper-0.1.0.tar", max compression
+gzip compressed data, was "ziper-0.1.1.tar", max compression
```

## Comparing `ziper-0.1.0.tar` & `ziper-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-05-24 02:08:04.922551 ziper-0.1.0/LICENSE
--rw-r--r--   0        0        0      434 2023-05-24 02:16:45.886586 ziper-0.1.0/README.md
--rw-r--r--   0        0        0      480 2023-05-24 02:19:42.446758 ziper-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       31 2023-05-24 02:08:34.702454 ziper-0.1.0/ziper/__init__.py
--rw-r--r--   0        0        0     2752 2023-05-24 02:08:34.701829 ziper-0.1.0/ziper/iter.py
--rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 ziper-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-24 02:08:04.922551 ziper-0.1.1/LICENSE
+-rw-r--r--   0        0        0      434 2023-05-24 02:16:45.886586 ziper-0.1.1/README.md
+-rw-r--r--   0        0        0      480 2023-05-25 03:29:08.832474 ziper-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-05-24 02:08:34.702454 ziper-0.1.1/ziper/__init__.py
+-rw-r--r--   0        0        0     3257 2023-05-25 03:28:29.581594 ziper-0.1.1/ziper/iter.py
+-rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 ziper-0.1.1/PKG-INFO
```

### Comparing `ziper-0.1.0/LICENSE` & `ziper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ziper-0.1.0/ziper/iter.py` & `ziper-0.1.1/ziper/iter.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,7 +112,24 @@
 
     def nth(self, n: int) -> Optional[T]:
         return self.skip(n).next()
 
     def for_each(self, f: Fn[T, None]) -> None:
         for x in self:
             f(x)
+
+    def step_by(self, step: int) -> Iter[T]:
+        return Iter(itertools.islice(self, 0, None, step))
+
+    def take_while(self, predicate: Fn[T, bool]) -> Iter[T]:
+        return Iter(itertools.takewhile(predicate, self))
+
+    def skip_while(self, predicate: Fn[T, bool]) -> Iter[T]:
+        return Iter(itertools.dropwhile(predicate, self))
+
+    def inspect(self, f: Fn[T, None]) -> Iter[T]:
+
+        def inspector(x: T) -> T:
+            f(x)
+            return x
+
+        return self.map(inspector)
```

### Comparing `ziper-0.1.0/PKG-INFO` & `ziper-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziper
-Version: 0.1.0
+Version: 0.1.1
 Summary: Rust-like iterator for Python
 Home-page: https://github.com/cospectrum/ziper
 License: Apache-2.0
 Author: cospectrum
 Author-email: severinalexeyv@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

