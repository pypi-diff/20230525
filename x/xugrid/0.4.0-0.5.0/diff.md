# Comparing `tmp/xugrid-0.4.0.tar.gz` & `tmp/xugrid-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xugrid-0.4.0.tar", last modified: Fri May  5 15:07:53 2023, max compression
+gzip compressed data, was "xugrid-0.5.0.tar", last modified: Thu May 25 15:30:10 2023, max compression
```

## Comparing `xugrid-0.4.0.tar` & `xugrid-0.5.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 15:07:53.242926 xugrid-0.4.0/
--rw-rw-rw-   0        0        0     1079 2021-09-15 16:10:43.000000 xugrid-0.4.0/LICENSE
--rw-rw-rw-   0        0        0       34 2021-10-06 12:44:47.000000 xugrid-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3298 2023-05-05 15:07:53.242926 xugrid-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2157 2023-03-13 10:25:22.000000 xugrid-0.4.0/README.rst
--rw-rw-rw-   0        0        0     2199 2023-05-05 15:03:53.000000 xugrid-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0      159 2023-05-05 15:07:53.244925 xugrid-0.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-05 15:07:53.031921 xugrid-0.4.0/tests/
--rw-rw-rw-   0        0        0    15587 2023-04-21 11:32:07.000000 xugrid-0.4.0/tests/test_connectivity.py
--rw-rw-rw-   0        0        0    10108 2023-03-13 10:25:22.000000 xugrid-0.4.0/tests/test_conventions.py
--rw-rw-rw-   0        0        0     9027 2023-03-13 10:25:22.000000 xugrid-0.4.0/tests/test_conversion.py
--rw-rw-rw-   0        0        0     1008 2023-03-13 10:25:22.000000 xugrid-0.4.0/tests/test_data.py
--rw-rw-rw-   0        0        0      851 2023-03-13 10:25:22.000000 xugrid-0.4.0/tests/test_interpolate.py
--rw-rw-rw-   0        0        0     1219 2023-03-13 10:25:22.000000 xugrid-0.4.0/tests/test_meshkernel_utils.py
--rw-rw-rw-   0        0        0     9084 2023-03-13 10:25:22.000000 xugrid-0.4.0/tests/test_plot.py
--rw-rw-rw-   0        0        0     4245 2023-03-13 10:25:22.000000 xugrid-0.4.0/tests/test_snap.py
--rw-rw-rw-   0        0        0     9280 2023-04-21 11:32:07.000000 xugrid-0.4.0/tests/test_ugrid1d.py
--rw-rw-rw-   0        0        0    30534 2023-04-21 11:32:07.000000 xugrid-0.4.0/tests/test_ugrid2d.py
--rw-rw-rw-   0        0        0    26751 2023-04-21 11:32:07.000000 xugrid-0.4.0/tests/test_ugrid_dataset.py
--rw-rw-rw-   0        0        0    10444 2023-04-21 11:32:07.000000 xugrid-0.4.0/tests/test_voronoi.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:07:53.049922 xugrid-0.4.0/xugrid/
--rw-rw-rw-   0        0        0     1020 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/__init__.py
--rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/constants.py
--rw-rw-rw-   0        0        0     8398 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/conversion.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:07:53.103930 xugrid-0.4.0/xugrid/core/
--rw-rw-rw-   0        0        0     3303 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/core/accessorbase.py
--rw-rw-rw-   0        0        0     3516 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/core/common.py
--rw-rw-rw-   0        0        0    18334 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/core/dataarray_accessor.py
--rw-rw-rw-   0        0        0    13439 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/core/dataset_accessor.py
--rw-rw-rw-   0        0        0    11821 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/core/wrap.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:07:53.124929 xugrid-0.4.0/xugrid/data/
--rw-rw-rw-   0        0        0      126 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/data/__init__.py
--rw-rw-rw-   0        0        0      331 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/data/registry.txt
--rw-rw-rw-   0        0        0     2109 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/data/sample_data.py
--rw-rw-rw-   0        0        0     3083 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/data/synthetic.py
--rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/meshkernel_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:07:53.138920 xugrid-0.4.0/xugrid/plot/
--rw-rw-rw-   0        0        0      149 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/plot/__init__.py
--rw-rw-rw-   0        0        0    24058 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/plot/plot.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:07:53.175924 xugrid-0.4.0/xugrid/regrid/
--rw-rw-rw-   0        0        0     7616 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/regrid/overlap_1d.py
--rw-rw-rw-   0        0        0     5015 2023-03-14 17:12:37.000000 xugrid-0.4.0/xugrid/regrid/reduce.py
--rw-rw-rw-   0        0        0    15067 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/regrid/regridder.py
--rw-rw-rw-   0        0        0     1998 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/regrid/structured.py
--rw-rw-rw-   0        0        0     4050 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/regrid/unstructured.py
--rw-rw-rw-   0        0        0      985 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/regrid/utils.py
--rw-rw-rw-   0        0        0     3661 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/regrid/weight_matrix.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:07:53.240925 xugrid-0.4.0/xugrid/ugrid/
--rw-rw-rw-   0        0        0        0 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/ugrid/__init__.py
--rw-rw-rw-   0        0        0    18746 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/ugrid/connectivity.py
--rw-rw-rw-   0        0        0    14841 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/ugrid/conventions.py
--rw-rw-rw-   0        0        0     4996 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/ugrid/interpolate.py
--rw-rw-rw-   0        0        0    10227 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/ugrid/partitioning.py
--rw-rw-rw-   0        0        0    14979 2023-05-05 14:49:08.000000 xugrid-0.4.0/xugrid/ugrid/snapping.py
--rw-rw-rw-   0        0        0    17949 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/ugrid/ugrid1d.py
--rw-rw-rw-   0        0        0    53962 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/ugrid/ugrid2d.py
--rw-rw-rw-   0        0        0    19806 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/ugrid/ugridbase.py
--rw-rw-rw-   0        0        0    14113 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/ugrid/voronoi.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:07:53.063936 xugrid-0.4.0/xugrid.egg-info/
--rw-rw-rw-   0        0        0     3298 2023-05-05 15:07:52.000000 xugrid-0.4.0/xugrid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1311 2023-05-05 15:07:52.000000 xugrid-0.4.0/xugrid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 15:07:52.000000 xugrid-0.4.0/xugrid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      252 2023-05-05 15:07:52.000000 xugrid-0.4.0/xugrid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 15:07:52.000000 xugrid-0.4.0/xugrid.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 15:30:10.924360 xugrid-0.5.0/
+-rw-rw-rw-   0        0        0     1079 2021-09-15 16:10:43.000000 xugrid-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0       34 2021-10-06 12:44:47.000000 xugrid-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3298 2023-05-25 15:30:10.925357 xugrid-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2157 2023-03-13 10:25:22.000000 xugrid-0.5.0/README.rst
+-rw-rw-rw-   0        0        0     2199 2023-05-25 15:26:07.000000 xugrid-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0      178 2023-05-25 15:30:10.934354 xugrid-0.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 15:30:10.283814 xugrid-0.5.0/tests/
+-rw-rw-rw-   0        0        0    15587 2023-04-21 11:32:07.000000 xugrid-0.5.0/tests/test_connectivity.py
+-rw-rw-rw-   0        0        0    10108 2023-03-13 10:25:22.000000 xugrid-0.5.0/tests/test_conventions.py
+-rw-rw-rw-   0        0        0     9027 2023-03-13 10:25:22.000000 xugrid-0.5.0/tests/test_conversion.py
+-rw-rw-rw-   0        0        0     1008 2023-03-13 10:25:22.000000 xugrid-0.5.0/tests/test_data.py
+-rw-rw-rw-   0        0        0      851 2023-03-13 10:25:22.000000 xugrid-0.5.0/tests/test_interpolate.py
+-rw-rw-rw-   0        0        0     1219 2023-03-13 10:25:22.000000 xugrid-0.5.0/tests/test_meshkernel_utils.py
+-rw-rw-rw-   0        0        0     9084 2023-03-13 10:25:22.000000 xugrid-0.5.0/tests/test_plot.py
+-rw-rw-rw-   0        0        0     4245 2023-03-13 10:25:22.000000 xugrid-0.5.0/tests/test_snap.py
+-rw-rw-rw-   0        0        0     9280 2023-04-21 11:32:07.000000 xugrid-0.5.0/tests/test_ugrid1d.py
+-rw-rw-rw-   0        0        0    30534 2023-04-21 11:32:07.000000 xugrid-0.5.0/tests/test_ugrid2d.py
+-rw-rw-rw-   0        0        0    26751 2023-04-21 11:32:07.000000 xugrid-0.5.0/tests/test_ugrid_dataset.py
+-rw-rw-rw-   0        0        0    10444 2023-04-21 11:32:07.000000 xugrid-0.5.0/tests/test_voronoi.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:30:10.307787 xugrid-0.5.0/xugrid/
+-rw-rw-rw-   0        0        0     1020 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/__init__.py
+-rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/constants.py
+-rw-rw-rw-   0        0        0     8398 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/conversion.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:30:10.367313 xugrid-0.5.0/xugrid/core/
+-rw-rw-rw-   0        0        0     3303 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/core/accessorbase.py
+-rw-rw-rw-   0        0        0     3516 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/core/common.py
+-rw-rw-rw-   0        0        0    18334 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/core/dataarray_accessor.py
+-rw-rw-rw-   0        0        0    13439 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/core/dataset_accessor.py
+-rw-rw-rw-   0        0        0    11821 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/core/wrap.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:30:10.387314 xugrid-0.5.0/xugrid/data/
+-rw-rw-rw-   0        0        0      126 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/data/__init__.py
+-rw-rw-rw-   0        0        0      331 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/data/registry.txt
+-rw-rw-rw-   0        0        0     2109 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/data/sample_data.py
+-rw-rw-rw-   0        0        0     3083 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/data/synthetic.py
+-rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/meshkernel_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:30:10.403313 xugrid-0.5.0/xugrid/plot/
+-rw-rw-rw-   0        0        0      149 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/plot/__init__.py
+-rw-rw-rw-   0        0        0    24058 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/plot/plot.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:30:10.555314 xugrid-0.5.0/xugrid/regrid/
+-rw-rw-rw-   0        0        0     7616 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/regrid/overlap_1d.py
+-rw-rw-rw-   0        0        0     5015 2023-03-14 17:12:37.000000 xugrid-0.5.0/xugrid/regrid/reduce.py
+-rw-rw-rw-   0        0        0    17648 2023-05-25 15:11:34.000000 xugrid-0.5.0/xugrid/regrid/regridder.py
+-rw-rw-rw-   0        0        0    22639 2023-05-25 15:11:34.000000 xugrid-0.5.0/xugrid/regrid/structured.py
+-rw-rw-rw-   0        0        0     4658 2023-05-25 15:11:34.000000 xugrid-0.5.0/xugrid/regrid/unstructured.py
+-rw-rw-rw-   0        0        0     1245 2023-05-25 15:11:34.000000 xugrid-0.5.0/xugrid/regrid/utils.py
+-rw-rw-rw-   0        0        0     3661 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/regrid/weight_matrix.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:30:10.921352 xugrid-0.5.0/xugrid/ugrid/
+-rw-rw-rw-   0        0        0        0 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/ugrid/__init__.py
+-rw-rw-rw-   0        0        0    18746 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/ugrid/connectivity.py
+-rw-rw-rw-   0        0        0    14841 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/ugrid/conventions.py
+-rw-rw-rw-   0        0        0     4996 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/ugrid/interpolate.py
+-rw-rw-rw-   0        0        0    10227 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/ugrid/partitioning.py
+-rw-rw-rw-   0        0        0    14979 2023-05-05 14:49:08.000000 xugrid-0.5.0/xugrid/ugrid/snapping.py
+-rw-rw-rw-   0        0        0    17949 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/ugrid/ugrid1d.py
+-rw-rw-rw-   0        0        0    53962 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/ugrid/ugrid2d.py
+-rw-rw-rw-   0        0        0    19806 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/ugrid/ugridbase.py
+-rw-rw-rw-   0        0        0    14113 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/ugrid/voronoi.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:30:10.330785 xugrid-0.5.0/xugrid.egg-info/
+-rw-rw-rw-   0        0        0     3298 2023-05-25 15:30:10.000000 xugrid-0.5.0/xugrid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1311 2023-05-25 15:30:10.000000 xugrid-0.5.0/xugrid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 15:30:10.000000 xugrid-0.5.0/xugrid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      252 2023-05-25 15:30:10.000000 xugrid-0.5.0/xugrid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-25 15:30:10.000000 xugrid-0.5.0/xugrid.egg-info/top_level.txt
```

### Comparing `xugrid-0.4.0/LICENSE` & `xugrid-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/PKG-INFO` & `xugrid-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xugrid
-Version: 0.4.0
+Version: 0.5.0
 Summary: Xarray extension for unstructured grids
 Maintainer-email: Huite Bootsma <huite.bootsma@deltares.nl>
 License: MIT
 Project-URL: Home, https://github.com/deltares/xugrid
 Project-URL: Code, https://github.com/deltares/xugrid
 Project-URL: Issues, https://github.com/deltares/xugrid/issues
 Keywords: mesh,ugrid,unstructured grid,xarray
