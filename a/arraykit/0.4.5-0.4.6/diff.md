# Comparing `tmp/arraykit-0.4.5.tar.gz` & `tmp/arraykit-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraykit-0.4.5.tar", last modified: Tue May 23 13:04:19 2023, max compression
+gzip compressed data, was "arraykit-0.4.6.tar", last modified: Tue May 23 23:18:55 2023, max compression
```

## Comparing `arraykit-0.4.5.tar` & `arraykit-0.4.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:04:19.330720 arraykit-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-23 13:04:12.000000 arraykit-0.4.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-23 13:04:12.000000 arraykit-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-23 13:04:19.330720 arraykit-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-23 13:04:12.000000 arraykit-0.4.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:04:19.326720 arraykit-0.4.5/arraykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-23 13:04:19.000000 arraykit-0.4.5/arraykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-23 13:04:19.000000 arraykit-0.4.5/arraykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:04:19.000000 arraykit-0.4.5/arraykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 13:04:19.000000 arraykit-0.4.5/arraykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 13:04:19.000000 arraykit-0.4.5/arraykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:04:19.330720 arraykit-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-23 13:04:12.000000 arraykit-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:04:19.330720 arraykit-0.4.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-23 13:04:12.000000 arraykit-0.4.5/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   189270 2023-05-23 13:04:12.000000 arraykit-0.4.5/src/_arraykit.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:04:19.330720 arraykit-0.4.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-23 13:04:12.000000 arraykit-0.4.5/test/test_array_go.py
--rw-r--r--   0 runner    (1001) docker     (123)    27208 2023-05-23 13:04:12.000000 arraykit-0.4.5/test/test_block_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    49054 2023-05-23 13:04:12.000000 arraykit-0.4.5/test/test_delimited_to_arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-23 13:04:12.000000 arraykit-0.4.5/test/test_delimited_to_arrays_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-23 13:04:12.000000 arraykit-0.4.5/test/test_delimited_to_arrays_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-23 13:04:12.000000 arraykit-0.4.5/test/test_pyi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-23 13:04:12.000000 arraykit-0.4.5/test/test_split_after_count.py
--rw-r--r--   0 runner    (1001) docker     (123)    28073 2023-05-23 13:04:12.000000 arraykit-0.4.5/test/test_type_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    27668 2023-05-23 13:04:12.000000 arraykit-0.4.5/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:18:55.883662 arraykit-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-23 23:18:49.000000 arraykit-0.4.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-23 23:18:49.000000 arraykit-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-23 23:18:55.883662 arraykit-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-23 23:18:49.000000 arraykit-0.4.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:18:55.879662 arraykit-0.4.6/arraykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-23 23:18:55.000000 arraykit-0.4.6/arraykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-23 23:18:55.000000 arraykit-0.4.6/arraykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:18:55.000000 arraykit-0.4.6/arraykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 23:18:55.000000 arraykit-0.4.6/arraykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 23:18:55.000000 arraykit-0.4.6/arraykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 23:18:55.883662 arraykit-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-23 23:18:49.000000 arraykit-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:18:55.879662 arraykit-0.4.6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-23 23:18:49.000000 arraykit-0.4.6/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   190538 2023-05-23 23:18:49.000000 arraykit-0.4.6/src/_arraykit.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:18:55.883662 arraykit-0.4.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-23 23:18:49.000000 arraykit-0.4.6/test/test_array_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28132 2023-05-23 23:18:49.000000 arraykit-0.4.6/test/test_block_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49054 2023-05-23 23:18:49.000000 arraykit-0.4.6/test/test_delimited_to_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-23 23:18:49.000000 arraykit-0.4.6/test/test_delimited_to_arrays_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-23 23:18:49.000000 arraykit-0.4.6/test/test_delimited_to_arrays_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-23 23:18:49.000000 arraykit-0.4.6/test/test_pyi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-23 23:18:49.000000 arraykit-0.4.6/test/test_split_after_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28073 2023-05-23 23:18:49.000000 arraykit-0.4.6/test/test_type_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27668 2023-05-23 23:18:49.000000 arraykit-0.4.6/test/test_util.py
```

### Comparing `arraykit-0.4.5/LICENSE.txt` & `arraykit-0.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.5/PKG-INFO` & `arraykit-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.4.5
+Version: 0.4.6
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
```

### Comparing `arraykit-0.4.5/README.rst` & `arraykit-0.4.6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,20 @@
 - NumPy >= 1.18.5
 
 
 
 What is New in ArrayKit
 -------------------------
 
