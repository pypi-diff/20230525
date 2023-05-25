# Comparing `tmp/musicTour-1.4.0.tar.gz` & `tmp/musicTour-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicTour-1.4.0.tar", last modified: Thu May 25 07:38:17 2023, max compression
+gzip compressed data, was "musicTour-1.5.0.tar", last modified: Thu May 25 08:36:06 2023, max compression
```

## Comparing `musicTour-1.4.0.tar` & `musicTour-1.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 07:38:17.844771 musicTour-1.4.0/
--rw-rw-rw-   0        0        0     1067 2023-05-24 11:26:32.000000 musicTour-1.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0      530 2023-05-25 07:38:17.843783 musicTour-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       53 2023-05-24 11:07:35.000000 musicTour-1.4.0/README.md
--rw-rw-rw-   0        0        0      469 2023-05-25 07:37:54.000000 musicTour-1.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 07:38:17.844771 musicTour-1.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 07:38:17.835769 musicTour-1.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 07:38:17.838769 musicTour-1.4.0/src/musicTour/
--rw-rw-rw-   0        0        0       33 2023-05-24 11:38:35.000000 musicTour-1.4.0/src/musicTour/__init__.py
--rw-rw-rw-   0        0        0     3607 2023-05-25 07:35:34.000000 musicTour-1.4.0/src/musicTour/musicTour.py
-drwxrwxrwx   0        0        0        0 2023-05-25 07:38:17.843783 musicTour-1.4.0/src/musicTour.egg-info/
--rw-rw-rw-   0        0        0      530 2023-05-25 07:38:17.000000 musicTour-1.4.0/src/musicTour.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-05-25 07:38:17.000000 musicTour-1.4.0/src/musicTour.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 07:38:17.000000 musicTour-1.4.0/src/musicTour.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-25 07:38:17.000000 musicTour-1.4.0/src/musicTour.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 08:36:06.090291 musicTour-1.5.0/
+-rw-rw-rw-   0        0        0     1067 2023-05-24 11:26:32.000000 musicTour-1.5.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1745 2023-05-25 08:36:06.090291 musicTour-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1268 2023-05-25 08:34:28.000000 musicTour-1.5.0/README.md
+-rw-rw-rw-   0        0        0      469 2023-05-25 07:48:00.000000 musicTour-1.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 08:36:06.091289 musicTour-1.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 08:36:06.079975 musicTour-1.5.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 08:36:06.085289 musicTour-1.5.0/src/musicTour/
+-rw-rw-rw-   0        0        0     1142 2023-05-25 08:35:24.000000 musicTour-1.5.0/src/musicTour/__init__.py
+-rw-rw-rw-   0        0        0     3490 2023-05-25 07:49:20.000000 musicTour-1.5.0/src/musicTour/musicTour.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:36:06.089290 musicTour-1.5.0/src/musicTour.egg-info/
+-rw-rw-rw-   0        0        0     1745 2023-05-25 08:36:06.000000 musicTour-1.5.0/src/musicTour.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-25 08:36:06.000000 musicTour-1.5.0/src/musicTour.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 08:36:06.000000 musicTour-1.5.0/src/musicTour.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-25 08:36:06.000000 musicTour-1.5.0/src/musicTour.egg-info/top_level.txt
```

### Comparing `musicTour-1.4.0/LICENSE.txt` & `musicTour-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `musicTour-1.4.0/src/musicTour/musicTour.py` & `musicTour-1.5.0/src/musicTour/musicTour.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) [année] [titulaire du droit d'auteur]
+# Copyright (c) [2023] [Snow Drop]
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,15 +18,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import requests
 from bs4 import BeautifulSoup
 import json
 
-def getAll(styles = True, artists = True, output = False):
+def getAll(styles = True, artists = True, output = True):
     base_url = 'http://everynoise.com/'
     result = {}
 
     artistsArr = []
     stylesArr = []
 
     response = requests.get(base_url)
@@ -47,19 +47,15 @@
 
                 remove_duplicates(result)
 
                 with open(name + ".json", 'w', encoding="utf-8") as f:
                     json.dump(result, f, ensure_ascii=False)
         
 
-    # for styleElement in stylesResult:
-    for i, styleElement in enumerate(stylesResult):
-        if i == 6:
-            break
-
+    for styleElement in stylesResult:
         styleNameRaw = styleElement.text
         styleName = styleNameRaw[:-2]
 
 
         artistLink = styleElement.find('a')['href']
         artistsUrl = base_url + artistLink
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

