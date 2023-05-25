# Comparing `tmp/misuma-0.5.tar.gz` & `tmp/misuma-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misuma-0.5.tar", last modified: Thu May 25 17:57:26 2023, max compression
+gzip compressed data, was "misuma-0.6.tar", last modified: Thu May 25 18:23:43 2023, max compression
```

## Comparing `misuma-0.5.tar` & `misuma-0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-25 17:57:26.622624 misuma-0.5/
--rw-r--r--   0 usuario   (1001) usuario   (1001)     1134 2023-05-16 14:58:24.000000 misuma-0.5/LICENSE
--rw-rw-r--   0 usuario   (1001) usuario   (1001)     2113 2023-05-25 17:57:26.622624 misuma-0.5/PKG-INFO
--rw-r--r--   0 usuario   (1001) usuario   (1001)     1675 2023-05-25 17:55:39.000000 misuma-0.5/README.md
-drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-25 17:57:26.622624 misuma-0.5/misuma/
--rw-r--r--   0 usuario   (1001) usuario   (1001)      222 2023-05-18 18:48:32.000000 misuma-0.5/misuma/__init__.py
-drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-25 17:57:26.622624 misuma-0.5/misuma.egg-info/
--rw-rw-r--   0 usuario   (1001) usuario   (1001)     2113 2023-05-25 17:57:26.000000 misuma-0.5/misuma.egg-info/PKG-INFO
--rw-rw-r--   0 usuario   (1001) usuario   (1001)      244 2023-05-25 17:57:26.000000 misuma-0.5/misuma.egg-info/SOURCES.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)        1 2023-05-25 17:57:26.000000 misuma-0.5/misuma.egg-info/dependency_links.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)       50 2023-05-25 17:57:26.000000 misuma-0.5/misuma.egg-info/entry_points.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)       30 2023-05-25 17:57:26.000000 misuma-0.5/misuma.egg-info/requires.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)        7 2023-05-25 17:57:26.000000 misuma-0.5/misuma.egg-info/top_level.txt
--rw-r--r--   0 usuario   (1001) usuario   (1001)      131 2023-05-16 14:58:32.000000 misuma-0.5/pyproject.toml
--rw-rw-r--   0 usuario   (1001) usuario   (1001)       38 2023-05-25 17:57:26.622624 misuma-0.5/setup.cfg
--rw-r--r--   0 usuario   (1001) usuario   (1001)     2177 2023-05-25 17:57:14.000000 misuma-0.5/setup.py
+drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-25 18:23:43.774645 misuma-0.6/
+-rw-r--r--   0 usuario   (1001) usuario   (1001)     1134 2023-05-16 14:58:24.000000 misuma-0.6/LICENSE
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)     1918 2023-05-25 18:23:43.774645 misuma-0.6/PKG-INFO
+-rw-r--r--   0 usuario   (1001) usuario   (1001)     1480 2023-05-25 18:22:01.000000 misuma-0.6/README.md
+drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-25 18:23:43.774645 misuma-0.6/misuma/
+-rw-r--r--   0 usuario   (1001) usuario   (1001)      222 2023-05-18 18:48:32.000000 misuma-0.6/misuma/__init__.py
+drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-25 18:23:43.774645 misuma-0.6/misuma.egg-info/
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)     1918 2023-05-25 18:23:43.000000 misuma-0.6/misuma.egg-info/PKG-INFO
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)      244 2023-05-25 18:23:43.000000 misuma-0.6/misuma.egg-info/SOURCES.txt
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)        1 2023-05-25 18:23:43.000000 misuma-0.6/misuma.egg-info/dependency_links.txt
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)       50 2023-05-25 18:23:43.000000 misuma-0.6/misuma.egg-info/entry_points.txt
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)       30 2023-05-25 18:23:43.000000 misuma-0.6/misuma.egg-info/requires.txt
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)        7 2023-05-25 18:23:43.000000 misuma-0.6/misuma.egg-info/top_level.txt
+-rw-r--r--   0 usuario   (1001) usuario   (1001)      131 2023-05-16 14:58:32.000000 misuma-0.6/pyproject.toml
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)       38 2023-05-25 18:23:43.774645 misuma-0.6/setup.cfg
+-rw-r--r--   0 usuario   (1001) usuario   (1001)     2177 2023-05-25 18:23:29.000000 misuma-0.6/setup.py
```

### Comparing `misuma-0.5/LICENSE` & `misuma-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `misuma-0.5/PKG-INFO` & `misuma-0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,81 @@
 Metadata-Version: 2.1
 Name: misuma
-Version: 0.5
+Version: 0.6
 Summary: Sum two numbers
 Home-page: https://pypi.org/project/misuma
 Author: Bang1329
 Author-email: santiago.hg2292@gmail.com
 License: MIT
 Keywords: Sum Addition
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PyMiau
-## Use a short explanatory subtitle like, Make a Miau and a Guau
+# Misuma
+## Make a sum between two values
 
 <!-- This are visual tags that you may add to your package at the beginning with useful information on your package --> 
-[![version](https://img.shields.io/pypi/v/pymiau?color=blue)](https://pypi.org/project/pymiau/)
-[![downloads](https://img.shields.io/pypi/dw/pymiau)](https://pypi.org/project/pymiau/)
+[![version](https://img.shields.io/pypi/v/pymiau?color=blue)](https://pypi.org/project/misuma/)
+[![downloads](https://img.shields.io/pypi/dw/pymiau)](https://pypi.org/project/misuma/)
 
-Always start the README explaining clearly what your package do.  If
-you can include here some beautiful image to call the attention of the
-potential user do it!
+With this package you can make the sum of two values, no matter if it is intergers
+or decimals
 
 This is an example:
 
 <p align="center"><img src="https://drive.google.com/uc?export=view&id=12WY5E_ImInwi-w0R0LFVG5AIJ5yp3_uL" alt="milogo"></p>
 ## Download and install
 
 Describe here how the package can be downloaded and install it in
 different arquitectures.
 
 If you are using `PyPI` installation it's as simple as:
 
 ```
