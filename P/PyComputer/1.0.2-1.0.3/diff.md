# Comparing `tmp/PyComputer-1.0.2.tar.gz` & `tmp/PyComputer-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyComputer-1.0.2.tar", last modified: Tue May 23 03:54:25 2023, max compression
+gzip compressed data, was "PyComputer-1.0.3.tar", last modified: Thu May 25 12:27:30 2023, max compression
```

## Comparing `PyComputer-1.0.2.tar` & `PyComputer-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 03:54:25.792131 PyComputer-1.0.2/
--rw-rw-rw-   0        0        0      602 2023-05-23 03:51:40.000000 PyComputer-1.0.2/CREDITS.md
--rw-rw-rw-   0        0        0     1091 2023-05-16 07:22:16.000000 PyComputer-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       98 2023-05-23 03:32:25.000000 PyComputer-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2689 2023-05-23 03:54:25.791133 PyComputer-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-23 03:54:25.760216 PyComputer-1.0.2/PyComputer/
--rw-rw-rw-   0        0        0      453 2023-05-23 03:27:34.000000 PyComputer-1.0.2/PyComputer/Brightness.py
--rw-rw-rw-   0        0        0     1339 2023-05-23 03:25:52.000000 PyComputer-1.0.2/PyComputer/Volume.py
--rw-rw-rw-   0        0        0       60 2023-05-23 02:07:40.000000 PyComputer-1.0.2/PyComputer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 03:54:25.783196 PyComputer-1.0.2/PyComputer/assets/
--rwxrwxrwx   0        0        0   899784 2023-05-23 02:05:42.000000 PyComputer-1.0.2/PyComputer/assets/SetVol.exe
-drwxrwxrwx   0        0        0        0 2023-05-23 03:54:25.777171 PyComputer-1.0.2/PyComputer.egg-info/
--rw-rw-rw-   0        0        0     2689 2023-05-23 03:54:25.000000 PyComputer-1.0.2/PyComputer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-05-23 03:54:25.000000 PyComputer-1.0.2/PyComputer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 03:54:25.000000 PyComputer-1.0.2/PyComputer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-23 03:54:25.000000 PyComputer-1.0.2/PyComputer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-23 03:54:25.000000 PyComputer-1.0.2/PyComputer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2097 2023-05-23 03:53:34.000000 PyComputer-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-23 03:54:25.793128 PyComputer-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1136 2023-05-23 03:53:38.000000 PyComputer-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:27:30.322836 PyComputer-1.0.3/
+-rw-rw-rw-   0        0        0      602 2023-05-23 03:51:40.000000 PyComputer-1.0.3/CREDITS.md
+-rw-rw-rw-   0        0        0     1091 2023-05-16 07:22:16.000000 PyComputer-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       98 2023-05-23 03:32:25.000000 PyComputer-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2689 2023-05-25 12:27:30.321853 PyComputer-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-25 12:27:30.279953 PyComputer-1.0.3/PyComputer/
+-rw-rw-rw-   0        0        0      455 2023-05-25 12:24:09.000000 PyComputer-1.0.3/PyComputer/Brightness.py
+-rw-rw-rw-   0        0        0      462 2023-05-23 16:49:19.000000 PyComputer-1.0.3/PyComputer/System.py
+-rw-rw-rw-   0        0        0     1339 2023-05-25 12:25:57.000000 PyComputer-1.0.3/PyComputer/Volume.py
+-rw-rw-rw-   0        0        0       60 2023-05-23 02:07:40.000000 PyComputer-1.0.3/PyComputer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:27:30.295910 PyComputer-1.0.3/PyComputer/assets/
+-rwxrwxrwx   0        0        0   899784 2023-05-23 02:05:42.000000 PyComputer-1.0.3/PyComputer/assets/SetVol.exe
+drwxrwxrwx   0        0        0        0 2023-05-25 12:27:30.292916 PyComputer-1.0.3/PyComputer.egg-info/
+-rw-rw-rw-   0        0        0     2689 2023-05-25 12:27:30.000000 PyComputer-1.0.3/PyComputer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-05-25 12:27:30.000000 PyComputer-1.0.3/PyComputer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 12:27:30.000000 PyComputer-1.0.3/PyComputer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-25 12:27:30.000000 PyComputer-1.0.3/PyComputer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-25 12:27:30.000000 PyComputer-1.0.3/PyComputer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2097 2023-05-25 12:18:26.000000 PyComputer-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-25 12:27:30.323834 PyComputer-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1136 2023-05-25 12:17:42.000000 PyComputer-1.0.3/setup.py
```

### Comparing `PyComputer-1.0.2/CREDITS.md` & `PyComputer-1.0.3/CREDITS.md`

 * *Files identical despite different names*

### Comparing `PyComputer-1.0.2/LICENSE.txt` & `PyComputer-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyComputer-1.0.2/PKG-INFO` & `PyComputer-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComputer
-Version: 1.0.2
+Version: 1.0.3
 Summary: PyComputer is an advanced Python package that manages and alters your computer's settings.
 Home-page: https://github.com/Anikethc/PyComputer
 Download-URL: https://pypi.org/project/PyComputer
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Computer,Settings
@@ -20,15 +20,15 @@
 PyComputer is an advanced Python package that manages and alters your computer's settings.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pycomputer-docs).
 
 ## Package Information
 
 **Name** - PyComputer</br>
