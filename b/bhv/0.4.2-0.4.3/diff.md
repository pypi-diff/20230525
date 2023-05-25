# Comparing `tmp/bhv-0.4.2.tar.gz` & `tmp/bhv-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.4.2.tar", last modified: Wed May 24 14:40:26 2023, max compression
+gzip compressed data, was "bhv-0.4.3.tar", last modified: Thu May 25 00:19:32 2023, max compression
```

## Comparing `bhv-0.4.2.tar` & `bhv-0.4.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-24 14:40:26.105539 bhv-0.4.2/
--rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.4.2/LICENSE
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1002 2023-05-24 14:40:26.105539 bhv-0.4.2/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3846 2023-05-23 17:55:24.000000 bhv-0.4.2/README.md
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-24 14:40:26.105539 bhv-0.4.2/bhv/
--rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.4.2/bhv/__init__.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    12999 2023-05-24 13:43:57.000000 bhv-0.4.2/bhv/abstract.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2120 2023-05-09 10:08:10.000000 bhv-0.4.2/bhv/embedding.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11721 2023-05-23 15:35:44.000000 bhv-0.4.2/bhv/np.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-04-24 21:41:56.000000 bhv-0.4.2/bhv/poibin.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.4.2/bhv/positions.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     8293 2023-05-23 15:35:44.000000 bhv-0.4.2/bhv/pytorch.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3360 2023-05-15 19:33:58.000000 bhv-0.4.2/bhv/shared.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1195 2023-05-23 15:35:44.000000 bhv-0.4.2/bhv/slice.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    26856 2023-05-23 16:18:47.000000 bhv-0.4.2/bhv/symbolic.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1747 2023-05-23 17:48:54.000000 bhv-0.4.2/bhv/unification.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3456 2023-05-24 13:05:15.000000 bhv-0.4.2/bhv/vanilla.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      782 2023-04-28 16:55:18.000000 bhv-0.4.2/bhv/visualization.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-24 14:40:26.105539 bhv-0.4.2/bhv.egg-info/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1002 2023-05-24 14:40:26.000000 bhv-0.4.2/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)      363 2023-05-24 14:40:26.000000 bhv-0.4.2/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-05-24 14:40:26.000000 bhv-0.4.2/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       45 2023-05-24 14:40:26.000000 bhv-0.4.2/bhv.egg-info/requires.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-05-24 14:40:26.000000 bhv-0.4.2/bhv.egg-info/top_level.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-05-24 14:40:26.105539 bhv-0.4.2/setup.cfg
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1290 2023-05-24 14:35:52.000000 bhv-0.4.2/setup.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-25 00:19:32.799492 bhv-0.4.3/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.4.3/LICENSE
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1055 2023-05-25 00:19:32.799492 bhv-0.4.3/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3846 2023-05-23 17:55:24.000000 bhv-0.4.3/README.md
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-25 00:19:32.796158 bhv-0.4.3/bhv/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.4.3/bhv/__init__.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    14714 2023-05-24 23:52:24.000000 bhv-0.4.3/bhv/abstract.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2120 2023-05-09 10:08:10.000000 bhv-0.4.3/bhv/embedding.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11951 2023-05-24 23:29:38.000000 bhv-0.4.3/bhv/np.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-04-24 21:41:56.000000 bhv-0.4.3/bhv/poibin.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.4.3/bhv/positions.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     8293 2023-05-23 15:35:44.000000 bhv-0.4.3/bhv/pytorch.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3360 2023-05-15 19:33:58.000000 bhv-0.4.3/bhv/shared.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1195 2023-05-23 15:35:44.000000 bhv-0.4.3/bhv/slice.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    26226 2023-05-25 00:18:10.000000 bhv-0.4.3/bhv/symbolic.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1747 2023-05-23 17:48:54.000000 bhv-0.4.3/bhv/unification.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3456 2023-05-24 13:05:15.000000 bhv-0.4.3/bhv/vanilla.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      782 2023-04-28 16:55:18.000000 bhv-0.4.3/bhv/visualization.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-25 00:19:32.799492 bhv-0.4.3/bhv.egg-info/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1055 2023-05-25 00:19:32.000000 bhv-0.4.3/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      363 2023-05-25 00:19:32.000000 bhv-0.4.3/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-05-25 00:19:32.000000 bhv-0.4.3/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       45 2023-05-25 00:19:32.000000 bhv-0.4.3/bhv.egg-info/requires.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-05-25 00:19:32.000000 bhv-0.4.3/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-05-25 00:19:32.799492 bhv-0.4.3/setup.cfg
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1343 2023-05-24 23:58:58.000000 bhv-0.4.3/setup.py
```

### Comparing `bhv-0.4.2/LICENSE` & `bhv-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bhv-0.4.2/PKG-INFO` & `bhv-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.4.2
+Version: 0.4.3
 Summary: Boolean Hypervectors
+Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `bhv-0.4.2/README.md` & `bhv-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `bhv-0.4.2/bhv/abstract.py` & `bhv-0.4.3/bhv/abstract.py`

 * *Files 20% similar despite different names*

```diff
@@ -349,14 +349,55 @@
 
     @classmethod
     def _majority7_via_3(cls, a: Self, b: Self, c: Self, d: Self, e: Self, f: Self, g: Self) -> Self:
         mdef = cls._majority3(d, e, f)
         mabc = cls._majority3(a, b, c)
         return cls._majority3(g, cls._majority3(c, mdef, cls._majority3(a, b, mdef)), cls._majority3(f, mabc, cls._majority3(d, e, mabc)))
 
+    @classmethod
+    def _majority9_via_3(cls, a: Self, b: Self, c: Self, d: Self, e: Self, f: Self, g: Self, h: Self, i: Self) -> Self:
+        mabc = cls._majority3(a, b, c)
+        mdef = cls._majority3(d, e, f)
+        mghi = cls._majority3(g, h, i)
+
+        l_ = cls._majority3(cls._majority3(c, mdef, b), mdef, a)
+        l = cls._majority3(cls._majority3(i, l_, h), l_, g)
+
+        r_ = cls._majority3(cls._majority3(c, mghi, b), mghi, a)
+        r = cls._majority3(cls._majority3(f, r_, e), r_, d)
+
+        m = cls._majority3(mabc, mdef, mghi)
+        return cls._majority3(l, m, r)
+
+    @classmethod
+    def _majority_via_custom(cls, vs: list[Self]):
+        n = len(vs)
+        if n == 0:
+            return cls.rand()
+        elif n == 1:
+            return vs[0]
+        elif n == 2:
+            return vs[0].select_rand(vs[1])
+        elif n == 3:
+            return cls._majority3(vs[0], vs[1], vs[2])
+        elif n == 4:
+            return cls._majority5_via_3(vs[0], vs[1], vs[2], vs[3], cls.rand())
+        elif n == 5:
+            return cls._majority5_via_3(vs[0], vs[1], vs[2], vs[3], vs[4])
+        elif n == 6:
+            return cls._majority7_via_3(vs[0], vs[1], vs[2], vs[3], vs[4], vs[5], cls.rand())
+        elif n == 7:
+            return cls._majority7_via_3(vs[0], vs[1], vs[2], vs[3], vs[4], vs[5], vs[6])
+        elif n == 8:
+            return cls._majority9_via_3(vs[0], vs[1], vs[2], vs[3], vs[4], vs[5], vs[6], vs[7], cls.rand())
+        elif n == 9:
+            return cls._majority9_via_3(vs[0], vs[1], vs[2], vs[3], vs[4], vs[5], vs[6], vs[7], vs[8])
+        else:
+            raise RuntimeError(f"No optimal implementations beyond MAJORITY-9 (tried to take MAJORITY-{n})")
+
     ZERO: Self
     ONE: Self
     HALF: Self
 
 
 class Permutation:
     @classmethod
