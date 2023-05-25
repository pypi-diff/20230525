# Comparing `tmp/PySciMath-1.5.5.tar.gz` & `tmp/PySciMath-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySciMath-1.5.5.tar", last modified: Mon May 22 12:53:15 2023, max compression
+gzip compressed data, was "PySciMath-1.5.6.tar", last modified: Thu May 25 10:55:08 2023, max compression
```

## Comparing `PySciMath-1.5.5.tar` & `PySciMath-1.5.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 12:53:15.935040 PySciMath-1.5.5/
--rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.5.5/LICENSE.txt
--rw-rw-rw-   0        0        0       38 2023-05-14 06:30:09.000000 PySciMath-1.5.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2616 2023-05-22 12:53:15.933045 PySciMath-1.5.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 12:53:15.887648 PySciMath-1.5.5/PySciMath/
--rw-rw-rw-   0        0        0     2663 2023-05-22 12:48:50.000000 PySciMath-1.5.5/PySciMath/Arithmetic.py
--rw-rw-rw-   0        0        0    22259 2023-05-22 12:49:01.000000 PySciMath-1.5.5/PySciMath/Geometry.py
--rw-rw-rw-   0        0        0      594 2023-05-22 12:49:09.000000 PySciMath-1.5.5/PySciMath/Quadratic.py
--rw-rw-rw-   0        0        0     1262 2023-05-22 12:49:15.000000 PySciMath-1.5.5/PySciMath/Statistics.py
--rw-rw-rw-   0        0        0      554 2023-05-22 12:49:19.000000 PySciMath-1.5.5/PySciMath/Trigonometry.py
--rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.5.5/PySciMath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 12:53:15.930116 PySciMath-1.5.5/PySciMath.egg-info/
--rw-rw-rw-   0        0        0     2616 2023-05-22 12:53:15.000000 PySciMath-1.5.5/PySciMath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-05-22 12:53:15.000000 PySciMath-1.5.5/PySciMath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 12:53:15.000000 PySciMath-1.5.5/PySciMath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-22 12:53:15.000000 PySciMath-1.5.5/PySciMath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2081 2023-05-22 12:51:51.000000 PySciMath-1.5.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 12:53:15.935040 PySciMath-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0      930 2023-05-22 12:51:47.000000 PySciMath-1.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:55:08.686609 PySciMath-1.5.6/
+-rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.5.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       38 2023-05-14 06:30:09.000000 PySciMath-1.5.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2616 2023-05-25 10:55:08.684615 PySciMath-1.5.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-25 10:55:08.664669 PySciMath-1.5.6/PySciMath/
+-rw-rw-rw-   0        0        0     2663 2023-05-22 12:48:50.000000 PySciMath-1.5.6/PySciMath/Arithmetic.py
+-rw-rw-rw-   0        0        0    21993 2023-05-25 10:41:29.000000 PySciMath-1.5.6/PySciMath/Geometry.py
+-rw-rw-rw-   0        0        0      564 2023-05-25 10:41:56.000000 PySciMath-1.5.6/PySciMath/Quadratic.py
+-rw-rw-rw-   0        0        0     1262 2023-05-25 10:42:52.000000 PySciMath-1.5.6/PySciMath/Statistics.py
+-rw-rw-rw-   0        0        0      554 2023-05-22 12:49:19.000000 PySciMath-1.5.6/PySciMath/Trigonometry.py
+-rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.5.6/PySciMath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:55:08.680626 PySciMath-1.5.6/PySciMath.egg-info/
+-rw-rw-rw-   0        0        0     2616 2023-05-25 10:55:08.000000 PySciMath-1.5.6/PySciMath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-05-25 10:55:08.000000 PySciMath-1.5.6/PySciMath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 10:55:08.000000 PySciMath-1.5.6/PySciMath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-25 10:55:08.000000 PySciMath-1.5.6/PySciMath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2081 2023-05-25 10:46:35.000000 PySciMath-1.5.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-25 10:55:08.686609 PySciMath-1.5.6/setup.cfg
+-rw-rw-rw-   0        0        0      930 2023-05-25 10:47:10.000000 PySciMath-1.5.6/setup.py
```

### Comparing `PySciMath-1.5.5/LICENSE.txt` & `PySciMath-1.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.5/PKG-INFO` & `PySciMath-1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.5.5
+Version: 1.5.6
 Summary: PySciMath is a general-purpose Python package to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/PySciMath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Mathematics,Science,Calculations
