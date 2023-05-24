# Comparing `tmp/iiif_tools-0.0.1.tar.gz` & `tmp/iiif_tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iiif_tools-0.0.1.tar", last modified: Wed May 24 22:18:13 2023, max compression
+gzip compressed data, was "iiif_tools-0.0.2.tar", last modified: Wed May 24 22:54:20 2023, max compression
```

## Comparing `iiif_tools-0.0.1.tar` & `iiif_tools-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-05-24 22:18:13.302866 iiif_tools-0.0.1/
--rw-rw-r--   0 nakamura   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 iiif_tools-0.0.1/LICENSE
--rw-rw-r--   0 nakamura   (501) staff       (20)      111 2023-04-27 10:12:58.000000 iiif_tools-0.0.1/MANIFEST.in
--rw-r--r--   0 nakamura   (501) staff       (20)     1068 2023-05-24 22:18:13.302476 iiif_tools-0.0.1/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      305 2023-05-24 22:15:17.000000 iiif_tools-0.0.1/README.md
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-05-24 22:18:13.300744 iiif_tools-0.0.1/iiif_tools/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-05-24 22:15:59.000000 iiif_tools-0.0.1/iiif_tools/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     2227 2023-05-24 22:15:59.000000 iiif_tools-0.0.1/iiif_tools/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)      142 2023-05-24 22:15:59.000000 iiif_tools-0.0.1/iiif_tools/core.py
--rw-r--r--   0 nakamura   (501) staff       (20)     6406 2023-05-24 22:15:59.000000 iiif_tools-0.0.1/iiif_tools/pdf.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-05-24 22:18:13.302198 iiif_tools-0.0.1/iiif_tools.egg-info/
--rw-r--r--   0 nakamura   (501) staff       (20)     1068 2023-05-24 22:18:13.000000 iiif_tools-0.0.1/iiif_tools.egg-info/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      372 2023-05-24 22:18:13.000000 iiif_tools-0.0.1/iiif_tools.egg-info/SOURCES.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-05-24 22:18:13.000000 iiif_tools-0.0.1/iiif_tools.egg-info/dependency_links.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       63 2023-05-24 22:18:13.000000 iiif_tools-0.0.1/iiif_tools.egg-info/entry_points.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-05-24 22:15:50.000000 iiif_tools-0.0.1/iiif_tools.egg-info/not-zip-safe
--rw-r--r--   0 nakamura   (501) staff       (20)       15 2023-05-24 22:18:13.000000 iiif_tools-0.0.1/iiif_tools.egg-info/requires.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       11 2023-05-24 22:18:13.000000 iiif_tools-0.0.1/iiif_tools.egg-info/top_level.txt
--rw-r--r--   0 nakamura   (501) staff       (20)      907 2023-05-24 22:16:14.000000 iiif_tools-0.0.1/settings.ini
--rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-05-24 22:18:13.302983 iiif_tools-0.0.1/setup.cfg
--rw-rw-r--   0 nakamura   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 iiif_tools-0.0.1/setup.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-05-24 22:54:20.017697 iiif_tools-0.0.2/
+-rw-rw-r--   0 nakamura   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 iiif_tools-0.0.2/LICENSE
+-rw-rw-r--   0 nakamura   (501) staff       (20)      111 2023-04-27 10:12:58.000000 iiif_tools-0.0.2/MANIFEST.in
+-rw-r--r--   0 nakamura   (501) staff       (20)     1068 2023-05-24 22:54:20.017479 iiif_tools-0.0.2/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      305 2023-05-24 22:15:17.000000 iiif_tools-0.0.2/README.md
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-05-24 22:54:20.015698 iiif_tools-0.0.2/iiif_tools/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-05-24 22:52:19.000000 iiif_tools-0.0.2/iiif_tools/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     2132 2023-05-24 22:52:19.000000 iiif_tools-0.0.2/iiif_tools/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)      142 2023-05-24 22:52:19.000000 iiif_tools-0.0.2/iiif_tools/core.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     6352 2023-05-24 22:52:19.000000 iiif_tools-0.0.2/iiif_tools/pdf.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-05-24 22:54:20.016992 iiif_tools-0.0.2/iiif_tools.egg-info/
+-rw-r--r--   0 nakamura   (501) staff       (20)     1068 2023-05-24 22:54:20.000000 iiif_tools-0.0.2/iiif_tools.egg-info/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      372 2023-05-24 22:54:20.000000 iiif_tools-0.0.2/iiif_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-05-24 22:54:20.000000 iiif_tools-0.0.2/iiif_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       63 2023-05-24 22:54:20.000000 iiif_tools-0.0.2/iiif_tools.egg-info/entry_points.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-05-24 22:15:50.000000 iiif_tools-0.0.2/iiif_tools.egg-info/not-zip-safe
+-rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-05-24 22:54:20.000000 iiif_tools-0.0.2/iiif_tools.egg-info/requires.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       11 2023-05-24 22:54:20.000000 iiif_tools-0.0.2/iiif_tools.egg-info/top_level.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)      921 2023-05-24 22:54:09.000000 iiif_tools-0.0.2/settings.ini
+-rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-05-24 22:54:20.017817 iiif_tools-0.0.2/setup.cfg
+-rw-rw-r--   0 nakamura   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 iiif_tools-0.0.2/setup.py
```

### Comparing `iiif_tools-0.0.1/LICENSE` & `iiif_tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iiif_tools-0.0.1/PKG-INFO` & `iiif_tools-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iiif_tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/iiif_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `iiif_tools-0.0.1/iiif_tools/_modidx.py` & `iiif_tools-0.0.2/iiif_tools/_modidx.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,9 +15,8 @@
                                 'iiif_tools.pdf.PdfClient.create_pdf_from_manifest_local': ( 'pdf.html#pdfclient.create_pdf_from_manifest_local',
                                                                                              'iiif_tools/pdf.py'),
                                 'iiif_tools.pdf.PdfClient.create_pdf_from_manifest_url': ( 'pdf.html#pdfclient.create_pdf_from_manifest_url',
                                                                                            'iiif_tools/pdf.py'),
                                 'iiif_tools.pdf.PdfClient.download_image': ('pdf.html#pdfclient.download_image', 'iiif_tools/pdf.py'),
                                 'iiif_tools.pdf.PdfClient.download_images': ('pdf.html#pdfclient.download_images', 'iiif_tools/pdf.py'),
                                 'iiif_tools.pdf.PdfClient.get_infos': ('pdf.html#pdfclient.get_infos', 'iiif_tools/pdf.py'),
-                                'iiif_tools.pdf.PdfClient.save': ('pdf.html#pdfclient.save', 'iiif_tools/pdf.py'),
-                                'iiif_tools.pdf.test': ('pdf.html#test', 'iiif_tools/pdf.py')}}}
+                                'iiif_tools.pdf.PdfClient.save': ('pdf.html#pdfclient.save', 'iiif_tools/pdf.py')}}}
```