```

### Comparing `bhv-0.4.2/bhv/embedding.py` & `bhv-0.4.3/bhv/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.2/bhv/np.py` & `bhv-0.4.3/bhv/np.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,14 +229,21 @@
 
     @classmethod
     def random(cls, active: float) -> 'NumPyPacked64BHV':
         assert 0. <= active <= 1.
         return NumPyBoolBHV.random(active).pack64()
 
     @classmethod
+    def majority(cls, vs: list['NumPyPacked64BHV']) -> 'NumPyPacked64BHV':
+        if len(vs) <= 9:
+            return cls._majority_via_custom(vs)
+        else:
+            return cls._majority_via_unpacked(vs)
+
+    @classmethod
     def _majority_via_unpacked(cls, vs: list['NumPyPacked64BHV']) -> 'NumPyPacked64BHV':
         return NumPyBoolBHV.majority([v.unpack() for v in vs]).pack64()
 
     def swap_halves(self) -> 'NumPyPacked64BHV':
         return self.roll_words(DIMENSION//128)
 
     def rehash(self) -> 'NumPyPacked64BHV':
```

### Comparing `bhv-0.4.2/bhv/poibin.py` & `bhv-0.4.3/bhv/poibin.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.2/bhv/positions.py` & `bhv-0.4.3/bhv/positions.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.2/bhv/pytorch.py` & `bhv-0.4.3/bhv/pytorch.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.2/bhv/shared.py` & `bhv-0.4.3/bhv/shared.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.2/bhv/slice.py` & `bhv-0.4.3/bhv/slice.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.2/bhv/symbolic.py` & `bhv-0.4.3/bhv/symbolic.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,24 +146,25 @@
                 t += c.size(**kwargs)
             counted[id(self)] = t
             return t
 
     def simplify(self, **kwargs):
         x = self
         while True:
-            x_ = x.map(lambda x: x.simplify(**kwargs)).reduce(**kwargs)
-            if x_ is None:
-                raise RuntimeError(f"{x} reduced to non (under {kwargs})")
+            x_ = x.map(lambda c: c.simplify(**kwargs))
+            x_r = x_.reduce(**kwargs)
+            if x_r is not None:
+                x_ = x_r
             if x == x_:
                 return x
             else:
                 x = x_
 
     def reduce(self, **kwargs):
-        return self.map(lambda c: c.simplify(**kwargs))
+        return None
 
     def preorder(self, p=lambda x: True):
         return [self]*p(self) + [v for c in self.children() for v in c.preorder(p)]
 
     def truth_assignments(self, vars):
         configs = bitconfigs(len(vars))
 
@@ -595,17 +596,14 @@
         elif isinstance(self.l, Invert) and isinstance(self.r, Invert):
             return Xor(self.l.v, self.r.v)
         elif isinstance(self.l, And) and isinstance(self.r, And):
             if self.l.l == self.r.l: return And(self.l.l, Xor(self.l.r, self.r.r))
             elif self.l.l == self.r.r: return And(self.l.l, Xor(self.l.r, self.r.l))
             elif self.l.r == self.r.l: return And(self.l.r, Xor(self.l.l, self.r.r))
             elif self.l.r == self.r.r: return And(self.l.r, Xor(self.l.l, self.r.l))
-            else: return Xor(self.l.simplify(**kwargs), self.r.simplify(**kwargs))
-        else:
-            return Xor(self.l.simplify(**kwargs), self.r.simplify(**kwargs))
 
     def expected_active_fraction(self, **kwargs):
         afl = self.l.expected_active_fraction(**kwargs)
         afr = self.r.expected_active_fraction(**kwargs)
         return afl*(1. - afr) + (1. - afl)*afr
 @dataclass
 class And(SymbolicBHV):
@@ -631,16 +629,14 @@
             return self.l
         elif isinstance(self.l, Invert) and self.l.v == self.r:
             return self.ZERO
         elif isinstance(self.r, Invert) and self.r.v == self.l:
             return self.ZERO
         elif isinstance(self.l, Invert) and isinstance(self.r, Invert):
             return Invert(Or(self.l.v, self.r.v))
-        else:
-            return And(self.l.simplify(**kwargs), self.r.simplify(**kwargs))
 
     def expected_active_fraction(self, **kwargs):
         afl = self.l.expected_active_fraction(**kwargs)
         afr = self.r.expected_active_fraction(**kwargs)
         return afl*afr
 @dataclass
 class Or(SymbolicBHV):
@@ -666,16 +662,14 @@
             return self.l
         elif isinstance(self.l, Invert) and self.l.v == self.r:
             return self.ONE
         elif isinstance(self.r, Invert) and self.r.v == self.l:
             return self.ONE
         elif isinstance(self.l, Invert) and isinstance(self.r, Invert):
             return Invert(And(self.l.v, self.r.v))
-        else:
-            return Or(self.l.simplify(**kwargs), self.r.simplify(**kwargs))
 
     def expected_active_fraction(self, **kwargs):
         afl = self.l.expected_active_fraction(**kwargs)
         afr = self.r.expected_active_fraction(**kwargs)
         return 1. - ((1. - afl)*(1. - afr))
 @dataclass
 class Invert(SymbolicBHV):
@@ -694,16 +688,14 @@
     def reduce(self, **kwargs):
         if self.v == self.ONE:
             return self.ZERO
         elif self.v == self.ZERO:
             return self.ONE
         elif isinstance(self.v, Invert):
             return self.v.v
-        else:
-            return Invert(self.v.simplify(**kwargs))
 
     def expected_active_fraction(self, **kwargs):
         return 1. - self.v.expected_active_fraction(**kwargs)
 @dataclass
 class Select(SymbolicBHV):
     cond: SymbolicBHV
     when1: SymbolicBHV
@@ -753,16 +745,14 @@
             elif isinstance(self.when0, Invert) and isinstance(self.when1, Invert):
                 return ~Select(self.cond, self.when1.v, self.when0.v)
             else:
                 if expand_select_xor:
                     return self.when0 ^ (self.cond & (self.when0 ^ self.when1))
                 elif expand_select_and_or:
                     return (self.cond & self.when1) | (~self.cond & self.when0)
-                else:
-                    return Select(self.cond.simplify(**kwargs), self.when1.simplify(**kwargs), self.when0.simplify(**kwargs))
 
     def expected_active_fraction(self, **kwargs):
         afc = self.cond.expected_active_fraction(**kwargs)
         af1 = self.when1.expected_active_fraction(**kwargs)
         af0 = self.when0.expected_active_fraction(**kwargs)
         return afc*af1 + (1. - afc)*af0
 @dataclass
```

### Comparing `bhv-0.4.2/bhv/unification.py` & `bhv-0.4.3/bhv/unification.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.2/bhv/vanilla.py` & `bhv-0.4.3/bhv/vanilla.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.2/bhv/visualization.py` & `bhv-0.4.3/bhv/visualization.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.2/bhv.egg-info/PKG-INFO` & `bhv-0.4.3/bhv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.4.2
+Version: 0.4.3
 Summary: Boolean Hypervectors
+Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `bhv-0.4.2/setup.py` & `bhv-0.4.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.4.2'
+VERSION = '0.4.3'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 setup(
     name="bhv",
     version=VERSION,
     author="Adam Vandervorst",
     author_email="contact@adamv.be",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
+    url="https://github.com/Adam-Vandervorst/PyBHV",
     packages=find_packages(),
     install_requires=[],
     extras_require={
         "torch": ["torch>=2.0.0"],
         "numpy": ["numpy>=1.24.2"],
     },
     keywords='ai binary hypervector hdc bsc',
```