@@ -18,15 +18,15 @@
 PySciMath is a general-purpose Python package to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Package Information
 
 **Name** - PySciMath</br>
-**Version** - 1.5.5</br>
+**Version** - 1.5.6</br>
 **Description** - PySciMath is a general-purpose Python package to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
```

### Comparing `PySciMath-1.5.5/PySciMath/Arithmetic.py` & `PySciMath-1.5.6/PySciMath/Arithmetic.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.5/PySciMath/Geometry.py` & `PySciMath-1.5.6/PySciMath/Geometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # PySciMath - Geometry
 
 ''' This is the "Geometry" module. '''
 
 # Imports
-import Arithmetic
+import math
 
 # Constants
 pi = 3.14159
 goldenRatio = 1.61803
 
 # Function 1 - Area (Areas and Volumes)
 def area(**kwargs):
@@ -44,15 +44,15 @@
                     else:
                         raise Exception("The 'base' and 'height' arguments must be an integer or float.")
                 else:
                     raise Exception("To check the area of a triangle, the 'base' and 'height' arguments must be present.")
             elif (shape == "circle"): # Circle
                 if ("radius" in keyList):
                     if (isinstance(kwargs["radius"], (int, float))):
-                        return 3.14 * Arithmetic.power(kwargs["radius"], 2)
+                        return 3.14 * math.pow(kwargs["radius"], 2)
                     else:
                         raise Exception("The 'radius' argument must be an integer or float.")
                 else:
                     raise Exception("To check the area of a circle, the 'radius' argument must be present.")
             elif (shape == "parallelogram"): # Parallelogram
                 if ("base" in keyList and "height" in keyList):
                     if (isinstance(kwargs["base"], (int, float)) and isinstance(kwargs["height"], (int, float))):
@@ -93,15 +93,15 @@
     if ("shape" in keyList):
         if (kwargs["shape"] in shapeList):
             shape = kwargs["shape"]
 
             if (shape == "cube"): # Cube
                 if ("side" in keyList):
                     if (isinstance(kwargs["side"], (int, float))):
-                        return Arithmetic.power(kwargs["side"], 3)
+                        return math.pow(kwargs["side"], 3)
                     else:
                         raise Exception("The 'side' argument must be an integer or float.")
                 else:
                     raise Exception("To check the volume of a cube, the 'side' argument must be present.")
             elif (shape == "cuboid"): # Cuboid
                 if ("length" in keyList and "width" in keyList and "height" in keyList):
                     if (isinstance(kwargs["length"], (int, float)) and isinstance(kwargs["width"], (int, float)) and isinstance(kwargs["height"], (int, float))):
@@ -109,39 +109,39 @@
                     else:
                         raise Exception("The 'length', 'width', and 'height' arguments must be an integer or float.")
                 else:
                     raise Exception("To check the volume of a cuboid, the 'length', 'width', and 'height' arguments must be present.")
             elif (shape == "cone"): # Cone
                 if ("raidus" in keyList and "height" in keyList):
                     if (isinstance(kwargs["radius"], (int, float)) and isinstance(kwargs["height"], (int, float))):
-                        return (1/3) * 3.14 * Arithmetic.power(kwargs["radius"], 2) * kwargs["height"]
+                        return (1/3) * 3.14 * math.pow(kwargs["radius"], 2) * kwargs["height"]
                     else:
                         raise Exception("The 'radius' and 'height' arguments must be an integer or float.")
                 else:
                     raise Exception("To check the volume of a cone, the 'radius' and 'height' arguments must be present.")
             elif (shape == "cylinder"): # Cylinder
                 if ("radius" in keyList and "height" in keyList):
                     if (isinstance(kwargs["radius"], (int, float)) and isinstance(kwargs["height"], (int, float))):
