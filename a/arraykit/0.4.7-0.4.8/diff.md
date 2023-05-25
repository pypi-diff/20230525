# Comparing `tmp/arraykit-0.4.7.tar.gz` & `tmp/arraykit-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraykit-0.4.7.tar", last modified: Wed May 24 20:50:23 2023, max compression
+gzip compressed data, was "arraykit-0.4.8.tar", last modified: Thu May 25 00:03:35 2023, max compression
```

## Comparing `arraykit-0.4.7.tar` & `arraykit-0.4.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:50:23.990385 arraykit-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-24 20:50:19.000000 arraykit-0.4.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-24 20:50:19.000000 arraykit-0.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-24 20:50:23.990385 arraykit-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-05-24 20:50:19.000000 arraykit-0.4.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:50:23.986385 arraykit-0.4.7/arraykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-24 20:50:23.000000 arraykit-0.4.7/arraykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-24 20:50:23.000000 arraykit-0.4.7/arraykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:50:23.000000 arraykit-0.4.7/arraykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-24 20:50:23.000000 arraykit-0.4.7/arraykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 20:50:23.000000 arraykit-0.4.7/arraykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:50:23.990385 arraykit-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-24 20:50:19.000000 arraykit-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:50:23.990385 arraykit-0.4.7/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-24 20:50:19.000000 arraykit-0.4.7/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   194111 2023-05-24 20:50:19.000000 arraykit-0.4.7/src/_arraykit.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:50:23.990385 arraykit-0.4.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-24 20:50:19.000000 arraykit-0.4.7/test/test_array_go.py
--rw-r--r--   0 runner    (1001) docker     (123)    29625 2023-05-24 20:50:19.000000 arraykit-0.4.7/test/test_block_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    49054 2023-05-24 20:50:19.000000 arraykit-0.4.7/test/test_delimited_to_arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-24 20:50:19.000000 arraykit-0.4.7/test/test_delimited_to_arrays_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-24 20:50:19.000000 arraykit-0.4.7/test/test_delimited_to_arrays_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-24 20:50:19.000000 arraykit-0.4.7/test/test_pyi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-24 20:50:19.000000 arraykit-0.4.7/test/test_split_after_count.py
--rw-r--r--   0 runner    (1001) docker     (123)    28073 2023-05-24 20:50:19.000000 arraykit-0.4.7/test/test_type_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    27668 2023-05-24 20:50:19.000000 arraykit-0.4.7/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:03:35.083628 arraykit-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-25 00:03:26.000000 arraykit-0.4.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-25 00:03:26.000000 arraykit-0.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-25 00:03:35.083628 arraykit-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-25 00:03:26.000000 arraykit-0.4.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:03:35.079627 arraykit-0.4.8/arraykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-25 00:03:34.000000 arraykit-0.4.8/arraykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-25 00:03:35.000000 arraykit-0.4.8/arraykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 00:03:34.000000 arraykit-0.4.8/arraykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 00:03:34.000000 arraykit-0.4.8/arraykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 00:03:34.000000 arraykit-0.4.8/arraykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 00:03:35.083628 arraykit-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-25 00:03:26.000000 arraykit-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:03:35.079627 arraykit-0.4.8/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-25 00:03:26.000000 arraykit-0.4.8/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   194087 2023-05-25 00:03:26.000000 arraykit-0.4.8/src/_arraykit.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:03:35.083628 arraykit-0.4.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-25 00:03:26.000000 arraykit-0.4.8/test/test_array_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29654 2023-05-25 00:03:26.000000 arraykit-0.4.8/test/test_block_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49054 2023-05-25 00:03:26.000000 arraykit-0.4.8/test/test_delimited_to_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-25 00:03:26.000000 arraykit-0.4.8/test/test_delimited_to_arrays_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-25 00:03:26.000000 arraykit-0.4.8/test/test_delimited_to_arrays_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-25 00:03:26.000000 arraykit-0.4.8/test/test_pyi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-25 00:03:26.000000 arraykit-0.4.8/test/test_split_after_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28073 2023-05-25 00:03:26.000000 arraykit-0.4.8/test/test_type_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29644 2023-05-25 00:03:26.000000 arraykit-0.4.8/test/test_util.py
```

### Comparing `arraykit-0.4.7/LICENSE.txt` & `arraykit-0.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.7/PKG-INFO` & `arraykit-0.4.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.4.7
+Version: 0.4.8
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
```

### Comparing `arraykit-0.4.7/README.rst` & `arraykit-0.4.8/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,19 @@
 - NumPy >= 1.18.5
 
 
 
 What is New in ArrayKit
 -------------------------
 