+0.4.6
+............
+
+Corrected handling of empty selections in ``BlockIndex.iter_contiguous()``.
+
+
 0.4.5
 ............
 
 Corrected handling of ``ascending`` in ``BlockIndex.iter_contiguous()`` with Boolean arrays.
 
 
 0.4.4
```

### Comparing `arraykit-0.4.5/arraykit.egg-info/PKG-INFO` & `arraykit-0.4.6/arraykit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.4.5
+Version: 0.4.6
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
```

### Comparing `arraykit-0.4.5/setup.py` & `arraykit-0.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import site
 import os
 import typing as tp
 from setuptools import Extension  # type: ignore
 from setuptools import setup
 from pathlib import Path
 
-AK_VERSION = '0.4.5'
+AK_VERSION = '0.4.6'
 
 def get_long_description() -> str:
     return '''The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
 
 Code: https://github.com/static-frame/arraykit
 
 Packages: https://pypi.org/project/arraykit
```

### Comparing `arraykit-0.4.5/src/__init__.py` & `arraykit-0.4.6/src/__init__.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.5/src/_arraykit.c` & `arraykit-0.4.6/src/_arraykit.c`

 * *Files 1% similar despite different names*

```diff
@@ -3259,25 +3259,69 @@
                 "unhashable name (type '%s')",
                 Py_TYPE(n)->tp_name);
     }
     Py_INCREF(n);
     return n;
 }
 
+// Returns NULL on error. Returns a new reference.
+static inline PyObject*
+AK_build_pair_ssize_t(Py_ssize_t a, Py_ssize_t b)
+{
+    PyObject* t = PyTuple_New(2);
+    if (t == NULL) {
+        return NULL;
+    }
+    PyObject* py_a = PyLong_FromSsize_t(a);
+    if (py_a == NULL) {
+        Py_DECREF(t);
+        return NULL;
+    }
+    PyObject* py_b = PyLong_FromSsize_t(b);
+    if (py_b == NULL) {
+        Py_DECREF(t);
+        Py_DECREF(py_a);
+        return NULL;
+    }
+    PyTuple_SET_ITEM(t, 0, py_a);
+    PyTuple_SET_ITEM(t, 1, py_b);
+    return t;
+}
+
+// Returns NULL on error. Returns a new reference. Note that a reference is stolen from the PyObject argument.
+static inline PyObject*
+AK_build_pair_ssize_t_slice(Py_ssize_t a, PyObject* py_b)
+{
+    if (py_b == NULL) { // construction failed
+        return NULL;
+    }
+    PyObject* t = PyTuple_New(2);
+    if (t == NULL) {
+        return NULL;
+    }
+    PyObject* py_a = PyLong_FromSsize_t(a);
+    if (py_a == NULL) {
+        Py_DECREF(t);
+        return NULL;
+    }
+    PyTuple_SET_ITEM(t, 0, py_a);
+    PyTuple_SET_ITEM(t, 1, py_b);
+    return t;
+}
+
 // Represent a 1D array as a 2D array with length as rows of a single-column array.
 // https://stackoverflow.com/questions/56182259/how-does-one-acces-numpy-multidimensionnal-array-in-c-extensions
 static PyObject *
 shape_filter(PyObject *Py_UNUSED(m), PyObject *a) {
     AK_CHECK_NUMPY_ARRAY_1D_2D(a);
     PyArrayObject *array = (PyArrayObject *)a;
-
-    npy_intp size0 = PyArray_DIM(array, 0);
+    npy_intp rows = PyArray_DIM(array, 0);
     // If 1D array, set size for axis 1 at 1, else use 2D array to get the size of axis 1
-    npy_intp size1 = PyArray_NDIM(array) == 1 ? 1 : PyArray_DIM(array, 1);
-    return Py_BuildValue("nn", size0, size1);
+    npy_intp cols = PyArray_NDIM(array) == 1 ? 1 : PyArray_DIM(array, 1);
+    return AK_build_pair_ssize_t(rows, cols);
 }
 
 // Reshape if necessary a flat ndim 1 array into a 2D array with one columns and rows of length.
 // related example: https://github.com/RhysU/ar/blob/master/ar-python.cpp
 static PyObject *
 column_2d_filter(PyObject *Py_UNUSED(m), PyObject *a)
 {
@@ -4236,15 +4280,15 @@
 static inline PyObject*
 AK_BI_item(BlockIndexObject* self, Py_ssize_t i) {
     if (!((size_t)i < (size_t)self->bir_count)) {
         PyErr_SetString(PyExc_IndexError, "index out of range");
         return NULL;
     }
     BlockIndexRecord* biri = &self->bir[i];
-    return Py_BuildValue("nn", biri->block, biri->column); // maybe NULL
+    return AK_build_pair_ssize_t(biri->block, biri->column); // may be NULL
 }
 
 //------------------------------------------------------------------------------
 // BI Iterator
 static PyTypeObject BIIterType;
 
 typedef struct BIIterObject {
@@ -4667,30 +4711,30 @@
     Py_ssize_t last_block;
     Py_ssize_t last_column;
     Py_ssize_t next_block;
     Py_ssize_t next_column;
     bool reduce; // optionally reduce slices to integers
 } BIIterContiguousObject;
 
+
+// Create a new contiguous slice iterator. Return NULL on error. Steals a reference to PyObject* iter.
 static PyObject *
 BIIterContiguous_new(BlockIndexObject *bi,
         bool reversed,
         PyObject* iter,
         bool reduce)
 {
     BIIterContiguousObject *bii = PyObject_New(BIIterContiguousObject, &BIIterContiguousType);
     if (!bii) {
         return NULL;
     }
     Py_INCREF((PyObject*)bi);
     bii->bi = bi;
 
-    Py_INCREF(iter);
-    bii->iter = iter;
-
+    bii->iter = iter; // steals ref
     bii->reversed = reversed;
 
     bii->last_block = -1;
     bii->last_column = -1;
     bii->next_block = -1;
     bii->next_column = -1;
     bii->reduce = reduce;
@@ -4742,17 +4786,16 @@
             BIIS_UNKNOWN, // let type be determined by selector
             0);
     if (iter == NULL) {
         return NULL;
     }
     PyObject* biiter = BIIterContiguous_new(self->bi,
             reversed,
-            self->iter,
+            iter, // steals ref
             self->reduce);
-    Py_DECREF(iter);
     return biiter;
 }
 
 static PyObject *
 BIIterContiguous_iternext(BIIterContiguousObject *self)
 {
     Py_ssize_t i = -1;
@@ -4784,15 +4827,18 @@
         }
         if (i == -1) { // end of iteration or error
             if (PyErr_Occurred()) {
                 break;
             }
             // no more pairs, return previous slice_start, flag for end on next call
             self->next_block = -2;
-            return Py_BuildValue("nN", // N steals ref
+            if (self->last_block == -1) { // iter produced no values, terminate
+                break;
+            }
+            return AK_build_pair_ssize_t_slice( // steals ref
                     self->last_block,
                     AK_build_slice_inclusive(slice_start,
                             self->last_column,
                             self->reduce));
         }
         // i is gauranteed to be within the range of self->bit_count at this point; the only source of arbitrary indices is in BIIterSeq_iternext_index, and that function validates the range
         BlockIndexRecord* biri = &self->bi->bir[i];
@@ -4809,15 +4855,15 @@
         if (self->last_block == block && llabs(column - self->last_column) == 1) {
             // contiguious region found, can be postive or negative
             self->last_column = column;
             continue;
         }
         self->next_block = block;
         self->next_column = column;
-        return Py_BuildValue("nN", // N steals ref
+        return AK_build_pair_ssize_t_slice( // steals ref
                 self->last_block,
                 AK_build_slice_inclusive(slice_start,
                         self->last_column,
                         self->reduce));
     }
     return NULL;
 }
@@ -5207,15 +5253,15 @@
     PyObject* list = PyList_New(self->bir_count);
     if (list == NULL) {
         return NULL;
     }
     BlockIndexRecord* bir = self->bir;
 
     for (Py_ssize_t i = 0; i < self->bir_count; i++) {
-        PyObject* item = Py_BuildValue("nn", bir[i].block, bir[i].column);
+        PyObject* item = AK_build_pair_ssize_t(bir[i].block, bir[i].column);
         if (item == NULL) {
             Py_DECREF(list);
             return NULL;
         }
         // set_item steals reference
         PyList_SET_ITEM(list, i, item);
     }
@@ -5244,25 +5290,22 @@
 static PyObject*
 BlockIndex_getstate(BlockIndexObject *self) {
     PyObject* bi = AK_BI_to_bytes(self);
     if (bi == NULL) {
         return NULL;
     }
     PyObject* dt = self->dtype == NULL ? Py_None : (PyObject*) self->dtype;
-
     // state might be NULL on failure; assume exception set
-    PyObject* state = Py_BuildValue("nnnnOO",
+    PyObject* state = Py_BuildValue("nnnnNO", // use N to steal ref of bytes
             self->block_count,
             self->row_count,
             self->bir_count,
             self->bir_capacity,
-            bi,
+            bi,  // stolen new ref
             dt); // increfs passed object
-
-    Py_DECREF(bi);
     return state;
 }
 
 
 // State returned here is a tuple of keys, suitable for usage as an `args` argument.
 static PyObject*
 BlockIndex_setstate(BlockIndexObject *self, PyObject *state)
@@ -5279,15 +5322,15 @@
 // getters
 
 static PyObject *
 BlockIndex_shape_getter(BlockIndexObject *self, void* Py_UNUSED(closure))
 {
     if (self->shape == NULL || self->shape_recache) {
         Py_XDECREF(self->shape); // get rid of old if it exists
-        self->shape = Py_BuildValue("nn", self->row_count, self->bir_count); // new ref
+        self->shape = AK_build_pair_ssize_t(self->row_count, self->bir_count);
     }
     // shape is not null and shape_recache is false
     Py_INCREF(self->shape); // for caller
     self->shape_recache = false;
     return self->shape;
 }
 
@@ -5443,22 +5486,19 @@
             iter_contiguous_kargs_names,
             &selector,
             &ascending,
             &reduce
             )) {
         return NULL;
     }
-
-    // might need to store enum type for branching
     PyObject* iter = BIIterSelector_new(self, selector, 0, BIIS_UNKNOWN, ascending);
     if (iter == NULL) {
         return NULL; // exception set
     }
-    PyObject* biiter = BIIterContiguous_new(self, 0, iter, reduce); // might be NULL, will incref iter
-    Py_DECREF(iter);
+    PyObject* biiter = BIIterContiguous_new(self, 0, iter, reduce); // might be NULL, steals iter ref
     return biiter;
 }
 
 //------------------------------------------------------------------------------
 // slot / method def
 
 static PySequenceMethods BlockIndex_as_sequece = {
```

### Comparing `arraykit-0.4.5/test/test_array_go.py` & `arraykit-0.4.6/test/test_array_go.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.5/test/test_block_index.py` & `arraykit-0.4.6/test/test_block_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -790,7 +790,29 @@
 
         post3 = list(bi1.iter_contiguous(sel, ascending=True, reduce=True))
         self.assertEqual(post3,
                 [(0, 0),
                 (0, 2),
                 (1, 1)])
 
+
+    def test_block_index_iter_contiguous_i1(self) -> None:
+        bi1 = BlockIndex()
+        bi1.register(np.arange(6).reshape(2,3))
+        bi1.register(np.arange(6).reshape(2,3))
+
+        self.assertEqual(list(bi1.iter_select(slice(0, 0))), [])
+        self.assertEqual(list(bi1.iter_contiguous(slice(0, 0))), [])
+
+        self.assertEqual(list(bi1.iter_select(slice(30, 60, 2))), [])
+        self.assertEqual(list(bi1.iter_contiguous(slice(30, 60, 2))), [])
+
+    def test_block_index_iter_contiguous_i2(self) -> None:
+        bi1 = BlockIndex()
+        bi1.register(np.arange(6).reshape(2,3))
+        bi1.register(np.arange(6).reshape(2,3))
+
+        self.assertEqual(list(bi1.iter_select([])), [])
+        self.assertEqual(list(bi1.iter_contiguous([])), [])
+
+        self.assertEqual(list(bi1.iter_select(np.full(len(bi1), False))), [])
+        self.assertEqual(list(bi1.iter_contiguous(np.full(len(bi1), False))), [])
```

### Comparing `arraykit-0.4.5/test/test_delimited_to_arrays.py` & `arraykit-0.4.6/test/test_delimited_to_arrays.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.5/test/test_delimited_to_arrays_integration.py` & `arraykit-0.4.6/test/test_delimited_to_arrays_integration.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.5/test/test_delimited_to_arrays_property.py` & `arraykit-0.4.6/test/test_delimited_to_arrays_property.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.5/test/test_pyi.py` & `arraykit-0.4.6/test/test_pyi.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.5/test/test_split_after_count.py` & `arraykit-0.4.6/test/test_split_after_count.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.5/test/test_type_discovery.py` & `arraykit-0.4.6/test/test_type_discovery.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.5/test/test_util.py` & `arraykit-0.4.6/test/test_util.py`

 * *Files identical despite different names*