### Comparing `iiif_tools-0.0.1/iiif_tools/pdf.py` & `iiif_tools-0.0.2/iiif_tools/pdf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/pdf.ipynb.
 
 # %% auto 0
-__all__ = ['test', 'PdfClient']
+__all__ = ['PdfClient']
 
 # %% ../nbs/pdf.ipynb 3
-from urllib import request  # urllib.requestモジュールをインポート
-from bs4 import BeautifulSoup  # BeautifulSoupクラスをインポート
 import requests
 from tqdm import tqdm
 import json
 import os
 import urllib.error
 import urllib.request
 import datetime
 import img2pdf
 from PIL import Image
 import shutil
 
 # %% ../nbs/pdf.ipynb 4
-def test():
-    print("boo")
-
-# %% ../nbs/pdf.ipynb 5
 class PdfClient:
     def __init__(self):
 
         dt = datetime.datetime.now()
         ts = datetime.datetime.timestamp(dt)
 
         tmp_dir = f"/tmp/iiif_pdf/{ts}"
@@ -39,18 +33,18 @@
         with open(input_path) as f:
             manifest = json.load(f)
         client.download_images(manifest, limit)
         client.create_pdf(outout_path)
         shutil.rmtree(client.tmp_dir)
 
     @staticmethod
-    def create_pdf_from_dir(input_dir, outout_path):
+    def create_pdf_from_dir(input_dir, outout_path, extension="jpg"):
         client = PdfClient()
         client.tmp_dir = input_dir
-        client.create_pdf(outout_path, extension="jpg")
+        client.create_pdf(outout_path, extension=extension)
         shutil.rmtree(client.tmp_dir)
 
 
     @staticmethod
     def create_pdf_from_manifest_url(manifest_url, outout_path, limit = -1):
         client = PdfClient()
         manifest = requests.get(manifest_url).json()
@@ -76,15 +70,19 @@
 
         if limit > 0:
             canvases = canvases[0:limit]
 
         for i in tqdm(range(len(canvases))):
             canvas = canvases[i]
             resource = canvas["images"][0]["resource"]
-            url = resource["@id"] #  + "/full/full/0/default.jpg"
+
+            if "service" in resource:
+                url = resource["service"]["@id"] + "/full/full/0/default.jpg"
+            else:
+                url = resource["@id"] #  + "/full/full/0/default.jpg"
             opath = self.tmp_dir + "/" + str(i).zfill(5) + ".jpg"
             self.download_image(url, opath)
 
     def download_image(self, url, dst_path):
         # dst_path = self.tmp_dir + "/" + url.replace("/", "_")
         try:
             with urllib.request.urlopen(url) as web_file:
```

### Comparing `iiif_tools-0.0.1/iiif_tools.egg-info/PKG-INFO` & `iiif_tools-0.0.2/iiif_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iiif-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/iiif_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `iiif_tools-0.0.1/settings.ini` & `iiif_tools-0.0.2/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = iiif_tools
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = iiif_tools
@@ -34,10 +34,10 @@
 description = 
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = nakamura196
 
 ### Optional ###
-requirements = img2pdf
+requirements = img2pdf requests tqdm
 # dev_requirements = 
 # console_scripts =
```

### Comparing `iiif_tools-0.0.1/setup.py` & `iiif_tools-0.0.2/setup.py`

 * *Files identical despite different names*

