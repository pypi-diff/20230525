# Comparing `tmp/brighteyes-ism-1.1.1.tar.gz` & `tmp/brighteyes-ism-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brighteyes-ism-1.1.1.tar", last modified: Thu May 18 17:06:15 2023, max compression
+gzip compressed data, was "brighteyes-ism-1.1.2.tar", last modified: Thu May 25 16:23:15 2023, max compression
```

## Comparing `brighteyes-ism-1.1.1.tar` & `brighteyes-ism-1.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 17:06:15.089085 brighteyes-ism-1.1.1/
--rw-rw-rw-   0        0        0    35823 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     3949 2023-05-18 17:06:15.089085 brighteyes-ism-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3086 2023-05-09 13:03:56.000000 brighteyes-ism-1.1.1/README.md
--rw-rw-rw-   0        0        0     1006 2023-05-09 13:03:07.000000 brighteyes-ism-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0     1658 2023-05-18 17:06:15.096095 brighteyes-ism-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0       72 2023-02-06 17:07:56.000000 brighteyes-ism-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 17:06:14.964418 brighteyes-ism-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-18 17:06:14.984364 brighteyes-ism-1.1.1/src/brighteyes_ism/
--rw-rw-rw-   0        0        0      123 2023-02-06 17:07:56.000000 brighteyes-ism-1.1.1/src/brighteyes_ism/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 17:06:15.058168 brighteyes-ism-1.1.1/src/brighteyes_ism/analysis/
--rw-rw-rw-   0        0        0     7276 2023-04-21 10:40:17.000000 brighteyes-ism-1.1.1/src/brighteyes_ism/analysis/APR_lib.py
--rw-rw-rw-   0        0        0    15991 2023-04-07 08:56:11.000000 brighteyes-ism-1.1.1/src/brighteyes_ism/analysis/Deconv_lib.py
--rw-rw-rw-   0        0        0     9410 2023-04-07 12:04:30.000000 brighteyes-ism-1.1.1/src/brighteyes_ism/analysis/FRC_lib.py
--rw-rw-rw-   0        0        0    11458 2023-05-18 16:44:26.000000 brighteyes-ism-1.1.1/src/brighteyes_ism/analysis/FocusISM_lib.py
--rw-rw-rw-   0        0        0    13646 2023-05-18 16:47:40.000000 brighteyes-ism-1.1.1/src/brighteyes_ism/analysis/Tools_lib.py
--rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.1/src/brighteyes_ism/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 17:06:15.067171 brighteyes-ism-1.1.1/src/brighteyes_ism/dataio/
--rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.1/src/brighteyes_ism/dataio/__init__.py
--rw-rw-rw-   0        0        0     5852 2023-04-06 15:11:23.000000 brighteyes-ism-1.1.1/src/brighteyes_ism/dataio/mcs.py
-drwxrwxrwx   0        0        0        0 2023-05-18 17:06:15.088088 brighteyes-ism-1.1.1/src/brighteyes_ism/simulation/
--rw-rw-rw-   0        0        0    18414 2023-04-21 10:52:49.000000 brighteyes-ism-1.1.1/src/brighteyes_ism/simulation/PSF_sim.py
--rw-rw-rw-   0        0        0     5701 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.1/src/brighteyes_ism/simulation/Tubulin_sim.py
--rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.1/src/brighteyes_ism/simulation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 17:06:15.010324 brighteyes-ism-1.1.1/src/brighteyes_ism.egg-info/
--rw-rw-rw-   0        0        0     3949 2023-05-18 17:06:14.000000 brighteyes-ism-1.1.1/src/brighteyes_ism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-05-18 17:06:14.000000 brighteyes-ism-1.1.1/src/brighteyes_ism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 17:06:14.000000 brighteyes-ism-1.1.1/src/brighteyes_ism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-05-18 17:06:14.000000 brighteyes-ism-1.1.1/src/brighteyes_ism.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-18 17:06:14.000000 brighteyes-ism-1.1.1/src/brighteyes_ism.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 16:23:15.888029 brighteyes-ism-1.1.2/
+-rw-rw-rw-   0        0        0    35823 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4246 2023-05-25 16:23:15.888029 brighteyes-ism-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3383 2023-05-23 10:37:26.000000 brighteyes-ism-1.1.2/README.md
+-rw-rw-rw-   0        0        0     1006 2023-05-25 15:29:32.000000 brighteyes-ism-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1658 2023-05-25 16:23:15.896037 brighteyes-ism-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0       72 2023-02-06 17:07:56.000000 brighteyes-ism-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:23:15.762390 brighteyes-ism-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 16:23:15.781341 brighteyes-ism-1.1.2/src/brighteyes_ism/
+-rw-rw-rw-   0        0        0      123 2023-02-06 17:07:56.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:23:15.857111 brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/
+-rw-rw-rw-   0        0        0     7276 2023-04-21 10:40:17.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/APR_lib.py
+-rw-rw-rw-   0        0        0    15991 2023-04-07 08:56:11.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/Deconv_lib.py
+-rw-rw-rw-   0        0        0     9410 2023-04-07 12:04:30.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/FRC_lib.py
+-rw-rw-rw-   0        0        0    11458 2023-05-18 16:44:26.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/FocusISM_lib.py
+-rw-rw-rw-   0        0        0    16427 2023-05-23 17:49:33.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/Tools_lib.py
+-rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:23:15.865122 brighteyes-ism-1.1.2/src/brighteyes_ism/dataio/
+-rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/dataio/__init__.py
+-rw-rw-rw-   0        0        0     5852 2023-04-06 15:11:23.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/dataio/mcs.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:23:15.887061 brighteyes-ism-1.1.2/src/brighteyes_ism/simulation/
+-rw-rw-rw-   0        0        0    19397 2023-05-25 15:44:43.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/simulation/PSF_sim.py
+-rw-rw-rw-   0        0        0     5701 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/simulation/Tubulin_sim.py
+-rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/simulation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:23:15.806274 brighteyes-ism-1.1.2/src/brighteyes_ism.egg-info/
+-rw-rw-rw-   0        0        0     4246 2023-05-25 16:23:15.000000 brighteyes-ism-1.1.2/src/brighteyes_ism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      735 2023-05-25 16:23:15.000000 brighteyes-ism-1.1.2/src/brighteyes_ism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 16:23:15.000000 brighteyes-ism-1.1.2/src/brighteyes_ism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-05-25 16:23:15.000000 brighteyes-ism-1.1.2/src/brighteyes_ism.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-25 16:23:15.000000 brighteyes-ism-1.1.2/src/brighteyes_ism.egg-info/top_level.txt
```

### Comparing `brighteyes-ism-1.1.1/LICENSE` & `brighteyes-ism-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.1.1/PKG-INFO` & `brighteyes-ism-1.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brighteyes-ism
-Version: 1.1.1
+Version: 1.1.2
 Summary: A toolbox for analysing and simulating ISM images
 Home-page: https://github.com/VicidominiLab/brighteyes-ism
 Author: Alessandro Zunino
 Author-email: Alessandro Zunino <alessandro.zunino@iit.it>
 Project-URL: Homepage, https://github.com/VicidominiLab/brighteyes-ism
 Project-URL: Documentation, https://brighteyes-ism.readthedocs.io
 Classifier: Programming Language :: Python :: 3.7
