# Comparing `tmp/PyFibreBundle-1.3.1.tar.gz` & `tmp/PyFibreBundle-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFibreBundle-1.3.1.tar", last modified: Tue May 23 11:13:37 2023, max compression
+gzip compressed data, was "PyFibreBundle-1.3.2.tar", last modified: Thu May 25 16:15:01 2023, max compression
```

## Comparing `PyFibreBundle-1.3.1.tar` & `PyFibreBundle-1.3.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:13:37.986429 PyFibreBundle-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-23 11:13:37.986429 PyFibreBundle-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 11:13:37.986429 PyFibreBundle-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:13:37.974429 PyFibreBundle-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:13:37.978429 PyFibreBundle-1.3.1/src/PyFibreBundle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-23 11:13:37.000000 PyFibreBundle-1.3.1/src/PyFibreBundle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-23 11:13:37.000000 PyFibreBundle-1.3.1/src/PyFibreBundle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 11:13:37.000000 PyFibreBundle-1.3.1/src/PyFibreBundle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-23 11:13:37.000000 PyFibreBundle-1.3.1/src/PyFibreBundle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 11:13:37.000000 PyFibreBundle-1.3.1/src/PyFibreBundle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:13:37.982429 PyFibreBundle-1.3.1/src/pybundle/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/src/pybundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/src/pybundle/bundle_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/src/pybundle/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    17767 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/src/pybundle/core_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/src/pybundle/core_interpolation_numba.py
--rw-r--r--   0 runner    (1001) docker     (123)    24572 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/src/pybundle/mosaic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28182 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/src/pybundle/pybundle.py
--rw-r--r--   0 runner    (1001) docker     (123)    25481 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/src/pybundle/super_res.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/src/pybundle/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:13:37.986429 PyFibreBundle-1.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_find_cores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_loc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_masking_col.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_mosaic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_mosaic_col.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_processing_im_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_pybundle_oop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_recon_tri_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_recon_tri_interp_col.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_simple_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_simple_processing_col.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_sr_sort_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_super_res.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_super_res_oop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:01.709135 PyFibreBundle-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-25 16:15:01.709135 PyFibreBundle-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 16:15:01.709135 PyFibreBundle-1.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:01.705134 PyFibreBundle-1.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:01.705134 PyFibreBundle-1.3.2/src/PyFibreBundle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-25 16:15:01.000000 PyFibreBundle-1.3.2/src/PyFibreBundle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-25 16:15:01.000000 PyFibreBundle-1.3.2/src/PyFibreBundle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:15:01.000000 PyFibreBundle-1.3.2/src/PyFibreBundle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-25 16:15:01.000000 PyFibreBundle-1.3.2/src/PyFibreBundle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 16:15:01.000000 PyFibreBundle-1.3.2/src/PyFibreBundle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:01.709135 PyFibreBundle-1.3.2/src/pybundle/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/src/pybundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/src/pybundle/bundle_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/src/pybundle/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/src/pybundle/core_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/src/pybundle/core_interpolation_numba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24572 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/src/pybundle/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32763 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/src/pybundle/pybundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25481 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/src/pybundle/super_res.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-25 16:14:46.000000 PyFibreBundle-1.3.2/src/pybundle/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:01.709135 PyFibreBundle-1.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_find_cores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_loc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_masking_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_mosaic_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_processing_im_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_pybundle_oop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_recon_tri_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_recon_tri_interp_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_simple_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_simple_processing_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_sr_sort_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_super_res.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-25 16:14:47.000000 PyFibreBundle-1.3.2/test/test_super_res_oop.py
```

### Comparing `PyFibreBundle-1.3.1/LICENSE` & `PyFibreBundle-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/PKG-INFO` & `PyFibreBundle-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFibreBundle
-Version: 1.3.1
+Version: 1.3.2
 Summary: Image processing of images acquired through fibre imaging bundle, including core removal, mosaicing and super-resolution..
 Author-email: Michael Hughes <m.r.hughes@kent.ac.uk>
 License: MIT License
         
         Copyright (c) [2022] [Michael Hughes]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `PyFibreBundle-1.3.1/README.md` & `PyFibreBundle-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/pyproject.toml` & `PyFibreBundle-1.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyFibreBundle"
-version = "1.3.1"
+version = "1.3.2"
 description = "Image processing of images acquired through fibre imaging bundle, including core removal, mosaicing and super-resolution.."
 readme = "README.md"
 authors = [{ name = "Michael Hughes", email = "m.r.hughes@kent.ac.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `PyFibreBundle-1.3.1/src/PyFibreBundle.egg-info/PKG-INFO` & `PyFibreBundle-1.3.2/src/PyFibreBundle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFibreBundle
