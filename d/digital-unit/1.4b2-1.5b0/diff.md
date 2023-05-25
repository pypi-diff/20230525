# Comparing `tmp/digital_unit-1.4b2.tar.gz` & `tmp/digital_unit-1.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital_unit-1.4b2.tar", last modified: Wed May 24 13:49:31 2023, max compression
+gzip compressed data, was "digital_unit-1.5b0.tar", last modified: Thu May 25 14:15:13 2023, max compression
```

## Comparing `digital_unit-1.4b2.tar` & `digital_unit-1.5b0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 13:49:30.998886 digital_unit-1.4b2/
--rw-rw-rw-   0        0        0      240 2023-05-24 13:49:30.997887 digital_unit-1.4b2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-24 13:49:30.977997 digital_unit-1.4b2/digital_unit/
--rw-rw-rw-   0        0        0      827 2023-05-24 12:55:31.000000 digital_unit-1.4b2/digital_unit/Area.py
--rw-rw-rw-   0        0        0      797 2023-05-24 12:55:26.000000 digital_unit-1.4b2/digital_unit/Lenth.py
--rw-rw-rw-   0        0        0      134 2023-04-16 13:27:44.000000 digital_unit-1.4b2/digital_unit/__init__.py
--rw-rw-rw-   0        0        0      976 2023-04-16 12:22:16.000000 digital_unit-1.4b2/digital_unit/root.py
--rw-rw-rw-   0        0        0      305 2023-04-16 13:27:53.000000 digital_unit-1.4b2/digital_unit/sample.py
-drwxrwxrwx   0        0        0        0 2023-05-24 13:49:30.994873 digital_unit-1.4b2/digital_unit.egg-info/
--rw-rw-rw-   0        0        0      240 2023-05-24 13:49:30.000000 digital_unit-1.4b2/digital_unit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-24 13:49:30.000000 digital_unit-1.4b2/digital_unit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 13:49:30.000000 digital_unit-1.4b2/digital_unit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-24 13:49:30.000000 digital_unit-1.4b2/digital_unit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 13:49:30.999887 digital_unit-1.4b2/setup.cfg
--rw-rw-rw-   0        0        0      776 2023-05-24 13:49:06.000000 digital_unit-1.4b2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:15:13.849369 digital_unit-1.5b0/
+-rw-rw-rw-   0        0        0      240 2023-05-25 14:15:13.848379 digital_unit-1.5b0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-25 14:15:13.831365 digital_unit-1.5b0/digital_unit/
+-rw-rw-rw-   0        0        0      827 2023-05-24 12:55:31.000000 digital_unit-1.5b0/digital_unit/Area.py
+-rw-rw-rw-   0        0        0      797 2023-05-24 12:55:26.000000 digital_unit-1.5b0/digital_unit/Lenth.py
+-rw-rw-rw-   0        0        0      169 2023-05-25 14:12:42.000000 digital_unit-1.5b0/digital_unit/__init__.py
+-rw-rw-rw-   0        0        0     1050 2023-05-24 14:05:13.000000 digital_unit-1.5b0/digital_unit/root.py
+-rw-rw-rw-   0        0        0      330 2023-05-25 13:54:40.000000 digital_unit-1.5b0/digital_unit/sample.py
+-rw-rw-rw-   0        0        0      294 2023-05-25 14:15:08.000000 digital_unit-1.5b0/digital_unit/volume.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:15:13.845265 digital_unit-1.5b0/digital_unit.egg-info/
+-rw-rw-rw-   0        0        0      240 2023-05-25 14:15:13.000000 digital_unit-1.5b0/digital_unit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-25 14:15:13.000000 digital_unit-1.5b0/digital_unit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 14:15:13.000000 digital_unit-1.5b0/digital_unit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-25 14:15:13.000000 digital_unit-1.5b0/digital_unit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 14:15:13.850380 digital_unit-1.5b0/setup.cfg
+-rw-rw-rw-   0        0        0      776 2023-05-25 14:08:23.000000 digital_unit-1.5b0/setup.py
```

### Comparing `digital_unit-1.4b2/digital_unit/Area.py` & `digital_unit-1.5b0/digital_unit/Area.py`

 * *Files identical despite different names*

### Comparing `digital_unit-1.4b2/digital_unit/Lenth.py` & `digital_unit-1.5b0/digital_unit/Lenth.py`

 * *Files identical despite different names*

### Comparing `digital_unit-1.4b2/digital_unit/root.py` & `digital_unit-1.5b0/digital_unit/root.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 class DigitalUnit:
     def __init__(self) -> None:
         self.type = "NONE"
 
 
 class Number:
-    def __init__(self, number, unit) -> None:
+    def __init__(self, number : float, unit:DigitalUnit) -> None:
         self.digital_part = number
         if unit.__class__.__base__.__base__ == DigitalUnit:
             self.unit = unit
         else:
             print(unit.__class__.__base__.__base__)
             raise TypeError('You should set the unit parameter to numerical units.')
 
@@ -19,8 +19,11 @@
                 self.unit = new_unit
             else:
                 raise TypeError('Different unit types')
         else:
             raise TypeError('You should set the unit parameter to numerical units.')
     
     def __str__(self) -> str:
-        return f'{self.digital_part}{self.unit}'
+        return f'{self.digital_part}{self.unit}'
+    
+    def __abs__():
+        return abs(Number)
```

### Comparing `digital_unit-1.4b2/setup.py` & `digital_unit-1.5b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'digital_unit',         # How you named your package folder (MyLib)
   packages = ['digital_unit'],   # Chose the same as "name"
-  version = '1.4b2',      # Start with a small number and increase it with every change you make
+  version = '1.5b0',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'number and units',   # Give a short description about your library
   author = 'st201109',                   # Type in your name
   author_email = 'st20110913@outlook.com',      # Type in your E-Mail
   
   keywords = ['SOME', 'MEANINGFULL', 'MATH'],   # Keywords that define your package best
```

