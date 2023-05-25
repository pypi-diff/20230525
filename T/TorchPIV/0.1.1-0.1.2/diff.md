# Comparing `tmp/TorchPIV-0.1.1.tar.gz` & `tmp/TorchPIV-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchPIV-0.1.1.tar", last modified: Tue May 23 03:33:44 2023, max compression
+gzip compressed data, was "TorchPIV-0.1.2.tar", last modified: Thu May 25 04:14:04 2023, max compression
```

## Comparing `TorchPIV-0.1.1.tar` & `TorchPIV-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 03:33:44.780071 TorchPIV-0.1.1/
--rw-rw-rw-   0        0        0     1090 2023-05-22 09:07:57.000000 TorchPIV-0.1.1/LICENCE.txt
--rw-rw-rw-   0        0        0     2660 2023-05-23 03:33:44.780071 TorchPIV-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2134 2023-05-23 03:32:06.000000 TorchPIV-0.1.1/README.md
--rw-rw-rw-   0        0        0      108 2023-05-22 09:16:41.000000 TorchPIV-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      815 2023-05-23 03:33:44.781068 TorchPIV-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 03:33:44.749153 TorchPIV-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 03:33:44.768103 TorchPIV-0.1.1/src/TorchPIV.egg-info/
--rw-rw-rw-   0        0        0     2660 2023-05-23 03:33:44.000000 TorchPIV-0.1.1/src/TorchPIV.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-05-23 03:33:44.000000 TorchPIV-0.1.1/src/TorchPIV.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 03:33:44.000000 TorchPIV-0.1.1/src/TorchPIV.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-23 03:33:44.000000 TorchPIV-0.1.1/src/TorchPIV.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 03:33:44.000000 TorchPIV-0.1.1/src/TorchPIV.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-23 03:33:44.778077 TorchPIV-0.1.1/src/torchPIV/
--rw-rw-rw-   0        0        0    17240 2023-05-22 10:05:56.000000 TorchPIV-0.1.1/src/torchPIV/ControlsWidgets.py
--rw-rw-rw-   0        0        0    31145 2023-05-22 10:02:28.000000 TorchPIV-0.1.1/src/torchPIV/PIVbackend.py
--rw-rw-rw-   0        0        0    11894 2023-05-22 10:04:04.000000 TorchPIV-0.1.1/src/torchPIV/PIVwidgets.py
--rw-rw-rw-   0        0        0     5481 2023-05-22 14:35:51.000000 TorchPIV-0.1.1/src/torchPIV/PlotterFunctions.py
--rw-rw-rw-   0        0        0       84 2023-05-22 10:07:12.000000 TorchPIV-0.1.1/src/torchPIV/__init__.py
--rw-rw-rw-   0        0        0     9264 2023-05-22 10:05:31.000000 TorchPIV-0.1.1/src/torchPIV/mainWindow.py
--rw-rw-rw-   0        0        0      391 2023-05-22 15:16:46.000000 TorchPIV-0.1.1/src/torchPIV/settings.json
--rw-rw-rw-   0        0        0      606 2023-05-22 09:09:13.000000 TorchPIV-0.1.1/src/torchPIV/watchman.py
--rw-rw-rw-   0        0        0     6918 2023-05-22 10:03:07.000000 TorchPIV-0.1.1/src/torchPIV/workers.py
+drwxrwxrwx   0        0        0        0 2023-05-25 04:14:04.300022 TorchPIV-0.1.2/
+-rw-rw-rw-   0        0        0     1090 2023-04-06 05:43:08.000000 TorchPIV-0.1.2/LICENCE.txt
+-rw-rw-rw-   0        0        0     2660 2023-05-25 04:14:04.302032 TorchPIV-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2134 2023-05-25 03:54:51.000000 TorchPIV-0.1.2/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-25 03:54:51.000000 TorchPIV-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      815 2023-05-25 04:14:04.313027 TorchPIV-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 04:14:04.062022 TorchPIV-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 04:14:04.158020 TorchPIV-0.1.2/src/TorchPIV.egg-info/
+-rw-rw-rw-   0        0        0     2660 2023-05-25 04:14:04.000000 TorchPIV-0.1.2/src/TorchPIV.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-05-25 04:14:04.000000 TorchPIV-0.1.2/src/TorchPIV.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 04:14:04.000000 TorchPIV-0.1.2/src/TorchPIV.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-25 04:14:04.000000 TorchPIV-0.1.2/src/TorchPIV.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-25 04:14:04.000000 TorchPIV-0.1.2/src/TorchPIV.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 04:14:04.299021 TorchPIV-0.1.2/src/torchPIV/
+-rw-rw-rw-   0        0        0    17240 2023-05-25 03:54:51.000000 TorchPIV-0.1.2/src/torchPIV/ControlsWidgets.py
+-rw-rw-rw-   0        0        0    31145 2023-05-25 04:08:49.000000 TorchPIV-0.1.2/src/torchPIV/PIVbackend.py
+-rw-rw-rw-   0        0        0    11894 2023-05-25 03:54:51.000000 TorchPIV-0.1.2/src/torchPIV/PIVwidgets.py
+-rw-rw-rw-   0        0        0     5481 2023-05-25 03:54:51.000000 TorchPIV-0.1.2/src/torchPIV/PlotterFunctions.py
+-rw-rw-rw-   0        0        0       82 2023-05-25 04:07:54.000000 TorchPIV-0.1.2/src/torchPIV/__init__.py
+-rw-rw-rw-   0        0        0     9264 2023-05-25 03:54:51.000000 TorchPIV-0.1.2/src/torchPIV/mainWindow.py
+-rw-rw-rw-   0        0        0      391 2023-05-25 03:54:51.000000 TorchPIV-0.1.2/src/torchPIV/settings.json
+-rw-rw-rw-   0        0        0      606 2023-05-25 03:54:51.000000 TorchPIV-0.1.2/src/torchPIV/watchman.py
+-rw-rw-rw-   0        0        0     6918 2023-05-25 03:54:51.000000 TorchPIV-0.1.2/src/torchPIV/workers.py
```

### Comparing `TorchPIV-0.1.1/LICENCE.txt` & `TorchPIV-0.1.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.1/PKG-INFO` & `TorchPIV-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: TorchPIV
-Version: 0.1.1
+Version: 0.1.2
 Summary: Package for PIV data analysis
 Home-page: https://github.com/NikNazarov/TorchPIV
 Author: Nikita Nazarov
 Author-email: nazarov.nik.an@gmail.com
 Project-URL: Bug Tracker, https://github.com/NikNazarov/TorchPIV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # PyTorch accelerated Particle Image Velocimetry
 This program implements the basic algorithms of the PIV method, such as an iterative cross-correlation method based on FFT with an integer and continuous displacement __(DWS, CWS)__ of the interrogation windows, filtering and interpolation of the pair loss effect, and so on. At this stage, the __graphical interface__ is available, the ability to select PIV hyperparameters. The key feature of the project is the use of graphics accelerators due to the __torch__ library. PIV algorithm is completely vectorized, what results in a very high performance using the GPU, but still has a room for improvement.
 
 __Parameters of the program:__
