# Comparing `tmp/ninia-0.0.8.tar.gz` & `tmp/ninia-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\ajs0201\PycharmProjects\ninia\dist\tmpi5649qt6\ninia-0.0.8.tar", last modified: Tue Jun 22 23:34:35 2021, max compression
+gzip compressed data, was "C:\Users\ajs0201\PycharmProjects\ninia\dist\tmpx63x1vgh\ninia-0.0.9.tar", last modified: Tue Jun 22 23:39:30 2021, max compression
```

## Comparing `ninia-0.0.8.tar` & `ninia-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2021-06-22 23:34:35.309873 ninia-0.0.8/
--rw-rw-rw-   0        0        0     1088 2021-06-21 22:31:41.000000 ninia-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      718 2021-06-22 23:34:35.309873 ninia-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      142 2021-06-21 22:29:54.000000 ninia-0.0.8/README.md
--rw-rw-rw-   0        0        0      111 2021-06-21 21:53:26.000000 ninia-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2021-06-22 23:34:35.309873 ninia-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      939 2021-06-22 23:34:10.000000 ninia-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-06-22 23:34:35.295910 ninia-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2021-06-22 23:34:35.303889 ninia-0.0.8/src/ninia/
--rw-rw-rw-   0        0        0        0 2021-06-21 21:45:05.000000 ninia-0.0.8/src/ninia/__init__.py
--rw-rw-rw-   0        0        0       45 2021-06-21 21:47:30.000000 ninia-0.0.8/src/ninia/example.py
--rw-rw-rw-   0        0        0     1995 2021-06-22 20:18:25.000000 ninia-0.0.8/src/ninia/mw_species_.py
--rw-rw-rw-   0        0        0    11249 2021-06-22 23:34:10.000000 ninia-0.0.8/src/ninia/relax.py
-drwxrwxrwx   0        0        0        0 2021-06-22 23:34:35.307878 ninia-0.0.8/src/ninia.egg-info/
--rw-rw-rw-   0        0        0      718 2021-06-22 23:34:35.000000 ninia-0.0.8/src/ninia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2021-06-22 23:34:35.000000 ninia-0.0.8/src/ninia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-22 23:34:35.000000 ninia-0.0.8/src/ninia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2021-06-22 23:34:35.000000 ninia-0.0.8/src/ninia.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-06-22 23:39:30.060138 ninia-0.0.9/
+-rw-rw-rw-   0        0        0     1088 2021-06-21 22:31:41.000000 ninia-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      718 2021-06-22 23:39:30.060138 ninia-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2021-06-21 22:29:54.000000 ninia-0.0.9/README.md
+-rw-rw-rw-   0        0        0      111 2021-06-21 21:53:26.000000 ninia-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2021-06-22 23:39:30.060138 ninia-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      939 2021-06-22 23:37:45.000000 ninia-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-06-22 23:39:30.046175 ninia-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2021-06-22 23:39:30.054154 ninia-0.0.9/src/ninia/
+-rw-rw-rw-   0        0        0        0 2021-06-21 21:45:05.000000 ninia-0.0.9/src/ninia/__init__.py
+-rw-rw-rw-   0        0        0       45 2021-06-21 21:47:30.000000 ninia-0.0.9/src/ninia/example.py
+-rw-rw-rw-   0        0        0     1995 2021-06-22 20:18:25.000000 ninia-0.0.9/src/ninia/mw_species_.py
+-rw-rw-rw-   0        0        0    11220 2021-06-22 23:37:45.000000 ninia-0.0.9/src/ninia/relax.py
+drwxrwxrwx   0        0        0        0 2021-06-22 23:39:30.059143 ninia-0.0.9/src/ninia.egg-info/
+-rw-rw-rw-   0        0        0      718 2021-06-22 23:39:30.000000 ninia-0.0.9/src/ninia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2021-06-22 23:39:30.000000 ninia-0.0.9/src/ninia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-06-22 23:39:30.000000 ninia-0.0.9/src/ninia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2021-06-22 23:39:30.000000 ninia-0.0.9/src/ninia.egg-info/top_level.txt
```

### Comparing `ninia-0.0.8/LICENSE` & `ninia-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ninia-0.0.8/PKG-INFO` & `ninia-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninia
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small Python wrapper for Quantum Espresso - still in development
 Home-page: https://github.com/ajsummers/ninia
 Author: Alex Summers
 Author-email: ajs0201@auburn.edu
 License: UNKNOWN
 Project-URL: Issues, https://github.com/ajsummers/ninia/issues
 Platform: UNKNOWN
```

### Comparing `ninia-0.0.8/setup.py` & `ninia-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ninia",
-    version="0.0.8",
+    version="0.0.9",
     author="Alex Summers",
     author_email="ajs0201@auburn.edu",
     description="A small Python wrapper for Quantum Espresso - still in development",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ajsummers/ninia",
     project_urls={
```

### Comparing `ninia-0.0.8/src/ninia/mw_species_.py` & `ninia-0.0.9/src/ninia/mw_species_.py`

 * *Files identical despite different names*

### Comparing `ninia-0.0.8/src/ninia/relax.py` & `ninia-0.0.9/src/ninia/relax.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,16 +85,16 @@
         self.num_elem = len(unique_symbols)
         self.atomic_positions = atomic_positions
 
         return unique_symbols
 
     def get_species_info_(self, species_list, pseudodir=None):
 
-        # if (self.pseudo_dir is None) and (pseudodir is None):
-        #     raise RuntimeError('Define pseudopotential directory before geometry.')
+        # For some stupid reason a commented out exception was still killing the program
+        # so I deleted it here.
 
         os.chdir(pseudodir)
         list_upf = flt(os.listdir('.'), '*.[Uu][Pp][Ff]')
         species_string = ''
 
         for species in species_list:
```

### Comparing `ninia-0.0.8/src/ninia.egg-info/PKG-INFO` & `ninia-0.0.9/src/ninia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninia
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small Python wrapper for Quantum Espresso - still in development
 Home-page: https://github.com/ajsummers/ninia
 Author: Alex Summers
 Author-email: ajs0201@auburn.edu
 License: UNKNOWN
 Project-URL: Issues, https://github.com/ajsummers/ninia/issues
 Platform: UNKNOWN
```