-Version: 1.3.1
+Version: 1.3.2
 Summary: Image processing of images acquired through fibre imaging bundle, including core removal, mosaicing and super-resolution..
 Author-email: Michael Hughes <m.r.hughes@kent.ac.uk>
 License: MIT License
         
         Copyright (c) [2022] [Michael Hughes]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `PyFibreBundle-1.3.1/src/PyFibreBundle.egg-info/SOURCES.txt` & `PyFibreBundle-1.3.2/src/PyFibreBundle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/src/pybundle/__init__.py` & `PyFibreBundle-1.3.2/src/pybundle/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/src/pybundle/bundle_calibration.py` & `PyFibreBundle-1.3.2/src/pybundle/bundle_calibration.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/src/pybundle/core.py` & `PyFibreBundle-1.3.2/src/pybundle/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -256,33 +256,46 @@
 
 
 
 ################ MASKING AND CROPPING ###################################
     
 
 def crop_rect(img, loc):
-    """Extracts a square around the bundle using specified co-ordinates.
+    """Extracts a square around the bundle using specified co-ordinates. If the
+    rectange is larger than the image then the returned image will be a rectangle,
+    limited by the extent of the image.
     
     Returns tuple of (cropped image as 2D numpy array, new location tuple)
 
     Arguments:  
         img  : input image as 2D numpy array
         loc  : location to crop, specified as bundle location tuple of 
                (centreX, centreY, radius)
     """
-    
-    cx,cy, rad = loc
-    imgCrop = img[cy-rad:cy+ rad, cx-rad:cx+rad]
-    
-    # Correct the co-ordinates of the bundle so that they
-    # are correct for new cropped image
-    newLoc = [rad,rad,loc[2]]
-   
-    return imgCrop, newLoc
-
+    if loc is not None:
+        
+        h,w = np.shape(img)[:2]
+        cx,cy, rad = loc
+        
+        minX = np.clip(cx-rad, 0, None)
+        maxX = np.clip(cx+rad, None, w)
+        
+         
+        minY = np.clip(cy-rad, 0, None)
+        maxY = np.clip(cy+rad, None, h)
+        
+        imgCrop = img[minY:maxY, minX: maxX]
+        
+        # Correct the co-ordinates of the bundle so that they
+        # are correct for new cropped image
+        newLoc = [rad,rad,loc[2]]
+       
+        return imgCrop, newLoc
+    else:
+        return img, None
 
 
 
 def get_mask(img, loc):
     """ Returns a circular mask, 1 inside bundle, 0 outside bundle, using specified
     bundle co-ordinates. Mask image has same dimensions as first two
     dimensions of input image (i.e. does not return a mask for each colour plane).
@@ -310,39 +323,53 @@
     
     Arguments:  
          img   : input image as 2D numpy array
          mask  : mask as 2D numy array with same dimensions as img, 
                  with areas to be kept as 1 and areas to be masked as 0.
     """
     
-    if img.ndim == 3:
-        m = np.expand_dims(mask, 2)
+    if mask is not None:
+        if img.ndim == 3:
+            m = np.expand_dims(mask, 2)
+        else:
+            m = mask
+        imgMasked = np.multiply(img, m)
+        
+        return imgMasked
     else:
-        m = mask
-    imgMasked = np.multiply(img, m)
+        return img
     
-    return imgMasked
-  
 
 def auto_mask(img, loc = None, **kwargs):
     """ Locates bundle and sets pixels outside to 0 .
     
     Arguments:  
         img  : input image as 2D numpy array
     
     Keyword Arguments:
         loc    : optional location of bundle as tuple of (centreX, centreY, radius), 
                  defaults to determining this using find_bundle
+        radius : optional, int, radius of mask to use rather than the automatically
+                 determined radius        
         Others : if loc is not specified, other optional keyword arguments will
                  be passed to find_bundle.
 
 
     """
+    radius = kwargs.get('radius', None)
+    
+    # If location not specified, find it
     if loc is None:
         loc = pybundle.find_bundle(img, **kwargs)
+    
+    # If radius was specified, replace auto determined radius
+    if radius is not None:
+        loc = (loc[0], loc[1], radius)
+        
+    # Mask image    
     mask = pybundle.get_mask(img, loc)
     imgMasked = pybundle.apply_mask(img, mask)
     
     return imgMasked
 
     
 def auto_mask_crop(img, loc = None, **kwargs):
```

### Comparing `PyFibreBundle-1.3.1/src/pybundle/core_interpolation.py` & `PyFibreBundle-1.3.2/src/pybundle/core_interpolation.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 """
 
 
 import numpy as np
 import math
 import time
 
+
+import matplotlib.pyplot as plt
+
 import cv2 as cv
 
 from scipy.spatial import Delaunay
 
 import pybundle
 from pybundle.bundle_calibration import BundleCalibration
 
