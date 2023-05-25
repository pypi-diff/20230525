# Comparing `tmp/agsi-1.3.tar.gz` & `tmp/agsi-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agsi-1.3.tar", last modified: Thu May 25 03:09:02 2023, max compression
+gzip compressed data, was "agsi-1.4.tar", last modified: Thu May 25 06:54:03 2023, max compression
```

## Comparing `agsi-1.3.tar` & `agsi-1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-25 03:09:02.052622 agsi-1.3/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       71 2023-05-24 10:23:11.000000 agsi-1.3/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-05-25 03:09:02.052622 agsi-1.3/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     2077 2023-05-17 09:13:44.000000 agsi-1.3/README.md
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-25 03:09:02.052622 agsi-1.3/agsi/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 09:19:23.000000 agsi-1.3/agsi/__init__.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-25 03:09:02.052622 agsi-1.3/agsi/data/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)    15405 2023-05-25 03:08:44.000000 agsi-1.3/agsi/data/FarmData.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:16:41.000000 agsi-1.3/agsi/data/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     5980 2023-05-17 09:13:44.000000 agsi-1.3/agsi/data/utils.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)   931124 2023-05-19 09:52:59.000000 agsi-1.3/agsi/demo_V2.ipynb
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-17 09:13:44.000000 agsi-1.3/agsi/main.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-17 09:13:44.000000 agsi-1.3/agsi/requirements.txt
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-25 03:09:02.052622 agsi-1.3/agsi.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-05-25 03:09:01.000000 agsi-1.3/agsi.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-05-25 03:09:02.000000 agsi-1.3/agsi.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-25 03:09:01.000000 agsi-1.3/agsi.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-25 03:09:01.000000 agsi-1.3/agsi.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-05-25 03:09:01.000000 agsi-1.3/agsi.egg-info/top_level.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-25 03:09:02.052622 agsi-1.3/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-05-25 03:08:52.000000 agsi-1.3/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-25 06:54:03.293002 agsi-1.4/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       71 2023-05-24 10:23:11.000000 agsi-1.4/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-05-25 06:54:03.293002 agsi-1.4/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     2077 2023-05-17 09:13:44.000000 agsi-1.4/README.md
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-25 06:54:03.293002 agsi-1.4/agsi/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 09:19:23.000000 agsi-1.4/agsi/__init__.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-25 06:54:03.293002 agsi-1.4/agsi/data/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)    15401 2023-05-25 06:53:51.000000 agsi-1.4/agsi/data/FarmData.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:16:41.000000 agsi-1.4/agsi/data/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     5980 2023-05-17 09:13:44.000000 agsi-1.4/agsi/data/utils.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)   931124 2023-05-19 09:52:59.000000 agsi-1.4/agsi/demo_V2.ipynb
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-17 09:13:44.000000 agsi-1.4/agsi/main.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-17 09:13:44.000000 agsi-1.4/agsi/requirements.txt
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-25 06:54:03.293002 agsi-1.4/agsi.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-05-25 06:54:03.000000 agsi-1.4/agsi.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-05-25 06:54:03.000000 agsi-1.4/agsi.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-25 06:54:03.000000 agsi-1.4/agsi.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-25 06:54:03.000000 agsi-1.4/agsi.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-05-25 06:54:03.000000 agsi-1.4/agsi.egg-info/top_level.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-25 06:54:03.293002 agsi-1.4/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-05-25 06:53:57.000000 agsi-1.4/setup.py
```

### Comparing `agsi-1.3/README.md` & `agsi-1.4/README.md`

 * *Files identical despite different names*

### Comparing `agsi-1.3/agsi/data/FarmData.py` & `agsi-1.4/agsi/data/FarmData.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
      for farm_key,farm_obj in self.farms.items():
         
         if farm_obj.info['owner']==farm_name:
            return farm_obj      
         
   def get_block_by_name(self,block_name):
     
-    for block_key,block_obj in self.farms_info.items():
+    for block_key,block_obj in self.blocks.items():
       
       if block_obj['block_name']==block_name:
           return block_obj 
         
   def __get_block_objects__(self):
 
     all_blocks={}
```

### Comparing `agsi-1.3/agsi/data/utils.py` & `agsi-1.4/agsi/data/utils.py`

 * *Files identical despite different names*

### Comparing `agsi-1.3/agsi/demo_V2.ipynb` & `agsi-1.4/agsi/demo_V2.ipynb`

 * *Files identical despite different names*

