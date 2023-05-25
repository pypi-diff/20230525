# Comparing `tmp/TorchPIV-0.1.4.tar.gz` & `tmp/TorchPIV-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchPIV-0.1.4.tar", last modified: Thu May 25 04:26:19 2023, max compression
+gzip compressed data, was "TorchPIV-0.1.6.tar", last modified: Thu May 25 04:36:29 2023, max compression
```

## Comparing `TorchPIV-0.1.4.tar` & `TorchPIV-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 04:26:19.709483 TorchPIV-0.1.4/
--rw-rw-rw-   0        0        0     1090 2023-04-06 05:43:08.000000 TorchPIV-0.1.4/LICENCE.txt
--rw-rw-rw-   0        0        0     2660 2023-05-25 04:26:19.710484 TorchPIV-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2134 2023-05-25 03:54:51.000000 TorchPIV-0.1.4/README.md
--rw-rw-rw-   0        0        0      108 2023-05-25 03:54:51.000000 TorchPIV-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0      829 2023-05-25 04:26:19.713483 TorchPIV-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 04:26:19.630942 TorchPIV-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 04:26:19.692483 TorchPIV-0.1.4/src/TorchPIV.egg-info/
--rw-rw-rw-   0        0        0     2660 2023-05-25 04:26:19.000000 TorchPIV-0.1.4/src/TorchPIV.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-05-25 04:26:19.000000 TorchPIV-0.1.4/src/TorchPIV.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 04:26:19.000000 TorchPIV-0.1.4/src/TorchPIV.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-05-25 04:26:19.000000 TorchPIV-0.1.4/src/TorchPIV.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-25 04:26:19.000000 TorchPIV-0.1.4/src/TorchPIV.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 04:26:19.708487 TorchPIV-0.1.4/src/torchPIV/
--rw-rw-rw-   0        0        0    17240 2023-05-25 03:54:51.000000 TorchPIV-0.1.4/src/torchPIV/ControlsWidgets.py
--rw-rw-rw-   0        0        0    31145 2023-05-25 04:08:49.000000 TorchPIV-0.1.4/src/torchPIV/PIVbackend.py
--rw-rw-rw-   0        0        0    11894 2023-05-25 03:54:51.000000 TorchPIV-0.1.4/src/torchPIV/PIVwidgets.py
--rw-rw-rw-   0        0        0     5481 2023-05-25 03:54:51.000000 TorchPIV-0.1.4/src/torchPIV/PlotterFunctions.py
--rw-rw-rw-   0        0        0       82 2023-05-25 04:07:54.000000 TorchPIV-0.1.4/src/torchPIV/__init__.py
--rw-rw-rw-   0        0        0     9264 2023-05-25 03:54:51.000000 TorchPIV-0.1.4/src/torchPIV/mainWindow.py
--rw-rw-rw-   0        0        0      391 2023-05-25 03:54:51.000000 TorchPIV-0.1.4/src/torchPIV/settings.json
--rw-rw-rw-   0        0        0      606 2023-05-25 03:54:51.000000 TorchPIV-0.1.4/src/torchPIV/watchman.py
--rw-rw-rw-   0        0        0     6918 2023-05-25 03:54:51.000000 TorchPIV-0.1.4/src/torchPIV/workers.py
+drwxrwxrwx   0        0        0        0 2023-05-25 04:36:29.664223 TorchPIV-0.1.6/
+-rw-rw-rw-   0        0        0     1090 2023-04-06 05:43:08.000000 TorchPIV-0.1.6/LICENCE.txt
+-rw-rw-rw-   0        0        0     2660 2023-05-25 04:36:29.664223 TorchPIV-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2134 2023-05-25 03:54:51.000000 TorchPIV-0.1.6/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-25 03:54:51.000000 TorchPIV-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0      931 2023-05-25 04:36:29.677224 TorchPIV-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 04:36:29.578225 TorchPIV-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 04:36:29.635236 TorchPIV-0.1.6/src/TorchPIV.egg-info/
+-rw-rw-rw-   0        0        0     2660 2023-05-25 04:36:29.000000 TorchPIV-0.1.6/src/TorchPIV.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-05-25 04:36:29.000000 TorchPIV-0.1.6/src/TorchPIV.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       91 2023-05-25 04:36:29.000000 TorchPIV-0.1.6/src/TorchPIV.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-25 04:36:29.000000 TorchPIV-0.1.6/src/TorchPIV.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-25 04:36:29.000000 TorchPIV-0.1.6/src/TorchPIV.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 04:36:29.662225 TorchPIV-0.1.6/src/torchPIV/
+-rw-rw-rw-   0        0        0    17240 2023-05-25 03:54:51.000000 TorchPIV-0.1.6/src/torchPIV/ControlsWidgets.py
+-rw-rw-rw-   0        0        0    31145 2023-05-25 04:08:49.000000 TorchPIV-0.1.6/src/torchPIV/PIVbackend.py
+-rw-rw-rw-   0        0        0    11894 2023-05-25 03:54:51.000000 TorchPIV-0.1.6/src/torchPIV/PIVwidgets.py
+-rw-rw-rw-   0        0        0     5481 2023-05-25 03:54:51.000000 TorchPIV-0.1.6/src/torchPIV/PlotterFunctions.py
+-rw-rw-rw-   0        0        0       82 2023-05-25 04:07:54.000000 TorchPIV-0.1.6/src/torchPIV/__init__.py
+-rw-rw-rw-   0        0        0     9264 2023-05-25 03:54:51.000000 TorchPIV-0.1.6/src/torchPIV/mainWindow.py
+-rw-rw-rw-   0        0        0      391 2023-05-25 03:54:51.000000 TorchPIV-0.1.6/src/torchPIV/settings.json
+-rw-rw-rw-   0        0        0      606 2023-05-25 03:54:51.000000 TorchPIV-0.1.6/src/torchPIV/watchman.py
+-rw-rw-rw-   0        0        0     6918 2023-05-25 03:54:51.000000 TorchPIV-0.1.6/src/torchPIV/workers.py
```

### Comparing `TorchPIV-0.1.4/LICENCE.txt` & `TorchPIV-0.1.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.4/PKG-INFO` & `TorchPIV-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TorchPIV
-Version: 0.1.4
+Version: 0.1.6
 Summary: Package for PIV data analysis
 Home-page: https://github.com/NikNazarov/TorchPIV
 Author: Nikita Nazarov
 Author-email: nazarov.nik.an@gmail.com
 Project-URL: Bug Tracker, https://github.com/NikNazarov/TorchPIV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `TorchPIV-0.1.4/README.md` & `TorchPIV-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.4/setup.cfg` & `TorchPIV-0.1.6/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2054 6f72 6368 5049 560d 0a76 6572   = TorchPIV..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e34 0d0a 6175  sion = 0.1.4..au
