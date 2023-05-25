# Comparing `tmp/p10k-edit-0.0.5.tar.gz` & `tmp/p10k-edit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p10k-edit-0.0.5.tar", last modified: Thu May 25 09:49:19 2023, max compression
+gzip compressed data, was "p10k-edit-0.0.6.tar", last modified: Thu May 25 09:54:11 2023, max compression
```

## Comparing `p10k-edit-0.0.5.tar` & `p10k-edit-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 09:49:19.977602 p10k-edit-0.0.5/
--rw-r--r--   0 katayama   (501) staff       (20)     1071 2023-05-25 02:35:29.000000 p10k-edit-0.0.5/LICENSE
--rw-r--r--   0 katayama   (501) staff       (20)     1770 2023-05-25 09:49:19.977292 p10k-edit-0.0.5/PKG-INFO
--rw-r--r--   0 katayama   (501) staff       (20)       11 2023-05-25 02:35:29.000000 p10k-edit-0.0.5/README.md
-drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 09:49:19.972418 p10k-edit-0.0.5/p10k_edit/
--rw-r--r--   0 katayama   (501) staff       (20)       18 2023-05-25 09:48:06.000000 p10k-edit-0.0.5/p10k_edit/__init__.py
-drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 09:49:19.976029 p10k-edit-0.0.5/p10k_edit/bin/
--rw-r--r--   0 katayama   (501) staff       (20)        0 2023-05-25 03:02:09.000000 p10k-edit-0.0.5/p10k_edit/bin/__init__.py
--rwxr-xr-x   0 katayama   (501) staff       (20)    26453 2023-05-25 09:47:48.000000 p10k-edit-0.0.5/p10k_edit/bin/__main__.py
-drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 09:49:19.975084 p10k-edit-0.0.5/p10k_edit.egg-info/
--rw-r--r--   0 katayama   (501) staff       (20)     1770 2023-05-25 09:49:19.000000 p10k-edit-0.0.5/p10k_edit.egg-info/PKG-INFO
--rw-r--r--   0 katayama   (501) staff       (20)      268 2023-05-25 09:49:19.000000 p10k-edit-0.0.5/p10k_edit.egg-info/SOURCES.txt
--rw-r--r--   0 katayama   (501) staff       (20)        1 2023-05-25 09:49:19.000000 p10k-edit-0.0.5/p10k_edit.egg-info/dependency_links.txt
--rw-r--r--   0 katayama   (501) staff       (20)       58 2023-05-25 09:49:19.000000 p10k-edit-0.0.5/p10k_edit.egg-info/entry_points.txt
--rw-r--r--   0 katayama   (501) staff       (20)       10 2023-05-25 09:49:19.000000 p10k-edit-0.0.5/p10k_edit.egg-info/top_level.txt
--rw-r--r--   0 katayama   (501) staff       (20)       38 2023-05-25 09:49:19.977692 p10k-edit-0.0.5/setup.cfg
--rw-r--r--   0 katayama   (501) staff       (20)     1017 2023-05-25 09:48:06.000000 p10k-edit-0.0.5/setup.py
+drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 09:54:11.855681 p10k-edit-0.0.6/
+-rw-r--r--   0 katayama   (501) staff       (20)     1071 2023-05-25 02:35:29.000000 p10k-edit-0.0.6/LICENSE
+-rw-r--r--   0 katayama   (501) staff       (20)     1770 2023-05-25 09:54:11.855310 p10k-edit-0.0.6/PKG-INFO
+-rw-r--r--   0 katayama   (501) staff       (20)       11 2023-05-25 02:35:29.000000 p10k-edit-0.0.6/README.md
+drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 09:54:11.850480 p10k-edit-0.0.6/p10k_edit/
+-rw-r--r--   0 katayama   (501) staff       (20)       18 2023-05-25 09:53:53.000000 p10k-edit-0.0.6/p10k_edit/__init__.py
+drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 09:54:11.854185 p10k-edit-0.0.6/p10k_edit/bin/
+-rw-r--r--   0 katayama   (501) staff       (20)        0 2023-05-25 03:02:09.000000 p10k-edit-0.0.6/p10k_edit/bin/__init__.py
+-rwxr-xr-x   0 katayama   (501) staff       (20)    26453 2023-05-25 09:47:48.000000 p10k-edit-0.0.6/p10k_edit/bin/__main__.py
+drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 09:54:11.853186 p10k-edit-0.0.6/p10k_edit.egg-info/
+-rw-r--r--   0 katayama   (501) staff       (20)     1770 2023-05-25 09:54:11.000000 p10k-edit-0.0.6/p10k_edit.egg-info/PKG-INFO
+-rw-r--r--   0 katayama   (501) staff       (20)      268 2023-05-25 09:54:11.000000 p10k-edit-0.0.6/p10k_edit.egg-info/SOURCES.txt
+-rw-r--r--   0 katayama   (501) staff       (20)        1 2023-05-25 09:54:11.000000 p10k-edit-0.0.6/p10k_edit.egg-info/dependency_links.txt
+-rw-r--r--   0 katayama   (501) staff       (20)       62 2023-05-25 09:54:11.000000 p10k-edit-0.0.6/p10k_edit.egg-info/entry_points.txt
+-rw-r--r--   0 katayama   (501) staff       (20)       10 2023-05-25 09:54:11.000000 p10k-edit-0.0.6/p10k_edit.egg-info/top_level.txt
+-rw-r--r--   0 katayama   (501) staff       (20)       38 2023-05-25 09:54:11.855841 p10k-edit-0.0.6/setup.cfg
+-rw-r--r--   0 katayama   (501) staff       (20)     1021 2023-05-25 09:53:53.000000 p10k-edit-0.0.6/setup.py
```

### Comparing `p10k-edit-0.0.5/LICENSE` & `p10k-edit-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `p10k-edit-0.0.5/PKG-INFO` & `p10k-edit-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p10k-edit
-Version: 0.0.5
+Version: 0.0.6
 Summary: Tool to Edit PowerLevel10k p10k.zsh Config File (work-in-progress)
 Home-page: https://github.com/kkatayama/p10k-edit
 Author: Teddy Katayama
 Author-email: katayama@udel.edu
 License: MIT License
         
         Copyright (c) 2023 Teddy Katayama
```

