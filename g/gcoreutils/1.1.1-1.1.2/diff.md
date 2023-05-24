# Comparing `tmp/gcoreutils-1.1.1.tar.gz` & `tmp/gcoreutils-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcoreutils-1.1.1.tar", last modified: Wed May 17 12:48:21 2023, max compression
+gzip compressed data, was "gcoreutils-1.1.2.tar", last modified: Wed May 24 22:06:11 2023, max compression
```

## Comparing `gcoreutils-1.1.1.tar` & `gcoreutils-1.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-17 12:48:21.429212 gcoreutils-1.1.1/
--rw-r--r--   0 hiro       (501) staff       (20)     1078 2023-05-15 02:20:50.000000 gcoreutils-1.1.1/LICENSE
--rw-------   0 hiro       (501) staff       (20)       50 2023-05-15 22:17:22.000000 gcoreutils-1.1.1/MANIFEST.in
--rw-r--r--   0 hiro       (501) staff       (20)      836 2023-05-17 12:48:21.429283 gcoreutils-1.1.1/PKG-INFO
--rw-------   0 hiro       (501) staff       (20)      463 2023-05-15 21:57:59.000000 gcoreutils-1.1.1/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-17 12:48:21.428330 gcoreutils-1.1.1/gcoreutils/
--rw-r--r--   0 hiro       (501) staff       (20)       54 2023-05-17 12:43:42.000000 gcoreutils-1.1.1/gcoreutils/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1343 2023-05-15 02:20:50.000000 gcoreutils-1.1.1/gcoreutils/basic_util.py
--rw-r--r--   0 hiro       (501) staff       (20)     2768 2023-05-15 12:04:16.000000 gcoreutils-1.1.1/gcoreutils/binary_manager.py
--rw-r--r--   0 hiro       (501) staff       (20)     6482 2023-05-15 12:04:16.000000 gcoreutils-1.1.1/gcoreutils/convert_util.py
--rw-r--r--   0 hiro       (501) staff       (20)     2946 2023-05-15 12:04:16.000000 gcoreutils-1.1.1/gcoreutils/crystal_util.py
--rw-r--r--   0 hiro       (501) staff       (20)     8035 2023-05-15 02:20:50.000000 gcoreutils-1.1.1/gcoreutils/dataset.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-17 12:48:21.429087 gcoreutils-1.1.1/gcoreutils/detail/
--rw-r--r--   0 hiro       (501) staff       (20)     8828 2023-05-15 12:04:16.000000 gcoreutils-1.1.1/gcoreutils/detail/nsarray_util.py
--rw-r--r--   0 hiro       (501) staff       (20)     1417 2023-05-15 02:20:50.000000 gcoreutils-1.1.1/gcoreutils/eigensystem.py
--rw-r--r--   0 hiro       (501) staff       (20)     2077 2023-05-15 02:20:50.000000 gcoreutils-1.1.1/gcoreutils/io_util.py
--rw-r--r--   0 hiro       (501) staff       (20)     2682 2023-05-15 02:20:50.000000 gcoreutils-1.1.1/gcoreutils/latex_util.py
--rw-r--r--   0 hiro       (501) staff       (20)     1742 2023-05-15 02:20:50.000000 gcoreutils-1.1.1/gcoreutils/list_util.py
--rw-r--r--   0 hiro       (501) staff       (20)    46345 2023-05-15 12:04:16.000000 gcoreutils-1.1.1/gcoreutils/nsarray.py
--rw-r--r--   0 hiro       (501) staff       (20)    16477 2023-05-15 02:20:50.000000 gcoreutils-1.1.1/gcoreutils/pdf_via_latex.py
--rw-r--r--   0 hiro       (501) staff       (20)     4580 2023-05-15 02:20:50.000000 gcoreutils-1.1.1/gcoreutils/plot_util.py
--rw-r--r--   0 hiro       (501) staff       (20)     2868 2023-05-15 02:20:50.000000 gcoreutils-1.1.1/gcoreutils/string_util.py
--rw-r--r--   0 hiro       (501) staff       (20)     4941 2023-05-15 02:20:50.000000 gcoreutils-1.1.1/gcoreutils/symdict.py
--rw-r--r--   0 hiro       (501) staff       (20)     4370 2023-05-15 02:20:50.000000 gcoreutils-1.1.1/gcoreutils/symlist.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-17 12:48:21.428950 gcoreutils-1.1.1/gcoreutils.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)      836 2023-05-17 12:48:21.000000 gcoreutils-1.1.1/gcoreutils.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)      645 2023-05-17 12:48:21.000000 gcoreutils-1.1.1/gcoreutils.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-05-17 12:48:21.000000 gcoreutils-1.1.1/gcoreutils.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)       64 2023-05-17 12:48:21.000000 gcoreutils-1.1.1/gcoreutils.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)       11 2023-05-17 12:48:21.000000 gcoreutils-1.1.1/gcoreutils.egg-info/top_level.txt
--rw-------   0 hiro       (501) staff       (20)      606 2023-05-17 12:48:21.429623 gcoreutils-1.1.1/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-15 02:20:50.000000 gcoreutils-1.1.1/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-24 22:06:11.990382 gcoreutils-1.1.2/
+-rw-r--r--   0 hiro       (501) staff       (20)     1078 2023-05-15 02:20:50.000000 gcoreutils-1.1.2/LICENSE
+-rw-------   0 hiro       (501) staff       (20)       50 2023-05-15 22:17:22.000000 gcoreutils-1.1.2/MANIFEST.in
+-rw-r--r--   0 hiro       (501) staff       (20)      836 2023-05-24 22:06:11.990469 gcoreutils-1.1.2/PKG-INFO
+-rw-------   0 hiro       (501) staff       (20)      463 2023-05-15 21:57:59.000000 gcoreutils-1.1.2/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-24 22:06:11.988709 gcoreutils-1.1.2/gcoreutils/
+-rw-r--r--   0 hiro       (501) staff       (20)       54 2023-05-24 22:05:53.000000 gcoreutils-1.1.2/gcoreutils/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1343 2023-05-15 02:20:50.000000 gcoreutils-1.1.2/gcoreutils/basic_util.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2768 2023-05-15 12:04:16.000000 gcoreutils-1.1.2/gcoreutils/binary_manager.py
+-rw-r--r--   0 hiro       (501) staff       (20)     6482 2023-05-15 12:04:16.000000 gcoreutils-1.1.2/gcoreutils/convert_util.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2946 2023-05-15 12:04:16.000000 gcoreutils-1.1.2/gcoreutils/crystal_util.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8035 2023-05-15 02:20:50.000000 gcoreutils-1.1.2/gcoreutils/dataset.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-24 22:06:11.990137 gcoreutils-1.1.2/gcoreutils/detail/
+-rw-r--r--   0 hiro       (501) staff       (20)     8828 2023-05-15 12:04:16.000000 gcoreutils-1.1.2/gcoreutils/detail/nsarray_util.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1417 2023-05-15 02:20:50.000000 gcoreutils-1.1.2/gcoreutils/eigensystem.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2077 2023-05-15 02:20:50.000000 gcoreutils-1.1.2/gcoreutils/io_util.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2682 2023-05-15 02:20:50.000000 gcoreutils-1.1.2/gcoreutils/latex_util.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1742 2023-05-15 02:20:50.000000 gcoreutils-1.1.2/gcoreutils/list_util.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46345 2023-05-15 12:04:16.000000 gcoreutils-1.1.2/gcoreutils/nsarray.py
+-rw-r--r--   0 hiro       (501) staff       (20)    16477 2023-05-15 02:20:50.000000 gcoreutils-1.1.2/gcoreutils/pdf_via_latex.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4580 2023-05-15 02:20:50.000000 gcoreutils-1.1.2/gcoreutils/plot_util.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2868 2023-05-15 02:20:50.000000 gcoreutils-1.1.2/gcoreutils/string_util.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4941 2023-05-15 02:20:50.000000 gcoreutils-1.1.2/gcoreutils/symdict.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4370 2023-05-15 02:20:50.000000 gcoreutils-1.1.2/gcoreutils/symlist.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-24 22:06:11.989965 gcoreutils-1.1.2/gcoreutils.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)      836 2023-05-24 22:06:11.000000 gcoreutils-1.1.2/gcoreutils.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)      645 2023-05-24 22:06:11.000000 gcoreutils-1.1.2/gcoreutils.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-05-24 22:06:11.000000 gcoreutils-1.1.2/gcoreutils.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       71 2023-05-24 22:06:11.000000 gcoreutils-1.1.2/gcoreutils.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       11 2023-05-24 22:06:11.000000 gcoreutils-1.1.2/gcoreutils.egg-info/top_level.txt
+-rw-------   0 hiro       (501) staff       (20)      613 2023-05-24 22:06:11.990875 gcoreutils-1.1.2/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-15 02:20:50.000000 gcoreutils-1.1.2/setup.py
```

### Comparing `gcoreutils-1.1.1/LICENSE` & `gcoreutils-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gcoreutils-1.1.1/PKG-INFO` & `gcoreutils-1.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcoreutils
-Version: 1.1.1
+Version: 1.1.2
 Summary: A versatile python utility library.
 Home-page: https://github.com/CMT-MU/GCoreUtils
 Author: Hiroaki Kusunose
 Author-email: hiroaki.kusunose@gmail.com
 License: MIT
 Keywords: numpy,scipy,sympy,pandas,LaTeX
 Requires-Python: >=3.8