-                        return 3.14 * Arithmetic.power(kwargs["radius"], 2) * kwargs["height"]
+                        return 3.14 * math.pow(kwargs["radius"], 2) * kwargs["height"]
                     else:
                         raise Exception("The 'radius' and 'height' arguments must be an integer or float.")
                 else:
                     raise Exception("To check the volume of a cylinder, the 'radius' and 'height' arguments must be present.")
             elif (shape == "sphere"): # Sphere
                 if ("radius" in keyList):
                     if (isinstance(kwargs["radius"], (int, float))):
-                        return (4/3) * 3.14 * Arithmetic.power(kwargs["radius"], 3)
+                        return (4/3) * 3.14 * math.pow(kwargs["radius"], 3)
                     else:
                         raise Exception("The 'radius' argument must be an integer or float.")
                 else:
                     raise Exception("To check the volume of a sphere, the 'radius' argument must be present.")
             elif (shape == "hemisphere"): # Hemisphere
                 if ("radius" in keyList):
                     if (isinstance(kwargs["radius"], (int, float))):
-                        return (2/3) * 3.14 * Arithmetic.power(kwargs["radius"], 3)
+                        return (2/3) * 3.14 * math.pow(kwargs["radius"], 3)
                     else:
                         raise Exception("The 'radius' argument must be an integer or float.")
                 else:
                     raise Exception("To check the volume of a hemisphere, the 'radius' argument must be present.")
             elif (shape == "pyramid"): # Pyramid
                 if ("length" in keyList and "width" in keyList and "height" in keyList):
                     if (isinstance(kwargs["length"], (int, float)) and isinstance(kwargs["width"], (int, float)) and isinstance(kwargs["height"], (int, float))):
@@ -169,21 +169,21 @@
 
             if (shape == "cube"): # Cube
                 if ("side" in keyList):
                     if (isinstance(kwargs["side"], (int, float))):
                         if ("lateral" in keyList):
                             if (isinstance(kwargs["lateral"], bool)):
                                 if (kwargs["lateral"] == True):
-                                    return 4 * Arithmetic.power(side, 2)
+                                    return 4 * math.pow(side, 2)
                                 else:
-                                    return 6 * Arithmetic.power(side, 2)
+                                    return 6 * math.pow(side, 2)
                             else:
                                 raise Exception("The 'lateral' argument must be either True or False.")
                         else:
-                            return 6 * Arithmetic.power(kwargs["side"], 2)
+                            return 6 * math.pow(kwargs["side"], 2)
                     else:
                         raise Exception("The 'side' argument must be an integer or float.")
                 else:
                     raise Exception("To check the surface area of a cube, the 'side' argument must be present.")
             elif (shape == "cuboid"): # Cuboid
                 if ("length" in keyList and "width" in keyList and "height" in keyList):
                     if (isinstance(kwargs["length"], (int, float)) and isinstance(kwargs["width"], (int, float)) and isinstance(kwargs["height"], (int, float))):
@@ -200,15 +200,15 @@
                     else:
                         raise Exception("The 'length', 'width', and 'height' arguments must be an integer or float.")
                 else:
                     raise Exception("To check the surface area of a cuboid, the 'length', 'width', and 'height' arguments must be present.")
             elif (shape == "cone"): # Cone
                 if ("raidus" in keyList and "height" in keyList):
                     if (isinstance(kwargs["radius"], (int, float)) and isinstance(kwargs["height"], (int, float))):
