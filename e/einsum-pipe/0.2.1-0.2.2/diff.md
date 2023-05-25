# Comparing `tmp/einsum_pipe-0.2.1.tar.gz` & `tmp/einsum_pipe-0.2.2.tar.gz`

## Comparing `einsum_pipe-0.2.1.tar` & `einsum_pipe-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/.vscode/settings.json
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/src/einsum_pipe/__init__.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/src/einsum_pipe/bidict.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/src/einsum_pipe/einsum_pipe.py
--rw-r--r--   0        0        0     9847 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/src/einsum_pipe/einsum_script.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/src/einsum_pipe/ops.py
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/tests/test_einsum_pipe.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/tests/test_ops.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/LICENSE
--rw-r--r--   0        0        0     4991 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/README.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/TODO
+-rwxr-xr-x   0        0        0     2960 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/temp.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/.vscode/settings.json
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/src/einsum_pipe/__init__.py
+-rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/src/einsum_pipe/einsum_pipe.py
+-rw-r--r--   0        0        0    10453 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/src/einsum_pipe/einsum_script.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/src/einsum_pipe/ops.py
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/tests/test_einsum_pipe.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/tests/test_ops.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4991 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/README.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/PKG-INFO
```

### Comparing `einsum_pipe-0.2.1/src/einsum_pipe/einsum_script.py` & `einsum_pipe-0.2.2/src/einsum_pipe/einsum_script.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 import copy
 import math
-from typing import Generator, List, Optional, Tuple, TypeVar, Union, cast
-from .bidict import _BiDict
+from typing import Generator, List, NamedTuple, Optional, Tuple, TypeVar
 
 
 class EinsumComp:
-    def __init__(self, size: int) -> None:
+    def __init__(self, size: int, parsed_from: Optional[str] = None) -> None:
         self.size = size
+        self._parsed_from = parsed_from
 
 
-class NullTag:
-    pass
+class IncompatibleShapeError(Exception):
+    def __init__(self, shape_a: Tuple[int, ...], shape_b: Tuple[int, ...]) -> None:
+        message = f'Incompatible shapes: {shape_a} vs {shape_b}'
+        super().__init__(message)
 
 
 def _get_char(index: int) -> str:
     assert index < 26*2
     return chr((ord('a') if index < 26 else (ord('A') - 26)) + index)
 
 
@@ -26,48 +28,48 @@
         self._parsed_script: Optional[str] = None
 
     @classmethod
     def parse(cls, input_shapes: List[List[int]], subscripts: str) -> EinsumScript:
         parsed_subscripts = subscripts
         subscripts = subscripts.replace(' ', '')
         # Easier to deal with broadcasting as a single character
-        subscripts = subscripts.replace('...', '?')
+        subscripts = subscripts.replace('...', '.')
         # The broadcasting character is automatically sorted to the start
         letters = sorted(subscripts.replace(',', '').replace('->', ''))
         if '->' not in subscripts:
             output_letters = [l for l in letters if l ==
-                              '?' or letters.count(l) == 1]
-            if (bc_count := output_letters.count('?')) > 1:
+                              '.' or letters.count(l) == 1]
+            if (bc_count := output_letters.count('.')) > 1:
                 output_letters = output_letters[bc_count - 1:]
             subscripts += '->' + ''.join(output_letters)
-        letter_dict = {v: EinsumComp(0) for v in set(letters) if v != '?'}
+        letter_dict = {v: EinsumComp(0, v) for v in set(letters) if v != '.'}
 
         inputs_subs, output_subs = subscripts.split('->')
         inputs: List[List[EinsumComp]] = []
         broadcast_comps: List[EinsumComp] = []
         assert len(inputs_subs.split(',')) == len(
             input_shapes), f'''Error while parsing "{subscripts}" with input shapes {input_shapes}: insuficient input shapes found for number of references in subscripts!'''
         for sub, shape in zip(inputs_subs.split(','), input_shapes):
             inputs.append([])
             for c in sub:
-                if c == '?':
+                if c == '.':
                     # Broadcasting works from the last axis to the first and shares these axes with other broadcasts
                     undefined_axes = len(shape) - (len(sub) - 1)
                     for _ in range(undefined_axes - len(broadcast_comps)):
