# Comparing `tmp/obpgenerator-0.0.19.tar.gz` & `tmp/obpgenerator-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obpgenerator-0.0.19.tar", last modified: Mon Apr 24 09:33:03 2023, max compression
+gzip compressed data, was "obpgenerator-0.0.20.tar", last modified: Thu May 25 09:57:19 2023, max compression
```

## Comparing `obpgenerator-0.0.19.tar` & `obpgenerator-0.0.20.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 09:33:03.860252 obpgenerator-0.0.19/
--rw-rw-rw-   0        0        0     1091 2023-03-14 16:54:43.000000 obpgenerator-0.0.19/LICENSE
--rw-rw-rw-   0        0        0     2880 2023-04-24 09:33:03.860252 obpgenerator-0.0.19/PKG-INFO
--rw-rw-rw-   0        0        0     2390 2023-04-21 15:00:47.000000 obpgenerator-0.0.19/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 09:33:03.775915 obpgenerator-0.0.19/obpgenerator/
--rw-rw-rw-   0        0        0     3681 2023-04-21 12:27:56.000000 obpgenerator-0.0.19/obpgenerator/Layer.py
--rw-rw-rw-   0        0        0     5214 2023-04-24 09:15:08.000000 obpgenerator-0.0.19/obpgenerator/Part.py
--rw-rw-rw-   0        0        0     4647 2023-04-21 13:56:52.000000 obpgenerator-0.0.19/obpgenerator/Shape.py
--rw-rw-rw-   0        0        0      171 2023-03-21 14:44:59.000000 obpgenerator-0.0.19/obpgenerator/__init__.py
--rw-rw-rw-   0        0        0     1311 2023-03-20 20:01:41.000000 obpgenerator-0.0.19/obpgenerator/file_import.py
--rw-rw-rw-   0        0        0      842 2023-03-24 15:54:31.000000 obpgenerator-0.0.19/obpgenerator/generate_obp.py
--rw-rw-rw-   0        0        0     3352 2023-03-22 07:43:38.000000 obpgenerator-0.0.19/obpgenerator/layer_sorting.py
--rw-rw-rw-   0        0        0     3150 2023-02-24 22:18:01.000000 obpgenerator-0.0.19/obpgenerator/manufacturing_settings.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:33:03.832781 obpgenerator-0.0.19/obpgenerator/melt_strategies/
--rw-rw-rw-   0        0        0       56 2023-04-11 11:45:09.000000 obpgenerator-0.0.19/obpgenerator/melt_strategies/__init__.py
--rw-rw-rw-   0        0        0     2940 2023-02-24 19:34:30.000000 obpgenerator-0.0.19/obpgenerator/melt_strategies/line_melting.py
--rw-rw-rw-   0        0        0      558 2023-02-24 19:10:25.000000 obpgenerator-0.0.19/obpgenerator/melt_strategies/point_melting.py
--rw-rw-rw-   0        0        0      703 2023-03-17 14:49:52.000000 obpgenerator-0.0.19/obpgenerator/shape_melting.py
--rw-rw-rw-   0        0        0     3131 2023-04-24 09:15:40.000000 obpgenerator-0.0.19/obpgenerator/slicer.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:33:03.858252 obpgenerator-0.0.19/obpgenerator/visualization/
--rw-rw-rw-   0        0        0       60 2023-04-12 12:20:29.000000 obpgenerator-0.0.19/obpgenerator/visualization/__init__.py
--rw-rw-rw-   0        0        0     1155 2023-04-12 14:51:19.000000 obpgenerator-0.0.19/obpgenerator/visualization/obp_to_matplotlib.py
--rw-rw-rw-   0        0        0     3178 2023-04-12 14:51:18.000000 obpgenerator-0.0.19/obpgenerator/visualization/visualization.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:33:03.805754 obpgenerator-0.0.19/obpgenerator.egg-info/
--rw-rw-rw-   0        0        0     2880 2023-04-24 09:33:03.000000 obpgenerator-0.0.19/obpgenerator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      753 2023-04-24 09:33:03.000000 obpgenerator-0.0.19/obpgenerator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 09:33:03.000000 obpgenerator-0.0.19/obpgenerator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-24 09:33:03.000000 obpgenerator-0.0.19/obpgenerator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-24 09:33:03.000000 obpgenerator-0.0.19/obpgenerator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      106 2023-03-20 19:39:06.000000 obpgenerator-0.0.19/pyproject.toml
--rw-rw-rw-   0        0        0      646 2023-04-24 09:33:03.863256 obpgenerator-0.0.19/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 09:57:19.617842 obpgenerator-0.0.20/
+-rw-rw-rw-   0        0        0     1091 2023-03-14 16:54:43.000000 obpgenerator-0.0.20/LICENSE
+-rw-rw-rw-   0        0        0     4470 2023-05-25 09:57:19.618842 obpgenerator-0.0.20/PKG-INFO
+-rw-rw-rw-   0        0        0     3980 2023-05-25 09:55:23.000000 obpgenerator-0.0.20/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 09:57:19.541725 obpgenerator-0.0.20/obpgenerator/
+-rw-rw-rw-   0        0        0     4402 2023-05-10 14:38:35.000000 obpgenerator-0.0.20/obpgenerator/Layer.py
+-rw-rw-rw-   0        0        0     7003 2023-05-10 14:38:32.000000 obpgenerator-0.0.20/obpgenerator/Part.py
+-rw-rw-rw-   0        0        0     4647 2023-04-21 13:56:52.000000 obpgenerator-0.0.20/obpgenerator/Shape.py
+-rw-rw-rw-   0        0        0      171 2023-03-21 14:44:59.000000 obpgenerator-0.0.20/obpgenerator/__init__.py
+-rw-rw-rw-   0        0        0     1311 2023-03-20 20:01:41.000000 obpgenerator-0.0.20/obpgenerator/file_import.py
+-rw-rw-rw-   0        0        0      842 2023-03-24 15:54:31.000000 obpgenerator-0.0.20/obpgenerator/generate_obp.py
+-rw-rw-rw-   0        0        0     3352 2023-03-22 07:43:38.000000 obpgenerator-0.0.20/obpgenerator/layer_sorting.py
+-rw-rw-rw-   0        0        0     3150 2023-02-24 22:18:01.000000 obpgenerator-0.0.20/obpgenerator/manufacturing_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:57:19.586836 obpgenerator-0.0.20/obpgenerator/melt_strategies/
+-rw-rw-rw-   0        0        0       56 2023-04-11 11:45:09.000000 obpgenerator-0.0.20/obpgenerator/melt_strategies/__init__.py
+-rw-rw-rw-   0        0        0     2940 2023-02-24 19:34:30.000000 obpgenerator-0.0.20/obpgenerator/melt_strategies/line_melting.py
+-rw-rw-rw-   0        0        0      558 2023-02-24 19:10:25.000000 obpgenerator-0.0.20/obpgenerator/melt_strategies/point_melting.py
+-rw-rw-rw-   0        0        0      703 2023-03-17 14:49:52.000000 obpgenerator-0.0.20/obpgenerator/shape_melting.py
+-rw-rw-rw-   0        0        0     3131 2023-04-24 09:15:40.000000 obpgenerator-0.0.20/obpgenerator/slicer.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:57:19.616843 obpgenerator-0.0.20/obpgenerator/visualization/
+-rw-rw-rw-   0        0        0       60 2023-04-12 12:20:29.000000 obpgenerator-0.0.20/obpgenerator/visualization/__init__.py
+-rw-rw-rw-   0        0        0     1155 2023-04-12 14:51:19.000000 obpgenerator-0.0.20/obpgenerator/visualization/obp_to_matplotlib.py
+-rw-rw-rw-   0        0        0     3178 2023-04-12 14:51:18.000000 obpgenerator-0.0.20/obpgenerator/visualization/visualization.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:57:19.573827 obpgenerator-0.0.20/obpgenerator.egg-info/
+-rw-rw-rw-   0        0        0     4470 2023-05-25 09:57:19.000000 obpgenerator-0.0.20/obpgenerator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      753 2023-05-25 09:57:19.000000 obpgenerator-0.0.20/obpgenerator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 09:57:19.000000 obpgenerator-0.0.20/obpgenerator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-25 09:57:19.000000 obpgenerator-0.0.20/obpgenerator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-25 09:57:19.000000 obpgenerator-0.0.20/obpgenerator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      106 2023-03-20 19:39:06.000000 obpgenerator-0.0.20/pyproject.toml
+-rw-rw-rw-   0        0        0      646 2023-05-25 09:57:19.621844 obpgenerator-0.0.20/setup.cfg
```

### Comparing `obpgenerator-0.0.19/LICENSE` & `obpgenerator-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.19/README.md` & `obpgenerator-0.0.20/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 - Melt strategy (can handle different versions of both line and point melting)
 - Number of scans
 
 Layer consist of one or more shapes. On this level you can change which order you want to scan the shapes and if you want to ramp manufacturing settings (successively increase/decrease e.g. energy input) between the scans of a shape
 
 Part consist of one or more layers. On this level you can select layer height, scraper settings and other.
 
