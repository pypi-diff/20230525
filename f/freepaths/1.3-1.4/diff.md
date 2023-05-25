# Comparing `tmp/freepaths-1.3.tar.gz` & `tmp/freepaths-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freepaths-1.3.tar", last modified: Thu May 11 08:56:37 2023, max compression
+gzip compressed data, was "freepaths-1.4.tar", last modified: Thu May 25 06:42:16 2023, max compression
```

## Comparing `freepaths-1.3.tar` & `freepaths-1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-11 08:56:37.149307 freepaths-1.3/
--rw-r--r--   0 r         (1000) r         (1000)     5298 2023-05-11 08:56:37.149307 freepaths-1.3/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)     4542 2023-02-22 13:18:35.000000 freepaths-1.3/README.md
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-11 08:56:37.149307 freepaths-1.3/freepaths/
--rw-r--r--   0 r         (1000) r         (1000)      869 2023-05-11 07:21:33.000000 freepaths-1.3/freepaths/__main__.py
--rw-r--r--   0 r         (1000) r         (1000)     3677 2023-05-11 08:30:00.000000 freepaths-1.3/freepaths/animation.py
--rw-r--r--   0 r         (1000) r         (1000)     8051 2023-05-11 07:22:21.000000 freepaths-1.3/freepaths/config.py
--rw-r--r--   0 r         (1000) r         (1000)     8022 2023-05-11 07:22:40.000000 freepaths-1.3/freepaths/data.py
--rw-r--r--   0 r         (1000) r         (1000)     2747 2023-05-11 07:15:01.000000 freepaths-1.3/freepaths/default_config.py
--rw-r--r--   0 r         (1000) r         (1000)     2650 2023-02-01 09:15:48.000000 freepaths-1.3/freepaths/flight.py
--rw-r--r--   0 r         (1000) r         (1000)     4366 2023-02-03 02:30:26.000000 freepaths-1.3/freepaths/main_mfp_sampling.py
--rw-r--r--   0 r         (1000) r         (1000)     3330 2023-05-11 07:20:52.000000 freepaths-1.3/freepaths/main_tracing.py
--rw-r--r--   0 r         (1000) r         (1000)     8647 2023-01-25 08:49:48.000000 freepaths-1.3/freepaths/maps.py
--rw-r--r--   0 r         (1000) r         (1000)     3797 2023-01-25 08:49:48.000000 freepaths-1.3/freepaths/materials.py
--rw-r--r--   0 r         (1000) r         (1000)      733 2023-01-24 09:26:17.000000 freepaths-1.3/freepaths/move.py
--rw-r--r--   0 r         (1000) r         (1000)      663 2023-05-11 06:25:40.000000 freepaths-1.3/freepaths/options.py
--rw-r--r--   0 r         (1000) r         (1000)     4837 2023-01-25 08:49:48.000000 freepaths-1.3/freepaths/output_info.py
--rw-r--r--   0 r         (1000) r         (1000)    15058 2023-05-11 06:36:24.000000 freepaths-1.3/freepaths/output_plots.py
--rw-r--r--   0 r         (1000) r         (1000)     2348 2023-02-03 08:43:58.000000 freepaths-1.3/freepaths/output_structure.py
--rw-r--r--   0 r         (1000) r         (1000)     8569 2023-05-11 06:25:46.000000 freepaths-1.3/freepaths/phonon.py
--rw-r--r--   0 r         (1000) r         (1000)      580 2023-01-24 09:16:58.000000 freepaths-1.3/freepaths/progress.py
--rw-r--r--   0 r         (1000) r         (1000)     2312 2023-05-11 06:31:01.000000 freepaths-1.3/freepaths/run_phonon.py
--rw-r--r--   0 r         (1000) r         (1000)    27604 2023-05-11 06:25:47.000000 freepaths-1.3/freepaths/scattering.py
--rw-r--r--   0 r         (1000) r         (1000)     1550 2023-01-25 08:51:17.000000 freepaths-1.3/freepaths/scattering_types.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-11 08:56:37.149307 freepaths-1.3/freepaths.egg-info/
--rw-r--r--   0 r         (1000) r         (1000)     5298 2023-05-11 08:56:37.000000 freepaths-1.3/freepaths.egg-info/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)      702 2023-05-11 08:56:37.000000 freepaths-1.3/freepaths.egg-info/SOURCES.txt
--rw-r--r--   0 r         (1000) r         (1000)        1 2023-05-11 08:56:37.000000 freepaths-1.3/freepaths.egg-info/dependency_links.txt
--rw-r--r--   0 r         (1000) r         (1000)       53 2023-05-11 08:56:37.000000 freepaths-1.3/freepaths.egg-info/entry_points.txt
--rw-r--r--   0 r         (1000) r         (1000)       31 2023-05-11 08:56:37.000000 freepaths-1.3/freepaths.egg-info/requires.txt
--rw-r--r--   0 r         (1000) r         (1000)       10 2023-05-11 08:56:37.000000 freepaths-1.3/freepaths.egg-info/top_level.txt
--rw-r--r--   0 r         (1000) r         (1000)       91 2022-11-27 00:35:48.000000 freepaths-1.3/pyproject.toml
--rw-r--r--   0 r         (1000) r         (1000)       38 2023-05-11 08:56:37.149307 freepaths-1.3/setup.cfg
--rw-r--r--   0 r         (1000) r         (1000)     1439 2023-02-03 05:40:49.000000 freepaths-1.3/setup.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-25 06:42:16.638523 freepaths-1.4/
+-rw-r--r--   0 r         (1000) r         (1000)     5298 2023-05-25 06:42:16.638523 freepaths-1.4/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)     4542 2023-02-22 13:18:35.000000 freepaths-1.4/README.md
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-25 06:42:16.638523 freepaths-1.4/freepaths/
+-rw-r--r--   0 r         (1000) r         (1000)      869 2023-05-25 05:49:31.000000 freepaths-1.4/freepaths/__main__.py
+-rw-r--r--   0 r         (1000) r         (1000)     3677 2023-05-11 08:30:00.000000 freepaths-1.4/freepaths/animation.py
+-rw-r--r--   0 r         (1000) r         (1000)    10197 2023-05-25 05:32:25.000000 freepaths-1.4/freepaths/config.py
+-rw-r--r--   0 r         (1000) r         (1000)     8140 2023-05-25 02:30:39.000000 freepaths-1.4/freepaths/data.py
+-rw-r--r--   0 r         (1000) r         (1000)     3122 2023-05-25 06:39:51.000000 freepaths-1.4/freepaths/default_config.py
+-rw-r--r--   0 r         (1000) r         (1000)     2650 2023-02-01 09:15:48.000000 freepaths-1.4/freepaths/flight.py
+-rw-r--r--   0 r         (1000) r         (1000)     4366 2023-02-03 02:30:26.000000 freepaths-1.4/freepaths/main_mfp_sampling.py
+-rw-r--r--   0 r         (1000) r         (1000)     3330 2023-05-11 07:20:52.000000 freepaths-1.4/freepaths/main_tracing.py
+-rw-r--r--   0 r         (1000) r         (1000)     8647 2023-01-25 08:49:48.000000 freepaths-1.4/freepaths/maps.py
+-rw-r--r--   0 r         (1000) r         (1000)     3797 2023-01-25 08:49:48.000000 freepaths-1.4/freepaths/materials.py
+-rw-r--r--   0 r         (1000) r         (1000)      733 2023-01-24 09:26:17.000000 freepaths-1.4/freepaths/move.py
+-rw-r--r--   0 r         (1000) r         (1000)      479 2023-05-25 02:30:36.000000 freepaths-1.4/freepaths/options.py
+-rw-r--r--   0 r         (1000) r         (1000)     4837 2023-01-25 08:49:48.000000 freepaths-1.4/freepaths/output_info.py
+-rw-r--r--   0 r         (1000) r         (1000)    15254 2023-05-25 02:30:34.000000 freepaths-1.4/freepaths/output_plots.py
+-rw-r--r--   0 r         (1000) r         (1000)     2348 2023-02-03 08:43:58.000000 freepaths-1.4/freepaths/output_structure.py
+-rw-r--r--   0 r         (1000) r         (1000)     8034 2023-05-25 02:30:40.000000 freepaths-1.4/freepaths/phonon.py
+-rw-r--r--   0 r         (1000) r         (1000)      580 2023-01-24 09:16:58.000000 freepaths-1.4/freepaths/progress.py
+-rw-r--r--   0 r         (1000) r         (1000)     2312 2023-05-25 02:30:38.000000 freepaths-1.4/freepaths/run_phonon.py
+-rw-r--r--   0 r         (1000) r         (1000)    28765 2023-05-25 05:20:49.000000 freepaths-1.4/freepaths/scattering.py
+-rw-r--r--   0 r         (1000) r         (1000)     1550 2023-01-25 08:51:17.000000 freepaths-1.4/freepaths/scattering_types.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-25 06:42:16.638523 freepaths-1.4/freepaths.egg-info/
+-rw-r--r--   0 r         (1000) r         (1000)     5298 2023-05-25 06:42:16.000000 freepaths-1.4/freepaths.egg-info/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)      702 2023-05-25 06:42:16.000000 freepaths-1.4/freepaths.egg-info/SOURCES.txt
+-rw-r--r--   0 r         (1000) r         (1000)        1 2023-05-25 06:42:16.000000 freepaths-1.4/freepaths.egg-info/dependency_links.txt
+-rw-r--r--   0 r         (1000) r         (1000)       53 2023-05-25 06:42:16.000000 freepaths-1.4/freepaths.egg-info/entry_points.txt
+-rw-r--r--   0 r         (1000) r         (1000)       31 2023-05-25 06:42:16.000000 freepaths-1.4/freepaths.egg-info/requires.txt
+-rw-r--r--   0 r         (1000) r         (1000)       10 2023-05-25 06:42:16.000000 freepaths-1.4/freepaths.egg-info/top_level.txt
+-rw-r--r--   0 r         (1000) r         (1000)       91 2022-11-27 00:35:48.000000 freepaths-1.4/pyproject.toml
+-rw-r--r--   0 r         (1000) r         (1000)       38 2023-05-25 06:42:16.638523 freepaths-1.4/setup.cfg
+-rw-r--r--   0 r         (1000) r         (1000)     1439 2023-02-03 05:40:49.000000 freepaths-1.4/setup.py
```

### Comparing `freepaths-1.3/PKG-INFO` & `freepaths-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freepaths
-Version: 1.3
+Version: 1.4
 Summary: Phonon Monte Carlo simulator
 Home-page: https://github.com/anufrievroman/freepaths
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `freepaths-1.3/README.md` & `freepaths-1.4/README.md`

 * *Files identical despite different names*

