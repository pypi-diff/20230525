# Comparing `tmp/grid2fp-0.0.1.tar.gz` & `tmp/grid2fp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grid2fp-0.0.1.tar", last modified: Thu May 25 04:10:46 2023, max compression
+gzip compressed data, was "grid2fp-0.0.2.tar", last modified: Thu May 25 15:52:18 2023, max compression
```

## Comparing `grid2fp-0.0.1.tar` & `grid2fp-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 04:10:46.051571 grid2fp-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 04:10:18.000000 grid2fp-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-25 04:10:46.051571 grid2fp-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-25 04:10:18.000000 grid2fp-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 04:10:46.047571 grid2fp-0.0.1/grid2fp/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 04:10:18.000000 grid2fp-0.0.1/grid2fp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-25 04:10:18.000000 grid2fp-0.0.1/grid2fp/grid2fp.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-25 04:10:18.000000 grid2fp-0.0.1/grid2fp/grid_segment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 04:10:46.051571 grid2fp-0.0.1/grid2fp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-25 04:10:46.000000 grid2fp-0.0.1/grid2fp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-25 04:10:46.000000 grid2fp-0.0.1/grid2fp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 04:10:46.000000 grid2fp-0.0.1/grid2fp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 04:10:46.000000 grid2fp-0.0.1/grid2fp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 04:10:46.000000 grid2fp-0.0.1/grid2fp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 04:10:46.051571 grid2fp-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-25 04:10:18.000000 grid2fp-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 04:10:46.051571 grid2fp-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 04:10:18.000000 grid2fp-0.0.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-25 04:10:18.000000 grid2fp-0.0.1/test/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:52:18.668267 grid2fp-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 15:51:53.000000 grid2fp-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-25 15:52:18.668267 grid2fp-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-25 15:51:53.000000 grid2fp-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:52:18.664267 grid2fp-0.0.2/grid2fp/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 15:51:53.000000 grid2fp-0.0.2/grid2fp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-25 15:51:53.000000 grid2fp-0.0.2/grid2fp/grid2fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-25 15:51:53.000000 grid2fp-0.0.2/grid2fp/grid_segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:52:18.668267 grid2fp-0.0.2/grid2fp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-25 15:52:18.000000 grid2fp-0.0.2/grid2fp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-25 15:52:18.000000 grid2fp-0.0.2/grid2fp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:52:18.000000 grid2fp-0.0.2/grid2fp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 15:52:18.000000 grid2fp-0.0.2/grid2fp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 15:52:18.000000 grid2fp-0.0.2/grid2fp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:52:18.668267 grid2fp-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-25 15:51:53.000000 grid2fp-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:52:18.668267 grid2fp-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 15:51:53.000000 grid2fp-0.0.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-25 15:51:53.000000 grid2fp-0.0.2/test/test_integration.py
```

### Comparing `grid2fp-0.0.1/LICENSE` & `grid2fp-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grid2fp-0.0.1/grid2fp/grid2fp.py` & `grid2fp-0.0.2/grid2fp/grid2fp.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,30 @@
 import csv
 from grid2fp.grid_segment import grid_segment
 
 
 class grid2fp:
     """The grid2fp class."""
 
-    def __init__(self, csv_file=None, diagram=None, eccentricity=0.9, scale=10) -> None:
+    def __init__(
+        self, csv_file=None, diagram=None, eccentricity=0.9, scale=10, out_file=None
+    ) -> None:
         """Init for the grid2fp object.
 
         Parameters
         ----------
         csv_file : str, optional
             The location of grid diagram as csv, by default None
-        diagram : _type_, optional
+        diagram : array, optional
             A grid diagram, by default None
         eccentricity : float, optional
             How far away to place the
             Bézier controls, by default 0.9
+        out_file : str
+            The output file, by default None
         """
         self.diagram = []
         if csv_file is None and diagram is None:
             raise Exception("You need a csv file or a diagram")
 
         if csv_file:
             with open(csv_file) as csvfile:
@@ -38,14 +42,17 @@
 
         if diagram:
             self.diagram = diagram
         self.eccentricity = eccentricity
         self.scale = scale
         self.segments = []
         self.__get_segments()
+        if out_file:
+            d = self.draw()
+            d.save_svg(out_file)
 
     def __rotate(self, x, y):
         """Do a 45 degree rotation of the point.
 
         Parameters
         ----------
         x : int
@@ -134,26 +141,29 @@
         x_ctr1 = step.source[0] + (self.eccentricity * delta_x)
         x_ctr2 = step.sink[0] - (self.eccentricity * delta_x)
         y_ctr1 = step.source[1]
         y_ctr2 = step.sink[1]
         p.C(x_ctr1, y_ctr1, x_ctr2, y_ctr2, step.sink[0], step.sink[1])
         return p
 
-    def draw(self, file, pixel_scale=2):
+    def draw(self, pixel_scale=2):
         """Draws the front projection of the given grid as an SVG.
 
         Parameters
         ----------
-        file : str
-            The output file
         pixel_scale : int, optional
             The scaling for pixel features, by default 2
         scale : int
             The scale factor for the file
 
+        Returns
+        -------
+        Drawing
+            The svg for the grid diagram.
+
         """
         try:
             d = draw.Drawing(
                 self.scale * len(self.diagram[0]),
                 self.scale * math.sqrt(2) * len(self.diagram[0]),
                 origin=(0, 0),
                 id_prefix="d",
@@ -166,12 +176,12 @@
             )
             for step in self.segments:
                 p = self.__draw_segment(step)
                 g.append(p)
             d.append(g)
 
             d.set_pixel_scale(pixel_scale)
-            d.save_svg(file)
+            return d
         except Exception as err:
             print(
                 f"Unexpected {err=}, {type(err)=}, this is probably because the grid diagram is broken in some way."
             )
```

### Comparing `grid2fp-0.0.1/setup.py` & `grid2fp-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import logging
 
 logger = logging.getLogger(__name__)
 
-version = "0.0.1"
+version = "0.0.2"
 
 try:
     with open("README.md", "r") as f:
         long_desc = f.read()
 except:
     logger.warning("Could not open README.md.  long_description will be set to None.")
     long_desc = None
```

### Comparing `grid2fp-0.0.1/test/test_integration.py` & `grid2fp-0.0.2/test/test_integration.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 from pathlib import Path
 
 file_location = Path(os.path.dirname(__file__))
 
 
 def test_un():
     """TODO: Update Testcase description."""
-    g = grid2fp(csv_file=file_location / "un.csv")
-    g.draw(file_location / "un.svg")
+    grid2fp(csv_file=file_location / "un.csv", out_file=file_location / "un.svg")
     assert 1 == 1
 
 
 def test_random():
     """TODO: Update Testcase description."""
     g = grid2fp(csv_file=file_location / "random.csv")
-    g.draw(file_location / "random.svg")
+    d = g.draw()
+    d.save_svg(file_location / "random.svg")
     assert 1 == 1
 
 
 def test_trefoil():
     g = grid2fp(csv_file=file_location / "trefoil.csv")
-    g.draw(file_location / "trefoil.svg")
+    d = g.draw()
+    d.save_svg(file_location / "trefoil.svg")
     assert 1 == 1
```

