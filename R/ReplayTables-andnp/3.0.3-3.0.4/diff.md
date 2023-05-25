# Comparing `tmp/ReplayTables-andnp-3.0.3.tar.gz` & `tmp/ReplayTables-andnp-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReplayTables-andnp-3.0.3.tar", last modified: Wed May 17 18:30:23 2023, max compression
+gzip compressed data, was "ReplayTables-andnp-3.0.4.tar", last modified: Thu May 25 16:59:24 2023, max compression
```

## Comparing `ReplayTables-andnp-3.0.3.tar` & `ReplayTables-andnp-3.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0        0 2023-05-17 18:29:50.220763 ReplayTables-andnp-3.0.3/README.md
--rw-r--r--   0        0        0     5167 2023-05-17 18:29:50.220763 ReplayTables-andnp-3.0.3/ReplayTables/Distributions.py
--rw-r--r--   0        0        0     2140 2023-05-17 18:29:50.220763 ReplayTables-andnp-3.0.3/ReplayTables/LagBuffer.py
--rw-r--r--   0        0        0     2392 2023-05-17 18:29:50.220763 ReplayTables-andnp-3.0.3/ReplayTables/PER.py
--rw-r--r--   0        0        0     2964 2023-05-17 18:29:50.220763 ReplayTables-andnp-3.0.3/ReplayTables/PrioritizedHeap.py
--rw-r--r--   0        0        0     3696 2023-05-17 18:29:50.220763 ReplayTables-andnp-3.0.3/ReplayTables/ReplayBuffer.py
--rw-r--r--   0        0        0     8237 2023-05-17 18:29:50.220763 ReplayTables-andnp-3.0.3/ReplayTables/Table.py
--rw-r--r--   0        0        0        0 2023-05-17 18:29:50.220763 ReplayTables-andnp-3.0.3/ReplayTables/__init__.py
--rw-r--r--   0        0        0     3418 2023-05-17 18:29:50.220763 ReplayTables-andnp-3.0.3/ReplayTables/_utils/MemoryWriter.py
--rw-r--r--   0        0        0     5811 2023-05-17 18:29:50.220763 ReplayTables-andnp-3.0.3/ReplayTables/_utils/MinMaxHeap.py
--rw-r--r--   0        0        0     1772 2023-05-17 18:29:50.220763 ReplayTables-andnp-3.0.3/ReplayTables/_utils/RandDict.py
--rw-r--r--   0        0        0     3822 2023-05-17 18:29:50.220763 ReplayTables-andnp-3.0.3/ReplayTables/_utils/SumTree.py
--rw-r--r--   0        0        0        0 2023-05-17 18:29:50.220763 ReplayTables-andnp-3.0.3/ReplayTables/_utils/__init__.py
--rw-r--r--   0        0        0     1356 2023-05-17 18:29:50.220763 ReplayTables-andnp-3.0.3/ReplayTables/_utils/jit.py
--rw-r--r--   0        0        0       58 2023-05-17 18:29:50.220763 ReplayTables-andnp-3.0.3/ReplayTables/_utils/logger.py
--rw-r--r--   0        0        0      886 2023-05-17 18:30:21.039559 ReplayTables-andnp-3.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-17 18:29:50.224763 ReplayTables-andnp-3.0.3/tests/__init__.py
--rw-r--r--   0        0        0     3076 2023-05-17 18:29:50.224763 ReplayTables-andnp-3.0.3/tests/test_LagBuffer.py
--rw-r--r--   0        0        0     2449 2023-05-17 18:29:50.224763 ReplayTables-andnp-3.0.3/tests/test_PER.py
--rw-r--r--   0        0        0     1384 2023-05-17 18:29:50.224763 ReplayTables-andnp-3.0.3/tests/test_PrioritizedHeap.py
--rw-r--r--   0        0        0     2679 2023-05-17 18:29:50.224763 ReplayTables-andnp-3.0.3/tests/test_ReplayBuffer.py
--rw-r--r--   0        0        0     1537 2023-05-17 18:29:50.224763 ReplayTables-andnp-3.0.3/tests/test_Table.py
--rw-r--r--   0        0        0     5619 2023-05-17 18:29:50.224763 ReplayTables-andnp-3.0.3/tests/test_View.py
--rw-r--r--   0        0        0        0 2023-05-17 18:29:50.224763 ReplayTables-andnp-3.0.3/tests/utils/__init__.py
--rw-r--r--   0        0        0     1217 2023-05-17 18:29:50.224763 ReplayTables-andnp-3.0.3/tests/utils/test_MinMaxHeap.py
--rw-r--r--   0        0        0     2998 2023-05-17 18:29:50.224763 ReplayTables-andnp-3.0.3/tests/utils/test_SumTree.py
--rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 ReplayTables-andnp-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/README.md
+-rw-r--r--   0        0        0     5167 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/Distributions.py
+-rw-r--r--   0        0        0     2140 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/LagBuffer.py
+-rw-r--r--   0        0        0     2392 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/PER.py
+-rw-r--r--   0        0        0     2964 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/PrioritizedHeap.py
+-rw-r--r--   0        0        0     3692 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/ReplayBuffer.py
+-rw-r--r--   0        0        0     8237 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/Table.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/__init__.py
+-rw-r--r--   0        0        0     3418 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/_utils/MemoryWriter.py
+-rw-r--r--   0        0        0     5811 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/_utils/MinMaxHeap.py
+-rw-r--r--   0        0        0     1772 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/_utils/RandDict.py
+-rw-r--r--   0        0        0     3822 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/_utils/SumTree.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/_utils/__init__.py
+-rw-r--r--   0        0        0     1356 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/_utils/jit.py
+-rw-r--r--   0        0        0       58 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/_utils/logger.py
+-rw-r--r--   0        0        0      886 2023-05-25 16:59:21.063285 ReplayTables-andnp-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     3076 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/test_LagBuffer.py
+-rw-r--r--   0        0        0     2449 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/test_PER.py
+-rw-r--r--   0        0        0     1384 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/test_PrioritizedHeap.py
+-rw-r--r--   0        0        0     3252 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/test_ReplayBuffer.py
+-rw-r--r--   0        0        0     1537 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/test_Table.py
+-rw-r--r--   0        0        0     5619 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/test_View.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1217 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/utils/test_MinMaxHeap.py
+-rw-r--r--   0        0        0     2998 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/utils/test_SumTree.py
+-rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 ReplayTables-andnp-3.0.4/PKG-INFO
```

### Comparing `ReplayTables-andnp-3.0.3/ReplayTables/Distributions.py` & `ReplayTables-andnp-3.0.4/ReplayTables/Distributions.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.3/ReplayTables/LagBuffer.py` & `ReplayTables-andnp-3.0.4/ReplayTables/LagBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.3/ReplayTables/PER.py` & `ReplayTables-andnp-3.0.4/ReplayTables/PER.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.3/ReplayTables/PrioritizedHeap.py` & `ReplayTables-andnp-3.0.4/ReplayTables/PrioritizedHeap.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.3/ReplayTables/ReplayBuffer.py` & `ReplayTables-andnp-3.0.4/ReplayTables/ReplayBuffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from abc import abstractmethod
-from typing import Any, Dict, Generic, List, NamedTuple, NewType, Tuple, TypeVar, Type, Union, cast
+from typing import Any, Dict, Generic, Iterable, List, NewType, Tuple, TypeVar, Type, Union, cast
 from ReplayTables.Distributions import UniformDistribution
 