### Comparing `freepaths-1.3/freepaths/__main__.py` & `freepaths-1.4/freepaths/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """FreePATHS - Free Phonon and THermal Simulator"""
 
 import argparse
 
 import freepaths.main_tracing
 import freepaths.main_mfp_sampling
 
-__version__ = "1.3"
+__version__ = "1.4"
 
 # Parse user arguments:
 parser = argparse.ArgumentParser(
                 prog = 'FreePATHS',
                 description = 'Monte Carlo simulator',
                 epilog = 'For more information, visit: https://anufrievroman.gitbook.io/freepaths'
                 )
```

### Comparing `freepaths-1.3/freepaths/animation.py` & `freepaths-1.4/freepaths/animation.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.3/freepaths/config.py` & `freepaths-1.4/freepaths/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Module that reads the user input file, provides default values, and converts the variables into enums"""
 
 import sys
 import argparse
 
-from freepaths.options import Materials, Distributions, Positions
+from freepaths.options import Materials, Distributions
 
 # Import a default input file:
 from freepaths.default_config import *
 
 
 # Parse user arguments:
 WEBSITE = 'https://anufrievroman.gitbook.io/freepaths'
@@ -40,15 +40,15 @@
         self.temp = T
         self.plots_in_terminal = PLOTS_IN_TERMINAL
         self.output_scattering_map = OUTPUT_SCATTERING_MAP
         self.output_raw_thermal_map = OUTPUT_RAW_THERMAL_MAP
         self.output_trajectories_of_first = OUTPUT_TRAJECTORIES_OF_FIRST
         self.output_structure_color = OUTPUT_STRUCTURE_COLOR
         self.number_of_length_segments = NUMBER_OF_LENGTH_SEGMENTS
-        self.hot_side_angle_distribution = HOT_SIDE_ANGLE_DISTRIBUTION
+        self.phonon_source_angle_distribution = PHONON_SOURCE_ANGLE_DISTRIBUTION
 
         # Animation:
         self.output_path_animation = OUTPUT_PATH_ANIMATION
         self.output_animation_fps = OUTPUT_ANIMATION_FPS
 
         # Map & profiles parameters:
         self.number_of_pixels_x = NUMBER_OF_PIXELS_X
@@ -69,22 +69,31 @@
         self.width = WIDTH
         self.length = LENGTH
         self.include_right_sidewall = INCLUDE_RIGHT_SIDEWALL
         self.include_left_sidewall = INCLUDE_LEFT_SIDEWALL
         self.include_top_sidewall = INCLUDE_TOP_SIDEWALL
         self.include_bottom_sidewall = INCLUDE_BOTTOM_SIDEWALL
 
-        # Hot and cold sides:
+        # Hot side positions:
+        self.hot_side_position_top = HOT_SIDE_POSITION_TOP
+        self.hot_side_position_bottom = HOT_SIDE_POSITION_BOTTOM
+        self.hot_side_position_right = HOT_SIDE_POSITION_RIGHT
+        self.hot_side_position_left = HOT_SIDE_POSITION_LEFT
+
         self.frequency_detector_size = FREQUENCY_DETECTOR_SIZE
-        self.cold_side_position = COLD_SIDE_POSITION
-        self.hot_side_position = HOT_SIDE_POSITION
-        self.hot_side_x = HOT_SIDE_X
-        self.hot_side_y = HOT_SIDE_Y
-        self.hot_side_width_x = HOT_SIDE_WIDTH_X
-        self.hot_side_width_y = HOT_SIDE_WIDTH_Y
+        self.phonon_source_x = PHONON_SOURCE_X
+        self.phonon_source_y = PHONON_SOURCE_Y
+        self.phonon_source_width_x = PHONON_SOURCE_WIDTH_X
+        self.phonon_source_width_y = PHONON_SOURCE_WIDTH_Y
+
+        # Cold side positions:
+        self.cold_side_position_top = COLD_SIDE_POSITION_TOP
+        self.cold_side_position_bottom = COLD_SIDE_POSITION_BOTTOM
+        self.cold_side_position_right = COLD_SIDE_POSITION_RIGHT
+        self.cold_side_position_left = COLD_SIDE_POSITION_LEFT
 
         # Roughness:
         self.side_wall_roughness = SIDE_WALL_ROUGHNESS
         self.hole_roughness = HOLE_ROUGHNESS
         self.pillar_roughness = PILLAR_ROUGHNESS
         self.top_roughness = TOP_ROUGHNESS
         self.bottom_roughness = BOTTOM_ROUGHNESS
@@ -118,81 +127,110 @@
 
 
     def convert_to_enums(self):
         """Convert some user generated parameters into enums"""
 
         # Distributions:
         valid_distributions =[member.name.lower() for member in Distributions]
-        if self.hot_side_angle_distribution in valid_distributions:
-            self.hot_side_angle_distribution = Distributions[self.hot_side_angle_distribution.upper()]
+        if self.phonon_source_angle_distribution in valid_distributions:
+            self.phonon_source_angle_distribution = Distributions[self.phonon_source_angle_distribution.upper()]
         else:
-            print("ERROR: Parameter HOT_SIDE_ANGLE_DISTRIBUTION is not set correctly.")
-            print("HOT_SIDE_ANGLE_DISTRIBUTION should be one of the following:")
+            print("ERROR: Parameter phonon_source_ANGLE_DISTRIBUTION is not set correctly.")
+            print("phonon_source_ANGLE_DISTRIBUTION should be one of the following:")
             print(*valid_distributions, sep = ", ")
             sys.exit()
 
         # Materials:
         valid_materials = [member.name for member in Materials]
         if self.media in valid_materials:
             self.media = Materials[self.media]
         else:
             print(f"ERROR: Material {self.media} is not in the database.")
             print("MEDIA should be one of the following:")
             print(*valid_materials, sep = ", ")
             sys.exit()
 
-        # Positions:
-        valid_positions = [member.name.lower() for member in Positions]
-        if self.cold_side_position in valid_positions:
-            self.cold_side_position = Positions[self.cold_side_position.upper()]
-        else:
-            print("ERROR: Parameter COLD_SIDE_POSITION is not set correctly.")
-            print("COLD_SIDE_POSITION should be one of the following:")
-            print(*valid_positions, sep = ", ")
-            sys.exit()
-
-        if self.hot_side_position in valid_positions:
-            self.hot_side_position = Positions[self.hot_side_position.upper()]
-        else:
-            print("ERROR: Parameter HOT_SIDE_POSITION is not set correctly.")
-            print("HOT_SIDE_POSITION should be one of the following:")
-            print(*valid_positions, sep = ", ")
-            sys.exit()
-
 
     def check_parameter_validity(self):
         """Check if various parameters are valid"""
         if self.number_of_phonons < self.output_trajectories_of_first:
             self.output_trajectories_of_first = self.number_of_phonons
             print("WARNING: Parameter OUTPUT_TRAJECTORIES_OF_FIRST exceeded NUMBER_OF_PHONONS.\n")
 
-        if self.hot_side_y > self.length:
-            self.hot_side_y = self.length
-            print("WARNING: Parameter HOT_SIDE_Y exceeded LENGHT.\n")
-
-        if self.hot_side_y < 0:
-            self.hot_side_y = 0
-            print("WARNING: Parameter HOT_SIDE_Y was negative.\n")
-
-        if self.hot_side_y - self.hot_side_width_y / 2 < 0:
-            self.hot_side_width_y = self.hot_side_y * 2
-            print("WARNING: Parameter HOT_SIDE_WIDTH_Y was too large.\n")
-
-        if self.hot_side_x > self.width/2:
-            self.hot_side_x = 0
-            print("WARNING: Parameter HOT_SIDE_X was larger than WIDTH.\n")
-
-        if self.hot_side_width_x > self.width:
-            self.hot_side_width_x = self.width
-            print("WARNING: Parameter HOT_SIDE_WIDTH_X exceeds WIDTH.\n")
-
-        if self.cold_side_position == self.hot_side_position:
-            print(f"ERROR: Hot and cold sides are set at {self.cold_side_position}.")
-            sys.exit()
+        if self.phonon_source_y > self.length:
+            self.phonon_source_y = self.length
+            print("WARNING: Parameter phonon_source_Y exceeded LENGHT.\n")
+
+        if self.phonon_source_y < 0:
+            self.phonon_source_y = 0
+            print("WARNING: Parameter PHONON_SOURCE_Y was negative.\n")
+
+        if self.phonon_source_y - self.phonon_source_width_y / 2 < 0:
+            self.phonon_source_width_y = self.phonon_source_y * 2
+            print("WARNING: Parameter PHONON_SOURCE_WIDTH_Y was too large.\n")
+
+        if self.phonon_source_x > self.width/2:
+            self.phonon_source_x = 0
+            print("WARNING: Parameter PHONON_SOURCE_X was larger than WIDTH.\n")
+
+        if self.phonon_source_width_x > self.width:
+            self.phonon_source_width_x = self.width
+            print("WARNING: Parameter PHONON_SOURCE_WIDTH_X exceeds WIDTH.\n")
 
         if self.output_path_animation and self.number_of_timesteps > 5000:
             print("WARNING: NUMBER_OF_TIMESTEPS is rather large for animation.\n")
 
+        if (self.cold_side_position_top and self.include_top_sidewall or
+            self.hot_side_position_top and self.include_top_sidewall or
+            self.cold_side_position_top and self.hot_side_position_top):
+            print("ERROR: Top side is assigned multiple functions.\n")
+            sys.exit()
+
+        if (self.cold_side_position_bottom and self.include_bottom_sidewall or
+            self.hot_side_position_bottom and self.include_bottom_sidewall or
+            self.cold_side_position_bottom and self.hot_side_position_bottom):
+            print("ERROR: Bottom side is assigned multiple functions.\n")
+            sys.exit()
+
+        if (self.cold_side_position_right and self.include_right_sidewall or
+            self.hot_side_position_right and self.include_right_sidewall or
+            self.cold_side_position_right and self.hot_side_position_right):
+            print("ERROR: Right side is assigned multiple functions.\n")
+            sys.exit()
+
+        if (self.cold_side_position_left and self.include_left_sidewall or
+            self.hot_side_position_left and self.include_left_sidewall or
+            self.cold_side_position_left and self.hot_side_position_left):
+            print("ERROR: Left side is assigned multiple functions.\n")
+            sys.exit()
+
+
+    def check_depricated_parameters(self):
+        """Check for depricated parameters and warn about them"""
+
+        if 'COLD_SIDE_POSITION' in globals():
+            print("WARNING: parameter COLD_SIDE_POSITION is depricated. ")
+            print("Use specific boolean parameters like COLD_SIDE_POSITION_TOP = True.\n")
+
+        if 'HOT_SIDE_POSITION' in globals():
+            print("WARNING: parameter HOT_SIDE_POSITION is depricated. ")
+            print("Use specific boolean parameters like HOT_SIDE_POSITION_BOTTOM = True.\n")
+
+        if 'HOT_SIDE_X' in globals():
+            print("WARNING: parameter HOT_SIDE_X was renamed to PHONON_SOURCE_X.\n")
+
+        if 'HOT_SIDE_Y' in globals():
+            print("WARNING: parameter HOT_SIDE_Y was renamed to PHONON_SOURCE_Y.\n")
+
+        if 'HOT_SIDE_WIDTH_X' in globals():
+            print("WARNING: parameter HOT_SIDE_WIDTH_X was renamed to PHONON_SOURCE_WIDTH_X.\n")
+
+        if 'HOT_SIDE_WIDTH_Y' in globals():
+            print("WARNING: parameter HOT_SIDE_WIDTH_Y was renamed to PHONON_SOURCE_WIDTH_Y.\n")
+
+        if 'HOT_SIDE_ANGLE_DISTRIBUTION' in globals():
+            print("WARNING: parameter HOT_SIDE_ANGLE_DISTRIBUTION was renamed to PHONON_SOURCE_ANGLE_DISTRIBUTION.\n")
 
 cf = Config()
 cf.convert_to_enums()
 cf.check_parameter_validity()
+cf.check_depricated_parameters()
```

### Comparing `freepaths-1.3/freepaths/data.py` & `freepaths-1.4/freepaths/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,37 +89,40 @@
         self.hot_side = np.zeros(cf.number_of_length_segments+1)
         self.internal = np.zeros(cf.number_of_length_segments+1)
         self.total = np.zeros(cf.number_of_length_segments+1)
 
     def save_scattering_events(self, y, scattering_types):
         """Analyze types of scattering at the current timestep and add it to the statistics"""
 
-        # Calculate in which length segment (starting from zero) we are:
-        segment = int(y // (cf.length / cf.number_of_length_segments))
-        self.total[segment] += 1
-
-        # Scattering on side walls:
-        self.wall_diffuse[segment]  += 1 if scattering_types.walls == Scattering.DIFFUSE else 0
-        self.wall_specular[segment] += 1 if scattering_types.walls == Scattering.SPECULAR else 0
-
-        # Scattering on top and bottom:
-        self.top_diffuse[segment]  += 1 if scattering_types.top_bottom == Scattering.DIFFUSE else 0
-        self.top_specular[segment] += 1 if scattering_types.top_bottom == Scattering.SPECULAR else 0
-
-        # Scattering on holes:
-        self.hole_diffuse[segment]  += 1 if scattering_types.holes == Scattering.DIFFUSE else 0
-        self.hole_specular[segment] += 1 if scattering_types.holes == Scattering.SPECULAR else 0
-
-        # Scattering on pillars:
-        self.pillar_diffuse[segment]  += 1 if scattering_types.pillars == Scattering.DIFFUSE else 0
-        self.pillar_specular[segment] += 1 if scattering_types.pillars == Scattering.SPECULAR else 0
-
-        # Internal scattering and rethermalization on hot side:
-        self.hot_side[segment] += 1 if scattering_types.hot_side == Scattering.DIFFUSE else 0
-        self.internal[segment] += 1 if scattering_types.internal == Scattering.DIFFUSE else 0
+        try:
+            # Calculate in which length segment (starting from zero) we are:
+            segment = int(y // (cf.length / cf.number_of_length_segments))
+            self.total[segment] += 1
+
+            # Scattering on side walls:
+            self.wall_diffuse[segment]  += 1 if scattering_types.walls == Scattering.DIFFUSE else 0
+            self.wall_specular[segment] += 1 if scattering_types.walls == Scattering.SPECULAR else 0
+
+            # Scattering on top and bottom:
+            self.top_diffuse[segment]  += 1 if scattering_types.top_bottom == Scattering.DIFFUSE else 0
+            self.top_specular[segment] += 1 if scattering_types.top_bottom == Scattering.SPECULAR else 0
+
+            # Scattering on holes:
+            self.hole_diffuse[segment]  += 1 if scattering_types.holes == Scattering.DIFFUSE else 0
+            self.hole_specular[segment] += 1 if scattering_types.holes == Scattering.SPECULAR else 0
+
+            # Scattering on pillars:
+            self.pillar_diffuse[segment]  += 1 if scattering_types.pillars == Scattering.DIFFUSE else 0
+            self.pillar_specular[segment] += 1 if scattering_types.pillars == Scattering.SPECULAR else 0
+
+            # Internal scattering and rethermalization on hot side:
+            self.hot_side[segment] += 1 if scattering_types.hot_side == Scattering.DIFFUSE else 0
+            self.internal[segment] += 1 if scattering_types.internal == Scattering.DIFFUSE else 0
+        except:
+            pass
 
     def write_into_files(self):
         """Write data into a file"""
         filename = "Data/Scattering events statistics.csv"
         data = np.vstack((self.wall_diffuse, self.wall_specular, self.top_diffuse, self.top_specular, self.hole_diffuse,
                         self.hole_specular, self.hot_side, self.internal, self.pillar_diffuse, self.pillar_specular)).T
         header1 = "Sidewalls diffuse, Sidewalls specular, Top & bottom diffuse, Top & bottom specular, "
```

### Comparing `freepaths-1.3/freepaths/flight.py` & `freepaths-1.4/freepaths/flight.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.3/freepaths/main_mfp_sampling.py` & `freepaths-1.4/freepaths/main_mfp_sampling.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.3/freepaths/main_tracing.py` & `freepaths-1.4/freepaths/main_tracing.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.3/freepaths/maps.py` & `freepaths-1.4/freepaths/maps.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.3/freepaths/materials.py` & `freepaths-1.4/freepaths/materials.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.3/freepaths/move.py` & `freepaths-1.4/freepaths/move.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.3/freepaths/output_info.py` & `freepaths-1.4/freepaths/output_info.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.3/freepaths/output_plots.py` & `freepaths-1.4/freepaths/output_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,29 +243,31 @@
     for patch in patches:
         ax.add_patch(patch)
 
     # Draw paths:
     for index in range(cf.output_trajectories_of_first):
         x_coordinates = np.trim_zeros(data[:, 3 * index], trim='b')
         y_coordinates = np.trim_zeros(data[:, 3 * index + 1], trim='b')
-        ax.plot(x_coordinates, y_coordinates, linewidth=0.2)
+        max_steps = min([x_coordinates.shape[0], y_coordinates.shape[0]])
+        ax.plot(x_coordinates[:max_steps], y_coordinates[:max_steps], linewidth=0.2)
 
     # Set labels:
     ax.set_xlabel('X (μm)', fontsize=12)
     ax.set_ylabel('Y (μm)', fontsize=12)
     ax.set_aspect('equal', 'datalim')
     fig.savefig("Phonon paths XY.pdf", dpi=600, format='pdf', bbox_inches="tight")
     if cf.plots_in_terminal: plt.show()
 
     # Create YZ plot:
     fig, ax = plt.subplots()
     for index in range(cf.output_trajectories_of_first):
         y_coordinates = np.trim_zeros(data[:, 3 * index + 1], trim='b')
         z_coordinates = np.trim_zeros(data[:, 3 * index + 2], trim='b')
-        ax.plot(y_coordinates, z_coordinates, linewidth=0.2)
+        max_steps = min([y_coordinates.shape[0], z_coordinates.shape[0]])
+        ax.plot(y_coordinates[:max_steps], z_coordinates[:max_steps], linewidth=0.2)
     ax.set_xlabel('Y (μm)', fontsize=12)
     ax.set_ylabel('Z (μm)', fontsize=12)
     ax.set_aspect('equal', 'datalim')
     fig.savefig("Phonon paths YZ.pdf", dpi=300, format='pdf', bbox_inches="tight")
     if cf.plots_in_terminal: plt.show()
```

### Comparing `freepaths-1.3/freepaths/output_structure.py` & `freepaths-1.4/freepaths/output_structure.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.3/freepaths/phonon.py` & `freepaths-1.4/freepaths/phonon.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from random import random, choice
 from numpy import sign
 from scipy.constants import k, hbar
 import numpy as np
 import enum
 
 from freepaths.config import cf
-from freepaths.options import Distributions, Materials, Positions, Polarizations
+from freepaths.options import Distributions, Materials, Polarizations
 import freepaths.move
 
 
 class Phonon:
     """A phonon particle with various physical properties"""
 
     def __init__(self, material, polarization=None, phonon_number=None):
@@ -43,64 +43,56 @@
     def wavelength(self):
         """Calculate wavelength of the phonon"""
         return self.speed/self.f
 
     @property
     def is_in_system(self):
         """Checks if the phonon at this timestep did not reach the cold side.
