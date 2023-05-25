# Comparing `tmp/geocontour-1.3.0.tar.gz` & `tmp/geocontour-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocontour-1.3.0.tar", last modified: Sat May 13 23:56:59 2023, max compression
+gzip compressed data, was "geocontour-1.3.1.tar", last modified: Thu May 25 02:17:50 2023, max compression
```

## Comparing `geocontour-1.3.0.tar` & `geocontour-1.3.1.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-13 23:56:59.249652 geocontour-1.3.0/
--rw-r--r--   0 bkrichman   (501) staff       (20)      190 2023-03-20 18:00:45.000000 geocontour-1.3.0/.gitignore
--rw-r--r--   0 bkrichman   (501) staff       (20)      559 2023-05-13 23:45:44.000000 geocontour-1.3.0/CITATION.cff
--rw-r--r--   0 bkrichman   (501) staff       (20)     1079 2023-03-07 20:16:09.000000 geocontour-1.3.0/LICENSE.txt
--rw-r--r--   0 bkrichman   (501) staff       (20)      314 2022-12-31 15:38:33.000000 geocontour-1.3.0/MANIFEST.in
--rw-r--r--   0 bkrichman   (501) staff       (20)    11470 2023-05-13 23:56:59.248463 geocontour-1.3.0/PKG-INFO
--rw-r--r--   0 bkrichman   (501) staff       (20)    10737 2023-05-13 23:52:27.000000 geocontour-1.3.0/README.md
-drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-13 23:56:59.164192 geocontour-1.3.0/geocontour/
--rw-r--r--   0 bkrichman   (501) staff       (20)      426 2023-03-20 16:17:38.000000 geocontour-1.3.0/geocontour/__init__.py
--rw-r--r--   0 bkrichman   (501) staff       (20)     7222 2023-03-20 16:17:38.000000 geocontour-1.3.0/geocontour/check.py
--rw-r--r--   0 bkrichman   (501) staff       (20)    54078 2023-05-13 23:30:17.000000 geocontour-1.3.0/geocontour/contourtrace.py
--rw-r--r--   0 bkrichman   (501) staff       (20)    11433 2023-03-20 16:17:38.000000 geocontour-1.3.0/geocontour/contourutil.py
-drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-13 23:56:59.179152 geocontour-1.3.0/geocontour/data/
--rw-r--r--   0 bkrichman   (501) staff       (20)   108990 2022-12-04 15:35:26.000000 geocontour-1.3.0/geocontour/data/MissBasin_boundary.npz
--rw-r--r--   0 bkrichman   (501) staff       (20)     3166 2022-12-04 15:26:13.000000 geocontour-1.3.0/geocontour/data/generic_boundary.npz
-drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-13 23:56:59.180234 geocontour-1.3.0/geocontour/examples/
--rw-r--r--   0 bkrichman   (501) staff       (20)     9417 2023-03-20 16:17:38.000000 geocontour-1.3.0/geocontour/examples/__init__.py
--rw-r--r--   0 bkrichman   (501) staff       (20)     5977 2023-03-20 16:17:38.000000 geocontour-1.3.0/geocontour/geocontour.py
--rw-r--r--   0 bkrichman   (501) staff       (20)     9263 2023-03-20 16:17:38.000000 geocontour-1.3.0/geocontour/grid.py
--rw-r--r--   0 bkrichman   (501) staff       (20)    14461 2023-03-20 16:17:38.000000 geocontour-1.3.0/geocontour/masksearch.py
--rw-r--r--   0 bkrichman   (501) staff       (20)     9951 2023-03-20 16:17:38.000000 geocontour-1.3.0/geocontour/maskutil.py
--rw-r--r--   0 bkrichman   (501) staff       (20)    29100 2023-03-20 16:17:38.000000 geocontour-1.3.0/geocontour/output.py
-drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-13 23:56:59.182896 geocontour-1.3.0/geocontour/tests/
--rw-r--r--   0 bkrichman   (501) staff       (20)     7285 2023-05-13 23:30:17.000000 geocontour-1.3.0/geocontour/tests/__init__.py
--rw-r--r--   0 bkrichman   (501) staff       (20)    13553 2023-05-13 23:30:17.000000 geocontour-1.3.0/geocontour/tests/timing.py
-drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-13 23:56:59.176411 geocontour-1.3.0/geocontour.egg-info/
--rw-r--r--   0 bkrichman   (501) staff       (20)    11470 2023-05-13 23:56:59.000000 geocontour-1.3.0/geocontour.egg-info/PKG-INFO
--rw-r--r--   0 bkrichman   (501) staff       (20)     1101 2023-05-13 23:56:59.000000 geocontour-1.3.0/geocontour.egg-info/SOURCES.txt
--rw-r--r--   0 bkrichman   (501) staff       (20)        1 2023-05-13 23:56:59.000000 geocontour-1.3.0/geocontour.egg-info/dependency_links.txt
--rw-r--r--   0 bkrichman   (501) staff       (20)       41 2023-05-13 23:56:59.000000 geocontour-1.3.0/geocontour.egg-info/requires.txt
--rw-r--r--   0 bkrichman   (501) staff       (20)       11 2023-05-13 23:56:59.000000 geocontour-1.3.0/geocontour.egg-info/top_level.txt
-drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-13 23:56:59.246876 geocontour-1.3.0/images/
--rwxrwxr--   0 bkrichman   (501) staff       (20)  1720228 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_large_boundary+mask.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)  1499990 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_large_contour.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)  1723815 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_large_contoursearch.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)  3480862 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_large_geocontour+bordfeat.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)  4377349 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_large_geocontour+natfeat.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)  1736596 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_large_geocontour.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)   148016 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_small_boundary+mask.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)    95607 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_small_contour.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)   161593 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_small_contoursearch.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)   142525 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_small_geocontour.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)   143125 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_small_geocontour_simp.png
--rw-r--r--   0 bkrichman   (501) staff       (20)    13364 2022-12-04 21:44:14.000000 geocontour-1.3.0/images/icon_geocontour.png
--rw-r--r--   0 bkrichman   (501) staff       (20)      330 2023-05-13 23:42:27.000000 geocontour-1.3.0/requirements+cartopy.txt
--rw-r--r--   0 bkrichman   (501) staff       (20)      269 2023-05-13 23:41:02.000000 geocontour-1.3.0/requirements.txt
--rw-r--r--   0 bkrichman   (501) staff       (20)       38 2023-05-13 23:56:59.249816 geocontour-1.3.0/setup.cfg
--rw-r--r--   0 bkrichman   (501) staff       (20)     1125 2023-05-13 23:34:09.000000 geocontour-1.3.0/setup.py
+drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-25 02:17:50.537950 geocontour-1.3.1/
+-rw-r--r--   0 bkrichman   (501) staff       (20)      190 2023-03-20 18:00:45.000000 geocontour-1.3.1/.gitignore
+-rw-r--r--   0 bkrichman   (501) staff       (20)      559 2023-05-25 02:15:12.000000 geocontour-1.3.1/CITATION.cff
+-rw-r--r--   0 bkrichman   (501) staff       (20)     1079 2023-03-07 20:16:09.000000 geocontour-1.3.1/LICENSE.txt
+-rw-r--r--   0 bkrichman   (501) staff       (20)      314 2022-12-31 15:38:33.000000 geocontour-1.3.1/MANIFEST.in
+-rw-r--r--   0 bkrichman   (501) staff       (20)    11470 2023-05-25 02:17:50.536539 geocontour-1.3.1/PKG-INFO
+-rw-r--r--   0 bkrichman   (501) staff       (20)    10737 2023-05-25 02:14:26.000000 geocontour-1.3.1/README.md
+drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-25 02:17:50.450133 geocontour-1.3.1/geocontour/
+-rw-r--r--   0 bkrichman   (501) staff       (20)      426 2023-03-20 16:17:38.000000 geocontour-1.3.1/geocontour/__init__.py
+-rw-r--r--   0 bkrichman   (501) staff       (20)     7222 2023-03-20 16:17:38.000000 geocontour-1.3.1/geocontour/check.py
+-rw-r--r--   0 bkrichman   (501) staff       (20)    53598 2023-05-22 01:49:09.000000 geocontour-1.3.1/geocontour/contourtrace.py
+-rw-r--r--   0 bkrichman   (501) staff       (20)    11433 2023-03-20 16:17:38.000000 geocontour-1.3.1/geocontour/contourutil.py
+drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-25 02:17:50.458884 geocontour-1.3.1/geocontour/data/
+-rw-r--r--   0 bkrichman   (501) staff       (20)   108990 2022-12-04 15:35:26.000000 geocontour-1.3.1/geocontour/data/MissBasin_boundary.npz
+-rw-r--r--   0 bkrichman   (501) staff       (20)     1028 2023-05-22 01:49:09.000000 geocontour-1.3.1/geocontour/data/box_boundary.npz
+-rw-r--r--   0 bkrichman   (501) staff       (20)     3166 2022-12-04 15:26:13.000000 geocontour-1.3.1/geocontour/data/generic_boundary.npz
+-rw-r--r--   0 bkrichman   (501) staff       (20)     1236 2023-05-22 01:49:09.000000 geocontour-1.3.1/geocontour/data/test_case_boundary.npz
+drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-25 02:17:50.459864 geocontour-1.3.1/geocontour/examples/
+-rw-r--r--   0 bkrichman   (501) staff       (20)     9417 2023-03-20 16:17:38.000000 geocontour-1.3.1/geocontour/examples/__init__.py
+-rw-r--r--   0 bkrichman   (501) staff       (20)     5977 2023-03-20 16:17:38.000000 geocontour-1.3.1/geocontour/geocontour.py
+-rw-r--r--   0 bkrichman   (501) staff       (20)     9263 2023-03-20 16:17:38.000000 geocontour-1.3.1/geocontour/grid.py
+-rw-r--r--   0 bkrichman   (501) staff       (20)    14461 2023-03-20 16:17:38.000000 geocontour-1.3.1/geocontour/masksearch.py
+-rw-r--r--   0 bkrichman   (501) staff       (20)     9951 2023-03-20 16:17:38.000000 geocontour-1.3.1/geocontour/maskutil.py
+-rw-r--r--   0 bkrichman   (501) staff       (20)    29644 2023-05-25 01:58:27.000000 geocontour-1.3.1/geocontour/output.py
+drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-25 02:17:50.461430 geocontour-1.3.1/geocontour/tests/
+-rw-r--r--   0 bkrichman   (501) staff       (20)     7285 2023-05-13 23:30:17.000000 geocontour-1.3.1/geocontour/tests/__init__.py
+-rw-r--r--   0 bkrichman   (501) staff       (20)    13553 2023-05-22 01:10:58.000000 geocontour-1.3.1/geocontour/tests/timing.py
+drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-25 02:17:50.453863 geocontour-1.3.1/geocontour.egg-info/
+-rw-r--r--   0 bkrichman   (501) staff       (20)    11470 2023-05-25 02:17:50.000000 geocontour-1.3.1/geocontour.egg-info/PKG-INFO
+-rw-r--r--   0 bkrichman   (501) staff       (20)     1173 2023-05-25 02:17:50.000000 geocontour-1.3.1/geocontour.egg-info/SOURCES.txt
+-rw-r--r--   0 bkrichman   (501) staff       (20)        1 2023-05-25 02:17:50.000000 geocontour-1.3.1/geocontour.egg-info/dependency_links.txt
+-rw-r--r--   0 bkrichman   (501) staff       (20)       41 2023-05-25 02:17:50.000000 geocontour-1.3.1/geocontour.egg-info/requires.txt
+-rw-r--r--   0 bkrichman   (501) staff       (20)       11 2023-05-25 02:17:50.000000 geocontour-1.3.1/geocontour.egg-info/top_level.txt
+drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-25 02:17:50.535039 geocontour-1.3.1/images/
+-rwxrwxr--   0 bkrichman   (501) staff       (20)  1720228 2022-12-19 01:54:17.000000 geocontour-1.3.1/images/example_large_boundary+mask.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)  1499990 2022-12-19 01:54:17.000000 geocontour-1.3.1/images/example_large_contour.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)  1723815 2022-12-19 01:54:17.000000 geocontour-1.3.1/images/example_large_contoursearch.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)  3480862 2022-12-19 01:54:17.000000 geocontour-1.3.1/images/example_large_geocontour+bordfeat.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)  4377349 2022-12-19 01:54:17.000000 geocontour-1.3.1/images/example_large_geocontour+natfeat.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)  1736596 2022-12-19 01:54:17.000000 geocontour-1.3.1/images/example_large_geocontour.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)   148016 2022-12-19 01:54:17.000000 geocontour-1.3.1/images/example_small_boundary+mask.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)    95607 2022-12-19 01:54:17.000000 geocontour-1.3.1/images/example_small_contour.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)   161593 2022-12-19 01:54:17.000000 geocontour-1.3.1/images/example_small_contoursearch.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)   142525 2022-12-19 01:54:17.000000 geocontour-1.3.1/images/example_small_geocontour.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)   143125 2022-12-19 01:54:17.000000 geocontour-1.3.1/images/example_small_geocontour_simp.png
+-rw-r--r--   0 bkrichman   (501) staff       (20)    13364 2022-12-04 21:44:14.000000 geocontour-1.3.1/images/icon_geocontour.png
+-rw-r--r--   0 bkrichman   (501) staff       (20)      330 2023-05-25 02:13:02.000000 geocontour-1.3.1/requirements+cartopy.txt
+-rw-r--r--   0 bkrichman   (501) staff       (20)      269 2023-05-25 02:11:52.000000 geocontour-1.3.1/requirements.txt
+-rw-r--r--   0 bkrichman   (501) staff       (20)       38 2023-05-25 02:17:50.538158 geocontour-1.3.1/setup.cfg
+-rw-r--r--   0 bkrichman   (501) staff       (20)     1125 2023-05-25 02:13:25.000000 geocontour-1.3.1/setup.py
```

### Comparing `geocontour-1.3.0/CITATION.cff` & `geocontour-1.3.1/CITATION.cff`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-cff-version: 1.3.0
+cff-version: 1.3.1
 message: "If you use this software, please cite it as below."
 abstract: "Utilities for masking, contour tracing, and geocontour construction with gridded geographic data"
 authors:
   -
     family-names: Krichman
     given-names: Benjamin
     orcid: "https://orcid.org/0000-0002-7481-8281"
 title: "geocontour"
-date-released: 2023-05-13
+date-released: 2023-05-24
 doi: "10.5281/zenodo.7402714"
 keywords:
   - python
   - geospatial
   - masking
   - contour-tracing
   - gridded-data
 license: MIT
 repository-code: "https://github.com/benkrichman/geocontour"
-version: "1.3.0"
+version: "1.3.1"
```

