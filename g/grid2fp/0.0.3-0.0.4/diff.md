# Comparing `tmp/grid2fp-0.0.3.tar.gz` & `tmp/grid2fp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grid2fp-0.0.3.tar", last modified: Thu May 25 19:17:08 2023, max compression
+gzip compressed data, was "grid2fp-0.0.4.tar", last modified: Thu May 25 20:19:04 2023, max compression
```

## Comparing `grid2fp-0.0.3.tar` & `grid2fp-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:17:08.956801 grid2fp-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 19:16:41.000000 grid2fp-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-25 19:17:08.956801 grid2fp-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-25 19:16:41.000000 grid2fp-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:17:08.956801 grid2fp-0.0.3/grid2fp/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 19:16:41.000000 grid2fp-0.0.3/grid2fp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-25 19:16:41.000000 grid2fp-0.0.3/grid2fp/grid2fp.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-25 19:16:41.000000 grid2fp-0.0.3/grid2fp/grid_segment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:17:08.956801 grid2fp-0.0.3/grid2fp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-25 19:17:08.000000 grid2fp-0.0.3/grid2fp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-25 19:17:08.000000 grid2fp-0.0.3/grid2fp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:17:08.000000 grid2fp-0.0.3/grid2fp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 19:17:08.000000 grid2fp-0.0.3/grid2fp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 19:17:08.000000 grid2fp-0.0.3/grid2fp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 19:17:08.956801 grid2fp-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-25 19:16:41.000000 grid2fp-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:17:08.956801 grid2fp-0.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 19:16:41.000000 grid2fp-0.0.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-25 19:16:41.000000 grid2fp-0.0.3/test/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:19:04.602119 grid2fp-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 20:18:33.000000 grid2fp-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-25 20:19:04.602119 grid2fp-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-25 20:18:33.000000 grid2fp-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:19:04.602119 grid2fp-0.0.4/grid2fp/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 20:18:33.000000 grid2fp-0.0.4/grid2fp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-25 20:18:33.000000 grid2fp-0.0.4/grid2fp/grid2fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-25 20:18:33.000000 grid2fp-0.0.4/grid2fp/grid_segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:19:04.602119 grid2fp-0.0.4/grid2fp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-25 20:19:04.000000 grid2fp-0.0.4/grid2fp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-25 20:19:04.000000 grid2fp-0.0.4/grid2fp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:19:04.000000 grid2fp-0.0.4/grid2fp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 20:19:04.000000 grid2fp-0.0.4/grid2fp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 20:19:04.000000 grid2fp-0.0.4/grid2fp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 20:19:04.602119 grid2fp-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-25 20:18:33.000000 grid2fp-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:19:04.602119 grid2fp-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 20:18:33.000000 grid2fp-0.0.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-25 20:18:33.000000 grid2fp-0.0.4/test/test_integration.py
```

### Comparing `grid2fp-0.0.3/LICENSE` & `grid2fp-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `grid2fp-0.0.3/PKG-INFO` & `grid2fp-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grid2fp
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tool to eat grid diagrams and generate its front projection.
 Home-page: https://github.com/Joecstarr/grid2fp
 Author: Casey Duckering
 Keywords: topology,Legendrian,Grid Diagram,knot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `grid2fp-0.0.3/README.md` & `grid2fp-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `grid2fp-0.0.3/grid2fp/grid2fp.py` & `grid2fp-0.0.4/grid2fp/grid2fp.py`

 * *Files 9% similar despite different names*

```diff
@@ -80,48 +80,50 @@
 
         Returns
         -------
         grid_segment
             The segment.
         """
         segments = []
+        dlen = len(self.diagram)
         for i, row in enumerate(self.diagram):
             seg = None
             for j, c in enumerate(row):
                 if c.strip() != "":
                     if seg is None:
                         seg = grid_segment()
                     if c.strip().lower() == "x":
-                        seg.sink = self.__rotate(i, j)
+                        seg.sink = self.__rotate(dlen - j, i)
                     if c.strip().lower() == "o":
-                        seg.source = self.__rotate(i, j)
+                        seg.source = self.__rotate(dlen - j, i)
             if seg is not None:
                 segments.append(seg)
         return segments
 
     def __get_segments_vertical(self):
         """Parse the grid for vertical segments.
 
         Returns
         -------
         grid_segment
             The segment.
         """
         segments = []
+        dlen = len(self.diagram)
         # Get vertical
         for j, c in enumerate(self.diagram[0]):
             seg = None
             for i, row in enumerate(self.diagram):
                 if row[j].strip() != "":
                     if seg is None:
                         seg = grid_segment()
                     if row[j].strip().lower() == "x":
-                        seg.source = self.__rotate(i, j)
+                        seg.source = self.__rotate(dlen - j, i)
                     if row[j].strip().lower() == "o":
-                        seg.sink = self.__rotate(i, j)
+                        seg.sink = self.__rotate(dlen - j, i)
             if seg is not None:
                 segments.append(seg)
         return segments
 
     def __draw_segment(self, step):
         """Draws a segment of the front projection as a Bézier curve.
 
@@ -159,15 +161,15 @@
         -------
         Drawing
             The svg for the grid diagram.
 
         """
         try:
             d = draw.Drawing(
-                self.scale * len(self.diagram[0]),
+                self.scale * math.sqrt(2) * len(self.diagram[0]),
                 self.scale * math.sqrt(2) * len(self.diagram[0]),
                 origin=(0, 0),
                 id_prefix="d",
             )
             g = draw.Group(
                 stroke_width=0.1 * self.scale,
                 stroke="black",
```

### Comparing `grid2fp-0.0.3/grid2fp.egg-info/PKG-INFO` & `grid2fp-0.0.4/grid2fp.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grid2fp
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tool to eat grid diagrams and generate its front projection.
 Home-page: https://github.com/Joecstarr/grid2fp
 Author: Casey Duckering
 Keywords: topology,Legendrian,Grid Diagram,knot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `grid2fp-0.0.3/setup.py` & `grid2fp-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import logging
 
 logger = logging.getLogger(__name__)
 
-version = "0.0.3"
+version = "0.0.4"
 
 try:
     with open("README.md", "r") as f:
         long_desc = f.read()
 except:
     logger.warning("Could not open README.md.  long_description will be set to None.")
     long_desc = None
```