```

### Comparing `TorchPIV-0.1.1/README.md` & `TorchPIV-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.1/setup.cfg` & `TorchPIV-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2054 6f72 6368 5049 560d 0a76 6572   = TorchPIV..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e31 0d0a 6175  sion = 0.1.1..au
+00000020: 7369 6f6e 203d 2030 2e31 2e32 0d0a 6175  sion = 0.1.2..au
 00000030: 7468 6f72 203d 204e 696b 6974 6120 4e61  thor = Nikita Na
 00000040: 7a61 726f 760d 0a61 7574 686f 725f 656d  zarov..author_em
 00000050: 6169 6c20 3d20 6e61 7a61 726f 762e 6e69  ail = nazarov.ni
 00000060: 6b2e 616e 4067 6d61 696c 2e63 6f6d 0d0a  k.an@gmail.com..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 5061  description = Pa
 00000080: 636b 6167 6520 666f 7220 5049 5620 6461  ckage for PIV da
 00000090: 7461 2061 6e61 6c79 7369 730d 0a6c 6f6e  ta analysis..lon
@@ -29,15 +29,15 @@
 000001c0: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
 000001d0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
 000001e0: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
 000001f0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
 00000200: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
 00000210: 2073 7263 0d0a 7061 636b 6167 6573 203d   src..packages =
 00000220: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
-00000230: 6571 7569 7265 7320 3d20 3e3d 332e 390d  equires = >=3.9.
+00000230: 6571 7569 7265 7320 3d20 3e3d 332e 380d  equires = >=3.8.
 00000240: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
 00000250: 7320 3d20 0d0a 096d 6174 706c 6f74 6c69  s = ...matplotli
 00000260: 620d 0a09 6e75 6d70 790d 0a09 6f70 656e  b...numpy...open
 00000270: 6376 5f70 7974 686f 6e0d 0a09 7061 6e64  cv_python...pand
 00000280: 6173 0d0a 0950 7951 7435 0d0a 0973 6369  as...PyQt5...sci
 00000290: 7079 0d0a 0977 6174 6368 646f 670d 0a64  py...watchdog..d
 000002a0: 6570 656e 6465 6e63 795f 6c69 6e6b 7320  ependency_links
