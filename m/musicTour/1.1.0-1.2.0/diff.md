# Comparing `tmp/musicTour-1.1.0.tar.gz` & `tmp/musicTour-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicTour-1.1.0.tar", last modified: Thu May 25 06:54:04 2023, max compression
+gzip compressed data, was "musicTour-1.2.0.tar", last modified: Thu May 25 06:59:08 2023, max compression
```

## Comparing `musicTour-1.1.0.tar` & `musicTour-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 06:54:04.768603 musicTour-1.1.0/
--rw-rw-rw-   0        0        0     1067 2023-05-24 11:26:32.000000 musicTour-1.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      530 2023-05-25 06:54:04.767602 musicTour-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       53 2023-05-24 11:07:35.000000 musicTour-1.1.0/README.md
--rw-rw-rw-   0        0        0      469 2023-05-24 14:02:02.000000 musicTour-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 06:54:04.768603 musicTour-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 06:54:04.755310 musicTour-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 06:54:04.762603 musicTour-1.1.0/src/musicTour/
--rw-rw-rw-   0        0        0       33 2023-05-24 11:38:35.000000 musicTour-1.1.0/src/musicTour/__init__.py
--rw-rw-rw-   0        0        0     4381 2023-05-25 06:53:32.000000 musicTour-1.1.0/src/musicTour/musicTour.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:54:04.767602 musicTour-1.1.0/src/musicTour.egg-info/
--rw-rw-rw-   0        0        0      530 2023-05-25 06:54:04.000000 musicTour-1.1.0/src/musicTour.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-05-25 06:54:04.000000 musicTour-1.1.0/src/musicTour.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 06:54:04.000000 musicTour-1.1.0/src/musicTour.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-25 06:54:04.000000 musicTour-1.1.0/src/musicTour.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 06:59:08.529181 musicTour-1.2.0/
+-rw-rw-rw-   0        0        0     1067 2023-05-24 11:26:32.000000 musicTour-1.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      530 2023-05-25 06:59:08.528180 musicTour-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2023-05-24 11:07:35.000000 musicTour-1.2.0/README.md
+-rw-rw-rw-   0        0        0      469 2023-05-25 06:58:09.000000 musicTour-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 06:59:08.529181 musicTour-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 06:59:08.517711 musicTour-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 06:59:08.522766 musicTour-1.2.0/src/musicTour/
+-rw-rw-rw-   0        0        0       33 2023-05-24 11:38:35.000000 musicTour-1.2.0/src/musicTour/__init__.py
+-rw-rw-rw-   0        0        0     4383 2023-05-25 06:57:50.000000 musicTour-1.2.0/src/musicTour/musicTour.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:59:08.527180 musicTour-1.2.0/src/musicTour.egg-info/
+-rw-rw-rw-   0        0        0      530 2023-05-25 06:59:08.000000 musicTour-1.2.0/src/musicTour.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-25 06:59:08.000000 musicTour-1.2.0/src/musicTour.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 06:59:08.000000 musicTour-1.2.0/src/musicTour.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-25 06:59:08.000000 musicTour-1.2.0/src/musicTour.egg-info/top_level.txt
```

### Comparing `musicTour-1.1.0/LICENSE.txt` & `musicTour-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `musicTour-1.1.0/PKG-INFO` & `musicTour-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicTour
-Version: 1.1.0
+Version: 1.2.0
 Summary: Get all the artists and/or all styles of the world
 Author-email: Nathan Arditti <nath.arditti@yahoo.fr>
 Project-URL: Homepage, https://github.com/SnowDhrop/musicTour
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `musicTour-1.1.0/src/musicTour/musicTour.py` & `musicTour-1.2.0/src/musicTour/musicTour.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,8 +117,8 @@
         
         elif (styles == False and artists == True) :
             return artistsArr    
         
         elif (styles == True and artists == True) :
             return result    
 
-getAll(True, True, True)
+# getAll(True, True, True)
```

### Comparing `musicTour-1.1.0/src/musicTour.egg-info/PKG-INFO` & `musicTour-1.2.0/src/musicTour.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicTour
-Version: 1.1.0
+Version: 1.2.0
 Summary: Get all the artists and/or all styles of the world
 Author-email: Nathan Arditti <nath.arditti@yahoo.fr>
 Project-URL: Homepage, https://github.com/SnowDhrop/musicTour
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

