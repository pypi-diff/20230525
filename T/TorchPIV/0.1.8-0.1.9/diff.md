# Comparing `tmp/TorchPIV-0.1.8.tar.gz` & `tmp/TorchPIV-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchPIV-0.1.8.tar", last modified: Thu May 25 05:18:22 2023, max compression
+gzip compressed data, was "TorchPIV-0.1.9.tar", last modified: Thu May 25 05:29:10 2023, max compression
```

## Comparing `TorchPIV-0.1.8.tar` & `TorchPIV-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 05:18:22.601053 TorchPIV-0.1.8/
--rw-rw-rw-   0        0        0     1090 2023-04-06 05:43:08.000000 TorchPIV-0.1.8/LICENCE.txt
--rw-rw-rw-   0        0        0     2660 2023-05-25 05:18:22.601053 TorchPIV-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2134 2023-05-25 03:54:51.000000 TorchPIV-0.1.8/README.md
--rw-rw-rw-   0        0        0      108 2023-05-25 03:54:51.000000 TorchPIV-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0      911 2023-05-25 05:18:22.604055 TorchPIV-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 05:18:22.467054 TorchPIV-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 05:18:22.556059 TorchPIV-0.1.8/src/TorchPIV.egg-info/
--rw-rw-rw-   0        0        0     2660 2023-05-25 05:18:22.000000 TorchPIV-0.1.8/src/TorchPIV.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-05-25 05:18:22.000000 TorchPIV-0.1.8/src/TorchPIV.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       59 2023-05-25 05:18:22.000000 TorchPIV-0.1.8/src/TorchPIV.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-05-25 05:18:22.000000 TorchPIV-0.1.8/src/TorchPIV.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-25 05:18:22.000000 TorchPIV-0.1.8/src/TorchPIV.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 05:18:22.599058 TorchPIV-0.1.8/src/torchPIV/
--rw-rw-rw-   0        0        0    17240 2023-05-25 03:54:51.000000 TorchPIV-0.1.8/src/torchPIV/ControlsWidgets.py
--rw-rw-rw-   0        0        0    31145 2023-05-25 04:08:49.000000 TorchPIV-0.1.8/src/torchPIV/PIVbackend.py
--rw-rw-rw-   0        0        0    11894 2023-05-25 03:54:51.000000 TorchPIV-0.1.8/src/torchPIV/PIVwidgets.py
--rw-rw-rw-   0        0        0     5481 2023-05-25 03:54:51.000000 TorchPIV-0.1.8/src/torchPIV/PlotterFunctions.py
--rw-rw-rw-   0        0        0       82 2023-05-25 04:57:42.000000 TorchPIV-0.1.8/src/torchPIV/__init__.py
--rw-rw-rw-   0        0        0     9264 2023-05-25 03:54:51.000000 TorchPIV-0.1.8/src/torchPIV/mainWindow.py
--rw-rw-rw-   0        0        0      391 2023-05-25 03:54:51.000000 TorchPIV-0.1.8/src/torchPIV/settings.json
--rw-rw-rw-   0        0        0      606 2023-05-25 03:54:51.000000 TorchPIV-0.1.8/src/torchPIV/watchman.py
--rw-rw-rw-   0        0        0     6918 2023-05-25 03:54:51.000000 TorchPIV-0.1.8/src/torchPIV/workers.py
+drwxrwxrwx   0        0        0        0 2023-05-25 05:29:10.000571 TorchPIV-0.1.9/
+-rw-rw-rw-   0        0        0     1090 2023-04-06 05:43:08.000000 TorchPIV-0.1.9/LICENCE.txt
+-rw-rw-rw-   0        0        0     2660 2023-05-25 05:29:10.000571 TorchPIV-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2134 2023-05-25 03:54:51.000000 TorchPIV-0.1.9/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-25 03:54:51.000000 TorchPIV-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      910 2023-05-25 05:29:10.017571 TorchPIV-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 05:29:09.915575 TorchPIV-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 05:29:09.966570 TorchPIV-0.1.9/src/TorchPIV.egg-info/
+-rw-rw-rw-   0        0        0     2660 2023-05-25 05:29:09.000000 TorchPIV-0.1.9/src/TorchPIV.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-05-25 05:29:09.000000 TorchPIV-0.1.9/src/TorchPIV.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 05:29:09.000000 TorchPIV-0.1.9/src/TorchPIV.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-25 05:29:09.000000 TorchPIV-0.1.9/src/TorchPIV.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-25 05:29:09.000000 TorchPIV-0.1.9/src/TorchPIV.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 05:29:09.991587 TorchPIV-0.1.9/src/torchPIV/
+-rw-rw-rw-   0        0        0    17240 2023-05-25 03:54:51.000000 TorchPIV-0.1.9/src/torchPIV/ControlsWidgets.py
+-rw-rw-rw-   0        0        0    31145 2023-05-25 04:08:49.000000 TorchPIV-0.1.9/src/torchPIV/PIVbackend.py
+-rw-rw-rw-   0        0        0    11894 2023-05-25 03:54:51.000000 TorchPIV-0.1.9/src/torchPIV/PIVwidgets.py
+-rw-rw-rw-   0        0        0     5481 2023-05-25 03:54:51.000000 TorchPIV-0.1.9/src/torchPIV/PlotterFunctions.py
+-rw-rw-rw-   0        0        0       82 2023-05-25 04:57:42.000000 TorchPIV-0.1.9/src/torchPIV/__init__.py
+-rw-rw-rw-   0        0        0     9264 2023-05-25 03:54:51.000000 TorchPIV-0.1.9/src/torchPIV/mainWindow.py
+-rw-rw-rw-   0        0        0      391 2023-05-25 03:54:51.000000 TorchPIV-0.1.9/src/torchPIV/settings.json
+-rw-rw-rw-   0        0        0      606 2023-05-25 03:54:51.000000 TorchPIV-0.1.9/src/torchPIV/watchman.py
+-rw-rw-rw-   0        0        0     6918 2023-05-25 03:54:51.000000 TorchPIV-0.1.9/src/torchPIV/workers.py
```

### Comparing `TorchPIV-0.1.8/LICENCE.txt` & `TorchPIV-0.1.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.8/PKG-INFO` & `TorchPIV-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TorchPIV
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package for PIV data analysis
 Home-page: https://github.com/NikNazarov/TorchPIV
 Author: Nikita Nazarov
 Author-email: nazarov.nik.an@gmail.com
 Project-URL: Bug Tracker, https://github.com/NikNazarov/TorchPIV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `TorchPIV-0.1.8/README.md` & `TorchPIV-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.8/setup.cfg` & `TorchPIV-0.1.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2054 6f72 6368 5049 560d 0a76 6572   = TorchPIV..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e38 0d0a 6175  sion = 0.1.8..au