@@ -49,23 +52,26 @@
      # Pre-filtering helps to minimse noise and reduce efffect of
      # multimodal patterns
      imgF = pybundle.g_filter(img, coreSpacing/5)
 
      # If a colour image, convert to greyscale by taking the maximum value across the channels
      imgF = pybundle.max_channels(imgF)
 
-     imgF = (imgF / np.max(imgF) * 255).astype('uint8')
+     imgF = (imgF / np.max(imgF) * 255).astype('uint8') 
 
      # Find regional maximum by taking difference between dilated and original
      # image. Because of the way dilation works, the local maxima are not changed
      # and so these will have a value of 0
-     kernel = cv.getStructuringElement(cv.MORPH_ELLIPSE, (coreSpacing,coreSpacing))
+     kernel = cv.getStructuringElement(cv.MORPH_ELLIPSE, (int(round(coreSpacing)),int(round(coreSpacing)) ))
+     kernel = cv.getStructuringElement(cv.MORPH_ELLIPSE, (3,3 ))
+
      imgD = cv.dilate(imgF, kernel)
+     
      imgMax = 255 - (imgF - imgD)  # we need to invert the image
-
+     
      # Just keep the maxima
      thres, imgBinary = cv.threshold(imgMax, 0,1,cv.THRESH_BINARY+cv.THRESH_OTSU)
 
      # Dilation step helps deal with mode patterns which have led to multiple
      # maxima within a core, the two maxima will end up merged into one connected
      # region
      elSize = math.ceil(coreSpacing / 3)
@@ -113,17 +119,18 @@
 
         numba  : optional, if true numba JIT used for faster execution, defaults to False.
     """
     numba = kwargs.get('numba', False)
     
     if filterSize is not None:
         img = pybundle.g_filter(img, filterSize)
-        
-    if numba and numbaAvailable:
-        cInt = core_value_extract_numba(img, coreX, coreY)
+
+    cInt = np.zeros(np.shape(coreX))
+    if numba and numbaAvailable:     
+        cInt = cInt + core_value_extract_numba(img, coreX, coreY)         
     else:
         cInt = img[coreY, coreX]
         
     return cInt
  
     
 def calib_tri_interp(img, coreSize, gridSize, **kwargs):
@@ -152,37 +159,39 @@
         background : optional, image used for background subtraction as 2D numpy array
         normalise  : optional, image used for normalisation, as 2D numpy array. Can be same as 
                      calibration image, defaults to no normalisation
         autoMask   : optional, boolean, if true the calibration image will be masked to prevent 
                      spurious core detections outside of bundle, defualts to True
         mask       : optional, boolean, when reconstructing output image will be masked outside of 
                      bundle, defaults to True
+        
     """
 
-    centreX = kwargs.get('centreX', -1)
-    centreY = kwargs.get('centreY', -1)
-    radius = kwargs.get('radius', -1)
+    centreX = kwargs.get('centreX', None)
+    centreY = kwargs.get('centreY', None)
+    radius = kwargs.get('radius', None)
     filterSize = kwargs.get('filterSize', 0)
     normalise = kwargs.get('normalise', None)
     autoMask = kwargs.get('autoMask', True)
     mask = kwargs.get('mask', True)
     background = kwargs.get('background', None)
+    
     if autoMask:
-        img = pybundle.auto_mask(img)
+        img = pybundle.auto_mask(img, radius = radius)
     # Find the cores in the calibration image
     coreX, coreY = pybundle.find_cores(img, coreSize)
     coreX = np.round(coreX).astype('uint16')
     coreY = np.round(coreY).astype('uint16')
 
     # Default values
-    if centreX < 0:
+    if centreX is None:
         centreX = np.mean(coreX)
-    if centreY < 0:
+    if centreY is None:
         centreY = np.mean(coreY)
-    if radius < 0:
+    if radius is None:
         dist = np.sqrt((coreX - centreX)**2 + (coreY - centreY)**2)
         radius = max(dist)
         
     # Delaunay triangulation and find barycentric co-ordinates for each pixel
     t1 = time.perf_counter()   
     
     calib = pybundle.init_tri_interp(img, coreX, coreY, centreX, centreY, radius, gridSize, filterSize= filterSize, background = background, normalise = normalise, mask = mask)
@@ -381,17 +390,18 @@
      Keyword Arguments:     
           numba: optional, if true use JIT acceleration using Numba, default is False
      """
     
      numba = kwargs.get('numba', True)
 
      # Extract intensity from each core
+     t1 = time.perf_counter()
      cVals = pybundle.core_values(
          img, calib.coreX, calib.coreY, calib.filterSize, **kwargs).astype('float64')
-
+     
      if calib.background is not None:
          cVals = cVals - calib.backgroundVals    
       
      if calib.normalise is not None:
          cVals = (cVals / calib.normaliseVals * 255)    
 
      # Triangular linear interpolation
```

### Comparing `PyFibreBundle-1.3.1/src/pybundle/core_interpolation_numba.py` & `PyFibreBundle-1.3.2/src/pybundle/core_interpolation_numba.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/src/pybundle/mosaic.py` & `PyFibreBundle-1.3.2/src/pybundle/mosaic.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/src/pybundle/pybundle.py` & `PyFibreBundle-1.3.2/src/pybundle/pybundle.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,38 +2,39 @@
 """
 PyFibreBundle is an open source Python package for image processing of
 fibre bundle images.
 
 This file contains the PyBundle class which provides object oriented
 usage of the key functionality.
 