+0.4.8
+............
+
+Restored behavior of ``Blockndex.rows`` to return -1 when ``BlockIndex`` has zero rows.
+
 
 0.4.7
 ............
 
 Added ``BlockIndex.iter_block()``.
 
 Corrected issue in ``BlockIndex.shape`` when the ``BlockIndex`` has zero rows.
```

### Comparing `arraykit-0.4.7/arraykit.egg-info/PKG-INFO` & `arraykit-0.4.8/arraykit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.4.7
+Version: 0.4.8
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
```

### Comparing `arraykit-0.4.7/setup.py` & `arraykit-0.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import site
 import os
 import typing as tp
 from setuptools import Extension  # type: ignore
 from setuptools import setup
 from pathlib import Path
 
-AK_VERSION = '0.4.7'
+AK_VERSION = '0.4.8'
 
 def get_long_description() -> str:
     return '''The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
 
 Code: https://github.com/static-frame/arraykit
 
 Packages: https://pypi.org/project/arraykit
```

### Comparing `arraykit-0.4.7/src/__init__.py` & `arraykit-0.4.8/src/__init__.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.7/src/_arraykit.c` & `arraykit-0.4.8/src/_arraykit.c`

 * *Files 0% similar despite different names*

```diff
@@ -5419,35 +5419,35 @@
     BlockIndex_init((PyObject*)self, state, NULL);
     Py_RETURN_NONE;
 }
 
 //------------------------------------------------------------------------------
 // getters
 
-// Never expose a negative row value to the caller
-#define AK_BI_ROWS(rows) ((rows) < 0 ? 0 : (rows))
-
+// In a shape tuple, rows will never be negative.
 static PyObject *
 BlockIndex_shape_getter(BlockIndexObject *self, void* Py_UNUSED(closure))
 {
     if (self->shape == NULL || self->shape_recache) {
         Py_XDECREF(self->shape); // get rid of old if it exists
         self->shape = AK_build_pair_ssize_t(
-                AK_BI_ROWS(self->row_count),
+                self->row_count < 0 ? 0 : self->row_count,
                 self->bir_count);
     }
     // shape is not null and shape_recache is false
     Py_INCREF(self->shape); // for caller
     self->shape_recache = false;
     return self->shape;
 }
 
+
+// Unset rows will be -1.
 static PyObject *
 BlockIndex_rows_getter(BlockIndexObject *self, void* Py_UNUSED(closure)){
-    return PyLong_FromSsize_t(AK_BI_ROWS(self->row_count));
+    return PyLong_FromSsize_t(self->row_count);
 }
 
 static PyObject *
 BlockIndex_columns_getter(BlockIndexObject *self, void* Py_UNUSED(closure)){
     return PyLong_FromSsize_t(self->bir_count);
 }
```

### Comparing `arraykit-0.4.7/test/test_array_go.py` & `arraykit-0.4.8/test/test_array_go.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.7/test/test_block_index.py` & `arraykit-0.4.8/test/test_block_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -850,15 +850,15 @@
         self.assertEqual(list(bi1.iter_block()), [(i, slc) for i in range(8)])
 
     #---------------------------------------------------------------------------
 
     def test_block_index_shape_a(self) -> None:
         bi1 = BlockIndex()
         self.assertEqual(bi1.shape, (0, 0))
-        self.assertEqual(bi1.rows, 0)
+        self.assertEqual(bi1.rows, -1) # kept to show no assignemt
 
         bi1.register(np.array(()).reshape(2,0))
         self.assertEqual(bi1.shape, (2, 0))
         self.assertEqual(bi1.rows, 2)
 
         with self.assertRaises(ErrorInitTypeBlocks):
             bi1.register(np.array(()).reshape(3,0))
```

### Comparing `arraykit-0.4.7/test/test_delimited_to_arrays.py` & `arraykit-0.4.8/test/test_delimited_to_arrays.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.7/test/test_delimited_to_arrays_integration.py` & `arraykit-0.4.8/test/test_delimited_to_arrays_integration.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.7/test/test_delimited_to_arrays_property.py` & `arraykit-0.4.8/test/test_delimited_to_arrays_property.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.7/test/test_pyi.py` & `arraykit-0.4.8/test/test_pyi.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.7/test/test_split_after_count.py` & `arraykit-0.4.8/test/test_split_after_count.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.7/test/test_type_discovery.py` & `arraykit-0.4.8/test/test_type_discovery.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.7/test/test_util.py` & `arraykit-0.4.8/test/test_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -740,10 +740,73 @@
                 (slice(97, 6, -7), 101),
                 ):
             self.assertEqual(
                 slice_to_ascending_slice(slc, size),
                 slice_to_ascending_slice_ref(slc, size),
                 )
 
+    def test_slice_to_ascending_slice_f(self) -> None:
+
+        a1 = np.arange(10)
+
+        def compare(slc: slice) -> None:
+            slc_asc = slice_to_ascending_slice(slc, len(a1))
+            self.assertEqual(sorted(a1[slc]), list(a1[slc_asc]))
+
+        compare(slice(4,))
+        compare(slice(6, 1, -1))
+        compare(slice(6, 1, -2))
+        compare(slice(6, None, -3))
+        compare(slice(6, 2, -2))
+        compare(slice(None, 1, -1))
+
+    def test_slice_to_ascending_slice_g(self) -> None:
+        self.assertEqual(
+            slice_to_ascending_slice(slice(3, None, -1), 10),
+            slice(0, 4, None)
+            )
+        self.assertEqual(
+            slice_to_ascending_slice(slice(3, None, -3), 10),
+            slice(0, 4, 3)
+            )
+        self.assertEqual(
+            slice_to_ascending_slice(slice(-3, 0, -1), 10),
+            slice(1, 8, None)
+            )
+        self.assertEqual(
+            slice_to_ascending_slice(slice(-3, None, -1), 10),
+            slice(0, 8, None)
+            )
+        self.assertEqual(
+            slice_to_ascending_slice(slice(-3, 0, -2), 10),
+            slice(1, 8, 2)
+            )
+        self.assertEqual(
+            slice_to_ascending_slice(slice(-3, None, -2), 10),
+            slice(1, 8, 2)
+            )
+        self.assertEqual(
+            slice_to_ascending_slice(slice(-3, None, -6), 10),
+            slice(1, 8, 6)
+            )
+
+    def test_slice_to_ascending_slice_h(self) -> None:
+        self.assertEqual(
+            slice_to_ascending_slice(slice(-9, -1, 1), 10),
+            slice(-9, -1, 1) # ascenidng
+            )
+        self.assertEqual(
+            slice_to_ascending_slice(slice(-9, -1, -1), 10),
+            slice(2, 2, None) # ascending start stop, descending
+            )
+
+    def test_slice_to_ascending_slice_i(self) -> None:
+        self.assertEqual(
+            slice_to_ascending_slice(slice(1, -10, -1), 10), # [1]
+            slice(1, 2, None)
+            )
+
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