-                        broadcast_comps.insert(0, EinsumComp(0))
+                        broadcast_comps.insert(0, EinsumComp(0, '...'))
                     if undefined_axes > 0:
                         inputs[-1].extend(broadcast_comps[-undefined_axes:])
                 else:
                     inputs[-1].append(letter_dict[c])
 
         assert len(inputs) > 0
 
         outputs: List[EinsumComp] = []
         for c in output_subs:
-            if c == '?':
+            if c == '.':
                 # All broadcasted axes are added in order
                 outputs.extend(broadcast_comps)
             else:
                 outputs.append(letter_dict[c])
 
         script = EinsumScript(inputs, outputs)
         script._parsed_script = parsed_subscripts
@@ -76,15 +78,16 @@
                 shape), f'Error while parsing "{subscripts}" with input shapes {input_shapes}: {len(inp)} != {len(shape)}'
             for comp, dim in zip(inp, shape):
                 comp.size = dim
 
         return script
 
     def split_comp(self, comp: EinsumComp, part_sizes: List[int]) -> None:
-        repeats = [EinsumComp(size) for size in part_sizes[1:]]
+        repeats = [EinsumComp(size, comp._parsed_from)
+                   for size in part_sizes[1:]]
         comp.size = part_sizes[0]
         for inp in [*self.inputs, self.outputs]:
             for i in range(len(inp)-1, -1, -1):
                 if inp[i] == comp:
                     for rep in repeats[::-1]:
                         inp.insert(i+1, rep)
 
@@ -98,95 +101,100 @@
     def input_shapes(self) -> List[Tuple[int]]:
         return [tuple(comp.size for comp in inp) for inp in self.inputs]
 
     @property
     def output_shape(self) -> Tuple[int]:
         return tuple(comp.size for comp in self.outputs)
 
-    def simplify(self, keep_shapes: Optional[List[Tuple[int, ...]]] = None):
+    def simplify(self):
         # Get sequences (repeated or not) in which each element is unique to the sequence
-        # Basically, run through it as something like a linked list
-        next_map: _BiDict[Union[NullTag, EinsumComp],
-                          Union[NullTag, EinsumComp]] = _BiDict()
-
+        # Might be more efficient with some sort of linked list, but doesn't matter
+        seqs: List[Optional[EinsumComp]] = []
         for comps in [*self.inputs, self.outputs]:
-            prev = NullTag()
-            for comp in comps:
-                if prev in next_map:
-                    if next_map[prev] != comp:
-                        next_map[NullTag()] = next_map[prev]
-                        next_map[NullTag()] = comp
-                        next_map[prev] = NullTag()
-                elif comp in next_map.values():
-                    # Don't need to check if key is already the same as this will be caught by the previous condition
-                    key = next_map.inverse[comp]
-                    next_map[key] = NullTag()
-                    next_map[prev] = NullTag()
-                    next_map[NullTag()] = comp
+            for prev_comp, comp, next_comp in zip([None, *comps[:-1]], comps,  [*comps[1:], None]):
+                if comp not in seqs:
+                    seqs.append(comp)
                 else:
-                    next_map[prev] = comp
-                prev = comp
-            next_map[prev] = NullTag()
-
-        null_tags = [key for key in next_map if isinstance(key, NullTag)]
-        group_pairs: List[Tuple[List[EinsumComp], EinsumComp]] = []
-        for tag in null_tags:
-            seq: List[EinsumComp] = []
-            while not isinstance(next_map[tag], NullTag):
-                seq.append(cast(EinsumComp, next_map[tag]))
-                tag = next_map[tag]
-            if len(seq) > 1:
-                group_pairs.append(
-                    (seq, EinsumComp(math.prod(comp.size for comp in seq))))
+                    seqs.append(None)
+                    i = seqs.index(comp)
+                    if i == len(seqs) - 1 or seqs[i + 1] != next_comp:
+                        seqs.insert(i + 1, None)
+                    if i == 0 or seqs[i - 1] != prev_comp:
+                        seqs.insert(i, None)
+            seqs.append(None)
+
+        groups: List[List[EinsumComp]] = [[]]
+        for comp in seqs:
+            if comp is None:
+                groups.append([])
+            else:
+                groups[-1].append(comp)
+
+        group_pairs = [(group, EinsumComp(math.prod(comp.size for comp in group), ''.join(
+            comp._parsed_from or '.' for comp in group))) for group in groups if len(group) > 1]
+
+        # To check if the sizes before reshaping are the same as the sizes after
+        sizes_before = [math.prod(shape) for shape in [
+            *self.input_shapes, self.output_shape]]
 
         # Replace sequences of comps with their respective group comp
         for comps in [*self.inputs, self.outputs]:
             for group, new_comp in group_pairs:
                 while group[0] in comps:
                     i = comps.index(group[0])
                     comps[i] = new_comp
                     for _ in range(len(group) - 1):
                         comps.pop(i + 1)
 
