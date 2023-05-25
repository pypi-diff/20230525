# Comparing `tmp/neuralint-0.0.3.tar.gz` & `tmp/neuralint-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\neuralint-0.0.3.tar", last modified: Wed May 24 21:35:23 2023, max compression
+gzip compressed data, was "dist\neuralint-0.0.4.tar", last modified: Thu May 25 15:29:45 2023, max compression
```

## Comparing `neuralint-0.0.3.tar` & `neuralint-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 21:35:23.694762 neuralint-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-05-24 21:35:23.679125 neuralint-0.0.3/Neuralint/
--rw-rw-rw-   0        0        0       25 2023-05-24 21:34:18.000000 neuralint-0.0.3/Neuralint/__init__.py
--rw-rw-rw-   0        0        0     3934 2023-05-24 16:22:31.000000 neuralint-0.0.3/Neuralint/endToEnd.py
--rw-rw-rw-   0        0        0     9648 2023-05-19 18:51:52.000000 neuralint-0.0.3/Neuralint/grooveParser.py
--rw-rw-rw-   0        0        0     4840 2023-05-19 18:51:52.000000 neuralint-0.0.3/Neuralint/mix_bugs_1.py
--rw-rw-rw-   0        0        0    63375 2023-05-19 18:51:52.000000 neuralint-0.0.3/Neuralint/nodes_Keras.py
--rw-rw-rw-   0        0        0    60891 2023-05-19 18:51:52.000000 neuralint-0.0.3/Neuralint/nodes_TF.py
--rw-rw-rw-   0        0        0    11164 2023-05-19 18:51:52.000000 neuralint-0.0.3/Neuralint/parser_Keras.py
--rw-rw-rw-   0        0        0     9675 2023-05-19 18:51:52.000000 neuralint-0.0.3/Neuralint/parser_TF.py
--rw-rw-rw-   0        0        0      582 2023-05-24 21:35:23.694762 neuralint-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-24 21:35:23.694762 neuralint-0.0.3/neuralint.egg-info/
--rw-rw-rw-   0        0        0      582 2023-05-24 21:35:23.000000 neuralint-0.0.3/neuralint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-05-24 21:35:23.000000 neuralint-0.0.3/neuralint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 21:35:23.000000 neuralint-0.0.3/neuralint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-24 21:35:23.000000 neuralint-0.0.3/neuralint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-24 21:35:23.000000 neuralint-0.0.3/neuralint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 21:35:23.694762 neuralint-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      844 2023-05-24 21:35:17.000000 neuralint-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:29:45.180610 neuralint-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-05-25 15:29:45.160538 neuralint-0.0.4/Neuralint/
+-rw-rw-rw-   0        0        0       25 2023-05-24 21:43:08.000000 neuralint-0.0.4/Neuralint/__init__.py
+-rw-rw-rw-   0        0        0     4151 2023-05-25 15:15:40.000000 neuralint-0.0.4/Neuralint/endToEnd.py
+-rw-rw-rw-   0        0        0     9648 2023-05-19 18:51:52.000000 neuralint-0.0.4/Neuralint/grooveParser.py
+-rw-rw-rw-   0        0        0     4840 2023-05-19 18:51:52.000000 neuralint-0.0.4/Neuralint/mix_bugs_1.py
+-rw-rw-rw-   0        0        0    63375 2023-05-19 18:51:52.000000 neuralint-0.0.4/Neuralint/nodes_Keras.py
+-rw-rw-rw-   0        0        0    60891 2023-05-19 18:51:52.000000 neuralint-0.0.4/Neuralint/nodes_TF.py
+-rw-rw-rw-   0        0        0    11164 2023-05-19 18:51:52.000000 neuralint-0.0.4/Neuralint/parser_Keras.py
+-rw-rw-rw-   0        0        0     9675 2023-05-19 18:51:52.000000 neuralint-0.0.4/Neuralint/parser_TF.py
+-rw-rw-rw-   0        0        0      582 2023-05-25 15:29:45.180610 neuralint-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-25 15:29:45.180610 neuralint-0.0.4/neuralint.egg-info/
+-rw-rw-rw-   0        0        0      582 2023-05-25 15:29:45.000000 neuralint-0.0.4/neuralint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-05-25 15:29:45.000000 neuralint-0.0.4/neuralint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 15:29:45.000000 neuralint-0.0.4/neuralint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-25 15:29:45.000000 neuralint-0.0.4/neuralint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-25 15:29:45.000000 neuralint-0.0.4/neuralint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 15:29:45.180610 neuralint-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      844 2023-05-25 15:29:38.000000 neuralint-0.0.4/setup.py
```

### Comparing `neuralint-0.0.3/Neuralint/endToEnd.py` & `neuralint-0.0.4/Neuralint/endToEnd.py`

 * *Files 12% similar despite different names*

```diff
@@ -68,27 +68,37 @@
         return False
     inOut = inOut[1:len(inOut)-1]
     inOutList = inOut.split(",")
     inOutList = list(map(int, inOutList))
 
     return inOutList
 