+00000020: 7369 6f6e 203d 2030 2e31 2e36 0d0a 6175  sion = 0.1.6..au
 00000030: 7468 6f72 203d 204e 696b 6974 6120 4e61  thor = Nikita Na
 00000040: 7a61 726f 760d 0a61 7574 686f 725f 656d  zarov..author_em
 00000050: 6169 6c20 3d20 6e61 7a61 726f 762e 6e69  ail = nazarov.ni
 00000060: 6b2e 616e 4067 6d61 696c 2e63 6f6d 0d0a  k.an@gmail.com..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 5061  description = Pa
 00000080: 636b 6167 6520 666f 7220 5049 5620 6461  ckage for PIV da
 00000090: 7461 2061 6e61 6c79 7369 730d 0a6c 6f6e  ta analysis..lon
@@ -36,17 +36,24 @@
 00000230: 6571 7569 7265 7320 3d20 3e3d 332e 380d  equires = >=3.8.
 00000240: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
 00000250: 7320 3d20 0d0a 096d 6174 706c 6f74 6c69  s = ...matplotli
 00000260: 620d 0a09 6e75 6d70 790d 0a09 6f70 656e  b...numpy...open
 00000270: 6376 5f70 7974 686f 6e0d 0a09 7061 6e64  cv_python...pand
 00000280: 6173 0d0a 0950 7951 7435 0d0a 0973 6369  as...PyQt5...sci
 00000290: 7079 0d0a 0977 6174 6368 646f 670d 0a09  py...watchdog...