-T = TypeVar('T', bound=NamedTuple)
+T = TypeVar('T', bound=Iterable)
 EID = NewType('EID', int)
 EIDS = NewType('EIDS', np.ndarray)
 
 class ReplayBufferInterface(Generic[T]):
     def __init__(self, max_size: int, structure: Type[T], rng: np.random.Generator):
         self._max_size = max_size
         self._structure = cast(Any, structure)
```

### Comparing `ReplayTables-andnp-3.0.3/ReplayTables/Table.py` & `ReplayTables-andnp-3.0.4/ReplayTables/Table.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.3/ReplayTables/_utils/MemoryWriter.py` & `ReplayTables-andnp-3.0.4/ReplayTables/_utils/MemoryWriter.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.3/ReplayTables/_utils/MinMaxHeap.py` & `ReplayTables-andnp-3.0.4/ReplayTables/_utils/MinMaxHeap.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.3/ReplayTables/_utils/RandDict.py` & `ReplayTables-andnp-3.0.4/ReplayTables/_utils/RandDict.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.3/ReplayTables/_utils/SumTree.py` & `ReplayTables-andnp-3.0.4/ReplayTables/_utils/SumTree.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.3/ReplayTables/_utils/jit.py` & `ReplayTables-andnp-3.0.4/ReplayTables/_utils/jit.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.3/pyproject.toml` & `ReplayTables-andnp-3.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "3.0.3"
+version = "3.0.4"
 tag_format = "$version"
 version_files = [
     "pyproject.toml",
 ]
 
 [tool.pdm]
 source = [
@@ -22,15 +22,15 @@
 ]
 
 [tool.mypy]
 mypy_path = "typings"
 
 [project]
 name = "ReplayTables-andnp"
