# Comparing `tmp/p10k-edit-0.0.7.tar.gz` & `tmp/p10k-edit-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p10k-edit-0.0.7.tar", last modified: Thu May 25 10:08:43 2023, max compression
+gzip compressed data, was "p10k-edit-0.0.8.tar", last modified: Thu May 25 17:14:05 2023, max compression
```

## Comparing `p10k-edit-0.0.7.tar` & `p10k-edit-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 10:08:43.725413 p10k-edit-0.0.7/
--rw-r--r--   0 katayama   (501) staff       (20)     1071 2023-05-25 02:35:29.000000 p10k-edit-0.0.7/LICENSE
--rw-r--r--   0 katayama   (501) staff       (20)     1770 2023-05-25 10:08:43.725123 p10k-edit-0.0.7/PKG-INFO
--rw-r--r--   0 katayama   (501) staff       (20)       11 2023-05-25 02:35:29.000000 p10k-edit-0.0.7/README.md
-drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 10:08:43.722421 p10k-edit-0.0.7/p10k_edit/
--rw-r--r--   0 katayama   (501) staff       (20)       18 2023-05-25 10:08:31.000000 p10k-edit-0.0.7/p10k_edit/__init__.py
-drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 10:08:43.724647 p10k-edit-0.0.7/p10k_edit/bin/
--rw-r--r--   0 katayama   (501) staff       (20)        0 2023-05-25 03:02:09.000000 p10k-edit-0.0.7/p10k_edit/bin/__init__.py
--rwxr-xr-x   0 katayama   (501) staff       (20)    26614 2023-05-25 10:07:13.000000 p10k-edit-0.0.7/p10k_edit/bin/__main__.py
-drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 10:08:43.724069 p10k-edit-0.0.7/p10k_edit.egg-info/
--rw-r--r--   0 katayama   (501) staff       (20)     1770 2023-05-25 10:08:43.000000 p10k-edit-0.0.7/p10k_edit.egg-info/PKG-INFO
--rw-r--r--   0 katayama   (501) staff       (20)      268 2023-05-25 10:08:43.000000 p10k-edit-0.0.7/p10k_edit.egg-info/SOURCES.txt
--rw-r--r--   0 katayama   (501) staff       (20)        1 2023-05-25 10:08:43.000000 p10k-edit-0.0.7/p10k_edit.egg-info/dependency_links.txt
--rw-r--r--   0 katayama   (501) staff       (20)       58 2023-05-25 10:08:43.000000 p10k-edit-0.0.7/p10k_edit.egg-info/entry_points.txt
--rw-r--r--   0 katayama   (501) staff       (20)       10 2023-05-25 10:08:43.000000 p10k-edit-0.0.7/p10k_edit.egg-info/top_level.txt
--rw-r--r--   0 katayama   (501) staff       (20)       38 2023-05-25 10:08:43.725517 p10k-edit-0.0.7/setup.cfg
--rw-r--r--   0 katayama   (501) staff       (20)     1017 2023-05-25 10:08:31.000000 p10k-edit-0.0.7/setup.py
+drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 17:14:05.303433 p10k-edit-0.0.8/
+-rw-r--r--   0 katayama   (501) staff       (20)     1071 2023-05-25 02:35:29.000000 p10k-edit-0.0.8/LICENSE
+-rw-r--r--   0 katayama   (501) staff       (20)     1770 2023-05-25 17:14:05.303147 p10k-edit-0.0.8/PKG-INFO
+-rw-r--r--   0 katayama   (501) staff       (20)       11 2023-05-25 02:35:29.000000 p10k-edit-0.0.8/README.md
+drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 17:14:05.299671 p10k-edit-0.0.8/p10k_edit/
+-rw-r--r--   0 katayama   (501) staff       (20)       18 2023-05-25 17:13:52.000000 p10k-edit-0.0.8/p10k_edit/__init__.py
+drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 17:14:05.302663 p10k-edit-0.0.8/p10k_edit/bin/
+-rw-r--r--   0 katayama   (501) staff       (20)        0 2023-05-25 03:02:09.000000 p10k-edit-0.0.8/p10k_edit/bin/__init__.py
+-rwxr-xr-x   0 katayama   (501) staff       (20)    26614 2023-05-25 10:07:13.000000 p10k-edit-0.0.8/p10k_edit/bin/__main__.py
+drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 17:14:05.302059 p10k-edit-0.0.8/p10k_edit.egg-info/
+-rw-r--r--   0 katayama   (501) staff       (20)     1770 2023-05-25 17:14:05.000000 p10k-edit-0.0.8/p10k_edit.egg-info/PKG-INFO
+-rw-r--r--   0 katayama   (501) staff       (20)      300 2023-05-25 17:14:05.000000 p10k-edit-0.0.8/p10k_edit.egg-info/SOURCES.txt
+-rw-r--r--   0 katayama   (501) staff       (20)        1 2023-05-25 17:14:05.000000 p10k-edit-0.0.8/p10k_edit.egg-info/dependency_links.txt
+-rw-r--r--   0 katayama   (501) staff       (20)       58 2023-05-25 17:14:05.000000 p10k-edit-0.0.8/p10k_edit.egg-info/entry_points.txt
+-rw-r--r--   0 katayama   (501) staff       (20)       26 2023-05-25 17:14:05.000000 p10k-edit-0.0.8/p10k_edit.egg-info/requires.txt
+-rw-r--r--   0 katayama   (501) staff       (20)       10 2023-05-25 17:14:05.000000 p10k-edit-0.0.8/p10k_edit.egg-info/top_level.txt
+-rw-r--r--   0 katayama   (501) staff       (20)       38 2023-05-25 17:14:05.303528 p10k-edit-0.0.8/setup.cfg
+-rw-r--r--   0 katayama   (501) staff       (20)     1096 2023-05-25 17:13:52.000000 p10k-edit-0.0.8/setup.py
```

### Comparing `p10k-edit-0.0.7/LICENSE` & `p10k-edit-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `p10k-edit-0.0.7/PKG-INFO` & `p10k-edit-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p10k-edit
-Version: 0.0.7
+Version: 0.0.8
 Summary: Tool to Edit PowerLevel10k p10k.zsh Config File (work-in-progress)
 Home-page: https://github.com/kkatayama/p10k-edit
 Author: Teddy Katayama
 Author-email: katayama@udel.edu
 License: MIT License
         
         Copyright (c) 2023 Teddy Katayama
```

