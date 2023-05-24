# Comparing `tmp/cerc-geometry-2.0.4.tar.gz` & `tmp/cerc-geometry-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/peteryefi/Desktop/dompark/geometry/dist/.tmp-ra6v6dlx/cerc-geometry-2.0.4.tar", last modified: Wed May 24 02:11:42 2023, max compression
+gzip compressed data, was "/Users/peteryefi/Desktop/dompark/geometry/dist/.tmp-_0646brc/cerc-geometry-2.0.5.tar", last modified: Wed May 24 23:45:11 2023, max compression
```

## Comparing `cerc-geometry-2.0.4.tar` & `cerc-geometry-2.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-24 02:11:42.577959 cerc-geometry-2.0.4/
--rw-rw-rw-   0 peteryefi   (501) staff       (20)     7431 2023-05-11 00:53:33.000000 cerc-geometry-2.0.4/LICENSE.md
--rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-24 02:11:42.577591 cerc-geometry-2.0.4/PKG-INFO
--rw-r--r--   0 peteryefi   (501) staff       (20)      522 2023-05-12 17:30:08.000000 cerc-geometry-2.0.4/README.md
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-24 02:11:42.516454 cerc-geometry-2.0.4/cerc_geometry.egg-info/
--rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-24 02:11:42.000000 cerc-geometry-2.0.4/cerc_geometry.egg-info/PKG-INFO
--rw-r--r--   0 peteryefi   (501) staff       (20)      577 2023-05-24 02:11:42.000000 cerc-geometry-2.0.4/cerc_geometry.egg-info/SOURCES.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)        1 2023-05-24 02:11:42.000000 cerc-geometry-2.0.4/cerc_geometry.egg-info/dependency_links.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)       48 2023-05-24 02:11:42.000000 cerc-geometry-2.0.4/cerc_geometry.egg-info/requires.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)        9 2023-05-24 02:11:42.000000 cerc-geometry-2.0.4/cerc_geometry.egg-info/top_level.txt
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-24 02:11:42.525533 cerc-geometry-2.0.4/geometry/
--rw-r--r--   0 peteryefi   (501) staff       (20)      200 2023-05-19 00:02:34.000000 cerc-geometry-2.0.4/geometry/__init__.py
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-24 02:11:42.510931 cerc-geometry-2.0.4/geometry/data/
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-24 02:11:42.526426 cerc-geometry-2.0.4/geometry/data/geolocation/
--rw-r--r--   0 peteryefi   (501) staff       (20)  6284352 2023-05-12 21:46:09.000000 cerc-geometry-2.0.4/geometry/data/geolocation/cities15000.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)     5690 2023-05-23 00:07:56.000000 cerc-geometry-2.0.4/geometry/helper.py
--rw-r--r--   0 peteryefi   (501) staff       (20)    11128 2023-05-24 02:09:54.000000 cerc-geometry-2.0.4/geometry/library.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      574 2023-05-18 23:39:06.000000 cerc-geometry-2.0.4/geometry/location.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      707 2023-05-18 23:38:20.000000 cerc-geometry-2.0.4/geometry/map_point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     2168 2023-05-15 23:21:05.000000 cerc-geometry-2.0.4/geometry/plane.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1002 2023-05-15 23:21:05.000000 cerc-geometry-2.0.4/geometry/point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)    14604 2023-05-16 00:05:51.000000 cerc-geometry-2.0.4/geometry/polygon.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     6590 2023-05-15 23:21:05.000000 cerc-geometry-2.0.4/geometry/polyhedron.py
--rw-r--r--   0 peteryefi   (501) staff       (20)       99 2023-05-15 23:40:38.000000 cerc-geometry-2.0.4/pyproject.toml
--rw-r--r--   0 peteryefi   (501) staff       (20)       37 2023-05-18 23:51:47.000000 cerc-geometry-2.0.4/requirements.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)       38 2023-05-24 02:11:42.578081 cerc-geometry-2.0.4/setup.cfg
--rw-r--r--   0 peteryefi   (501) staff       (20)     1391 2023-05-24 02:11:04.000000 cerc-geometry-2.0.4/setup.py
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-24 02:11:42.576886 cerc-geometry-2.0.4/tests/
--rw-r--r--   0 peteryefi   (501) staff       (20)     1961 2023-05-16 00:05:50.000000 cerc-geometry-2.0.4/tests/test_helper.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      736 2023-05-16 00:05:50.000000 cerc-geometry-2.0.4/tests/test_plane.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      842 2023-05-16 00:05:50.000000 cerc-geometry-2.0.4/tests/test_point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1513 2023-05-16 00:05:50.000000 cerc-geometry-2.0.4/tests/test_polygon.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1076 2023-05-16 00:05:50.000000 cerc-geometry-2.0.4/tests/test_polyhedron.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-24 23:45:11.634207 cerc-geometry-2.0.5/
+-rw-rw-rw-   0 peteryefi   (501) staff       (20)     7431 2023-05-11 00:53:33.000000 cerc-geometry-2.0.5/LICENSE.md
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-24 23:45:11.633776 cerc-geometry-2.0.5/PKG-INFO
+-rw-r--r--   0 peteryefi   (501) staff       (20)      522 2023-05-12 17:30:08.000000 cerc-geometry-2.0.5/README.md
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-24 23:45:11.591169 cerc-geometry-2.0.5/cerc_geometry.egg-info/
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-24 23:45:11.000000 cerc-geometry-2.0.5/cerc_geometry.egg-info/PKG-INFO
+-rw-r--r--   0 peteryefi   (501) staff       (20)      577 2023-05-24 23:45:11.000000 cerc-geometry-2.0.5/cerc_geometry.egg-info/SOURCES.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)        1 2023-05-24 23:45:11.000000 cerc-geometry-2.0.5/cerc_geometry.egg-info/dependency_links.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)       48 2023-05-24 23:45:11.000000 cerc-geometry-2.0.5/cerc_geometry.egg-info/requires.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)        9 2023-05-24 23:45:11.000000 cerc-geometry-2.0.5/cerc_geometry.egg-info/top_level.txt
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-24 23:45:11.597846 cerc-geometry-2.0.5/geometry/
+-rw-r--r--   0 peteryefi   (501) staff       (20)      200 2023-05-19 00:02:34.000000 cerc-geometry-2.0.5/geometry/__init__.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-24 23:45:11.585605 cerc-geometry-2.0.5/geometry/data/
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-24 23:45:11.598512 cerc-geometry-2.0.5/geometry/data/geolocation/
+-rw-r--r--   0 peteryefi   (501) staff       (20)  6284352 2023-05-12 21:46:09.000000 cerc-geometry-2.0.5/geometry/data/geolocation/cities15000.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)     5690 2023-05-23 00:07:56.000000 cerc-geometry-2.0.5/geometry/helper.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)    11128 2023-05-24 23:38:41.000000 cerc-geometry-2.0.5/geometry/library.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      574 2023-05-18 23:39:06.000000 cerc-geometry-2.0.5/geometry/location.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      707 2023-05-18 23:38:20.000000 cerc-geometry-2.0.5/geometry/map_point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     2168 2023-05-15 23:21:05.000000 cerc-geometry-2.0.5/geometry/plane.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1002 2023-05-15 23:21:05.000000 cerc-geometry-2.0.5/geometry/point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)    14604 2023-05-16 00:05:51.000000 cerc-geometry-2.0.5/geometry/polygon.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     6590 2023-05-15 23:21:05.000000 cerc-geometry-2.0.5/geometry/polyhedron.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)       99 2023-05-15 23:40:38.000000 cerc-geometry-2.0.5/pyproject.toml
+-rw-r--r--   0 peteryefi   (501) staff       (20)       37 2023-05-18 23:51:47.000000 cerc-geometry-2.0.5/requirements.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)       38 2023-05-24 23:45:11.634338 cerc-geometry-2.0.5/setup.cfg
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1408 2023-05-24 23:42:52.000000 cerc-geometry-2.0.5/setup.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-24 23:45:11.633061 cerc-geometry-2.0.5/tests/
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1961 2023-05-16 00:05:50.000000 cerc-geometry-2.0.5/tests/test_helper.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      736 2023-05-16 00:05:50.000000 cerc-geometry-2.0.5/tests/test_plane.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      842 2023-05-16 00:05:50.000000 cerc-geometry-2.0.5/tests/test_point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1513 2023-05-16 00:05:50.000000 cerc-geometry-2.0.5/tests/test_polygon.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1076 2023-05-16 00:05:50.000000 cerc-geometry-2.0.5/tests/test_polyhedron.py
```

### Comparing `cerc-geometry-2.0.4/LICENSE.md` & `cerc-geometry-2.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.4/PKG-INFO` & `cerc-geometry-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-geometry
-Version: 2.0.4
+Version: 2.0.5
 Summary: CERC Geometry Library with different modules to manipulate geometric objects
 Home-page: https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Author: CERC
 Author-email:  cerc@concordia.ca
 Project-URL: Repository, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Project-URL: Bug Tracker, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cerc-geometry-2.0.4/README.md` & `cerc-geometry-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.4/cerc_geometry.egg-info/PKG-INFO` & `cerc-geometry-2.0.5/cerc_geometry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-geometry
