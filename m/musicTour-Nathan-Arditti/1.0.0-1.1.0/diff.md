# Comparing `tmp/musicTour_Nathan_Arditti-1.0.0.tar.gz` & `tmp/musicTour_Nathan_Arditti-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicTour_Nathan_Arditti-1.0.0.tar", last modified: Wed May 24 12:39:44 2023, max compression
+gzip compressed data, was "musicTour_Nathan_Arditti-1.1.0.tar", last modified: Wed May 24 13:45:32 2023, max compression
```

## Comparing `musicTour_Nathan_Arditti-1.0.0.tar` & `musicTour_Nathan_Arditti-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 12:39:44.331386 musicTour_Nathan_Arditti-1.0.0/
--rw-rw-rw-   0        0        0     1067 2023-05-24 11:26:32.000000 musicTour_Nathan_Arditti-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      545 2023-05-24 12:39:44.331386 musicTour_Nathan_Arditti-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       53 2023-05-24 11:07:35.000000 musicTour_Nathan_Arditti-1.0.0/README.md
--rw-rw-rw-   0        0        0      484 2023-05-24 11:59:47.000000 musicTour_Nathan_Arditti-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 12:39:44.331386 musicTour_Nathan_Arditti-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-24 12:39:44.320403 musicTour_Nathan_Arditti-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 12:39:44.325386 musicTour_Nathan_Arditti-1.0.0/src/musicTour/
--rw-rw-rw-   0        0        0       33 2023-05-24 11:38:35.000000 musicTour_Nathan_Arditti-1.0.0/src/musicTour/__init__.py
--rw-rw-rw-   0        0        0     4807 2023-05-24 12:38:18.000000 musicTour_Nathan_Arditti-1.0.0/src/musicTour/musicTour.py
-drwxrwxrwx   0        0        0        0 2023-05-24 12:39:44.330386 musicTour_Nathan_Arditti-1.0.0/src/musicTour_Nathan_Arditti.egg-info/
--rw-rw-rw-   0        0        0      545 2023-05-24 12:39:44.000000 musicTour_Nathan_Arditti-1.0.0/src/musicTour_Nathan_Arditti.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-05-24 12:39:44.000000 musicTour_Nathan_Arditti-1.0.0/src/musicTour_Nathan_Arditti.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 12:39:44.000000 musicTour_Nathan_Arditti-1.0.0/src/musicTour_Nathan_Arditti.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-24 12:39:44.000000 musicTour_Nathan_Arditti-1.0.0/src/musicTour_Nathan_Arditti.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 13:45:32.783112 musicTour_Nathan_Arditti-1.1.0/
+-rw-rw-rw-   0        0        0     1067 2023-05-24 11:26:32.000000 musicTour_Nathan_Arditti-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      545 2023-05-24 13:45:32.781562 musicTour_Nathan_Arditti-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2023-05-24 11:07:35.000000 musicTour_Nathan_Arditti-1.1.0/README.md
+-rw-rw-rw-   0        0        0      484 2023-05-24 13:45:13.000000 musicTour_Nathan_Arditti-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 13:45:32.783112 musicTour_Nathan_Arditti-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 13:45:32.750280 musicTour_Nathan_Arditti-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 13:45:32.774563 musicTour_Nathan_Arditti-1.1.0/src/musicTour/
+-rw-rw-rw-   0        0        0       33 2023-05-24 11:38:35.000000 musicTour_Nathan_Arditti-1.1.0/src/musicTour/__init__.py
+-rw-rw-rw-   0        0        0     4472 2023-05-24 13:34:28.000000 musicTour_Nathan_Arditti-1.1.0/src/musicTour/musicTour.py
+drwxrwxrwx   0        0        0        0 2023-05-24 13:45:32.780563 musicTour_Nathan_Arditti-1.1.0/src/musicTour_Nathan_Arditti.egg-info/
+-rw-rw-rw-   0        0        0      545 2023-05-24 13:45:32.000000 musicTour_Nathan_Arditti-1.1.0/src/musicTour_Nathan_Arditti.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-05-24 13:45:32.000000 musicTour_Nathan_Arditti-1.1.0/src/musicTour_Nathan_Arditti.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 13:45:32.000000 musicTour_Nathan_Arditti-1.1.0/src/musicTour_Nathan_Arditti.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-24 13:45:32.000000 musicTour_Nathan_Arditti-1.1.0/src/musicTour_Nathan_Arditti.egg-info/top_level.txt
```

### Comparing `musicTour_Nathan_Arditti-1.0.0/LICENSE.txt` & `musicTour_Nathan_Arditti-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `musicTour_Nathan_Arditti-1.0.0/PKG-INFO` & `musicTour_Nathan_Arditti-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicTour_Nathan_Arditti
-Version: 1.0.0
+Version: 1.1.0
 Summary: Get all the artists and/or all styles of the world
 Author-email: Nathan Arditti <nath.arditti@yahoo.fr>
 Project-URL: Homepage, https://github.com/SnowDhrop/musicTour
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `musicTour_Nathan_Arditti-1.0.0/src/musicTour/musicTour.py` & `musicTour_Nathan_Arditti-1.1.0/src/musicTour/musicTour.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,51 +92,39 @@
         # print('Style:', style_name)
 
     # print(result)
 
     if (output == True):
         name = "all"
 
-        def return_json(style, artist, name, newName, result):
-            if (styles == style and artists == artist):
-                name += newName
-
-                remove_duplicates(result)
-
-                with open(name + ".json", 'w', encoding="utf-8") as f:
-                    json.dump(result, f, ensure_ascii=False)
-
         if (styles == True and artists == False):
             name += "Styles"
-
             remove_duplicates(stylesArr)
 
             with open(name + ".json", 'w', encoding="utf-8") as f:
                     json.dump(stylesArr, f, ensure_ascii=False)
 
-        if (styles == False and artists == True):
+        elif (styles == False and artists == True):
             name += "Artists"
-
             remove_duplicates(artistsArr)
 
             with open(name + ".json", 'w', encoding="utf-8") as f:
                     json.dump(artistsArr, f, ensure_ascii=False)
 
-        if (styles == True and artists == True):
+        elif (styles == True and artists == True):
             name += "StylesArtists"
-
             remove_duplicates(result)
 
             with open(name + ".json", 'w', encoding="utf-8") as f:
                     json.dump(result, f, ensure_ascii=False)
 
     else: 
         if (styles == True and artists == False) :
             return stylesArr        
         
-        if (styles == False and artists == True) :
+        elif (styles == False and artists == True) :
             return artistsArr    
         
-        if (styles == True and artists == True) :
+        elif (styles == True and artists == True) :
             return result    
 
 getAll(True, True, True)
```

### Comparing `musicTour_Nathan_Arditti-1.0.0/src/musicTour_Nathan_Arditti.egg-info/PKG-INFO` & `musicTour_Nathan_Arditti-1.1.0/src/musicTour_Nathan_Arditti.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicTour-Nathan-Arditti
-Version: 1.0.0
+Version: 1.1.0
 Summary: Get all the artists and/or all styles of the world
 Author-email: Nathan Arditti <nath.arditti@yahoo.fr>
 Project-URL: Homepage, https://github.com/SnowDhrop/musicTour
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

