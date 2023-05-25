# Comparing `tmp/samarium62-0.0.3.tar.gz` & `tmp/samarium62-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samarium62-0.0.3.tar", last modified: Thu May 25 18:46:41 2023, max compression
+gzip compressed data, was "samarium62-0.0.4.tar", last modified: Thu May 25 21:56:03 2023, max compression
```

## Comparing `samarium62-0.0.3.tar` & `samarium62-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:46:41.255041 samarium62-0.0.3/
--rw-r--r--   0 samarthshastry   (501) staff       (20)     1073 2023-05-24 07:57:59.000000 samarium62-0.0.3/LICENSE
--rw-r--r--   0 samarthshastry   (501) staff       (20)      557 2023-05-25 18:46:41.254065 samarium62-0.0.3/PKG-INFO
--rw-r--r--   0 samarthshastry   (501) staff       (20)      104 2023-05-24 08:21:01.000000 samarium62-0.0.3/README.md
--rw-r--r--   0 samarthshastry   (501) staff       (20)      569 2023-05-25 18:46:18.000000 samarium62-0.0.3/pyproject.toml
--rw-r--r--   0 samarthshastry   (501) staff       (20)       38 2023-05-25 18:46:41.255214 samarium62-0.0.3/setup.cfg
-drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:46:41.227403 samarium62-0.0.3/src/
-drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:46:41.233432 samarium62-0.0.3/src/samarium62/
--rw-r--r--   0 samarthshastry   (501) staff       (20)      298 2023-05-25 18:46:00.000000 samarium62-0.0.3/src/samarium62/__init__.py
-drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:46:41.251405 samarium62-0.0.3/src/samarium62/discord/
--rw-r--r--   0 samarthshastry   (501) staff       (20)       78 2023-05-23 23:49:35.000000 samarium62-0.0.3/src/samarium62/discord/__init__.py
--rw-r--r--   0 samarthshastry   (501) staff       (20)     4488 2023-05-25 18:35:26.000000 samarium62-0.0.3/src/samarium62/discord/component.py
--rw-r--r--   0 samarthshastry   (501) staff       (20)     7820 2023-05-25 18:31:37.000000 samarium62-0.0.3/src/samarium62/discord/embed.py
--rw-r--r--   0 samarthshastry   (501) staff       (20)     1025 2023-05-23 23:58:01.000000 samarium62-0.0.3/src/samarium62/discord/image_processing.py
-drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 18:46:41.244630 samarium62-0.0.3/src/samarium62.egg-info/
--rw-r--r--   0 samarthshastry   (501) staff       (20)      557 2023-05-25 18:46:41.000000 samarium62-0.0.3/src/samarium62.egg-info/PKG-INFO
--rw-r--r--   0 samarthshastry   (501) staff       (20)      394 2023-05-25 18:46:41.000000 samarium62-0.0.3/src/samarium62.egg-info/SOURCES.txt
--rw-r--r--   0 samarthshastry   (501) staff       (20)        1 2023-05-25 18:46:41.000000 samarium62-0.0.3/src/samarium62.egg-info/dependency_links.txt
--rw-r--r--   0 samarthshastry   (501) staff       (20)       14 2023-05-25 18:46:41.000000 samarium62-0.0.3/src/samarium62.egg-info/requires.txt
--rw-r--r--   0 samarthshastry   (501) staff       (20)       11 2023-05-25 18:46:41.000000 samarium62-0.0.3/src/samarium62.egg-info/top_level.txt
+drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 21:56:03.854162 samarium62-0.0.4/
+-rw-r--r--   0 samarthshastry   (501) staff       (20)     1073 2023-05-24 07:57:59.000000 samarium62-0.0.4/LICENSE
+-rw-r--r--   0 samarthshastry   (501) staff       (20)      557 2023-05-25 21:56:03.852817 samarium62-0.0.4/PKG-INFO
+-rw-r--r--   0 samarthshastry   (501) staff       (20)      104 2023-05-24 08:21:01.000000 samarium62-0.0.4/README.md
+-rw-r--r--   0 samarthshastry   (501) staff       (20)      569 2023-05-25 21:55:39.000000 samarium62-0.0.4/pyproject.toml
+-rw-r--r--   0 samarthshastry   (501) staff       (20)       38 2023-05-25 21:56:03.854316 samarium62-0.0.4/setup.cfg
+drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 21:56:03.808013 samarium62-0.0.4/src/
+drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 21:56:03.818318 samarium62-0.0.4/src/samarium62/
+-rw-r--r--   0 samarthshastry   (501) staff       (20)      317 2023-05-25 21:07:40.000000 samarium62-0.0.4/src/samarium62/__init__.py
+drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 21:56:03.838088 samarium62-0.0.4/src/samarium62/discord/
+-rw-r--r--   0 samarthshastry   (501) staff       (20)       78 2023-05-23 23:49:35.000000 samarium62-0.0.4/src/samarium62/discord/__init__.py
+-rw-r--r--   0 samarthshastry   (501) staff       (20)     5458 2023-05-25 21:55:01.000000 samarium62-0.0.4/src/samarium62/discord/component.py
+-rw-r--r--   0 samarthshastry   (501) staff       (20)     7820 2023-05-25 18:31:37.000000 samarium62-0.0.4/src/samarium62/discord/embed.py
+-rw-r--r--   0 samarthshastry   (501) staff       (20)     1025 2023-05-23 23:58:01.000000 samarium62-0.0.4/src/samarium62/discord/image_processing.py
+drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 21:56:03.850101 samarium62-0.0.4/src/samarium62/ext/
+-rw-r--r--   0 samarthshastry   (501) staff       (20)       21 2023-05-25 20:55:26.000000 samarium62-0.0.4/src/samarium62/ext/__init__.py
+-rw-r--r--   0 samarthshastry   (501) staff       (20)      511 2023-05-25 21:49:29.000000 samarium62-0.0.4/src/samarium62/ext/checks.py
+drwxr-xr-x   0 samarthshastry   (501) staff       (20)        0 2023-05-25 21:56:03.824443 samarium62-0.0.4/src/samarium62.egg-info/
+-rw-r--r--   0 samarthshastry   (501) staff       (20)      557 2023-05-25 21:56:03.000000 samarium62-0.0.4/src/samarium62.egg-info/PKG-INFO
+-rw-r--r--   0 samarthshastry   (501) staff       (20)      454 2023-05-25 21:56:03.000000 samarium62-0.0.4/src/samarium62.egg-info/SOURCES.txt
+-rw-r--r--   0 samarthshastry   (501) staff       (20)        1 2023-05-25 21:56:03.000000 samarium62-0.0.4/src/samarium62.egg-info/dependency_links.txt
+-rw-r--r--   0 samarthshastry   (501) staff       (20)       14 2023-05-25 21:56:03.000000 samarium62-0.0.4/src/samarium62.egg-info/requires.txt
+-rw-r--r--   0 samarthshastry   (501) staff       (20)       11 2023-05-25 21:56:03.000000 samarium62-0.0.4/src/samarium62.egg-info/top_level.txt
```

### Comparing `samarium62-0.0.3/LICENSE` & `samarium62-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `samarium62-0.0.3/PKG-INFO` & `samarium62-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samarium62
-Version: 0.0.3
+Version: 0.0.4
 Summary: A wrapper package for creating custom discord embed
 Author-email: GitYACC <shastrysamarth@gmail.com>
 Project-URL: Homepage, https://home.page
 Project-URL: Bug Tracker, https://github.com/Future-Lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

### Comparing `samarium62-0.0.3/pyproject.toml` & `samarium62-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "samarium62"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="GitYACC", email="shastrysamarth@gmail.com" },
 ]
 description = "A wrapper package for creating custom discord embed"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `samarium62-0.0.3/src/samarium62/discord/component.py` & `samarium62-0.0.4/src/samarium62/discord/component.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from enum import Enum
 from typing import *
 from PIL import Image, ImageFont
 import json
 from .image_processing import ImageProcessing
+from ..ext.checks import enforce_type
 
 class ComponentType(Enum):
     PANEL = 1
     TEXT = 2
     IMAGE = 3
     HTML = 4
 
@@ -17,79 +18,121 @@
 configs["foreground_color"] = tuple(configs["foreground_color"])
 
 class BaseComponent:
     def __init__(self, name: str, type: ComponentType, **attrs):
         self.name = name
         self.type = type
         self.font = configs["base_font"]
-        self.fsize: int = (
+        self.fsize: int = enforce_type(
+            "font-size",
             attrs.get("fsize") or
             attrs.get("font-size") or
-            configs["base_font_size"]
+            configs["base_font_size"],
+            int
         )
 
         # ALL Flags
-        self.pos: Tuple[int, int] = attrs.get("position")
+        self.pos: Tuple[int, int] = enforce_type(
+            "position",
+            attrs.get("position"),
+            tuple
+        )
 
         # if self.type == ComponentType.PANEL
-        self.repos: Tuple[int, int] = (
+        self.repos: Tuple[int, int] = enforce_type(
+            "relative-position",
             attrs.get("repos") or
-            attrs.get("relative-position")
+            attrs.get("relative-position"),
+            tuple
+        )
+        self.attached_to: str = enforce_type(
+            "attached-to",
+            attrs.get("attached-to"),
+            str
         )
-        self.attached_to = attrs.get("attached-to")
         # self.focus: bool = attrs.get("focus")
 
         # Partial Flags (excludes Text)
-        self.bradius = (
+        self.bradius = enforce_type(
+            "border-radius",
             attrs.get("bradius") or
             attrs.get("border-radius") or
-            0
+            0,
+            int
         )
 
-        self.bcolor: Tuple[int, int, int] = (
+        self.bcolor: Tuple[int, int, int] = enforce_type(
+            "border-color",
             attrs.get("bcolor") or
             attrs.get("border-color") or
-            (0, 0, 0)
+            (0, 0, 0),
+            tuple
         )
 
         # Panel Flags
         self.bgcolor: Tuple[int, int, int] = (
             attrs.get("bgcolor") or
             attrs.get("background-color") or
             (0, 0, 0)
         )
 
-        self.psize: Tuple[int, int] = (
+        self.psize: Tuple[int, int] = enforce_type(
+            "panel-size",
             attrs.get("psize") or
-            attrs.get("panel-size")
+            attrs.get("panel-size"),
+            tuple
         )
 
         self.children: Dict[str, self.__class__] = {}
 
 
 
         # Text Flags (can be applied into a panel)
-        self.text: str = attrs.get("text")
-        self.tcolor: Tuple[int, int, int] = (
+        self.text: str = enforce_type(
+            "text",
+            attrs.get("text"),
+            str
+        )
+        self.tcolor: Tuple[int, int, int] = enforce_type(
+            "text-color",
             attrs.get("tcolor") or
             attrs.get("text-color") or
-            (0, 0, 0)
+            (0, 0, 0),
+            tuple
         )
 
-        self.highlight: bool = attrs.get("highlight")
-        self.italicize: bool = attrs.get("italicize")
-        self.bold: bool = attrs.get("bold")
+        self.highlight: bool = enforce_type(
+            "highlight",
+            attrs.get("highlight"),
+            bool
+        )
+        self.italicize: bool = enforce_type(
+            "italicize",
+            attrs.get("italicize"),
+            bool
+        )
+        self.bold: bool = enforce_type(
+            "bold",
+            attrs.get("bold"),
+            bool
+        )
 
         # Image Flags
-        self.image = (
+        self.image = enforce_type(
+            "image",
             attrs.get("image") or
-            attrs.get("ipath")
+            attrs.get("ipath"),
+            str
         )
 
-        self.ratio: int = attrs.get("ratio")
+        self.ratio: int = enforce_type(
+            "ratio",
+            attrs.get("ratio"),
+            int
+        )
 
         # HTML Flags
         self.html = attrs.get("html")
         self.shtml: str = (
             attrs.get("shtml") or
             attrs.get("string-html")
         )
@@ -121,15 +164,15 @@
             cen[0] -= size[0] // 2
             cen[1] -= size[1] // 2
         return cen[0] + self.pos[0], cen[1] + self.pos[1] - 10
         
     @property
     def center(self):
         if self.type == ComponentType.TEXT:
-            font = ImageFont.truetype(component.font, component.fsize)
+            font = ImageFont.truetype(self.font, self.fsize)
             bbox = font.getbbox(self.text)
             return (bbox[2] - bbox[0], bbox[3] - bbox[1])
         elif self.type == ComponentType.IMAGE:
             bbox = ImageProcessing.ratio(
                 self, Image.open(self.image)
             ).getbbox()
             return (bbox[2] - bbox[0], bbox[3] - bbox[1])
```

### Comparing `samarium62-0.0.3/src/samarium62/discord/embed.py` & `samarium62-0.0.4/src/samarium62/discord/embed.py`

 * *Files identical despite different names*

### Comparing `samarium62-0.0.3/src/samarium62/discord/image_processing.py` & `samarium62-0.0.4/src/samarium62/discord/image_processing.py`

 * *Files identical despite different names*

### Comparing `samarium62-0.0.3/src/samarium62.egg-info/PKG-INFO` & `samarium62-0.0.4/src/samarium62.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samarium62
-Version: 0.0.3
+Version: 0.0.4
 Summary: A wrapper package for creating custom discord embed
 Author-email: GitYACC <shastrysamarth@gmail.com>
 Project-URL: Homepage, https://home.page
 Project-URL: Bug Tracker, https://github.com/Future-Lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