-                        slantHeight = Arithmetic.squareRoot(Arithmetic.power(kwargs["radius"], 2) + Arithmetic.power(kwargs["height"], 2))
+                        slantHeight = math.sqrt(math.pow(kwargs["radius"], 2) + math.pow(kwargs["height"], 2))
 
                         if ("lateral" in keyList):
                             if (isinstance(kwargs["lateral"], bool)):
                                 if (kwargs["lateral"] == True):
                                     return 3.14 * kwargs["radius"] * slantHeight
                                 else:
                                     return 3.14 * kwargs["radius"] * (slantHeight + kwargs["radius"])
@@ -239,38 +239,38 @@
                     raise Exception("To check the surface area of a cylinder, the 'radius' and 'height' arguments must be present.")
             elif (shape == "sphere"): # Sphere
                 if ("radius" in keyList):
                     if (isinstance(kwargs["radius"], (int, float))):
                         if ("lateral" in keyList):
                             if (isinstance(kwargs["lateral"], bool)):
                                 if (kwargs["lateral"] == True):
-                                    return 4 * 3.14 * Arithmetic.power(kwargs["radius"], 2)
+                                    return 4 * 3.14 * math.pow(kwargs["radius"], 2)
                                 else:
-                                    return 4 * 3.14 * Arithmetic.power(kwargs["radius"], 2)
+                                    return 4 * 3.14 * math.pow(kwargs["radius"], 2)
                             else:
                                 raise Exception("The 'lateral' argument must be either True or False.")
                         else:
-                            return 4 * 3.14 * Arithmetic.power(kwargs["radius"], 2)
+                            return 4 * 3.14 * math.pow(kwargs["radius"], 2)
                     else:
                         raise Exception("The 'radius' argument must be an integer or float.")
                 else:
                     raise Exception("To check the surface area of a sphere, the 'radius' argument must be present.")
             elif (shape == "hemisphere"): # Hemisphere
                 if ("radius" in keyList):
                     if (isinstance(kwargs["radius"], (int, float))):
                         if ("lateral" in keyList):
                             if (isinstance(kwargs["lateral"], bool)):
                                 if (kwargs["lateral"] == True):
-                                    return 2 * 3.14 * Arithmetic.power(kwargs["radius"], 2)
+                                    return 2 * 3.14 * math.pow(kwargs["radius"], 2)
                                 else:
-                                    return 3 * 3.14 * Arithmetic.power(kwargs["radius"], 2)
+                                    return 3 * 3.14 * math.pow(kwargs["radius"], 2)
                             else:
                                 raise Exception("The 'lateral' argument must be either True or False.")
                         else:
-                            return 3 * 3.14 * Arithmetic.power(kwargs["radius"], 2)
+                            return 3 * 3.14 * math.pow(kwargs["radius"], 2)
                     else:
                         raise Exception("The 'radius' argument must be an integer or float.")
                 else:
                     raise Exception("To check the surface area of a hemisphere, the 'radius' argument must be present.")
         else:
             raise Exception("The 'shape' argument must be a cube, cuboid, cone, cylinder, sphere, or hemisphere.")
     else:
@@ -288,22 +288,22 @@
             y1 = point1[1]
             y2 = point2[1]
 
             newX = x2 - x1
             newY = y2 - y1
 
             if (len(point1) == 2 and len(point2) == 2): # 2D
-                distance = Arithmetic.squareRoot(Arithmetic.power(newX, 2) + Arithmetic.power(newY, 2))
+                distance = math.sqrt(math.pow(newX, 2) + math.pow(newY, 2))
             else: # 3D
                 z1 = point1[2]
                 z2 = point2[2]
 
                 newZ = z2 - z1
 
-                distance = Arithmetic.squareRoot(Arithmetic.power(newX, 2) + Arithmetic.power(newY, 2) + Arithmetic.power(newZ, 2))
+                distance = math.sqrt(math.pow(newX, 2) + math.pow(newY, 2) + math.pow(newZ, 2))
 
             return distance
         else:
             raise Exception("Both tuples must be in the form (x₁, y₁) and (x₂, y₂) or (x₁, y₁, z₁) and (x₂, y₂, z₂).")
     else:
         raise TypeError("Both Point 1 and Point 2 must be in the form of a tuple.")
 