-# Example
+# Examples
 
+2D:
 Example from examples/snake_cube.py where an svg file file is imported.
 
 ```bash
 import obpgenerator
 
 file_path1 = "examples\layer_nine_cubes.svg"
 file_path2 = "examples\layer_15x15_cube.svg"
@@ -50,12 +51,42 @@
 my_layer.set_melt_strategies("line_snake")
 my_layer.set_nmb_of_scans(3)
 my_layer.sorting_strategy = "ramp_manufacturing_settings"
 
 my_layer.export_obp("output.obp")
 ```
 
+3D:
+Example from examples/example_3D.py where two stl files are imported.
+
+```bash
+import obpgenerator.Part as Part
+import obpgenerator.slicer as slicer
+import obpgenerator.manufacturing_settings as manufacturing_settings
+
+stl_files = ["examples\\cube1.stl", "examples\\cube2.stl"]
+slices = slicer.slice_stl(stl_files,0.15) #slices the stl files with a layer height of 0.15 mm
+my_part = Part.Part()
+my_part.create_from_mplt_paths(slices)
+
+#Sets two different manufacturing settings for the two geometries
+settings1 = manufacturing_settings.ManufacturingSetting()
+settings1.set_spot_size(0.5) #[µm]
+settings1.set_beam_power(1000) #[W]
+settings1.set_dwell_time(1) #[ns]
+settings1.set_scan_speed(12) #[micrometers/second] 
+settings2 = manufacturing_settings.ManufacturingSetting()
+settings1.set_spot_size(0.75) #[µm]
+settings1.set_beam_power(1500) #[W]
+settings1.set_dwell_time(1) #[ns]
+settings1.set_scan_speed(10) #[micrometers/second] 
+
+my_part.set_layers(0.15, settings1, size=60, angle_between_layers=10, melt_strategy="point_random", nmb_of_scans=1, sorting_strategy="shapes_first") #First we just set one manufacturing setting
+my_part.set_settings(manufacturing_settings = [settings1, settings2], melt_strategies=["line_snake","point_random"]) #We can then set different settings for the seperate geometries
+my_part.export_build_file(r"C:\Users\antwi87\Downloads\obp_files", export_shapes_individual=False) #Exports the build file (each layer will be one obp file, if export_shapes_individual=True each geoemtry will be in seperate obp files)
+```
+
 # To package
 - Delete old builds in the \dist folder 
 - Update the version in the setup.cfg file
 - run "python -m build"
 - upload to pip with "twine upload dist/*"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `obpgenerator-0.0.19/obpgenerator/Layer.py` & `obpgenerator-0.0.20/obpgenerator/Layer.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,32 @@
         obp_elements = []
         for shape in self.shapes_to_export:
             shape.generate_melt_strategy()
             shape.generate_obp_elements()
             obp_elements = obp_elements + shape.obp_elements
         return obp_elements
 
+    def export_shape_obp(self,path):
+        layer_path = path[0:-4]
+        self.sort_layers()
+        for i, shape in enumerate(self.shapes_to_export):
+            shape.generate_melt_strategy()
+            shape.generate_obp_elements()
+            path = layer_path + "_" + str(i) + ".obp" 
+            obp.write_obp(shape.obp_elements,path)
+    
+    def export_shape_obpj(self,path):
+        layer_path = path[0:-5]
+        self.sort_layers()
+        for i, shape in enumerate(self.shapes_to_export):
+            shape.generate_melt_strategy()
+            shape.generate_obp_elements()
+            path = layer_path + "_" + str(i) + ".obpj" 
+            obp.write_obpj(shape.obp_elements,path)
+    
     def export_obp(self,path):
         obp_elements = self.create_obp_elements()
         obp.write_obp(obp_elements,path)
     
     def export_obpj(self,path):
         obp_elements = self.create_obp_elements()
         obp.write_obpj(obp_elements,path)
```

