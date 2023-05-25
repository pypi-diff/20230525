# Comparing `tmp/einsum_pipe-0.2.2.tar.gz` & `tmp/einsum_pipe-0.3.0.tar.gz`

## Comparing `einsum_pipe-0.2.2.tar` & `einsum_pipe-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,16 @@
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/TODO
--rwxr-xr-x   0        0        0     2960 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/temp.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/.vscode/settings.json
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/src/einsum_pipe/__init__.py
--rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/src/einsum_pipe/einsum_pipe.py
--rw-r--r--   0        0        0    10453 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/src/einsum_pipe/einsum_script.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/src/einsum_pipe/ops.py
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/tests/test_einsum_pipe.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/tests/test_ops.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/LICENSE
--rw-r--r--   0        0        0     4991 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/README.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 einsum_pipe-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 einsum_pipe-0.3.0/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 einsum_pipe-0.3.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 einsum_pipe-0.3.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 einsum_pipe-0.3.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 einsum_pipe-0.3.0/.vscode/settings.json
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 einsum_pipe-0.3.0/src/einsum_pipe/__init__.py
+-rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 einsum_pipe-0.3.0/src/einsum_pipe/einsum_pipe.py
+-rw-r--r--   0        0        0    10441 2020-02-02 00:00:00.000000 einsum_pipe-0.3.0/src/einsum_pipe/einsum_script.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 einsum_pipe-0.3.0/src/einsum_pipe/ops.py
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 einsum_pipe-0.3.0/tests/test_einsum_pipe.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 einsum_pipe-0.3.0/tests/test_ops.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 einsum_pipe-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 einsum_pipe-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4991 2020-02-02 00:00:00.000000 einsum_pipe-0.3.0/README.md
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 einsum_pipe-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 einsum_pipe-0.3.0/PKG-INFO
```

### Comparing `einsum_pipe-0.2.2/src/einsum_pipe/einsum_pipe.py` & `einsum_pipe-0.3.0/src/einsum_pipe/einsum_pipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from functools import reduce
 import itertools
 import math
 from typing import Callable, Dict, List, Optional, Tuple, Union, cast, overload
 
 import numpy as np
 from .einsum_script import EinsumScript, IncompatibleShapeError
+import opt_einsum
 
 Shape = Tuple[int, ...]
 Subscript = Union[Shape, str, Callable[[List[Shape]],
                                        'Subscript'], List['Subscript'], Tuple['Subscript', ...]]
 
 
 class _ScriptAdder:
@@ -153,10 +154,11 @@
 
     ops_iter = iter(ops)
     state = next(ops_iter)
 
     for script in output_scripts:
         reshaped_ops = [np.reshape(op, shape)
                         for shape, op in zip(script.input_shapes, itertools.chain([state], ops_iter))]
-        state = np.einsum(str(script), *reshaped_ops, **kwargs)
+        state = cast(np.ndarray, opt_einsum.contract(
+            str(script), *reshaped_ops, **kwargs))
 
     return state.reshape(cast(Shape, output_shape))
```

### Comparing `einsum_pipe-0.2.2/src/einsum_pipe/einsum_script.py` & `einsum_pipe-0.3.0/src/einsum_pipe/einsum_script.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 import copy
 import math
-from typing import Generator, List, NamedTuple, Optional, Tuple, TypeVar
+from typing import Generator, List, Optional, Tuple, TypeVar
 
 
 class EinsumComp:
     def __init__(self, size: int, parsed_from: Optional[str] = None) -> None:
         self.size = size
         self._parsed_from = parsed_from
```

### Comparing `einsum_pipe-0.2.2/src/einsum_pipe/ops.py` & `einsum_pipe-0.3.0/src/einsum_pipe/ops.py`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.2.2/tests/test_einsum_pipe.py` & `einsum_pipe-0.3.0/tests/test_einsum_pipe.py`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.2.2/tests/test_ops.py` & `einsum_pipe-0.3.0/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.2.2/LICENSE` & `einsum_pipe-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.2.2/README.md` & `einsum_pipe-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.2.2/pyproject.toml` & `einsum_pipe-0.3.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "einsum_pipe"
-version = "0.2.2"
+version = "0.3.0"
 authors = [
   { name="David Armstrong" },
 ]
 description = "A Python package to compile multiple Numpy einsum operations into one"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "numpy"
+    "numpy",
+    "opt_einsum"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/davystrong/Einsum-Pipe"
 "Bug Tracker" = "https://github.com/davystrong/Einsum-Pipe/issues"
```

### Comparing `einsum_pipe-0.2.2/PKG-INFO` & `einsum_pipe-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: einsum_pipe
-Version: 0.2.2
+Version: 0.3.0
 Summary: A Python package to compile multiple Numpy einsum operations into one
 Project-URL: Homepage, https://github.com/davystrong/Einsum-Pipe
 Project-URL: Bug Tracker, https://github.com/davystrong/Einsum-Pipe/issues
 Author: David Armstrong
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: numpy
+Requires-Dist: opt-einsum
 Description-Content-Type: text/markdown
 
 # Einsum Pipe
 
 A Python package to compile multiple Numpy [einsum](https://numpy.org/doc/stable/reference/generated/numpy.einsum.html) operations into one.
 
 ## Installation
```