-        Depending on where we set the cold side, we check if phonon crossed that line"""
-        small_offset = 10e-9
-        if cf.cold_side_position == Positions.TOP:
-            return self.y < cf.length
-        if cf.cold_side_position == Positions.BOTTOM:
-            return self.y > 0
-        if cf.cold_side_position == Positions.RIGHT:
-            # return (self.y < cf.length - 1.1e-6) or (self.y > cf.length - 1.1e-6 and self.x < cf.width / 2.0 - small_offset)
-            return self.x < cf.width / 2.0
-        if cf.cold_side_position == Positions.LEFT:
-            # return (self.y < cf.length - 1.1e-6) or (self.y > cf.length - 1.1e-6 and self.x < cf.width / 2.0 - small_offset)
-            return self.x > - cf.width / 2.0
-        # if cf.cold_side_position == Positions.TOP_AND_RIGHT:
-            # return (self.y < 1.0e-6) or (1.0e-6 < self.y < cf.length and self.x < cf.width / 2.0 - small_offset)
-        # if cf.cold_side_position == Positions.TOP_AND_BOTTOM:
-            # return cf.length > self.y > 0
-        raise ValueError('Specified "cold_side" is not valid. Only TOP, RIGHT, TOP_AND_RIGH, TOP_AND_BOTTOM')
+        Depending on where user set cold sides, we check if phonon crossed that line"""
+        is_inside_top = self.y < cf.length
+        is_inside_bottom = self.y > 0
+        is_inside_right = self.x < cf.width / 2.0
+        is_inside_left = self.x > - cf.width / 2.0
+        return ((not cf.cold_side_position_top or is_inside_top) and
+                (not cf.cold_side_position_bottom or is_inside_bottom) and
+                (not cf.cold_side_position_right or is_inside_right) and
+                (not cf.cold_side_position_left or is_inside_left))
 
     def assign_polarization(self):
         """Assign branch of phonon dispersion"""
         self.polarization = choice([Polarizations.TA, Polarizations.TA, Polarizations.LA])
 
     def assign_coordinates(self):
         """Assign initial coordinates at the hot side"""