-@author: Mike Hughes
-Applied Optics Group, University of Kent
-https://github.com/mikehugheskent
+@author: Mike Hughes, Applied Optics Group, University of Kent
+
 """
 
 
 import numpy as np
 import math
 import time
 
 import cv2 as cv
 import pybundle
 
 from pybundle.core_interpolation import *    
 from pybundle.bundle_calibration import BundleCalibration
-from pybundle.core import normalise_image
+from pybundle.core import normalise_image, g_filter, edge_filter, filter_image, crop_rect
 
 
 class PyBundle:
        
     coreMethod = None
 
     background = None
     normaliseImage = None
+    normaliseImageFiltered = None
+    normaliseImageFilterSize = None
     
     autoLoc = True
     loc = None
 
     autoMask = True
     mask = None    
     applyMask = False
@@ -80,14 +81,15 @@
     
     def __init__(self, **kwargs):
         """ Initialise a PyBundle object, for OOP functionality of the pybundle package."""
         
         self.background = kwargs.get('backgroundImage', self.background)
         self.normaliseImage = kwargs.get('normaliseImage',self.normaliseImage)
         
+        self.radius = kwargs.get('radius', None)
         self.loc = kwargs.get('loc', self.loc )
         if self.loc is not None:
             self.autoLoc = False
         self.autoLoc = kwargs.get('autoLoc', self.autoLoc )
         
         self.applyMask = kwargs.get('applyMask', self.applyMask)
 
@@ -118,14 +120,225 @@
         self.srNormToBackgrounds = kwargs.get('srNormToBackgrounds', self.srNormToBackgrounds)
         self.srNormToImages = kwargs.get('srNormToImages', self.srNormToImages)
         self.srMultiBackgrounds = kwargs.get('srMultiBackgrounds' , self.srMultiBackgrounds)
         self.srMultiNormalisation = kwargs.get('srMultiNormalisation' ,self.srMultiNormalisation )
         self.srDarkFrame = kwargs.get('srDarkFrame', self.srDarkFrame)
         self.srUseLut = kwargs.get('srUseLut', self.srUseLut)
         
+
+            
+
+    def __process_filter(self, img, cropLoc, mask):
+         """ Process fibre bundle image using FILTER method using current settings.
+         Designed to be called from process.
+         
+         Returns processed image as 2D/3D numpy array.
+         
+         Arguments:
+             img: input image as 2D/3D numpy array
+             cropLoc : location to crop to, tuple of (centre_x, centre_y, radius)
+                       (None for no crop)
+             mask : mask to apply (None for no mask)
+             
+         """
+         
+         imgOut = img        
+                         
+         if self.background is not None: imgOut = imgOut - self.background
+                 
+         if self.filterSize is not None: imgOut = pybundle.g_filter(imgOut, self.filterSize)            
+                   
+         if self.normaliseImage is not None:
+             # Check we have a filtered normaliseImage, otherwise
+             # we need to do that now
+             if self.normaliseImageFilterSize != self.filterSize:
+                 self.normaliseImageFiltered = g_filter(self.normaliseImage, self.filterSize)
+                 self.normaliseImageFilterSize = self.filterSize
+             if self.filterSize is None:
+                 self.normaliseImageFiltered = self.normaliseImage
+             # Do the normalisation
+             imgOut = normalise_image(imgOut, self.normaliseImageFiltered)         
+       
+         
+         # Masking
+         imgOut = pybundle.apply_mask(imgOut, mask)        
+         
+         # Cropping
+         if self.crop: imgOut = pybundle.crop_rect(imgOut, cropLoc)[0]
+
+         return imgOut
+         
+     
+        
+    def __process_edge_filter(self, img, cropLoc, mask):
+        """ Process fibre bundle image using EDGE FILTER method using current settings.
+        Designed to be called from process.
+        
+        Returns processed image as 2D/3D numpy array.
+        
+        Arguments:
+            img: input image as 2D/3D numpy array
+            cropLoc : location to crop to, tuple of (centre_x, centre_y, radius)
+                      (None for no crop)
+            mask : mask to apply (None for no mask)
+            
+        """
+        
+        imgOut = img
+        
+        if self.background is not None: imgOut = imgOut - self.background
+        
+         
+        # Masking
+        if mask is not None: imgOut = pybundle.apply_mask(imgOut, mask)
+       
+        
+        # Cropping
+        if cropLoc is not None: imgOut = pybundle.crop_rect(imgOut, cropLoc)[0]
+
+                
+        # If there isn't an edge filter created, create it now          
+        if self.edgeFilter is None:
+            assert cropLoc is not None, "Edge filter requires the bundle location."
+            assert self.edgeFilterShape is not None, "Edge filter requires the edge filter shape to be set using set_edge_filter_shape()."
+            self.edgeFilter = pybundle.edge_filter(cropLoc[2] * 2 , self.edgeFilterShape[0], self.edgeFilterShape[1])
+           
+        
+        # Normalisation.
+        # (If there is a normalisation image but not a filtered version of it
+        # create a filtered version now)
+        if self.normaliseImage is not None:
+            
+            # Create the filtered normalisation image if we don't have it
+            if self.normaliseImageFilterSize != self.edgeFilterShape or self.normaliseImageFiltered is None:
+                self.normaliseImageFiltered = filter_image(crop_rect(self.normaliseImage, cropLoc)[0], self.edgeFilter)
+                self.normaliseImageFilterSize = self.edgeFilterShape
+            
+            # Do the normalisation
+            imgOut = normalise_image(imgOut, self.normaliseImageFiltered)    
+       
+        
+        # Apply edge filter
+        if self.edgeFilter is not None and cropLoc is not None:
+               imgOut = pybundle.filter_image(imgOut, self.edgeFilter) 
+        
+        return imgOut
+    
+    
+    
+
+    def __process_trilin(self, img):
+        
+        """ Process fibre bundle image using TRILIN method using current settings.
+        Designed to be called from process.
+        
+        Returns processed image as 2D/3D numpy array.
+        
+        Arguments:
+            img: input image as 2D/3D numpy array            
+        """
+        
+        imgOut = img
+        
+        # Normal Triangular linear interpolation    
+        if not self.superRes:
+            if self.calibration is None and self.calibImage is not None:
+                self.calibrate()
+            if self.calibration is None: return None
+            if imgOut.ndim != 2 and imgOut.ndim != 3: return None            
+            imgOut = pybundle.recon_tri_interp(imgOut, self.calibration, numba = self.useNumba)
+            
+        # Super Res Triangular linear interpolation
+        else:        
+            
+            # Check that we have a stack of images
+            if imgOut.ndim != 3: return None           
+            
+            # If we have a calibration LUT and have opted to use this and we have a value for the parameter, pull out the
+            # correct calibration and use this for recon
+          
+            if self.srUseLut and self.srCalibrationLUT is not None and self.srParamValue is not None:
+                calibSR = self.srCalibrationLUT.calibrationSR(self.srParamValue)
+            elif self.calibrationSR is not None:
+                calibSR = self.calibrationSR
+            elif ( (self.srCalibImages is not None) or (self.srShifts is not None)):
+                self.calibrate_sr() 
+                # If we still don't have a calibration we cannot proceed    
+                if self.calibrationSR is None: return None
+                calibSR = self.calibrationSR
+            else:
+                return None
+            
+            # If we don't have the correct number of images in the stack, we cannot proceeed            
+            if np.shape(imgOut)[2] != calibSR.nShifts: return None
+            imgOut = pybundle.SuperRes.recon_multi_tri_interp(imgOut, calibSR, numba = self.useNumba)
+       
+        return imgOut
+    
+    
+    def process(self, img):
+        """ Process fibre bundle image using current settings.
+        
+        Returns processed image as 2D/3D numpy array.
+        
+        Arguments:
+            img: input image as 2D/3D numpy array
+            
+        """        
+       
+        # If autoLoc is still True, meaning calibrate() was not called,
+        # and we need to crop, mask apply an edge filter, 
+        # then we find the location for the crop now, otherwise
+        # we use the stored location (if this is None then there will be no crop)
+        if self.autoLoc and ((self.crop or self.coreMethod == self.EDGE_FILTER) or self.applyMask):
+            if self.calibImage is not None:
+
+                self.loc = pybundle.find_bundle(self.calibImage) 
+                cropLoc = self.loc
+                self.autoLoc = False   # We have done this, don't do it again
+            else:
+                cropLoc = pybundle.find_bundle(img) 
+        else:
+            cropLoc = self.loc
+         
+         
+        # If autoMask is still True, meaning calibrate() was not called, and we 
+        # are applying a mask, we create a mask now, otherwise we
+        # we use the stored mask (and if this is None then there will be no mask)    
+        if self.autoMask and cropLoc is not None and self.applyMask is not None:
+            if self.calibImage is not None:
+                self.mask = pybundle.get_mask(self.calibImage, cropLoc)
+                mask = self.mask
+                self.autoMask = False  # We have done this, don't do it again
+            else:
+                mask = pybundle.get_mask(img, cropLoc)
+        else:
+            mask = self.mask
+            
+        # Call the specific method for core removal    
+        if self.coreMethod == self.FILTER: imgOut = self.__process_filter(img, cropLoc, mask)     
+        if self.coreMethod == self.EDGE_FILTER: imgOut = self.__process_edge_filter(img, cropLoc, mask)     
+        if self.coreMethod == self.TRILIN: imgOut = self.__process_trilin(img)
+        
+        # Autocontrast
+        if self.autoContrast:
+            imgOut = imgOut - np.min(imgOut)
+            imgOut = imgOut / np.max(imgOut)
+            if self.outputType == 'uint8':
+                imgOut = imgOut * 255
+            elif self.outputType == 'uint16':
+                imgOut = imgOut * (2**16 - 1)
+            elif self.outputType == 'float':
+                imgOut = imgOut                
+                
+        # Type casting
+        if imgOut.dtype != self.outputType:
+            imgOut = imgOut.astype(self.outputType)        
+        
+        return imgOut
                
 
     def set_filter_size(self, filterSize):
         """ Set the size of Gaussian filter used if filtering method employed.
         
         Arguments:
             filterSize : float, sigma of Gaussian filter
