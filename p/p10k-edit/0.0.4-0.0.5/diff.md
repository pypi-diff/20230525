# Comparing `tmp/p10k-edit-0.0.4.tar.gz` & `tmp/p10k-edit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p10k-edit-0.0.4.tar", last modified: Thu May 25 09:41:13 2023, max compression
+gzip compressed data, was "p10k-edit-0.0.5.tar", last modified: Thu May 25 09:49:19 2023, max compression
```

## Comparing `p10k-edit-0.0.4.tar` & `p10k-edit-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 09:41:13.452715 p10k-edit-0.0.4/
--rw-r--r--   0 katayama   (501) staff       (20)     1071 2023-05-25 02:35:29.000000 p10k-edit-0.0.4/LICENSE
--rw-r--r--   0 katayama   (501) staff       (20)     1770 2023-05-25 09:41:13.452396 p10k-edit-0.0.4/PKG-INFO
--rw-r--r--   0 katayama   (501) staff       (20)       11 2023-05-25 02:35:29.000000 p10k-edit-0.0.4/README.md
-drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 09:41:13.448435 p10k-edit-0.0.4/p10k_edit/
--rw-r--r--   0 katayama   (501) staff       (20)       18 2023-05-25 09:39:14.000000 p10k-edit-0.0.4/p10k_edit/__init__.py
-drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 09:41:13.451197 p10k-edit-0.0.4/p10k_edit/bin/
--rw-r--r--   0 katayama   (501) staff       (20)        0 2023-05-25 03:02:09.000000 p10k-edit-0.0.4/p10k_edit/bin/__init__.py
--rwxr-xr-x   0 katayama   (501) staff       (20)    26454 2023-05-25 06:31:58.000000 p10k-edit-0.0.4/p10k_edit/bin/__main__.py
-drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 09:41:13.450577 p10k-edit-0.0.4/p10k_edit.egg-info/
--rw-r--r--   0 katayama   (501) staff       (20)     1770 2023-05-25 09:41:13.000000 p10k-edit-0.0.4/p10k_edit.egg-info/PKG-INFO
--rw-r--r--   0 katayama   (501) staff       (20)      268 2023-05-25 09:41:13.000000 p10k-edit-0.0.4/p10k_edit.egg-info/SOURCES.txt
--rw-r--r--   0 katayama   (501) staff       (20)        1 2023-05-25 09:41:13.000000 p10k-edit-0.0.4/p10k_edit.egg-info/dependency_links.txt
--rw-r--r--   0 katayama   (501) staff       (20)       58 2023-05-25 09:41:13.000000 p10k-edit-0.0.4/p10k_edit.egg-info/entry_points.txt
--rw-r--r--   0 katayama   (501) staff       (20)       10 2023-05-25 09:41:13.000000 p10k-edit-0.0.4/p10k_edit.egg-info/top_level.txt
--rw-r--r--   0 katayama   (501) staff       (20)       38 2023-05-25 09:41:13.452837 p10k-edit-0.0.4/setup.cfg
--rw-r--r--   0 katayama   (501) staff       (20)     1017 2023-05-25 09:39:14.000000 p10k-edit-0.0.4/setup.py
+drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 09:49:19.977602 p10k-edit-0.0.5/
+-rw-r--r--   0 katayama   (501) staff       (20)     1071 2023-05-25 02:35:29.000000 p10k-edit-0.0.5/LICENSE
+-rw-r--r--   0 katayama   (501) staff       (20)     1770 2023-05-25 09:49:19.977292 p10k-edit-0.0.5/PKG-INFO
+-rw-r--r--   0 katayama   (501) staff       (20)       11 2023-05-25 02:35:29.000000 p10k-edit-0.0.5/README.md
+drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 09:49:19.972418 p10k-edit-0.0.5/p10k_edit/
+-rw-r--r--   0 katayama   (501) staff       (20)       18 2023-05-25 09:48:06.000000 p10k-edit-0.0.5/p10k_edit/__init__.py
+drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 09:49:19.976029 p10k-edit-0.0.5/p10k_edit/bin/
+-rw-r--r--   0 katayama   (501) staff       (20)        0 2023-05-25 03:02:09.000000 p10k-edit-0.0.5/p10k_edit/bin/__init__.py
+-rwxr-xr-x   0 katayama   (501) staff       (20)    26453 2023-05-25 09:47:48.000000 p10k-edit-0.0.5/p10k_edit/bin/__main__.py
+drwxr-xr-x   0 katayama   (501) staff       (20)        0 2023-05-25 09:49:19.975084 p10k-edit-0.0.5/p10k_edit.egg-info/
+-rw-r--r--   0 katayama   (501) staff       (20)     1770 2023-05-25 09:49:19.000000 p10k-edit-0.0.5/p10k_edit.egg-info/PKG-INFO
+-rw-r--r--   0 katayama   (501) staff       (20)      268 2023-05-25 09:49:19.000000 p10k-edit-0.0.5/p10k_edit.egg-info/SOURCES.txt
+-rw-r--r--   0 katayama   (501) staff       (20)        1 2023-05-25 09:49:19.000000 p10k-edit-0.0.5/p10k_edit.egg-info/dependency_links.txt
+-rw-r--r--   0 katayama   (501) staff       (20)       58 2023-05-25 09:49:19.000000 p10k-edit-0.0.5/p10k_edit.egg-info/entry_points.txt
+-rw-r--r--   0 katayama   (501) staff       (20)       10 2023-05-25 09:49:19.000000 p10k-edit-0.0.5/p10k_edit.egg-info/top_level.txt
+-rw-r--r--   0 katayama   (501) staff       (20)       38 2023-05-25 09:49:19.977692 p10k-edit-0.0.5/setup.cfg
+-rw-r--r--   0 katayama   (501) staff       (20)     1017 2023-05-25 09:48:06.000000 p10k-edit-0.0.5/setup.py
```

### Comparing `p10k-edit-0.0.4/LICENSE` & `p10k-edit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `p10k-edit-0.0.4/PKG-INFO` & `p10k-edit-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p10k-edit
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tool to Edit PowerLevel10k p10k.zsh Config File (work-in-progress)
 Home-page: https://github.com/kkatayama/p10k-edit
 Author: Teddy Katayama
 Author-email: katayama@udel.edu
 License: MIT License
         
         Copyright (c) 2023 Teddy Katayama
```