@@ -375,16 +375,16 @@
             raise TypeError("Point 1, Point 2, and the Ratio must be in the form of a tuple.")
     else:
         raise Exception("The paramater 'typeOfSection' must be either Internal or External.")
 
 # Functions - Circles
 def circumference(radius): return 2 * 3.14 * radius
 def diameter(radius): return 2 * radius
-def areaOfSector(angle, radius): return (angle / 360) * 3.14 * Arithmetic.power(radius, 2)
+def areaOfSector(angle, radius): return (angle / 360) * 3.14 * math.pow(radius, 2)
 def arcLength(angle, radius): return (angle / 360) * circumference(radius)
 
 # Functions - Triangles
-def hypotenuse(side1, side2): return Arithmetic.squareRoot(Arithmetic.power(side1, 2) + Arithmetic.power(side2, 2))
+def hypotenuse(side1, side2): return math.sqrt(math.pow(side1, 2) + math.pow(side2, 2))
 def heronsFormula(side1, side2, side3):
     semiPerimeter = (side1 + side2 + side3) / 2
 
-    return Arithmetic.squareRoot(semiPerimeter * (semiPerimeter - side1) * (semiPerimeter - side2) * (semiPerimeter - side3))
+    return math.sqrt(semiPerimeter * (semiPerimeter - side1) * (semiPerimeter - side2) * (semiPerimeter - side3))
```

### Comparing `PySciMath-1.5.5/PySciMath/Quadratic.py` & `PySciMath-1.5.6/PySciMath/Quadratic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # PySciMath - Quadratic
 
 ''' This is the "Quadratic" module. '''
 
 # Imports
-import Arithmetic
+import math
 
 # Function 1 - Find Discriminant
 def findDiscriminant(a, b, c):
     newA = float(a)
     newB = float(b)
     newC = float(c)
 
@@ -17,11 +17,11 @@
 def findRoots(a, b, c):
     newA = float(a)
     newB = float(b)
     newC = float(c)
 
     discriminant = findDiscriminant(a, b, c)
 
-    alpha = (-newB + Arithmetic.squareRoot(discriminant)) / (2*newA)
-    beta = (-newB - Arithmetic.squareRoot(discriminant)) / (2*newA)
+    alpha = (-newB + math.sqrt(discriminant)) / (2*newA)
+    beta = (-newB - math.sqrt(discriminant)) / (2*newA)
 
     return (alpha, beta)
```

### Comparing `PySciMath-1.5.5/PySciMath/Statistics.py` & `PySciMath-1.5.6/PySciMath/Statistics.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.5/PySciMath/Trigonometry.py` & `PySciMath-1.5.6/PySciMath/Trigonometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.5/PySciMath.egg-info/PKG-INFO` & `PySciMath-1.5.6/PySciMath.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.5.5
+Version: 1.5.6
 Summary: PySciMath is a general-purpose Python package to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/PySciMath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Mathematics,Science,Calculations
@@ -18,15 +18,15 @@
 PySciMath is a general-purpose Python package to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Package Information
 
 **Name** - PySciMath</br>
-**Version** - 1.5.5</br>
+**Version** - 1.5.6</br>
 **Description** - PySciMath is a general-purpose Python package to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
```

### Comparing `PySciMath-1.5.5/README.md` & `PySciMath-1.5.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PySciMath is a general-purpose Python package to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Package Information
 
 **Name** - PySciMath</br>
-**Version** - 1.5.5</br>
+**Version** - 1.5.6</br>
 **Description** - PySciMath is a general-purpose Python package to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
```

### Comparing `PySciMath-1.5.5/setup.py` & `PySciMath-1.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PySciMath",
-    version="1.5.5",
+    version="1.5.6",
     description="PySciMath is a general-purpose Python package to work on calculations and solve mathmematical and scientific problems.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
```

