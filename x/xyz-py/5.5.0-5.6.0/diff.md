# Comparing `tmp/xyz_py-5.5.0.tar.gz` & `tmp/xyz_py-5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xyz_py-5.5.0.tar", last modified: Thu Apr 27 16:01:59 2023, max compression
+gzip compressed data, was "xyz_py-5.6.0.tar", last modified: Thu May 25 13:55:41 2023, max compression
```

## Comparing `xyz_py-5.5.0.tar` & `xyz_py-5.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:01:59.982057 xyz_py-5.5.0/
--rw-rw-rw-   0 root         (0) root         (0)    35072 2023-04-27 16:01:31.000000 xyz_py-5.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1303 2023-04-27 16:01:59.980056 xyz_py-5.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-04-27 16:01:31.000000 xyz_py-5.5.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-04-27 16:01:31.000000 xyz_py-5.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 16:01:59.982057 xyz_py-5.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-27 16:01:55.000000 xyz_py-5.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:01:59.974056 xyz_py-5.5.0/xyz_py/
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-27 16:01:31.000000 xyz_py-5.5.0/xyz_py/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7424 2023-04-27 16:01:31.000000 xyz_py-5.5.0/xyz_py/atomic.py
--rw-rw-rw-   0 root         (0) root         (0)    10677 2023-04-27 16:01:31.000000 xyz_py-5.5.0/xyz_py/cli.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-27 16:01:55.000000 xyz_py-5.5.0/xyz_py/version.py
--rw-rw-rw-   0 root         (0) root         (0)    37858 2023-04-27 16:01:31.000000 xyz_py-5.5.0/xyz_py/xyz_py.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:01:59.980056 xyz_py-5.5.0/xyz_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1303 2023-04-27 16:01:59.000000 xyz_py-5.5.0/xyz_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      308 2023-04-27 16:01:59.000000 xyz_py-5.5.0/xyz_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 16:01:59.000000 xyz_py-5.5.0/xyz_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-04-27 16:01:59.000000 xyz_py-5.5.0/xyz_py.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-27 16:01:59.000000 xyz_py-5.5.0/xyz_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-27 16:01:59.000000 xyz_py-5.5.0/xyz_py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 13:55:41.629097 xyz_py-5.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35072 2023-05-25 13:55:23.000000 xyz_py-5.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-05-25 13:55:41.629097 xyz_py-5.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-05-25 13:55:23.000000 xyz_py-5.6.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-05-25 13:55:23.000000 xyz_py-5.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 13:55:41.630097 xyz_py-5.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-05-25 13:55:39.000000 xyz_py-5.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 13:55:41.627097 xyz_py-5.6.0/xyz_py/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-05-25 13:55:23.000000 xyz_py-5.6.0/xyz_py/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7424 2023-05-25 13:55:23.000000 xyz_py-5.6.0/xyz_py/atomic.py
+-rw-rw-rw-   0 root         (0) root         (0)    10677 2023-05-25 13:55:23.000000 xyz_py-5.6.0/xyz_py/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-25 13:55:39.000000 xyz_py-5.6.0/xyz_py/version.py
+-rw-rw-rw-   0 root         (0) root         (0)    38593 2023-05-25 13:55:23.000000 xyz_py-5.6.0/xyz_py/xyz_py.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 13:55:41.629097 xyz_py-5.6.0/xyz_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-05-25 13:55:41.000000 xyz_py-5.6.0/xyz_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      308 2023-05-25 13:55:41.000000 xyz_py-5.6.0/xyz_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 13:55:41.000000 xyz_py-5.6.0/xyz_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-25 13:55:41.000000 xyz_py-5.6.0/xyz_py.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-25 13:55:41.000000 xyz_py-5.6.0/xyz_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-25 13:55:41.000000 xyz_py-5.6.0/xyz_py.egg-info/top_level.txt
```

### Comparing `xyz_py-5.5.0/LICENSE` & `xyz_py-5.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xyz_py-5.5.0/PKG-INFO` & `xyz_py-5.6.0/xyz_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xyz_py
-Version: 5.5.0
+Name: xyz-py
+Version: 5.6.0
 Summary: A package for manipulating xyz files and chemical structures
 Home-page: https://gitlab.com/jonkragskow/xyz_py
 Author: Jon Kragskow
 Author-email: jonkragskow@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/jonkragskow/xyz_py/-/issues
 Project-URL: Documentation, https://jonkragskow.gitlab.io/xyz_py
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xyz_py-5.5.0/README.md` & `xyz_py-5.6.0/README.md`

 * *Files identical despite different names*

### Comparing `xyz_py-5.5.0/setup.py` & `xyz_py-5.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-__version__ = "5.5.0"
+__version__ = "5.6.0"
 
 setuptools.setup(
     name="xyz_py",
     version=__version__,
     author="Jon Kragskow",
     author_email="jonkragskow@gmail.com",
     description="A package for manipulating xyz files and chemical structures",
```

### Comparing `xyz_py-5.5.0/xyz_py/atomic.py` & `xyz_py-5.6.0/xyz_py/atomic.py`

 * *Files identical despite different names*

### Comparing `xyz_py-5.5.0/xyz_py/cli.py` & `xyz_py-5.6.0/xyz_py/cli.py`

 * *Files identical despite different names*

### Comparing `xyz_py-5.5.0/xyz_py/xyz_py.py` & `xyz_py-5.6.0/xyz_py/xyz_py.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,21 @@
 from . import version
 from . import atomic
 
 __version__ = version.__version__
 
 
 def load_xyz(f_name: str, atomic_numbers: bool = False,
-             add_indices: bool = False, capitalise: bool = True):
+             add_indices: bool = False, capitalise: bool = True) -> None:
     '''
     Load labels and coordinates from a .xyz file
 
+    File assumes two header lines, first containing number of atoms
+    and second containing a comment or blank, followed by actual data
+
     Parameters
     ----------
     f_name : str
         File name
     atomic_numbers : bool, default False
         If True, reads xyz file with atomic numbers and converts to labels
     add_indices : bool, default False
@@ -40,16 +43,34 @@
 
     Returns
     -------
     list
         atomic labels
     np.ndarray
         (n_atoms,3) array containing xyz coordinates of each atom
+
+    Raises
+    ------
+    ValueError
+        If the .xyz file has incorrect length, or is missing the number
+        of atoms and comment lines
     '''
 