-version = "3.0.3"
+version = "3.0.4"
 description = "A simple replay buffer implementation in python for sampling n-step trajectories"
 authors = [
     { name = "Andy Patterson", email = "andnpatterson@gmail.com" },
 ]
 dependencies = [
     "numba>=0.57",
     "numpy>=1.23.5",
```

### Comparing `ReplayTables-andnp-3.0.3/tests/test_LagBuffer.py` & `ReplayTables-andnp-3.0.4/tests/test_LagBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.3/tests/test_PER.py` & `ReplayTables-andnp-3.0.4/tests/test_PER.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.3/tests/test_PrioritizedHeap.py` & `ReplayTables-andnp-3.0.4/tests/test_PrioritizedHeap.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.3/tests/test_ReplayBuffer.py` & `ReplayTables-andnp-3.0.4/tests/test_ReplayBuffer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 import unittest
 import numpy as np
 import pickle
+from dataclasses import dataclass, fields
 from typing import NamedTuple
 
 from ReplayTables.ReplayBuffer import ReplayBuffer
 
 class Data(NamedTuple):
     a: float | np.ndarray
     b: int | np.ndarray
 
+@dataclass
+class Data2:
+    b: float | np.ndarray
+    c: float | np.ndarray
+
+    def __iter__(self):
+        return (getattr(self, field.name) for field in fields(self))
 
 class TestReplayBuffer(unittest.TestCase):
     def test_simple_buffer(self):
         rng = np.random.default_rng(0)
         buffer = ReplayBuffer(5, Data, rng)
 
         # on creation, the buffer should have no size
@@ -45,14 +53,27 @@
         self.assertEqual(buffer.size(), 5)
 
         samples, _, _ = buffer.sample(1000)
         unique = np.unique(samples.b)
         unique.sort()
         self.assertTrue(np.all(unique == np.array([2, 3, 4, 5, 6])))
 
+        # -------------------------------
+        # Can also handle other iterables
+
+        rng = np.random.default_rng(0)
+        buffer = ReplayBuffer(5, Data2, rng)
+        buffer.add(Data2(1, 2))
+        buffer.add(Data2(2, 3))
+
+        samples, _, _ = buffer.sample(2)
+        self.assertTrue(
+            np.all(samples.b == np.array([2, 2]))
+        )
+
     def test_getitem(self):
         rng = np.random.default_rng(0)
         buffer = ReplayBuffer(10, Data, rng)
 
         for i in range(15):
             buffer.add(Data(a=i, b=2 * i))
```

### Comparing `ReplayTables-andnp-3.0.3/tests/test_Table.py` & `ReplayTables-andnp-3.0.4/tests/test_Table.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.3/tests/test_View.py` & `ReplayTables-andnp-3.0.4/tests/test_View.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.3/tests/utils/test_MinMaxHeap.py` & `ReplayTables-andnp-3.0.4/tests/utils/test_MinMaxHeap.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.3/tests/utils/test_SumTree.py` & `ReplayTables-andnp-3.0.4/tests/utils/test_SumTree.py`

 * *Files identical despite different names*

