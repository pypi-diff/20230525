# Comparing `tmp/misuma-0.4.tar.gz` & `tmp/misuma-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misuma-0.4.tar", last modified: Thu May 18 18:17:49 2023, max compression
+gzip compressed data, was "misuma-0.5.tar", last modified: Thu May 25 17:57:26 2023, max compression
```

## Comparing `misuma-0.4.tar` & `misuma-0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-18 18:17:49.015535 misuma-0.4/
--rw-r--r--   0 usuario   (1001) usuario   (1001)     1134 2023-05-16 14:58:24.000000 misuma-0.4/LICENSE
--rw-rw-r--   0 usuario   (1001) usuario   (1001)     2113 2023-05-18 18:17:49.015535 misuma-0.4/PKG-INFO
--rw-r--r--   0 usuario   (1001) usuario   (1001)     1675 2023-05-16 14:58:20.000000 misuma-0.4/README.md
-drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-18 18:17:49.015535 misuma-0.4/misuma/
--rw-r--r--   0 usuario   (1001) usuario   (1001)      500 2023-05-16 14:58:43.000000 misuma-0.4/misuma/__init__.py
-drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-18 18:17:49.015535 misuma-0.4/misuma.egg-info/
--rw-rw-r--   0 usuario   (1001) usuario   (1001)     2113 2023-05-18 18:17:48.000000 misuma-0.4/misuma.egg-info/PKG-INFO
--rw-rw-r--   0 usuario   (1001) usuario   (1001)      244 2023-05-18 18:17:48.000000 misuma-0.4/misuma.egg-info/SOURCES.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)        1 2023-05-18 18:17:48.000000 misuma-0.4/misuma.egg-info/dependency_links.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)       50 2023-05-18 18:17:48.000000 misuma-0.4/misuma.egg-info/entry_points.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)       30 2023-05-18 18:17:48.000000 misuma-0.4/misuma.egg-info/requires.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)        7 2023-05-18 18:17:48.000000 misuma-0.4/misuma.egg-info/top_level.txt
--rw-r--r--   0 usuario   (1001) usuario   (1001)      131 2023-05-16 14:58:32.000000 misuma-0.4/pyproject.toml
--rw-rw-r--   0 usuario   (1001) usuario   (1001)       38 2023-05-18 18:17:49.015535 misuma-0.4/setup.cfg
--rw-r--r--   0 usuario   (1001) usuario   (1001)     2177 2023-05-18 18:00:13.000000 misuma-0.4/setup.py
+drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-25 17:57:26.622624 misuma-0.5/
+-rw-r--r--   0 usuario   (1001) usuario   (1001)     1134 2023-05-16 14:58:24.000000 misuma-0.5/LICENSE
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)     2113 2023-05-25 17:57:26.622624 misuma-0.5/PKG-INFO
+-rw-r--r--   0 usuario   (1001) usuario   (1001)     1675 2023-05-25 17:55:39.000000 misuma-0.5/README.md
+drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-25 17:57:26.622624 misuma-0.5/misuma/
+-rw-r--r--   0 usuario   (1001) usuario   (1001)      222 2023-05-18 18:48:32.000000 misuma-0.5/misuma/__init__.py
+drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-25 17:57:26.622624 misuma-0.5/misuma.egg-info/
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)     2113 2023-05-25 17:57:26.000000 misuma-0.5/misuma.egg-info/PKG-INFO
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)      244 2023-05-25 17:57:26.000000 misuma-0.5/misuma.egg-info/SOURCES.txt
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)        1 2023-05-25 17:57:26.000000 misuma-0.5/misuma.egg-info/dependency_links.txt
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)       50 2023-05-25 17:57:26.000000 misuma-0.5/misuma.egg-info/entry_points.txt
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)       30 2023-05-25 17:57:26.000000 misuma-0.5/misuma.egg-info/requires.txt
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)        7 2023-05-25 17:57:26.000000 misuma-0.5/misuma.egg-info/top_level.txt
+-rw-r--r--   0 usuario   (1001) usuario   (1001)      131 2023-05-16 14:58:32.000000 misuma-0.5/pyproject.toml
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)       38 2023-05-25 17:57:26.622624 misuma-0.5/setup.cfg
+-rw-r--r--   0 usuario   (1001) usuario   (1001)     2177 2023-05-25 17:57:14.000000 misuma-0.5/setup.py
```

### Comparing `misuma-0.4/LICENSE` & `misuma-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `misuma-0.4/PKG-INFO` & `misuma-0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misuma
-Version: 0.4
+Version: 0.5
 Summary: Sum two numbers
 Home-page: https://pypi.org/project/misuma
 Author: Bang1329
 Author-email: santiago.hg2292@gmail.com
 License: MIT
 Keywords: Sum Addition
 Platform: UNKNOWN
@@ -23,16 +23,15 @@
 
 Always start the README explaining clearly what your package do.  If
 you can include here some beautiful image to call the attention of the
 potential user do it!
 
 This is an example:
 
-<p align="center"><img src="https://drive.google.com/uc?export=view&id=1XWnQLEt_oBJjVzMLFVGEAm_uh4zmiYvC" alt="Logo""/></p>
-
+<p align="center"><img src="https://drive.google.com/uc?export=view&id=12WY5E_ImInwi-w0R0LFVG5AIJ5yp3_uL" alt="milogo"></p>
 ## Download and install
 
 Describe here how the package can be downloaded and install it in
 different arquitectures.
 
 If you are using `PyPI` installation it's as simple as:
 
@@ -83,7 +82,8 @@
 
 - First version of the package.
 
 ------------
 
 This package has been designed and written by Fulanit@ de Tal (C) 2023
 
+
```

