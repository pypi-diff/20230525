# Comparing `tmp/clonalEvolution-2.0.5.tar.gz` & `tmp/clonalEvolution-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clonalEvolution-2.0.5.tar", last modified: Mon May 22 16:31:53 2023, max compression
+gzip compressed data, was "clonalEvolution-2.0.6.tar", last modified: Thu May 25 21:36:39 2023, max compression
```

## Comparing `clonalEvolution-2.0.5.tar` & `clonalEvolution-2.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 16:31:53.218993 clonalEvolution-2.0.5/
--rw-rw-rw-   0        0        0    33092 2022-08-22 08:14:00.000000 clonalEvolution-2.0.5/LICENSE
--rw-rw-rw-   0        0        0     5378 2023-05-22 16:31:53.219991 clonalEvolution-2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4385 2022-11-14 12:37:06.000000 clonalEvolution-2.0.5/README.md
--rw-rw-rw-   0        0        0      101 2022-08-26 06:02:56.000000 clonalEvolution-2.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       81 2023-05-22 16:31:53.220988 clonalEvolution-2.0.5/setup.cfg
--rw-rw-rw-   0        0        0     3866 2023-05-22 16:23:37.000000 clonalEvolution-2.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:31:53.157040 clonalEvolution-2.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 16:31:53.202116 clonalEvolution-2.0.5/src/clonalEvolution/
--rw-rw-rw-   0        0        0        0 2022-08-19 13:09:48.000000 clonalEvolution-2.0.5/src/clonalEvolution/__init__.py
--rw-rw-rw-   0        0        0    21317 2023-05-22 16:22:59.000000 clonalEvolution-2.0.5/src/clonalEvolution/__main__.py
--rw-rw-rw-   0        0        0    11534 2022-10-20 07:43:40.000000 clonalEvolution-2.0.5/src/clonalEvolution/clonal_evolution_binned_loop.py
--rw-rw-rw-   0        0        0     8264 2022-12-14 17:16:26.000000 clonalEvolution-2.0.5/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py
--rw-rw-rw-   0        0        0    25157 2023-05-16 23:45:49.000000 clonalEvolution-2.0.5/src/clonalEvolution/clonal_evolution_init.py
--rw-rw-rw-   0        0        0     5977 2022-11-06 16:00:04.000000 clonalEvolution-2.0.5/src/clonalEvolution/clonal_evolution_loop.py
--rw-rw-rw-   0        0        0    32529 2023-05-16 08:25:54.000000 clonalEvolution-2.0.5/src/clonalEvolution/external_plots.py
--rw-rw-rw-   0        0        0    45629 2023-05-16 23:36:11.000000 clonalEvolution-2.0.5/src/clonalEvolution/mainView.py
--rw-rw-rw-   0        0        0      185 2022-08-22 08:11:04.000000 clonalEvolution-2.0.5/src/clonalEvolution/wmean.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:31:53.214007 clonalEvolution-2.0.5/src/clonalEvolution.egg-info/
--rw-rw-rw-   0        0        0     5378 2023-05-22 16:31:53.000000 clonalEvolution-2.0.5/src/clonalEvolution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      695 2023-05-22 16:31:53.000000 clonalEvolution-2.0.5/src/clonalEvolution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 16:31:53.000000 clonalEvolution-2.0.5/src/clonalEvolution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-22 16:31:53.000000 clonalEvolution-2.0.5/src/clonalEvolution.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-05-22 16:31:53.000000 clonalEvolution-2.0.5/src/clonalEvolution.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-22 16:31:53.000000 clonalEvolution-2.0.5/src/clonalEvolution.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-22 16:31:53.216998 clonalEvolution-2.0.5/tests/
--rw-rw-rw-   0        0        0      417 2022-03-24 22:23:18.000000 clonalEvolution-2.0.5/tests/test_simple.py
+drwxrwxrwx   0        0        0        0 2023-05-25 21:36:39.006946 clonalEvolution-2.0.6/
+-rw-rw-rw-   0        0        0    33092 2022-08-22 08:14:00.000000 clonalEvolution-2.0.6/LICENSE
+-rw-rw-rw-   0        0        0     5378 2023-05-25 21:36:39.006946 clonalEvolution-2.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4385 2022-11-14 12:37:06.000000 clonalEvolution-2.0.6/README.md
+-rw-rw-rw-   0        0        0      101 2022-08-26 06:02:56.000000 clonalEvolution-2.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2023-05-25 21:36:39.007944 clonalEvolution-2.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     3866 2023-05-25 21:36:12.000000 clonalEvolution-2.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 21:36:38.952070 clonalEvolution-2.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 21:36:38.985005 clonalEvolution-2.0.6/src/clonalEvolution/
+-rw-rw-rw-   0        0        0        0 2022-08-19 13:09:48.000000 clonalEvolution-2.0.6/src/clonalEvolution/__init__.py
+-rw-rw-rw-   0        0        0    21317 2023-05-22 16:22:59.000000 clonalEvolution-2.0.6/src/clonalEvolution/__main__.py
+-rw-rw-rw-   0        0        0    11534 2022-10-20 07:43:40.000000 clonalEvolution-2.0.6/src/clonalEvolution/clonal_evolution_binned_loop.py
+-rw-rw-rw-   0        0        0     8264 2022-12-14 17:16:26.000000 clonalEvolution-2.0.6/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py
+-rw-rw-rw-   0        0        0    25157 2023-05-16 23:45:49.000000 clonalEvolution-2.0.6/src/clonalEvolution/clonal_evolution_init.py
+-rw-rw-rw-   0        0        0     5977 2022-11-06 16:00:04.000000 clonalEvolution-2.0.6/src/clonalEvolution/clonal_evolution_loop.py
+-rw-rw-rw-   0        0        0    32531 2023-05-25 21:35:45.000000 clonalEvolution-2.0.6/src/clonalEvolution/external_plots.py
+-rw-rw-rw-   0        0        0    45629 2023-05-16 23:36:11.000000 clonalEvolution-2.0.6/src/clonalEvolution/mainView.py
+-rw-rw-rw-   0        0        0      185 2022-08-22 08:11:04.000000 clonalEvolution-2.0.6/src/clonalEvolution/wmean.py
+drwxrwxrwx   0        0        0        0 2023-05-25 21:36:39.000967 clonalEvolution-2.0.6/src/clonalEvolution.egg-info/
+-rw-rw-rw-   0        0        0     5378 2023-05-25 21:36:38.000000 clonalEvolution-2.0.6/src/clonalEvolution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2023-05-25 21:36:38.000000 clonalEvolution-2.0.6/src/clonalEvolution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 21:36:38.000000 clonalEvolution-2.0.6/src/clonalEvolution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-25 21:36:38.000000 clonalEvolution-2.0.6/src/clonalEvolution.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2023-05-25 21:36:38.000000 clonalEvolution-2.0.6/src/clonalEvolution.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-25 21:36:38.000000 clonalEvolution-2.0.6/src/clonalEvolution.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 21:36:39.003954 clonalEvolution-2.0.6/tests/
+-rw-rw-rw-   0        0        0      417 2022-03-24 22:23:18.000000 clonalEvolution-2.0.6/tests/test_simple.py
```

### Comparing `clonalEvolution-2.0.5/LICENSE` & `clonalEvolution-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.5/PKG-INFO` & `clonalEvolution-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clonalEvolution
-Version: 2.0.5
+Version: 2.0.6
 Summary: Software for simulating clonal evolution in binned and tau leap version.
 Home-page: https://github.com/JGil-polsl/clonalEvolution
 Author: Jaroslaw Gil
 Author-email: jaroslaw.gil@polsl.pl
 Project-URL: Bug Reports, https://github.com/JGil-polsl/clonalEvolution/issues
 Project-URL: Source, https://github.com/JGil-polsl/clonalEvolution
 Keywords: clonal evolution,microbial,numerical modelling