```

### Comparing `TorchPIV-0.1.1/src/TorchPIV.egg-info/PKG-INFO` & `TorchPIV-0.1.2/src/TorchPIV.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: TorchPIV
-Version: 0.1.1
+Version: 0.1.2
 Summary: Package for PIV data analysis
 Home-page: https://github.com/NikNazarov/TorchPIV
 Author: Nikita Nazarov
 Author-email: nazarov.nik.an@gmail.com
 Project-URL: Bug Tracker, https://github.com/NikNazarov/TorchPIV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # PyTorch accelerated Particle Image Velocimetry
 This program implements the basic algorithms of the PIV method, such as an iterative cross-correlation method based on FFT with an integer and continuous displacement __(DWS, CWS)__ of the interrogation windows, filtering and interpolation of the pair loss effect, and so on. At this stage, the __graphical interface__ is available, the ability to select PIV hyperparameters. The key feature of the project is the use of graphics accelerators due to the __torch__ library. PIV algorithm is completely vectorized, what results in a very high performance using the GPU, but still has a room for improvement.
 
 __Parameters of the program:__
```

### Comparing `TorchPIV-0.1.1/src/torchPIV/ControlsWidgets.py` & `TorchPIV-0.1.2/src/torchPIV/ControlsWidgets.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.1/src/torchPIV/PIVbackend.py` & `TorchPIV-0.1.2/src/torchPIV/PIVbackend.py`

 * *Files 0% similar despite different names*

```diff
@@ -543,15 +543,15 @@
     x0: np.ndarray,  
     y0: np.ndarray,  
     u0: np.ndarray,  
     v0: np.ndarray,
     validation_mask: np.ndarray,
     wind_size: int, 
     overlap: int,
-    device: torch.device) -> tuple[np.ndarray, ...]:
+    device: torch.device) -> Tuple[np.ndarray, ...]:
         iter_proc = time()
         spline_u = interpolate.RectBivariateSpline(y0[:,0], x0[0,:], u0)
         spline_v = interpolate.RectBivariateSpline(y0[:,0], x0[0,:], v0)
         u0 = spline_u(self.slice_y, self.slice_x)
         v0 = spline_v(self.slice_y, self.slice_x)
         validate = False
         if validation_mask is not None:
@@ -615,15 +615,15 @@
     def __call__(self,
     frame_a: torch.Tensor,
     frame_b: torch.Tensor, 
     x0: np.ndarray,  
     y0: np.ndarray,  
     u0: np.ndarray,  
     v0: np.ndarray,
-    validation_mask: np.ndarray) -> tuple[np.ndarray, ...]:
+    validation_mask: np.ndarray) -> Tuple[np.ndarray, ...]:
         
         iter_proc = time()
         spline_u = interpolate.RectBivariateSpline(y0[:,0], x0[0,:], u0)
         spline_v = interpolate.RectBivariateSpline(y0[:,0], x0[0,:], v0)
 
         u0 = spline_u(self.slice_y, self.slice_x)
         v0 = spline_v(self.slice_y, self.slice_x)
@@ -682,15 +682,15 @@
     def __call__(self,
     frame_a: torch.Tensor, 
     frame_b: torch.Tensor, 
     x0:       np.ndarray, 
     y0:       np.ndarray, 
     u0:      np.ndarray, 
     v0:      np.ndarray,
-    validation_mask: np.ndarray)->tuple[np.ndarray, ...]:
+    validation_mask: np.ndarray)->Tuple[np.ndarray, ...]:
 
         iter_proc = time()
 
 
         spline_u = interpolate.RectBivariateSpline(y0[:,0], x0[0,:], u0)
         spline_v = interpolate.RectBivariateSpline(y0[:,0], x0[0,:], v0)
```

### Comparing `TorchPIV-0.1.1/src/torchPIV/PIVwidgets.py` & `TorchPIV-0.1.2/src/torchPIV/PIVwidgets.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.1/src/torchPIV/PlotterFunctions.py` & `TorchPIV-0.1.2/src/torchPIV/PlotterFunctions.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.1/src/torchPIV/mainWindow.py` & `TorchPIV-0.1.2/src/torchPIV/mainWindow.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.1/src/torchPIV/watchman.py` & `TorchPIV-0.1.2/src/torchPIV/watchman.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.1/src/torchPIV/workers.py` & `TorchPIV-0.1.2/src/torchPIV/workers.py`

 * *Files identical despite different names*