-000002a0: 746f 7263 683d 3d32 2e30 2e31 2b63 7531  torch==2.0.1+cu1
-000002b0: 3137 0d0a 0974 6f72 6368 7669 7369 6f6e  17...torchvision
-000002c0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-000002d0: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
-000002e0: 7265 203d 2073 7263 0d0a 0d0a 5b6f 7074  re = src....[opt
-000002f0: 696f 6e73 2e70 6163 6b61 6765 5f64 6174  ions.package_dat
-00000300: 615d 0d0a 2a20 3d20 2a2e 6a73 6f6e 2c0d  a]..* = *.json,.
-00000310: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-00000320: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-00000330: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+000002a0: 746f 7263 680d 0a09 746f 7263 6876 6973  torch...torchvis
+000002b0: 696f 6e0d 0a64 6570 656e 6465 6e63 795f  ion..dependency_
+000002c0: 6c69 6e6b 7320 3d20 0d0a 0974 6f72 6368  links = ...torch
+000002d0: 2040 2068 7474 7073 3a2f 2f64 6f77 6e6c   @ https://downl
+000002e0: 6f61 642e 7079 746f 7263 682e 6f72 672f  oad.pytorch.org/
+000002f0: 7768 6c2f 6375 3131 372f 746f 7263 682d  whl/cu117/torch-
+00000300: 322e 302e 3125 2532 4263 7531 3137 2d63  2.0.1%%2Bcu117-c
+00000310: 7033 382d 6370 3338 2d77 696e 5f61 6d64  p38-cp38-win_amd
+00000320: 3634 2e77 686c 0d0a 0d0a 5b6f 7074 696f  64.whl....[optio
+00000330: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
+00000340: 5d0d 0a77 6865 7265 203d 2073 7263 0d0a  ]..where = src..
+00000350: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+00000360: 6765 5f64 6174 615d 0d0a 2a20 3d20 2a2e  ge_data]..* = *.
+00000370: 6a73 6f6e 2c0d 0a0d 0a5b 6567 675f 696e  json,....[egg_in
+00000380: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+00000390: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+000003a0: 0a0d 0a                                  ...
```

### Comparing `TorchPIV-0.1.4/src/TorchPIV.egg-info/PKG-INFO` & `TorchPIV-0.1.6/src/TorchPIV.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TorchPIV
-Version: 0.1.4
+Version: 0.1.6
 Summary: Package for PIV data analysis
 Home-page: https://github.com/NikNazarov/TorchPIV
 Author: Nikita Nazarov
 Author-email: nazarov.nik.an@gmail.com
 Project-URL: Bug Tracker, https://github.com/NikNazarov/TorchPIV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `TorchPIV-0.1.4/src/torchPIV/ControlsWidgets.py` & `TorchPIV-0.1.6/src/torchPIV/ControlsWidgets.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.4/src/torchPIV/PIVbackend.py` & `TorchPIV-0.1.6/src/torchPIV/PIVbackend.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.4/src/torchPIV/PIVwidgets.py` & `TorchPIV-0.1.6/src/torchPIV/PIVwidgets.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.4/src/torchPIV/PlotterFunctions.py` & `TorchPIV-0.1.6/src/torchPIV/PlotterFunctions.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.4/src/torchPIV/mainWindow.py` & `TorchPIV-0.1.6/src/torchPIV/mainWindow.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.4/src/torchPIV/watchman.py` & `TorchPIV-0.1.6/src/torchPIV/watchman.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.4/src/torchPIV/workers.py` & `TorchPIV-0.1.6/src/torchPIV/workers.py`

 * *Files identical despite different names*

