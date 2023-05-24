# Comparing `tmp/meow-sim-0.3.2.tar.gz` & `tmp/meow-sim-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.3.2.tar", last modified: Tue May 23 17:35:13 2023, max compression
+gzip compressed data, was "meow-sim-0.3.3.tar", last modified: Wed May 24 05:39:20 2023, max compression
```

## Comparing `meow-sim-0.3.2.tar` & `meow-sim-0.3.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:35:13.275930 meow-sim-0.3.2/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-05-23 17:35:07.000000 meow-sim-0.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3178 2023-05-23 17:35:13.271930 meow-sim-0.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2060 2023-05-23 17:35:07.000000 meow-sim-0.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:35:13.263930 meow-sim-0.3.2/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-05-23 17:35:07.000000 meow-sim-0.3.2/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:35:13.267930 meow-sim-0.3.2/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-05-23 17:35:07.000000 meow-sim-0.3.2/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-05-23 17:35:07.000000 meow-sim-0.3.2/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8007 2023-05-23 17:35:07.000000 meow-sim-0.3.2/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-05-23 17:35:07.000000 meow-sim-0.3.2/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-05-23 17:35:07.000000 meow-sim-0.3.2/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2783 2023-05-23 17:35:07.000000 meow-sim-0.3.2/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:35:13.267930 meow-sim-0.3.2/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-05-23 17:35:07.000000 meow-sim-0.3.2/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4600 2023-05-23 17:35:07.000000 meow-sim-0.3.2/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3316 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:35:13.267930 meow-sim-0.3.2/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3440 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     2734 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2052 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)     9211 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      944 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10785 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3564 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)     9814 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     2787 2023-05-23 17:35:08.000000 meow-sim-0.3.2/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:35:13.271930 meow-sim-0.3.2/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3178 2023-05-23 17:35:13.000000 meow-sim-0.3.2/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      657 2023-05-23 17:35:13.000000 meow-sim-0.3.2/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 17:35:13.000000 meow-sim-0.3.2/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      385 2023-05-23 17:35:13.000000 meow-sim-0.3.2/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-23 17:35:13.000000 meow-sim-0.3.2/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1874 2023-05-23 17:35:08.000000 meow-sim-0.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 17:35:13.275930 meow-sim-0.3.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:35:13.271930 meow-sim-0.3.2/tests/
--rw-r--r--   0 root         (0) root         (0)     4009 2023-05-23 17:35:08.000000 meow-sim-0.3.2/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-05-23 17:35:08.000000 meow-sim-0.3.2/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 05:39:20.089592 meow-sim-0.3.3/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-05-24 05:39:15.000000 meow-sim-0.3.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3178 2023-05-24 05:39:20.089592 meow-sim-0.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-05-24 05:39:15.000000 meow-sim-0.3.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 05:39:20.085592 meow-sim-0.3.3/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 05:39:20.089592 meow-sim-0.3.3/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8007 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4818 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 05:39:20.089592 meow-sim-0.3.3/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4600 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3316 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 05:39:20.089592 meow-sim-0.3.3/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3440 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10197 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      944 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10785 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3564 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)     9814 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-05-24 05:39:15.000000 meow-sim-0.3.3/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 05:39:20.089592 meow-sim-0.3.3/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3178 2023-05-24 05:39:20.000000 meow-sim-0.3.3/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      657 2023-05-24 05:39:20.000000 meow-sim-0.3.3/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 05:39:20.000000 meow-sim-0.3.3/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      385 2023-05-24 05:39:20.000000 meow-sim-0.3.3/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-24 05:39:20.000000 meow-sim-0.3.3/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-05-24 05:39:15.000000 meow-sim-0.3.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 05:39:20.089592 meow-sim-0.3.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 05:39:20.089592 meow-sim-0.3.3/tests/
+-rw-r--r--   0 root         (0) root         (0)     4009 2023-05-24 05:39:15.000000 meow-sim-0.3.3/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-05-24 05:39:15.000000 meow-sim-0.3.3/tests/test_nbs.py
```

### Comparing `meow-sim-0.3.2/LICENSE` & `meow-sim-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/PKG-INFO` & `meow-sim-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.3.2
+Version: 0.3.3
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.3.2/README.md` & `meow-sim-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow/__init__.py` & `meow-sim-0.3.3/meow/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.3.2"
+__version__ = "0.3.3"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.3.2/meow/assets/silicon.csv` & `meow-sim-0.3.3/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow/assets/silicon_oxide.csv` & `meow-sim-0.3.3/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow/base_model.py` & `meow-sim-0.3.3/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow/cache.py` & `meow-sim-0.3.3/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow/cell.py` & `meow-sim-0.3.3/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow/cross_section.py` & `meow-sim-0.3.3/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow/eme/__init__.py` & `meow-sim-0.3.3/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow/eme/common.py` & `meow-sim-0.3.3/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow/eme/sax.py` & `meow-sim-0.3.3/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow/environment.py` & `meow-sim-0.3.3/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow/fde/lumerical.py` & `meow-sim-0.3.3/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow/fde/tidy3d.py` & `meow-sim-0.3.3/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow/gds_structures.py` & `meow-sim-0.3.3/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow/geometries.py` & `meow-sim-0.3.3/meow/geometries.py`

 * *Files 10% similar despite different names*

```diff
@@ -146,33 +146,55 @@
     def _mask2d_single(self, X, Y, z):
         poly = sg.Polygon(self.poly)
         if self.axis == "x":
             # x, y, z -> y, z, x
             y_min, _ = self.poly.min(0)
             y_max, _ = self.poly.max(0)
             line = sg.LineString([(y_min, z), (y_max, z)])