### Comparing `obpgenerator-0.0.19/obpgenerator/Part.py` & `obpgenerator-0.0.20/obpgenerator/Part.py`

 * *Files 18% similar despite different names*

```diff
@@ -53,19 +53,42 @@
             self.layers[i].set_shapes(spacing, size=size, angle=angle)
             self.layers[i].set_manufacturing_settings(manufacturing_settings)
             self.layers[i].set_melt_strategies(melt_strategy)
             self.layers[i].set_nmb_of_scans(nmb_of_scans)
             self.layers[i].sorting_strategy = sorting_strategy
             angle = angle + angle_between_layers
     
+    def set_settings(self, manufacturing_settings = None, melt_strategies=None, nmb_of_scans=None):
+        #Sets settings for each shape in each layer, the settings should be arrays where the first element in the array is assigned to the
+        #first shape in each layer, the second element to the second shape in each layer, and so on. If the array is shorter than the number
+        #number of shapes in a layer it will loop from the beginning in the array
+        if manufacturing_settings != None:
+            for layer in self.layers:
+                layer_settings = []
+                for idx in range(layer.shapes):
+                    layer_settings.append(manufacturing_settings[idx % len(manufacturing_settings)])
+                layer.set_manufacturing_settings(layer_settings)
+        if melt_strategies != None:
+            for layer in self.layers:
+                layer_settings = []
+                for idx in range(layer.shapes):
+                    layer_settings.append(melt_strategies[idx % len(melt_strategies)])
+                layer.set_melt_strategies(layer_settings)
+        if nmb_of_scans != None:
+            for layer in self.layers:
+                layer_settings = []
+                for idx in range(layer.shapes):
+                    layer_settings.append(nmb_of_scans[idx % len(nmb_of_scans)])
+                layer.set_nmb_of_scans(layer_settings)
+
     def create_obps(self):
         for i in range(len(self.layers)):
             self.layers[i].create_obp_elements()
 
-    def export_build_file(self, folder_path, file_name="freemelt_run_file.yml"):
+    def export_build_file(self, folder_path, file_name="freemelt_run_file.yml", export_shapes_individual=False):
         
         # Create directory to save obp files
         path = os.path.join(folder_path, "obp_files")
         layer_paths = []
         try:
             os.mkdir(path)
         except FileExistsError:
@@ -85,16 +108,22 @@
         build_file.append("    file: \"" + self.post_heat.file + "\"")
         build_file.append("    repetitions: " + str(self.post_heat.repetitions))
         build_file.append("  build:")
         build_file.append("    layers: " + str(len(self.layers)))
         build_file.append("    files:")
         for i in range(len(self.layers)):
             file_path = os.path.join(path, "layer"+str(i)+".obp")
-            self.layers[i].export_obp(file_path)
-            build_file.append("      - \"" + "/obp_files/layer"+str(i)+".obp" + "\"")
+            if export_shapes_individual:
+                build_file.append("      -")
+                self.layers[i].export_shape_obp(file_path)
+                for ii in range(len(self.layers[i].shapes)):
+                    build_file.append("        - \"" + "/obp_files/layer"+str(i)+"_"+str(ii)+".obp" + "\"")
+            else:
+                self.layers[i].export_obp(file_path)
+                build_file.append("      - \"" + "/obp_files/layer"+str(i)+".obp" + "\"")
         build_file.append("  layerfeed:")
         build_file.append("    build_piston_distance: " + str(self.layer_feed.build_piston_distance))
         build_file.append("    powder_piston_distance: " + str(self.layer_feed.powder_piston_distance))
         build_file.append("    recoater_advance_speed: " + str(self.layer_feed.recoater_advance_speed))
         build_file.append("    recoater_retract_speed: " + str(self.layer_feed.recoater_retract_speed))
         build_file.append("    recoater_dwell_time: " + str(self.layer_feed.recoater_dwell_time))
         build_file.append("    recoater_full_repeats: " + str(self.layer_feed.recoater_full_repeats))
```

