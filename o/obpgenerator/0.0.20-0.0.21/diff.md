# Comparing `tmp/obpgenerator-0.0.20.tar.gz` & `tmp/obpgenerator-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obpgenerator-0.0.20.tar", last modified: Thu May 25 09:57:19 2023, max compression
+gzip compressed data, was "obpgenerator-0.0.21.tar", last modified: Thu May 25 13:54:19 2023, max compression
```

## Comparing `obpgenerator-0.0.20.tar` & `obpgenerator-0.0.21.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 09:57:19.617842 obpgenerator-0.0.20/
--rw-rw-rw-   0        0        0     1091 2023-03-14 16:54:43.000000 obpgenerator-0.0.20/LICENSE
--rw-rw-rw-   0        0        0     4470 2023-05-25 09:57:19.618842 obpgenerator-0.0.20/PKG-INFO
--rw-rw-rw-   0        0        0     3980 2023-05-25 09:55:23.000000 obpgenerator-0.0.20/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 09:57:19.541725 obpgenerator-0.0.20/obpgenerator/
--rw-rw-rw-   0        0        0     4402 2023-05-10 14:38:35.000000 obpgenerator-0.0.20/obpgenerator/Layer.py
--rw-rw-rw-   0        0        0     7003 2023-05-10 14:38:32.000000 obpgenerator-0.0.20/obpgenerator/Part.py
--rw-rw-rw-   0        0        0     4647 2023-04-21 13:56:52.000000 obpgenerator-0.0.20/obpgenerator/Shape.py
--rw-rw-rw-   0        0        0      171 2023-03-21 14:44:59.000000 obpgenerator-0.0.20/obpgenerator/__init__.py
--rw-rw-rw-   0        0        0     1311 2023-03-20 20:01:41.000000 obpgenerator-0.0.20/obpgenerator/file_import.py
--rw-rw-rw-   0        0        0      842 2023-03-24 15:54:31.000000 obpgenerator-0.0.20/obpgenerator/generate_obp.py
--rw-rw-rw-   0        0        0     3352 2023-03-22 07:43:38.000000 obpgenerator-0.0.20/obpgenerator/layer_sorting.py
--rw-rw-rw-   0        0        0     3150 2023-02-24 22:18:01.000000 obpgenerator-0.0.20/obpgenerator/manufacturing_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:57:19.586836 obpgenerator-0.0.20/obpgenerator/melt_strategies/
--rw-rw-rw-   0        0        0       56 2023-04-11 11:45:09.000000 obpgenerator-0.0.20/obpgenerator/melt_strategies/__init__.py
--rw-rw-rw-   0        0        0     2940 2023-02-24 19:34:30.000000 obpgenerator-0.0.20/obpgenerator/melt_strategies/line_melting.py
--rw-rw-rw-   0        0        0      558 2023-02-24 19:10:25.000000 obpgenerator-0.0.20/obpgenerator/melt_strategies/point_melting.py
--rw-rw-rw-   0        0        0      703 2023-03-17 14:49:52.000000 obpgenerator-0.0.20/obpgenerator/shape_melting.py
--rw-rw-rw-   0        0        0     3131 2023-04-24 09:15:40.000000 obpgenerator-0.0.20/obpgenerator/slicer.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:57:19.616843 obpgenerator-0.0.20/obpgenerator/visualization/
--rw-rw-rw-   0        0        0       60 2023-04-12 12:20:29.000000 obpgenerator-0.0.20/obpgenerator/visualization/__init__.py
--rw-rw-rw-   0        0        0     1155 2023-04-12 14:51:19.000000 obpgenerator-0.0.20/obpgenerator/visualization/obp_to_matplotlib.py
--rw-rw-rw-   0        0        0     3178 2023-04-12 14:51:18.000000 obpgenerator-0.0.20/obpgenerator/visualization/visualization.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:57:19.573827 obpgenerator-0.0.20/obpgenerator.egg-info/
--rw-rw-rw-   0        0        0     4470 2023-05-25 09:57:19.000000 obpgenerator-0.0.20/obpgenerator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      753 2023-05-25 09:57:19.000000 obpgenerator-0.0.20/obpgenerator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 09:57:19.000000 obpgenerator-0.0.20/obpgenerator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-25 09:57:19.000000 obpgenerator-0.0.20/obpgenerator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-25 09:57:19.000000 obpgenerator-0.0.20/obpgenerator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      106 2023-03-20 19:39:06.000000 obpgenerator-0.0.20/pyproject.toml
--rw-rw-rw-   0        0        0      646 2023-05-25 09:57:19.621844 obpgenerator-0.0.20/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 13:54:19.457991 obpgenerator-0.0.21/
+-rw-rw-rw-   0        0        0     1091 2023-03-14 16:54:43.000000 obpgenerator-0.0.21/LICENSE
+-rw-rw-rw-   0        0        0     4470 2023-05-25 13:54:19.458992 obpgenerator-0.0.21/PKG-INFO
+-rw-rw-rw-   0        0        0     3980 2023-05-25 09:55:23.000000 obpgenerator-0.0.21/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 13:54:19.362624 obpgenerator-0.0.21/obpgenerator/
+-rw-rw-rw-   0        0        0     4402 2023-05-10 14:38:35.000000 obpgenerator-0.0.21/obpgenerator/Layer.py
+-rw-rw-rw-   0        0        0     7018 2023-05-25 13:51:26.000000 obpgenerator-0.0.21/obpgenerator/Part.py
+-rw-rw-rw-   0        0        0     4647 2023-04-21 13:56:52.000000 obpgenerator-0.0.21/obpgenerator/Shape.py
+-rw-rw-rw-   0        0        0      171 2023-03-21 14:44:59.000000 obpgenerator-0.0.21/obpgenerator/__init__.py
+-rw-rw-rw-   0        0        0     1311 2023-03-20 20:01:41.000000 obpgenerator-0.0.21/obpgenerator/file_import.py
+-rw-rw-rw-   0        0        0      842 2023-03-24 15:54:31.000000 obpgenerator-0.0.21/obpgenerator/generate_obp.py
+-rw-rw-rw-   0        0        0     3352 2023-03-22 07:43:38.000000 obpgenerator-0.0.21/obpgenerator/layer_sorting.py
+-rw-rw-rw-   0        0        0     3150 2023-02-24 22:18:01.000000 obpgenerator-0.0.21/obpgenerator/manufacturing_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:54:19.426638 obpgenerator-0.0.21/obpgenerator/melt_strategies/
+-rw-rw-rw-   0        0        0       56 2023-04-11 11:45:09.000000 obpgenerator-0.0.21/obpgenerator/melt_strategies/__init__.py
+-rw-rw-rw-   0        0        0     2940 2023-02-24 19:34:30.000000 obpgenerator-0.0.21/obpgenerator/melt_strategies/line_melting.py
+-rw-rw-rw-   0        0        0      558 2023-02-24 19:10:25.000000 obpgenerator-0.0.21/obpgenerator/melt_strategies/point_melting.py
+-rw-rw-rw-   0        0        0      703 2023-03-17 14:49:52.000000 obpgenerator-0.0.21/obpgenerator/shape_melting.py
+-rw-rw-rw-   0        0        0     3131 2023-04-24 09:15:40.000000 obpgenerator-0.0.21/obpgenerator/slicer.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:54:19.455984 obpgenerator-0.0.21/obpgenerator/visualization/
+-rw-rw-rw-   0        0        0       60 2023-04-12 12:20:29.000000 obpgenerator-0.0.21/obpgenerator/visualization/__init__.py
+-rw-rw-rw-   0        0        0     1155 2023-04-12 14:51:19.000000 obpgenerator-0.0.21/obpgenerator/visualization/obp_to_matplotlib.py
+-rw-rw-rw-   0        0        0     3178 2023-04-12 14:51:18.000000 obpgenerator-0.0.21/obpgenerator/visualization/visualization.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:54:19.395631 obpgenerator-0.0.21/obpgenerator.egg-info/
+-rw-rw-rw-   0        0        0     4470 2023-05-25 13:54:19.000000 obpgenerator-0.0.21/obpgenerator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      753 2023-05-25 13:54:19.000000 obpgenerator-0.0.21/obpgenerator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 13:54:19.000000 obpgenerator-0.0.21/obpgenerator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-25 13:54:19.000000 obpgenerator-0.0.21/obpgenerator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-25 13:54:19.000000 obpgenerator-0.0.21/obpgenerator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      106 2023-03-20 19:39:06.000000 obpgenerator-0.0.21/pyproject.toml
+-rw-rw-rw-   0        0        0      646 2023-05-25 13:54:19.460993 obpgenerator-0.0.21/setup.cfg
```

### Comparing `obpgenerator-0.0.20/LICENSE` & `obpgenerator-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.20/PKG-INFO` & `obpgenerator-0.0.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obpgenerator
-Version: 0.0.20
+Version: 0.0.21
 Summary: Generation of open beam path files based on different strategies
 Home-page: https://github.com/wiberganton/obpgenerator
 Author: Anton Wiberg
 Author-email: wiberg.anton@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `obpgenerator-0.0.20/README.md` & `obpgenerator-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.20/obpgenerator/Layer.py` & `obpgenerator-0.0.21/obpgenerator/Layer.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.20/obpgenerator/Part.py` & `obpgenerator-0.0.21/obpgenerator/Part.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,27 +60,27 @@
     def set_settings(self, manufacturing_settings = None, melt_strategies=None, nmb_of_scans=None):
         #Sets settings for each shape in each layer, the settings should be arrays where the first element in the array is assigned to the
         #first shape in each layer, the second element to the second shape in each layer, and so on. If the array is shorter than the number
         #number of shapes in a layer it will loop from the beginning in the array
         if manufacturing_settings != None:
             for layer in self.layers:
                 layer_settings = []
-                for idx in range(layer.shapes):
+                for idx in range(len(layer.shapes)):
                     layer_settings.append(manufacturing_settings[idx % len(manufacturing_settings)])
                 layer.set_manufacturing_settings(layer_settings)
         if melt_strategies != None:
             for layer in self.layers:
                 layer_settings = []
-                for idx in range(layer.shapes):
+                for idx in range(len(layer.shapes)):
                     layer_settings.append(melt_strategies[idx % len(melt_strategies)])
                 layer.set_melt_strategies(layer_settings)
         if nmb_of_scans != None:
             for layer in self.layers:
                 layer_settings = []
-                for idx in range(layer.shapes):
+                for idx in range(len(layer.shapes)):
                     layer_settings.append(nmb_of_scans[idx % len(nmb_of_scans)])
                 layer.set_nmb_of_scans(layer_settings)
 
     def create_obps(self):
         for i in range(len(self.layers)):
             self.layers[i].create_obp_elements()
```