```

### Comparing `clonalEvolution-2.0.5/README.md` & `clonalEvolution-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.5/setup.py` & `clonalEvolution-2.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Fields marked as "Optional" may be commented out.
 
 setup(
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name="clonalEvolution", 
-    version="2.0.5",
+    version="2.0.6",
     description="Software for simulating clonal evolution in binned and tau leap version.",
     url="https://github.com/JGil-polsl/clonalEvolution",
     author="Jaroslaw Gil",  
     author_email="jaroslaw.gil@polsl.pl",
     long_description=long_description,
     long_description_content_type='text/markdown',
     # Classifiers help users find your project by categorizing it.
```

### Comparing `clonalEvolution-2.0.5/src/clonalEvolution/__main__.py` & `clonalEvolution-2.0.6/src/clonalEvolution/__main__.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.5/src/clonalEvolution/clonal_evolution_binned_loop.py` & `clonalEvolution-2.0.6/src/clonalEvolution/clonal_evolution_binned_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.5/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py` & `clonalEvolution-2.0.6/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.5/src/clonalEvolution/clonal_evolution_init.py` & `clonalEvolution-2.0.6/src/clonalEvolution/clonal_evolution_init.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.5/src/clonalEvolution/clonal_evolution_loop.py` & `clonalEvolution-2.0.6/src/clonalEvolution/clonal_evolution_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.5/src/clonalEvolution/external_plots.py` & `clonalEvolution-2.0.6/src/clonalEvolution/external_plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -498,15 +498,15 @@
     path_out - absolute path to figures save localization
     '''
     prop = np.transpose([paths_in, ids])
     for path_in, _id in prop:    
         if not path_in.endswith('.mtx'):
             print("Wrong file")
             return
-        os.chdir(paths_out)
+        # os.chdir(paths_out)
         path_out = '/'.join(np.array(path_in.split('/'))[0:len(path_in.split('/'))-1]) + '/Figures/' + _id +'/'
     
         df = pd.read_csv(path_in)
         
         mm = []
         for row in df.iterrows():
             try:
```

### Comparing `clonalEvolution-2.0.5/src/clonalEvolution/mainView.py` & `clonalEvolution-2.0.6/src/clonalEvolution/mainView.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.5/src/clonalEvolution.egg-info/PKG-INFO` & `clonalEvolution-2.0.6/src/clonalEvolution.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clonalEvolution
-Version: 2.0.5
+Version: 2.0.6
 Summary: Software for simulating clonal evolution in binned and tau leap version.
 Home-page: https://github.com/JGil-polsl/clonalEvolution
 Author: Jaroslaw Gil
 Author-email: jaroslaw.gil@polsl.pl
 Project-URL: Bug Reports, https://github.com/JGil-polsl/clonalEvolution/issues
 Project-URL: Source, https://github.com/JGil-polsl/clonalEvolution
 Keywords: clonal evolution,microbial,numerical modelling
```

### Comparing `clonalEvolution-2.0.5/src/clonalEvolution.egg-info/SOURCES.txt` & `clonalEvolution-2.0.6/src/clonalEvolution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