### Comparing `obpgenerator-0.0.19/obpgenerator/Shape.py` & `obpgenerator-0.0.20/obpgenerator/Shape.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.19/obpgenerator/file_import.py` & `obpgenerator-0.0.20/obpgenerator/file_import.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.19/obpgenerator/generate_obp.py` & `obpgenerator-0.0.20/obpgenerator/generate_obp.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.19/obpgenerator/layer_sorting.py` & `obpgenerator-0.0.20/obpgenerator/layer_sorting.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.19/obpgenerator/manufacturing_settings.py` & `obpgenerator-0.0.20/obpgenerator/manufacturing_settings.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.19/obpgenerator/melt_strategies/line_melting.py` & `obpgenerator-0.0.20/obpgenerator/melt_strategies/line_melting.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.19/obpgenerator/melt_strategies/point_melting.py` & `obpgenerator-0.0.20/obpgenerator/melt_strategies/point_melting.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.19/obpgenerator/shape_melting.py` & `obpgenerator-0.0.20/obpgenerator/shape_melting.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.19/obpgenerator/slicer.py` & `obpgenerator-0.0.20/obpgenerator/slicer.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.19/obpgenerator/visualization/obp_to_matplotlib.py` & `obpgenerator-0.0.20/obpgenerator/visualization/obp_to_matplotlib.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.19/obpgenerator/visualization/visualization.py` & `obpgenerator-0.0.20/obpgenerator/visualization/visualization.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.19/obpgenerator.egg-info/SOURCES.txt` & `obpgenerator-0.0.20/obpgenerator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.19/setup.cfg` & `obpgenerator-0.0.20/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206f 6270 6765 6e65 7261 746f 720d   = obpgenerator.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e31  .version = 0.0.1
-00000030: 390d 0a61 7574 686f 7220 3d20 416e 746f  9..author = Anto
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e32  .version = 0.0.2
+00000030: 300d 0a61 7574 686f 7220 3d20 416e 746f  0..author = Anto
 00000040: 6e20 5769 6265 7267 0d0a 6175 7468 6f72  n Wiberg..author
 00000050: 5f65 6d61 696c 203d 2077 6962 6572 672e  _email = wiberg.
 00000060: 616e 746f 6e40 676d 6169 6c2e 636f 6d0d  anton@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2047  .description = G
 00000080: 656e 6572 6174 696f 6e20 6f66 206f 7065  eneration of ope
 00000090: 6e20 6265 616d 2070 6174 6820 6669 6c65  n beam path file
 000000a0: 7320 6261 7365 6420 6f6e 2064 6966 6665  s based on diffe
```