-            intersection = np.asarray(poly.intersection(line).coords)
-            if not intersection.shape[0]:
-                return np.zeros_like(X, dtype=bool)
-            (y_min, _), (y_max, _) = intersection
-            y_min, y_max = min(y_min, y_max), max(y_min, y_max)
-            x_min, x_max = min(self.h_min, self.h_max), max(self.h_min, self.h_max)
-            return (x_min <= X) & (X <= x_max) & (y_min <= Y) & (Y <= y_max)
+            intersections = np.asarray(poly.intersection(line).coords)
+
+            if not isinstance(intersections, sg.MultiLineString):
+                intersection_array = np.asarray(intersections.coords)
+                if not intersection_array.shape[0]:
+                    return np.zeros_like(Y, dtype=bool)
+                intersections = sg.MultiLineString([intersections])
+
+            mask = np.zeros_like(Y, dtype=bool)
+            for intersection in intersections.geoms:
+                intersection = np.asarray(intersection.coords)
+                if not intersection.shape[0]:
+                    return np.zeros_like(X, dtype=bool)
+                (y_min, _), (y_max, _) = intersection
+                y_min, y_max = min(y_min, y_max), max(y_min, y_max)
+                x_min, x_max = min(self.h_min, self.h_max), max(self.h_min, self.h_max)
+                return (x_min <= X) & (X <= x_max) & (y_min <= Y) & (Y <= y_max)
+
         elif self.axis == "y":
             # x, y, z -> z, x, y
             _, x_min = self.poly.min(0)
             _, x_max = self.poly.max(0)
             line = sg.LineString([(z, x_min), (z, x_max)])
-            intersection = np.asarray(poly.intersection(line).coords)
-            if not intersection.shape[0]:
-                return np.zeros_like(X, dtype=bool)
-            (_, x_min), (_, x_max) = intersection
-            x_min, x_max = min(x_min, x_max), max(x_min, x_max)
-            y_min, y_max = min(self.h_min, self.h_max), max(self.h_min, self.h_max)
-            return (x_min <= X) & (X <= x_max) & (y_min <= Y) & (Y <= y_max)
+            intersections = poly.intersection(line)
+
+            if not isinstance(intersections, sg.MultiLineString):
+                intersection_array = np.asarray(intersections.coords)
+                if not intersection_array.shape[0]:
+                    return np.zeros_like(Y, dtype=bool)
+                intersections = sg.MultiLineString([intersections])
+
+            mask = np.zeros_like(Y, dtype=bool)
+            for intersection in intersections.geoms:
+                intersection = np.asarray(intersection.coords)
+                if not intersection.shape[0]:
+                    continue
+                (_, x_min), (_, x_max) = intersection
+                x_min, x_max = min(x_min, x_max), max(x_min, x_max)
+                y_min, y_max = min(self.h_min, self.h_max), max(self.h_min, self.h_max)
+                mask |= (x_min <= X) & (X <= x_max) & (y_min <= Y) & (Y <= y_max)
+            return mask
         else:
             # x, y, z -> x, y, z
             if (z < self.h_min) or (self.h_max < z):
                 return np.zeros_like(X, dtype=bool)
             return np.asarray(
                 [poly.contains(sg.Point(x, y)) for x, y in zip(X.ravel(), Y.ravel())],
                 dtype=bool,
```

### Comparing `meow-sim-0.3.2/meow/integrate.py` & `meow-sim-0.3.3/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow/materials.py` & `meow-sim-0.3.3/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow/mesh.py` & `meow-sim-0.3.3/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow/mode.py` & `meow-sim-0.3.3/meow/mode.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow/structures.py` & `meow-sim-0.3.3/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow/visualize.py` & `meow-sim-0.3.3/meow/visualize.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.3.3/meow_sim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.3.2
+Version: 0.3.3
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.3.2/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.3.3/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/pyproject.toml` & `meow-sim-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.3.2/tests/test_deserialization.py` & `meow-sim-0.3.3/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.2/tests/test_nbs.py` & `meow-sim-0.3.3/tests/test_nbs.py`

 * *Files identical despite different names*