@@ -38,15 +38,15 @@
 * Fourier Ring Correlation (https://doi.org/10.1038/s41467-019-11024-z)
 
 The simulation module contains libraries for:
 
 * Generation of ISM point spread functions (https://doi.org/10.1016/j.cpc.2022.108315)
 * Generation of tubulin phantom samples
 
-The dataio module contains libraries for
+The dataio module contains libraries for:
 
 * Reading the data and metadata from the MCS software (https://github.com/VicidominiLab/BrightEyes-MCS)
 
 ----------------------------------
 
 ## Installation
 
@@ -78,14 +78,21 @@
 
 https://github.com/VicidominiLab/BrightEyes-ISM/tree/main/examples
 
 You can read the manual of this package on Read the Docs:
 
 https://brighteyes-ism.readthedocs.io
 
+## Citation
+
+If you find BrightEyes-ISM useful for your research, please cite it as:
+
+_Zunino, A., Slenders, E., Fersini, F. et al. Open-source tools enable accessible and advanced image scanning microscopy data analysis. Nat. Photon. (2023). https://doi.org/10.1038/s41566-023-01216-x_
+
+
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

### Comparing `brighteyes-ism-1.1.1/README.md` & `brighteyes-ism-1.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 * Fourier Ring Correlation (https://doi.org/10.1038/s41467-019-11024-z)
 
 The simulation module contains libraries for:
 
 * Generation of ISM point spread functions (https://doi.org/10.1016/j.cpc.2022.108315)
 * Generation of tubulin phantom samples
 
-The dataio module contains libraries for
+The dataio module contains libraries for:
 
 * Reading the data and metadata from the MCS software (https://github.com/VicidominiLab/BrightEyes-MCS)
 
 ----------------------------------
 
 ## Installation
 
@@ -58,14 +58,21 @@
 
 https://github.com/VicidominiLab/BrightEyes-ISM/tree/main/examples
 
 You can read the manual of this package on Read the Docs:
 
 https://brighteyes-ism.readthedocs.io
 
+## Citation
+
+If you find BrightEyes-ISM useful for your research, please cite it as:
+
+_Zunino, A., Slenders, E., Fersini, F. et al. Open-source tools enable accessible and advanced image scanning microscopy data analysis. Nat. Photon. (2023). https://doi.org/10.1038/s41566-023-01216-x_
+
+
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

### Comparing `brighteyes-ism-1.1.1/pyproject.toml` & `brighteyes-ism-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "scikit-image>=0.19.2", "scikit-learn", "numpy", "scipy", "matplotlib", "joblib", "poppy", 	"PyCustomFocus", "h5py", "statsmodels", "tqdm", "matplotlib-scalebar"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "brighteyes-ism"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Alessandro Zunino", email="alessandro.zunino@iit.it" },
 ]
 description = "A toolbox for analysing and simulating ISM images"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
```

### Comparing `brighteyes-ism-1.1.1/setup.cfg` & `brighteyes-ism-1.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 7269 6768 7465 7965 732d 6973   = brighteyes-is
 00000020: 6d0d 0a76 6572 7369 6f6e 203d 2031 2e31  m..version = 1.1
-00000030: 2e31 0d0a 6175 7468 6f72 203d 2041 6c65  .1..author = Ale
+00000030: 2e32 0d0a 6175 7468 6f72 203d 2041 6c65  .2..author = Ale
 00000040: 7373 616e 6472 6f20 5a75 6e69 6e6f 0d0a  ssandro Zunino..
 00000050: 6175 7468 6f72 5f65 6d61 696c 203d 2061  author_email = a
 00000060: 6c65 7373 616e 6472 6f2e 7a75 6e69 6e6f  lessandro.zunino
 00000070: 4069 6974 2e69 740d 0a75 726c 203d 2068  @iit.it..url = h
 00000080: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 00000090: 6d2f 5669 6369 646f 6d69 6e69 4c61 622f  m/VicidominiLab/
 000000a0: 6272 6967 6874 6579 6573 2d69 736d 0d0a  brighteyes-ism..
```

### Comparing `brighteyes-ism-1.1.1/src/brighteyes_ism/analysis/APR_lib.py` & `brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/APR_lib.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.1.1/src/brighteyes_ism/analysis/Deconv_lib.py` & `brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/Deconv_lib.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.1.1/src/brighteyes_ism/analysis/FRC_lib.py` & `brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/FRC_lib.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.1.1/src/brighteyes_ism/analysis/FocusISM_lib.py` & `brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/FocusISM_lib.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.1.1/src/brighteyes_ism/analysis/Tools_lib.py` & `brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/Tools_lib.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 
 from .FRC_lib import radial_profile
 
-#%%
+
+# %%
 
 def Reorder(data, inOrder: str, outOrder: str = 'rzxytc'):
     '''
     It reorders a dataset to match the desired order of dimensions.
     If some dimensions are missing, it adds new dimensions.
 
     Parameters
@@ -21,38 +22,39 @@
 
     Returns
     -------
     data : ndarray
         ISM dataset reordered.
 
     '''
-    
-    if not(inOrder == outOrder):
+
+    if not (inOrder == outOrder):
         # adds missing dimensions
         Nout = len(outOrder)
         dataShape = np.shape(data)
         Ndim = len(dataShape)
-        for i in range(Nout-Ndim):
-            data = np.expand_dims(data, Ndim+i)
-        
+        for i in range(Nout - Ndim):
+            data = np.expand_dims(data, Ndim + i)
+
         # check order of dimensions
         order = []
         newdim = 0
         for i in range(Nout):
             dim = outOrder[i]
             if dim in inOrder:
                 order.append(inOrder.find(dim))
             else:
-                order.append(Ndim+newdim)
+                order.append(Ndim + newdim)
                 newdim += 1
         data = np.transpose(data, order)
-    
+
     return data
 
-def CropEdge(dset, npx = 10, edges = 'l', order: str = 'rzxytc'):
+
+def CropEdge(dset, npx=10, edges='l', order: str = 'rzxytc'):
     '''
     It crops an ISM dataset along the specified edges of the xy plane.
     
     Parameters
     ----------
     dset : ndarray
         ISM dataset
@@ -66,31 +68,32 @@
 
     Returns
     -------
     dset_cropped : ndarray
         ISM dataset cropped
 
     '''
-    
+
     dset_cropped = Reorder(dset, order)
-    
+
     if 'l' in edges:
         dset_cropped = dset_cropped[..., npx:, :, :, :]
-        
+
     if 'r' in edges:
         dset_cropped = dset_cropped[..., :-npx, :, :, :]
-        
+
     if 'u' in edges:
         dset_cropped = dset_cropped[..., :, npx:, :, :]
-        
+
     if 'd' in edges:
         dset_cropped = dset_cropped[..., :, :-npx, :, :]
-        
+
     return np.squeeze(dset_cropped)
 
+
 def DownSample(dset, ds: int = 2, order: str = 'rzxytc'):
     '''
     It downsamples an ISM dataset on the xy plane.
     
     Parameters
     ----------
     dset : ndarray
@@ -102,21 +105,22 @@
         
     Returns
     -------
     dset_ds : ndarray
         ISM dataset downsampled.
 
     '''
-    
+
     dset = Reorder(dset, order)
-    
+
     dset_ds = dset[..., ::ds, ::ds, :, :]
-    
+
     return np.squeeze(dset_ds)
 
+
 def UpSample(dset, us: int = 2, npx: str = 'even', order: str = 'rzxytc'):
     '''
     It upsamples an ISM dataset on the xy plane.
 
     Parameters
     ----------
     dset : TYPE
@@ -130,33 +134,34 @@
 
     Returns
     -------
     dset_us : ndarray
         ISM dataset upsampled.
 
     '''
-    
+
     dset = Reorder(dset, order)
-    
+
     sz = dset.shape
-    
+
     if npx == 'even':
         sz_us = np.asarray(sz)
-        sz_us[2] = sz_us[2]*us
-        sz_us[3] = sz_us[3]*us
+        sz_us[2] = sz_us[2] * us
+        sz_us[3] = sz_us[3] * us
     elif npx == 'odd':
         sz_us = np.asarray(sz)
-        sz_us[2] = sz_us[2]*us - 1
-        sz_us[3] = sz_us[3]*us - 1
-        
-    dset_us = np.zeros( sz_us )
+        sz_us[2] = sz_us[2] * us - 1
+        sz_us[3] = sz_us[3] * us - 1
+
+    dset_us = np.zeros(sz_us)
     dset_us[..., ::us, ::us, :, :] = dset
-    
+
     return np.squeeze(dset_us)
 
+
 def ArgMaxND(data):
     '''
     It finds the the maximum and the corresponding indeces of a N-dimensional array.
 
     Parameters
     ----------
     data : ndarray
@@ -166,23 +171,24 @@
     -------
     arg : ndarray(int)
         indeces of the maximum.
     mx : float
         maximum value.
 
     '''
-    
+
     idx = np.argmax(data)
 
     mx = np.array(data).ravel()[idx]
 
     arg = np.unravel_index(idx, np.array(data).shape)
-    
+
     return arg, mx
 
+
 def FWHM(x, y):
     '''
     It calculates the Full Width at Half Maximum of a 1D curve.
 
     Parameters
     ----------
     x : ndarray
@@ -192,23 +198,24 @@
 
     Returns
     -------
     FWHM: float
         Full Width at Half Maximum of the y curve.
 
     '''
-    
+
     height = 0.5
     height_half_max = np.max(y) * height
     index_max = np.argmax(y)
     x_low = np.interp(height_half_max, y[:index_max], x[:index_max])
     x_high = np.interp(height_half_max, np.flip(y[index_max:]), np.flip(x[index_max:]))
 
     return x_high - x_low
 
+
 def RadialSpectrum(img, pxsize: float = 1, normalize: bool = True):
     '''
     It calculates the radial spectrum of a 2D image.
 
     Parameters
     ----------
     img : ndarray
@@ -222,45 +229,48 @@
     -------
     ftR : ndarray
         Radial spectrum.
     space_f : ndarray
         Frequency axis.
 
     '''
-    
-    fft_img = np.fft.fftn(img, axes = [0, 1])
-    fft_img = np.abs( np.fft.fftshift( fft_img, axes = [0, 1]) )    
-    
+
+    fft_img = np.fft.fftn(img, axes=[0, 1])
+    fft_img = np.abs(np.fft.fftshift(fft_img, axes=[0, 1]))
+
     sx, sy = fft_img.shape
-    c = (sx//2, sy//2)
-    
+    c = (sx // 2, sy // 2)
+
     space_f = np.fft.fftfreq(sx, pxsize)[:c[0]]
-    
+
     ftR = radial_profile(fft_img, c)
-    
+
     ftR = ftR[0][:c[0]] / ftR[1][:c[0]]
-    
+
     ftR = np.real(ftR)
-    
+
     if normalize == True:
-        ftR /= np.max( ftR )
-    
+        ftR /= np.max(ftR)
+
     return ftR, space_f
 
-#%%
+
+# %%
 
 import matplotlib.pyplot as plt
 
 from matplotlib_scalebar.scalebar import ScaleBar
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from matplotlib.colors import Normalize
 
 import numbers
 
-def ShowImg(image: np.ndarray, pxsize_x: float, clabel: str, vmin: float = None, vmax: float = None, fig: plt.Figure = None, ax: plt.axis = None, cmap: str = 'hot'):
+
+def ShowImg(image: np.ndarray, pxsize_x: float, clabel: str = None, vmin: float = None, vmax: float = None,
+            fig: plt.Figure = None, ax: plt.axis = None, cmap: str = 'hot'):
     """
     It shows the input image with a scalebar and a colorbar.
     It returns the corresponding figure and axis.
 
     Parameters
     ----------
     image : np.ndarray
@@ -291,40 +301,50 @@
     -------
     fig : plt.Figure
         Matplotlib figure.
     ax : plt.axis
         Matplotlib axis.
 
     """
-    
+
     if fig == None or ax == None:
         fig, ax = plt.subplots()
-    
-    im = ax.imshow( image, vmin = vmin, vmax = vmax, cmap = cmap )
+
+    im = ax.imshow(image, vmin=vmin, vmax=vmax, cmap=cmap)
     ax.axis('off')
-    
+
     divider = make_axes_locatable(ax)
     cax = divider.append_axes("right", size="5%", pad=0.05)
-    cbar = fig.colorbar(im, cax=cax, ticks = [])# np.floor( [np.min(image), np.max(image)] ), )
+    cbar = fig.colorbar(im, cax=cax, ticks=[])
     # ax.text(1.0,0.4, clabel, rotation=90, transform=ax.transAxes)
 
-    cbar.ax.set_ylabel(clabel, labelpad=-11, rotation=90)
-    
-    cbar.ax.text(1.02, 0.9, f'{ int(np.floor(np.max(image))) }', rotation=90, transform=ax.transAxes)
-    
-    cbar.ax.text(1.02, 0.02, f'{ int(np.floor(np.min(image))) }', rotation=90, transform=ax.transAxes, color = 'white')
-    
+    # cbar.ax.set_ylabel(clabel, labelpad=-11, rotation=90)
+    #
+    # cbar.ax.text(1.02, 0.9, f'{int(np.floor(np.max(image)))}', rotation=90, transform=ax.transAxes)
+    #
+    # cbar.ax.text(1.02, 0.02, f'{int(np.floor(np.min(image)))}', rotation=90, transform=ax.transAxes, color='white')
+
+    vmax = int(np.floor(np.max(image)))
+    vmin = int(np.floor(np.min(image)))
+
+    cbar.ax.text(0.6, 0.5, clabel, horizontalalignment='center', verticalalignment='center',
+                 rotation='vertical', transform=cax.transAxes)
+    cbar.ax.text(0.6, 0.98, f'{vmax}', horizontalalignment='center', verticalalignment='top',
+                 rotation='vertical', transform=cax.transAxes)
+    cbar.ax.text(0.6, 0.02, f'{vmin}', horizontalalignment='center', verticalalignment='bottom',
+                 rotation='vertical', transform=cax.transAxes, color='white')
+
     scalebar = ScaleBar(
-    pxsize_x, "um", # default, extent is calibrated in meters
-    box_alpha=0,
-    color='w',
-    length_fraction=0.25)
-    
+        pxsize_x, "um",  # default, extent is calibrated in meters
+        box_alpha=0,
+        color='w',
+        length_fraction=0.25)
+
     ax.add_artist(scalebar)
-    
+
     return fig, ax
 
 
 def ShowDataset(dset: np.ndarray, cmap: str = 'hot', pxsize: float = None, normalize: bool = False,
                 colorbar: bool = False, xlims: list = [None, None], ylims: list = [None, None],
                 figsize: tuple = (6, 6)) -> plt.Figure:
     '''
@@ -353,62 +373,62 @@
         Size of the figure. The default is (6, 6).
 
     Returns
     -------
     fig : plt.Figure
         Matplotlib figure.
     '''
-    
-    N = int( np.sqrt(dset.shape[-1]) )
-    
+
+    N = int(np.sqrt(dset.shape[-1]))
+
     if normalize == True:
         vmin = np.min(dset)
         vmax = np.max(dset)
-        norm = Normalize(vmin = vmin, vmax = vmax)
+        norm = Normalize(vmin=vmin, vmax=vmax)
 
     fig, ax = plt.subplots(N, N, sharex=True, sharey=True, figsize=figsize)
-    for i in range(N*N):
-        idx = np.unravel_index(i, [N,N])
+    for i in range(N * N):
+        idx = np.unravel_index(i, [N, N])
         if normalize == True:
-            im = ax[idx].imshow(dset[:,:,i], norm = norm, cmap = cmap)
+            im = ax[idx].imshow(dset[:, :, i], norm=norm, cmap=cmap)
         else:
             im = ax[idx].imshow(dset[:, :, i], cmap=cmap)
         ax[idx].set_xlim(xlims)
         ax[idx].set_ylim(ylims)
         ax[idx].axis('off')
-    
+
     if isinstance(pxsize, numbers.Number):
         scalebar = ScaleBar(
-        pxsize, "um", # default, extent is calibrated in meters
-        box_alpha=0,
-        color='w',
-        location = 'lower right',
-        length_fraction=0.5)
-        
-        ax[-1,-1].add_artist(scalebar)
-    
+            pxsize, "um",  # default, extent is calibrated in meters
+            box_alpha=0,
+            color='w',
+            location='lower right',
+            length_fraction=0.5)
+
+        ax[-1, -1].add_artist(scalebar)
+
     fig.tight_layout()
     if colorbar == True and normalize == True:
-        y0 = ax[-1,-1].get_position().y0
-        y1 = ax[0,0].get_position().y1
+        y0 = ax[-1, -1].get_position().y0
+        y1 = ax[0, 0].get_position().y1
         height = y1 - y0
-        
+
         fig.subplots_adjust(right=0.92)
         cbar_ax = fig.add_axes([0.94, y0, 0.05, height])
-        cbar = fig.colorbar(im, cax=cbar_ax, ticks = [])
-        
-        cbar.ax.text(0.3, 0.95, f'{ int(np.floor(vmax)) }', rotation=90, transform=cbar_ax.transAxes)
-        
-        cbar.ax.text(0.3, 0.02, f'{ int(np.floor(vmin)) }', rotation=90, transform=cbar_ax.transAxes, color = 'white')
-        
+        cbar = fig.colorbar(im, cax=cbar_ax, ticks=[])
+
+        cbar.ax.text(0.3, 0.95, f'{int(np.floor(vmax))}', rotation=90, transform=cbar_ax.transAxes)
+
+        cbar.ax.text(0.3, 0.02, f'{int(np.floor(vmin))}', rotation=90, transform=cbar_ax.transAxes, color='white')
+
     return fig
 
 
-def PlotShiftVectors(shift_vectors: np.ndarray, pxsize: float = 1, labels: bool = True, color: np.ndarray = None, cmap: str = 'summer_r', fig: plt.Figure = None,
-                     ax: plt.axis = None):
+def PlotShiftVectors(shift_vectors: np.ndarray, pxsize: float = 1, labels: bool = True, color: np.ndarray = None,
+                     cmap: str = 'summer_r', fig: plt.Figure = None, ax: plt.axis = None):
     """
     It plots the shift vectors in a scatter plot.
     It returns the corresponding figure and axis.
 
     Parameters
     ----------
     shift_vectors : np.ndarray
@@ -435,36 +455,101 @@
     -------
     fig : plt.Figure
         Matplotlib figure.
     ax : plt.axis
         Matplotlib axis.
 
     """
-    
+
     if fig == None or ax == None:
         fig, ax = plt.subplots()
-        
+
     shift = shift_vectors * pxsize
-    
+
     Nch = shift.shape[0]
-    
+
     if color == 'auto':
-        N = int( np.sqrt( Nch ) )
-        x = np.arange(-(N//2), N//2 +1)
-        X,Y = np.meshgrid(x,x)
-        R = np.sqrt(X**2 + Y**2)
+        N = int(np.sqrt(Nch))
+        x = np.arange(-(N // 2), N // 2 + 1)
+        X, Y = np.meshgrid(x, x)
+        R = np.sqrt(X ** 2 + Y ** 2)
         color = R
-    
-    ax.scatter(shift[:,0], shift[:,1], s = 80, c = color, edgecolors = 'black', cmap = cmap)
+
+    ax.scatter(shift[:, 0], shift[:, 1], s=80, c=color, edgecolors='black', cmap=cmap)
     ax.set_aspect('equal', 'box')
-    
+
     if labels == True:
         for n in range(Nch):
-            ax.annotate(str(n), shift[n], xytext=(3, 3), textcoords= 'offset points')
-    
+            ax.annotate(str(n), shift[n], xytext=(3, 3), textcoords='offset points')
+
     ax.set_xlabel(r'Shift$_x$ (nm)')
     ax.set_ylabel(r'Shift$_y$ (nm)')
     ax.set_title('Shift vectors')
 
     ax.set_aspect('equal')
 
-    return fig, ax
+    return fig, ax
+
+
+def ShowFingerprint(dset: np.ndarray, cmap: str = 'hot', colorbar: bool = False, clabel: str = None, normalize: bool = False, fig: plt.Figure = None,
+                    ax: plt.axis = None):
+    """
+    It calculates and shows the fingerprint of an ISM dataset.
+    It returns the corresponding figure and axis.
+
+    Parameters
+    ----------
+    dset : np.ndarray
+        ISM dataset (Nx x Ny x Nch).
+    cmap : str, optional
+        Colormap, to be chosen within the matplotlib list. The default is 'hot'.
+    colorbar : bool, optional
+        If true, a colorbar is shown. The default is False
+    clabel : str, optional
+        Label of the colorbar. The default is None
+    normalize : bool, optional
+        If true, the fingerprint values are normalized between 0 and 1. The default is False
+    fig : plt.Figure, optional
+        Figure where to display the plot. If None, a new figure is created.
+        The default is None.
+    ax : plt.axis, optional
+        Axis where to display the plot. If None, a new axis is created.
+        The default is None.
+
+    Returns
+    -------
+    fig : plt.Figure
+        Matplotlib figure.
+    ax : plt.axis
+        Matplotlib axis.
+    """
+
+    if fig == None or ax == None:
+        fig, ax = plt.subplots()
+
+    N = int( np.sqrt(dset.shape[-1]) )
+    fingerprint = dset.sum(axis=(0, 1)).reshape(N, N)
+    if normalize == True:
+        max_counts = np.max(fingerprint)
+        fingerprint = fingerprint / max_counts
+    im = ax.imshow(fingerprint, cmap=cmap)
+
+    ax.axis('off')
+    fig.tight_layout()
+
+    if colorbar == True:
+
+        vmax = int(np.floor(np.max(fingerprint)))
+        vmin = int(np.floor(np.min(fingerprint)))
+
+        divider = make_axes_locatable(ax)
+        cax = divider.append_axes("right", size="5%", pad=0.05)
+        cbar = fig.colorbar(im, cax=cax, ticks=[])
+
+        cbar.ax.text(0.6, 0.5, clabel, horizontalalignment='center', verticalalignment='center',
+                     rotation='vertical', transform=cax.transAxes)
+        cbar.ax.text(0.6, 0.98, f'{vmax}', horizontalalignment='center', verticalalignment='top',
+                     rotation='vertical', transform=cax.transAxes)
+        cbar.ax.text(0.6, 0.02, f'{vmin}', horizontalalignment='center', verticalalignment='bottom',
+                     rotation='vertical', transform=cax.transAxes, color='white')
+
+    return fig, ax
```

### Comparing `brighteyes-ism-1.1.1/src/brighteyes_ism/dataio/mcs.py` & `brighteyes-ism-1.1.2/src/brighteyes_ism/dataio/mcs.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.1.1/src/brighteyes_ism/simulation/PSF_sim.py` & `brighteyes-ism-1.1.2/src/brighteyes_ism/simulation/PSF_sim.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import scipy.signal as sgn
+from skimage.transform import rotate
 from PyFocus.custom_mask_functions import generate_incident_field, custom_mask_focus_field_XY, plot_in_cartesian
 from poppy.zernike import noll_indices, R, zern_name
 import copy as cp
 
 #%% Zernike
 
 def Zernike(index, A, h, rho, phi, normalize = True):
@@ -332,55 +333,58 @@
     p : np.array(Nx x Nx x N**2)
         array with the pinholes of each detector element
     
     """
     
     p = np.zeros((Nx, Nx, N*N))
     center = Nx//2
-    sizeDet = int(pxdim / M / pxsizex)
+    sizeDet = int( np.round(pxdim / M / pxsizex) )
     if np.mod(sizeDet, 2) == 0:
         sizeDet -= 1 # let this be odd
     sizeDet = np.max((sizeDet, 1))
-    stepDet = int(pxpitch / M / pxsizex)
+    stepDet = int( np.round(pxpitch / M / pxsizex) )
     startcoord = int(np.ceil(center - np.floor(N/2) * stepDet - 0.5 * sizeDet))
 
     i = 0
     for dy in range(N):
         for dx in range(N):
             ymin = np.max((startcoord+dy*stepDet, 0))
             ymax = np.max((startcoord+dy*stepDet+sizeDet, 0))
             xmin = np.max((startcoord+dx*stepDet, 0))
             xmax = np.max((startcoord+dx*stepDet+sizeDet, 0))
             p[ymin:ymax, xmin:xmax, i] = 1
             i += 1    
 
     return p
 
-def SPAD_PSF_2D(N, Nx, pxpitch, pxdim, pxsizex, M, exPar, emPar, stedPar = None, z_shift=0, spad = None, return_entrance_field = False):
+def SPAD_PSF_2D(N, Nx, pxpitch, pxdim, pxsizex, M, exPar, emPar, rotParam = None, stedPar = None, z_shift=0, spad = None, return_entrance_field = False):
     """
     Calculate PSFs for all pixels of the SPAD array by using FFTs
 
     Parameters
     ----------
     N : int
         Number of detector elements in the array in each dimension (typically 5)
     Nx : int
         Number of pixels in each dimension in the simulation array (e.g. 1024)
     pxpitch : float
         Pixel pitch of the detector [nm] (real space, typically 75000)
     pxdim : float
         Detector element size [nm] (real space, typically 50000)
-    pxsize : float
+    pxsizex : float
         Pixel size of the simulation space [nm] (typically 1)
     M : float
         Total magnification of the optical system (typically 500)
     exPar : simSettings object
         object with excitation PSF parameters
     emPar : simSettings object
         object with emission PSF parameters
+    rotParam : np.ndarray
+        array with the mirror and rotation angle to apply to the detection PSFs.
+        The default is None.
     stedPar : simSettings object
         object with STED beam parameters
     z_shift : float
         Distance from the focal plane at which generate the PSF [nm] (optional)
     spad : np.array( N**2 x Nx x Nx)
         Pinholes distribution . If none it is calculated using the input parameters
     return_entrance_field : bool
@@ -419,51 +423,72 @@
     
     if type(stedPar) == simSettings:
         stedPar.mask = 'VP'
         donut = singlePSF(stedPar, pxsizex, Nx, z_shift = z_shift)
         donut *= stedPar.sted_sat/np.max(donut)
         stedPSF = np.exp( - donut * stedPar.sted_pulse / stedPar.sted_tau )
         exPSF *= stedPSF
-    
+
+    # Rotate and mirror detPSF
+
+    if rotParam is None:
+        detPSFrot = detPSF
+    else:
+        detPSFrot = detPSF.copy()
+
+        theta = rotParam[1] * 180 / np.pi
+        mirror = rotParam[2]
+
+        if mirror == -1:
+            detPSFrot = detPSFrot.reshape(Nx, Nx, N, N)
+            detPSFrot = np.flip(detPSFrot, axis=-1)
+            detPSFrot = detPSFrot.reshape(Nx, Nx, N ** 2)
+
+        detPSFrot = rotate(detPSFrot, theta, resize=False, center=None, order=None, mode='constant', cval=0,
+                           clip=True, preserve_range=False)
+
     # Calculate total PSF
     
-    PSF = np.einsum('ijk, ij -> ijk', detPSF, exPSF)
+    PSF = np.einsum('ijk, ij -> ijk', detPSFrot, exPSF)
     
     if return_entrance_field == True:
-        return PSF, detPSF, exPSF, ex_fields, em_fields
+        return PSF, detPSFrot, exPSF, ex_fields, em_fields
     else:
-        return PSF, detPSF, exPSF
+        return PSF, detPSFrot, exPSF
     
-def SPAD_PSF_3D(N, Nx, pxpitch, pxdim, pxsizex, M, exPar, emPar, Nz, pxsizez, stedPar = None, spad = None, stack: str = 'symmetrical'):
+def SPAD_PSF_3D(N, Nx, pxpitch, pxdim, pxsizex, M, exPar, emPar, Nz, pxsizez, rotParam = None, stedPar = None, spad = None, stack: str = 'symmetrical'):
     """
     It calculates a z-stack of PSFs for all the elements of the SPAD array detector.
 
     Parameters
     ----------
     N : int
         Number of detector elements in the array in each dimension (typically 5)
     Nx : int
         Number of pixels in each dimension in the simulation array (e.g. 1024)
     pxpitch : float
         Pixel pitch of the detector [nm] (real space, typically 75000)
     pxdim : float
         Detector element size [nm] (real space, typically 50000)
-    pxsize : float
+    pxsizex : float
         Pixel size of the simulation space [nm] (typically 1)
     M : float
         Total magnification of the optical system (typically 500)
     exPar : simSettings object
         object with excitation PSF parameters
     emPar : simSettings object
         object with emission PSF parameters
     Nz : int
         number of axial planes (typically an odd integer)
         the planes are symmetrically calculated around the focal plane (z = 0)
     pxisez : float
         distance between axial planes [nm]
+    rotParam : np.ndarray
+        array with the mirror and rotation angle to apply to the detection PSFs.
+        The default is None.
     stedPar : simSettings object
         object with STED beam parameters
     spad : np.array( N**2 x Nx x Nx)
         Pinholes distribution . If none it is calculated using the input parameters
     stack : str
         String that defines the direction along z of the simulation.
         If "symmetrical", the stack is generated at planes around z = 0 both on the negative and positive directions.
@@ -492,15 +517,15 @@
     
     PSF = np.empty( (Nz, Nx, Nx, N*N) )
     detPSF = np.empty( (Nz, Nx, Nx, N*N) )
     exPSF = np.empty( (Nz, Nx, Nx) )
     
     for i, z in enumerate(zeta):
         print( f'Calculating the PSFs at z = {z} nm')
-        PSF[i, :, :, :], detPSF[i, :, :, :], exPSF[i, :, :] = SPAD_PSF_2D(N, Nx, pxpitch, pxdim, pxsizex, M, exPar, emPar, stedPar = stedPar, z_shift = z, spad = spad)
+        PSF[i, :, :, :], detPSF[i, :, :, :], exPSF[i, :, :] = SPAD_PSF_2D(N, Nx, pxpitch, pxdim, pxsizex, M, exPar, emPar, rotParam = rotParam, stedPar = stedPar, z_shift = z, spad = spad)
         
     return PSF, detPSF, exPSF
 
 def Fingerprint(dset, volumetric = False):
     """
     Calculate the fingerprint of an ISM dataset.
     The last dimension has to be the spad array channel.
```

### Comparing `brighteyes-ism-1.1.1/src/brighteyes_ism/simulation/Tubulin_sim.py` & `brighteyes-ism-1.1.2/src/brighteyes_ism/simulation/Tubulin_sim.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.1.1/src/brighteyes_ism.egg-info/PKG-INFO` & `brighteyes-ism-1.1.2/src/brighteyes_ism.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brighteyes-ism
-Version: 1.1.1
+Version: 1.1.2
 Summary: A toolbox for analysing and simulating ISM images
 Home-page: https://github.com/VicidominiLab/brighteyes-ism
 Author: Alessandro Zunino
 Author-email: Alessandro Zunino <alessandro.zunino@iit.it>
 Project-URL: Homepage, https://github.com/VicidominiLab/brighteyes-ism
 Project-URL: Documentation, https://brighteyes-ism.readthedocs.io
 Classifier: Programming Language :: Python :: 3.7
@@ -38,15 +38,15 @@
 * Fourier Ring Correlation (https://doi.org/10.1038/s41467-019-11024-z)
 
 The simulation module contains libraries for:
 
 * Generation of ISM point spread functions (https://doi.org/10.1016/j.cpc.2022.108315)
 * Generation of tubulin phantom samples
 
-The dataio module contains libraries for
+The dataio module contains libraries for:
 
 * Reading the data and metadata from the MCS software (https://github.com/VicidominiLab/BrightEyes-MCS)
 
 ----------------------------------
 
 ## Installation
 
@@ -78,14 +78,21 @@
 
 https://github.com/VicidominiLab/BrightEyes-ISM/tree/main/examples
 
 You can read the manual of this package on Read the Docs:
 
 https://brighteyes-ism.readthedocs.io
 
+## Citation
+
+If you find BrightEyes-ISM useful for your research, please cite it as:
+
+_Zunino, A., Slenders, E., Fersini, F. et al. Open-source tools enable accessible and advanced image scanning microscopy data analysis. Nat. Photon. (2023). https://doi.org/10.1038/s41566-023-01216-x_
+
+
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

### Comparing `brighteyes-ism-1.1.1/src/brighteyes_ism.egg-info/SOURCES.txt` & `brighteyes-ism-1.1.2/src/brighteyes_ism.egg-info/SOURCES.txt`

 * *Files identical despite different names*