### Comparing `obpgenerator-0.0.20/obpgenerator/Shape.py` & `obpgenerator-0.0.21/obpgenerator/Shape.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.20/obpgenerator/file_import.py` & `obpgenerator-0.0.21/obpgenerator/file_import.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.20/obpgenerator/generate_obp.py` & `obpgenerator-0.0.21/obpgenerator/generate_obp.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.20/obpgenerator/layer_sorting.py` & `obpgenerator-0.0.21/obpgenerator/layer_sorting.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.20/obpgenerator/manufacturing_settings.py` & `obpgenerator-0.0.21/obpgenerator/manufacturing_settings.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.20/obpgenerator/melt_strategies/line_melting.py` & `obpgenerator-0.0.21/obpgenerator/melt_strategies/line_melting.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.20/obpgenerator/melt_strategies/point_melting.py` & `obpgenerator-0.0.21/obpgenerator/melt_strategies/point_melting.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.20/obpgenerator/shape_melting.py` & `obpgenerator-0.0.21/obpgenerator/shape_melting.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.20/obpgenerator/slicer.py` & `obpgenerator-0.0.21/obpgenerator/slicer.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.20/obpgenerator/visualization/obp_to_matplotlib.py` & `obpgenerator-0.0.21/obpgenerator/visualization/obp_to_matplotlib.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.20/obpgenerator/visualization/visualization.py` & `obpgenerator-0.0.21/obpgenerator/visualization/visualization.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.20/obpgenerator.egg-info/PKG-INFO` & `obpgenerator-0.0.21/obpgenerator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obpgenerator
-Version: 0.0.20
+Version: 0.0.21
 Summary: Generation of open beam path files based on different strategies
 Home-page: https://github.com/wiberganton/obpgenerator
 Author: Anton Wiberg
 Author-email: wiberg.anton@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `obpgenerator-0.0.20/obpgenerator.egg-info/SOURCES.txt` & `obpgenerator-0.0.21/obpgenerator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.20/setup.cfg` & `obpgenerator-0.0.21/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206f 6270 6765 6e65 7261 746f 720d   = obpgenerator.
 00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e32  .version = 0.0.2
-00000030: 300d 0a61 7574 686f 7220 3d20 416e 746f  0..author = Anto
+00000030: 310d 0a61 7574 686f 7220 3d20 416e 746f  1..author = Anto
 00000040: 6e20 5769 6265 7267 0d0a 6175 7468 6f72  n Wiberg..author
 00000050: 5f65 6d61 696c 203d 2077 6962 6572 672e  _email = wiberg.
 00000060: 616e 746f 6e40 676d 6169 6c2e 636f 6d0d  anton@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2047  .description = G
 00000080: 656e 6572 6174 696f 6e20 6f66 206f 7065  eneration of ope
 00000090: 6e20 6265 616d 2070 6174 6820 6669 6c65  n beam path file
 000000a0: 7320 6261 7365 6420 6f6e 2064 6966 6665  s based on diffe
```