-pip install pymiau
+pip install misuma
 ```
 
 You can also test the unstable version of the package with:
 
 ```
-pip install -i https://test.pypi.org/simple/ pymiau
+pip install -i https://test.pypi.org/simple/ misuma
 ```
 
 ## Quick start
 
 In this section you should provide the most simple instructions to use
 your package.
 
 For instance:
 
 ```
-import pymiau
-print(pymiau.miau())
+import misuma
+print(misuma.miau())
 ```
 
 ## Code examples
 
 Provide some detailed examples for more advanced users.
 
 For instance:
 
 ```
-import pymiau
-print(pymiau.miau(n=2))
+import misuma
+print(misuma.miau(n=2))
 ```
 
 ## What's new
 
 If your package will be frequently updated with new features include a
 section describing the new features added to it:
 
-Version 0.2:
-
-- Function `guau` was implemented.
-- New parameters added to the `miau` routine.
-
 Version 0.1:
 
 - First version of the package.
 
 ------------
 
 This package has been designed and written by Fulanit@ de Tal (C) 2023
```

### Comparing `misuma-0.5/README.md` & `misuma-0.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,65 @@
-# PyMiau
-## Use a short explanatory subtitle like, Make a Miau and a Guau
+# Misuma
+## Make a sum between two values
 
 <!-- This are visual tags that you may add to your package at the beginning with useful information on your package --> 