-**Version** - 1.0.2</br>
+**Version** - 1.0.3</br>
 **Description** - PyComputer is an advanced Python package that manages and alters your computer's settings.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyComputer](https://github.com/Anikethc/PyComputer)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyComputer](https://pypi.org/project/PyComputer)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pycomputer-docs](https://aniketh-chavare.gitbook.io/pycomputer-docs)
 
 ## License
```

### Comparing `PyComputer-1.0.2/PyComputer/Volume.py` & `PyComputer-1.0.3/PyComputer/Volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # PyComputer - Volume
 
 ''' This is the "Volume" module. '''
 
 # Imports
 import os
 
-# Set Directory
+# The Directory
 directory = os.path.dirname(os.path.realpath(__file__)).replace(os.sep, "/")
 
 # Function 1 - Max
 def max():
     os.chdir(directory + "/assets")
 
     os.system("setvol 100")
```

### Comparing `PyComputer-1.0.2/PyComputer/assets/SetVol.exe` & `PyComputer-1.0.3/PyComputer/assets/SetVol.exe`

 * *Files identical despite different names*

### Comparing `PyComputer-1.0.2/PyComputer.egg-info/PKG-INFO` & `PyComputer-1.0.3/PyComputer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComputer
-Version: 1.0.2
+Version: 1.0.3
 Summary: PyComputer is an advanced Python package that manages and alters your computer's settings.
 Home-page: https://github.com/Anikethc/PyComputer
 Download-URL: https://pypi.org/project/PyComputer
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Computer,Settings
@@ -20,15 +20,15 @@
 PyComputer is an advanced Python package that manages and alters your computer's settings.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pycomputer-docs).
 
 ## Package Information
 
 **Name** - PyComputer</br>
-**Version** - 1.0.2</br>
+**Version** - 1.0.3</br>
 **Description** - PyComputer is an advanced Python package that manages and alters your computer's settings.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyComputer](https://github.com/Anikethc/PyComputer)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyComputer](https://pypi.org/project/PyComputer)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pycomputer-docs](https://aniketh-chavare.gitbook.io/pycomputer-docs)
 
 ## License
```

### Comparing `PyComputer-1.0.2/README.md` & `PyComputer-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PyComputer is an advanced Python package that manages and alters your computer's settings.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pycomputer-docs).
 
 ## Package Information
 
 **Name** - PyComputer</br>
-**Version** - 1.0.2</br>
+**Version** - 1.0.3</br>
 **Description** - PyComputer is an advanced Python package that manages and alters your computer's settings.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyComputer](https://github.com/Anikethc/PyComputer)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyComputer](https://pypi.org/project/PyComputer)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pycomputer-docs](https://aniketh-chavare.gitbook.io/pycomputer-docs)
 
 ## License
```

### Comparing `PyComputer-1.0.2/setup.py` & `PyComputer-1.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PyComputer",
-    version="1.0.2",
+    version="1.0.3",
     description="PyComputer is an advanced Python package that manages and alters your computer's settings.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
```

