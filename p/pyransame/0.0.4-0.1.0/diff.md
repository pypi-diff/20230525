# Comparing `tmp/pyransame-0.0.4.tar.gz` & `tmp/pyransame-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyransame-0.0.4.tar", last modified: Wed Apr 26 16:22:29 2023, max compression
+gzip compressed data, was "pyransame-0.1.0.tar", last modified: Thu May 25 12:03:39 2023, max compression
```

## Comparing `pyransame-0.0.4.tar` & `pyransame-0.1.0.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.287916 pyransame-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.283916 pyransame-0.0.4/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-26 16:22:15.000000 pyransame-0.0.4/.devcontainer/devcontainer.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      253 2023-04-26 16:22:15.000000 pyransame-0.0.4/.devcontainer/oncreatecommand.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.283916 pyransame-0.0.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-26 16:22:15.000000 pyransame-0.0.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.283916 pyransame-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-26 16:22:15.000000 pyransame-0.0.4/.github/workflows/pages_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-26 16:22:15.000000 pyransame-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-26 16:22:15.000000 pyransame-0.0.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-26 16:22:15.000000 pyransame-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-26 16:22:15.000000 pyransame-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-26 16:22:15.000000 pyransame-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-26 16:22:29.287916 pyransame-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-26 16:22:15.000000 pyransame-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.283916 pyransame-0.0.4/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-26 16:22:15.000000 pyransame-0.0.4/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.283916 pyransame-0.0.4/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   146735 2023-04-26 16:22:15.000000 pyransame-0.0.4/doc/_static/surface_sampling.png
--rw-r--r--   0 runner    (1001) docker     (123)   183927 2023-04-26 16:22:15.000000 pyransame-0.0.4/doc/_static/volume_sampling.png
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-26 16:22:15.000000 pyransame-0.0.4/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-26 16:22:15.000000 pyransame-0.0.4/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-26 16:22:15.000000 pyransame-0.0.4/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-26 16:22:15.000000 pyransame-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-26 16:22:15.000000 pyransame-0.0.4/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-26 16:22:15.000000 pyransame-0.0.4/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 16:22:29.287916 pyransame-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.279915 pyransame-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.283916 pyransame-0.0.4/src/pyransame/
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-04-26 16:22:15.000000 pyransame-0.0.4/src/pyransame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 16:22:29.000000 pyransame-0.0.4/src/pyransame/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-26 16:22:15.000000 pyransame-0.0.4/src/pyransame/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.287916 pyransame-0.0.4/src/pyransame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-26 16:22:29.000000 pyransame-0.0.4/src/pyransame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-26 16:22:29.000000 pyransame-0.0.4/src/pyransame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:22:29.000000 pyransame-0.0.4/src/pyransame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 16:22:29.000000 pyransame-0.0.4/src/pyransame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 16:22:29.000000 pyransame-0.0.4/src/pyransame.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.287916 pyransame-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 16:22:15.000000 pyransame-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-26 16:22:15.000000 pyransame-0.0.4/tests/test_random_surface_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-26 16:22:15.000000 pyransame-0.0.4/tests/test_random_volume_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-04-26 16:22:15.000000 pyransame-0.0.4/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.397144 pyransame-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.393144 pyransame-0.1.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 12:03:28.000000 pyransame-0.1.0/.devcontainer/devcontainer.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      253 2023-05-25 12:03:28.000000 pyransame-0.1.0/.devcontainer/oncreatecommand.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.393144 pyransame-0.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-25 12:03:28.000000 pyransame-0.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.393144 pyransame-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-25 12:03:28.000000 pyransame-0.1.0/.github/workflows/pages_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-25 12:03:28.000000 pyransame-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-25 12:03:28.000000 pyransame-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-25 12:03:28.000000 pyransame-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-25 12:03:28.000000 pyransame-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-25 12:03:28.000000 pyransame-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-25 12:03:39.393144 pyransame-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-25 12:03:28.000000 pyransame-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.393144 pyransame-0.1.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-25 12:03:28.000000 pyransame-0.1.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.393144 pyransame-0.1.0/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   146735 2023-05-25 12:03:28.000000 pyransame-0.1.0/doc/_static/surface_sampling.png
+-rw-r--r--   0 runner    (1001) docker     (123)   183927 2023-05-25 12:03:28.000000 pyransame-0.1.0/doc/_static/volume_sampling.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-25 12:03:28.000000 pyransame-0.1.0/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-05-25 12:03:28.000000 pyransame-0.1.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-25 12:03:28.000000 pyransame-0.1.0/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-25 12:03:28.000000 pyransame-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 12:03:28.000000 pyransame-0.1.0/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 12:03:28.000000 pyransame-0.1.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 12:03:39.397144 pyransame-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.389144 pyransame-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.393144 pyransame-0.1.0/src/pyransame/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-25 12:03:28.000000 pyransame-0.1.0/src/pyransame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 12:03:39.000000 pyransame-0.1.0/src/pyransame/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:28.000000 pyransame-0.1.0/src/pyransame/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-25 12:03:28.000000 pyransame-0.1.0/src/pyransame/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-25 12:03:28.000000 pyransame-0.1.0/src/pyransame/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-25 12:03:28.000000 pyransame-0.1.0/src/pyransame/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.393144 pyransame-0.1.0/src/pyransame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-25 12:03:39.000000 pyransame-0.1.0/src/pyransame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-25 12:03:39.000000 pyransame-0.1.0/src/pyransame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:03:39.000000 pyransame-0.1.0/src/pyransame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 12:03:39.000000 pyransame-0.1.0/src/pyransame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 12:03:39.000000 pyransame-0.1.0/src/pyransame.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:03:39.393144 pyransame-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-25 12:03:28.000000 pyransame-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-05-25 12:03:28.000000 pyransame-0.1.0/tests/test_random_surface_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-25 12:03:28.000000 pyransame-0.1.0/tests/test_random_volume_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-25 12:03:28.000000 pyransame-0.1.0/tests/test_rng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-25 12:03:28.000000 pyransame-0.1.0/tests/test_util.py
```

### Comparing `pyransame-0.0.4/.github/workflows/pages_publish.yml` & `pyransame-0.1.0/.github/workflows/pages_publish.yml`

 * *Files identical despite different names*

### Comparing `pyransame-0.0.4/.github/workflows/python-publish.yml` & `pyransame-0.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyransame-0.0.4/.gitignore` & `pyransame-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyransame-0.0.4/LICENSE` & `pyransame-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyransame-0.0.4/doc/Makefile` & `pyransame-0.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyransame-0.0.4/doc/_static/surface_sampling.png` & `pyransame-0.1.0/doc/_static/surface_sampling.png`

 * *Files identical despite different names*

### Comparing `pyransame-0.0.4/doc/_static/volume_sampling.png` & `pyransame-0.1.0/doc/_static/volume_sampling.png`

 * *Files identical despite different names*

### Comparing `pyransame-0.0.4/doc/conf.py` & `pyransame-0.1.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pyransame-0.0.4/doc/index.rst` & `pyransame-0.1.0/doc/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Welcome to pyransame's documentation!
 =====================================
 
 PYthon RAndom SAmpling for MEshes (pyransame) provides utilities
