# Comparing `tmp/easy_pil-0.2.4.tar.gz` & `tmp/easy-pil-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_pil-0.2.4.tar", max compression
+gzip compressed data, was "easy-pil-0.2.5.tar", last modified: Wed May 24 07:10:50 2023, max compression
```

## Comparing `easy_pil-0.2.4.tar` & `easy-pil-0.2.5.tar`

### file list

```diff
@@ -1,24 +1,45 @@
--rw-r--r--   0        0        0     1056 2023-05-12 14:58:42.195381 easy_pil-0.2.4/LICENSE
--rw-r--r--   0        0        0      911 2023-05-12 14:58:42.195381 easy_pil-0.2.4/README.md
--rw-r--r--   0        0        0      454 2023-05-12 14:58:42.199381 easy_pil-0.2.4/easy_pil/__init__.py
--rw-r--r--   0        0        0      209 2023-05-12 14:58:42.199381 easy_pil-0.2.4/easy_pil/_version.py
--rw-r--r--   0        0        0     1059 2023-05-12 14:58:42.203382 easy_pil-0.2.4/easy_pil/canvas.py
--rw-r--r--   0        0        0    18927 2023-05-12 14:58:42.203382 easy_pil-0.2.4/easy_pil/editor.py
--rw-r--r--   0        0        0     3359 2023-05-12 14:58:42.203382 easy_pil-0.2.4/easy_pil/font.py
--rw-r--r--   0        0        0   256900 2023-05-12 14:58:42.203382 easy_pil-0.2.4/easy_pil/fonts/caveat/caveat.ttf
--rw-r--r--   0        0        0   244468 2023-05-12 14:58:42.207382 easy_pil-0.2.4/easy_pil/fonts/montserrat/montserrat_bold.ttf
--rw-r--r--   0        0        0   249088 2023-05-12 14:58:42.207382 easy_pil-0.2.4/easy_pil/fonts/montserrat/montserrat_italic.ttf
--rw-r--r--   0        0        0   242068 2023-05-12 14:58:42.211382 easy_pil-0.2.4/easy_pil/fonts/montserrat/montserrat_light.ttf
--rw-r--r--   0        0        0   245708 2023-05-12 14:58:42.211382 easy_pil-0.2.4/easy_pil/fonts/montserrat/montserrat_regular.ttf
--rw-r--r--   0        0        0   153900 2023-05-12 14:58:42.215382 easy_pil-0.2.4/easy_pil/fonts/poppins/poppins_bold.ttf
--rw-r--r--   0        0        0   181972 2023-05-12 14:58:42.215382 easy_pil-0.2.4/easy_pil/fonts/poppins/poppins_italic.ttf
--rw-r--r--   0        0        0   159848 2023-05-12 14:58:42.215382 easy_pil-0.2.4/easy_pil/fonts/poppins/poppins_light.ttf
--rw-r--r--   0        0        0   158192 2023-05-12 14:58:42.219382 easy_pil-0.2.4/easy_pil/fonts/poppins/poppins_regular.ttf
--rw-r--r--   0        0        0      807 2023-05-12 14:58:42.219382 easy_pil-0.2.4/easy_pil/text.py
--rw-r--r--   0        0        0        0 2023-05-12 14:58:42.219382 easy_pil-0.2.4/easy_pil/types/__init__.py
--rw-r--r--   0        0        0      106 2023-05-12 14:58:42.219382 easy_pil-0.2.4/easy_pil/types/common.py
--rw-r--r--   0        0        0     1490 2023-05-12 14:58:42.219382 easy_pil-0.2.4/easy_pil/types/workspace.py
--rw-r--r--   0        0        0     1608 2023-05-12 14:58:42.219382 easy_pil-0.2.4/easy_pil/utils.py
--rw-r--r--   0        0        0     6651 2023-05-12 14:58:42.219382 easy_pil-0.2.4/easy_pil/workspace.py
--rw-r--r--   0        0        0     1560 2023-05-12 14:58:42.223382 easy_pil-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 easy_pil-0.2.4/PKG-INFO
+drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-05-24 07:10:50.773918 easy-pil-0.2.5/
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1056 2023-05-17 17:50:11.000000 easy-pil-0.2.5/LICENSE
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)       89 2023-05-17 17:50:11.000000 easy-pil-0.2.5/MANIFEST.in
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1940 2023-05-24 07:10:50.773918 easy-pil-0.2.5/PKG-INFO
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      911 2023-05-17 17:50:11.000000 easy-pil-0.2.5/README.md
+drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-05-24 07:10:50.773918 easy-pil-0.2.5/easy_pil/
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      454 2023-05-24 07:04:36.000000 easy-pil-0.2.5/easy_pil/__init__.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      209 2023-05-24 07:07:15.000000 easy-pil-0.2.5/easy_pil/_version.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1059 2023-05-17 17:50:11.000000 easy-pil-0.2.5/easy_pil/canvas.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)    18946 2023-05-24 07:06:29.000000 easy-pil-0.2.5/easy_pil/editor.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     3359 2023-05-17 17:50:11.000000 easy-pil-0.2.5/easy_pil/font.py
+drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-05-24 07:10:50.769918 easy-pil-0.2.5/easy_pil/fonts/
+drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-05-24 07:10:50.773918 easy-pil-0.2.5/easy_pil/fonts/caveat/
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   256900 2023-05-17 17:50:11.000000 easy-pil-0.2.5/easy_pil/fonts/caveat/caveat.ttf
+drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-05-24 07:10:50.773918 easy-pil-0.2.5/easy_pil/fonts/montserrat/
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   244468 2023-05-17 17:50:11.000000 easy-pil-0.2.5/easy_pil/fonts/montserrat/montserrat_bold.ttf
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   249088 2023-05-17 17:50:11.000000 easy-pil-0.2.5/easy_pil/fonts/montserrat/montserrat_italic.ttf
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   242068 2023-05-17 17:50:11.000000 easy-pil-0.2.5/easy_pil/fonts/montserrat/montserrat_light.ttf
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   245708 2023-05-17 17:50:11.000000 easy-pil-0.2.5/easy_pil/fonts/montserrat/montserrat_regular.ttf
+drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-05-24 07:10:50.773918 easy-pil-0.2.5/easy_pil/fonts/poppins/
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   153900 2023-05-17 17:50:11.000000 easy-pil-0.2.5/easy_pil/fonts/poppins/poppins_bold.ttf
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   181972 2023-05-17 17:50:11.000000 easy-pil-0.2.5/easy_pil/fonts/poppins/poppins_italic.ttf
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   159848 2023-05-17 17:50:11.000000 easy-pil-0.2.5/easy_pil/fonts/poppins/poppins_light.ttf
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   158192 2023-05-17 17:50:11.000000 easy-pil-0.2.5/easy_pil/fonts/poppins/poppins_regular.ttf
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      807 2023-05-17 17:50:11.000000 easy-pil-0.2.5/easy_pil/text.py
+drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-05-24 07:10:50.773918 easy-pil-0.2.5/easy_pil/types/
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)        0 2023-05-17 17:50:11.000000 easy-pil-0.2.5/easy_pil/types/__init__.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      106 2023-05-17 17:50:11.000000 easy-pil-0.2.5/easy_pil/types/common.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1490 2023-05-24 07:04:36.000000 easy-pil-0.2.5/easy_pil/types/workspace.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1608 2023-05-17 17:50:11.000000 easy-pil-0.2.5/easy_pil/utils.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     6651 2023-05-17 17:50:11.000000 easy-pil-0.2.5/easy_pil/workspace.py
+drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-05-24 07:10:50.773918 easy-pil-0.2.5/easy_pil.egg-info/
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1940 2023-05-24 07:10:50.000000 easy-pil-0.2.5/easy_pil.egg-info/PKG-INFO
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      914 2023-05-24 07:10:50.000000 easy-pil-0.2.5/easy_pil.egg-info/SOURCES.txt
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)        1 2023-05-24 07:10:50.000000 easy-pil-0.2.5/easy_pil.egg-info/dependency_links.txt
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      119 2023-05-24 07:10:50.000000 easy-pil-0.2.5/easy_pil.egg-info/requires.txt
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)        9 2023-05-24 07:10:50.000000 easy-pil-0.2.5/easy_pil.egg-info/top_level.txt
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1560 2023-05-24 07:04:36.000000 easy-pil-0.2.5/pyproject.toml
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)       88 2023-05-17 17:50:11.000000 easy-pil-0.2.5/requirements.txt
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)       38 2023-05-24 07:10:50.773918 easy-pil-0.2.5/setup.cfg
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     2167 2023-05-17 17:50:11.000000 easy-pil-0.2.5/setup.py
+drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-05-24 07:10:50.773918 easy-pil-0.2.5/tests/
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      402 2023-05-17 17:50:11.000000 easy-pil-0.2.5/tests/test_canvas.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     5152 2023-05-17 17:50:11.000000 easy-pil-0.2.5/tests/test_editor.py
+-rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1004 2023-05-17 17:50:11.000000 easy-pil-0.2.5/tests/test_utils.py
```

### Comparing `easy_pil-0.2.4/LICENSE` & `easy-pil-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_pil-0.2.4/README.md` & `easy-pil-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `easy_pil-0.2.4/easy_pil/canvas.py` & `easy-pil-0.2.5/easy_pil/canvas.py`

 * *Files identical despite different names*