### Comparing `p10k-edit-0.0.5/p10k_edit/bin/__main__.py` & `p10k-edit-0.0.6/p10k_edit/bin/__main__.py`

 * *Files identical despite different names*

### Comparing `p10k-edit-0.0.5/p10k_edit.egg-info/PKG-INFO` & `p10k-edit-0.0.6/p10k_edit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p10k-edit
-Version: 0.0.5
+Version: 0.0.6
 Summary: Tool to Edit PowerLevel10k p10k.zsh Config File (work-in-progress)
 Home-page: https://github.com/kkatayama/p10k-edit
 Author: Teddy Katayama
 Author-email: katayama@udel.edu
 License: MIT License
         
         Copyright (c) 2023 Teddy Katayama
```

### Comparing `p10k-edit-0.0.5/setup.py` & `p10k-edit-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 LICENSE = (CWD / "LICENSE").read_text()
 
 with open('README.md') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='p10k-edit',
-    version='0.0.5',
+    version='0.0.6',
     author='Teddy Katayama',
     author_email='katayama@udel.edu',
     description='Tool to Edit PowerLevel10k p10k.zsh Config File (work-in-progress)',
     license = LICENSE,
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kkatayama/p10k-edit',
     packages=setuptools.find_packages(),
     entry_points={
         'console_scripts': [
-            'p10k-edit=p10k_edit.bin.__main__:main'
+            'p10k-edit=p10k_edit.bin.__main__:__main__'
         ]
     },
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
```