-for choosing rando samples of points within cells of
+for choosing random samples of points within cells of
 `PyVista <https://docs.pyvista.org/>`_ meshes.
 
 Examples
 --------
 
 Random points on surface
 ~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `pyransame-0.0.4/doc/make.bat` & `pyransame-0.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pyransame-0.0.4/src/pyransame.egg-info/SOURCES.txt` & `pyransame-0.1.0/src/pyransame.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,17 +15,21 @@
 doc/conf.py
 doc/index.rst
 doc/make.bat
 doc/_static/surface_sampling.png
 doc/_static/volume_sampling.png
 src/pyransame/__init__.py
 src/pyransame/_version.py
+src/pyransame/py.typed
+src/pyransame/surface.py
 src/pyransame/util.py
+src/pyransame/volume.py
 src/pyransame.egg-info/PKG-INFO
 src/pyransame.egg-info/SOURCES.txt
 src/pyransame.egg-info/dependency_links.txt
 src/pyransame.egg-info/requires.txt
 src/pyransame.egg-info/top_level.txt
 tests/__init__.py
 tests/test_random_surface_points.py
 tests/test_random_volume_points.py
+tests/test_rng.py
 tests/test_util.py
```

### Comparing `pyransame-0.0.4/tests/test_util.py` & `pyransame-0.1.0/tests/test_util.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,17 +6,20 @@
 import pyvista as pv
 from hypothesis import assume, given, settings
 from hypothesis import strategies as st
 from hypothesis.extra.numpy import arrays
 
 from pyransame.util import (
     _generate_points_in_pixel,
+    _generate_points_in_polygon,
+    _generate_points_in_pyramid,
     _generate_points_in_quad,
     _generate_points_in_tetra,
     _generate_points_in_tri,
+    _generate_points_in_tri_strip,
     _generate_points_in_voxel,
 )
 
 
 @settings(deadline=timedelta(milliseconds=500))
 # Use min_value and max_value to avoid numerical imprecision artifacts, but still span a large space
 @given(
@@ -29,15 +32,15 @@
     # make sure that the points are not coincident
     assume(not np.allclose(a, b, rtol=1e-3, atol=1e-3))
     assume(not np.allclose(b, c, rtol=1e-3, atol=1e-3))
     assume(not np.allclose(a, c, rtol=1e-3, atol=1e-3))
     tri = pv.Triangle([a, b, c])
     assume(tri.area > 1e-4)
 
-    points = _generate_points_in_tri(a, b, c, 1000)
+    points = _generate_points_in_tri(np.array([a, b, c]), 1000)
     for i in range(1000):
         assert tri.find_containing_cell(points[i, :]) == 0
 
 
 # equations from https://mathworld.wolfram.com/TrianglePointPicking.html
 # Weisstein, Eric W. "Triangle Point Picking." From MathWorld--A Wolfram Web Resource.
 def test_uniformity_tri():
@@ -45,15 +48,15 @@
     a = np.array((0.0, 0.0, 0.0))
     b = np.array((1.0, 0.0, 0.0))
     c = np.array((0.5, np.sqrt(3.0) / 2.0, 0.0))
 
     center = np.array((0.5, np.sqrt(3.0) / 6.0, 0.0))
 
     # needs a lot of points to converge
-    points = _generate_points_in_tri(a, b, c, 2000000)
+    points = _generate_points_in_tri(np.array([a, b, c]), 2000000)
 
     distances = np.linalg.norm(points - center, axis=-1)
     exp_distance = (
         1 / 72 * (8 * np.sqrt(3) + 3 * np.arcsinh(np.sqrt(3)) + np.log(2 + np.sqrt(3)))
     )
     assert distances.mean() == pytest.approx(exp_distance, rel=2e-3)
 
@@ -69,15 +72,15 @@
     b = np.array((-np.sqrt(3) / 6, 0.5, -np.sqrt(6) / 12.0))
     c = np.array((-np.sqrt(3) / 6, -0.5, -np.sqrt(6) / 12.0))
     d = np.array((0.0, 0.0, np.sqrt(6) / 4))
 
     center = np.array((0.0, 0.0, 0.0))
 
     # needs a lot of points to converge
-    points = _generate_points_in_tetra(a, b, c, d, 2000000)
+    points = _generate_points_in_tetra(np.array([a, b, c, d]), 2000000)
 
     assert np.allclose(points.mean(axis=0), center, rtol=1e-3, atol=1e-3)
 
 
 @settings(deadline=timedelta(milliseconds=500))
 # Use min_value and max_value to avoid numerical imprecision artifacts, but still span a large space
 @given(
@@ -97,15 +100,15 @@
     assume(not np.allclose(c, d, rtol=1e-3, atol=1e-3))
 
     cells = [4, 0, 1, 2, 3]
     celltypes = [pv.CellType.TETRA]
     tetra = pv.UnstructuredGrid(cells, celltypes, [a, b, c, d])
     assume(tetra.volume > 1e-4)
 
-    points = _generate_points_in_tetra(a, b, c, d, 1000)
+    points = _generate_points_in_tetra(np.array([a, b, c, d]), 1000)
     for i in range(1000):
         assert tetra.find_containing_cell(points[i, :]) == 0
 
 
 def test_uniformity_quad():
     # Quad can be non-square
     a = np.array([0.0, 0.0, 0.0])
@@ -125,33 +128,106 @@
 
     center_abc = b + 2 / 3 * np.array([-0.5, 0.5, 0.0])
     center_acd = d + 2 / 3 * np.array([0.25, -0.25, 0.0])
 
     center = (center_abc * area_abc + center_acd * area_acd) / (area_abc + area_acd)
 
     # needs a lot of points to converge
-    points = _generate_points_in_quad(a, b, c, d, 2000000)
+    points = _generate_points_in_quad(np.array([a, b, c, d]), 2000000)
+
+    assert np.allclose(points.mean(axis=0), center, rtol=1e-3, atol=1e-3)
+
+
+def test_uniformity_polygon():
+    # Use same quad test
+    a = np.array([0.0, 0.0, 0.0])
+    b = np.array([1.0, 0.0, 0.0])
+    c = np.array([1.0, 1.0, 0.0])
+    d = np.array([0.25, 0.75, 0.0])
+
+    area_abc = 1 * 1 / 2.0
+    l_side_acd = np.sqrt(0.75**2 + 0.25**2)
+    l_base_acd = np.sqrt(2.0)
+    area_acd = (
+        1.0
+        / 2.0
+        * l_base_acd**2
+        * np.sqrt(l_side_acd**2 / l_base_acd**2 - 1.0 / 4.0)
+    )
+
+    center_abc = b + 2 / 3 * np.array([-0.5, 0.5, 0.0])
+    center_acd = d + 2 / 3 * np.array([0.25, -0.25, 0.0])
+
+    center = (center_abc * area_abc + center_acd * area_acd) / (area_abc + area_acd)
+
+    # needs a lot of points to converge
+    points = _generate_points_in_polygon(np.array([a, b, c, d]), 2000000)
+
+    assert np.allclose(points.mean(axis=0), center, rtol=1e-3, atol=1e-3)
+
+
+def test_uniformity_tri_strip():
+    a = np.array([0.0, 0.0, 0.0])
+    b = np.array([1.0, 0.0, 0.0])
+    c = np.array([1.0, 1.0, 0.0])
+    d = np.array([0.25, 0.75, 0.0])
+
+    area_abc = 1 * 1 / 2.0
+    l_side_acd = np.sqrt(0.75**2 + 0.25**2)
+    l_base_acd = np.sqrt(2.0)
+    area_acd = (
+        1.0
+        / 2.0
+        * l_base_acd**2
+        * np.sqrt(l_side_acd**2 / l_base_acd**2 - 1.0 / 4.0)
+    )
+
+    center_abc = b + 2 / 3 * np.array([-0.5, 0.5, 0.0])
+    center_acd = d + 2 / 3 * np.array([0.25, -0.25, 0.0])
+
+    center = (center_abc * area_abc + center_acd * area_acd) / (area_abc + area_acd)
+
+    # needs a lot of points to converge
+    points = _generate_points_in_tri_strip(np.array([b, a, c, d]), 2000000)
 
     assert np.allclose(points.mean(axis=0), center, rtol=1e-3, atol=1e-3)
 
 
 def test_uniformity_pixel():
     a = np.array([0.0, 0.0, 0.0])
     b = np.array([1.0, 0.0, 0.0])
     c = np.array([1.0, 2.0, 0.0])
     d = np.array([0.0, 2.0, 0.0])
 
     # needs a lot of points to converge
-    points = _generate_points_in_pixel(a, b, d, c, 2000000)
+    points = _generate_points_in_pixel(np.array([a, b, d, c]), 2000000)
     center = np.array([0.5, 1.0, 0.0])
 
     assert np.allclose(points.mean(axis=0), center, rtol=1e-3, atol=1e-3)
 
 
 def test_uniformity_voxel():
     mesh = pv.UniformGrid(dimensions=(2, 2, 2), spacing=(1.0, 1.0, 2.0))
 
     # needs a lot of points to converge
-    points = _generate_points_in_voxel(*mesh.points, 2000000)
+    points = _generate_points_in_voxel(mesh.points, 2000000)
     center = np.array([0.5, 0.5, 1.0])
 
     assert np.allclose(points.mean(axis=0), center, rtol=1e-3, atol=1e-3)
+
+
+def test_uniformity_pyramid():
+    mesh = pv.Pyramid(
+        [
+            [1.0, 1.0, 0.0],
+            [-1.0, 1.0, 0.0],
+            [-1.0, -1.0, 0.0],
+            [1.0, -1.0, 0.0],
+            [0.0, 0.0, 1.0],
+        ]
+    )
+
+    center = np.array([0.0, 0.0, 0.25])
+
+    points = _generate_points_in_pyramid(mesh.points, 2000000)
+
+    assert np.allclose(points.mean(axis=0), center, rtol=1e-3, atol=1e-3)
```