```

### Comparing `gcoreutils-1.1.1/gcoreutils/basic_util.py` & `gcoreutils-1.1.2/gcoreutils/basic_util.py`

 * *Files identical despite different names*

### Comparing `gcoreutils-1.1.1/gcoreutils/binary_manager.py` & `gcoreutils-1.1.2/gcoreutils/binary_manager.py`

 * *Files identical despite different names*

### Comparing `gcoreutils-1.1.1/gcoreutils/convert_util.py` & `gcoreutils-1.1.2/gcoreutils/convert_util.py`

 * *Files identical despite different names*

### Comparing `gcoreutils-1.1.1/gcoreutils/crystal_util.py` & `gcoreutils-1.1.2/gcoreutils/crystal_util.py`

 * *Files identical despite different names*

### Comparing `gcoreutils-1.1.1/gcoreutils/dataset.py` & `gcoreutils-1.1.2/gcoreutils/dataset.py`

 * *Files identical despite different names*

### Comparing `gcoreutils-1.1.1/gcoreutils/detail/nsarray_util.py` & `gcoreutils-1.1.2/gcoreutils/detail/nsarray_util.py`

 * *Files identical despite different names*

### Comparing `gcoreutils-1.1.1/gcoreutils/eigensystem.py` & `gcoreutils-1.1.2/gcoreutils/eigensystem.py`

 * *Files identical despite different names*

### Comparing `gcoreutils-1.1.1/gcoreutils/io_util.py` & `gcoreutils-1.1.2/gcoreutils/io_util.py`

 * *Files identical despite different names*

### Comparing `gcoreutils-1.1.1/gcoreutils/latex_util.py` & `gcoreutils-1.1.2/gcoreutils/latex_util.py`

 * *Files identical despite different names*

### Comparing `gcoreutils-1.1.1/gcoreutils/list_util.py` & `gcoreutils-1.1.2/gcoreutils/list_util.py`

 * *Files identical despite different names*

### Comparing `gcoreutils-1.1.1/gcoreutils/nsarray.py` & `gcoreutils-1.1.2/gcoreutils/nsarray.py`

 * *Files identical despite different names*

### Comparing `gcoreutils-1.1.1/gcoreutils/pdf_via_latex.py` & `gcoreutils-1.1.2/gcoreutils/pdf_via_latex.py`

 * *Files identical despite different names*

### Comparing `gcoreutils-1.1.1/gcoreutils/plot_util.py` & `gcoreutils-1.1.2/gcoreutils/plot_util.py`

 * *Files identical despite different names*

### Comparing `gcoreutils-1.1.1/gcoreutils/string_util.py` & `gcoreutils-1.1.2/gcoreutils/string_util.py`

 * *Files identical despite different names*

### Comparing `gcoreutils-1.1.1/gcoreutils/symdict.py` & `gcoreutils-1.1.2/gcoreutils/symdict.py`

 * *Files identical despite different names*

### Comparing `gcoreutils-1.1.1/gcoreutils/symlist.py` & `gcoreutils-1.1.2/gcoreutils/symlist.py`

 * *Files identical despite different names*

### Comparing `gcoreutils-1.1.1/gcoreutils.egg-info/PKG-INFO` & `gcoreutils-1.1.2/gcoreutils.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcoreutils
-Version: 1.1.1
+Version: 1.1.2
 Summary: A versatile python utility library.
 Home-page: https://github.com/CMT-MU/GCoreUtils
 Author: Hiroaki Kusunose
 Author-email: hiroaki.kusunose@gmail.com
 License: MIT
 Keywords: numpy,scipy,sympy,pandas,LaTeX
 Requires-Python: >=3.8
```

### Comparing `gcoreutils-1.1.1/gcoreutils.egg-info/SOURCES.txt` & `gcoreutils-1.1.2/gcoreutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcoreutils-1.1.1/setup.cfg` & `gcoreutils-1.1.2/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 [options]
 python_requires = >=3.8
 install_requires = 
 	numpy
 	scipy
 	sympy
-	pandas
+	pandas==1.4.1
 packages = find:
 include_package_data = True
 
 [options.extras_require]
 dev = 
 	sphinx
 	sphinx-rtd-theme
```

