# Comparing `tmp/gltf-shapes-0.0.1.tar.gz` & `tmp/gltf-shapes-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gltf-shapes-0.0.1.tar", last modified: Tue May  3 13:44:38 2022, max compression
+gzip compressed data, was "dist/gltf-shapes-0.0.2.tar", last modified: Thu May 25 10:22:09 2023, max compression
```

## Comparing `gltf-shapes-0.0.1.tar` & `gltf-shapes-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2022-05-03 13:44:38.000000 gltf-shapes-0.0.1/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      598 2022-04-07 08:06:31.000000 gltf-shapes-0.0.1/setup.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      399 2022-05-03 13:44:38.000000 gltf-shapes-0.0.1/PKG-INFO
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2022-05-03 13:44:38.000000 gltf-shapes-0.0.1/gltf_shapes.egg-info/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      399 2022-05-03 13:44:38.000000 gltf-shapes-0.0.1/gltf_shapes.egg-info/PKG-INFO
--rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2022-05-03 13:44:38.000000 gltf-shapes-0.0.1/gltf_shapes.egg-info/dependency_links.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       11 2022-05-03 13:44:38.000000 gltf-shapes-0.0.1/gltf_shapes.egg-info/top_level.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       21 2022-05-03 13:44:38.000000 gltf-shapes-0.0.1/gltf_shapes.egg-info/requires.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      278 2022-05-03 13:44:38.000000 gltf-shapes-0.0.1/gltf_shapes.egg-info/SOURCES.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2022-05-03 13:44:38.000000 gltf-shapes-0.0.1/setup.cfg
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2022-05-03 13:44:38.000000 gltf-shapes-0.0.1/gltfshapes/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)        0 2022-04-07 08:04:02.000000 gltf-shapes-0.0.1/gltfshapes/__init__.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     3616 2022-04-07 12:18:21.000000 gltf-shapes-0.0.1/gltfshapes/cube_evenly_sampled.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1129 2022-04-07 12:11:16.000000 gltf-shapes-0.0.1/gltfshapes/linear_samples.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      243 2022-04-07 13:48:34.000000 gltf-shapes-0.0.1/README.md
+drwxr-xr-x   0 craigchristensen   (501) staff       (20)        0 2023-05-25 10:22:09.587933 gltf-shapes-0.0.2/
+-rw-r--r--   0 craigchristensen   (501) staff       (20)      399 2023-05-25 10:22:09.587626 gltf-shapes-0.0.2/PKG-INFO
+-rw-r--r--   0 craigchristensen   (501) staff       (20)      395 2023-05-25 10:19:31.000000 gltf-shapes-0.0.2/README.md
+drwxr-xr-x   0 craigchristensen   (501) staff       (20)        0 2023-05-25 10:22:09.585069 gltf-shapes-0.0.2/gltf_shapes.egg-info/
+-rw-r--r--   0 craigchristensen   (501) staff       (20)      399 2023-05-25 10:22:09.000000 gltf-shapes-0.0.2/gltf_shapes.egg-info/PKG-INFO
+-rw-r--r--   0 craigchristensen   (501) staff       (20)      300 2023-05-25 10:22:09.000000 gltf-shapes-0.0.2/gltf_shapes.egg-info/SOURCES.txt
+-rw-r--r--   0 craigchristensen   (501) staff       (20)        1 2023-05-25 10:22:09.000000 gltf-shapes-0.0.2/gltf_shapes.egg-info/dependency_links.txt
+-rw-r--r--   0 craigchristensen   (501) staff       (20)       21 2023-05-25 10:22:09.000000 gltf-shapes-0.0.2/gltf_shapes.egg-info/requires.txt
+-rw-r--r--   0 craigchristensen   (501) staff       (20)       11 2023-05-25 10:22:09.000000 gltf-shapes-0.0.2/gltf_shapes.egg-info/top_level.txt
+drwxr-xr-x   0 craigchristensen   (501) staff       (20)        0 2023-05-25 10:22:09.587009 gltf-shapes-0.0.2/gltfshapes/
+-rw-r--r--   0 craigchristensen   (501) staff       (20)        0 2023-05-25 10:19:31.000000 gltf-shapes-0.0.2/gltfshapes/__init__.py
+-rw-r--r--   0 craigchristensen   (501) staff       (20)     3616 2023-05-25 10:19:31.000000 gltf-shapes-0.0.2/gltfshapes/cube_evenly_sampled.py
+-rw-r--r--   0 craigchristensen   (501) staff       (20)     1129 2023-05-25 10:19:31.000000 gltf-shapes-0.0.2/gltfshapes/linear_samples.py
+-rw-r--r--   0 craigchristensen   (501) staff       (20)     3346 2023-05-25 10:19:31.000000 gltf-shapes-0.0.2/gltfshapes/surface.py
+-rw-r--r--   0 craigchristensen   (501) staff       (20)       38 2023-05-25 10:22:09.588034 gltf-shapes-0.0.2/setup.cfg
+-rw-r--r--   0 craigchristensen   (501) staff       (20)      598 2023-05-25 10:20:12.000000 gltf-shapes-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gltf-shapes-0.0.1/setup.py` & `gltf-shapes-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 import setuptools
 import os
 
 setuptools.setup(
     name='gltf-shapes',
-    version='0.0.1',
+    version='0.0.2',
     description='Transform numpy arrays and pandas dataframes to 3d exports',
     long_description="""Transform numpy arrays and pandas dataframes to 3d exports using trimesh""",
     long_description_content_type="text/markdown",
     author='Egil Moeller',
     author_email='em@emeraldgeo.no',
     url='https://github.com/emerald-geomodelling/gltf-shapes',
     packages=setuptools.find_packages(),
```

### Comparing `gltf-shapes-0.0.1/gltfshapes/cube_evenly_sampled.py` & `gltf-shapes-0.0.2/gltfshapes/cube_evenly_sampled.py`

 * *Files identical despite different names*

### Comparing `gltf-shapes-0.0.1/gltfshapes/linear_samples.py` & `gltf-shapes-0.0.2/gltfshapes/linear_samples.py`

 * *Files identical despite different names*

