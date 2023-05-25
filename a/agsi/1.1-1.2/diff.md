# Comparing `tmp/agsi-1.1.tar.gz` & `tmp/agsi-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agsi-1.1.tar", last modified: Wed May 24 10:24:00 2023, max compression
+gzip compressed data, was "agsi-1.2.tar", last modified: Wed May 24 15:19:22 2023, max compression
```

## Comparing `agsi-1.1.tar` & `agsi-1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-24 10:24:00.176120 agsi-1.1/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       71 2023-05-24 10:23:11.000000 agsi-1.1/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-05-24 10:24:00.176120 agsi-1.1/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     2077 2023-05-17 09:13:44.000000 agsi-1.1/README.md
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-24 10:24:00.176120 agsi-1.1/agsi/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 09:19:23.000000 agsi-1.1/agsi/__init__.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-24 10:24:00.176120 agsi-1.1/agsi/data/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)    14628 2023-05-24 10:22:28.000000 agsi-1.1/agsi/data/FarmData.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:16:41.000000 agsi-1.1/agsi/data/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     5980 2023-05-17 09:13:44.000000 agsi-1.1/agsi/data/utils.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)   931124 2023-05-19 09:52:59.000000 agsi-1.1/agsi/demo_V2.ipynb
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-17 09:13:44.000000 agsi-1.1/agsi/main.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-17 09:13:44.000000 agsi-1.1/agsi/requirements.txt
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-24 10:24:00.176120 agsi-1.1/agsi.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-05-24 10:24:00.000000 agsi-1.1/agsi.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-05-24 10:24:00.000000 agsi-1.1/agsi.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-24 10:24:00.000000 agsi-1.1/agsi.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-24 10:24:00.000000 agsi-1.1/agsi.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-05-24 10:24:00.000000 agsi-1.1/agsi.egg-info/top_level.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-24 10:24:00.176120 agsi-1.1/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-05-24 10:22:52.000000 agsi-1.1/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-24 15:19:22.954627 agsi-1.2/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       71 2023-05-24 10:23:11.000000 agsi-1.2/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-05-24 15:19:22.954627 agsi-1.2/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     2077 2023-05-17 09:13:44.000000 agsi-1.2/README.md
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-24 15:19:22.954627 agsi-1.2/agsi/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 09:19:23.000000 agsi-1.2/agsi/__init__.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-24 15:19:22.954627 agsi-1.2/agsi/data/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)    15130 2023-05-24 15:18:44.000000 agsi-1.2/agsi/data/FarmData.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:16:41.000000 agsi-1.2/agsi/data/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     5980 2023-05-17 09:13:44.000000 agsi-1.2/agsi/data/utils.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)   931124 2023-05-19 09:52:59.000000 agsi-1.2/agsi/demo_V2.ipynb
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-17 09:13:44.000000 agsi-1.2/agsi/main.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-17 09:13:44.000000 agsi-1.2/agsi/requirements.txt
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-24 15:19:22.954627 agsi-1.2/agsi.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-05-24 15:19:22.000000 agsi-1.2/agsi.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-05-24 15:19:22.000000 agsi-1.2/agsi.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-24 15:19:22.000000 agsi-1.2/agsi.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-24 15:19:22.000000 agsi-1.2/agsi.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-05-24 15:19:22.000000 agsi-1.2/agsi.egg-info/top_level.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-24 15:19:22.954627 agsi-1.2/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-05-24 15:19:18.000000 agsi-1.2/setup.py
```

### Comparing `agsi-1.1/README.md` & `agsi-1.2/README.md`

 * *Files identical despite different names*

### Comparing `agsi-1.1/agsi/data/FarmData.py` & `agsi-1.2/agsi/data/FarmData.py`

 * *Files 7% similar despite different names*

```diff
@@ -308,30 +308,41 @@
 
       """
 
       self.info=block_info
       self.block_id=self.info['block_id']
       self.farm_info=farm_info
         
-  def get_modality(self,modality_type="drone_75",timestamp=None):
+  def get_modality(self,modality_type="drone_75",timestamp=None,shp_clip=True):
       
       """
       Retrieves the block geometry from the shapefile and clips it from the farm image.
 
       Args:
           shp_file (str): The file path to the shapefile.
           farm_image_path (str): The file path to the farm image.
 
       Returns:
           numpy.ndarray: The clipped block chip.
 
       """
       if self.info['data_path'][modality_type]!="":
-         image_path=self.info['data_path'][timestamp][modality_type]
-         return open_tiff(image_path)
+         if shp_clip:            
+            shp_file=self.info['shp']
+            block_image_path=self.info['data_path'][timestamp][modality_type]
+            if modality_type.startswith("drone_"):
+              crs="epsg:32644"
+            else:
+              crs="epsg:3857"
+            block_polygon=open_shp(shp_file,crs)['geometry'].values[0]
+            clipped_chip=get_clipped_chip(block_image_path,[block_polygon])
+            return clipped_chip
+         else:
+            image_path=self.info['data_path'][timestamp][modality_type]
+            return open_tiff(image_path)        
       else:
         shp_file=self.info['shp']
         farm_image_path=self.farm_info['data_path'][timestamp][modality_type]
         if modality_type.startswith("drone_"):
            crs="epsg:32644"
         else:
            crs="epsg:3857"
```

### Comparing `agsi-1.1/agsi/data/utils.py` & `agsi-1.2/agsi/data/utils.py`

 * *Files identical despite different names*

### Comparing `agsi-1.1/agsi/demo_V2.ipynb` & `agsi-1.2/agsi/demo_V2.ipynb`

 * *Files identical despite different names*