### Comparing `p10k-edit-0.0.4/p10k_edit/bin/__main__.py` & `p10k-edit-0.0.5/p10k_edit/bin/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
 def setup():
     old = get_py_path()
     extractTheme()
     cwd = Path.home().joinpath("Library", "Application Support")
     if shutil.get_terminal_size().columns >= 96:
         os.chdir(cwd)
-    elif shutil.get_terminal_size().columns >= 76::
+    elif shutil.get_terminal_size().columns >= 76:
         cwd = Path.home().joinpath("Library")
         os.chdir(cwd)
     else:
         iterm2.run_until_complete(resizeShell)
     return old, cwd
 
 def cleanup(old):
```

### Comparing `p10k-edit-0.0.4/p10k_edit.egg-info/PKG-INFO` & `p10k-edit-0.0.5/p10k_edit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p10k-edit
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tool to Edit PowerLevel10k p10k.zsh Config File (work-in-progress)
 Home-page: https://github.com/kkatayama/p10k-edit
 Author: Teddy Katayama
 Author-email: katayama@udel.edu
 License: MIT License
         
         Copyright (c) 2023 Teddy Katayama
```

### Comparing `p10k-edit-0.0.4/setup.py` & `p10k-edit-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 LICENSE = (CWD / "LICENSE").read_text()
 
 with open('README.md') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='p10k-edit',
-    version='0.0.4',
+    version='0.0.5',
     author='Teddy Katayama',
     author_email='katayama@udel.edu',
     description='Tool to Edit PowerLevel10k p10k.zsh Config File (work-in-progress)',
     license = LICENSE,
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kkatayama/p10k-edit',
```