### Comparing `misuma-0.4/README.md` & `misuma-0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 
 Always start the README explaining clearly what your package do.  If
 you can include here some beautiful image to call the attention of the
 potential user do it!
 
 This is an example:
 
-<p align="center"><img src="https://drive.google.com/uc?export=view&id=1XWnQLEt_oBJjVzMLFVGEAm_uh4zmiYvC" alt="Logo""/></p>
-
+<p align="center"><img src="https://drive.google.com/uc?export=view&id=12WY5E_ImInwi-w0R0LFVG5AIJ5yp3_uL" alt="milogo"></p>
 ## Download and install
 
 Describe here how the package can be downloaded and install it in
 different arquitectures.
 
 If you are using `PyPI` installation it's as simple as:
 
@@ -65,8 +64,8 @@
 
 Version 0.1:
 
 - First version of the package.
 
 ------------
 
-This package has been designed and written by Fulanit@ de Tal (C) 2023
+This package has been designed and written by Fulanit@ de Tal (C) 2023
```

### Comparing `misuma-0.4/misuma.egg-info/PKG-INFO` & `misuma-0.5/misuma.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misuma
-Version: 0.4
+Version: 0.5
 Summary: Sum two numbers
 Home-page: https://pypi.org/project/misuma
 Author: Bang1329
 Author-email: santiago.hg2292@gmail.com
 License: MIT
 Keywords: Sum Addition
 Platform: UNKNOWN
@@ -23,16 +23,15 @@
 
 Always start the README explaining clearly what your package do.  If
 you can include here some beautiful image to call the attention of the
 potential user do it!
 
 This is an example:
 
-<p align="center"><img src="https://drive.google.com/uc?export=view&id=1XWnQLEt_oBJjVzMLFVGEAm_uh4zmiYvC" alt="Logo""/></p>
-
+<p align="center"><img src="https://drive.google.com/uc?export=view&id=12WY5E_ImInwi-w0R0LFVG5AIJ5yp3_uL" alt="milogo"></p>
 ## Download and install
 
 Describe here how the package can be downloaded and install it in
 different arquitectures.
 
 If you are using `PyPI` installation it's as simple as:
 
@@ -83,7 +82,8 @@
 
 - First version of the package.
 
 ------------
 
 This package has been designed and written by Fulanit@ de Tal (C) 2023
 
+
```

### Comparing `misuma-0.4/setup.py` & `misuma-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # CLASSIFIER
     # ######################################################################
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         ],
-    version='0.4',
+    version='0.5',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={'': '.'},
     packages=setuptools.find_packages(where='.'),
```

