# Comparing `tmp/PyFibreBundle-1.3.2.tar.gz` & `tmp/PyFibreBundle-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFibreBundle-1.3.2.tar", last modified: Thu May 25 16:15:01 2023, max compression
+gzip compressed data, was "PyFibreBundle-1.3.3.tar", last modified: Thu May 25 16:31:47 2023, max compression
```

## Comparing `PyFibreBundle-1.3.2.tar` & `PyFibreBundle-1.3.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:01.709135 PyFibreBundle-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-25 16:15:01.709135 PyFibreBundle-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 16:15:01.709135 PyFibreBundle-1.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:01.705134 PyFibreBundle-1.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:01.705134 PyFibreBundle-1.3.2/src/PyFibreBundle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-25 16:15:01.000000 PyFibreBundle-1.3.2/src/PyFibreBundle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-25 16:15:01.000000 PyFibreBundle-1.3.2/src/PyFibreBundle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:15:01.000000 PyFibreBundle-1.3.2/src/PyFibreBundle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-25 16:15:01.000000 PyFibreBundle-1.3.2/src/PyFibreBundle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 16:15:01.000000 PyFibreBundle-1.3.2/src/PyFibreBundle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:01.709135 PyFibreBundle-1.3.2/src/pybundle/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/src/pybundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/src/pybundle/bundle_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/src/pybundle/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/src/pybundle/core_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/src/pybundle/core_interpolation_numba.py
--rw-r--r--   0 runner    (1001) docker     (123)    24572 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/src/pybundle/mosaic.py
--rw-r--r--   0 runner    (1001) docker     (123)    32763 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/src/pybundle/pybundle.py
--rw-r--r--   0 runner    (1001) docker     (123)    25481 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/src/pybundle/super_res.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/src/pybundle/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:01.709135 PyFibreBundle-1.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_find_cores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_loc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_masking_col.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_mosaic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_mosaic_col.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_processing_im_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_pybundle_oop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_recon_tri_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_recon_tri_interp_col.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_simple_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_simple_processing_col.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_sr_sort_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_super_res.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_super_res_oop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:31:47.818773 PyFibreBundle-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-25 16:31:47.818773 PyFibreBundle-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 16:31:47.818773 PyFibreBundle-1.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:31:47.814773 PyFibreBundle-1.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:31:47.814773 PyFibreBundle-1.3.3/src/PyFibreBundle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-25 16:31:47.000000 PyFibreBundle-1.3.3/src/PyFibreBundle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-25 16:31:47.000000 PyFibreBundle-1.3.3/src/PyFibreBundle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:31:47.000000 PyFibreBundle-1.3.3/src/PyFibreBundle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-25 16:31:47.000000 PyFibreBundle-1.3.3/src/PyFibreBundle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 16:31:47.000000 PyFibreBundle-1.3.3/src/PyFibreBundle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:31:47.818773 PyFibreBundle-1.3.3/src/pybundle/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/src/pybundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/src/pybundle/bundle_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/src/pybundle/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/src/pybundle/core_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/src/pybundle/core_interpolation_numba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24572 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/src/pybundle/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32763 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/src/pybundle/pybundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25481 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/src/pybundle/super_res.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/src/pybundle/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:31:47.818773 PyFibreBundle-1.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/test/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/test/test_find_cores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/test/test_loc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/test/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/test/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/test/test_masking_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/test/test_mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/test/test_mosaic_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/test/test_processing_im_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/test/test_pybundle_oop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/test/test_recon_tri_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/test/test_recon_tri_interp_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/test/test_simple_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/test/test_simple_processing_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/test/test_sr_sort_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/test/test_super_res.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-25 16:31:34.000000 PyFibreBundle-1.3.3/test/test_super_res_oop.py
```

### Comparing `PyFibreBundle-1.3.2/LICENSE` & `PyFibreBundle-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/PKG-INFO` & `PyFibreBundle-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFibreBundle
-Version: 1.3.2
+Version: 1.3.3
 Summary: Image processing of images acquired through fibre imaging bundle, including core removal, mosaicing and super-resolution..
 Author-email: Michael Hughes <m.r.hughes@kent.ac.uk>
 License: MIT License
         
         Copyright (c) [2022] [Michael Hughes]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `PyFibreBundle-1.3.2/README.md` & `PyFibreBundle-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/pyproject.toml` & `PyFibreBundle-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyFibreBundle"
-version = "1.3.2"
+version = "1.3.3"
 description = "Image processing of images acquired through fibre imaging bundle, including core removal, mosaicing and super-resolution.."
 readme = "README.md"
 authors = [{ name = "Michael Hughes", email = "m.r.hughes@kent.ac.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `PyFibreBundle-1.3.2/src/PyFibreBundle.egg-info/PKG-INFO` & `PyFibreBundle-1.3.3/src/PyFibreBundle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFibreBundle
-Version: 1.3.2
+Version: 1.3.3
 Summary: Image processing of images acquired through fibre imaging bundle, including core removal, mosaicing and super-resolution..
 Author-email: Michael Hughes <m.r.hughes@kent.ac.uk>
 License: MIT License
         
         Copyright (c) [2022] [Michael Hughes]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `PyFibreBundle-1.3.2/src/PyFibreBundle.egg-info/SOURCES.txt` & `PyFibreBundle-1.3.3/src/PyFibreBundle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/src/pybundle/__init__.py` & `PyFibreBundle-1.3.3/src/pybundle/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/src/pybundle/bundle_calibration.py` & `PyFibreBundle-1.3.3/src/pybundle/bundle_calibration.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/src/pybundle/core.py` & `PyFibreBundle-1.3.3/src/pybundle/core.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/src/pybundle/core_interpolation.py` & `PyFibreBundle-1.3.3/src/pybundle/core_interpolation.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
      Arguments:
          img         : 2D/3D numpy array
          coreSpacing : float, estimate of the separation between cores in
                        pixels.
      """
      # Pre-filtering helps to minimse noise and reduce efffect of
      # multimodal patterns
-     imgF = pybundle.g_filter(img, coreSpacing/5)
+     imgF = pybundle.g_filter(img.astype('float32'), coreSpacing/5)
 
      # If a colour image, convert to greyscale by taking the maximum value across the channels
      imgF = pybundle.max_channels(imgF)
 
      imgF = (imgF / np.max(imgF) * 255).astype('uint8') 
 
      # Find regional maximum by taking difference between dilated and original
```

### Comparing `PyFibreBundle-1.3.2/src/pybundle/core_interpolation_numba.py` & `PyFibreBundle-1.3.3/src/pybundle/core_interpolation_numba.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/src/pybundle/mosaic.py` & `PyFibreBundle-1.3.3/src/pybundle/mosaic.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/src/pybundle/pybundle.py` & `PyFibreBundle-1.3.3/src/pybundle/pybundle.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/src/pybundle/super_res.py` & `PyFibreBundle-1.3.3/src/pybundle/super_res.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/src/pybundle/utility.py` & `PyFibreBundle-1.3.3/src/pybundle/utility.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/test/test_all.py` & `PyFibreBundle-1.3.3/test/test_all.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/test/test_find_cores.py` & `PyFibreBundle-1.3.3/test/test_find_cores.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/test/test_loc.py` & `PyFibreBundle-1.3.3/test/test_loc.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/test/test_mask.py` & `PyFibreBundle-1.3.3/test/test_mask.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/test/test_masking.py` & `PyFibreBundle-1.3.3/test/test_masking.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/test/test_masking_col.py` & `PyFibreBundle-1.3.3/test/test_masking_col.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/test/test_mosaic.py` & `PyFibreBundle-1.3.3/test/test_mosaic.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/test/test_mosaic_col.py` & `PyFibreBundle-1.3.3/test/test_mosaic_col.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/test/test_processing_im_type.py` & `PyFibreBundle-1.3.3/test/test_processing_im_type.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/test/test_pybundle_oop.py` & `PyFibreBundle-1.3.3/test/test_pybundle_oop.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/test/test_recon_tri_interp.py` & `PyFibreBundle-1.3.3/test/test_recon_tri_interp.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/test/test_recon_tri_interp_col.py` & `PyFibreBundle-1.3.3/test/test_recon_tri_interp_col.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/test/test_simple_processing.py` & `PyFibreBundle-1.3.3/test/test_simple_processing.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/test/test_simple_processing_col.py` & `PyFibreBundle-1.3.3/test/test_simple_processing_col.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/test/test_sr_sort_stack.py` & `PyFibreBundle-1.3.3/test/test_sr_sort_stack.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/test/test_super_res.py` & `PyFibreBundle-1.3.3/test/test_super_res.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.2/test/test_super_res_oop.py` & `PyFibreBundle-1.3.3/test/test_super_res_oop.py`

 * *Files identical despite different names*