### Comparing `p10k-edit-0.0.7/p10k_edit/bin/__main__.py` & `p10k-edit-0.0.8/p10k_edit/bin/__main__.py`

 * *Files identical despite different names*

### Comparing `p10k-edit-0.0.7/p10k_edit.egg-info/PKG-INFO` & `p10k-edit-0.0.8/p10k_edit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p10k-edit
-Version: 0.0.7
+Version: 0.0.8
 Summary: Tool to Edit PowerLevel10k p10k.zsh Config File (work-in-progress)
 Home-page: https://github.com/kkatayama/p10k-edit
 Author: Teddy Katayama
 Author-email: katayama@udel.edu
 License: MIT License
         
         Copyright (c) 2023 Teddy Katayama
```

### Comparing `p10k-edit-0.0.7/setup.py` & `p10k-edit-0.0.8/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 #!/usr/bin/env python3
 
 import pathlib
 
 import setuptools
 
 CWD = pathlib.Path(__file__).parent
-
 README = (CWD / "README.md").read_text()
-
 LICENSE = (CWD / "LICENSE").read_text()
+REQUIRED = (CWD / "requirements.txt").read_text()
 
 with open('README.md') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='p10k-edit',
-    version='0.0.7',
+    version='0.0.8',
     author='Teddy Katayama',
     author_email='katayama@udel.edu',
     description='Tool to Edit PowerLevel10k p10k.zsh Config File (work-in-progress)',
     license = LICENSE,
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kkatayama/p10k-edit',
@@ -32,8 +31,9 @@
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
+    install_requires=REQUIRED,
 )
```