-[![version](https://img.shields.io/pypi/v/pymiau?color=blue)](https://pypi.org/project/pymiau/)
-[![downloads](https://img.shields.io/pypi/dw/pymiau)](https://pypi.org/project/pymiau/)
+[![version](https://img.shields.io/pypi/v/pymiau?color=blue)](https://pypi.org/project/misuma/)
+[![downloads](https://img.shields.io/pypi/dw/pymiau)](https://pypi.org/project/misuma/)
 
-Always start the README explaining clearly what your package do.  If
-you can include here some beautiful image to call the attention of the
-potential user do it!
+With this package you can make the sum of two values, no matter if it is intergers
+or decimals
 
 This is an example:
 
 <p align="center"><img src="https://drive.google.com/uc?export=view&id=12WY5E_ImInwi-w0R0LFVG5AIJ5yp3_uL" alt="milogo"></p>
 ## Download and install
 
 Describe here how the package can be downloaded and install it in
 different arquitectures.
 
 If you are using `PyPI` installation it's as simple as:
 
 ```
-pip install pymiau
+pip install misuma
 ```
 
 You can also test the unstable version of the package with:
 
 ```
-pip install -i https://test.pypi.org/simple/ pymiau
+pip install -i https://test.pypi.org/simple/ misuma
 ```
 
 ## Quick start
 
 In this section you should provide the most simple instructions to use
 your package.
 
 For instance:
 
 ```
-import pymiau
-print(pymiau.miau())
+import misuma
+print(misuma.miau())
 ```
 
 ## Code examples
 
 Provide some detailed examples for more advanced users.
 
 For instance:
 
 ```
-import pymiau
-print(pymiau.miau(n=2))
+import misuma
+print(misuma.miau(n=2))
 ```
 
 ## What's new
 
 If your package will be frequently updated with new features include a
 section describing the new features added to it:
 
-Version 0.2:
-
-- Function `guau` was implemented.
-- New parameters added to the `miau` routine.
-
 Version 0.1:
 
 - First version of the package.
 
 ------------
 
 This package has been designed and written by Fulanit@ de Tal (C) 2023
```

### Comparing `misuma-0.5/misuma.egg-info/PKG-INFO` & `misuma-0.6/misuma.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,81 @@
 Metadata-Version: 2.1
 Name: misuma
-Version: 0.5
+Version: 0.6
 Summary: Sum two numbers
 Home-page: https://pypi.org/project/misuma
 Author: Bang1329
 Author-email: santiago.hg2292@gmail.com
 License: MIT
 Keywords: Sum Addition
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PyMiau
-## Use a short explanatory subtitle like, Make a Miau and a Guau
+# Misuma
+## Make a sum between two values
 
 <!-- This are visual tags that you may add to your package at the beginning with useful information on your package --> 
-[![version](https://img.shields.io/pypi/v/pymiau?color=blue)](https://pypi.org/project/pymiau/)
-[![downloads](https://img.shields.io/pypi/dw/pymiau)](https://pypi.org/project/pymiau/)
+[![version](https://img.shields.io/pypi/v/pymiau?color=blue)](https://pypi.org/project/misuma/)
+[![downloads](https://img.shields.io/pypi/dw/pymiau)](https://pypi.org/project/misuma/)
 
-Always start the README explaining clearly what your package do.  If
-you can include here some beautiful image to call the attention of the
-potential user do it!
+With this package you can make the sum of two values, no matter if it is intergers
+or decimals
 
 This is an example:
 
 <p align="center"><img src="https://drive.google.com/uc?export=view&id=12WY5E_ImInwi-w0R0LFVG5AIJ5yp3_uL" alt="milogo"></p>
 ## Download and install
 
 Describe here how the package can be downloaded and install it in
 different arquitectures.
 
 If you are using `PyPI` installation it's as simple as:
 
 ```
-pip install pymiau
+pip install misuma
 ```
 
 You can also test the unstable version of the package with:
 
 ```
-pip install -i https://test.pypi.org/simple/ pymiau
+pip install -i https://test.pypi.org/simple/ misuma
 ```
 
 ## Quick start
 
 In this section you should provide the most simple instructions to use
 your package.
 
 For instance:
 
 ```
-import pymiau
-print(pymiau.miau())
+import misuma
+print(misuma.miau())
 ```
 
 ## Code examples
 
 Provide some detailed examples for more advanced users.
 
 For instance:
 
 ```
-import pymiau
-print(pymiau.miau(n=2))
+import misuma
+print(misuma.miau(n=2))
 ```
 
 ## What's new
 
 If your package will be frequently updated with new features include a
 section describing the new features added to it:
 
-Version 0.2:
-
-- Function `guau` was implemented.
-- New parameters added to the `miau` routine.
-
 Version 0.1:
 
 - First version of the package.
 
 ------------
 
 This package has been designed and written by Fulanit@ de Tal (C) 2023
```

### Comparing `misuma-0.5/setup.py` & `misuma-0.6/setup.py`

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
-    version='0.5',
+    version='0.6',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={'': '.'},
     packages=setuptools.find_packages(where='.'),
```