-def main(file_folderName,inputSize,outputSize,parserName,resultFileName):
-    if inputSize == False or outputSize==False:
-        raise SystemExit("Error : Input and output size should be entered as array([x1, x2, x3, ...]).")
-    parserName=parserName.lower()
-    if parserName != "tf" and parserName != "keras":
-        raise SystemExit("Error : Parser type should be 'tf' or 'keras'")
+def main():
+    arguments = sys.argv
+    if len(arguments) != 6:
+        raise SystemExit('usage: endToEnd.py [input filename] [input size] [output size] [parser type] [output filename]')
+    else:
+        file_folderName = arguments[1]
+        inputSize = checkInOutSize(arguments[2])
+        outputSize = checkInOutSize(arguments[3])
+
+        if inputSize == False or outputSize==False:
+            raise SystemExit("Error : Input and output size should be entered as array([x1, x2, x3, ...]).")
+
+        parserName = arguments[4].lower()
+        resultFileName = arguments[5]
+        if parserName != "tf" and parserName != "keras":
+            raise SystemExit("Error : Parser type should be 'tf' or 'keras'")
     try:
         outputFile = open(f"{resultFileName}.txt" ,"w", encoding="ISO-8859-1")
     except IOError:
         raise SystemExit("Error : output filename should meet host operating system filename rules")
+
     extention = os.path.splitext(file_folderName)[1]
+
     if extention == ".py":
         output = parsDnnScript(fileName = os.path.splitext(file_folderName)[0], inputSize = inputSize ,outputSize = outputSize , parser=parserName)
         outputFile.write(output)
     else:
         raise SystemExit("Error : input should be a python script file")
-    
 if __name__ == '__main__':
-    main(file_folderName="mix_bugs_1.py",inputSize=[32,28,28,1],outputSize=[32,10],parserName="tf",resultFileName="result")
-
+    main()
```

### Comparing `neuralint-0.0.3/Neuralint/grooveParser.py` & `neuralint-0.0.4/Neuralint/grooveParser.py`

 * *Files identical despite different names*

### Comparing `neuralint-0.0.3/Neuralint/mix_bugs_1.py` & `neuralint-0.0.4/Neuralint/mix_bugs_1.py`

 * *Files identical despite different names*

### Comparing `neuralint-0.0.3/Neuralint/nodes_Keras.py` & `neuralint-0.0.4/Neuralint/nodes_Keras.py`

 * *Files identical despite different names*

### Comparing `neuralint-0.0.3/Neuralint/nodes_TF.py` & `neuralint-0.0.4/Neuralint/nodes_TF.py`

 * *Files identical despite different names*

### Comparing `neuralint-0.0.3/Neuralint/parser_Keras.py` & `neuralint-0.0.4/Neuralint/parser_Keras.py`

 * *Files identical despite different names*

### Comparing `neuralint-0.0.3/Neuralint/parser_TF.py` & `neuralint-0.0.4/Neuralint/parser_TF.py`

 * *Files identical despite different names*

### Comparing `neuralint-0.0.3/PKG-INFO` & `neuralint-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralint
-Version: 0.0.3
+Version: 0.0.4
 Summary: Neuralint package
 Home-page: UNKNOWN
 Author: Poly
 Author-email: <ghassendaoud99@gmail.com>
 License: UNKNOWN
 Description: Neuralint package.
 Keywords: python,cnn,test
```

### Comparing `neuralint-0.0.3/neuralint.egg-info/PKG-INFO` & `neuralint-0.0.4/neuralint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralint
-Version: 0.0.3
+Version: 0.0.4
 Summary: Neuralint package
 Home-page: UNKNOWN
 Author: Poly
 Author-email: <ghassendaoud99@gmail.com>
 License: UNKNOWN
 Description: Neuralint package.
 Keywords: python,cnn,test
```

### Comparing `neuralint-0.0.3/setup.py` & `neuralint-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Neuralint package'
 LONG_DESCRIPTION = 'Neuralint package.'
 
 # Setting up
 setup(
     name="neuralint",
     version=VERSION,
```