### Comparing `easy_pil-0.2.4/easy_pil/editor.py` & `easy-pil-0.2.5/easy_pil/editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,23 +24,25 @@
 
     def __init__(
         self, _image: Union[Image, str, BytesIO, Editor, Canvas]
     ) -> None:
         if isinstance(_image, (str, BytesIO, Path)):
             self.image: Image = PilImage.open(_image)
         elif isinstance(_image, (Canvas, Editor)):
-            self.image: Image = _image.image.convert("RGBA")
+            self.image: Image = _image.image
         elif isinstance(_image, Image):
-            self.image: Image = _image.convert("RGBA")
+            self.image: Image = _image
         else:
             raise ValueError(
                 "Editor requires an Image, Path, "
                 "Editor or Canvas to start with"
             )
 
+        self.image = self.image.convert("RGBA")
+
     @property
     def image_bytes(self) -> BytesIO:
         """Return image bytes
 
         Returns
         -------
         BytesIO
```

### Comparing `easy_pil-0.2.4/easy_pil/font.py` & `easy-pil-0.2.5/easy_pil/font.py`

 * *Files identical despite different names*

### Comparing `easy_pil-0.2.4/easy_pil/fonts/caveat/caveat.ttf` & `easy-pil-0.2.5/easy_pil/fonts/caveat/caveat.ttf`

 * *Files identical despite different names*

### Comparing `easy_pil-0.2.4/easy_pil/fonts/montserrat/montserrat_bold.ttf` & `easy-pil-0.2.5/easy_pil/fonts/montserrat/montserrat_bold.ttf`

 * *Files identical despite different names*

### Comparing `easy_pil-0.2.4/easy_pil/fonts/montserrat/montserrat_italic.ttf` & `easy-pil-0.2.5/easy_pil/fonts/montserrat/montserrat_italic.ttf`

 * *Files identical despite different names*

### Comparing `easy_pil-0.2.4/easy_pil/fonts/montserrat/montserrat_light.ttf` & `easy-pil-0.2.5/easy_pil/fonts/montserrat/montserrat_light.ttf`

 * *Files identical despite different names*

### Comparing `easy_pil-0.2.4/easy_pil/fonts/montserrat/montserrat_regular.ttf` & `easy-pil-0.2.5/easy_pil/fonts/montserrat/montserrat_regular.ttf`

 * *Files identical despite different names*

### Comparing `easy_pil-0.2.4/easy_pil/fonts/poppins/poppins_bold.ttf` & `easy-pil-0.2.5/easy_pil/fonts/poppins/poppins_bold.ttf`

 * *Files identical despite different names*

### Comparing `easy_pil-0.2.4/easy_pil/fonts/poppins/poppins_italic.ttf` & `easy-pil-0.2.5/easy_pil/fonts/poppins/poppins_italic.ttf`

 * *Files identical despite different names*

### Comparing `easy_pil-0.2.4/easy_pil/fonts/poppins/poppins_light.ttf` & `easy-pil-0.2.5/easy_pil/fonts/poppins/poppins_light.ttf`

 * *Files identical despite different names*

### Comparing `easy_pil-0.2.4/easy_pil/fonts/poppins/poppins_regular.ttf` & `easy-pil-0.2.5/easy_pil/fonts/poppins/poppins_regular.ttf`

 * *Files identical despite different names*

### Comparing `easy_pil-0.2.4/easy_pil/text.py` & `easy-pil-0.2.5/easy_pil/text.py`

 * *Files identical despite different names*

### Comparing `easy_pil-0.2.4/easy_pil/types/workspace.py` & `easy-pil-0.2.5/easy_pil/types/workspace.py`

 * *Files identical despite different names*

### Comparing `easy_pil-0.2.4/easy_pil/utils.py` & `easy-pil-0.2.5/easy_pil/utils.py`

 * *Files identical despite different names*

### Comparing `easy_pil-0.2.4/easy_pil/workspace.py` & `easy-pil-0.2.5/easy_pil/workspace.py`

 * *Files identical despite different names*

### Comparing `easy_pil-0.2.4/pyproject.toml` & `easy-pil-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easy_pil-0.2.4/PKG-INFO` & `easy-pil-0.2.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 Metadata-Version: 2.1
 Name: easy-pil
-Version: 0.2.4
-Summary: A Python library built on top of PIL to easily edit/modify images
+Version: 0.2.5
+Summary: A library to make common tasks of Pillow easy.
 Home-page: https://github.com/shahriyardx/easy-pil
-Keywords: easy-pil,easy pillow,Pillow,image editing
 Author: Md Shahriyar Alam
-Author-email: mdshahriyaralam552@gmail.com
-Requires-Python: >=3.8.1,<3.12
+Author-email: contact@shahriyar.dev
+Project-URL: Documentation, https://easy-pil.readthedocs.io/en/latest/
+Project-URL: Bug Reports, https://github.com/shahriyardx/easy-pil/issues
+Project-URL: Source, https://github.com/shahriyardx/easy-pil/
+Keywords: Pillow,PIL,Pillow wrapper,PIL wrapper,Easy Pillow,Easy PIL,discord rank card,discord card
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Build Tools
-Requires-Dist: aiocache (>=0.12.1,<0.13.0)
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: pillow (>=9.5.0,<10.0.0)
-Requires-Dist: requests (>=2.30.0,<3.0.0)
-Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
-Project-URL: Documentation, https://easy-pil.readthedocs.io/en/latest/
-Project-URL: Repository, https://github.com/shahriyardx/easy-pil
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
 
 # Easy PIL
 ![Lint-Test](https://github.com/shahriyardx/easy-pil/actions/workflows/lint-test.yml/badge.svg)
 
 A Python library built on top of [PIL](https://github.com/python-pillow/Pillow) to easily edit/modify images.
 
 ## Getting Started
@@ -41,8 +35,7 @@
 - Integrate in a [Discord bot](https://easy-pil.readthedocs.io/en/latest/pages/discordbot.html)
 - Some premade [Examples](https://github.com/shahriyardx/easy-pil/tree/master/examples)
 - [Report bugs](https://github.com/shahriyardx/easy-pil/issues/)
 
 ## Get help
 - Ask us in our [Discord server](https://discord.gg/fVzt5THTNb)
 - Watch [Youtube Tutorials](https://www.youtube.com/playlist?list=PLb_oBhGqAlbT4yVqV0TSXggA8b0lZhGhn)
-
```

