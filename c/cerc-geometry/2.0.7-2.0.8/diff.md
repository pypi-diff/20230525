# Comparing `tmp/cerc-geometry-2.0.7.tar.gz` & `tmp/cerc-geometry-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/peteryefi/Desktop/dompark/geometry/dist/.tmp-8yr57ewh/cerc-geometry-2.0.7.tar", last modified: Thu May 25 00:09:17 2023, max compression
+gzip compressed data, was "/Users/peteryefi/Desktop/dompark/geometry/dist/.tmp-erilokke/cerc-geometry-2.0.8.tar", last modified: Thu May 25 00:22:27 2023, max compression
```

## Comparing `cerc-geometry-2.0.7.tar` & `cerc-geometry-2.0.8.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:09:17.918547 cerc-geometry-2.0.7/
--rw-rw-rw-   0 peteryefi   (501) staff       (20)     7431 2023-05-11 00:53:33.000000 cerc-geometry-2.0.7/LICENSE.md
--rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-25 00:09:17.917677 cerc-geometry-2.0.7/PKG-INFO
--rw-r--r--   0 peteryefi   (501) staff       (20)      522 2023-05-12 17:30:08.000000 cerc-geometry-2.0.7/README.md
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:09:17.906604 cerc-geometry-2.0.7/cerc_geometry.egg-info/
--rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-25 00:09:17.000000 cerc-geometry-2.0.7/cerc_geometry.egg-info/PKG-INFO
--rw-r--r--   0 peteryefi   (501) staff       (20)      535 2023-05-25 00:09:17.000000 cerc-geometry-2.0.7/cerc_geometry.egg-info/SOURCES.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)        1 2023-05-25 00:09:17.000000 cerc-geometry-2.0.7/cerc_geometry.egg-info/dependency_links.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)       48 2023-05-25 00:09:17.000000 cerc-geometry-2.0.7/cerc_geometry.egg-info/requires.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)        9 2023-05-25 00:09:17.000000 cerc-geometry-2.0.7/cerc_geometry.egg-info/top_level.txt
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:09:17.912812 cerc-geometry-2.0.7/geometry/
--rw-r--r--   0 peteryefi   (501) staff       (20)      200 2023-05-19 00:02:34.000000 cerc-geometry-2.0.7/geometry/__init__.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     5690 2023-05-23 00:07:56.000000 cerc-geometry-2.0.7/geometry/helper.py
--rw-r--r--   0 peteryefi   (501) staff       (20)    11128 2023-05-24 23:38:41.000000 cerc-geometry-2.0.7/geometry/library.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      574 2023-05-18 23:39:06.000000 cerc-geometry-2.0.7/geometry/location.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      707 2023-05-18 23:38:20.000000 cerc-geometry-2.0.7/geometry/map_point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     2168 2023-05-15 23:21:05.000000 cerc-geometry-2.0.7/geometry/plane.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1002 2023-05-15 23:21:05.000000 cerc-geometry-2.0.7/geometry/point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)    14604 2023-05-16 00:05:51.000000 cerc-geometry-2.0.7/geometry/polygon.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     6590 2023-05-15 23:21:05.000000 cerc-geometry-2.0.7/geometry/polyhedron.py
--rw-r--r--   0 peteryefi   (501) staff       (20)       99 2023-05-15 23:40:38.000000 cerc-geometry-2.0.7/pyproject.toml
--rw-r--r--   0 peteryefi   (501) staff       (20)       37 2023-05-18 23:51:47.000000 cerc-geometry-2.0.7/requirements.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)       38 2023-05-25 00:09:17.918856 cerc-geometry-2.0.7/setup.cfg
--rw-r--r--   0 peteryefi   (501) staff       (20)     1385 2023-05-25 00:04:31.000000 cerc-geometry-2.0.7/setup.py
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:09:17.916952 cerc-geometry-2.0.7/tests/
--rw-r--r--   0 peteryefi   (501) staff       (20)     1961 2023-05-16 00:05:50.000000 cerc-geometry-2.0.7/tests/test_helper.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      736 2023-05-16 00:05:50.000000 cerc-geometry-2.0.7/tests/test_plane.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      842 2023-05-16 00:05:50.000000 cerc-geometry-2.0.7/tests/test_point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1513 2023-05-16 00:05:50.000000 cerc-geometry-2.0.7/tests/test_polygon.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1076 2023-05-16 00:05:50.000000 cerc-geometry-2.0.7/tests/test_polyhedron.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:22:27.591605 cerc-geometry-2.0.8/
+-rw-rw-rw-   0 peteryefi   (501) staff       (20)     7431 2023-05-11 00:53:33.000000 cerc-geometry-2.0.8/LICENSE.md
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-25 00:22:27.591102 cerc-geometry-2.0.8/PKG-INFO
+-rw-r--r--   0 peteryefi   (501) staff       (20)      522 2023-05-12 17:30:08.000000 cerc-geometry-2.0.8/README.md
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:22:27.499414 cerc-geometry-2.0.8/cerc_geometry.egg-info/
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-25 00:22:27.000000 cerc-geometry-2.0.8/cerc_geometry.egg-info/PKG-INFO
+-rw-r--r--   0 peteryefi   (501) staff       (20)      577 2023-05-25 00:22:27.000000 cerc-geometry-2.0.8/cerc_geometry.egg-info/SOURCES.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)        1 2023-05-25 00:22:27.000000 cerc-geometry-2.0.8/cerc_geometry.egg-info/dependency_links.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)       48 2023-05-25 00:22:27.000000 cerc-geometry-2.0.8/cerc_geometry.egg-info/requires.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)        9 2023-05-25 00:22:27.000000 cerc-geometry-2.0.8/cerc_geometry.egg-info/top_level.txt
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:22:27.510610 cerc-geometry-2.0.8/geometry/
+-rw-r--r--   0 peteryefi   (501) staff       (20)      200 2023-05-19 00:02:34.000000 cerc-geometry-2.0.8/geometry/__init__.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:22:27.490342 cerc-geometry-2.0.8/geometry/data/
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:22:27.513284 cerc-geometry-2.0.8/geometry/data/geolocation/
+-rw-r--r--   0 peteryefi   (501) staff       (20)  6284352 2023-05-12 21:46:09.000000 cerc-geometry-2.0.8/geometry/data/geolocation/cities15000.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)     5690 2023-05-23 00:07:56.000000 cerc-geometry-2.0.8/geometry/helper.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)    11128 2023-05-24 23:38:41.000000 cerc-geometry-2.0.8/geometry/library.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      574 2023-05-18 23:39:06.000000 cerc-geometry-2.0.8/geometry/location.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      707 2023-05-18 23:38:20.000000 cerc-geometry-2.0.8/geometry/map_point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     2168 2023-05-15 23:21:05.000000 cerc-geometry-2.0.8/geometry/plane.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1002 2023-05-15 23:21:05.000000 cerc-geometry-2.0.8/geometry/point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)    14604 2023-05-16 00:05:51.000000 cerc-geometry-2.0.8/geometry/polygon.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     6590 2023-05-15 23:21:05.000000 cerc-geometry-2.0.8/geometry/polyhedron.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)       99 2023-05-15 23:40:38.000000 cerc-geometry-2.0.8/pyproject.toml
+-rw-r--r--   0 peteryefi   (501) staff       (20)       37 2023-05-18 23:51:47.000000 cerc-geometry-2.0.8/requirements.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)       38 2023-05-25 00:22:27.591959 cerc-geometry-2.0.8/setup.cfg
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1400 2023-05-25 00:22:04.000000 cerc-geometry-2.0.8/setup.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:22:27.590306 cerc-geometry-2.0.8/tests/
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1961 2023-05-16 00:05:50.000000 cerc-geometry-2.0.8/tests/test_helper.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      736 2023-05-16 00:05:50.000000 cerc-geometry-2.0.8/tests/test_plane.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      842 2023-05-16 00:05:50.000000 cerc-geometry-2.0.8/tests/test_point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1513 2023-05-16 00:05:50.000000 cerc-geometry-2.0.8/tests/test_polygon.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1076 2023-05-16 00:05:50.000000 cerc-geometry-2.0.8/tests/test_polyhedron.py
```

### Comparing `cerc-geometry-2.0.7/LICENSE.md` & `cerc-geometry-2.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.7/PKG-INFO` & `cerc-geometry-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-geometry
-Version: 2.0.7
+Version: 2.0.8
 Summary: CERC Geometry Library with different modules to manipulate geometric objects
 Home-page: https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Author: CERC
 Author-email:  cerc@concordia.ca
 Project-URL: Repository, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Project-URL: Bug Tracker, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cerc-geometry-2.0.7/README.md` & `cerc-geometry-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.7/cerc_geometry.egg-info/PKG-INFO` & `cerc-geometry-2.0.8/cerc_geometry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-geometry