```

### Comparing `xugrid-0.4.0/README.rst` & `xugrid-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/pyproject.toml` & `xugrid-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xugrid"
 description = "Xarray extension for unstructured grids"
 readme = { file = "README.rst", content-type = "text/x-rst" }
-version = "0.4.0"
+version = "0.5.0"
 maintainers = [{ name = "Huite Bootsma", email = "huite.bootsma@deltares.nl" }]
 requires-python = ">=3.7"
 dependencies = [
     'pandas',
     'numba',
     'numba_celltree',
     'numpy',
```

### Comparing `xugrid-0.4.0/tests/test_connectivity.py` & `xugrid-0.5.0/tests/test_connectivity.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/tests/test_conventions.py` & `xugrid-0.5.0/tests/test_conventions.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/tests/test_conversion.py` & `xugrid-0.5.0/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/tests/test_data.py` & `xugrid-0.5.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/tests/test_interpolate.py` & `xugrid-0.5.0/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/tests/test_meshkernel_utils.py` & `xugrid-0.5.0/tests/test_meshkernel_utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/tests/test_plot.py` & `xugrid-0.5.0/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/tests/test_snap.py` & `xugrid-0.5.0/tests/test_snap.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/tests/test_ugrid1d.py` & `xugrid-0.5.0/tests/test_ugrid1d.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/tests/test_ugrid2d.py` & `xugrid-0.5.0/tests/test_ugrid2d.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/tests/test_ugrid_dataset.py` & `xugrid-0.5.0/tests/test_ugrid_dataset.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/tests/test_voronoi.py` & `xugrid-0.5.0/tests/test_voronoi.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/__init__.py` & `xugrid-0.5.0/xugrid/__init__.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/constants.py` & `xugrid-0.5.0/xugrid/constants.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/conversion.py` & `xugrid-0.5.0/xugrid/conversion.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/core/accessorbase.py` & `xugrid-0.5.0/xugrid/core/accessorbase.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/core/common.py` & `xugrid-0.5.0/xugrid/core/common.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/core/dataarray_accessor.py` & `xugrid-0.5.0/xugrid/core/dataarray_accessor.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/core/dataset_accessor.py` & `xugrid-0.5.0/xugrid/core/dataset_accessor.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/core/wrap.py` & `xugrid-0.5.0/xugrid/core/wrap.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/data/sample_data.py` & `xugrid-0.5.0/xugrid/data/sample_data.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/data/synthetic.py` & `xugrid-0.5.0/xugrid/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/meshkernel_utils.py` & `xugrid-0.5.0/xugrid/meshkernel_utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/plot/plot.py` & `xugrid-0.5.0/xugrid/plot/plot.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/regrid/overlap_1d.py` & `xugrid-0.5.0/xugrid/regrid/overlap_1d.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/regrid/reduce.py` & `xugrid-0.5.0/xugrid/regrid/reduce.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/regrid/regridder.py` & `xugrid-0.5.0/xugrid/regrid/regridder.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 except ImportError:
     DaskArray = ()
 
 import xugrid
 from xugrid.constants import FloatArray
 from xugrid.core.wrap import UgridDataArray
 from xugrid.regrid import reduce
+from xugrid.regrid.structured import StructuredGrid2d
 from xugrid.regrid.unstructured import UnstructuredGrid2d
 from xugrid.regrid.weight_matrix import (
     WeightMatrixCOO,
     WeightMatrixCSR,
     nzrange,
     weight_matrix_coo,
     weight_matrix_csr,
@@ -49,24 +50,50 @@
                 if len(indices) > 0:
                     out[extra_index, target_index] = f(source_flat, indices, weights)
         return out
 
     return numba.njit(_regrid, parallel=True, cache=True)
 
 
+def setup_grid(obj):
+    if isinstance(obj, (xu.Ugrid2d, xu.UgridDataArray, xu.UgridDataset)):
+        return UnstructuredGrid2d(obj)
+    elif isinstance(obj, (xr.DataArray, xr.Dataset)):
+        return StructuredGrid2d(obj, name_y="y", name_x="x")
+    else:
+        raise TypeError()
+
+
+def convert_to_match(source, target):
+    PROMOTIONS = {
+        frozenset({StructuredGrid2d}): StructuredGrid2d,
+        frozenset({StructuredGrid2d, UnstructuredGrid2d}): UnstructuredGrid2d,
+        frozenset({UnstructuredGrid2d, UnstructuredGrid2d}): UnstructuredGrid2d,
+        #    {StructuredGrid3d, ExplicitStructuredGrid3d}: ExplicitStructuredGrid3d,
+        #    {LayeredUnstructuredGrid2d, StructuredGrid2d}: StructuredGrid2d,
+        #    {LayeredUnstructuredGrid2d, StructuredGrid2d}: StructuredGrid2d,
+        #    {StructuredGrid3d, StructuredGrid2d}: StructuredGrid2d,
+        #    # etc.
+    }
+    types = set({type(source), type(target)})
+    matched_type = PROMOTIONS[frozenset(types)]
+    return source.convert_to(matched_type), target.convert_to(matched_type)
+
+
 class BaseRegridder(abc.ABC):
     _JIT_FUNCTIONS = {}
 
     def __init__(
         self,
         source: "xugrid.Ugrid2d",
         target: "xugrid.Ugrid2d",
     ):
-        self._target = UnstructuredGrid2d(target)
-        self._compute_weights(UnstructuredGrid2d(source), self._target)
+        self._source = setup_grid(source)
+        self._target = setup_grid(target)
+        self._compute_weights(self._source, self._target)
         return
 
     @abc.abstractproperty
     def weights(self):
         """ """
 
     @abc.abstractmethod
@@ -88,36 +115,41 @@
             self._regrid = make_regrid(func)
         else:
             raise TypeError(
                 f"method must be string or callable, received: {type(func).__name}"
             )
         return
 
-    def regrid_array(self, source):
-        first_dims = source.shape[:-1]
-        last_dims = source.shape[-1:]
-
-        # TODO: store source and do some checking.
-        # Alternatively, check by weights.
-        # if last_dims != self._source.shape:
-        #    raise ValueError(
-        #        "Shape of last source dimensions does not match regridder "
-        #        f"shape: {last_dims} versus {self._source.shape}"
-        #    )
+    def _regrid_array(self, source):
+        if hasattr(self, "_source"):
+            source_grid = self._source
+        else:
+            source_grid = source
+        first_dims_shape = source.shape[: -source_grid.ndim]
 
-        if source.ndim == 1:
+        # The regridding can be mapped over additional dimensions (e.g. for every time slice).
+        # This is the `extra_index` iteration in _regrid().
+        # But it should work consistently even if no additional present: in that case we create
+        # a 1-sized additional dimension in front, so the `extra_index` iteration always applies.
+        if source.ndim == source_grid.ndim:
             source = source[np.newaxis]
-        elif source.ndim > 2:
-            source = source.reshape((-1,) + last_dims)
 
-        size = self._target.size
-        out_shape = first_dims + self._target.shape
+        # All additional dimension are flattened into one, in front.
+        # E.g.:
+        #
+        #   * ("dummy", "face") -> ("dummy", "face")
+        #   * ("time", "layer", "y", "x") -> ("stacked_time_layer", "stacked_y_x")
+        #   * ("time", "layer", "face") -> ("stacked_time_layer", "face")
+        #
+        # Source is always 2D after this step, sized: (n_extra, size).
+        source = source.reshape((-1, source_grid.size))
 
+        size = self._target.size
         if isinstance(source, DaskArray):
-            chunks = source.chunks[:-1] + (self._target.shape,)
+            chunks = source.chunks[: -source_grid.ndim] + (self._target.shape,)
             out = dask.array.map_blocks(
                 self._regrid,  # func
                 source,  # *args
                 self._weights,  # *args
                 size,  # *args
                 dtype=np.float64,
                 chunks=chunks,
@@ -127,21 +159,23 @@
             out = self._regrid(source, self._weights, size)
         else:
             raise TypeError(
                 "Expected dask.array.Array or numpy.ndarray. Received: "
                 f"{type(source).__name__}"
             )
 
+        # E.g.: sizes of ("time", "layer") + ("y", "x")
+        out_shape = first_dims_shape + self._target.shape
         return out.reshape(out_shape)
 
     def regrid_dataarray(self, source: xr.DataArray, source_dims: Tuple[str]):
         # Do not set vectorize=True: numba will run the for loop more
         # efficiently, and guarantees a single large allocation.
         out = xr.apply_ufunc(
-            self.regrid_array,
+            self._regrid_array,
             source,
             input_core_dims=[source_dims],
             exclude_dims=set(source_dims),
             output_core_dims=[self._target.dims],
             dask="allowed",
             keep_attrs=True,
             output_dtypes=[source.dtype],
@@ -155,26 +189,38 @@
 
         Automatically regrids over additional dimensions (e.g. time).
 
         Supports lazy evaluation for dask arrays inside the DataArray.
 
         Parameters
         ----------
-        object: UgridDataArray
+        object: UgridDataArray or xarray.DataArray
 
         Returns
         -------
-        regridded: UgridDataArray
+        regridded: UgridDataArray or xarray.DataArray
         """
-        source_dims = (object.ugrid.grid.face_dimension,)
-        regridded = self.regrid_dataarray(object.ugrid.obj, source_dims)
-        return UgridDataArray(
-            regridded,
-            self._target.ugrid_topology,
-        )
+
+        if type(self._target) is StructuredGrid2d:
+            source_dims = ("y", "x")
+            regridded = self.regrid_dataarray(object, source_dims)
+            regridded = regridded.assign_coords(
+                coords={
+                    "y": np.flip(self._target.ybounds.midpoints),
+                    "x": self._target.xbounds.midpoints,
+                }
+            )
+            return regridded
+        else:
+            source_dims = (object.ugrid.grid.face_dimension,)
+            regridded = self.regrid_dataarray(object.ugrid.obj, source_dims)
+            return UgridDataArray(
+                regridded,
+                self._target.ugrid_topology,
+            )
 
     def to_dataset(self) -> xr.Dataset:
         """
         Store the computed weights and target in a dataset for re-use.
         """
         ds = xr.Dataset(
             {f"__regrid_{k}": v for k, v in zip(self._weights._fields, self._weights)}
@@ -239,14 +285,15 @@
     ----------
     source: Ugrid2d, UgridDataArray
     target: Ugrid2d, UgridDataArray
     weights: Optional[WeightMatrixCOO]
     """
 
     def _compute_weights(self, source, target):
+        source, target = convert_to_match(source, target)
         source_index, target_index, weight_values = source.locate_centroids(target)
         self._weights = weight_matrix_coo(source_index, target_index, weight_values)
         return
 
     @staticmethod
     @numba.njit(parallel=True, cache=True)
     def _regrid(source: FloatArray, A: WeightMatrixCOO, size: int):
@@ -274,14 +321,15 @@
     @classmethod
     def _weights_from_dataset(cls, dataset: xr.Dataset) -> WeightMatrixCOO:
         return cls._coo_from_dataset(dataset)
 
 
 class BaseOverlapRegridder(BaseRegridder, abc.ABC):
     def _compute_weights(self, source, target, relative: bool) -> None:
+        source, target = convert_to_match(source, target)
         source_index, target_index, weight_values = source.overlap(
             target, relative=relative
         )
         self._weights = weight_matrix_csr(source_index, target_index, weight_values)
         return
 
     @property
@@ -435,15 +483,19 @@
     ):
         super().__init__(source, target)
         # Since the weights for a target face sum up to 1.0, a weight mean is
         # appropriate, and takes care of NaN values in the source data.
         self._setup_regrid("mean")
 
     def _compute_weights(self, source, target):
-        source_index, target_index, weights = source.barycentric(target)
+        source, target = convert_to_match(source, target)
+        if type(source) == StructuredGrid2d:
+            source_index, target_index, weights = source.linear_weights(target)
+        else:
+            source_index, target_index, weights = source.barycentric(target)
         self._weights = weight_matrix_csr(source_index, target_index, weights)
         return
 
     @property
     def weights(self):
         return self._weights
```

### Comparing `xugrid-0.4.0/xugrid/regrid/unstructured.py` & `xugrid-0.5.0/xugrid/regrid/unstructured.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from xugrid.constants import FloatDType
 from xugrid.ugrid import voronoi
 from xugrid.ugrid.ugrid2d import Ugrid2d
 
 
 class UnstructuredGrid2d:
     """
+    Stores only the grid topology.
+
     e.g. face -> face
 
     Parameters
     ----------
     grid: Ugrid2d
     """
 
@@ -23,14 +25,18 @@
         else:
             options = {"Ugrid2d", "UgridDataArray", "UgridDataset"}
             raise TypeError(
                 f"Expected one of {options}, received: {type(obj).__name__}"
             )
 
     @property
+    def ndim(self):
+        return 1
+
+    @property
     def dims(self):
         return (self.ugrid_topology.face_dimension,)
 
     @property
     def shape(self):
         return (self.ugrid_topology.n_face,)
 
@@ -38,19 +44,34 @@
     def size(self):
         return self.ugrid_topology.n_face
 
     @property
     def area(self):
         return self.ugrid_topology.area
 
+    def convert_to(self, matched_type):
+        if type(self) == matched_type:
+            return self
+        else:
+            TypeError(f"Cannot convert UnstructuredGrid2d to {matched_type.__name__}")
+
     def overlap(self, other, relative: bool):
         """
         Parameters
         ----------
         other: UnstructuredGrid2d
+        relative: bool
+            Whether to divide by the original area. Used for e.g.
+            first-order-conservative methods.
+
+        Returns
+        -------
+        source_index: 1d np.ndarray of int
+        target_index: 1d np.ndarray of int
+        weights: 1d np.ndarray of float
         """
         (
             target_index,
             source_index,
             weights,
         ) = self.ugrid_topology.celltree.intersect_faces(
             vertices=other.ugrid_topology.node_coordinates,
```

### Comparing `xugrid-0.4.0/xugrid/regrid/weight_matrix.py` & `xugrid-0.5.0/xugrid/regrid/weight_matrix.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/ugrid/connectivity.py` & `xugrid-0.5.0/xugrid/ugrid/connectivity.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/ugrid/conventions.py` & `xugrid-0.5.0/xugrid/ugrid/conventions.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/ugrid/interpolate.py` & `xugrid-0.5.0/xugrid/ugrid/interpolate.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/ugrid/partitioning.py` & `xugrid-0.5.0/xugrid/ugrid/partitioning.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/ugrid/snapping.py` & `xugrid-0.5.0/xugrid/ugrid/snapping.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/ugrid/ugrid1d.py` & `xugrid-0.5.0/xugrid/ugrid/ugrid1d.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/ugrid/ugrid2d.py` & `xugrid-0.5.0/xugrid/ugrid/ugrid2d.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/ugrid/ugridbase.py` & `xugrid-0.5.0/xugrid/ugrid/ugridbase.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid/ugrid/voronoi.py` & `xugrid-0.5.0/xugrid/ugrid/voronoi.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.4.0/xugrid.egg-info/PKG-INFO` & `xugrid-0.5.0/xugrid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xugrid
-Version: 0.4.0
+Version: 0.5.0
 Summary: Xarray extension for unstructured grids
 Maintainer-email: Huite Bootsma <huite.bootsma@deltares.nl>
 License: MIT
 Project-URL: Home, https://github.com/deltares/xugrid
 Project-URL: Code, https://github.com/deltares/xugrid
 Project-URL: Issues, https://github.com/deltares/xugrid/issues
 Keywords: mesh,ugrid,unstructured grid,xarray
```

### Comparing `xugrid-0.4.0/xugrid.egg-info/SOURCES.txt` & `xugrid-0.5.0/xugrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