-        self.x = cf.hot_side_x + 0.49 * cf.hot_side_width_x * (2 * random() - 1)
-        self.y = cf.hot_side_y + 0.49 * cf.hot_side_width_y * (2 * random() - 1)
+        self.x = cf.phonon_source_x + 0.49 * cf.phonon_source_width_x * (2 * random() - 1)
+        self.y = cf.phonon_source_y + 0.49 * cf.phonon_source_width_y * (2 * random() - 1)
         self.z = 0.49 * cf.thickness * (2 * random() - 1)
 
     def assign_angles(self):
         """Depending on angle distribution, assign angles"""
-        if cf.hot_side_angle_distribution == Distributions.RANDOM_UP:
+        if cf.phonon_source_angle_distribution == Distributions.RANDOM_UP:
             self.theta = -pi/2 + pi*random()
             self.phi = asin(2*random() - 1)
-        if cf.hot_side_angle_distribution == Distributions.RANDOM_DOWN:
+        if cf.phonon_source_angle_distribution == Distributions.RANDOM_DOWN:
             rand_sign = sign((2*random() - 1))
             self.theta = rand_sign*(pi/2 + pi/2*random())
             self.phi = asin(2*random() - 1)
-        if cf.hot_side_angle_distribution == Distributions.RANDOM_RIGHT:
+        if cf.phonon_source_angle_distribution == Distributions.RANDOM_RIGHT:
             self.theta = pi*random()
             self.phi = asin(2*random() - 1)
