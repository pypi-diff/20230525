# Comparing `tmp/samarium62-0.0.1.tar.gz` & `tmp/samarium62-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samarium62-0.0.1.tar", last modified: Wed May 24 08:43:54 2023, max compression
+gzip compressed data, was "samarium62-0.0.2.tar", last modified: Thu May 25 18:39:35 2023, max compression
```

## Comparing `samarium62-0.0.1.tar` & `samarium62-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-24 08:43:54.671748 samarium62-0.0.1/
--rw-r--r--   0 samarthshastry   (501) staff       (20)     1073 2023-05-24 07:57:59.000000 samarium62-0.0.1/LICENSE
--rw-r--r--   0 samarthshastry   (501) staff       (20)      557 2023-05-24 08:43:54.668468 samarium62-0.0.1/PKG-INFO
--rw-r--r--   0 samarthshastry   (501) staff       (20)      104 2023-05-24 08:21:01.000000 samarium62-0.0.1/README.md
--rw-r--r--   0 samarthshastry   (501) staff       (20)      530 2023-05-24 08:17:39.000000 samarium62-0.0.1/pyproject.toml
--rw-r--r--   0 samarthshastry   (501) staff       (20)       38 2023-05-24 08:43:54.682097 samarium62-0.0.1/setup.cfg
-drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-24 08:43:54.599602 samarium62-0.0.1/src/
-drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-24 08:43:54.618088 samarium62-0.0.1/src/samarium62/
--rw-r--r--   0 samarthshastry   (501) staff       (20)      299 2023-05-24 03:20:40.000000 samarium62-0.0.1/src/samarium62/__init__.py
-drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-24 08:43:54.666370 samarium62-0.0.1/src/samarium62/discord/
--rw-r--r--   0 samarthshastry   (501) staff       (20)       78 2023-05-23 23:49:35.000000 samarium62-0.0.1/src/samarium62/discord/__init__.py
--rw-r--r--   0 samarthshastry   (501) staff       (20)     4422 2023-05-24 03:27:02.000000 samarium62-0.0.1/src/samarium62/discord/component.py
--rw-r--r--   0 samarthshastry   (501) staff       (20)     7771 2023-05-24 03:27:26.000000 samarium62-0.0.1/src/samarium62/discord/embed.py
--rw-r--r--   0 samarthshastry   (501) staff       (20)     1025 2023-05-23 23:58:01.000000 samarium62-0.0.1/src/samarium62/discord/image_processing.py
-drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-24 08:43:54.642990 samarium62-0.0.1/src/samarium62.egg-info/
--rw-r--r--   0 samarthshastry   (501) staff       (20)      557 2023-05-24 08:43:54.000000 samarium62-0.0.1/src/samarium62.egg-info/PKG-INFO
--rw-r--r--   0 samarthshastry   (501) staff       (20)      357 2023-05-24 08:43:54.000000 samarium62-0.0.1/src/samarium62.egg-info/SOURCES.txt
--rw-r--r--   0 samarthshastry   (501) staff       (20)        1 2023-05-24 08:43:54.000000 samarium62-0.0.1/src/samarium62.egg-info/dependency_links.txt
--rw-r--r--   0 samarthshastry   (501) staff       (20)       11 2023-05-24 08:43:54.000000 samarium62-0.0.1/src/samarium62.egg-info/top_level.txt
+drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:39:35.820840 samarium62-0.0.2/
+-rw-r--r--   0 samarthshastry   (501) staff       (20)     1073 2023-05-24 07:57:59.000000 samarium62-0.0.2/LICENSE
+-rw-r--r--   0 samarthshastry   (501) staff       (20)      557 2023-05-25 18:39:35.817957 samarium62-0.0.2/PKG-INFO
+-rw-r--r--   0 samarthshastry   (501) staff       (20)      104 2023-05-24 08:21:01.000000 samarium62-0.0.2/README.md
+-rw-r--r--   0 samarthshastry   (501) staff       (20)      569 2023-05-25 18:38:49.000000 samarium62-0.0.2/pyproject.toml
+-rw-r--r--   0 samarthshastry   (501) staff       (20)       38 2023-05-25 18:39:35.821375 samarium62-0.0.2/setup.cfg
+drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:39:35.693254 samarium62-0.0.2/src/
+drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:39:35.731071 samarium62-0.0.2/src/samarium62/
+-rw-r--r--   0 samarthshastry   (501) staff       (20)      299 2023-05-24 03:20:40.000000 samarium62-0.0.2/src/samarium62/__init__.py
+drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:39:35.815573 samarium62-0.0.2/src/samarium62/discord/
+-rw-r--r--   0 samarthshastry   (501) staff       (20)       78 2023-05-23 23:49:35.000000 samarium62-0.0.2/src/samarium62/discord/__init__.py
+-rw-r--r--   0 samarthshastry   (501) staff       (20)     4488 2023-05-25 18:35:26.000000 samarium62-0.0.2/src/samarium62/discord/component.py
+-rw-r--r--   0 samarthshastry   (501) staff       (20)     7820 2023-05-25 18:31:37.000000 samarium62-0.0.2/src/samarium62/discord/embed.py
+-rw-r--r--   0 samarthshastry   (501) staff       (20)     1025 2023-05-23 23:58:01.000000 samarium62-0.0.2/src/samarium62/discord/image_processing.py
+drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:39:35.796677 samarium62-0.0.2/src/samarium62.egg-info/
+-rw-r--r--   0 samarthshastry   (501) staff       (20)      557 2023-05-25 18:39:35.000000 samarium62-0.0.2/src/samarium62.egg-info/PKG-INFO
+-rw-r--r--   0 samarthshastry   (501) staff       (20)      394 2023-05-25 18:39:35.000000 samarium62-0.0.2/src/samarium62.egg-info/SOURCES.txt
+-rw-r--r--   0 samarthshastry   (501) staff       (20)        1 2023-05-25 18:39:35.000000 samarium62-0.0.2/src/samarium62.egg-info/dependency_links.txt
+-rw-r--r--   0 samarthshastry   (501) staff       (20)       14 2023-05-25 18:39:35.000000 samarium62-0.0.2/src/samarium62.egg-info/requires.txt
+-rw-r--r--   0 samarthshastry   (501) staff       (20)       11 2023-05-25 18:39:35.000000 samarium62-0.0.2/src/samarium62.egg-info/top_level.txt
```

### Comparing `samarium62-0.0.1/LICENSE` & `samarium62-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `samarium62-0.0.1/PKG-INFO` & `samarium62-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samarium62
-Version: 0.0.1
+Version: 0.0.2
 Summary: A wrapper package for creating custom discord embed
 Author-email: GitYACC <shastrysamarth@gmail.com>
 Project-URL: Homepage, https://home.page
 Project-URL: Bug Tracker, https://github.com/Future-Lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

### Comparing `samarium62-0.0.1/pyproject.toml` & `samarium62-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "samarium62"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="GitYACC", email="shastrysamarth@gmail.com" },
 ]
 description = "A wrapper package for creating custom discord embed"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License"
 ]