+00000020: 7369 6f6e 203d 2030 2e31 2e39 0d0a 6175  sion = 0.1.9..au
 00000030: 7468 6f72 203d 204e 696b 6974 6120 4e61  thor = Nikita Na
 00000040: 7a61 726f 760d 0a61 7574 686f 725f 656d  zarov..author_em
 00000050: 6169 6c20 3d20 6e61 7a61 726f 762e 6e69  ail = nazarov.ni
 00000060: 6b2e 616e 4067 6d61 696c 2e63 6f6d 0d0a  k.an@gmail.com..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 5061  description = Pa
 00000080: 636b 6167 6520 666f 7220 5049 5620 6461  ckage for PIV da
 00000090: 7461 2061 6e61 6c79 7369 730d 0a6c 6f6e  ta analysis..lon
@@ -30,28 +30,28 @@
 000001d0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
 000001e0: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
 000001f0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
 00000200: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
 00000210: 2073 7263 0d0a 7061 636b 6167 6573 203d   src..packages =
 00000220: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
 00000230: 6571 7569 7265 7320 3d20 3e3d 332e 380d  equires = >=3.8.
-00000240: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-00000250: 7320 3d20 0d0a 096d 6174 706c 6f74 6c69  s = ...matplotli
-00000260: 620d 0a09 6e75 6d70 790d 0a09 6f70 656e  b...numpy...open
-00000270: 6376 5f70 7974 686f 6e0d 0a09 7061 6e64  cv_python...pand
-00000280: 6173 0d0a 0950 7951 7435 0d0a 0973 6369  as...PyQt5...sci
-00000290: 7079 0d0a 0977 6174 6368 646f 670d 0a09  py...watchdog...
-000002a0: 746f 7263 683d 3d32 2e30 2e31 2b63 7531  torch==2.0.1+cu1
-000002b0: 3137 0d0a 0974 6f72 6368 7669 7369 6f6e  17...torchvision
-000002c0: 0d0a 6465 7065 6e64 656e 6379 5f6c 696e  ..dependency_lin
-000002d0: 6b73 203d 200d 0a09 746f 7263 6820 4020  ks = ...torch @ 
-000002e0: 6874 7470 733a 2f2f 646f 776e 6c6f 6164  https://download
-000002f0: 2e70 7974 6f72 6368 2e6f 7267 2f77 686c  .pytorch.org/whl
-00000300: 2f74 6f72 6368 5f73 7461 626c 652e 6874  /torch_stable.ht
-00000310: 6d6c 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  ml....[options.p
-00000320: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
-00000330: 6865 7265 203d 2073 7263 0d0a 0d0a 5b6f  here = src....[o
-00000340: 7074 696f 6e73 2e70 6163 6b61 6765 5f64  ptions.package_d
-00000350: 6174 615d 0d0a 2a20 3d20 2a2e 6a73 6f6e  ata]..* = *.json
-00000360: 2c0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  ,....[egg_info].
-00000370: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000380: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000240: 0a74 6f72 6368 2040 2068 7474 7073 203d  .torch @ https =
+00000250: 202f 2f64 6f77 6e6c 6f61 642e 7079 746f   //download.pyto
+00000260: 7263 682e 6f72 672f 7768 6c2f 6375 3131  rch.org/whl/cu11
+00000270: 372f 746f 7263 682d 322e 302e 3125 2532  7/torch-2.0.1%%2
+00000280: 4263 7531 3137 2d63 7033 382d 6370 3338  Bcu117-cp38-cp38
+00000290: 2d77 696e 5f61 6d64 3634 2e77 686c 0d0a  -win_amd64.whl..
+000002a0: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
+000002b0: 203d 200d 0a09 6d61 7470 6c6f 746c 6962   = ...matplotlib
+000002c0: 0d0a 096e 756d 7079 0d0a 096f 7065 6e63  ...numpy...openc
+000002d0: 765f 7079 7468 6f6e 0d0a 0970 616e 6461  v_python...panda
+000002e0: 730d 0a09 5079 5174 350d 0a09 7363 6970  s...PyQt5...scip
+000002f0: 790d 0a09 7761 7463 6864 6f67 0d0a 6465  y...watchdog..de
+00000300: 7065 6e64 656e 6379 5f6c 696e 6b73 203d  pendency_links =
+00000310: 200d 0a0d 0a5b 6f70 7469 6f6e 732e 7061   ....[options.pa
+00000320: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
+00000330: 6572 6520 3d20 7372 630d 0a0d 0a5b 6f70  ere = src....[op
+00000340: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
+00000350: 7461 5d0d 0a2a 203d 202a 2e6a 736f 6e2c  ta]..* = *.json,
+00000360: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000370: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000380: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `TorchPIV-0.1.8/src/TorchPIV.egg-info/PKG-INFO` & `TorchPIV-0.1.9/src/TorchPIV.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TorchPIV
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package for PIV data analysis
 Home-page: https://github.com/NikNazarov/TorchPIV
 Author: Nikita Nazarov
 Author-email: nazarov.nik.an@gmail.com
 Project-URL: Bug Tracker, https://github.com/NikNazarov/TorchPIV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `TorchPIV-0.1.8/src/torchPIV/ControlsWidgets.py` & `TorchPIV-0.1.9/src/torchPIV/ControlsWidgets.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.8/src/torchPIV/PIVbackend.py` & `TorchPIV-0.1.9/src/torchPIV/PIVbackend.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.8/src/torchPIV/PIVwidgets.py` & `TorchPIV-0.1.9/src/torchPIV/PIVwidgets.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.8/src/torchPIV/PlotterFunctions.py` & `TorchPIV-0.1.9/src/torchPIV/PlotterFunctions.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.8/src/torchPIV/mainWindow.py` & `TorchPIV-0.1.9/src/torchPIV/mainWindow.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.8/src/torchPIV/watchman.py` & `TorchPIV-0.1.9/src/torchPIV/watchman.py`

 * *Files identical despite different names*

### Comparing `TorchPIV-0.1.8/src/torchPIV/workers.py` & `TorchPIV-0.1.9/src/torchPIV/workers.py`

 * *Files identical despite different names*