### Comparing `geocontour-1.3.0/LICENSE.txt` & `geocontour-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/PKG-INFO` & `geocontour-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocontour
-Version: 1.3.0
+Version: 1.3.1
 Summary: Utilities for masking, contour tracing, and geocontour construction with gridded geographic data
 Home-page: https://github.com/benkrichman/geocontour
 Author: Benjamin Krichman
 Author-email: benkrichman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -48,28 +48,28 @@
 
 Find the full documentation hosted [here](https://geocontour.readthedocs.io/en/latest/index.html).
 
 ## Citation
 
 If geocontour played a significant role in your work and you would like to cite it, the following is suggested (APA):
 
-Krichman, B. (2023). *geocontour* (Version 1.3.0) [Computer Software]. https://doi.org/10.5281/zenodo.7402714
+Krichman, B. (2023). *geocontour* (Version 1.3.1) [Computer Software]. https://doi.org/10.5281/zenodo.7402714
 
 Bibtex:
 
 ```latex
 @software{geocontour,
 author={Krichman, Benjamin},
 doi={10.5281/zenodo.7402714},
 license={MIT},
 month={5},
 year={2023},
 title={{geocontour}},
 url={https://github.com/benkrichman/geocontour},
-version={1.3.0},
+version={1.3.1},
 note = {Computer Software}
 }
 ```
 
 ## Features
 
 ### Masks
```

### Comparing `geocontour-1.3.0/README.md` & `geocontour-1.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -30,28 +30,28 @@
 
 Find the full documentation hosted [here](https://geocontour.readthedocs.io/en/latest/index.html).
 
 ## Citation
 
 If geocontour played a significant role in your work and you would like to cite it, the following is suggested (APA):
 
-Krichman, B. (2023). *geocontour* (Version 1.3.0) [Computer Software]. https://doi.org/10.5281/zenodo.7402714
+Krichman, B. (2023). *geocontour* (Version 1.3.1) [Computer Software]. https://doi.org/10.5281/zenodo.7402714
 
 Bibtex:
 
 ```latex
 @software{geocontour,
 author={Krichman, Benjamin},
 doi={10.5281/zenodo.7402714},
 license={MIT},
 month={5},
 year={2023},
 title={{geocontour}},
 url={https://github.com/benkrichman/geocontour},
-version={1.3.0},
+version={1.3.1},
 note = {Computer Software}
 }
 ```
 
 ## Features
 
 ### Masks
```

### Comparing `geocontour-1.3.0/geocontour/check.py` & `geocontour-1.3.1/geocontour/check.py`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/geocontour/contourtrace.py` & `geocontour-1.3.1/geocontour/contourtrace.py`

 * *Files 1% similar despite different names*

```diff
@@ -498,15 +498,15 @@
                 stops when the start cell has been re-visited with the
                 same orientation as started with
             ``Nvisits``
                 stops when the start cell has been re-visited N number
                 of times (N set by `startvisits` parameter)
             ``either``
                 stops when either Elisoff or Nvisits has been satisfied
-    startvisits : int, default=3
+    startvisits : int, default=1
         the number of times re-visiting the start cell will trigger an
         end to the search
     remcontourrepeat : bool, default=True
         select whether to remove consecutive repeating cells in the
         output `contour`
     remsearchrepeat : bool, default=False
         select whether to remove consecutive repeating cells in the
@@ -603,46 +603,40 @@
         FO=cell+orientation+outsideturn(orientation)
         F=cell+orientation
         FI=cell+orientation+insideturn(orientation)
         if buffermask[FO[0],FO[1]]==True:
             searchcells.append(FO)
             contourcells.append(FO)
             cell=FO
-            if (cell==startcell).all():
-                Nvisits+=1
-            rotations=0
-            breakloop=checkbreak(cell,orientation,Nvisits)
             orientation=outsideturn(orientation)
+            rotations=0
         elif buffermask[F[0],F[1]]==True:
             searchcells.append(FO)
             searchcells.append(F)
             contourcells.append(F)
             cell=F
-            if (cell==startcell).all():
-                Nvisits+=1
             rotations=0
-            breakloop=checkbreak(cell,orientation,Nvisits)
         elif buffermask[FI[0],FI[1]]==True:
             searchcells.append(FO)
             searchcells.append(F)
             searchcells.append(FI)
             contourcells.append(FI)
             cell=FI
-            if (cell==startcell).all():
-                Nvisits+=1
             rotations=0
-            breakloop=checkbreak(cell,orientation,Nvisits)
         else:
             searchcells.append(FO)
             searchcells.append(F)
             searchcells.append(FI)
             orientation=insideturn(orientation)
             rotations+=1
         if rotations>3:
             sys.exit('ERROR - Stuck on isolated cell '+str(cell))
+        if (cell==startcell).all() and len(contourcells)>1:
+            Nvisits+=1
+        breakloop=checkbreak(cell,orientation,Nvisits)
     contour,contoursearch=gccu.clean(contourcells,searchcells,latitudes=latitudes,longitudes=longitudes,closecontour=closecontour,remcontourrepeat=remcontourrepeat,remsearchrepeat=remsearchrepeat)
     return contour,contoursearch
 
 def pavlidis_imp(mask,latitudes=None,longitudes=None,direction='cw',start='auto',stop='Nvisits',startvisits=1,remcontourrepeat=True,remsearchrepeat=False,closecontour=True):
     """
     Find the contour of a mask using an improved Pavlidis algorithm that
     reliably captures inside corners
@@ -675,15 +669,15 @@
                 stops when the start cell has been re-visited with the
                 same orientation as started with
             ``Nvisits``
                 stops when the start cell has been re-visited N number
                 of times (N set by `startvisits` parameter)
             ``either``
                 stops when either Elisoff or Nvisits has been satisfied
-    startvisits : int, default=3
+    startvisits : int, default=1
         the number of times re-visiting the start cell will trigger an
         end to the search
     remcontourrepeat : bool, default=True
         select whether to remove consecutive repeating cells in the
         output `contour`
     remsearchrepeat : bool, default=False
         select whether to remove consecutive repeating cells in the
@@ -775,53 +769,47 @@
         if buffermask[FO[0],FO[1]]==True:
             if buffermask[F[0],F[1]]==True:
                 contourcells.append(F)
             searchcells.append(F)
             searchcells.append(FO)
             contourcells.append(FO)
             cell=FO
-            if (cell==startcell).all():
-                Nvisits+=1
             rotations=0
-            breakloop=checkbreak(cell,orientation,Nvisits)
             orientation=outsideturn(orientation)
         elif buffermask[F[0],F[1]]==True:
             searchcells.append(FO)
             searchcells.append(F)
             contourcells.append(F)
             cell=F
-            if (cell==startcell).all():
-                Nvisits+=1
             rotations=0
-            breakloop=checkbreak(cell,orientation,Nvisits)
         elif buffermask[FI[0],FI[1]]==True:
             if buffermask[I[0],I[1]]==True:
                 contourcells.append(I)
             searchcells.append(FO)
             searchcells.append(F)
             searchcells.append(I)
             searchcells.append(FI)
             contourcells.append(FI)
             cell=FI
-            if (cell==startcell).all():
-                Nvisits+=1
             rotations=0
-            breakloop=checkbreak(cell,orientation,Nvisits)
         else:
             searchcells.append(FO)
             searchcells.append(F)
             searchcells.append(FI)
             orientation=insideturn(orientation)
             rotations+=1
         if rotations>3:
             sys.exit('ERROR - Stuck on isolated cell '+str(cell))
+        if (cell==startcell).all() and len(contourcells)>1:
+            Nvisits+=1
+        breakloop=checkbreak(cell,orientation,Nvisits)
     contour,contoursearch=gccu.clean(contourcells,searchcells,latitudes=latitudes,longitudes=longitudes,closecontour=closecontour,remcontourrepeat=remcontourrepeat,remsearchrepeat=remsearchrepeat)
     return contour,contoursearch
 
-def MSBF(mask,latitudes=None,longitudes=None,direction='cw',start='auto',stop='either',startvisits=4,remcontourrepeat=True,remsearchrepeat=False,closecontour=True):
+def MSBF(mask,latitudes=None,longitudes=None,direction='cw',start='auto',stop='either',startvisits=3,remcontourrepeat=True,remsearchrepeat=False,closecontour=True):
     """
     Find the contour of a mask using the modified simple boundary
     following algorithm
 
     Parameters
     ----------
     mask : ndarray
@@ -969,15 +957,15 @@
             tag=False
         if (cell==startcell).all():
             Nvisits+=1
         breakloop=checkbreak(cell,orientation,Nvisits)
     contour,contoursearch=gccu.clean(contourcells,searchcells,latitudes=latitudes,longitudes=longitudes,closecontour=closecontour,remcontourrepeat=remcontourrepeat,remsearchrepeat=remsearchrepeat)
     return contour,contoursearch
 
-def ISBF(mask,latitudes=None,longitudes=None,direction='cw',start='auto',stop='either',startvisits=4,remcontourrepeat=True,remsearchrepeat=False,closecontour=True):
+def ISBF(mask,latitudes=None,longitudes=None,direction='cw',start='auto',stop='either',startvisits=3,remcontourrepeat=True,remsearchrepeat=False,closecontour=True):
     """
     Find the contour of a mask using the improved simple boundary
     following algorithm
 
     Parameters
     ----------
     mask : ndarray
@@ -1155,15 +1143,15 @@
                 tag=False
         if (cell==startcell).all():
             Nvisits+=1
         breakloop=checkbreak(cell,orientation,Nvisits)
     contour,contoursearch=gccu.clean(contourcells,searchcells,latitudes=latitudes,longitudes=longitudes,closecontour=closecontour,remcontourrepeat=remcontourrepeat,remsearchrepeat=remsearchrepeat)
     return contour,contoursearch
 
-def TSR(mask,latitudes=None,longitudes=None,direction='cw',start='auto',stop='either',startvisits=4,remcontourrepeat=True,remsearchrepeat=False,closecontour=True):
+def TSR(mask,latitudes=None,longitudes=None,direction='cw',start='auto',stop='either',startvisits=3,remcontourrepeat=True,remsearchrepeat=False,closecontour=True):
     """
     Find the contour of a mask using the two-step representative tracing
     algorithm
 
     Parameters
     ----------
     mask : ndarray
```

### Comparing `geocontour-1.3.0/geocontour/contourutil.py` & `geocontour-1.3.1/geocontour/contourutil.py`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/geocontour/data/MissBasin_boundary.npz` & `geocontour-1.3.1/geocontour/data/MissBasin_boundary.npz`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/geocontour/data/generic_boundary.npz` & `geocontour-1.3.1/geocontour/data/generic_boundary.npz`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/geocontour/examples/__init__.py` & `geocontour-1.3.1/geocontour/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/geocontour/geocontour.py` & `geocontour-1.3.1/geocontour/geocontour.py`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/geocontour/grid.py` & `geocontour-1.3.1/geocontour/grid.py`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/geocontour/masksearch.py` & `geocontour-1.3.1/geocontour/masksearch.py`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/geocontour/maskutil.py` & `geocontour-1.3.1/geocontour/maskutil.py`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/geocontour/output.py` & `geocontour-1.3.1/geocontour/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import geocontour.contourutil as gccu
 try:
     import cartopy as cp
     cp_exists='y'
 except:
     cp_exists='n'
 
-def plot(latitudes,longitudes,boundary=None,mask=None,contour=None,contoursearch=None,geocontour=None,vertices=None,boundingbox='all',buffer=False,grid=True,cells='default',showcontour=True,startcell=True,contourarrows=True,contoursearcharrows=True,fancycontoursearch=True,contoursearch_contraction=0.2,contoursearch_shift=0.25,geocontourvectors=True,emptycellcolor='lightgrey',fullcellcolor='sandybrown',boundarycolor='tab:blue',contourcolor='olivedrab',contoursearchcolor='firebrick',geocontourcolor='olivedrab',vertexcolor='tab:cyan',gridcolor='black',lw_boundary=0.1,lw_contour=0.1,lw_contoursearch='auto',lw_geocontour=0.1,mw_contourarrows=0.5,mw_contoursearcharrows='auto',mw_vertices=0.4,features=None,title=None,labs=True,outname='plot',outdpi='high',transp=False):
+def plot(latitudes,longitudes,boundary=None,mask=None,contour=None,contoursearch=None,geocontour=None,vertices=None,boundingbox='all',buffer=False,grid=True,cells='default',undermask=False,showcontour=True,startcell=True,contourarrows=True,contoursearcharrows=True,fancycontoursearch=True,contoursearch_contraction=0.2,contoursearch_shift=0.25,geocontourvectors=True,emptycellcolor='lightgrey',fullcellcolor='sandybrown',undermaskcolor='slategrey',boundarycolor='tab:blue',contourcolor='olivedrab',contoursearchcolor='firebrick',geocontourcolor='olivedrab',vertexcolor='tab:cyan',gridcolor='black',lw_boundary=0.1,lw_contour=0.1,lw_contoursearch='auto',lw_geocontour=0.1,mw_contourarrows=0.5,mw_contoursearcharrows='auto',mw_vertices=0.4,features=None,title=None,labs=True,outname='plot',outdpi='high',transp=False):
     """
     Plot any/all geocontour-created elements:
 
     - `boundary`
     - `mask`
     - `contour`
     - `contoursearch`
@@ -77,14 +77,17 @@
                 4-connected `mask` edge cells
             ``maskedge-8``
                 8-connected `mask` edge cells
             ``contour``
                 `contour` cells
             ``geocontour``
                 `geocontour` cells
+    undermask : bool, default=False
+        show/hide the mask cells independently of the `cells` input
+        [allows showing a mask underlay beneath selected contour cells]
     showcontour : bool, default=True
         show/hide the `contour` (if provided)
         [allows showing contour cells without line plot of `contour`]
     startcell : bool, default=True
         show/hide the startcell (`contour` or `contoursearch`, if
         provided)
     contourarrows : bool, default=True
@@ -104,14 +107,16 @@
     geocontourvectors : bool, default=True
         show/hide outward normal vectors on the `geocontour` (if
         provided)
     emptycellcolor : matplotlib_color, default='lightgray'
         color for unmasked cells
     fullcellcolor : matplotlib_color, default='sandybrown'
         color for masked cells
+    undermaskcolor : matplotlib_color, default='slategrey'
+        color for mask underlay cells
     boundarycolor : matplotlib_color, default='tab:blue'
         color for `boundary` (if provided)
     contourcolor : matplotlib_color, default='olivedrab'
         color for `contour` (if provided)
     contoursearchcolor : matplotlib_color, default='firebrickred'
         color for `contoursearch` (if provided)
     geocontourcolor : matplotlib_color, default='olivedrab'
@@ -365,20 +370,27 @@
     elif cells=='geocontour':
          latinds=latitudes.argsort()[np.searchsorted(latitudes,geocontour[:,0,0],sorter=latitudes.argsort())]
          loninds=np.searchsorted(longitudes,geocontour[:,1,0])
          pltmask=np.full((len(latitudes),len(longitudes)),0)
          pltmask[latinds,loninds]=1
     else:
         sys.exit('ERROR - cells=\''+cells+'\' is not a valid selection, valid selections are \'none\'/\'mask\'/\'maskedge-8\'/\'maskedge-4\'/\'contour\'/\'geocontour\'')
+    if undermask==True:
+        if mask is not None:
+            pltmask+=mask
+        else:
+            sys.exit('ERROR - Can not set undermask=True if no mask input provided')
+    else:
+        pltmask+=pltmask
     if latdir=='inc':
         org='lower'
     elif latdir=='dec':
         org='upper'
     ext=[gridlonmin,gridlonmax,gridlatmin,gridlatmax]
-    cmp=mplc.ListedColormap([emptycellcolor,fullcellcolor])
+    cmp=mplc.ListedColormap([emptycellcolor,undermaskcolor,fullcellcolor])
     plt.ioff()
     yminor=np.arange(ylimmin,ylimmax+latspc,latspc)
     xminor=np.arange(xlimmin,xlimmax+lonspc,lonspc)
     ymajor=(yminor[:-1]+latspc/2)[::np.ceil(len(yminor)/7).astype('int')]
     xmajor=(xminor[:-1]+lonspc/2)[::np.ceil(len(xminor)/7).astype('int')]
     fig=plt.figure()
     if transp==True:
@@ -401,15 +413,15 @@
     if title is not None:
         ax.set_title(title)
     if labs==True:
         ax.set_xlabel('Longitude (deg)')
         ax.set_ylabel('Latitude (deg)')
     ax.set_ylim((ylimmin,ylimmax))
     ax.set_xlim((xlimmin,xlimmax)) 
-    ax.imshow(pltmask,aspect='equal',interpolation='none',vmin=0,vmax=1,extent=ext,origin=org,cmap=cmp,zorder=-1)
+    ax.imshow(pltmask,aspect='equal',interpolation='none',vmin=0,vmax=2,extent=ext,origin=org,cmap=cmp,zorder=-1)
     pdw=ds.plotdatasize(ax,axis='xy',mult=(latspc+lonspc)/2,plottype='line')
     pds=ds.plotdatasize(ax,axis='xy',mult=(latspc+lonspc)/2,plottype='scatter')
     if features is None:
         ax.set_yticks(ymajor)
         ax.set_xticks(xmajor)
         ax.set_yticks(yminor,minor=True)
         ax.set_xticks(xminor,minor=True)
```

### Comparing `geocontour-1.3.0/geocontour/tests/__init__.py` & `geocontour-1.3.1/geocontour/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/geocontour/tests/timing.py` & `geocontour-1.3.1/geocontour/tests/timing.py`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/geocontour.egg-info/PKG-INFO` & `geocontour-1.3.1/geocontour.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocontour
-Version: 1.3.0
+Version: 1.3.1
 Summary: Utilities for masking, contour tracing, and geocontour construction with gridded geographic data
 Home-page: https://github.com/benkrichman/geocontour
 Author: Benjamin Krichman
 Author-email: benkrichman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -48,28 +48,28 @@
 
 Find the full documentation hosted [here](https://geocontour.readthedocs.io/en/latest/index.html).
 
 ## Citation
 
 If geocontour played a significant role in your work and you would like to cite it, the following is suggested (APA):
 
-Krichman, B. (2023). *geocontour* (Version 1.3.0) [Computer Software]. https://doi.org/10.5281/zenodo.7402714
+Krichman, B. (2023). *geocontour* (Version 1.3.1) [Computer Software]. https://doi.org/10.5281/zenodo.7402714
 
 Bibtex:
 
 ```latex
 @software{geocontour,
 author={Krichman, Benjamin},
 doi={10.5281/zenodo.7402714},
 license={MIT},
 month={5},
 year={2023},
 title={{geocontour}},
 url={https://github.com/benkrichman/geocontour},
-version={1.3.0},
+version={1.3.1},
 note = {Computer Software}
 }
 ```
 
 ## Features
 
 ### Masks
```

### Comparing `geocontour-1.3.0/geocontour.egg-info/SOURCES.txt` & `geocontour-1.3.1/geocontour.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 geocontour/output.py
 geocontour.egg-info/PKG-INFO
 geocontour.egg-info/SOURCES.txt
 geocontour.egg-info/dependency_links.txt
 geocontour.egg-info/requires.txt
 geocontour.egg-info/top_level.txt
 geocontour/data/MissBasin_boundary.npz
+geocontour/data/box_boundary.npz
 geocontour/data/generic_boundary.npz
+geocontour/data/test_case_boundary.npz
 geocontour/examples/__init__.py
 geocontour/tests/__init__.py
 geocontour/tests/timing.py
 images/example_large_boundary+mask.png
 images/example_large_contour.png
 images/example_large_contoursearch.png
 images/example_large_geocontour+bordfeat.png
```

### Comparing `geocontour-1.3.0/images/example_large_boundary+mask.png` & `geocontour-1.3.1/images/example_large_boundary+mask.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/images/example_large_contour.png` & `geocontour-1.3.1/images/example_large_contour.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/images/example_large_contoursearch.png` & `geocontour-1.3.1/images/example_large_contoursearch.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/images/example_large_geocontour+bordfeat.png` & `geocontour-1.3.1/images/example_large_geocontour+bordfeat.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/images/example_large_geocontour+natfeat.png` & `geocontour-1.3.1/images/example_large_geocontour+natfeat.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/images/example_large_geocontour.png` & `geocontour-1.3.1/images/example_large_geocontour.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/images/example_small_boundary+mask.png` & `geocontour-1.3.1/images/example_small_boundary+mask.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/images/example_small_contour.png` & `geocontour-1.3.1/images/example_small_contour.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/images/example_small_contoursearch.png` & `geocontour-1.3.1/images/example_small_contoursearch.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/images/example_small_geocontour.png` & `geocontour-1.3.1/images/example_small_geocontour.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/images/example_small_geocontour_simp.png` & `geocontour-1.3.1/images/example_small_geocontour_simp.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/images/icon_geocontour.png` & `geocontour-1.3.1/images/icon_geocontour.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.3.0/setup.py` & `geocontour-1.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools as st
 
 with open('README.md','r') as ldf:
     longdesc=ldf.read()
 
 st.setup(
     name='geocontour',
-    version='1.3.0',
+    version='1.3.1',
     license='MIT',
     url='https://github.com/benkrichman/geocontour',
     description='Utilities for masking, contour tracing, and geocontour construction with gridded geographic data',
     long_description=longdesc,
     long_description_content_type="text/markdown",
     author='Benjamin Krichman',
     author_email='benkrichman@gmail.com',
```

