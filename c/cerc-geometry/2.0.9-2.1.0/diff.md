# Comparing `tmp/cerc-geometry-2.0.9.tar.gz` & `tmp/cerc-geometry-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/peteryefi/Desktop/dompark/geometry/dist/.tmp-m3eeucuj/cerc-geometry-2.0.9.tar", last modified: Thu May 25 00:45:38 2023, max compression
+gzip compressed data, was "/Users/peteryefi/Desktop/dompark/geometry/dist/.tmp-g0rha1bz/cerc-geometry-2.1.0.tar", last modified: Thu May 25 00:54:03 2023, max compression
```

## Comparing `cerc-geometry-2.0.9.tar` & `cerc-geometry-2.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:45:38.144760 cerc-geometry-2.0.9/
--rw-rw-rw-   0 peteryefi   (501) staff       (20)     7431 2023-05-11 00:53:33.000000 cerc-geometry-2.0.9/LICENSE.md
--rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-25 00:45:38.144401 cerc-geometry-2.0.9/PKG-INFO
--rw-r--r--   0 peteryefi   (501) staff       (20)      522 2023-05-12 17:30:08.000000 cerc-geometry-2.0.9/README.md
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:45:38.016470 cerc-geometry-2.0.9/cerc_geometry.egg-info/
--rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-25 00:45:38.000000 cerc-geometry-2.0.9/cerc_geometry.egg-info/PKG-INFO
--rw-r--r--   0 peteryefi   (501) staff       (20)      577 2023-05-25 00:45:38.000000 cerc-geometry-2.0.9/cerc_geometry.egg-info/SOURCES.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)        1 2023-05-25 00:45:38.000000 cerc-geometry-2.0.9/cerc_geometry.egg-info/dependency_links.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)       48 2023-05-25 00:45:38.000000 cerc-geometry-2.0.9/cerc_geometry.egg-info/requires.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)        9 2023-05-25 00:45:38.000000 cerc-geometry-2.0.9/cerc_geometry.egg-info/top_level.txt
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:45:38.023925 cerc-geometry-2.0.9/geometry/
--rw-r--r--   0 peteryefi   (501) staff       (20)      200 2023-05-19 00:02:34.000000 cerc-geometry-2.0.9/geometry/__init__.py
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:45:38.012417 cerc-geometry-2.0.9/geometry/data/
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:45:38.024698 cerc-geometry-2.0.9/geometry/data/geolocation/
--rw-r--r--   0 peteryefi   (501) staff       (20)  6284352 2023-05-12 21:46:09.000000 cerc-geometry-2.0.9/geometry/data/geolocation/cities15000.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)     5690 2023-05-23 00:07:56.000000 cerc-geometry-2.0.9/geometry/helper.py
--rw-r--r--   0 peteryefi   (501) staff       (20)    11128 2023-05-24 23:38:41.000000 cerc-geometry-2.0.9/geometry/library.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      574 2023-05-18 23:39:06.000000 cerc-geometry-2.0.9/geometry/location.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      707 2023-05-18 23:38:20.000000 cerc-geometry-2.0.9/geometry/map_point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     2168 2023-05-15 23:21:05.000000 cerc-geometry-2.0.9/geometry/plane.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1002 2023-05-15 23:21:05.000000 cerc-geometry-2.0.9/geometry/point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)    14604 2023-05-16 00:05:51.000000 cerc-geometry-2.0.9/geometry/polygon.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     6590 2023-05-15 23:21:05.000000 cerc-geometry-2.0.9/geometry/polyhedron.py
--rw-r--r--   0 peteryefi   (501) staff       (20)       99 2023-05-15 23:40:38.000000 cerc-geometry-2.0.9/pyproject.toml
--rw-r--r--   0 peteryefi   (501) staff       (20)       37 2023-05-18 23:51:47.000000 cerc-geometry-2.0.9/requirements.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)       38 2023-05-25 00:45:38.145019 cerc-geometry-2.0.9/setup.cfg
--rw-r--r--   0 peteryefi   (501) staff       (20)     1417 2023-05-25 00:43:15.000000 cerc-geometry-2.0.9/setup.py
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:45:38.143649 cerc-geometry-2.0.9/tests/
--rw-r--r--   0 peteryefi   (501) staff       (20)     1961 2023-05-16 00:05:50.000000 cerc-geometry-2.0.9/tests/test_helper.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      736 2023-05-16 00:05:50.000000 cerc-geometry-2.0.9/tests/test_plane.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      842 2023-05-16 00:05:50.000000 cerc-geometry-2.0.9/tests/test_point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1513 2023-05-16 00:05:50.000000 cerc-geometry-2.0.9/tests/test_polygon.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1076 2023-05-16 00:05:50.000000 cerc-geometry-2.0.9/tests/test_polyhedron.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:54:03.681570 cerc-geometry-2.1.0/
+-rw-rw-rw-   0 peteryefi   (501) staff       (20)     7431 2023-05-11 00:53:33.000000 cerc-geometry-2.1.0/LICENSE.md
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-25 00:54:03.681228 cerc-geometry-2.1.0/PKG-INFO
+-rw-r--r--   0 peteryefi   (501) staff       (20)      522 2023-05-12 17:30:08.000000 cerc-geometry-2.1.0/README.md
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:54:03.639041 cerc-geometry-2.1.0/cerc_geometry.egg-info/
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-25 00:54:03.000000 cerc-geometry-2.1.0/cerc_geometry.egg-info/PKG-INFO
+-rw-r--r--   0 peteryefi   (501) staff       (20)      577 2023-05-25 00:54:03.000000 cerc-geometry-2.1.0/cerc_geometry.egg-info/SOURCES.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)        1 2023-05-25 00:54:03.000000 cerc-geometry-2.1.0/cerc_geometry.egg-info/dependency_links.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)       48 2023-05-25 00:54:03.000000 cerc-geometry-2.1.0/cerc_geometry.egg-info/requires.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)        9 2023-05-25 00:54:03.000000 cerc-geometry-2.1.0/cerc_geometry.egg-info/top_level.txt
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:54:03.645038 cerc-geometry-2.1.0/geometry/
+-rw-r--r--   0 peteryefi   (501) staff       (20)      200 2023-05-19 00:02:34.000000 cerc-geometry-2.1.0/geometry/__init__.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:54:03.635628 cerc-geometry-2.1.0/geometry/data/
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:54:03.645706 cerc-geometry-2.1.0/geometry/data/geolocation/
+-rw-r--r--   0 peteryefi   (501) staff       (20)  6284352 2023-05-12 21:46:09.000000 cerc-geometry-2.1.0/geometry/data/geolocation/cities15000.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)     5690 2023-05-23 00:07:56.000000 cerc-geometry-2.1.0/geometry/helper.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)    11128 2023-05-24 23:38:41.000000 cerc-geometry-2.1.0/geometry/library.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      574 2023-05-18 23:39:06.000000 cerc-geometry-2.1.0/geometry/location.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      707 2023-05-18 23:38:20.000000 cerc-geometry-2.1.0/geometry/map_point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     2168 2023-05-15 23:21:05.000000 cerc-geometry-2.1.0/geometry/plane.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1002 2023-05-15 23:21:05.000000 cerc-geometry-2.1.0/geometry/point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)    14604 2023-05-16 00:05:51.000000 cerc-geometry-2.1.0/geometry/polygon.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     6590 2023-05-15 23:21:05.000000 cerc-geometry-2.1.0/geometry/polyhedron.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)       99 2023-05-15 23:40:38.000000 cerc-geometry-2.1.0/pyproject.toml
+-rw-r--r--   0 peteryefi   (501) staff       (20)       37 2023-05-18 23:51:47.000000 cerc-geometry-2.1.0/requirements.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)       38 2023-05-25 00:54:03.681696 cerc-geometry-2.1.0/setup.cfg
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1446 2023-05-25 00:53:17.000000 cerc-geometry-2.1.0/setup.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-25 00:54:03.680566 cerc-geometry-2.1.0/tests/
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1961 2023-05-16 00:05:50.000000 cerc-geometry-2.1.0/tests/test_helper.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      736 2023-05-16 00:05:50.000000 cerc-geometry-2.1.0/tests/test_plane.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      842 2023-05-16 00:05:50.000000 cerc-geometry-2.1.0/tests/test_point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1513 2023-05-16 00:05:50.000000 cerc-geometry-2.1.0/tests/test_polygon.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1076 2023-05-16 00:05:50.000000 cerc-geometry-2.1.0/tests/test_polyhedron.py
```

### Comparing `cerc-geometry-2.0.9/LICENSE.md` & `cerc-geometry-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.9/PKG-INFO` & `cerc-geometry-2.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-geometry
-Version: 2.0.9
+Version: 2.1.0
 Summary: CERC Geometry Library with different modules to manipulate geometric objects
 Home-page: https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Author: CERC
 Author-email:  cerc@concordia.ca
 Project-URL: Repository, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Project-URL: Bug Tracker, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cerc-geometry-2.0.9/README.md` & `cerc-geometry-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.9/cerc_geometry.egg-info/PKG-INFO` & `cerc-geometry-2.1.0/cerc_geometry.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-geometry