+    # Check file contains number of atoms on first line
+    with open(f_name, 'r') as f:
+        line = next(f)
+        if len(line.split()) != 1:
+            raise ValueError('.xyz file does not contain number of atoms')
+        else:
+            n_atoms = int(line)
+            n_lines = len(f.readlines()) + 1  # + 1 for next
+            if n_atoms + 2 != n_lines:
+
+                raise ValueError('.xyz file length/format is incorrect')
+
     if atomic_numbers:
         _numbers = np.loadtxt(
             f_name, skiprows=2, usecols=0, dtype=int, ndmin=1
         )
         _labels = num_to_lab(_numbers.tolist())
     else:
         _labels = np.loadtxt(f_name, skiprows=2, usecols=0, dtype=str, ndmin=1)
```

### Comparing `xyz_py-5.5.0/xyz_py.egg-info/PKG-INFO` & `xyz_py-5.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xyz-py
-Version: 5.5.0
+Name: xyz_py
+Version: 5.6.0
 Summary: A package for manipulating xyz files and chemical structures
 Home-page: https://gitlab.com/jonkragskow/xyz_py
 Author: Jon Kragskow
 Author-email: jonkragskow@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/jonkragskow/xyz_py/-/issues
 Project-URL: Documentation, https://jonkragskow.gitlab.io/xyz_py
 Classifier: Programming Language :: Python :: 3
```

