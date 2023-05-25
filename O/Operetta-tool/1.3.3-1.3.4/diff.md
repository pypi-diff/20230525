# Comparing `tmp/Operetta_tool-1.3.3.tar.gz` & `tmp/Operetta_tool-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Operetta_tool-1.3.3.tar", last modified: Wed May 24 10:40:00 2023, max compression
+gzip compressed data, was "Operetta_tool-1.3.4.tar", last modified: Thu May 25 17:51:48 2023, max compression
```

## Comparing `Operetta_tool-1.3.3.tar` & `Operetta_tool-1.3.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 10:40:00.711283 Operetta_tool-1.3.3/
--rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 Operetta_tool-1.3.3/LICENSE
--rw-rw-rw-   0        0        0       28 2023-03-16 18:37:03.000000 Operetta_tool-1.3.3/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-24 10:40:00.703339 Operetta_tool-1.3.3/Operetta_tool.egg-info/
--rw-rw-rw-   0        0        0      725 2023-05-24 10:39:59.000000 Operetta_tool-1.3.3/Operetta_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-05-24 10:40:00.000000 Operetta_tool-1.3.3/Operetta_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 10:39:59.000000 Operetta_tool-1.3.3/Operetta_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-05-24 10:40:00.000000 Operetta_tool-1.3.3/Operetta_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-24 10:40:00.000000 Operetta_tool-1.3.3/Operetta_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      725 2023-05-24 10:40:00.711283 Operetta_tool-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    11126 2023-03-20 21:02:31.000000 Operetta_tool-1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 10:40:00.710291 Operetta_tool-1.3.3/operetta/
--rw-rw-rw-   0        0        0      153 2023-05-24 10:38:15.000000 Operetta_tool-1.3.3/operetta/__init__.py
--rw-rw-rw-   0        0        0   261950 2023-03-14 17:41:39.000000 Operetta_tool-1.3.3/operetta/jbsicon.ico
--rw-rw-rw-   0        0        0    51061 2023-05-24 10:37:03.000000 Operetta_tool-1.3.3/operetta/operetta_annotation.py
--rw-rw-rw-   0        0        0       42 2023-05-24 10:40:00.711283 Operetta_tool-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1276 2023-05-24 10:37:56.000000 Operetta_tool-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:51:48.169333 Operetta_tool-1.3.4/
+-rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 Operetta_tool-1.3.4/LICENSE
+-rw-rw-rw-   0        0        0       28 2023-03-16 18:37:03.000000 Operetta_tool-1.3.4/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-25 17:51:48.153350 Operetta_tool-1.3.4/Operetta_tool.egg-info/
+-rw-rw-rw-   0        0        0      725 2023-05-25 17:51:46.000000 Operetta_tool-1.3.4/Operetta_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-05-25 17:51:47.000000 Operetta_tool-1.3.4/Operetta_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 17:51:46.000000 Operetta_tool-1.3.4/Operetta_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-05-25 17:51:47.000000 Operetta_tool-1.3.4/Operetta_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-25 17:51:47.000000 Operetta_tool-1.3.4/Operetta_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      725 2023-05-25 17:51:48.169333 Operetta_tool-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11126 2023-03-20 21:02:31.000000 Operetta_tool-1.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 17:51:48.169333 Operetta_tool-1.3.4/operetta/
+-rw-rw-rw-   0        0        0      153 2023-05-25 17:51:03.000000 Operetta_tool-1.3.4/operetta/__init__.py
+-rw-rw-rw-   0        0        0   261950 2023-03-14 17:41:39.000000 Operetta_tool-1.3.4/operetta/jbsicon.ico
+-rw-rw-rw-   0        0        0    52247 2023-05-25 17:47:22.000000 Operetta_tool-1.3.4/operetta/operetta_annotation.py
+-rw-rw-rw-   0        0        0       42 2023-05-25 17:51:48.169333 Operetta_tool-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1276 2023-05-25 17:50:56.000000 Operetta_tool-1.3.4/setup.py
```

### Comparing `Operetta_tool-1.3.3/LICENSE` & `Operetta_tool-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.3.3/Operetta_tool.egg-info/PKG-INFO` & `Operetta_tool-1.3.4/Operetta_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Operetta-tool
-Version: 1.3.3
+Version: 1.3.4
 Summary: operetta_tool
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: python,opera,images,annotation,AI,cv,perkin
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Operetta_tool-1.3.3/PKG-INFO` & `Operetta_tool-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Operetta_tool
-Version: 1.3.3
+Version: 1.3.4
 Summary: operetta_tool
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: python,opera,images,annotation,AI,cv,perkin
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Operetta_tool-1.3.3/README.md` & `Operetta_tool-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.3.3/operetta/jbsicon.ico` & `Operetta_tool-1.3.4/operetta/jbsicon.ico`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.3.3/operetta/operetta_annotation.py` & `Operetta_tool-1.3.4/operetta/operetta_annotation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1138,26 +1138,60 @@
                 
     except:
         print("Something went wrong. Check the function input data and try again!")
             
             
             
             
-     
 def add_scalebar(image, metadata):
 
     try:
         global image2
         global met
         
         met = metadata.copy()
 
         image2 = image.copy()
         
-       
+        h = image2.shape[0]
+        w = image2.shape[1]
+        
+        
+        if w > 20000:
+            rw = 20000/w
+            
+            nw = int(w*rw)
+            nh = int(h*rw)
+            
+            image2 = cv2.resize(image2, (nw, nh))
+            metadata['X_resolution[m]'][0] = metadata['X_resolution[m]'][0]*rw
+            metadata['Y_resolution[m]'][0] = metadata['X_resolution[m]'][0]*rw
+            h = image2.shape[0]
+            w = image2.shape[1]
+    
+                               
+        if h > 20000:
+            rh = 20000/h
+            
+            nw = int(w*rh)
+            nh = int(h*rh)
+            
+            image2 = cv2.resize(image2, (nw, nh))
+            metadata['X_resolution[m]'][0] = metadata['X_resolution[m]'][0]*rh
+            metadata['Y_resolution[m]'][0] = metadata['X_resolution[m]'][0]*rh
+            h = image2.shape[0]
+            w = image2.shape[1]
+           
+                                
+        if w != image2.shape[0] or h != image2.shape[0]:
+            print('Resolution of the image wass too large')
+            print('Current resolution is ' + str(nw) + 'x' + str(nh))
+
+            
+        
         window = tk.Tk()
         
         window.geometry("500x800")
         window.title("SCALE-BAR")
     
         window.iconbitmap(pkg_resources.resource_filename("operetta", "jbsicon.ico"))
        
@@ -1423,8 +1457,8 @@
     
         cv2.destroyAllWindows()
     
         
         return image3
 
     except:
-        print("Something went wrong. Check the function input data and try again!")
+        print("Something went wrong. Check the function input data and try again!")
```

### Comparing `Operetta_tool-1.3.3/setup.py` & `Operetta_tool-1.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.3.3' 
+VERSION = '1.3.4' 
 DESCRIPTION = 'operetta_tool'
 LONG_DESCRIPTION = 'The Operetta_tool is a python library created for handling and annotation images from the Opera Phenix platform used for ML / AI applications. Instructions for use on github [https://github.com/jkubis96/Operetta_tool] '
 
 # Setting up
 setup(
         name="Operetta_tool", 
         version=VERSION,
```