-        if cf.hot_side_angle_distribution == Distributions.RANDOM_LEFT:
+        if cf.phonon_source_angle_distribution == Distributions.RANDOM_LEFT:
             self.theta = - pi*random()
             self.phi = asin(2*random() - 1)
-        if cf.hot_side_angle_distribution == Distributions.DIRECTIONAL:
+        if cf.phonon_source_angle_distribution == Distributions.DIRECTIONAL:
             self.theta = 0
             self.phi = -pi/2 + pi*random()
-        if cf.hot_side_angle_distribution == Distributions.LAMBERT:
+        if cf.phonon_source_angle_distribution == Distributions.LAMBERT:
             self.theta = asin(2*random() - 1)
             self.phi = asin((asin(2*random() - 1))/(pi/2))
-        if cf.hot_side_angle_distribution == Distributions.UNIFORM:
+        if cf.phonon_source_angle_distribution == Distributions.UNIFORM:
             self.theta = -pi + 2*pi*random()
             self.phi = asin(2*random() - 1)
 
     def assign_frequency(self, material):
         """Assigning frequency with probability according to Planckian distribution"""
 
         # Frequency of the peak of the Plank distribution:
```

### Comparing `freepaths-1.3/freepaths/progress.py` & `freepaths-1.4/freepaths/progress.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.3/freepaths/run_phonon.py` & `freepaths-1.4/freepaths/run_phonon.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.3/freepaths/scattering.py` & `freepaths-1.4/freepaths/scattering.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from math import pi, cos, sin, tan, exp, sqrt, atan, asin, acos
 from random import random
 from numpy import sign
 
 from freepaths.config import cf
 from freepaths.move import move
 from freepaths.scattering_types import Scattering