@@ -213,14 +426,18 @@
         It is also possible to provide an image as a 2D numpy array, in which
         case the mask will be generated of the correct size for this image, but
         this is deprecated, use calibrate() instead. Optionally provide a 
         radius rather than using radius of determined bundle location.
         
         Arguments:
             img: boolean, True to automically create mask
+            
+        Keyword Arguments:
+            radius : optional, int, overrides automically determined radius for
+                     mask.
        
         """       
         if type(img) is bool:
             if img is True:
                 self.mask = None
                 self.autoMask = True     
             
@@ -293,15 +510,15 @@
         if self.calibration is not None:
             self.calibration = pybundle.tri_interp_background(self.calibration, self.background)
             
         
     def set_normalise_image(self, normaliseImage):
         """ Store an image to be used for normalisation. If TRILIN is being used and a 
         calibration has already been performed, the normalisation will be added to the
-        calibration.
+        calibration. 
         
         Arguments:
 
             normaliseImage : normalisation image as 2D/3D numpy array. Set as 
                              None to remove normalisation.
         """
         if normaliseImage is not None:
@@ -332,14 +549,23 @@
         
         Arguments:
             calibImg : calibration image as 2D/3D numpy array
         """
         self.calibImage = calibImg.astype('float')
         
         
+    def set_radius(self, radius):
+        """ Sets the radius of the bundle in the image. This will override
+        any automically determined value.
+        
+        Arguments:
+            radius : int, bundle radius
+        """
+        self.radius = radius
+        
         
     def set_grid_size(self, gridSize):
         """ Sets output image size if TRLIN method used. If not called prior 
         to calling 'calibrate', the default value of 512 will be used.
         
         Arguments:
             gridSize : int, size of square image output 
@@ -480,14 +706,16 @@
         
     def calibrate(self):
         """ Peforms calibraion steps appropriate to chosen method. A calibration 
         image must have been set prior to calling this.
         
         For TRILIN, creates interpolation calibration.
         