-Version: 2.0.7
+Version: 2.0.8
 Summary: CERC Geometry Library with different modules to manipulate geometric objects
 Home-page: https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Author: CERC
 Author-email:  cerc@concordia.ca
 Project-URL: Repository, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Project-URL: Bug Tracker, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cerc-geometry-2.0.7/cerc_geometry.egg-info/SOURCES.txt` & `cerc-geometry-2.0.8/cerc_geometry.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -13,12 +13,13 @@
 geometry/library.py
 geometry/location.py
 geometry/map_point.py
 geometry/plane.py
 geometry/point.py
 geometry/polygon.py
 geometry/polyhedron.py
+geometry/data/geolocation/cities15000.txt
 tests/test_helper.py
 tests/test_plane.py
 tests/test_point.py
 tests/test_polygon.py
 tests/test_polyhedron.py
```

### Comparing `cerc-geometry-2.0.7/geometry/helper.py` & `cerc-geometry-2.0.8/geometry/helper.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.7/geometry/library.py` & `cerc-geometry-2.0.8/geometry/library.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.7/geometry/location.py` & `cerc-geometry-2.0.8/geometry/location.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.7/geometry/map_point.py` & `cerc-geometry-2.0.8/geometry/map_point.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.7/geometry/plane.py` & `cerc-geometry-2.0.8/geometry/plane.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.7/geometry/point.py` & `cerc-geometry-2.0.8/geometry/point.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.7/geometry/polygon.py` & `cerc-geometry-2.0.8/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.7/geometry/polyhedron.py` & `cerc-geometry-2.0.8/geometry/polyhedron.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.7/tests/test_helper.py` & `cerc-geometry-2.0.8/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.7/tests/test_plane.py` & `cerc-geometry-2.0.8/tests/test_plane.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.7/tests/test_point.py` & `cerc-geometry-2.0.8/tests/test_point.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.7/tests/test_polygon.py` & `cerc-geometry-2.0.8/tests/test_polygon.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.7/tests/test_polyhedron.py` & `cerc-geometry-2.0.8/tests/test_polyhedron.py`

 * *Files identical despite different names*