-from freepaths.options import Positions
 
 
 def specularity(angle, roughness, wavelength):
     """Calculate probability of specular scattering with Soffer's equation"""
     return exp(-16 * pi**2 * roughness**2 * ((cos(angle))**2) / wavelength**2)
 
 
@@ -24,23 +23,60 @@
         scattering_types.internal = Scattering.DIFFUSE
 
 
 def reinitialization(ph, scattering_types):
     """Re-thermalize phonon if it comes back to the hot side"""
     x, y, _ = move(ph, cf.timestep)
 
-    # If phonon returns to the hot side, generate it again:
-    if (
-        (cf.hot_side_position == Positions.BOTTOM and y < 0) or
-        (cf.hot_side_position == Positions.TOP and y > cf.length) or
-        (cf.hot_side_position == Positions.RIGHT and x > cf.width/2) or
-        (cf.hot_side_position == Positions.LEFT and x < -cf.width/2)
-        ):
-        ph.assign_angles()
+    # Bottom sidewall:
+    if cf.hot_side_position_bottom and y < 0:
         scattering_types.hot_side = Scattering.DIFFUSE
+        attempt = 0
+        while attempt < 10:
+            attempt += 1
+
+            # Lambert cosine distribution:
+            ph.theta = asin(2*random() - 1)
+            ph.phi = asin((asin(2*random() - 1))/(pi/2))
+
+            # Accept the angles only if they do not immediately cause new scattering:
+            if no_new_scattering(ph):
+                break
+
+    # Top sidewall:
+    if cf.hot_side_position_top and y > cf.length:
+        scattering_types.hot_side = Scattering.DIFFUSE
+        attempt = 0
+        while attempt < 10:
+            attempt += 1
+
+            # Lambert cosine distribution:
+            rand_sign = sign((2*random() - 1))
+            ph.theta = rand_sign*pi/2 + rand_sign*acos(random())
+            ph.phi = asin((asin(2*random() - 1))/(pi/2))
+
+            # Accept the angles only if they do not immediately cause new scattering:
+            if no_new_scattering(ph):
+                break
+
+    # Right and left sidewalls:
+    if ((cf.hot_side_position_right and x > cf.width/2) or
+          (cf.hot_side_position_left and x < -cf.width/2)):
+        scattering_types.hot_side = Scattering.DIFFUSE
+        attempt = 0
+        while attempt < 10:
+            attempt += 1
+
+            # Lambert cosine distribution:
+            ph.theta = -sign(x)*pi/2 + asin(2*random() - 1)
+            ph.phi = asin((asin(2*random() - 1))/(pi/2))
+
+            # Accept the angles if they do not cause new scattering:
+            if no_new_scattering(ph):
+                break
 
 
 def top_parabola_scattering(ph, scattering_types):
     """Scattering on top parabolic boundary"""
     x, y, z = move(ph, cf.timestep)
 
     # If phonon is beyond the parabola:
@@ -363,15 +399,17 @@
                 scattering_types.holes = Scattering.DIFFUSE
 
 
 def no_new_scattering(ph):
     """Check if new angles do not immediately lead to new top/bottom or sidewall scattering.
     This is necessary to prevent phonons leaving the structure boundaries."""
     x, y, z = move(ph, cf.timestep)
-    return True if (abs(z) < cf.thickness / 2 and abs(x) < cf.width / 2 and y > 0) else False
+    return (abs(z) < cf.thickness / 2 and
+            abs(x) < cf.width / 2 and
+            cf.length > y > 0)
 
 
 def scattering_on_right_sidewall(ph, scattering_types):
     """Check if the phonon hits right side wall and output new vector"""
     x, y, z = move(ph, cf.timestep)
 
     # If phonon is beyond the side wall:
```

### Comparing `freepaths-1.3/freepaths/scattering_types.py` & `freepaths-1.4/freepaths/scattering_types.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.3/freepaths.egg-info/PKG-INFO` & `freepaths-1.4/freepaths.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freepaths
-Version: 1.3
+Version: 1.4
 Summary: Phonon Monte Carlo simulator
 Home-page: https://github.com/anufrievroman/freepaths
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `freepaths-1.3/freepaths.egg-info/SOURCES.txt` & `freepaths-1.4/freepaths.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freepaths-1.3/setup.py` & `freepaths-1.4/setup.py`

 * *Files identical despite different names*