+dependencies = [
+    "pillow>=9.3.0"
+]
 
 [project.urls]
 "Homepage" = "https://home.page"
 "Bug Tracker" = "https://github.com/Future-Lib/issues"
```

### Comparing `samarium62-0.0.1/src/samarium62/discord/component.py` & `samarium62-0.0.2/src/samarium62/discord/component.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,15 +121,16 @@
             cen[0] -= size[0] // 2
             cen[1] -= size[1] // 2
         return cen[0] + self.pos[0], cen[1] + self.pos[1] - 10
         
     @property
     def center(self):
         if self.type == ComponentType.TEXT:
-            bbox = self.font.getbbox(self.text)
+            font = ImageFont.truetype(component.font, component.fsize)
+            bbox = font.getbbox(self.text)
             return (bbox[2] - bbox[0], bbox[3] - bbox[1])
         elif self.type == ComponentType.IMAGE:
             bbox = ImageProcessing.ratio(
                 self, Image.open(self.image)
             ).getbbox()
             return (bbox[2] - bbox[0], bbox[3] - bbox[1])
         elif self.type == ComponentType.PANEL:
```

### Comparing `samarium62-0.0.1/src/samarium62/discord/embed.py` & `samarium62-0.0.2/src/samarium62/discord/embed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from dataclasses import dataclass
 from enum import Enum
-import hikari
-import lightbulb
 from typing import Any, Tuple, TextIO, List
 from PIL import Image, ImageFont, ImageDraw, ImageFilter
 from .component import BaseComponent, ComponentType
 from .image_processing import ImageProcessing
-from html2image import Html2Image
+#from html2image import Html2Image
 import typing
 import json
 
 RGB = Tuple[int, int, int]
 RGBA = Tuple[int, int, int, int]
 
 EmbedConfig = json.load(open("configs.json"))
@@ -168,14 +166,15 @@
             self.root.paste(im, pos)
         elif command.type == ComponentType.PANEL:
             im = Image.new("RGB", command.psize, color=self._front_fill)
             render = ImageDraw.Draw(im)
             self._panel_rounded(render, dim=im.size, fill=command.bgcolor, radius=command.bradius)
             self.root.paste(im, pos)
         elif command.type == ComponentType.HTML:
+            raise Exception("undeveloped component type <ComponentType.HTML>")
             hti = Html2Image(custom_flags=["--disable-gpu"])
             if command.url:
                 hti.screenshot(url=command.url)
             elif command.shtml or command.scss:
                 hti.screenshot(
                     html_str=command.shtml or [], 
                     css_str=command.scss or []
```

### Comparing `samarium62-0.0.1/src/samarium62/discord/image_processing.py` & `samarium62-0.0.2/src/samarium62/discord/image_processing.py`

 * *Files identical despite different names*

### Comparing `samarium62-0.0.1/src/samarium62.egg-info/PKG-INFO` & `samarium62-0.0.2/src/samarium62.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samarium62
-Version: 0.0.1
+Version: 0.0.2
 Summary: A wrapper package for creating custom discord embed
 Author-email: GitYACC <shastrysamarth@gmail.com>
 Project-URL: Homepage, https://home.page
 Project-URL: Bug Tracker, https://github.com/Future-Lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