-        if keep_shapes is not None:
-            for inp, input_shape in zip(self.inputs, keep_shapes):
-                input_shape_iter = iter(input_shape[::-1])
-                inp_in_iter = rev_mut_iter(inp)
-
-                try:
-                    input_shape_val = next(input_shape_iter)
-                    inp_in_val = next(inp_in_iter)
-
-                    while True:
-                        if input_shape_val == inp_in_val.size:
-                            input_shape_val = next(input_shape_iter)
-                            inp_in_val = next(inp_in_iter)
-                        elif input_shape_val > inp_in_val.size:
-                            input_shape_val //= inp_in_val.size
-                            inp_in_val = next(inp_in_iter)
-                        else:
-                            self.split_comp(inp_in_val, [
-                                inp_in_val.size // input_shape_val, input_shape_val])
-                            input_shape_val = next(input_shape_iter)
-                except StopIteration:
-                    pass
+        sizes_after = [math.prod(shape) for shape in [
+            *self.input_shapes, self.output_shape]]
+        assert all(before == after for before,
+                   after in zip(sizes_before, sizes_after)), 'This is a bug. Please submit a bug report!'
 
-    def simplified(self, keep_shape: Optional[List[Tuple[int, ...]]] = None) -> EinsumScript:
+    def simplified(self) -> EinsumScript:
         val = copy.deepcopy(self)
-        val.simplify(keep_shape)
+        val.simplify()
         return val
 
+    def match_splits(self, shapes: List[Optional[Tuple[int, ...]]]) -> None:
+        for inp, input_shape in zip(self.inputs, shapes):
+            if input_shape is None:
+                continue
+            input_shape_iter = iter(input_shape[::-1])
+            inp_in_iter = rev_mut_iter(inp)
+
+            try:
+                input_shape_val = next(input_shape_iter)
+                inp_in_val = next(inp_in_iter)
+
+                while True:
+                    if input_shape_val == inp_in_val.size:
+                        input_shape_val = next(input_shape_iter)
+                        inp_in_val = next(inp_in_iter)
+                    elif input_shape_val > inp_in_val.size:
+                        input_shape_val //= inp_in_val.size
+                        inp_in_val = next(inp_in_iter)
+                    else:
+                        self.split_comp(inp_in_val, [
+                            inp_in_val.size // input_shape_val, input_shape_val])
+                        input_shape_val = next(input_shape_iter)
+            except StopIteration:
+                pass
+
     def __repr__(self) -> str:
         if self._parsed_script is None:
             return f'"{self}"'
         else:
             return f'"{self}" (parsed from "{self._parsed_script}")'
 
     def __str__(self) -> str:
-        comps = list(set(comp for inp in self.inputs for comp in inp))
+        # This is equivalent to using a set except that it preserves order (at least since Python 3.7)
+        # This isn't required but produces more natural string outputs
+        comps: List[EinsumComp] = list(dict.fromkeys(
+            comp for inp in self.inputs for comp in inp).keys())
 
         subs = []
         for inp in self.inputs:
             subs.append(''.join(_get_char(comps.index(comp)) for comp in inp))
 
         output_str = ''.join(_get_char(comps.index(comp))
                              for comp in self.outputs)
@@ -203,22 +211,25 @@
             lhs_out_val = next(lhs_out_iter)
             rhs_in_val = next(rhs_in_iter)
 
             while True:
                 if lhs_out_val.size == rhs_in_val.size:
                     lhs_out_val = next(lhs_out_iter)
                     rhs_in_val = next(rhs_in_iter)
-                elif lhs_out_val.size > rhs_in_val.size:
+                elif lhs_out_val.size % rhs_in_val.size == 0:
                     lhs.split_comp(lhs_out_val, [
                         lhs_out_val.size // rhs_in_val.size, rhs_in_val.size])
                     rhs_in_val = next(rhs_in_iter)
-                else:
+                elif rhs_in_val.size % lhs_out_val.size == 0:
                     rhs.split_comp(rhs_in_val, [
                         rhs_in_val.size // lhs_out_val.size, lhs_out_val.size])
                     lhs_out_val = next(lhs_out_iter)
+                else:
+                    raise IncompatibleShapeError(
+                        lhs.output_shape, rhs.input_shapes[0])
         except StopIteration:
             pass
 
         rhs.remove_ones()
         lhs.remove_ones()
 
         assert len(lhs.outputs) == len(
```

### Comparing `einsum_pipe-0.2.1/src/einsum_pipe/ops.py` & `einsum_pipe-0.2.2/src/einsum_pipe/ops.py`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.2.1/tests/test_einsum_pipe.py` & `einsum_pipe-0.2.2/tests/test_einsum_pipe.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 from einsum_pipe import einsum_pipe, compile_einsum_args
+from einsum_pipe.einsum_script import EinsumScript
 
 
 def einsum_pipe_simple(*args):
     subs = [arg for arg in args if isinstance(arg, (str, list, tuple))]
     ops = [arg for arg in args if not isinstance(arg, (str, list, tuple))]
 
     state: np.ndarray = ops.pop(0)
@@ -120,23 +121,57 @@
     args = [
         '...,...',
         A, B
     ]
     assert np.allclose(einsum_pipe(*args), einsum_pipe_simple(*args))
 
 
+def test_basic_simplify():
+    script_a = EinsumScript.parse([[10, 20, 5, 6]], 'abcd->acd')
+    script_a.simplify()
+    script_b = EinsumScript.parse([[10, 20, 30]], 'abc->ac')
+    assert str(script_a) == str(script_b)
+
+
 def test_simplify():
     # Make a discontiguous array
     A = np.random.rand(3, 3, 3, 9).transpose((0, 2, 1, 3))
     assert not A.flags['CONTIGUOUS']
 
-    script, output_shape = compile_einsum_args(
+    (script, *_), output_shape = compile_einsum_args(
         [(27, 3, 3), 'abc->bc'], [A.shape], True)
-    script_max, output_shape_max = compile_einsum_args(
+    (script_max, *_), output_shape_max = compile_einsum_args(
         [(27, 3, 3), 'abc->bc'], [A.shape], 'max')
 
     X = A.reshape(script.input_shapes[0])
     Y = A.reshape(script_max.input_shapes[0])
     assert all(x == y for x, y in zip(output_shape, output_shape_max))
     assert np.shares_memory(A, X) and not np.shares_memory(A, Y)
     assert np.allclose(einsum_pipe(A, script=script, output_shape=output_shape), einsum_pipe(
         A, script=script_max, output_shape=output_shape_max))
+
+
+def test_incompatible_steps_simple():
+    A = np.random.rand(6)
+    args = [
+        [3, 2],
+        'ij->ji',
+        [3, 2],
+        'ij->ji',
+        A
+    ]
+    assert np.allclose(einsum_pipe(*args), einsum_pipe_simple(*args))
+
+
+def test_incompatible_steps_many():
+    A = np.random.rand(6, 4, 12)
+    B = np.random.rand(4, 4, 12)
+    args = [
+        [3, 2, 4, 12],
+        'ijkl->ji',
+        [6],
+        'i,klm->iklm',
+        [3, 2, 4, 4, 12],
+        'ijklm->jiklm',
+        A, B
+    ]
+    assert np.allclose(einsum_pipe(*args), einsum_pipe_simple(*args))
```

### Comparing `einsum_pipe-0.2.1/tests/test_ops.py` & `einsum_pipe-0.2.2/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.2.1/LICENSE` & `einsum_pipe-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.2.1/README.md` & `einsum_pipe-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.2.1/pyproject.toml` & `einsum_pipe-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "einsum_pipe"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="David Armstrong" },
 ]
 description = "A Python package to compile multiple Numpy einsum operations into one"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `einsum_pipe-0.2.1/PKG-INFO` & `einsum_pipe-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: einsum_pipe
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python package to compile multiple Numpy einsum operations into one
 Project-URL: Homepage, https://github.com/davystrong/Einsum-Pipe
 Project-URL: Bug Tracker, https://github.com/davystrong/Einsum-Pipe/issues
 Author: David Armstrong
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