-Version: 2.0.9
+Version: 2.1.0
 Summary: CERC Geometry Library with different modules to manipulate geometric objects
 Home-page: https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Author: CERC
 Author-email:  cerc@concordia.ca
 Project-URL: Repository, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Project-URL: Bug Tracker, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cerc-geometry-2.0.9/cerc_geometry.egg-info/SOURCES.txt` & `cerc-geometry-2.1.0/cerc_geometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.9/geometry/data/geolocation/cities15000.txt` & `cerc-geometry-2.1.0/geometry/data/geolocation/cities15000.txt`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.9/geometry/helper.py` & `cerc-geometry-2.1.0/geometry/helper.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.9/geometry/library.py` & `cerc-geometry-2.1.0/geometry/library.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.9/geometry/location.py` & `cerc-geometry-2.1.0/geometry/location.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.9/geometry/map_point.py` & `cerc-geometry-2.1.0/geometry/map_point.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.9/geometry/plane.py` & `cerc-geometry-2.1.0/geometry/plane.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.9/geometry/point.py` & `cerc-geometry-2.1.0/geometry/point.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.9/geometry/polygon.py` & `cerc-geometry-2.1.0/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.9/geometry/polyhedron.py` & `cerc-geometry-2.1.0/geometry/polyhedron.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.9/setup.py` & `cerc-geometry-2.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     for requirement
     in pkg_resources.parse_requirements(r)
   ]
 install_requires.append('setuptools')
 
 setuptools.setup(
   name="cerc-geometry",
-  version="2.0.9",
+  version="2.1.0",
   author="CERC",
   author_email=" cerc@concordia.ca",
   description="CERC Geometry Library with different modules to manipulate geometric objects",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry",
   project_urls={
@@ -31,12 +31,13 @@
     "License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)",
     "Operating System :: OS Independent",
   ],
   data_files=[
     ('geometry', glob.glob('requirements.txt')),
     ('geometry/data/geolocation', glob.glob('geometry/data/geolocation/*.txt'))
   ],
+  include_package_data=True,
   packages=['geometry', 'geometry.data'],
   setup_requires=install_requires,
   install_requires=install_requires,
   python_requires=">=3.6"
 )
```

### Comparing `cerc-geometry-2.0.9/tests/test_helper.py` & `cerc-geometry-2.1.0/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.9/tests/test_plane.py` & `cerc-geometry-2.1.0/tests/test_plane.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.9/tests/test_point.py` & `cerc-geometry-2.1.0/tests/test_point.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.9/tests/test_polygon.py` & `cerc-geometry-2.1.0/tests/test_polygon.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.0.9/tests/test_polyhedron.py` & `cerc-geometry-2.1.0/tests/test_polyhedron.py`

 * *Files identical despite different names*