-Version: 2.0.4
+Version: 2.0.5
 Summary: CERC Geometry Library with different modules to manipulate geometric objects
 Home-page: https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Author: CERC
 Author-email:  cerc@concordia.ca
 Project-URL: Repository, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Project-URL: Bug Tracker, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cerc-geometry-2.0.4/cerc_geometry.egg-info/SOURCES.txt` & `cerc-geometry-2.0.5/cerc_geometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.4/geometry/data/geolocation/cities15000.txt` & `cerc-geometry-2.0.5/geometry/data/geolocation/cities15000.txt`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.4/geometry/helper.py` & `cerc-geometry-2.0.5/geometry/helper.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.4/geometry/library.py` & `cerc-geometry-2.0.5/geometry/library.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.4/geometry/location.py` & `cerc-geometry-2.0.5/geometry/location.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.4/geometry/map_point.py` & `cerc-geometry-2.0.5/geometry/map_point.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.4/geometry/plane.py` & `cerc-geometry-2.0.5/geometry/plane.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.4/geometry/point.py` & `cerc-geometry-2.0.5/geometry/point.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.4/geometry/polygon.py` & `cerc-geometry-2.0.5/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.4/geometry/polyhedron.py` & `cerc-geometry-2.0.5/geometry/polyhedron.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.4/setup.py` & `cerc-geometry-2.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     for requirement
     in pkg_resources.parse_requirements(r)
   ]
 install_requires.append('setuptools')
 
 setuptools.setup(
   name="cerc-geometry",
-  version="2.0.4",
+  version="2.0.5",
   author="CERC",
   author_email=" cerc@concordia.ca",
   description="CERC Geometry Library with different modules to manipulate geometric objects",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry",
   project_urls={
@@ -31,12 +31,12 @@
     "License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)",
     "Operating System :: OS Independent",
   ],
   data_files=[
     ('geometry', glob.glob('requirements.txt')),
     ('data/geolocation', glob.glob('geometry/data/geolocation/*.txt'))
   ],
-  packages=['geometry'],
+  packages=['geometry', 'geometry.data'],
   setup_requires=install_requires,
   install_requires=install_requires,
   python_requires=">=3.6"
 )
```

### Comparing `cerc-geometry-2.0.4/tests/test_helper.py` & `cerc-geometry-2.0.5/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.4/tests/test_plane.py` & `cerc-geometry-2.0.5/tests/test_plane.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.4/tests/test_point.py` & `cerc-geometry-2.0.5/tests/test_point.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.4/tests/test_polygon.py` & `cerc-geometry-2.0.5/tests/test_polygon.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.4/tests/test_polyhedron.py` & `cerc-geometry-2.0.5/tests/test_polyhedron.py`

 * *Files identical despite different names*