+        For FILTER, EDGE_FILTER, a filtered normalisation image is created.
+        
         For FILTER, EDGE_FILTER the bundle will be located if autoLoc has been set.
         
         For FILTER, EDGE_FILTER the mask will be located if autoMask has been set.
         
         """
         assert self.calibImage is not None, "Calibration requires calibration image, use set_calib_image()."
         
@@ -495,30 +723,47 @@
             if self.calibImage is not None:
 
                 self.calibration = pybundle.calib_tri_interp(self.calibImage, self.coreSize, self.gridSize, 
                                                          background = self.background, 
                                                          normalise = self.normaliseImage,
                                                          filterSize = self.filterSize,
                                                          mask = True,
-                                                         autoMask = True)
+                                                         autoMask = True,
+                                                         radius = self.radius)
         else:
             
             if self.autoLoc and self.calibImage is not None:
                 self.loc = pybundle.find_bundle(self.calibImage)
+                # If user has specified a radius, over-ride the auto determined
+                # one from find_bundle
+                if self.radius is not None:
+                    self.loc = (self.loc[0], self.loc[1], self.radius)
                 self.autoLoc = False    
             
             if self.autoMask and self.calibImage is not None and self.loc is not None:
                 self.mask = pybundle.get_mask(self.calibImage, self.loc)
                 self.autoMask = False
+                
+        # If we are Gaussian filtering and we have a normalisation image
+        # create a filtered version of it for use later.
+        if self.coreMethod == self.FILTER:
+             if self.filterSize is not None and self.normaliseImage is not None:  
+                 self.normaliseImageFiltered = g_filter(self.normaliseImage, self.filterSize)
+                 self.normaliseImageFilterSize = self.filterSize     # So we can realise if the filtersize changes we
+                                                                     # need to redo this
          
         if self.coreMethod == self.EDGE_FILTER:
              assert self.loc is not None, "Calibration for edge filter requires the bundle location."
              assert type(self.edgeFilterShape) is tuple, "Edge filter shape not defined."
              self.edgeFilter = pybundle.edge_filter(self.loc[2] *2 , self.edgeFilterShape[0], self.edgeFilterShape[1])
-            
+             # If we have a normalisation image, create a filtered version of it for use later.
+             if self.normaliseImage is not None and self.loc is not None:
+                 self.nomaliseImageFiltered = filter_image(crop_rect(self.normaliseImage, self.loc)[0], self.edgeFilter)
+                 self.normaliseImageFilterSize = self.edgeFilterShape
+                 
     
     def calibrate_sr(self):
         """ Creates calibration for TRILIN SR method. A calibration image, 
         set of super-res shift images, coreSize and gridSize must have been 
         set prior to calling this.
         """
         
@@ -533,155 +778,14 @@
                 normToBackground = self.srNormToBackgrounds,
                 normToImage = self.srNormToImages,
                 shifts = self.srShifts,
                 multiBackgrounds = self.srMultiBackgrounds,
                 multiNormalisation = self.srMultiNormalisation,
                 darkFrame = self.srDarkFrame,
                 filterSize = self.filterSize)
-
-    
-    def process(self, img):
-        """ Process fibre bundle image using current settings.
-        
-        Returns processed image as 2D/3D numpy array.
-        
-        Arguments:
-            img: input image as 2D/3D numpy array
-            
-        """
-        
-        method = self.coreMethod  # to insulate against a change during processing
-        
-        imgOut = img        
-        
-        
-        
-        # If autoLoc is True (or if we are doing EDGE_FILTER), we find the location for the crop now, otherwise
-        # we use the stored location (if this is None then there will be no crop)
-        # We avoid doing this if we are not cropping or masking to save time
-        if self.autoLoc and ((self.crop or self.coreMethod == self.EDGE_FILTER) or self.applyMask):
-            if self.calibImage is not None:
-
-                self.loc = pybundle.find_bundle(self.calibImage) 
-                cropLoc = self.loc
-                self.autoLoc = False   # We have done this, don't do it again
-            else:
-                cropLoc = pybundle.find_bundle(img) 
-        else:
-            cropLoc = self.loc
-         
-         
-        # If autoMask is True, we find the location for mask crop now, otherwise
-        # we use the stored mask (if this is None then there will be no mask)
-        # We avoid doing this if we are not masking to save time         
-        if self.autoMask and cropLoc is not None and self.applyMask is not None:
-            if self.calibImage is not None:
-                self.mask = pybundle.get_mask(self.calibImage, cropLoc)
-                mask = self.mask
-                self.autoMask = False  # We have done this, don't do it again
-            else:
-                mask = pybundle.get_mask(img, cropLoc)
-
-        else:
-            mask = self.mask
-            
-            
-        # Background subtraction (This is handled separately for TRILIN)     
-        if method == self.FILTER or method == self.EDGE_FILTER:
-            if self.background is not None:
-                imgOut = imgOut - self.background
-                
-        
-        # Normalisation (This is handled separately for TRILIN)     
-        if method == self.FILTER or method == self.EDGE_FILTER:
-            if self.normaliseImage is not None:
-                imgOut = normalise_image(imgOut, self.normaliseImage)              
-
-        
-        # Gaussian Filter
-        if method == self.FILTER and self.filterSize is not None:
-            imgOut = pybundle.g_filter(imgOut, self.filterSize)            
-                  
-                
-        # Masking
-        if (method == self.FILTER or method == self.EDGE_FILTER) and mask is not None:
-            imgOut = pybundle.apply_mask(imgOut, mask)
-       
-        
-        # Cropping
-        if method == self.EDGE_FILTER or (method == self.FILTER and self.crop):
-            if cropLoc is not None:
-                imgOut = pybundle.crop_rect(imgOut, cropLoc)[0]
-
-       
-        # Edge Filter
-        if method == self.EDGE_FILTER:
-
-           if self.edgeFilter is None:
-               assert cropLoc is not None, "Edge filter requires the bundle location."
-               assert self.edgeFilterShape is not None, "Edge filter requires the edge filter shape to be set using set_edge_filter_shape()."
-               self.edgeFilter = pybundle.edge_filter(cropLoc[2] *2 , self.edgeFilterShape[0], self.edgeFilterShape[1])
-                
-           if self.edgeFilter is not None and cropLoc is not None:
-               imgOut = pybundle.filter_image(imgOut, self.edgeFilter) 
-        
-        # Normal Triangular linear interpolation    
-        if method == self.TRILIN and not self.superRes:
-            if self.calibration is None and self.calibImage is not None:
-                self.calibrate()
-            if self.calibration is None: return None
-            if imgOut.ndim != 2 and imgOut.ndim != 3: return None            
-            imgOut = pybundle.recon_tri_interp(imgOut, self.calibration, numba = self.useNumba)
-            
-         
-        # Super-resolution triangular linear interpolation    
-        if method == self.TRILIN and self.superRes:
-            
-            # Check that we have a stack of images
-            if imgOut.ndim != 3: return None           
-            
-            # If we have a calibration LUT and have opted to use this and we have a value for the parameter, pull out the
-            # correct calibration and use this for recon
-          
-            if self.srUseLut and self.srCalibrationLUT is not None and self.srParamValue is not None:
-                calibSR = self.srCalibrationLUT.calibrationSR(self.srParamValue)
-            elif self.calibrationSR is not None:
-                calibSR = self.calibrationSR
-            elif ( (self.srCalibImages is not None) or (self.srShifts is not None)):
-                self.calibrate_sr() 
-                # If we still don't have a calibration we cannot proceed    
-                if self.calibrationSR is None: return None
-                calibSR = self.calibrationSR
-            else:
-                return None
-            
-            # If we don't have the correct number of images in the stack, we cannot proceeed            
-            if np.shape(imgOut)[2] != calibSR.nShifts: return None
-            imgOut = pybundle.SuperRes.recon_multi_tri_interp(imgOut, calibSR, numba = self.useNumba)
-       
-           
-        
-        # Autocontrast
-        if self.autoContrast:
-            t1 = time.perf_counter()
-            imgOut = imgOut - np.min(imgOut)
-            imgOut = imgOut / np.max(imgOut)
-            if self.outputType == 'uint8':
-                imgOut = imgOut * 255
-            elif self.outputType == 'uint16':
-                imgOut = imgOut * (2**16 - 1)
-            elif self.outputType == 'float':
-                imgOut = imgOut
-                
-                
-        # Type casting
-        if imgOut.dtype != self.outputType:
-            imgOut = imgOut.astype(self.outputType)        
-        
-        return imgOut
     
 
     def get_pixel_scale(self):
         """ Returns the scaling factor between the pixel size in the raw image
         and the pixel size in the processed image. If the TRILIN method is
         selected, but a calibration has not yet been performed, returns None.
         """
```

### Comparing `PyFibreBundle-1.3.1/src/pybundle/super_res.py` & `PyFibreBundle-1.3.2/src/pybundle/super_res.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/src/pybundle/utility.py` & `PyFibreBundle-1.3.2/src/pybundle/utility.py`

 * *Files 5% similar despite different names*

```diff
@@ -205,8 +205,20 @@
     Arguments:
         img: image as 2D/3D numpy array
     """     
 
     if img.ndim == 3:
         return np.max(img, 2)
     else:
-        return img
+        return img
+    
+def resample(img, factor):
+    
+    h,w = np.shape(img)
+    img = cv.resize(img, ( int(w * factor), int(h * factor)))
+    
+    return img
+    
+    
+    
+    
+
```

### Comparing `PyFibreBundle-1.3.1/test/test_all.py` & `PyFibreBundle-1.3.2/test/test_all.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/test/test_find_cores.py` & `PyFibreBundle-1.3.2/test/test_find_cores.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/test/test_loc.py` & `PyFibreBundle-1.3.2/test/test_loc.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/test/test_mask.py` & `PyFibreBundle-1.3.2/test/test_mask.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/test/test_masking.py` & `PyFibreBundle-1.3.2/test/test_masking.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/test/test_masking_col.py` & `PyFibreBundle-1.3.2/test/test_masking_col.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/test/test_mosaic.py` & `PyFibreBundle-1.3.2/test/test_mosaic.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/test/test_mosaic_col.py` & `PyFibreBundle-1.3.2/test/test_mosaic_col.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/test/test_processing_im_type.py` & `PyFibreBundle-1.3.2/test/test_processing_im_type.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/test/test_pybundle_oop.py` & `PyFibreBundle-1.3.2/test/test_pybundle_oop.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/test/test_recon_tri_interp.py` & `PyFibreBundle-1.3.2/test/test_recon_tri_interp.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/test/test_recon_tri_interp_col.py` & `PyFibreBundle-1.3.2/test/test_recon_tri_interp_col.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/test/test_simple_processing.py` & `PyFibreBundle-1.3.2/test/test_simple_processing.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/test/test_simple_processing_col.py` & `PyFibreBundle-1.3.2/test/test_simple_processing_col.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/test/test_sr_sort_stack.py` & `PyFibreBundle-1.3.2/test/test_sr_sort_stack.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/test/test_super_res.py` & `PyFibreBundle-1.3.2/test/test_super_res.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3.1/test/test_super_res_oop.py` & `PyFibreBundle-1.3.2/test/test_super_res_oop.py`

 * *Files identical despite different names*

